# Comparing `tmp/molgraph-0.5.3.tar.gz` & `tmp/molgraph-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.3.tar", last modified: Mon Jul 17 08:25:19 2023, max compression
+gzip compressed data, was "molgraph-0.5.4.tar", last modified: Mon Jul 17 13:47:02 2023, max compression
```

## Comparing `molgraph-0.5.3.tar` & `molgraph-0.5.4.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.3/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-17 08:25:19.510153 molgraph-0.5.3/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5949 2023-07-11 18:19:33.000000 molgraph-0.5.3/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.502153 molgraph-0.5.3/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.3/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 07:56:35.000000 molgraph-0.5.3/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.3/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.3/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.3/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.3/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.3/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.3/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.3/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.3/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.3/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.3/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.3/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16276 2023-07-17 07:54:08.000000 molgraph-0.5.3/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.3/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.3/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.3/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.3/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.3/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.3/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.3/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.3/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.3/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.3/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.3/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.3/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.3/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.3/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 08:25:19.510153 molgraph-0.5.3/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.3/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.4/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6765 2023-07-17 13:47:02.666568 molgraph-0.5.4/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6045 2023-07-17 13:46:46.000000 molgraph-0.5.4/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.4/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.4/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.4/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.4/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.4/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.4/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.4/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.4/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.4/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.4/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.4/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.4/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.4/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16276 2023-07-17 07:54:08.000000 molgraph-0.5.4/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.4/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.4/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.4/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11154 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11974 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20628 2023-07-17 13:46:46.000000 molgraph-0.5.4/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.4/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.4/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.662568 molgraph-0.5.4/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.4/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.4/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.4/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.4/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.4/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.4/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.4/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.4/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.666568 molgraph-0.5.4/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.4/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.4/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.4/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 13:47:02.658568 molgraph-0.5.4/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6765 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 13:47:02.000000 molgraph-0.5.4/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 13:47:02.666568 molgraph-0.5.4/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.4/setup.py
```

### Comparing `molgraph-0.5.3/LICENSE` & `molgraph-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/PKG-INFO` & `molgraph-0.5.4/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.3
+Version: 0.5.4
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
@@ -29,18 +29,18 @@
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
 - **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
     - A composite tensor holding graph data.
     - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-    - Can conveniently go between both states (merge() and separate())
+    - Can conveniently go between both states (merge(), separate())
     - Can propagate node information (features) based on edges (propagate())
     - Can add, update and remove graph data (update(), remove())
-    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+    - Has an associated GraphTensorSpec which makes it compatible with Keras and TensorFlow API.
         - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
@@ -55,31 +55,35 @@
     - **Message-passing**
         - MPNNConv ([MPNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/mpnn_conv.py))
         - EdgeConv ([EdgeConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/edge_conv.py))
     - **Distance-geometric**
         - DTNNConv ([DTNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/dtnn_conv.py))
         - GCFConv ([GCFConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/gcf_conv.py))
     - **Pre- and post-processing**
-        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See `readout/`, `preprocessing/`, `postprocessing/`, `positional_encoding/`.
+        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See [readout/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/readout), [preprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/preprocessing), [postprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/postprocessing), [positional_encoding/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/positional_encoding).
 - **Models**
