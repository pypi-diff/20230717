# Comparing `tmp/molgraph-0.5.2.tar.gz` & `tmp/molgraph-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molgraph-0.5.2.tar", last modified: Tue Jul 11 18:19:52 2023, max compression
+gzip compressed data, was "molgraph-0.5.3.tar", last modified: Mon Jul 17 08:25:19 2023, max compression
```

## Comparing `molgraph-0.5.2.tar` & `molgraph-0.5.3.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.2/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-11 18:19:52.431043 molgraph-0.5.2/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     5949 2023-07-11 18:19:33.000000 molgraph-0.5.2/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/
--rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.2/molgraph/_filter_warnings.py
--rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/_version.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/applications/
--rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.2/molgraph/applications/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.2/molgraph/applications/graph_transformer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph/chemistry/
--rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/chemistry/benchmark/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/configs.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/datasets.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/splitters.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.2/molgraph/chemistry/benchmark/tf_records.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.2/molgraph/chemistry/conformer_generator.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.2/molgraph/chemistry/conformer_utils.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/chemistry/features.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.2/molgraph/chemistry/molecular_encoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.2/molgraph/chemistry/ops.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.2/molgraph/chemistry/vis.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/layers/__init__.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/attentional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.2/molgraph/layers/attentional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/attentive_fp_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gat_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gated_gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gatv2_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gmm_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/attentional/gt_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/convolutional/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.2/molgraph/layers/convolutional/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gcn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gcnii_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/gin_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/convolutional/graph_sage_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/geometric/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.2/molgraph/layers/geometric/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/dtnn_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/gcf_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/geometric/radial_basis.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/gnn_layer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/layers/gnn_ops.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/message_passing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.2/molgraph/layers/message_passing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    16271 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/message_passing/edge_conv.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/message_passing/mpnn_conv.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/positional_encoding/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.2/molgraph/layers/positional_encoding/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/positional_encoding/laplacian.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/postprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.2/molgraph/layers/postprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/dot_product_incident.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/extract_field.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/postprocessing/gather_incident.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/preprocessing/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.2/molgraph/layers/preprocessing/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/center_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/embedding_lookup.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/masking.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/min_max_scaling.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/projection.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/preprocessing/standard_scaling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/layers/readout/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.2/molgraph/layers/readout/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/attentive_fp_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/node_readout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/segment_pool.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/set_gather.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/layers/readout/transformer_encoder.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/losses/
--rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.2/molgraph/losses/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/losses/link_losses.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/losses/masked_losses.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.427043 molgraph-0.5.2/molgraph/metrics/
--rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.2/molgraph/metrics/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/metrics/masked_metrics.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/metrics/mean_relative_error.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/
--rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.2/molgraph/models/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/models/dgin.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.2/molgraph/models/dmpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/interpretability/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/activation_maps.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.2/molgraph/models/interpretability/saliency.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/models/mpnn.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/models/pretraining/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.2/molgraph/models/pretraining/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.2/molgraph/models/pretraining/autoencoders.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.2/molgraph/models/pretraining/masked_modeling.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.431043 molgraph-0.5.2/molgraph/tensors/
--rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.2/molgraph/tensors/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.2/molgraph/tensors/_graph_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/tensors/graph_keras_tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.2/molgraph/tensors/graph_tensor.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-11 18:19:52.423043 molgraph-0.5.2/molgraph.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-11 18:19:52.000000 molgraph-0.5.2/molgraph.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-11 18:19:52.431043 molgraph-0.5.2/setup.cfg
--rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.2/setup.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2022-05-10 17:47:45.000000 molgraph-0.5.3/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-17 08:25:19.510153 molgraph-0.5.3/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5949 2023-07-11 18:19:33.000000 molgraph-0.5.3/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.502153 molgraph-0.5.3/molgraph/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      351 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1154 2023-07-10 07:53:56.000000 molgraph-0.5.3/molgraph/_filter_warnings.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)       22 2023-07-17 07:56:35.000000 molgraph-0.5.3/molgraph/_version.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/applications/
+-rw-rw-r--   0 alex      (1000) alex      (1000)       68 2023-07-04 19:57:47.000000 molgraph-0.5.3/molgraph/applications/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7735 2023-07-11 16:19:06.000000 molgraph-0.5.3/molgraph/applications/graph_transformer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/chemistry/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      754 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/chemistry/benchmark/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-29 19:00:10.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    36677 2022-08-02 17:30:01.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/configs.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13653 2022-09-20 11:35:03.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/datasets.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     8971 2022-09-02 12:17:48.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/splitters.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10276 2023-07-05 11:29:34.000000 molgraph-0.5.3/molgraph/chemistry/benchmark/tf_records.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2718 2022-09-02 12:17:48.000000 molgraph-0.5.3/molgraph/chemistry/conformer_generator.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10471 2022-08-03 19:47:51.000000 molgraph-0.5.3/molgraph/chemistry/conformer_utils.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14301 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13964 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/chemistry/features.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    21484 2023-07-05 11:29:41.000000 molgraph-0.5.3/molgraph/chemistry/molecular_encoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1840 2022-09-02 12:44:02.000000 molgraph-0.5.3/molgraph/chemistry/ops.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2760 2023-04-06 16:32:34.000000 molgraph-0.5.3/molgraph/chemistry/vis.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3937 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/layers/__init__.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/attentional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:18.000000 molgraph-0.5.3/molgraph/layers/attentional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    12880 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/attentive_fp_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11688 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gat_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9876 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gated_gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11816 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gatv2_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10799 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gmm_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    17096 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/attentional/gt_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/convolutional/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:16.000000 molgraph-0.5.3/molgraph/layers/convolutional/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10195 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gcn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10145 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gcnii_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11217 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/gin_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10508 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/convolutional/graph_sage_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/geometric/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-06-10 12:47:57.000000 molgraph-0.5.3/molgraph/layers/geometric/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9934 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/dtnn_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10824 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/gcf_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1586 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/geometric/radial_basis.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    25885 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/gnn_layer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7023 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/layers/gnn_ops.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/message_passing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-23 17:04:39.000000 molgraph-0.5.3/molgraph/layers/message_passing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    16276 2023-07-17 07:54:08.000000 molgraph-0.5.3/molgraph/layers/message_passing/edge_conv.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14447 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/message_passing/mpnn_conv.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/positional_encoding/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:08.000000 molgraph-0.5.3/molgraph/layers/positional_encoding/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    10725 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/positional_encoding/laplacian.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/postprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:18:09.000000 molgraph-0.5.3/molgraph/layers/postprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3408 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/dot_product_incident.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2014 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/extract_field.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2984 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/postprocessing/gather_incident.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph/layers/preprocessing/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:11.000000 molgraph-0.5.3/molgraph/layers/preprocessing/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11134 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/center_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4559 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9716 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/embedding_lookup.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4237 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/masking.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11954 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/min_max_scaling.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6668 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/projection.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20608 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/preprocessing/standard_scaling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/layers/readout/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2022-05-10 18:07:24.000000 molgraph-0.5.3/molgraph/layers/readout/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6399 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/attentive_fp_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4640 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/node_readout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3286 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/segment_pool.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6241 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/set_gather.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5348 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/layers/readout/transformer_encoder.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/losses/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      456 2022-08-09 16:26:08.000000 molgraph-0.5.3/molgraph/losses/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2428 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/losses/link_losses.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     5375 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/losses/masked_losses.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/metrics/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      342 2022-08-09 16:18:46.000000 molgraph-0.5.3/molgraph/metrics/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2075 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/metrics/masked_metrics.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      519 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/metrics/mean_relative_error.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      971 2023-07-11 11:46:21.000000 molgraph-0.5.3/molgraph/models/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6940 2023-07-11 18:19:33.000000 molgraph-0.5.3/molgraph/models/dgin.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     7054 2023-07-11 18:19:33.000000 molgraph-0.5.3/molgraph/models/dmpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/interpretability/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3405 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/activation_maps.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11059 2023-07-07 12:40:08.000000 molgraph-0.5.3/molgraph/models/interpretability/saliency.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6858 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/models/mpnn.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/models/pretraining/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-06-14 11:03:03.000000 molgraph-0.5.3/molgraph/models/pretraining/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    23576 2023-07-10 07:10:13.000000 molgraph-0.5.3/molgraph/models/pretraining/autoencoders.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13013 2023-07-05 11:40:27.000000 molgraph-0.5.3/molgraph/models/pretraining/masked_modeling.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.510153 molgraph-0.5.3/molgraph/tensors/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      184 2023-07-05 11:17:52.000000 molgraph-0.5.3/molgraph/tensors/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22917 2022-08-05 18:22:59.000000 molgraph-0.5.3/molgraph/tensors/_graph_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1991 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/tensors/graph_keras_tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    52163 2023-07-10 07:57:12.000000 molgraph-0.5.3/molgraph/tensors/graph_tensor.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-07-17 08:25:19.506153 molgraph-0.5.3/molgraph.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6669 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3308 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       78 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        9 2023-07-17 08:25:19.000000 molgraph-0.5.3/molgraph.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-07-17 08:25:19.510153 molgraph-0.5.3/setup.cfg
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1438 2023-07-10 07:57:12.000000 molgraph-0.5.3/setup.py
```

### Comparing `molgraph-0.5.2/LICENSE` & `molgraph-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/PKG-INFO` & `molgraph-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.2
+Version: 0.5.3
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.2/README.md` & `molgraph-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/_filter_warnings.py` & `molgraph-0.5.3/molgraph/_filter_warnings.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/applications/graph_transformer.py` & `molgraph-0.5.3/molgraph/applications/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/__init__.py` & `molgraph-0.5.3/molgraph/chemistry/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/benchmark/configs.py` & `molgraph-0.5.3/molgraph/chemistry/benchmark/configs.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/benchmark/datasets.py` & `molgraph-0.5.3/molgraph/chemistry/benchmark/datasets.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/benchmark/splitters.py` & `molgraph-0.5.3/molgraph/chemistry/benchmark/splitters.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/benchmark/tf_records.py` & `molgraph-0.5.3/molgraph/chemistry/benchmark/tf_records.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/conformer_generator.py` & `molgraph-0.5.3/molgraph/chemistry/conformer_generator.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/conformer_utils.py` & `molgraph-0.5.3/molgraph/chemistry/conformer_utils.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/encoders.py` & `molgraph-0.5.3/molgraph/chemistry/encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/features.py` & `molgraph-0.5.3/molgraph/chemistry/features.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/molecular_encoders.py` & `molgraph-0.5.3/molgraph/chemistry/molecular_encoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/ops.py` & `molgraph-0.5.3/molgraph/chemistry/ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/chemistry/vis.py` & `molgraph-0.5.3/molgraph/chemistry/vis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/__init__.py` & `molgraph-0.5.3/molgraph/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/attentive_fp_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/attentive_fp_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/gat_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/gat_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/gated_gcn_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/gated_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/gatv2_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/gatv2_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/gmm_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/gmm_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/attentional/gt_conv.py` & `molgraph-0.5.3/molgraph/layers/attentional/gt_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/convolutional/gcn_conv.py` & `molgraph-0.5.3/molgraph/layers/convolutional/gcn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/convolutional/gcnii_conv.py` & `molgraph-0.5.3/molgraph/layers/convolutional/gcnii_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/convolutional/gin_conv.py` & `molgraph-0.5.3/molgraph/layers/convolutional/gin_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/convolutional/graph_sage_conv.py` & `molgraph-0.5.3/molgraph/layers/convolutional/graph_sage_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/geometric/dtnn_conv.py` & `molgraph-0.5.3/molgraph/layers/geometric/dtnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/geometric/gcf_conv.py` & `molgraph-0.5.3/molgraph/layers/geometric/gcf_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/geometric/radial_basis.py` & `molgraph-0.5.3/molgraph/layers/geometric/radial_basis.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/gnn_layer.py` & `molgraph-0.5.3/molgraph/layers/gnn_layer.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/gnn_ops.py` & `molgraph-0.5.3/molgraph/layers/gnn_ops.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/message_passing/edge_conv.py` & `molgraph-0.5.3/molgraph/layers/message_passing/edge_conv.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,14 +326,15 @@
             kernel_regularizer=self.kernel_regularizer,
             bias_regularizer=self.bias_regularizer,
             recurrent_regularizer=self.recurrent_regularizer,
             kernel_constraint=self.kernel_constraint,
             bias_constraint=self.bias_constraint,
             recurrent_constraint=self.recurrent_constraint)
     
