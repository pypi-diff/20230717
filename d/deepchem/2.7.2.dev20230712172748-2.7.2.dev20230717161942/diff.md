# Comparing `tmp/deepchem-2.7.2.dev20230712172748.tar.gz` & `tmp/deepchem-2.7.2.dev20230717161942.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepchem-2.7.2.dev20230712172748.tar", last modified: Wed Jul 12 17:27:48 2023, max compression
+gzip compressed data, was "deepchem-2.7.2.dev20230717161942.tar", last modified: Mon Jul 17 16:19:42 2023, max compression
```

## Comparing `deepchem-2.7.2.dev20230712172748.tar` & `deepchem-2.7.2.dev20230717161942.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.458189 deepchem-2.7.2.dev20230712172748/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 17:27:48.458189 deepchem-2.7.2.dev20230712172748/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.426189 deepchem-2.7.2.dev20230712172748/deepchem/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.430189 deepchem-2.7.2.dev20230712172748/deepchem/data/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/data/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/data/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/data/pytorch_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/data/supports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.430189 deepchem-2.7.2.dev20230712172748/deepchem/dock/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/dock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/dock/binding_pocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/dock/docking.py
--rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/dock/pose_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/dock/pose_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.430189 deepchem-2.7.2.dev20230712172748/deepchem/feat/
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/atomic_conformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/bert_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/binding_pocket_features.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.430189 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/contact_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/grid_featurizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/splif_fingerprints.py
--rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/dft_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/graph_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/graph_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/huggingface_featurizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.430189 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/cgcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/element_property_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/elemnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/lcnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/mol_graphs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.434189 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/atomic_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/circular_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/conformer_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/coulomb_matrices.py
--rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/grover_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mat_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/molgan_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mordred_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/raw_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/smiles_to_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/smiles_to_seq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/snap_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/reaction_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/roberta_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.434189 deepchem-2.7.2.dev20230712172748/deepchem/feat/sequence_featurizers/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/sequence_featurizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/smiles_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.434189 deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/grover_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/hf_vocab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/vocabulary_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.434189 deepchem-2.7.2.dev20230712172748/deepchem/hyper/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/hyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/hyper/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/hyper/gaussian_process.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/hyper/grid_search.py
--rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/hyper/random_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.434189 deepchem-2.7.2.dev20230712172748/deepchem/metalearning/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metalearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metalearning/maml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.438189 deepchem-2.7.2.dev20230712172748/deepchem/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metrics/genomic_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/metrics/score_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.438189 deepchem-2.7.2.dev20230712172748/deepchem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/IRV.py
--rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/atomic_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/chemnet_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/chemnet_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.438189 deepchem-2.7.2.dev20230712172748/deepchem/models/dft/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/dft/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/dft/dftxc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/dft/nnxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/dft/scf.py
--rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/fcnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/gan.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.438189 deepchem-2.7.2.dev20230712172748/deepchem/models/gbdt_models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/gbdt_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/gbdt_models/gbdt_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/graph_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.442189 deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/jax_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/pinns_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/keras_model.py
--rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.442189 deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/dc_lightning_dataset_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/dc_lightning_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/molgan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/normalizing_flows.py
--rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/progressive_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/robust_multitask.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/scscore.py
--rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/seqtoseq.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.442189 deepchem-2.7.2.dev20230712172748/deepchem/models/sklearn_models/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/sklearn_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/sklearn_models/sklearn_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/text_cnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.446189 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/attentivefp.py
--rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/cgcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/chemberta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/cnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/dmpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/ferminet.py
--rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gat.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gcn.py
--rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gnn3d.py
--rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/grover_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/hf_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/infograph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/kfac_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)   153539 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/lcnn.py
--rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/mat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/megnet.py
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/modular.py
--rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/mpnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/normalizing_flows_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/pagtn.py
--rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/pna_gnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/readout.py
--rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/torch_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/models/wandblogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.446189 deepchem-2.7.2.dev20230712172748/deepchem/molnet/
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/check_availability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/dnasim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.450189 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bace_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bace_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bbbc_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bbbp_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/cell_counting_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl25_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/clearance_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/clintox_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/delaney_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/factors_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/freesolv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hiv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hopv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kaggle_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kaggle_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kinase_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/lipo_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/load_dataset_template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.450189 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_bandgap.py
--rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_perovskite.py
--rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/molnet_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/muv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/nci_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/pcba_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/pdbbind_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/ppb_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm7_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm8_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm9_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sampl_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sider_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sweetlead_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/thermosol_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/tox21_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/toxcast_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uspto_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uv_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uv_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/zinc15_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/preset_hyper_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark_low_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.454189 deepchem-2.7.2.dev20230712172748/deepchem/rl/
--rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/a2c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.454189 deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/test_tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/tictactoe.py
--rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/rl/ppo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.454189 deepchem-2.7.2.dev20230712172748/deepchem/splits/
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/splits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/splits/splitters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/splits/task_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.454189 deepchem-2.7.2.dev20230712172748/deepchem/trans/
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/trans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/trans/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/trans/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.458189 deepchem-2.7.2.dev20230712172748/deepchem/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/conformers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/debug_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/sequence_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.458189 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_coordinate_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_dftutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_docking_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_electron_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_fake_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_fragment_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_generator_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_genomics_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_grover.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_hash_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_molecule_feature_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_noncovalent_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_pdbqt_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_pytorch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_rdkit_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_sequence_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_updated_scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_voxel_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/vina_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-12 17:27:31.000000 deepchem-2.7.2.dev20230712172748/deepchem/utils/voxel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-12 17:27:48.426189 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-12 17:27:48.000000 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-12 17:27:48.000000 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-12 17:27:48.000000 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-12 17:27:48.000000 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-12 17:27:48.000000 deepchem-2.7.2.dev20230712172748/deepchem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-12 17:27:48.458189 deepchem-2.7.2.dev20230712172748/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-12 17:27:32.000000 deepchem-2.7.2.dev20230712172748/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.481118 deepchem-2.7.2.dev20230717161942/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1047 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 16:19:42.481118 deepchem-2.7.2.dev20230717161942/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7124 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.449118 deepchem-2.7.2.dev20230717161942/deepchem/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.449118 deepchem-2.7.2.dev20230717161942/deepchem/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67994 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/data/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118009 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/data/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/data/pytorch_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12606 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/data/supports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.453118 deepchem-2.7.2.dev20230717161942/deepchem/dock/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/dock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/dock/binding_pocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/dock/docking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19576 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/dock/pose_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/dock/pose_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.457118 deepchem-2.7.2.dev20230717161942/deepchem/feat/
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/atomic_conformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19458 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/bert_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/binding_pocket_features.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.457118 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/contact_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27676 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/grid_featurizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20248 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11465 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/splif_fingerprints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11743 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/dft_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22111 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/graph_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38890 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/graph_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/huggingface_featurizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.457118 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/cgcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/element_property_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/elemnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28058 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/lcnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3823 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/sine_coulomb_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14808 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/mol_graphs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/atomic_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/circular_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9242 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/conformer_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/coulomb_matrices.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19123 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7507 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/grover_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mat_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7587 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9346 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/molgan_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mordred_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6359 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/raw_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9855 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/rdkit_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7280 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/smiles_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/smiles_to_seq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/snap_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3448 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/reaction_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/roberta_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/feat/sequence_featurizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/sequence_featurizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/smiles_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18726 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/grover_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/hf_vocab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/vocabulary_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/hyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/hyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/hyper/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17151 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/hyper/gaussian_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/hyper/grid_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12427 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/hyper/random_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/metalearning/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metalearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10539 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metalearning/maml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.461118 deepchem-2.7.2.dev20230717161942/deepchem/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7715 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metrics/genomic_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31620 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/metrics/score_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/IRV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4420 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13833 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/atomic_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/chemnet_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15504 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/chemnet_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/dft/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/dft/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9553 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/dft/dftxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14020 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/dft/nnxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/dft/scf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23457 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/fcnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24548 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/gan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/gbdt_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/gbdt_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/gbdt_models/gbdt_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57408 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/graph_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28179 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/jax_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/pinns_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56522 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/keras_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144759 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/dc_lightning_dataset_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/dc_lightning_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61903 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8256 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/molgan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/normalizing_flows.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26871 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13095 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/progressive_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17830 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/robust_multitask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/scscore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25969 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/seqtoseq.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.465118 deepchem-2.7.2.dev20230717161942/deepchem/models/sklearn_models/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/sklearn_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/sklearn_models/sklearn_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10552 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/text_cnn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.469118 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/attentivefp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14455 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/cgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/chemberta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9543 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31166 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/dmpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/ferminet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gcn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51159 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24969 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gnn3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38126 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38432 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/grover_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22942 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/hf_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30077 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/infograph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/kfac_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   162322 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18575 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/lcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17126 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/mat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/megnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/modular.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12074 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/mpnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4165 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/normalizing_flows_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12297 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/pagtn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23016 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/pna_gnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/readout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52726 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/torch_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/models/wandblogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.469118 deepchem-2.7.2.dev20230717161942/deepchem/molnet/
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/check_availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/dnasim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.473118 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bace_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14202 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bace_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5785 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bbbc_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bbbp_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/cell_counting_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl25_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10252 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/clearance_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4245 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/clintox_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/delaney_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6957 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/factors_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/freesolv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hiv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hopv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kaggle_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)   165414 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kaggle_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8104 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kinase_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/lipo_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9165 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/load_dataset_template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.477118 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4474 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_bandgap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_perovskite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8680 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/molnet_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/muv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/nci_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/pcba_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/pdbbind_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/ppb_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm7_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm8_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm9_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sampl_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sider_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sweetlead_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/thermosol_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3530 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/tox21_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18900 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/toxcast_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7662 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uspto_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uv_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uv_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6895 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/zinc15_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/preset_hyper_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13549 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark_low_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36564 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.477118 deepchem-2.7.2.dev20230717161942/deepchem/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)     9312 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23102 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/a2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.477118 deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/test_tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/tictactoe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/rl/ppo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.477118 deepchem-2.7.2.dev20230717161942/deepchem/splits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/splits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63895 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/splits/splitters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/splits/task_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.477118 deepchem-2.7.2.dev20230717161942/deepchem/trans/
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/trans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6571 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/trans/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91191 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/trans/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.481118 deepchem-2.7.2.dev20230717161942/deepchem/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     6141 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10069 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/conformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13294 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20923 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/debug_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14881 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19454 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6134 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13312 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17713 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11749 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65672 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/sequence_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.481118 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_coordinate_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_dftutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_docking_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_electron_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_fake_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_fragment_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_generator_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_genomics_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3296 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_grover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_hash_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9115 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_molecule_feature_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6251 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_noncovalent_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_pdbqt_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_pytorch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_rdkit_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_sequence_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_updated_scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_voxel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/vina_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7797 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/deepchem/utils/voxel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 16:19:42.449118 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 16:19:42.000000 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-17 16:19:42.000000 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 16:19:42.000000 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-17 16:19:42.000000 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 16:19:42.000000 deepchem-2.7.2.dev20230717161942/deepchem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 16:19:42.481118 deepchem-2.7.2.dev20230717161942/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-17 16:19:31.000000 deepchem-2.7.2.dev20230717161942/setup.py
```

### Comparing `deepchem-2.7.2.dev20230712172748/LICENSE` & `deepchem-2.7.2.dev20230717161942/LICENSE`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/PKG-INFO` & `deepchem-2.7.2.dev20230717161942/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230712172748
+Version: 2.7.2.dev20230717161942
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230712172748/README.md` & `deepchem-2.7.2.dev20230717161942/README.md`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/data/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/data/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/data/data_loader.py` & `deepchem-2.7.2.dev20230717161942/deepchem/data/data_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/data/datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/data/datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/data/pytorch_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/data/pytorch_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/data/supports.py` & `deepchem-2.7.2.dev20230717161942/deepchem/data/supports.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/dock/binding_pocket.py` & `deepchem-2.7.2.dev20230717161942/deepchem/dock/binding_pocket.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/dock/docking.py` & `deepchem-2.7.2.dev20230717161942/deepchem/dock/docking.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/dock/pose_generation.py` & `deepchem-2.7.2.dev20230717161942/deepchem/dock/pose_generation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/dock/pose_scoring.py` & `deepchem-2.7.2.dev20230717161942/deepchem/dock/pose_scoring.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/atomic_conformation.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/atomic_conformation.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/base_classes.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/bert_tokenizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/binding_pocket_features.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/binding_pocket_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/complex_atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/contact_fingerprints.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/contact_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/grid_featurizers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/grid_featurizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/rdkit_grid_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/complex_featurizers/splif_fingerprints.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/complex_featurizers/splif_fingerprints.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/dft_data.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/dft_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/graph_data.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/graph_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/graph_features.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/graph_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/huggingface_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/huggingface_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/cgcnn_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/cgcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/element_property_fingerprint.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/element_property_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/elemnet_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/elemnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/lcnn_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/lcnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/material_featurizers/sine_coulomb_matrix.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/material_featurizers/sine_coulomb_matrix.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/mol_graphs.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/mol_graphs.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/atomic_coordinates.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/atomic_coordinates.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/bp_symmetry_function_input.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/circular_fingerprint.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/circular_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/conformer_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/conformer_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/coulomb_matrices.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/coulomb_matrices.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/dmpnn_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/grover_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/grover_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/maccs_keys_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mat_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mat_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mol2vec_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mol_graph_conv_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/molgan_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/molgan_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mordred_descriptors.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mordred_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/mxmnet_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/one_hot_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/pubchem_fingerprint.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/raw_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/raw_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/rdkit_descriptors.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/rdkit_descriptors.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/smiles_to_image.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/smiles_to_image.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/smiles_to_seq.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/smiles_to_seq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/snap_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/snap_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/molecule_featurizers/sparse_matrix_one_hot_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/reaction_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/reaction_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/roberta_tokenizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/sequence_featurizers/position_frequency_matrix_featurizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/smiles_tokenizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/smiles_tokenizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/grover_vocab.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/grover_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/hf_vocab.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/hf_vocab.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/feat/vocabulary_builders/vocabulary_builder.py` & `deepchem-2.7.2.dev20230717161942/deepchem/feat/vocabulary_builders/vocabulary_builder.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/hyper/base_classes.py` & `deepchem-2.7.2.dev20230717161942/deepchem/hyper/base_classes.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/hyper/gaussian_process.py` & `deepchem-2.7.2.dev20230717161942/deepchem/hyper/gaussian_process.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/hyper/grid_search.py` & `deepchem-2.7.2.dev20230717161942/deepchem/hyper/grid_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/hyper/random_search.py` & `deepchem-2.7.2.dev20230717161942/deepchem/hyper/random_search.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/metalearning/maml.py` & `deepchem-2.7.2.dev20230717161942/deepchem/metalearning/maml.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/metrics/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/metrics/genomic_metrics.py` & `deepchem-2.7.2.dev20230717161942/deepchem/metrics/genomic_metrics.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/metrics/metric.py` & `deepchem-2.7.2.dev20230717161942/deepchem/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/metrics/score_function.py` & `deepchem-2.7.2.dev20230717161942/deepchem/metrics/score_function.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/IRV.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/IRV.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/atomic_conv.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/atomic_conv.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/callbacks.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/chemnet_layers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/chemnet_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/chemnet_models.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/chemnet_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/dft/dftxc.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/dft/dftxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/dft/nnxc.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/dft/nnxc.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/dft/scf.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/dft/scf.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/fcnet.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/fcnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/gan.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/gan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/gbdt_models/gbdt_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/gbdt_models/gbdt_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/graph_models.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/graph_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/jax_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/jax_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/layers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/jax_models/pinns_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/jax_models/pinns_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/keras_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/keras_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/layers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/dc_lightning_dataset_module.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/dc_lightning_dataset_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/lightning/dc_lightning_module.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/lightning/dc_lightning_module.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/losses.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/losses.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/models.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/molgan.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/molgan.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/multitask.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/normalizing_flows.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/normalizing_flows.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/optimizers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/progressive_multitask.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/progressive_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/robust_multitask.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/robust_multitask.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/scscore.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/scscore.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/seqtoseq.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/seqtoseq.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/sklearn_models/sklearn_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/sklearn_models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/text_cnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/text_cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from deepchem.models.torch_models.infograph import InfoGraphStar, InfoGraphStarModel, InfoGraphEncoder, GINEncoder, InfoGraph, InfoGraphModel, InfoGraphEncoder
 from deepchem.models.torch_models.mpnn import MPNN, MPNNModel
 from deepchem.models.torch_models.lcnn import LCNN, LCNNModel
 from deepchem.models.torch_models.pagtn import Pagtn, PagtnModel
 from deepchem.models.torch_models.mat import MAT, MATModel
 from deepchem.models.torch_models.megnet import MEGNetModel
 from deepchem.models.torch_models.normalizing_flows_pytorch import NormalizingFlow