-    - Although model building is easy with MolGraph, there are some built-in GNN models:
+    - Although model building is easy with MolGraph, there are some built-in GNN [models](https://github.com/akensert/molgraph/tree/main/molgraph/models):
         - **DGIN**
         - **DMPNN**
         - **MPNN**
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
-**Important notes**
-- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+## Requirements/dependencies
+- **Python** (version >= 3.6 recommended)
+    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **RDKit** (version >= 2022.3.3 recommended)
+    - **NumPy** (version >= 1.21.2 recommended)
+    - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -115,15 +119,15 @@
 bond_encoder = chemistry.Featurizer([
     chemistry.features.BondType(),
     # ...
 ])
 
 encoder = chemistry.MolecularGraphEncoder(atom_encoder, bond_encoder)
 
-# Obtain features and associated labels
+# Obtain graphs and associated labels
 x_train = encoder(qm7['train']['x'])
 y_train = qm7['train']['y']
 
 x_test = encoder(qm7['test']['x'])
 y_test = qm7['test']['y']
 
 # Build model via Keras API
@@ -143,18 +147,7 @@
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
 maps = gam_model(x_train)
 ```
-
-## Requirements/dependencies
-- **Python** (version >= 3.6 recommended)
-- **TensorFlow** (version >= 2.7.0 recommended)
-- **RDKit** (version >= 2022.3.3 recommended)
-- **NumPy** (version >= 1.21.2 recommended)
-- **Pandas** (version >= 1.0.3 recommended)
-
-## Tested with
-- **Ubuntu 20.04 - Python 3.8.10**
-- **MacOS Monterey (12.3.1) - Python 3.10.3**
```

### Comparing `molgraph-0.5.3/README.md` & `molgraph-0.5.4/molgraph.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: molgraph
+Version: 0.5.4
+Summary: Implementations of graph neural networks for molecular machine learning
+Home-page: https://github.com/akensert/molgraph
+Author: Alexander Kensert
+Author-email: alexander.kensert@gmail.com
+License: MIT
+Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
+Classifier: Programming Language :: Python :: 3
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # MolGraph: Graph Neural Networks for Molecular Machine Learning
 
 *This is an early release; things are still being updated, added and experimented with. Hence, API compatibility may break in the future.*
 
 *Any feedback is welcomed!*
 
 ## Manuscript
@@ -11,18 +29,18 @@
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
 - **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
     - A composite tensor holding graph data.
     - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-    - Can conveniently go between both states (merge() and separate())
+    - Can conveniently go between both states (merge(), separate())
     - Can propagate node information (features) based on edges (propagate())
     - Can add, update and remove graph data (update(), remove())
-    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+    - Has an associated GraphTensorSpec which makes it compatible with Keras and TensorFlow API.
         - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
@@ -37,31 +55,35 @@
     - **Message-passing**
         - MPNNConv ([MPNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/mpnn_conv.py))
         - EdgeConv ([EdgeConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/edge_conv.py))
     - **Distance-geometric**
         - DTNNConv ([DTNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/dtnn_conv.py))
         - GCFConv ([GCFConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/gcf_conv.py))
     - **Pre- and post-processing**
-        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See `readout/`, `preprocessing/`, `postprocessing/`, `positional_encoding/`.
+        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See [readout/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/readout), [preprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/preprocessing), [postprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/postprocessing), [positional_encoding/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/positional_encoding).
 - **Models**
-    - Although model building is easy with MolGraph, there are some built-in GNN models:
+    - Although model building is easy with MolGraph, there are some built-in GNN [models](https://github.com/akensert/molgraph/tree/main/molgraph/models):
         - **DGIN**
         - **DMPNN**
         - **MPNN**
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
-**Important notes**
-- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+## Requirements/dependencies
+- **Python** (version >= 3.6 recommended)
+    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **RDKit** (version >= 2022.3.3 recommended)
+    - **NumPy** (version >= 1.21.2 recommended)
+    - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -97,15 +119,15 @@
 bond_encoder = chemistry.Featurizer([
     chemistry.features.BondType(),
     # ...
 ])
 
 encoder = chemistry.MolecularGraphEncoder(atom_encoder, bond_encoder)
 
-# Obtain features and associated labels
+# Obtain graphs and associated labels
 x_train = encoder(qm7['train']['x'])
 y_train = qm7['train']['y']
 
 x_test = encoder(qm7['test']['x'])
 y_test = qm7['test']['y']
 
 # Build model via Keras API
@@ -125,18 +147,7 @@
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
 maps = gam_model(x_train)
 ```
-
-## Requirements/dependencies
-- **Python** (version >= 3.6 recommended)
-- **TensorFlow** (version >= 2.7.0 recommended)
-- **RDKit** (version >= 2022.3.3 recommended)
-- **NumPy** (version >= 1.21.2 recommended)
-- **Pandas** (version >= 1.0.3 recommended)
-
-## Tested with
-- **Ubuntu 20.04 - Python 3.8.10**
-- **MacOS Monterey (12.3.1) - Python 3.10.3**
```

### Comparing `molgraph-0.5.3/molgraph/_filter_warnings.py` & `molgraph-0.5.4/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/applications/graph_transformer.py` & `molgraph-0.5.4/molgraph/applications/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/__init__.py` & `molgraph-0.5.4/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.4/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.4/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.4/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.4/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.4/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.4/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/encoders.py` & `molgraph-0.5.4/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/features.py` & `molgraph-0.5.4/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.4/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/ops.py` & `molgraph-0.5.4/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/chemistry/vis.py` & `molgraph-0.5.4/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/__init__.py` & `molgraph-0.5.4/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.4/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.4/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.4/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.4/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.4/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.4/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.4/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.4/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/gnn_layer.py` & `molgraph-0.5.4/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/gnn_ops.py` & `molgraph-0.5.4/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.4/molgraph/layers/message_passing/edge_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.4/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.4/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.4/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.4/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.4/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/center_scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 
+import numpy as np
+
 from typing import Optional
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 try:
     PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
 except AttributeError:
```

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 from keras import initializers
 
+import numpy as np
+
 from typing import Tuple
 from typing import Optional
 from typing import Tuple
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 try:
```

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.4/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import tensorflow as tf
 from tensorflow import keras
 from keras import layers
 from keras import initializers
 
+import numpy as np
+
 from typing import Optional
 from typing import Union
 
 from molgraph.tensors.graph_tensor import GraphTensor
 
 try:
     PreprocessingLayer = layers.experimental.preprocessing.PreprocessingLayer
```

### Comparing `molgraph-0.5.3/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.4/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.4/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.4/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.4/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.4/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/losses/link_losses.py` & `molgraph-0.5.4/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/losses/masked_losses.py` & `molgraph-0.5.4/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.4/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.4/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/__init__.py` & `molgraph-0.5.4/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/dgin.py` & `molgraph-0.5.4/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/dmpnn.py` & `molgraph-0.5.4/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.4/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.4/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/mpnn.py` & `molgraph-0.5.4/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.4/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.4/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.4/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.4/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.4/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.4/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: molgraph
-Version: 0.5.3
-Summary: Implementations of graph neural networks for molecular machine learning
-Home-page: https://github.com/akensert/molgraph
-Author: Alexander Kensert
-Author-email: alexander.kensert@gmail.com
-License: MIT
-Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
-Classifier: Programming Language :: Python :: 3
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # MolGraph: Graph Neural Networks for Molecular Machine Learning
 
 *This is an early release; things are still being updated, added and experimented with. Hence, API compatibility may break in the future.*
 
 *Any feedback is welcomed!*
 
 ## Manuscript
@@ -29,18 +11,18 @@
 See [readthedocs](https://molgraph.readthedocs.io/en/latest/)
 
 ## Implementations
 
 - **Graph tensor** ([GraphTensor](http://github.com/akensert/molgraph/tree/main/molgraph/tensors/graph_tensor.py))
     - A composite tensor holding graph data.
     - Has a ragged (multiple graphs) and a non-ragged state (single disjoint graph)
-    - Can conveniently go between both states (merge() and separate())
+    - Can conveniently go between both states (merge(), separate())
     - Can propagate node information (features) based on edges (propagate())
     - Can add, update and remove graph data (update(), remove())
-    - Has an associated GraphTensorSpec which it makes it compatible with Keras and TensorFlow API.
+    - Has an associated GraphTensorSpec which makes it compatible with Keras and TensorFlow API.
         - This includes keras.Sequential, keras.Functional, tf.data.Dataset, and tf.saved_model API.
 - **Layers**
     
     - **Convolutional**
         - GCNConv ([GCNConv](http://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcn_conv.py))
         - GINConv ([GINConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gin_conv.py))
         - GCNIIConv ([GCNIIConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/convolutional/gcnii_conv.py))
@@ -55,31 +37,35 @@
     - **Message-passing**
         - MPNNConv ([MPNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/mpnn_conv.py))
         - EdgeConv ([EdgeConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/message_passing/edge_conv.py))
     - **Distance-geometric**
         - DTNNConv ([DTNNConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/dtnn_conv.py))
         - GCFConv ([GCFConv](https://github.com/akensert/molgraph/tree/main/molgraph/layers/geometric/gcf_conv.py))
     - **Pre- and post-processing**
-        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See `readout/`, `preprocessing/`, `postprocessing/`, `positional_encoding/`.
+        - In addition to the aforementioned GNN layers, there are also several other layers which improves model-building. See [readout/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/readout), [preprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/preprocessing), [postprocessing/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/postprocessing), [positional_encoding/](https://github.com/akensert/molgraph/tree/main/molgraph/layers/positional_encoding).
 - **Models**
-    - Although model building is easy with MolGraph, there are some built-in GNN models:
+    - Although model building is easy with MolGraph, there are some built-in GNN [models](https://github.com/akensert/molgraph/tree/main/molgraph/models):
         - **DGIN**
         - **DMPNN**
         - **MPNN**
     - And models for improved interpretability of GNNs:
         - **SaliencyMapping**
         - **IntegratedSaliencyMapping**
         - **SmoothGradSaliencyMapping**
         - **GradientActivationMapping** (Recommended)
 
 ## Changelog
 For a detailed list of changes, see the [CHANGELOG.md](https://github.com/akensert/molgraph/blob/main/CHANGELOG.md).
 
-**Important notes**
-- Since version **0.5.0**, default normalization for the GNN layers is layer normalization. This significantly improved the performance on some of the MoleculeNet datasets.
+## Requirements/dependencies
+- **Python** (version >= 3.6 recommended)
+    - **TensorFlow** (version >= 2.7.0 recommended)
+    - **RDKit** (version >= 2022.3.3 recommended)
+    - **NumPy** (version >= 1.21.2 recommended)
+    - **Pandas** (version >= 1.0.3 recommended)
 
 ## Installation
 
 Install via **pip**:
 
 <pre>
 pip install molgraph
@@ -115,15 +101,15 @@
 bond_encoder = chemistry.Featurizer([
     chemistry.features.BondType(),
     # ...
 ])
 
 encoder = chemistry.MolecularGraphEncoder(atom_encoder, bond_encoder)
 
-# Obtain features and associated labels
+# Obtain graphs and associated labels
 x_train = encoder(qm7['train']['x'])
 y_train = qm7['train']['y']
 
 x_test = encoder(qm7['test']['x'])
 y_test = qm7['test']['y']
 
 # Build model via Keras API
@@ -143,18 +129,7 @@
 
 # Compute gradient activation maps
 gam_model = models.GradientActivationMapping(
     model=gnn_model, layer_names=['gat_conv_1', 'gat_conv_2'])
 
 maps = gam_model(x_train)
 ```
-
-## Requirements/dependencies
-- **Python** (version >= 3.6 recommended)
-- **TensorFlow** (version >= 2.7.0 recommended)
-- **RDKit** (version >= 2022.3.3 recommended)
-- **NumPy** (version >= 1.21.2 recommended)
-- **Pandas** (version >= 1.0.3 recommended)
-
-## Tested with
-- **Ubuntu 20.04 - Python 3.8.10**
-- **MacOS Monterey (12.3.1) - Python 3.10.3**
```

### Comparing `molgraph-0.5.3/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.4/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.3/setup.py` & `molgraph-0.5.4/setup.py`

 * *Files identical despite different names*

