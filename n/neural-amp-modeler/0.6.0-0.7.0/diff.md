# Comparing `tmp/neural-amp-modeler-0.6.0.tar.gz` & `tmp/neural-amp-modeler-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural-amp-modeler-0.6.0.tar", last modified: Mon Jun 12 04:38:05 2023, max compression
+gzip compressed data, was "neural-amp-modeler-0.7.0.tar", last modified: Mon Jul 17 03:45:30 2023, max compression
```

## Comparing `neural-amp-modeler-0.6.0.tar` & `neural-amp-modeler-0.7.0.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.025730 neural-amp-modeler-0.6.0/
--rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.6.0/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-06-12 04:38:05.025209 neural-amp-modeler-0.6.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     4536 2023-06-12 04:35:43.000000 neural-amp-modeler-0.6.0/README.md
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.970623 neural-amp-modeler-0.6.0/nam/
--rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.6.0/nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.6.0/nam/_core.py
--rw-r--r--   0 steve      (501) staff       (20)       22 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/_version.py
--rw-r--r--   0 steve      (501) staff       (20)    25028 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/nam/data.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.984008 neural-amp-modeler-0.6.0/nam/models/
--rw-r--r--   0 steve      (501) staff       (20)      372 2023-05-20 03:46:31.000000 neural-amp-modeler-0.6.0/nam/models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/_activations.py
--rw-r--r--   0 steve      (501) staff       (20)     5326 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/models/_base.py
--rw-r--r--   0 steve      (501) staff       (20)     4816 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/nam/models/_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/_names.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.985183 neural-amp-modeler-0.6.0/nam/models/_resources/
--rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.6.0/nam/models/_resources/loudness_input.wav
--rw-r--r--   0 steve      (501) staff       (20)    13555 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     9052 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1952 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/linear.py
--rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/models/losses.py
--rw-r--r--   0 steve      (501) staff       (20)     1187 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/models/metadata.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.992068 neural-amp-modeler-0.6.0/nam/models/parametric/
--rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/parametric/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/nam/models/parametric/catnets.py
--rw-r--r--   0 steve      (501) staff       (20)    18233 2023-05-20 03:46:31.000000 neural-amp-modeler-0.6.0/nam/models/parametric/hyper_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/models/parametric/params.py
--rw-r--r--   0 steve      (501) staff       (20)    16232 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/nam/models/recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)    13909 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/nam/models/wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:04.997691 neural-amp-modeler-0.6.0/nam/train/
--rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/nam/train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      852 2023-05-17 02:24:00.000000 neural-amp-modeler-0.6.0/nam/train/_version.py
--rw-r--r--   0 steve      (501) staff       (20)     3911 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/train/colab.py
--rw-r--r--   0 steve      (501) staff       (20)    30769 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/nam/train/core.py
--rw-r--r--   0 steve      (501) staff       (20)    21047 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/nam/train/gui.py
--rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-29 18:46:19.000000 neural-amp-modeler-0.6.0/nam/util.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.003270 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)      211 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)     1793 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)       42 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/entry_points.txt
--rw-r--r--   0 steve      (501) staff       (20)      114 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)       10 2023-06-12 04:38:04.000000 neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/top_level.txt
--rw-r--r--   0 steve      (501) staff       (20)       38 2023-06-12 04:38:05.025895 neural-amp-modeler-0.6.0/setup.cfg
--rw-r--r--   0 steve      (501) staff       (20)      977 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/setup.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.004405 neural-amp-modeler-0.6.0/tests/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.005306 neural-amp-modeler-0.6.0/tests/resources/
--rw-r--r--   0 steve      (501) staff       (20)      676 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/resources/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.006443 neural-amp-modeler-0.6.0/tests/test_bin/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.6.0/tests/test_bin/__init__.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.007316 neural-amp-modeler-0.6.0/tests/test_bin/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.6.0/tests/test_bin/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     6583 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/test_bin/test_train/test_main.py
--rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_install.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.010116 neural-amp-modeler-0.6.0/tests/test_nam/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)    10062 2023-06-12 04:30:52.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_data.py
--rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_importable.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.017716 neural-amp-modeler-0.6.0/tests/test_nam/test_models/
--rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/base.py
--rw-r--r--   0 steve      (501) staff       (20)     2754 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_base.py
--rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_conv_net.py
--rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_exportable.py
--rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_losses.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.020831 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/
--rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     1218 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_catnets.py
--rw-r--r--   0 steve      (501) staff       (20)     2474 2022-12-20 07:51:29.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_hyper_net.py
--rw-r--r--   0 steve      (501) staff       (20)     1951 2023-04-10 01:24:24.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_recurrent.py
--rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_wavenet.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-06-12 04:38:05.023909 neural-amp-modeler-0.6.0/tests/test_nam/test_train/
--rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)     4535 2023-05-28 20:20:41.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_core.py
--rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_version.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.574165 neural-amp-modeler-0.7.0/
+-rw-r--r--   0 steve      (501) staff       (20)     1072 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       49 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.0/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-17 03:45:30.573726 neural-amp-modeler-0.7.0/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     4536 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/README.md
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.522248 neural-amp-modeler-0.7.0/nam/
+-rw-r--r--   0 steve      (501) staff       (20)      729 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.0/nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      362 2023-03-18 16:36:25.000000 neural-amp-modeler-0.7.0/nam/_core.py
+-rw-r--r--   0 steve      (501) staff       (20)       22 2023-06-20 00:48:33.000000 neural-amp-modeler-0.7.0/nam/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)    25956 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/nam/data.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.534211 neural-amp-modeler-0.7.0/nam/models/
+-rw-r--r--   0 steve      (501) staff       (20)      372 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.0/nam/models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      209 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.0/nam/models/_activations.py
+-rw-r--r--   0 steve      (501) staff       (20)     5964 2023-06-25 16:27:08.000000 neural-amp-modeler-0.7.0/nam/models/_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     4816 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/nam/models/_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/nam/models/_names.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.534959 neural-amp-modeler-0.7.0/nam/models/_resources/
+-rw-r--r--   0 steve      (501) staff       (20)   144044 2023-04-01 05:02:40.000000 neural-amp-modeler-0.7.0/nam/models/_resources/loudness_input.wav
+-rw-r--r--   0 steve      (501) staff       (20)    13555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.0/nam/models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     9120 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/nam/models/conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1984 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/nam/models/linear.py
+-rw-r--r--   0 steve      (501) staff       (20)     2440 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.0/nam/models/losses.py
+-rw-r--r--   0 steve      (501) staff       (20)     1187 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.0/nam/models/metadata.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.541643 neural-amp-modeler-0.7.0/nam/models/parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.0/nam/models/parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6572 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.0/nam/models/parametric/catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)    18233 2023-05-20 03:46:31.000000 neural-amp-modeler-0.7.0/nam/models/parametric/hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     1521 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/nam/models/parametric/params.py
+-rw-r--r--   0 steve      (501) staff       (20)    16557 2023-06-25 16:29:54.000000 neural-amp-modeler-0.7.0/nam/models/recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)    13969 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/nam/models/wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.547897 neural-amp-modeler-0.7.0/nam/train/
+-rw-r--r--   0 steve      (501) staff       (20)      108 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/nam/train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      852 2023-05-17 02:24:00.000000 neural-amp-modeler-0.7.0/nam/train/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)     3911 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.0/nam/train/colab.py
+-rw-r--r--   0 steve      (501) staff       (20)    32555 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.0/nam/train/core.py
+-rw-r--r--   0 steve      (501) staff       (20)    21047 2023-06-22 07:01:43.000000 neural-amp-modeler-0.7.0/nam/train/gui.py
+-rw-r--r--   0 steve      (501) staff       (20)      307 2023-04-29 18:46:19.000000 neural-amp-modeler-0.7.0/nam/util.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.552898 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)      211 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)     1793 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)       42 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/entry_points.txt
+-rw-r--r--   0 steve      (501) staff       (20)      114 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)       10 2023-07-17 03:45:30.000000 neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/top_level.txt
+-rw-r--r--   0 steve      (501) staff       (20)       38 2023-07-17 03:45:30.574361 neural-amp-modeler-0.7.0/setup.cfg
+-rw-r--r--   0 steve      (501) staff       (20)      977 2023-06-12 04:30:52.000000 neural-amp-modeler-0.7.0/setup.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.554015 neural-amp-modeler-0.7.0/tests/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.0/tests/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.555010 neural-amp-modeler-0.7.0/tests/resources/
+-rw-r--r--   0 steve      (501) staff       (20)      676 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.0/tests/resources/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.556193 neural-amp-modeler-0.7.0/tests/test_bin/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.0/tests/test_bin/__init__.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.557218 neural-amp-modeler-0.7.0/tests/test_bin/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-30 18:53:40.000000 neural-amp-modeler-0.7.0/tests/test_bin/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     6583 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.0/tests/test_bin/test_train/test_main.py
+-rw-r--r--   0 steve      (501) staff       (20)      237 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_install.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.559801 neural-amp-modeler-0.7.0/tests/test_nam/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)    10343 2023-06-22 07:13:06.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_data.py
+-rw-r--r--   0 steve      (501) staff       (20)      231 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_importable.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.567589 neural-amp-modeler-0.7.0/tests/test_nam/test_models/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      988 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/base.py
+-rw-r--r--   0 steve      (501) staff       (20)     2754 2023-06-25 16:12:51.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_base.py
+-rw-r--r--   0 steve      (501) staff       (20)     1061 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_conv_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     4588 2023-04-25 01:51:12.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_exportable.py
+-rw-r--r--   0 steve      (501) staff       (20)     1727 2023-06-03 04:33:38.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_losses.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.570322 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/
+-rw-r--r--   0 steve      (501) staff       (20)      105 2023-04-10 01:24:24.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     1218 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/test_catnets.py
+-rw-r--r--   0 steve      (501) staff       (20)     2474 2022-12-20 07:51:29.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/test_hyper_net.py
+-rw-r--r--   0 steve      (501) staff       (20)     2360 2023-06-20 00:48:33.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_recurrent.py
+-rw-r--r--   0 steve      (501) staff       (20)      817 2023-05-07 19:58:11.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_wavenet.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2023-07-17 03:45:30.572646 neural-amp-modeler-0.7.0/tests/test_nam/test_train/
+-rw-r--r--   0 steve      (501) staff       (20)        0 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_train/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)     4535 2023-05-28 20:20:41.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_train/test_core.py
+-rw-r--r--   0 steve      (501) staff       (20)      773 2023-04-29 20:17:32.000000 neural-amp-modeler-0.7.0/tests/test_nam/test_train/test_version.py
```

### Comparing `neural-amp-modeler-0.6.0/LICENSE` & `neural-amp-modeler-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/README.md` & `neural-amp-modeler-0.7.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ## How to use (Google Colab)
 
 If you don't have a good computer for training ML models, you use Google Colab to train
 in the cloud using the pre-made notebooks under `bin\train`.
 
 For the very easiest experience, open 