+    
 def edge_update_step(
     edge_feature: tf.Tensor, 
     edge_feature_prev: tf.Tensor,
     update_projection: Union[
         keras.layers.Dense, keras.layers.GRUCell, keras.layers.LSTMCell],
 ) -> tf.Tensor:
     if isinstance(update_projection, keras.layers.Dense):
@@ -354,16 +355,16 @@
     message = tf.math.unsorted_segment_sum(edge_feature, edge_dst, num_nodes)
     message = tf.gather(message, edge_src)
     message -= _get_reverse_edge_features(edge_feature, edge_src, edge_dst)
     return message
 
 def _get_reverse_edge_features(edge_feature, edge_src, edge_dst):
     edge_exclude = tf.logical_and(
-        edge_src[:, None] == edge_src,
-        edge_dst[:, None] == edge_dst
+        edge_src[:, None] == edge_dst,
+        edge_dst[:, None] == edge_src
     )
     edge_forward, edge_reverse = tf.split(tf.where(edge_exclude), 2, axis=-1)
     return tf.tensor_scatter_nd_add(
         tf.zeros_like(edge_feature), 
         tf.expand_dims(edge_forward, -1), 
         tf.gather(edge_feature, edge_reverse)
     )
```

### Comparing `molgraph-0.5.2/molgraph/layers/message_passing/mpnn_conv.py` & `molgraph-0.5.3/molgraph/layers/message_passing/mpnn_conv.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/positional_encoding/laplacian.py` & `molgraph-0.5.3/molgraph/layers/positional_encoding/laplacian.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/postprocessing/dot_product_incident.py` & `molgraph-0.5.3/molgraph/layers/postprocessing/dot_product_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/postprocessing/extract_field.py` & `molgraph-0.5.3/molgraph/layers/postprocessing/extract_field.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/postprocessing/gather_incident.py` & `molgraph-0.5.3/molgraph/layers/postprocessing/gather_incident.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/center_scaling.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/center_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/dropout.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/dropout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/embedding_lookup.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/embedding_lookup.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/masking.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/masking.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/min_max_scaling.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/min_max_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/projection.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/projection.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/preprocessing/standard_scaling.py` & `molgraph-0.5.3/molgraph/layers/preprocessing/standard_scaling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/readout/attentive_fp_readout.py` & `molgraph-0.5.3/molgraph/layers/readout/attentive_fp_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/readout/node_readout.py` & `molgraph-0.5.3/molgraph/layers/readout/node_readout.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/readout/segment_pool.py` & `molgraph-0.5.3/molgraph/layers/readout/segment_pool.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/readout/set_gather.py` & `molgraph-0.5.3/molgraph/layers/readout/set_gather.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/layers/readout/transformer_encoder.py` & `molgraph-0.5.3/molgraph/layers/readout/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/losses/link_losses.py` & `molgraph-0.5.3/molgraph/losses/link_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/losses/masked_losses.py` & `molgraph-0.5.3/molgraph/losses/masked_losses.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/metrics/masked_metrics.py` & `molgraph-0.5.3/molgraph/metrics/masked_metrics.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/metrics/mean_relative_error.py` & `molgraph-0.5.3/molgraph/metrics/mean_relative_error.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/__init__.py` & `molgraph-0.5.3/molgraph/models/__init__.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/dgin.py` & `molgraph-0.5.3/molgraph/models/dgin.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/dmpnn.py` & `molgraph-0.5.3/molgraph/models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/interpretability/activation_maps.py` & `molgraph-0.5.3/molgraph/models/interpretability/activation_maps.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/interpretability/saliency.py` & `molgraph-0.5.3/molgraph/models/interpretability/saliency.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/mpnn.py` & `molgraph-0.5.3/molgraph/models/mpnn.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/pretraining/autoencoders.py` & `molgraph-0.5.3/molgraph/models/pretraining/autoencoders.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/models/pretraining/masked_modeling.py` & `molgraph-0.5.3/molgraph/models/pretraining/masked_modeling.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/tensors/_graph_tensor.py` & `molgraph-0.5.3/molgraph/tensors/_graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/tensors/graph_keras_tensor.py` & `molgraph-0.5.3/molgraph/tensors/graph_keras_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph/tensors/graph_tensor.py` & `molgraph-0.5.3/molgraph/tensors/graph_tensor.py`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/molgraph.egg-info/PKG-INFO` & `molgraph-0.5.3/molgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: molgraph
-Version: 0.5.2
+Version: 0.5.3
 Summary: Implementations of graph neural networks for molecular machine learning
 Home-page: https://github.com/akensert/molgraph
 Author: Alexander Kensert
 Author-email: alexander.kensert@gmail.com
 License: MIT
 Keywords: graph-neural-networks,deep-learning,machine-learning,molecular-machine-learning,molecular-graphs,cheminformatics,bioinformatics
 Classifier: Programming Language :: Python :: 3
```

### Comparing `molgraph-0.5.2/molgraph.egg-info/SOURCES.txt` & `molgraph-0.5.3/molgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `molgraph-0.5.2/setup.py` & `molgraph-0.5.3/setup.py`

 * *Files identical despite different names*