-from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, MolGANConvolutionLayer, MolGANAggregationLayer
+from deepchem.models.torch_models.layers import MultilayerPerceptron, CNNModule, CombineMeanStd, WeightedLinearCombo, AtomicConvolution, NeighborList, SetGather, EdgeNetwork, WeaveLayer, WeaveGather, MolGANConvolutionLayer, MolGANAggregationLayer
 from deepchem.models.torch_models.cnn import CNN
 from deepchem.models.torch_models.attention import ScaledDotProductAttention, SelfAttention
 from deepchem.models.torch_models.grover import GroverModel, GroverPretrain, GroverFinetune
 from deepchem.models.torch_models.readout import GroverReadout
 try:
     from deepchem.models.torch_models.dmpnn import DMPNN, DMPNNModel
     from deepchem.models.torch_models.gnn import GNN, GNNHead, GNNModular
```

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/attention.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/attention.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/attentivefp.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/attentivefp.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/cgcnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/cgcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/chemberta.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/chemberta.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/cnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/cnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/dmpnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/dmpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/ferminet.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/ferminet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gat.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gcn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gcn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/gnn3d.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/gnn3d.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/grover.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/grover_layers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/grover_layers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/hf_models.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/hf_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/infograph.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/infograph.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/kfac_optimizer.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/kfac_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/layers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -9590,8 +9590,557 @@
 00025750: 2050 203d 2073 656c 662e 505f 626e 2850   P = self.P_bn(P
 00025760: 290a 2020 2020 2020 2020 2020 2020 5020  ).            P 
 00025770: 3d20 6163 7469 7661 7469 6f6e 2850 290a  = activation(P).
 00025780: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
 00025790: 2020 2020 2020 2020 2020 5020 3d20 7061            P = pa
 000257a0: 6972 5f66 6561 7475 7265 730a 0a20 2020  ir_features..   
 000257b0: 2020 2020 2072 6574 7572 6e20 5b41 2c20       return [A, 
-000257c0: 505d 0a                                  P].
+000257c0: 505d 0a0a 0a63 6c61 7373 2057 6561 7665  P]...class Weave
+000257d0: 4761 7468 6572 286e 6e2e 4d6f 6475 6c65  Gather(nn.Module
+000257e0: 293a 0a20 2020 2022 2222 496d 706c 656d  ):.    """Implem
+000257f0: 656e 7473 2074 6865 2077 6561 7665 2d67  ents the weave-g
+00025800: 6174 6865 7269 6e67 2073 6563 7469 6f6e  athering section
+00025810: 206f 6620 7765 6176 6520 636f 6e76 6f6c   of weave convol
+00025820: 7574 696f 6e73 2e0a 2020 2020 5468 6973  utions..    This
+00025830: 2069 7320 7468 6520 546f 7263 6820 6571   is the Torch eq
+00025840: 7569 7661 6c65 6e74 206f 6620 7468 6520  uivalent of the 
+00025850: 6f72 6967 696e 616c 2069 6d70 6c65 6d65  original impleme
+00025860: 6e74 6174 696f 6e20 7573 696e 6720 4b65  ntation using Ke
+00025870: 7261 732e 0a0a 2020 2020 496d 706c 656d  ras...    Implem
+00025880: 656e 7473 2074 6865 2067 6174 6865 7269  ents the gatheri
+00025890: 6e67 206c 6179 6572 2066 726f 6d20 5b31  ng layer from [1
+000258a0: 5d5f 2e20 5468 6520 7765 6176 6520 6761  ]_. The weave ga
+000258b0: 7468 6572 696e 6720 6c61 7965 7220 6761  thering layer ga
+000258c0: 7468 6572 730a 2020 2020 7065 722d 6174  thers.    per-at
+000258d0: 6f6d 2066 6561 7475 7265 7320 746f 2063  om features to c
+000258e0: 7265 6174 6520 6120 6d6f 6c65 6375 6c65  reate a molecule
+000258f0: 2d6c 6576 656c 2066 696e 6765 7270 7269  -level fingerpri
+00025900: 6e74 2069 6e20 6120 7765 6176 650a 2020  nt in a weave.  
+00025910: 2020 636f 6e76 6f6c 7574 696f 6e61 6c20    convolutional 
+00025920: 6e65 7477 6f72 6b2e 2054 6869 7320 6c61  network. This la
+00025930: 7965 7220 6361 6e20 616c 736f 2070 6572  yer can also per
+00025940: 666f 726d 7320 4761 7573 7369 616e 2068  forms Gaussian h
+00025950: 6973 746f 6772 616d 0a20 2020 2065 7870  istogram.    exp
+00025960: 616e 7369 6f6e 2061 7320 6465 7461 696c  ansion as detail
+00025970: 6564 2069 6e20 5b31 5d5f 2e20 4e6f 7465  ed in [1]_. Note
+00025980: 2074 6861 7420 7468 6520 6761 7468 6572   that the gather
+00025990: 696e 6720 6675 6e63 7469 6f6e 2068 6572  ing function her
+000259a0: 6520 6973 0a20 2020 2073 696d 706c 7920  e is.    simply 
+000259b0: 6164 6469 7469 6f6e 2061 7320 696e 205b  addition as in [
+000259c0: 315d 5f3e 0a0a 2020 2020 4578 616d 706c  1]_>..    Exampl
+000259d0: 6573 0a20 2020 202d 2d2d 2d2d 2d2d 2d0a  es.    --------.
+000259e0: 2020 2020 5468 6973 206c 6179 6572 2065      This layer e
+000259f0: 7870 6563 7473 2032 2069 6e70 7574 7320  xpects 2 inputs 
+00025a00: 696e 2061 206c 6973 7420 6f66 2074 6865  in a list of the
+00025a10: 2066 6f72 6d20 605b 6174 6f6d 5f66 6561   form `[atom_fea
+00025a20: 7475 7265 732c 0a20 2020 2070 6169 725f  tures,.    pair_
+00025a30: 6665 6174 7572 6573 5d60 2e20 5765 276c  features]`. We'l
+00025a40: 6c20 7761 6c6b 2074 6872 6f75 6768 2074  l walk through t
+00025a50: 6865 2073 7472 7563 7475 7265 0a20 2020  he structure.   
+00025a60: 206f 6620 7468 6573 6520 696e 7075 7473   of these inputs
+00025a70: 2e20 4c65 7427 7320 7374 6172 7420 7769  . Let's start wi
+00025a80: 7468 2073 6f6d 6520 6261 7369 6320 6465  th some basic de
+00025a90: 6669 6e69 7469 6f6e 732e 0a0a 2020 2020  finitions...    
+00025aa0: 3e3e 3e20 696d 706f 7274 2064 6565 7063  >>> import deepc
+00025ab0: 6865 6d20 6173 2064 630a 2020 2020 3e3e  hem as dc.    >>
+00025ac0: 3e20 696d 706f 7274 206e 756d 7079 2061  > import numpy a
+00025ad0: 7320 6e70 0a0a 2020 2020 5375 7070 6f73  s np..    Suppos
+00025ae0: 6520 796f 7520 6861 7665 2061 2062 6174  e you have a bat
+00025af0: 6368 206f 6620 6d6f 6c65 6375 6c65 730a  ch of molecules.
+00025b00: 0a20 2020 203e 3e3e 2073 6d69 6c65 7320  .    >>> smiles 
+00025b10: 3d20 5b22 4343 4322 2c20 2243 225d 0a0a  = ["CCC", "C"]..
+00025b20: 2020 2020 4e6f 7465 2074 6861 7420 7468      Note that th
+00025b30: 6572 6520 6172 6520 3420 6174 6f6d 7320  ere are 4 atoms 
+00025b40: 696e 2074 6f74 616c 2069 6e20 7468 6973  in total in this
+00025b50: 2073 7973 7465 6d2e 2054 6869 7320 6c61   system. This la
+00025b60: 7965 7220 6578 7065 6374 7320 6974 730a  yer expects its.
+00025b70: 2020 2020 696e 7075 7420 6d6f 6c65 6375      input molecu
+00025b80: 6c65 7320 746f 2062 6520 6261 7463 6865  les to be batche
+00025b90: 6420 746f 6765 7468 6572 2e0a 0a20 2020  d together...   
+00025ba0: 203e 3e3e 2074 6f74 616c 5f6e 5f61 746f   >>> total_n_ato
+00025bb0: 6d73 203d 2034 0a0a 2020 2020 4c65 7427  ms = 4..    Let'
+00025bc0: 7320 7375 7070 6f73 6520 7468 6174 2077  s suppose that w
+00025bd0: 6520 6861 7665 2060 6e5f 6174 6f6d 5f66  e have `n_atom_f
+00025be0: 6561 7460 2066 6561 7475 7265 7320 7065  eat` features pe
+00025bf0: 7220 6174 6f6d 2e0a 0a20 2020 203e 3e3e  r atom...    >>>
+00025c00: 206e 5f61 746f 6d5f 6665 6174 203d 2037   n_atom_feat = 7
+00025c10: 350a 0a20 2020 2054 6865 6e20 636f 6e63  5..    Then conc
+00025c20: 6570 7475 616c 6c79 2c20 6061 746f 6d5f  eptually, `atom_
+00025c30: 6665 6174 6020 6973 2074 6865 2061 7272  feat` is the arr
+00025c40: 6179 206f 6620 7368 6170 6520 6028 746f  ay of shape `(to
+00025c50: 7461 6c5f 6e5f 6174 6f6d 732c 0a20 2020  tal_n_atoms,.   
+00025c60: 206e 5f61 746f 6d5f 6665 6174 2960 206f   n_atom_feat)` o
+00025c70: 6620 6174 6f6d 6963 2066 6561 7475 7265  f atomic feature
+00025c80: 732e 2046 6f72 2073 696d 706c 6963 6974  s. For simplicit
+00025c90: 792c 206c 6574 2773 206a 7573 7420 676f  y, let's just go
+00025ca0: 2077 6974 6820 610a 2020 2020 7261 6e64   with a.    rand
+00025cb0: 6f6d 2073 7563 6820 6d61 7472 6978 2e0a  om such matrix..
+00025cc0: 0a20 2020 203e 3e3e 2061 746f 6d5f 6665  .    >>> atom_fe
+00025cd0: 6174 203d 206e 702e 7261 6e64 6f6d 2e72  at = np.random.r
+00025ce0: 616e 6428 746f 7461 6c5f 6e5f 6174 6f6d  and(total_n_atom
+00025cf0: 732c 206e 5f61 746f 6d5f 6665 6174 290a  s, n_atom_feat).
+00025d00: 0a20 2020 2057 6520 7468 656e 206e 6565  .    We then nee
+00025d10: 6420 746f 2070 726f 7669 6465 2061 206d  d to provide a m
+00025d20: 6170 7069 6e67 206f 6620 696e 6469 6365  apping of indice
+00025d30: 7320 746f 2074 6865 2061 746f 6d73 2074  s to the atoms t
+00025d40: 6865 7920 6265 6c6f 6e67 2074 6f2e 2049  hey belong to. I
+00025d50: 6e0a 2020 2020 6f75 7273 2063 6173 6520  n.    ours case 
+00025d60: 7468 6973 2077 6f75 6c64 2062 650a 0a20  this would be.. 
+00025d70: 2020 203e 3e3e 2061 746f 6d5f 7370 6c69     >>> atom_spli
+00025d80: 7420 3d20 6e70 2e61 7272 6179 285b 302c  t = np.array([0,
+00025d90: 2030 2c20 302c 2031 5d29 0a0a 2020 2020   0, 0, 1])..    
+00025da0: 4c65 7427 7320 6e6f 7720 6465 6669 6e65  Let's now define
+00025db0: 2074 6865 2061 6374 7561 6c20 6c61 7965   the actual laye
+00025dc0: 720a 0a20 2020 203e 3e3e 2067 6174 6865  r..    >>> gathe
+00025dd0: 7220 3d20 5765 6176 6547 6174 6865 7228  r = WeaveGather(
+00025de0: 6261 7463 685f 7369 7a65 3d32 2c20 6e5f  batch_size=2, n_
+00025df0: 696e 7075 743d 6e5f 6174 6f6d 5f66 6561  input=n_atom_fea
+00025e00: 7429 0a20 2020 203e 3e3e 206f 7574 7075  t).    >>> outpu
+00025e10: 745f 6d6f 6c65 6375 6c65 7320 3d20 6761  t_molecules = ga
+00025e20: 7468 6572 285b 6174 6f6d 5f66 6561 742c  ther([atom_feat,
+00025e30: 2061 746f 6d5f 7370 6c69 745d 290a 2020   atom_split]).  
+00025e40: 2020 3e3e 3e20 6c65 6e28 6f75 7470 7574    >>> len(output
+00025e50: 5f6d 6f6c 6563 756c 6573 290a 2020 2020  _molecules).    
+00025e60: 320a 0a20 2020 2052 6566 6572 656e 6365  2..    Reference
+00025e70: 730a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  s.    ----------
+00025e80: 0a20 2020 202e 2e20 5b31 5d20 4b65 6172  .    .. [1] Kear
+00025e90: 6e65 732c 2053 7465 7665 6e2c 2065 7420  nes, Steven, et 
+00025ea0: 616c 2e20 224d 6f6c 6563 756c 6172 2067  al. "Molecular g
+00025eb0: 7261 7068 2063 6f6e 766f 6c75 7469 6f6e  raph convolution
+00025ec0: 733a 206d 6f76 696e 6720 6265 796f 6e64  s: moving beyond
+00025ed0: 0a20 2020 2020 2020 2066 696e 6765 7270  .        fingerp
+00025ee0: 7269 6e74 732e 2220 4a6f 7572 6e61 6c20  rints." Journal 
+00025ef0: 6f66 2063 6f6d 7075 7465 722d 6169 6465  of computer-aide
+00025f00: 6420 6d6f 6c65 6375 6c61 7220 6465 7369  d molecular desi
+00025f10: 676e 2033 302e 3820 2832 3031 3629 3a0a  gn 30.8 (2016):.
+00025f20: 2020 2020 2020 2020 3539 352d 3630 382e          595-608.
+00025f30: 0a20 2020 2022 2222 0a0a 2020 2020 6465  .    """..    de
+00025f40: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
+00025f50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00025f60: 2020 6261 7463 685f 7369 7a65 3a20 696e    batch_size: in
+00025f70: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00025f80: 2020 2020 6e5f 696e 7075 743a 2069 6e74      n_input: int
+00025f90: 203d 2031 3238 2c0a 2020 2020 2020 2020   = 128,.        
+00025fa0: 2020 2020 2020 2020 2067 6175 7373 6961           gaussia
+00025fb0: 6e5f 6578 7061 6e64 3a20 626f 6f6c 203d  n_expand: bool =
+00025fc0: 2054 7275 652c 0a20 2020 2020 2020 2020   True,.         
+00025fd0: 2020 2020 2020 2020 636f 6d70 7265 7373          compress
+00025fe0: 5f70 6f73 745f 6761 7573 7369 616e 5f65  _post_gaussian_e
+00025ff0: 7870 616e 7369 6f6e 3a20 626f 6f6c 203d  xpansion: bool =
+00026000: 2046 616c 7365 2c0a 2020 2020 2020 2020   False,.        
+00026010: 2020 2020 2020 2020 2069 6e69 745f 3a20           init_: 
+00026020: 7374 7220 3d20 2778 6176 6965 725f 756e  str = 'xavier_un
+00026030: 6966 6f72 6d5f 272c 0a20 2020 2020 2020  iform_',.       
+00026040: 2020 2020 2020 2020 2020 6163 7469 7661            activa
+00026050: 7469 6f6e 3a20 7374 7220 3d20 2774 616e  tion: str = 'tan
+00026060: 6827 2c0a 2020 2020 2020 2020 2020 2020  h',.            
+00026070: 2020 2020 202a 2a6b 7761 7267 7329 3a0a       **kwargs):.
+00026080: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00026090: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+000260a0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+000260b0: 2d0a 2020 2020 2020 2020 6261 7463 685f  -.        batch_
+000260c0: 7369 7a65 3a20 696e 740a 2020 2020 2020  size: int.      
+000260d0: 2020 2020 2020 6e75 6d62 6572 206f 6620        number of 
+000260e0: 6d6f 6c65 6375 6c65 7320 696e 2061 2062  molecules in a b
+000260f0: 6174 6368 0a20 2020 2020 2020 206e 5f69  atch.        n_i
+00026100: 6e70 7574 3a20 696e 742c 206f 7074 696f  nput: int, optio
+00026110: 6e61 6c20 2864 6566 6175 6c74 2031 3238  nal (default 128
+00026120: 290a 2020 2020 2020 2020 2020 2020 6e75  ).            nu
+00026130: 6d62 6572 206f 6620 6665 6174 7572 6573  mber of features
+00026140: 2066 6f72 2065 6163 6820 696e 7075 7420   for each input 
+00026150: 6d6f 6c65 6375 6c65 0a20 2020 2020 2020  molecule.       
+00026160: 2067 6175 7373 6961 6e5f 6578 7061 6e64   gaussian_expand
+00026170: 3a20 626f 6f6c 6561 6e2c 206f 7074 696f  : boolean, optio
+00026180: 6e61 6c20 2864 6566 6175 6c74 2054 7275  nal (default Tru
+00026190: 6529 0a20 2020 2020 2020 2020 2020 2057  e).            W
+000261a0: 6865 7468 6572 2074 6f20 6578 7061 6e64  hether to expand
+000261b0: 2065 6163 6820 6469 6d65 6e73 696f 6e20   each dimension 
+000261c0: 6f66 2061 746f 6d69 6320 6665 6174 7572  of atomic featur
+000261d0: 6573 2062 7920 6761 7573 7369 616e 2068  es by gaussian h
+000261e0: 6973 746f 6772 616d 0a20 2020 2020 2020  istogram.       
+000261f0: 2063 6f6d 7072 6573 735f 706f 7374 5f67   compress_post_g
+00026200: 6175 7373 6961 6e5f 6578 7061 6e73 696f  aussian_expansio
+00026210: 6e3a 2062 6f6f 6c2c 206f 7074 696f 6e61  n: bool, optiona
+00026220: 6c20 2864 6566 6175 6c74 2046 616c 7365  l (default False
+00026230: 290a 2020 2020 2020 2020 2020 2020 4966  ).            If
+00026240: 2054 7275 652c 2063 6f6d 7072 6573 7320   True, compress 
+00026250: 7468 6520 7265 7375 6c74 7320 6f66 2074  the results of t
+00026260: 6865 2047 6175 7373 6961 6e20 6578 7061  he Gaussian expa
+00026270: 6e73 696f 6e20 6261 636b 2074 6f20 7468  nsion back to th
+00026280: 650a 2020 2020 2020 2020 2020 2020 6f72  e.            or
+00026290: 6967 696e 616c 2064 696d 656e 7369 6f6e  iginal dimension
+000262a0: 7320 6f66 2074 6865 2069 6e70 7574 2062  s of the input b
+000262b0: 7920 7573 696e 6720 6120 6c69 6e65 6172  y using a linear
+000262c0: 206c 6179 6572 2077 6974 6820 7370 6563   layer with spec
+000262d0: 6966 6965 640a 2020 2020 2020 2020 2020  ified.          
+000262e0: 2020 6163 7469 7661 7469 6f6e 2066 756e    activation fun
+000262f0: 6374 696f 6e2e 204e 6f74 6520 7468 6174  ction. Note that
+00026300: 2074 6869 7320 636f 6d70 7265 7373 696f   this compressio
+00026310: 6e20 7761 7320 6e6f 7420 696e 2074 6865  n was not in the
+00026320: 206f 7269 6769 6e61 6c0a 2020 2020 2020   original.      
+00026330: 2020 2020 2020 7061 7065 722c 2062 7574        paper, but
+00026340: 2077 6173 2070 7265 7365 6e74 2069 6e20   was present in 
+00026350: 7468 6520 6f72 6967 696e 616c 2044 6565  the original Dee
+00026360: 7043 6865 6d20 696d 706c 656d 656e 7461  pChem implementa
+00026370: 7469 6f6e 2073 6f20 6973 0a20 2020 2020  tion so is.     
+00026380: 2020 2020 2020 206c 6566 7420 7072 6573         left pres
+00026390: 656e 7420 666f 7220 6261 636b 7761 7264  ent for backward
+000263a0: 7320 636f 6d70 6174 6962 696c 6974 792e  s compatibility.
+000263b0: 0a20 2020 2020 2020 2069 6e69 743a 2073  .        init: s
+000263c0: 7472 2c20 6f70 7469 6f6e 616c 2028 6465  tr, optional (de
+000263d0: 6661 756c 7420 2778 6176 6965 725f 756e  fault 'xavier_un
+000263e0: 6966 6f72 6d5f 2729 0a20 2020 2020 2020  iform_').       
+000263f0: 2020 2020 2057 6569 6768 7420 696e 6974       Weight init
+00026400: 6961 6c69 7a61 7469 6f6e 2066 6f72 2066  ialization for f
+00026410: 696c 7465 7273 2069 6620 6063 6f6d 7072  ilters if `compr
+00026420: 6573 735f 706f 7374 5f67 6175 7373 6961  ess_post_gaussia
+00026430: 6e5f 6578 7061 6e73 696f 6e60 0a20 2020  n_expansion`.   
+00026440: 2020 2020 2020 2020 2069 7320 5472 7565           is True
+00026450: 2e0a 2020 2020 2020 2020 6163 7469 7661  ..        activa
+00026460: 7469 6f6e 3a20 7374 722c 206f 7074 696f  tion: str, optio
+00026470: 6e61 6c20 2864 6566 6175 6c74 2027 7461  nal (default 'ta
+00026480: 6e68 2729 0a20 2020 2020 2020 2020 2020  nh').           
+00026490: 2041 6374 6976 6174 696f 6e20 6675 6e63   Activation func
+000264a0: 7469 6f6e 2061 7070 6c69 6564 2066 6f72  tion applied for
+000264b0: 2066 696c 7465 7273 2069 660a 2020 2020   filters if.    
+000264c0: 2020 2020 2020 2020 6063 6f6d 7072 6573          `compres
+000264d0: 735f 706f 7374 5f67 6175 7373 6961 6e5f  s_post_gaussian_
+000264e0: 6578 7061 6e73 696f 6e60 2069 7320 5472  expansion` is Tr
+000264f0: 7565 2e0a 2020 2020 2020 2020 2222 220a  ue..        """.
+00026500: 2020 2020 2020 2020 7375 7065 7228 5765          super(We
+00026510: 6176 6547 6174 6865 722c 2073 656c 6629  aveGather, self)
+00026520: 2e5f 5f69 6e69 745f 5f28 2a2a 6b77 6172  .__init__(**kwar
+00026530: 6773 290a 2020 2020 2020 2020 7365 6c66  gs).        self
+00026540: 2e6e 5f69 6e70 7574 3a20 696e 7420 3d20  .n_input: int = 
+00026550: 6e5f 696e 7075 740a 2020 2020 2020 2020  n_input.        
+00026560: 7365 6c66 2e62 6174 6368 5f73 697a 653a  self.batch_size:
+00026570: 2069 6e74 203d 2062 6174 6368 5f73 697a   int = batch_siz
+00026580: 650a 2020 2020 2020 2020 7365 6c66 2e67  e.        self.g
+00026590: 6175 7373 6961 6e5f 6578 7061 6e64 3a20  aussian_expand: 
+000265a0: 626f 6f6c 203d 2067 6175 7373 6961 6e5f  bool = gaussian_
+000265b0: 6578 7061 6e64 0a20 2020 2020 2020 2073  expand.        s
+000265c0: 656c 662e 636f 6d70 7265 7373 5f70 6f73  elf.compress_pos
+000265d0: 745f 6761 7573 7369 616e 5f65 7870 616e  t_gaussian_expan
+000265e0: 7369 6f6e 3a20 626f 6f6c 203d 2063 6f6d  sion: bool = com
+000265f0: 7072 6573 735f 706f 7374 5f67 6175 7373  press_post_gauss
+00026600: 6961 6e5f 6578 7061 6e73 696f 6e0a 2020  ian_expansion.  
+00026610: 2020 2020 2020 7365 6c66 2e69 6e69 743a        self.init:
+00026620: 2073 7472 203d 2069 6e69 745f 2020 2320   str = init_  # 
+00026630: 5365 7420 7765 6967 6874 2069 6e69 7469  Set weight initi
+00026640: 616c 697a 6174 696f 6e0a 2020 2020 2020  alization.      
+00026650: 2020 7365 6c66 2e61 6374 6976 6174 696f    self.activatio
+00026660: 6e3a 2073 7472 203d 2061 6374 6976 6174  n: str = activat
+00026670: 696f 6e20 2023 2047 6574 2061 6374 6976  ion  # Get activ
+00026680: 6174 696f 6e73 0a20 2020 2020 2020 2073  ations.        s
+00026690: 656c 662e 6163 7469 7661 7469 6f6e 5f66  elf.activation_f
+000266a0: 6e3a 2074 6f72 6368 2e6e 6e2e 4d6f 6475  n: torch.nn.Modu
+000266b0: 6c65 203d 2067 6574 5f61 6374 6976 6174  le = get_activat
+000266c0: 696f 6e28 6163 7469 7661 7469 6f6e 290a  ion(activation).
+000266d0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+000266e0: 2e63 6f6d 7072 6573 735f 706f 7374 5f67  .compress_post_g
+000266f0: 6175 7373 6961 6e5f 6578 7061 6e73 696f  aussian_expansio
+00026700: 6e3a 0a20 2020 2020 2020 2020 2020 2069  n:.            i
+00026710: 6e69 7420 3d20 6765 7461 7474 7228 696e  nit = getattr(in
+00026720: 6974 6961 6c69 7a65 7273 2c20 7365 6c66  itializers, self
+00026730: 2e69 6e69 7429 0a20 2020 2020 2020 2020  .init).         
+00026740: 2020 2073 656c 662e 573a 2074 6f72 6368     self.W: torch
+00026750: 2e54 656e 736f 7220 3d20 696e 6974 280a  .Tensor = init(.
+00026760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026770: 746f 7263 682e 656d 7074 7928 5b73 656c  torch.empty([sel
+00026780: 662e 6e5f 696e 7075 7420 2a20 3131 2c20  f.n_input * 11, 
+00026790: 7365 6c66 2e6e 5f69 6e70 7574 5d29 290a  self.n_input])).
+000267a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000267b0: 2e62 3a20 746f 7263 682e 5465 6e73 6f72  .b: torch.Tensor
+000267c0: 203d 2074 6f72 6368 2e7a 6572 6f73 2828   = torch.zeros((
+000267d0: 7365 6c66 2e6e 5f69 6e70 7574 2c29 290a  self.n_input,)).
+000267e0: 2020 2020 2020 2020 7365 6c66 2e62 7569          self.bui
+000267f0: 6c74 203d 2054 7275 650a 0a20 2020 2064  lt = True..    d
+00026800: 6566 205f 5f72 6570 725f 5f28 7365 6c66  ef __repr__(self
+00026810: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00026820: 2020 2020 2020 2052 6574 7572 6e73 2061         Returns a
+00026830: 2073 7472 696e 6720 7265 7072 6573 656e   string represen
+00026840: 7461 7469 6f6e 206f 6620 7468 6520 6f62  tation of the ob
+00026850: 6a65 6374 2e0a 0a20 2020 2020 2020 2052  ject...        R
+00026860: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00026870: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00026880: 7374 723a 2041 2073 7472 696e 6720 7468  str: A string th
+00026890: 6174 2063 6f6e 7461 696e 7320 7468 6520  at contains the 
+000268a0: 636c 6173 7320 6e61 6d65 2066 6f6c 6c6f  class name follo
+000268b0: 7765 6420 6279 2074 6865 2076 616c 7565  wed by the value
+000268c0: 7320 6f66 2069 7473 2069 6e73 7461 6e63  s of its instanc
+000268d0: 6520 7661 7269 6162 6c65 2e0a 2020 2020  e variable..    
+000268e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000268f0: 7265 7475 726e 2028 0a20 2020 2020 2020  return (.       
+00026900: 2020 2020 2066 277b 7365 6c66 2e5f 5f63       f'{self.__c
+00026910: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f7d  lass__.__name__}
+00026920: 2862 6174 6368 5f73 697a 653a 7b73 656c  (batch_size:{sel
+00026930: 662e 6261 7463 685f 7369 7a65 7d2c 6e5f  f.batch_size},n_
+00026940: 696e 7075 743a 7b73 656c 662e 6e5f 696e  input:{self.n_in
+00026950: 7075 747d 2c67 6175 7373 6961 6e5f 6578  put},gaussian_ex
+00026960: 7061 6e64 3a7b 7365 6c66 2e67 6175 7373  pand:{self.gauss
+00026970: 6961 6e5f 6578 7061 6e64 7d2c 696e 6974  ian_expand},init
+00026980: 3a7b 7365 6c66 2e69 6e69 747d 2c61 6374  :{self.init},act
+00026990: 6976 6174 696f 6e3a 7b73 656c 662e 6163  ivation:{self.ac
+000269a0: 7469 7661 7469 6f6e 7d2c 636f 6d70 7265  tivation},compre
+000269b0: 7373 5f70 6f73 745f 6761 7573 7369 616e  ss_post_gaussian
+000269c0: 5f65 7870 616e 7369 6f6e 3a7b 7365 6c66  _expansion:{self
+000269d0: 2e63 6f6d 7072 6573 735f 706f 7374 5f67  .compress_post_g
+000269e0: 6175 7373 6961 6e5f 6578 7061 6e73 696f  aussian_expansio
+000269f0: 6e7d 2927 0a20 2020 2020 2020 2029 0a0a  n})'.        )..
+00026a00: 2020 2020 6465 6620 666f 7277 6172 6428      def forward(
+00026a10: 7365 6c66 2c20 696e 7075 7473 3a20 4c69  self, inputs: Li
+00026a20: 7374 5b55 6e69 6f6e 5b6e 702e 6e64 6172  st[Union[np.ndar
+00026a30: 7261 792c 0a20 2020 2020 2020 2020 2020  ray,.           
+00026a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00026a50: 2020 2020 2020 2020 2020 2020 2020 6e70                np
+00026a60: 2e6e 6461 7272 6179 5d5d 2920 2d3e 2074  .ndarray]]) -> t
+00026a70: 6f72 6368 2e54 656e 736f 723a 0a20 2020  orch.Tensor:.   
+00026a80: 2020 2020 2022 2222 4372 6561 7465 7320       """Creates 
+00026a90: 7765 6176 6520 7465 6e73 6f72 732e 0a0a  weave tensors...
+00026aa0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+00026ab0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
+00026ac0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 696e  -----.        in
+00026ad0: 7075 7473 3a20 4c69 7374 5b55 6e69 6f6e  puts: List[Union
+00026ae0: 5b6e 702e 6e64 6172 7261 792c 6e70 2e6e  [np.ndarray,np.n
+00026af0: 6461 7272 6179 5d5d 0a20 2020 2020 2020  darray]].       
+00026b00: 2020 2020 2053 686f 756c 6420 636f 6e74       Should cont
+00026b10: 6169 6e20 3220 7465 6e73 6f72 7320 5b61  ain 2 tensors [a
+00026b20: 746f 6d5f 6665 6174 7572 6573 2c20 6174  tom_features, at
+00026b30: 6f6d 5f73 706c 6974 5d0a 0a20 2020 2020  om_split]..     
+00026b40: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00026b50: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00026b60: 2020 206f 7574 7075 745f 6d6f 6c65 6375     output_molecu
+00026b70: 6c65 733a 2074 6f72 6368 2e54 656e 736f  les: torch.Tenso
+00026b80: 720a 2020 2020 2020 2020 2020 2020 4561  r.            Ea
+00026b90: 6368 2065 6e74 7279 2069 6e20 7468 6973  ch entry in this
+00026ba0: 206c 6973 7420 6973 206f 6620 7368 6170   list is of shap
+00026bb0: 6520 6028 7365 6c66 2e6e 5f69 6e70 7574  e `(self.n_input
+00026bc0: 732c 2960 0a0a 2020 2020 2020 2020 2222  s,)`..        ""
+00026bd0: 220a 2020 2020 2020 2020 6f75 7470 7574  ".        output
+00026be0: 733a 2074 6f72 6368 2e54 656e 736f 7220  s: torch.Tensor 
+00026bf0: 3d20 746f 7263 682e 7465 6e73 6f72 2869  = torch.tensor(i
+00026c00: 6e70 7574 735b 305d 290a 2020 2020 2020  nputs[0]).      
+00026c10: 2020 6174 6f6d 5f73 706c 6974 3a20 746f    atom_split: to
+00026c20: 7263 682e 5465 6e73 6f72 203d 2074 6f72  rch.Tensor = tor
+00026c30: 6368 2e74 656e 736f 7228 696e 7075 7473  ch.tensor(inputs
+00026c40: 5b31 5d29 0a0a 2020 2020 2020 2020 6966  [1])..        if
+00026c50: 2073 656c 662e 6761 7573 7369 616e 5f65   self.gaussian_e
+00026c60: 7870 616e 643a 0a20 2020 2020 2020 2020  xpand:.         
+00026c70: 2020 206f 7574 7075 7473 203d 2073 656c     outputs = sel
+00026c80: 662e 6761 7573 7369 616e 5f68 6973 746f  f.gaussian_histo
+00026c90: 6772 616d 286f 7574 7075 7473 290a 0a20  gram(outputs).. 
+00026ca0: 2020 2020 2020 2074 5f67 7270 3a20 4469         t_grp: Di
+00026cb0: 6374 5b54 656e 736f 722c 2054 656e 736f  ct[Tensor, Tenso
+00026cc0: 725d 203d 207b 7d0a 2020 2020 2020 2020  r] = {}.        
+00026cd0: 6964 783a 2069 6e74 203d 2030 0a20 2020  idx: int = 0.   
+00026ce0: 2020 2020 2066 6f72 2069 2c20 735f 6964       for i, s_id
+00026cf0: 2069 6e20 656e 756d 6572 6174 6528 6174   in enumerate(at
+00026d00: 6f6d 5f73 706c 6974 293a 0a20 2020 2020  om_split):.     
+00026d10: 2020 2020 2020 2073 5f69 6420 3d20 735f         s_id = s_
+00026d20: 6964 2e69 7465 6d28 290a 2020 2020 2020  id.item().      
+00026d30: 2020 2020 2020 6966 2073 5f69 6420 696e        if s_id in
+00026d40: 2074 5f67 7270 3a0a 2020 2020 2020 2020   t_grp:.        
+00026d50: 2020 2020 2020 2020 745f 6772 705b 735f          t_grp[s_
+00026d60: 6964 5d20 3d20 745f 6772 705b 735f 6964  id] = t_grp[s_id
+00026d70: 5d20 2b20 6f75 7470 7574 735b 6964 785d  ] + outputs[idx]
+00026d80: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00026d90: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00026da0: 2020 2074 5f67 7270 5b73 5f69 645d 203d     t_grp[s_id] =
+00026db0: 206f 7574 7075 7473 5b69 6478 5d0a 2020   outputs[idx].  
+00026dc0: 2020 2020 2020 2020 2020 6964 7820 3d20            idx = 
+00026dd0: 6920 2b20 310a 0a20 2020 2020 2020 2020  i + 1..         
+00026de0: 2020 206c 7374 203d 206c 6973 7428 745f     lst = list(t_
+00026df0: 6772 702e 7661 6c75 6573 2829 290a 2020  grp.values()).  
+00026e00: 2020 2020 2020 2020 2020 7465 6e73 6f72            tensor
+00026e10: 203d 2074 6f72 6368 2e73 7461 636b 286c   = torch.stack(l
+00026e20: 7374 290a 2020 2020 2020 2020 6f75 7470  st).        outp
+00026e30: 7574 5f6d 6f6c 6563 756c 6573 3a20 746f  ut_molecules: to
+00026e40: 7263 682e 5465 6e73 6f72 203d 2074 656e  rch.Tensor = ten
+00026e50: 736f 720a 0a20 2020 2020 2020 2069 6620  sor..        if 
+00026e60: 7365 6c66 2e63 6f6d 7072 6573 735f 706f  self.compress_po
+00026e70: 7374 5f67 6175 7373 6961 6e5f 6578 7061  st_gaussian_expa
+00026e80: 6e73 696f 6e3a 0a20 2020 2020 2020 2020  nsion:.         
+00026e90: 2020 206f 7574 7075 745f 6d6f 6c65 6375     output_molecu
+00026ea0: 6c65 7320 3d20 746f 7263 682e 6d61 746d  les = torch.matm
+00026eb0: 756c 280a 2020 2020 2020 2020 2020 2020  ul(.            
+00026ec0: 2020 2020 6f75 7470 7574 5f6d 6f6c 6563      output_molec
+00026ed0: 756c 6573 2e74 7970 6528 746f 7263 682e  ules.type(torch.
+00026ee0: 666c 6f61 7433 3229 2c20 7365 6c66 2e57  float32), self.W
+00026ef0: 2920 2b20 7365 6c66 2e62 0a20 2020 2020  ) + self.b.     
+00026f00: 2020 2020 2020 206f 7574 7075 745f 6d6f         output_mo
+00026f10: 6c65 6375 6c65 7320 3d20 7365 6c66 2e61  lecules = self.a
+00026f20: 6374 6976 6174 696f 6e5f 666e 286f 7574  ctivation_fn(out
+00026f30: 7075 745f 6d6f 6c65 6375 6c65 7329 0a0a  put_molecules)..
+00026f40: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00026f50: 7574 7075 745f 6d6f 6c65 6375 6c65 730a  utput_molecules.
+00026f60: 0a20 2020 2064 6566 2067 6175 7373 6961  .    def gaussia
+00026f70: 6e5f 6869 7374 6f67 7261 6d28 7365 6c66  n_histogram(self
+00026f80: 2c20 783a 2074 6f72 6368 2e54 656e 736f  , x: torch.Tenso
+00026f90: 7229 202d 3e20 746f 7263 682e 5465 6e73  r) -> torch.Tens
+00026fa0: 6f72 3a0a 2020 2020 2020 2020 2222 2245  or:.        """E
+00026fb0: 7870 616e 6473 2069 6e70 7574 2069 6e74  xpands input int
+00026fc0: 6f20 6120 7365 7420 6f66 2067 6175 7373  o a set of gauss
+00026fd0: 6961 6e20 6869 7374 6f67 7261 6d20 6269  ian histogram bi
+00026fe0: 6e73 2e0a 0a20 2020 2020 2020 2050 6172  ns...        Par
+00026ff0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00027000: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00027010: 2020 2078 3a20 746f 7263 682e 5465 6e73     x: torch.Tens
+00027020: 6f72 0a20 2020 2020 2020 2020 2020 204f  or.            O
+00027030: 6620 7368 6170 6520 6028 4e2c 206e 5f66  f shape `(N, n_f
+00027040: 6561 7429 600a 0a20 2020 2020 2020 2045  eat)`..        E
+00027050: 7861 6d70 6c65 730a 2020 2020 2020 2020  xamples.        
+00027060: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
+00027070: 2054 6869 7320 6d65 7468 6f64 2075 7365   This method use
+00027080: 7320 3131 2062 696e 7320 7370 616e 6e69  s 11 bins spanni
+00027090: 6e67 2070 6f72 7469 6f6e 7320 6f66 2061  ng portions of a
+000270a0: 2047 6175 7373 6961 6e20 7769 7468 207a   Gaussian with z
+000270b0: 6572 6f20 6d65 616e 0a20 2020 2020 2020  ero mean.       
+000270c0: 2061 6e64 2075 6e69 7420 7374 616e 6461   and unit standa
+000270d0: 7264 2064 6576 6961 7469 6f6e 2e0a 0a20  rd deviation... 
+000270e0: 2020 2020 2020 203e 3e3e 2067 6175 7373         >>> gauss
+000270f0: 6961 6e5f 6d65 6d62 6572 7368 6970 7320  ian_memberships 
+00027100: 3d20 5b28 2d31 2e36 3435 2c20 302e 3238  = [(-1.645, 0.28
+00027110: 3329 2c20 282d 312e 3038 302c 2030 2e31  3), (-1.080, 0.1
+00027120: 3730 292c 0a20 2020 2020 2020 202e 2e2e  70),.        ...
+00027130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027140: 2020 2020 2020 2020 2028 2d30 2e37 3339           (-0.739
+00027150: 2c20 302e 3133 3429 2c20 282d 302e 3436  , 0.134), (-0.46
+00027160: 382c 2030 2e31 3138 292c 0a20 2020 2020  8, 0.118),.     
+00027170: 2020 202e 2e2e 2020 2020 2020 2020 2020     ...          
+00027180: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00027190: 2d30 2e32 3238 2c20 302e 3131 3429 2c20  -0.228, 0.114), 
+000271a0: 2830 2e2c 2030 2e31 3134 292c 0a20 2020  (0., 0.114),.   
+000271b0: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
+000271c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000271d0: 2028 302e 3232 382c 2030 2e31 3134 292c   (0.228, 0.114),
+000271e0: 2028 302e 3436 382c 2030 2e31 3138 292c   (0.468, 0.118),
+000271f0: 0a20 2020 2020 2020 202e 2e2e 2020 2020  .        ...    
+00027200: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027210: 2020 2020 2028 302e 3733 392c 2030 2e31       (0.739, 0.1
+00027220: 3334 292c 2028 312e 3038 302c 2030 2e31  34), (1.080, 0.1
+00027230: 3730 292c 0a20 2020 2020 2020 202e 2e2e  70),.        ...
+00027240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027250: 2020 2020 2020 2020 2028 312e 3634 352c           (1.645,
+00027260: 2030 2e32 3833 295d 0a0a 2020 2020 2020   0.283)]..      
+00027270: 2020 5765 2063 6f6e 7374 7275 6374 2061    We construct a
+00027280: 2047 6175 7373 6961 6e20 6174 2060 6761   Gaussian at `ga
+00027290: 7573 7369 616e 5f6d 656d 6265 7273 6869  ussian_membershi
+000272a0: 7073 5b69 5d5b 305d 6020 7769 7468 2073  ps[i][0]` with s
+000272b0: 7461 6e64 6172 640a 2020 2020 2020 2020  tandard.        
+000272c0: 6465 7669 6174 696f 6e20 6067 6175 7373  deviation `gauss
+000272d0: 6961 6e5f 6d65 6d62 6572 7368 6970 735b  ian_memberships[
+000272e0: 695d 5b31 5d60 2e20 4561 6368 2066 6561  i][1]`. Each fea
+000272f0: 7475 7265 2069 6e20 6078 6020 6973 2061  ture in `x` is a
+00027300: 7373 6967 6e65 640a 2020 2020 2020 2020  ssigned.        
+00027310: 7468 6520 7072 6f62 6162 696c 6974 7920  the probability 
+00027320: 6f66 2066 616c 6c69 6e67 2069 6e20 6561  of falling in ea
+00027330: 6368 2047 6175 7373 6961 6e2c 2061 6e64  ch Gaussian, and
+00027340: 2070 726f 6261 6269 6c69 7469 6573 2061   probabilities a
+00027350: 7265 0a20 2020 2020 2020 206e 6f72 6d61  re.        norma
+00027360: 6c69 7a65 6420 6163 726f 7373 2074 6865  lized across the
+00027370: 2031 3120 6469 6666 6572 656e 7420 4761   11 different Ga
+00027380: 7573 7369 616e 732e 0a0a 2020 2020 2020  ussians...      
+00027390: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
+000273a0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
+000273b0: 2020 6f75 7470 7574 733a 2074 6f72 6368    outputs: torch
+000273c0: 2e54 656e 736f 720a 2020 2020 2020 2020  .Tensor.        
+000273d0: 2020 2020 4f66 2073 6861 7065 2060 284e      Of shape `(N
+000273e0: 2c20 3131 2a6e 5f66 6561 7429 600a 2020  , 11*n_feat)`.  
+000273f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00027400: 2020 696d 706f 7274 2074 6f72 6368 2e64    import torch.d
+00027410: 6973 7472 6962 7574 696f 6e73 2061 7320  istributions as 
+00027420: 6469 7374 0a20 2020 2020 2020 2067 6175  dist.        gau
+00027430: 7373 6961 6e5f 6d65 6d62 6572 7368 6970  ssian_membership
+00027440: 733a 204c 6973 745b 5475 706c 655b 666c  s: List[Tuple[fl
+00027450: 6f61 742c 2066 6c6f 6174 5d5d 203d 205b  oat, float]] = [
+00027460: 282d 312e 3634 352c 2030 2e32 3833 292c  (-1.645, 0.283),
+00027470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00027480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027490: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000274a0: 2020 2020 2020 2020 2020 2020 282d 312e              (-1.
+000274b0: 3038 302c 2030 2e31 3730 292c 0a20 2020  080, 0.170),.   
+000274c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000274d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000274e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000274f0: 2020 2020 2020 2020 282d 302e 3733 392c          (-0.739,
+00027500: 2030 2e31 3334 292c 0a20 2020 2020 2020   0.134),.       
+00027510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027530: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027540: 2020 2020 282d 302e 3436 382c 2030 2e31      (-0.468, 0.1
+00027550: 3138 292c 0a20 2020 2020 2020 2020 2020  18),.           
+00027560: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027590: 282d 302e 3232 382c 2030 2e31 3134 292c  (-0.228, 0.114),
+000275a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000275b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000275c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000275d0: 2020 2020 2020 2020 2020 2020 2830 2e2c              (0.,
+000275e0: 2030 2e31 3134 292c 0a20 2020 2020 2020   0.114),.       
+000275f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027620: 2020 2020 2830 2e32 3238 2c20 302e 3131      (0.228, 0.11
+00027630: 3429 2c0a 2020 2020 2020 2020 2020 2020  4),.            
+00027640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027660: 2020 2020 2020 2020 2020 2020 2020 2028                 (
+00027670: 302e 3436 382c 2030 2e31 3138 292c 0a20  0.468, 0.118),. 
+00027680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000276a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000276b0: 2020 2020 2020 2020 2020 2830 2e37 3339            (0.739
+000276c0: 2c20 302e 3133 3429 2c0a 2020 2020 2020  , 0.134),.      
+000276d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000276e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000276f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027700: 2020 2020 2028 312e 3038 302c 2030 2e31       (1.080, 0.1
+00027710: 3730 292c 0a20 2020 2020 2020 2020 2020  70),.           
+00027720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00027750: 2831 2e36 3435 2c20 302e 3238 3329 5d0a  (1.645, 0.283)].
+00027760: 0a20 2020 2020 2020 2064 6973 7472 6962  .        distrib
+00027770: 7574 696f 6e73 3a20 4c69 7374 5b64 6973  utions: List[dis
+00027780: 742e 4e6f 726d 616c 5d20 3d20 5b0a 2020  t.Normal] = [.  
+00027790: 2020 2020 2020 2020 2020 6469 7374 2e4e            dist.N
+000277a0: 6f72 6d61 6c28 746f 7263 682e 7465 6e73  ormal(torch.tens
+000277b0: 6f72 2870 5b30 5d29 2c20 746f 7263 682e  or(p[0]), torch.
+000277c0: 7465 6e73 6f72 2870 5b31 5d29 290a 2020  tensor(p[1])).  
+000277d0: 2020 2020 2020 2020 2020 666f 7220 7020            for p 
+000277e0: 696e 2067 6175 7373 6961 6e5f 6d65 6d62  in gaussian_memb
+000277f0: 6572 7368 6970 730a 2020 2020 2020 2020  erships.        
+00027800: 5d0a 2020 2020 2020 2020 6469 7374 5f6d  ].        dist_m
+00027810: 6178 3a20 4c69 7374 5b74 6f72 6368 2e54  ax: List[torch.T
+00027820: 656e 736f 725d 203d 205b 0a20 2020 2020  ensor] = [.     
+00027830: 2020 2020 2020 2064 6973 7472 6962 7574         distribut
+00027840: 696f 6e73 5b69 5d2e 6c6f 675f 7072 6f62  ions[i].log_prob
+00027850: 2874 6f72 6368 2e74 656e 736f 7228 0a20  (torch.tensor(. 
+00027860: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00027870: 6175 7373 6961 6e5f 6d65 6d62 6572 7368  aussian_membersh
+00027880: 6970 735b 695d 5b30 5d29 292e 6578 7028  ips[i][0])).exp(
+00027890: 2920 666f 7220 6920 696e 2072 616e 6765  ) for i in range
+000278a0: 2831 3129 0a20 2020 2020 2020 205d 0a0a  (11).        ]..
+000278b0: 2020 2020 2020 2020 6f75 7470 7574 733a          outputs:
+000278c0: 204c 6973 745b 746f 7263 682e 5465 6e73   List[torch.Tens
+000278d0: 6f72 5d20 3d20 5b0a 2020 2020 2020 2020  or] = [.        
+000278e0: 2020 2020 6469 7374 7269 6275 7469 6f6e      distribution
+000278f0: 735b 695d 2e6c 6f67 5f70 726f 6228 746f  s[i].log_prob(to
+00027900: 7263 682e 7465 6e73 6f72 2878 2929 2e65  rch.tensor(x)).e
+00027910: 7870 2829 202f 2064 6973 745f 6d61 785b  xp() / dist_max[
+00027920: 695d 0a20 2020 2020 2020 2020 2020 2066  i].            f
+00027930: 6f72 2069 2069 6e20 7261 6e67 6528 3131  or i in range(11
+00027940: 290a 2020 2020 2020 2020 5d0a 2020 2020  ).        ].    
+00027950: 2020 2020 6f75 7470 7574 3a20 746f 7263      output: torc
+00027960: 682e 5465 6e73 6f72 203d 2074 6f72 6368  h.Tensor = torch
+00027970: 2e73 7461 636b 286f 7574 7075 7473 2c20  .stack(outputs, 
+00027980: 6469 6d3d 3229 0a20 2020 2020 2020 206f  dim=2).        o
+00027990: 7574 7075 7420 3d20 6f75 7470 7574 202f  utput = output /
+000279a0: 2074 6f72 6368 2e73 756d 286f 7574 7075   torch.sum(outpu
+000279b0: 742c 2064 696d 3d32 2c20 6b65 6570 6469  t, dim=2, keepdi
+000279c0: 6d3d 5472 7565 290a 2020 2020 2020 2020  m=True).        
+000279d0: 6f75 7470 7574 203d 206f 7574 7075 742e  output = output.
+000279e0: 7669 6577 282d 312c 2073 656c 662e 6e5f  view(-1, self.n_
+000279f0: 696e 7075 7420 2a20 3131 290a 2020 2020  input * 11).    
+00027a00: 2020 2020 7265 7475 726e 206f 7574 7075      return outpu
+00027a10: 740a                                     t.
```

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/lcnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/lcnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/mat.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/mat.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/megnet.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/megnet.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/modular.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/modular.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/mpnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/mpnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/normalizing_flows_pytorch.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/normalizing_flows_pytorch.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/pagtn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/pagtn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/pna_gnn.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/pna_gnn.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/readout.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/readout.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/torch_models/torch_model.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/torch_models/torch_model.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/models/wandblogger.py` & `deepchem-2.7.2.dev20230717161942/deepchem/models/wandblogger.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/check_availability.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/check_availability.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/defaults.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/defaults.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/dnasim.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/dnasim.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bace_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bace_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bace_features.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bace_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bbbc_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bbbc_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/bbbp_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/bbbp_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/cell_counting_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/cell_counting_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl25_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl25_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/chembl_tasks.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/chembl_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/clearance_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/clearance_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/clintox_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/clintox_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/delaney_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/delaney_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/factors_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/factors_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/freesolv_dataset.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/freesolv_dataset.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hiv_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hiv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hopv_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hopv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/hppb_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/hppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kaggle_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kaggle_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kaggle_features.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kaggle_features.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/kinase_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/kinase_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/lipo_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/lipo_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/load_dataset_template.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/load_dataset_template.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_Pt_NO_surface_adsorbate_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_bandgap.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_bandgap.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_mp_formation_energy.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_mp_metallicity.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/material_datasets/load_perovskite.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/material_datasets/load_perovskite.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/molnet_loader.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/molnet_loader.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/muv_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/muv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/nci_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/nci_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/pcba_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/pcba_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/pdbbind_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/pdbbind_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/ppb_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/ppb_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm7_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm7_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm8_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm8_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/qm9_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/qm9_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sampl_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sampl_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sider_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sider_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/sweetlead_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/sweetlead_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/thermosol_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/thermosol_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/tox21_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/tox21_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/toxcast_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/toxcast_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uspto_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uspto_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uv_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uv_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/uv_tasks.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/uv_tasks.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/load_function/zinc15_datasets.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/load_function/zinc15_datasets.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/preset_hyper_parameters.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/preset_hyper_parameters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark_low_data.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark_low_data.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/molnet/run_benchmark_models.py` & `deepchem-2.7.2.dev20230717161942/deepchem/molnet/run_benchmark_models.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/rl/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/rl/a2c.py` & `deepchem-2.7.2.dev20230717161942/deepchem/rl/a2c.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/test_tictactoe.py` & `deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/test_tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/rl/envs/tictactoe.py` & `deepchem-2.7.2.dev20230717161942/deepchem/rl/envs/tictactoe.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/rl/ppo.py` & `deepchem-2.7.2.dev20230717161942/deepchem/rl/ppo.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/splits/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/splits/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/splits/splitters.py` & `deepchem-2.7.2.dev20230717161942/deepchem/splits/splitters.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/splits/task_splitter.py` & `deepchem-2.7.2.dev20230717161942/deepchem/splits/task_splitter.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/trans/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/trans/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/trans/duplicate.py` & `deepchem-2.7.2.dev20230717161942/deepchem/trans/duplicate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/trans/transformers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/trans/transformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/__init__.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/conformers.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/conformers.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/coordinate_box_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/data_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/debug_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/debug_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/dftutils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/docking_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/electron_sampler.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/evaluate.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/fake_data_generator.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/fragment_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/genomics_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/geometry_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/graph_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/grover.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/hash_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/molecule_feature_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/noncovalent_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/pdbqt_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/pytorch_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/rdkit_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/save.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/save.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/sequence_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_coordinate_box_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_coordinate_box_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_data_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_data_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_dftutils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_dftutils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_docking_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_docking_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_electron_sampler.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_electron_sampler.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_evaluate.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_evaluate.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_fake_data_generator.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_fake_data_generator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_fragment_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_fragment_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_generator_evaluator.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_generator_evaluator.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_genomics_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_genomics_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_geometry_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_geometry_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_graph_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_graph_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_grover.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_grover.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_hash_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_hash_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_molecule_feature_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_molecule_feature_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_noncovalent_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_noncovalent_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_pdbqt_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_pdbqt_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_pytorch_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_pytorch_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_rdkit_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_rdkit_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_sequence_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_sequence_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/test/test_voxel_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/test/test_voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/typing.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/vina_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/vina_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem/utils/voxel_utils.py` & `deepchem-2.7.2.dev20230717161942/deepchem/utils/voxel_utils.py`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem.egg-info/PKG-INFO` & `deepchem-2.7.2.dev20230717161942/deepchem.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepchem
-Version: 2.7.2.dev20230712172748
+Version: 2.7.2.dev20230717161942
 Summary: Deep learning models for drug discovery,         quantum chemistry, and the life sciences.
 Home-page: https://github.com/deepchem/deepchem
 Maintainer: DeepChem contributors
 License: MIT
 Project-URL: Documentation, https://deepchem.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/deepchem/deepchem
 Keywords: deepchem,chemistry,biology,materials-science,life-science,drug-discovery
```

### Comparing `deepchem-2.7.2.dev20230712172748/deepchem.egg-info/SOURCES.txt` & `deepchem-2.7.2.dev20230717161942/deepchem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/setup.cfg` & `deepchem-2.7.2.dev20230717161942/setup.cfg`

 * *Files identical despite different names*

### Comparing `deepchem-2.7.2.dev20230712172748/setup.py` & `deepchem-2.7.2.dev20230717161942/setup.py`

 * *Files identical despite different names*