-[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/f67f17b/bin/train/easy_colab.ipynb) 
+[`easy_colab.ipynb` on Google Colab](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/2992b47/bin/train/easy_colab.ipynb) 
 and follow the steps!
 
 For a little more visibility under the hood, you can use [colab.ipynb](https://colab.research.google.com/github/sdatkinson/neural-amp-modeler/blob/main/bin/train/colab.ipynb) instead.
 
 **Pros:**
 
 - No local installation required!
```

### Comparing `neural-amp-modeler-0.6.0/nam/__init__.py` & `neural-amp-modeler-0.7.0/nam/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/data.py` & `neural-amp-modeler-0.7.0/nam/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # File: data.py
 # Created Date: Saturday February 5th 2022
 # Author: Steven Atkinson (steven@atkinson.mn)
 
 import abc
+import logging
 from collections import namedtuple
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import Dict, Optional, Sequence, Tuple, Union
 
@@ -15,14 +16,16 @@
 import wavio
 from scipy.interpolate import interp1d
 from torch.utils.data import Dataset as _Dataset
 from tqdm import tqdm
 
 from ._core import InitializableFromConfig
 
+logger = logging.getLogger(__name__)
+
 _REQUIRED_SAMPWIDTH = 3
 REQUIRED_RATE = 48_000
 _REQUIRED_CHANNELS = 1  # Mono
 
 
 class Split(Enum):
     TRAIN = "train"
@@ -90,15 +93,15 @@
     arr_premono = x_wav.data[preroll:] / (2.0 ** (8 * x_wav.sampwidth - 1))
     if required_shape is not None:
         if arr_premono.shape != required_shape:
             raise AudioShapeMismatchError(
                 required_shape,  # Expected
                 arr_premono.shape,  # Actual
                 f"Mismatched shapes. Expected {required_shape}, but this is "
-                f"{arr_premono.shape}!"
+                f"{arr_premono.shape}!",
             )
         # sampwidth fine--we're just casting to 32-bit float anyways
     arr = arr_premono[:, 0]
     return arr if not info else (arr, WavInfo(x_wav.sampwidth, x_wav.rate))
 
 
 def wav_to_tensor(
@@ -118,26 +121,26 @@
 
 
 def np_to_wav(
     x: np.ndarray,
     filename: Union[str, Path],
     rate: int = 48_000,
     sampwidth: int = 3,
-    scale = None,
-    **kwargs
+    scale=None,
+    **kwargs,
 ):
     if wavio.__version__ <= "0.0.4" and scale is None:
         scale = "none"
     wavio.write(
         str(filename),
         (np.clip(x, -1.0, 1.0) * (2 ** (8 * sampwidth - 1))).astype(np.int32),
         rate,
         scale=scale,
         sampwidth=sampwidth,
-        **kwargs
+        **kwargs,
     )
 
 
 class AbstractDataset(_Dataset, abc.ABC):
     @abc.abstractmethod
     def __getitem__(
         self, idx: int
@@ -231,15 +234,16 @@
         delay_interpolation_method: Union[
             str, _DelayInterpolationMethod
         ] = _DelayInterpolationMethod.CUBIC,
         y_scale: float = 1.0,
         x_path: Optional[Union[str, Path]] = None,
         y_path: Optional[Union[str, Path]] = None,
         input_gain: float = 0.0,
-        rate: int = REQUIRED_RATE,
+        sample_rate: Optional[int] = None,
+        rate: Optional[int] = None,
         require_input_pre_silence: Optional[float] = _DEFAULT_REQUIRE_INPUT_PRE_SILENCE,
     ):
         """
         :param x: The input signal. A 1D array.
         :param y: The associated output from the model. A 1D array.
         :param nx: The number of samples required as input for the model. For example,
             for a ConvNet, this would be the receptive field.
@@ -268,36 +272,36 @@
         :param require_input_pre_silence: If provided, require that this much time (in
             seconds) preceding the start of the data set (`start`) have a silent input.
             If it's not, then raise an exception because the output due to it will leak
             into the data set that we're trying to use. If `None`, don't assert.
         """
         self._validate_x_y(x, y)
         self._validate_start_stop(x, y, start, stop)
+        self._sample_rate = self._validate_sample_rate(sample_rate, rate)
         if not isinstance(delay_interpolation_method, _DelayInterpolationMethod):
             delay_interpolation_method = _DelayInterpolationMethod(
                 delay_interpolation_method
             )
         if require_input_pre_silence is not None:
             self._validate_preceding_silence(
-                x, start, int(require_input_pre_silence * rate)
+                x, start, int(require_input_pre_silence * self._sample_rate)
             )
         x, y = [z[start:stop] for z in (x, y)]
         if delay is not None and delay != 0:
             x, y = self._apply_delay(x, y, delay, delay_interpolation_method)
         x_scale = 10.0 ** (input_gain / 20.0)
         x = x * x_scale
         y = y * y_scale
         self._x_path = x_path
         self._y_path = y_path
         self._validate_inputs_after_processing(x, y, nx, ny)
         self._x = x
         self._y = y
         self._nx = nx
         self._ny = ny if ny is not None else len(x) - nx + 1
-        self._rate = rate
 
     def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         :return:
             Input (NX+NY-1,)
             Output (NY,)
         """
@@ -314,14 +318,18 @@
         return single_pairs // self._ny
 
     @property
     def ny(self) -> int:
         return self._ny
 
     @property
+    def sample_rate(self) -> Optional[float]:
+        return self._sample_rate
+
+    @property
     def x(self) -> torch.Tensor:
         """
         The input audio data
 
         :return: (N,)
         """
         return self._x
@@ -441,14 +449,33 @@
             x = x[:n_out]
         elif delay < 0:
             x = x[-n_out:]
         y = _interpolate_delay(y, delay, method)
         return x, y
 
     @classmethod
+    def _validate_sample_rate(
+        cls, sample_rate: Optional[float], rate: Optional[int]
+    ) -> float:
+        if sample_rate is None and rate is None:  # Default value
+            return REQUIRED_RATE
+        if rate is not None:
+            if sample_rate is not None:
+                raise ValueError(
+                    "Provided both sample_rate and rate. Provide only sample_rate!"
+                )
+            else:
+                logger.warning(
+                    "Use of 'rate' is deprecated and will be removed. Use sample_rate instead"
+                )
+                return float(rate)
+        else:
+            return sample_rate
+
+    @classmethod
     def _validate_start_stop(
         self,
         x: torch.Tensor,
         y: torch.Tensor,
         start: Optional[int] = None,
         stop: Optional[int] = None,
     ):
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/_base.py` & `neural-amp-modeler-0.7.0/nam/models/_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,18 @@
 
 from .._core import InitializableFromConfig
 from ..data import REQUIRED_RATE, wav_to_tensor
 from ._exportable import Exportable
 
 
 class _Base(nn.Module, InitializableFromConfig, Exportable):
+    def __init__(self, sample_rate: Optional[float] = None):
+        super().__init__()
+        self.sample_rate = sample_rate
+
     @abc.abstractproperty
     def pad_start_default(self) -> bool:
         pass
 
     @abc.abstractproperty
     def receptive_field(self) -> int:
         """
@@ -33,26 +37,41 @@
         """
         pass
 
     @abc.abstractmethod
     def forward(self, *args, **kwargs) -> torch.Tensor:
         pass
 
+    @classmethod
+    def _metadata_loudness_x(cls) -> torch.Tensor:
+        return wav_to_tensor(
+            pkg_resources.resource_filename(
+                "nam", "models/_resources/loudness_input.wav"
+            )
+        )
+
+    def _get_export_dict(self):
+        d = super()._get_export_dict()
+        sample_rate_key = "sample_rate"
+        if sample_rate_key in d:
+            raise RuntimeError(
+                "Model wants to put 'sample_rate' into model export dict, but the key "
+                "is already taken!"
+            )
+        d[sample_rate_key] = self.sample_rate
+        return d
+
     def _metadata_loudness(self, gain: float = 1.0, db: bool = True) -> float:
         """
         How loud is this model when given a standardized input?
         In dB
 
         :param gain: Multiplies input signal
         """
-        x = wav_to_tensor(
-            pkg_resources.resource_filename(
-                "nam", "models/_resources/loudness_input.wav"
-            )
-        )
+        x = self._metadata_loudness_x()
         y = self._at_nominal_settings(gain * x)
         loudness = torch.sqrt(torch.mean(torch.square(y)))
         if db:
             loudness = 20.0 * torch.log10(loudness)
         return loudness.item()
 
     def _metadata_gain(self) -> float:
@@ -115,22 +134,22 @@
         return (
             x.detach().cpu().numpy(),
             self(*args, x, pad_start=True).detach().cpu().numpy(),
         )
 
 
 class BaseNet(_Base):
-    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None):
+    def forward(self, x: torch.Tensor, pad_start: Optional[bool] = None, **kwargs):
         pad_start = self.pad_start_default if pad_start is None else pad_start
         scalar = x.ndim == 1
         if scalar:
             x = x[None]
         if pad_start:
             x = torch.cat((torch.zeros((len(x), self.receptive_field - 1)), x), dim=1)
-        y = self._forward(x)
+        y = self._forward(x, **kwargs)
         if scalar:
             y = y[0]
         return y
 
     def _at_nominal_settings(self, x: torch.Tensor) -> torch.Tensor:
         return self(x)
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/_exportable.py` & `neural-amp-modeler-0.7.0/nam/models/_exportable.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from ..data import np_to_wav
 from .metadata import Date, UserMetadata
 
 logger = logging.getLogger(__name__)
 
 # Model version is independent from package version as of package version 0.5.2 so that
 # the API of the package can iterate at a different pace from that of the model files.
-_MODEL_VERSION = "0.5.1"
+_MODEL_VERSION = "0.5.2"
 
 
 def _cast_enums(d: Dict[Any, Any]) -> Dict[Any, Any]:
     """
     Casts enum-type keys to their values
     """
     out = {}
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/_resources/loudness_input.wav` & `neural-amp-modeler-0.7.0/nam/models/_resources/loudness_input.wav`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/base.py` & `neural-amp-modeler-0.7.0/nam/models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/conv_net.py` & `neural-amp-modeler-0.7.0/nam/models/conv_net.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,17 +106,18 @@
     """
 
     def __init__(
         self,
         *args,
         train_strategy: TrainStrategy = default_train_strategy,
         ir: Optional[_IR] = None,
+        sample_rate: Optional[float] = None,
         **kwargs,
     ):
-        super().__init__()
+        super().__init__(sample_rate=sample_rate)
         self._net = _conv_net(*args, **kwargs)
         assert train_strategy == TrainStrategy.DILATE, "Stride no longer supported"
         self._train_strategy = train_strategy
         self._num_blocks = self._get_num_blocks(self._net)
         self._pad_start_default = True
         self._ir = ir
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/linear.py` & `neural-amp-modeler-0.7.0/nam/models/linear.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 import torch.nn as nn
 
 from .._version import __version__
 from ._base import BaseNet
 
 
 class Linear(BaseNet):
-    def __init__(self, receptive_field: int, bias: bool = False):
-        super().__init__()
+    def __init__(self, receptive_field: int, *args, bias: bool = False, **kwargs):
+        super().__init__(*args, **kwargs)
         self._net = nn.Conv1d(1, 1, receptive_field, bias=bias)
 
     @property
     def pad_start_default(self) -> bool:
         return True
 
     @property
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/losses.py` & `neural-amp-modeler-0.7.0/nam/models/losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/metadata.py` & `neural-amp-modeler-0.7.0/nam/models/metadata.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/parametric/catnets.py` & `neural-amp-modeler-0.7.0/nam/models/parametric/catnets.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/parametric/hyper_net.py` & `neural-amp-modeler-0.7.0/nam/models/parametric/hyper_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/parametric/params.py` & `neural-amp-modeler-0.7.0/nam/models/parametric/params.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/models/recurrent.py` & `neural-amp-modeler-0.7.0/nam/models/recurrent.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,41 +127,43 @@
 
     def __init__(
         self,
         hidden_size,
         train_burn_in: Optional[int] = None,
         train_truncate: Optional[int] = None,
         input_size: int = 1,
+        sample_rate: Optional[float] = None,
         **lstm_kwargs,
     ):
         """
         :param hidden_size: for LSTM
         :param train_burn_in: Detach calculations from first (this many) samples when
             training to burn in the hidden state.
         :param train_truncate: detach the hidden & cell states every this many steps
             during training so that backpropagation through time is faster + to simulate
             better starting states for h(t0)&c(t0) (instead of zeros)
             TODO recognition head to start the hidden state in a good place?
         :param input_size: Usually 1 (mono input). A catnet extending this might change
             it and provide the parametric inputs as additional input dimensions.
         """
-        super().__init__()
+        super().__init__(sample_rate=sample_rate)
         if "batch_first" in lstm_kwargs:
             raise ValueError("batch_first cannot be set.")
         self._input_size = input_size
         self._core = _L(self._input_size, hidden_size, batch_first=True, **lstm_kwargs)
         self._head = nn.Linear(hidden_size, 1)
         self._train_burn_in = train_burn_in
         self._train_truncate = train_truncate
         self._initial_cell = nn.Parameter(
             torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
         )
         self._initial_hidden = nn.Parameter(
             torch.zeros((lstm_kwargs.get("num_layers", 1), hidden_size))
         )
+        self._get_initial_state_burn_in = 48_000
 
     @property
     def receptive_field(self) -> int:
         return 1
 
     @property
     def pad_start_default(self) -> bool:
@@ -237,20 +239,24 @@
     def _apply_head(self, features: torch.Tensor) -> torch.Tensor:
         """
         :param features: (B,S,DH)
         :return: (B,S)
         """
         return self._head(features)[:, :, 0]
 
-    def _forward(self, x: torch.Tensor) -> torch.Tensor:
+    def _forward(
+        self, x: torch.Tensor, initial_state: Optional[_LSTMHiddenCellType] = None
+    ) -> torch.Tensor:
         """
         :param x: (B,L) or (B,L,D)
         :return: (B,L)
         """
-        last_hidden_state = self._initial_state(len(x))
+        last_hidden_state = (
+            self._initial_state(len(x)) if initial_state is None else initial_state
+        )
         if x.ndim == 2:
             x = x[:, :, None]
         if not self.training or self._train_truncate is None:
             output_features = self._core(x, last_hidden_state)[0]
         else:
             output_features_list = []
             if self._train_burn_in is not None:
@@ -336,15 +342,19 @@
         DX=input size
         L=num layers
         S=sequence length
         :param inputs: (1,S,DX)
 
         :return: (L,DH), (L,DH)
         """
-        inputs = torch.zeros((1, 48_000, 1)) if inputs is None else inputs
+        inputs = (
+            torch.zeros((1, self._get_initial_state_burn_in, 1))
+            if inputs is None
+            else inputs
+        )
         _, (h, c) = self._core(inputs)
         return h, c
 
     def _initial_state(self, n: Optional[int]) -> _LSTMHiddenCellType:
         """
         Literally what the forward pass starts with.
         Default is zeroes; this should be better since it can be learned.
```

### Comparing `neural-amp-modeler-0.6.0/nam/models/wavenet.py` & `neural-amp-modeler-0.7.0/nam/models/wavenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -335,16 +335,16 @@
         for layer in self._layers:
             head_input, y = layer(y, x, head_input=head_input)
         head_input = self._head_scale * head_input
         return head_input if self._head is None else self._head(head_input)
 
 
 class WaveNet(BaseNet):
-    def __init__(self, *args, **kwargs):
-        super().__init__()
+    def __init__(self, *args, sample_rate: Optional[float] = None, **kwargs):
+        super().__init__(sample_rate=sample_rate)
         self._net = _WaveNet(*args, **kwargs)
 
     @property
     def pad_start_default(self) -> bool:
         return True
 
     @property
```

### Comparing `neural-amp-modeler-0.6.0/nam/train/_version.py` & `neural-amp-modeler-0.7.0/nam/train/_version.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/train/colab.py` & `neural-amp-modeler-0.7.0/nam/train/colab.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/nam/train/core.py` & `neural-amp-modeler-0.7.0/nam/train/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from ._version import Version
 
 
 class Architecture(Enum):
     STANDARD = "standard"
     LITE = "lite"
     FEATHER = "feather"
+    NANO = "nano"
 
 
 def _detect_input_version(input_path) -> Tuple[Version, bool]:
     """
     Check to see if the input matches any of the known inputs
 
     :return: version, strong match
@@ -341,27 +342,33 @@
         plot(delay, input_path, output_path)
     return delay
 
 
 def _get_lstm_config(architecture):
     return {
         Architecture.STANDARD: {
-            "num_layers": 3,
+            "num_layers": 1,
             "hidden_size": 24,
             "train_burn_in": 4096,
             "train_truncate": 512,
         },
         Architecture.LITE: {
             "num_layers": 2,
-            "hidden_size": 16,
+            "hidden_size": 8,
             "train_burn_in": 4096,
             "train_truncate": 512,
         },
         Architecture.FEATHER: {
             "num_layers": 1,
+            "hidden_size": 16,
+            "train_burn_in": 4096,
+            "train_truncate": 512,
+        },
+        Architecture.NANO: {
+            "num_layers": 1,
             "hidden_size": 12,
             "train_burn_in": 4096,
             "train_truncate": 512,
         },
     }[architecture]
 
 
@@ -560,14 +567,41 @@
                     "activation": "Tanh",
                     "gated": False,
                     "head_bias": True,
                 },
             ],
             "head_scale": 0.02,
         },
+        Architecture.NANO: {
+            "layers_configs": [
+                {
+                    "input_size": 1,
+                    "condition_size": 1,
+                    "channels": 4,
+                    "head_size": 2,
+                    "kernel_size": 3,
+                    "dilations": [1, 2, 4, 8, 16, 32, 64],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": False,
+                },
+                {
+                    "condition_size": 1,
+                    "input_size": 4,
+                    "channels": 2,
+                    "head_size": 1,
+                    "kernel_size": 3,
+                    "dilations": [128, 256, 512, 1, 2, 4, 8, 16, 32, 64, 128, 256, 512],
+                    "activation": "Tanh",
+                    "gated": False,
+                    "head_bias": True,
+                },
+            ],
+            "head_scale": 0.02,
+        },
     }[architecture]
 
 
 _CAB_MRSTFT_PRE_EMPH_WEIGHT = 2.0e-4
 _CAB_MRSTFT_PRE_EMPH_COEF = 0.85
 
 
@@ -835,18 +869,29 @@
         lr,
         lr_decay,
         batch_size,
         fit_cab,
     )
 
     print("Starting training. It's time to kick ass and chew bubblegum!")
+    # Issue:
+    # * Model needs sample rate from data, but data set needs nx from model.
+    # * Model is re-instantiated after training anyways.
+    # (Hacky) solution: set sample rate in model from dataloader after second
+    # instantiation from final checkpoint.
     model = Model.init_from_config(model_config)
     train_dataloader, val_dataloader = _get_dataloaders(
         data_config, learning_config, model
     )
+    if train_dataloader.dataset.sample_rate != val_dataloader.dataset.sample_rate:
+        raise RuntimeError(
+            "Train and validation data loaders have different data set sample rates: "
+            f"{train_dataloader.dataset.sample_rate}, "
+            f"{val_dataloader.dataset.sample_rate}"
+        )
 
     trainer = pl.Trainer(
         callbacks=[
             pl.callbacks.model_checkpoint.ModelCheckpoint(
                 filename="checkpoint_best_{epoch:04d}_{step}_{ESR:.4g}_{MSE:.3e}",
                 save_top_k=3,
                 monitor="val_loss",
@@ -866,14 +911,15 @@
     if best_checkpoint != "":
         model = Model.load_from_checkpoint(
             trainer.checkpoint_callback.best_model_path,
             **Model.parse_config(model_config),
         )
     model.cpu()
     model.eval()
+    model.net.sample_rate = train_dataloader.dataset.sample_rate
 
     def window_kwargs(version: Version):
         if version.major == 1:
             return dict(
                 window_start=100_000,  # Start of the plotting window, in samples
                 window_end=101_000,  # End of the plotting window, in samples
             )
```

### Comparing `neural-amp-modeler-0.6.0/nam/train/gui.py` & `neural-amp-modeler-0.7.0/nam/train/gui.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/neural_amp_modeler.egg-info/SOURCES.txt` & `neural-amp-modeler-0.7.0/neural_amp_modeler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/setup.py` & `neural-amp-modeler-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/resources/__init__.py` & `neural-amp-modeler-0.7.0/tests/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_bin/test_train/test_main.py` & `neural-amp-modeler-0.7.0/tests/test_bin/test_train/test_main.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_data.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,14 +81,22 @@
         assert torch.all(x_out == torch.Tensor([0, 1, 2, 3]))
         assert torch.all(y_out == torch.Tensor([3, 4, 5, 6]))
 
     def test_init(self):
         x, y = self._create_xy()
         data.Dataset(x, y, 3, None)
 
+    def test_init_sample_rate(self):
+        x, y = self._create_xy()
+        sample_rate = 48_000.0
+        d = data.Dataset(x, y, 3, None, sample_rate=sample_rate)
+        assert hasattr(d, "sample_rate")
+        assert isinstance(d.sample_rate, float)
+        assert d.sample_rate == sample_rate
+
     def test_init_zero_delay(self):
         """
         Assert https://github.com/sdatkinson/neural-amp-modeler/issues/15 fixed
         """
         x, y = self._create_xy()
         data.Dataset(x, y, 3, None, delay=0)
 
@@ -281,35 +289,36 @@
         filename = os.path.join(tmpdir, "test.wav")
         data.np_to_wav(x, filename, scale=None)
         # Load WAV file
         y = data.wav_to_np(filename)
         # Check if the two arrays are equal
         assert y == pytest.approx(x, abs=self.tolerance)
 
+
 def test_audio_mismatch_shapes_in_order():
     """
     https://github.com/sdatkinson/neural-amp-modeler/issues/257
     """
     x_samples, y_samples = 5, 7
     num_channels = 1
 
     x, y = [np.zeros((n, num_channels)) for n in (x_samples, y_samples)]
-    
+
     with TemporaryDirectory() as tmpdir:
         y_path = Path(tmpdir, "y.wav")
         data.np_to_wav(y, y_path)
         f = lambda: data.wav_to_np(y_path, required_shape=x.shape)
-    
+
         with pytest.raises(data.AudioShapeMismatchError) as e:
             f()
 
         try:
             f()
             assert False, "Shouldn't have succeeded!"
         except data.AudioShapeMismatchError as e:
             # x is loaded first; we expect that y matches.
             assert e.shape_expected == (x_samples, num_channels)
             assert e.shape_actual == (y_samples, num_channels)
-            
+
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/base.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_base.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_base.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_conv_net.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_conv_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_exportable.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_exportable.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_losses.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_losses.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_catnets.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/test_catnets.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_parametric/test_hyper_net.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_parametric/test_hyper_net.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_recurrent.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_recurrent.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,22 +10,33 @@
 import pytest
 import torch
 
 from nam.models import recurrent
 
 from .base import Base
 
+_metadata_loudness_x_mocked = 0.1 * torch.randn((11,))  # Shorter for speed
+
 
 class TestLSTM(Base):
     @classmethod
     def setup_class(cls):
+        class LSTMWithMocks(recurrent.LSTM):
+            def __init__(self, *args, **kwargs):
+                super().__init__(*args, **kwargs)
+                self._get_initial_state_burn_in = 7
+
+            @classmethod
+            def _metadata_loudness_x(cls) -> torch.Tensor:
+                return _metadata_loudness_x_mocked
+
         num_layers = 2
         hidden_size = 3
         super().setup_class(
-            recurrent.LSTM,
+            LSTMWithMocks,
             args=(hidden_size,),
             kwargs={"train_burn_in": 3, "train_truncate": 5, "num_layers": num_layers},
         )
         cls._num_layers = num_layers
         cls._hidden_size = hidden_size
 
     def test_export_onnx(self):
```

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_models/test_wavenet.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_models/test_wavenet.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_core.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_train/test_core.py`

 * *Files identical despite different names*

### Comparing `neural-amp-modeler-0.6.0/tests/test_nam/test_train/test_version.py` & `neural-amp-modeler-0.7.0/tests/test_nam/test_train/test_version.py`

 * *Files identical despite different names*

