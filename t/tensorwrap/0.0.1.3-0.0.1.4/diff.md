# Comparing `tmp/tensorwrap-0.0.1.3.tar.gz` & `tmp/tensorwrap-0.0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorwrap-0.0.1.3.tar", last modified: Sun Jul 16 19:59:58 2023, max compression
+gzip compressed data, was "tensorwrap-0.0.1.4.tar", last modified: Mon Jul 17 03:22:34 2023, max compression
```

## Comparing `tensorwrap-0.0.1.3.tar` & `tensorwrap-0.0.1.4.tar`

### file list

```diff
@@ -1,58 +1,61 @@
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/
--rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/LICENSE
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6345 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/README.md
--rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/setup.cfg
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1918 2023-07-16 18:50:48.000000 tensorwrap-0.0.1.3/setup.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.161547 tensorwrap-0.0.1.3/tensorwrap/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1609 2023-07-16 18:43:03.000000 tensorwrap-0.0.1.3/tensorwrap/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/config.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/core/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/core/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/core/losses/mean.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/data.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap/experimental/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      133 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/serialize.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/experimental/wrappers.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/module.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      562 2023-07-16 17:08:50.000000 tensorwrap-0.0.1.3/tensorwrap/nn/__init__.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/activations/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/activations/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/activations/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/nn/callbacks.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.3/tensorwrap/nn/checkpoints.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/initializers/base.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.163547 tensorwrap-0.0.1.3/tensorwrap/nn/layers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      125 2023-07-16 19:58:59.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     4489 2023-07-16 17:43:32.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      629 2023-07-16 19:55:13.000000 tensorwrap-0.0.1.3/tensorwrap/nn/layers/lambda_layers.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/losses/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      156 2023-07-16 19:04:47.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      585 2023-07-16 19:55:31.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/categorical.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/mean.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      912 2023-07-16 19:03:35.000000 tensorwrap-0.0.1.3/tensorwrap/nn/losses/metrics.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/models/
--rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)     7384 2023-07-16 17:34:25.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/models/train.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.164547 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/
--rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/__init__.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/base.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.3/tensorwrap/ops.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.3/tensorwrap/test.py
--rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 19:59:53.000000 tensorwrap-0.0.1.3/tensorwrap/version.py
-drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-16 19:59:58.162547 tensorwrap-0.0.1.3/tensorwrap.egg-info/
--rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/PKG-INFO
--rw-r--r--   0 impureking  (1000) impureking  (1000)     1261 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/SOURCES.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/dependency_links.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/not-zip-safe
--rw-r--r--   0 impureking  (1000) impureking  (1000)      335 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/requires.txt
--rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-16 19:59:58.000000 tensorwrap-0.0.1.3/tensorwrap.egg-info/top_level.txt
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.117564 tensorwrap-0.0.1.4/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)    11313 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/LICENSE
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-17 03:22:34.117564 tensorwrap-0.0.1.4/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6345 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/README.md
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       38 2023-07-17 03:22:34.117564 tensorwrap-0.0.1.4/setup.cfg
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1918 2023-07-16 18:50:48.000000 tensorwrap-0.0.1.4/setup.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.113564 tensorwrap-0.0.1.4/tensorwrap/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1686 2023-07-17 01:52:23.000000 tensorwrap-0.0.1.4/tensorwrap/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      769 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/config.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.114565 tensorwrap-0.0.1.4/tensorwrap/core/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       20 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/core/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.114565 tensorwrap-0.0.1.4/tensorwrap/core/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      107 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/core/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      419 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/core/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      274 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/core/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      258 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/data.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.115564 tensorwrap-0.0.1.4/tensorwrap/experimental/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      151 2023-07-17 01:32:03.000000 tensorwrap-0.0.1.4/tensorwrap/experimental/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.115564 tensorwrap-0.0.1.4/tensorwrap/experimental/data/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       31 2023-07-17 01:51:17.000000 tensorwrap-0.0.1.4/tensorwrap/experimental/data/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      888 2023-07-17 02:08:20.000000 tensorwrap-0.0.1.4/tensorwrap/experimental/data/arraybased.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      587 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/experimental/serialize.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      244 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/experimental/wrappers.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     2924 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/module.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.115564 tensorwrap-0.0.1.4/tensorwrap/nn/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      562 2023-07-16 17:08:50.000000 tensorwrap-0.0.1.4/tensorwrap/nn/__init__.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.115564 tensorwrap-0.0.1.4/tensorwrap/nn/activations/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       55 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/activations/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1402 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/activations/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/nn/callbacks.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        0 2023-05-26 22:29:09.000000 tensorwrap-0.0.1.4/tensorwrap/nn/checkpoints.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.115564 tensorwrap-0.0.1.4/tensorwrap/nn/initializers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      604 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/initializers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      124 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/initializers/base.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.116564 tensorwrap-0.0.1.4/tensorwrap/nn/layers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      125 2023-07-16 19:58:59.000000 tensorwrap-0.0.1.4/tensorwrap/nn/layers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     4489 2023-07-16 17:43:32.000000 tensorwrap-0.0.1.4/tensorwrap/nn/layers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      629 2023-07-16 19:55:13.000000 tensorwrap-0.0.1.4/tensorwrap/nn/layers/lambda_layers.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.116564 tensorwrap-0.0.1.4/tensorwrap/nn/losses/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      156 2023-07-16 19:04:47.000000 tensorwrap-0.0.1.4/tensorwrap/nn/losses/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      371 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/losses/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      585 2023-07-16 19:55:31.000000 tensorwrap-0.0.1.4/tensorwrap/nn/losses/categorical.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      697 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/losses/mean.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      918 2023-07-17 03:08:36.000000 tensorwrap-0.0.1.4/tensorwrap/nn/losses/metrics.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.116564 tensorwrap-0.0.1.4/tensorwrap/nn/models/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      102 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/models/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     8855 2023-07-17 03:18:02.000000 tensorwrap-0.0.1.4/tensorwrap/nn/models/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       71 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/models/train.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.116564 tensorwrap-0.0.1.4/tensorwrap/nn/optimizers/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       66 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/optimizers/__init__.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      775 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/nn/optimizers/base.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      663 2023-07-16 17:07:55.000000 tensorwrap-0.0.1.4/tensorwrap/ops.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      448 2023-05-26 22:29:10.000000 tensorwrap-0.0.1.4/tensorwrap/test.py
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      110 2023-07-16 20:00:22.000000 tensorwrap-0.0.1.4/tensorwrap/version.py
+drwxr-xr-x   0 impureking  (1000) impureking  (1000)        0 2023-07-17 03:22:34.114565 tensorwrap-0.0.1.4/tensorwrap.egg-info/
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     6914 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/PKG-INFO
+-rw-r--r--   0 impureking  (1000) impureking  (1000)     1345 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/SOURCES.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/dependency_links.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)        1 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/not-zip-safe
+-rw-r--r--   0 impureking  (1000) impureking  (1000)      335 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/requires.txt
+-rw-r--r--   0 impureking  (1000) impureking  (1000)       11 2023-07-17 03:22:34.000000 tensorwrap-0.0.1.4/tensorwrap.egg-info/top_level.txt
```

### Comparing `tensorwrap-0.0.1.3/LICENSE` & `tensorwrap-0.0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/PKG-INFO` & `tensorwrap-0.0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tensorwrap-0.0.1.3/README.md` & `tensorwrap-0.0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/setup.py` & `tensorwrap-0.0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/__init__.py` & `tensorwrap-0.0.1.4/tensorwrap/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,28 +7,30 @@
 import os
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 # Library Paths:
 from tensorwrap import nn
 from tensorwrap import test
 from tensorwrap import config
+from tensorwrap import experimental
 
 # Path Shortener:
 from tensorwrap.module import Module
 from tensorwrap.version import __version__
 from tensorwrap.experimental.serialize import save_model, load_model
 from tensorwrap.experimental.wrappers import function
 from tensorwrap.ops import (last_dim,
                             randu,
                             randn)
 
 # JAX Built-ins:
 from jax import (disable_jit,
                  value_and_grad,
-                 grad)
+                 grad,
+                 vmap as vectorized_map)
 from jax.numpy import (array as tensor,
                        arange as range,
                        expand_dims,
                        matmul,
                        square,
                        abs,
                        mean,
```

### Comparing `tensorwrap-0.0.1.3/tensorwrap/config.py` & `tensorwrap-0.0.1.4/tensorwrap/config.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/experimental/serialize.py` & `tensorwrap-0.0.1.4/tensorwrap/experimental/serialize.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/module.py` & `tensorwrap-0.0.1.4/tensorwrap/module.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/__init__.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/activations/base.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/activations/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/initializers/__init__.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/initializers/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/layers/base.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/layers/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/layers/lambda_layers.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/layers/lambda_layers.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/losses/categorical.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/losses/categorical.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/losses/mean.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/losses/mean.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/losses/metrics.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/losses/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 
         """
         if from_logits:
             y_pred = jnp.argmax(y_pred, axis=-1)
 
         correct = jnp.sum(y_true == y_pred)
         total = y_true.shape[0]
-        return correct / total
+        return correct / total * 100
```

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/models/base.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/models/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Stable Modules:
+import time
 import jax
 import optax
 from jax import numpy as jnp
 from typing import (Any,
                     Tuple,
                     final)
 from jaxtyping import Array
@@ -144,37 +145,65 @@
         params = optax.apply_updates(params, updates)
         return params, (losses, y_pred)
 
 
     def fit(self,
             x_train,
             y_train,
-            epochs = 1):
+            epochs = 1,
+            batch_size=32):
         """ Built-in in training method that updates gradients with minimalistic setup.
         
         Args:
             x_train: The labels array.
             y_train: The targets array.
             epochs: Number of repetition for gradient updates.
 
         NOTE: Doesn't support batching and requires initiating of parameters and compilation of loss function
         and optimizers.
         """
         if epochs < 1:
             raise ValueError("Epochs must be a positive value.")
 
+        # Batching the data:
+        X_train_batched, y_train_batched = tf.experimental.data.Dataset(x_train).batch(batch_size), tf.experimental.data.Dataset(y_train).batch(batch_size)
 
+        batch_num = len(x_train)//batch_size
+        update_time = batch_num//20
+        prev_loss = "nan"
+        prev_acc = "nan"
+        metric = tf.randn((batch_num,))
         for epoch in range(1, epochs + 1):
-            self.trainable_variables, (loss, pred) = self.train_step(self.trainable_variables, x_train, y_train)
-            metric = self.metrics(y_train, pred)
-            print(f"Epoch: {epoch} \t\t Loss: {loss:.5f} \t\t Metrics: {metric:.5f}")
-        
+            for index, (x_batch, y_batch) in enumerate(zip(X_train_batched, y_train_batched)):
+                self.trainable_variables, (loss, pred) = self.train_step(self.trainable_variables, x_batch, y_batch)
+                metric = metric.at[index].set(self.metrics(y_batch, pred))
+                if index % (update_time + 1) == 0:
+                    prev_loss = loss
+                    prev_acc = metric.mean()
+                self.__show_loading_animation(epoch, batch_num, index + 1, prev_loss, prev_acc)
+            print('\n')
+        
+    def __show_loading_animation(self, epoch, total_batches, current_batch, loss, metric):
+        prefix = f'Epoch {epoch}: '
+        length = 30
+        filled_length = int(length * current_batch // total_batches)
+        bar = '=' * filled_length + '>' + '-' * (length - filled_length - 1)
+        print(f'\r{prefix} [{bar}] {current_batch}/{total_batches} \t Loss: {loss} \t metric: {metric}', end='', flush=True)
 
     def predict(self, x):
         return self.__call__(self.trainable_variables, x)
+    
+    def evaluate(self, x, y):
+        if not self._compiled:
+            raise NotImplementedError("The model has not been compiled. Please compile using ``self.compile``.")
+        
+        pred = self.predict(x)
+        metric = self.metrics(y, pred)
+        loss = self.loss_fn(y, pred)
+        print(f"Epoch 1 \t\t\t Loss: {loss} \t\t\t metric: {metric}")
 
 
     def __call__(self, params = None, inputs = None) -> Any:
         if not self._init:
             raise NotImplementedError("The model is not initialized using ``self.init_params``.")
 
     def __repr__(self) -> str:
```

### Comparing `tensorwrap-0.0.1.3/tensorwrap/nn/optimizers/base.py` & `tensorwrap-0.0.1.4/tensorwrap/nn/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap/ops.py` & `tensorwrap-0.0.1.4/tensorwrap/ops.py`

 * *Files identical despite different names*

### Comparing `tensorwrap-0.0.1.3/tensorwrap.egg-info/PKG-INFO` & `tensorwrap-0.0.1.4/tensorwrap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorwrap
-Version: 0.0.1.3
+Version: 0.0.1.4
 Summary: TensorWrap: A high level TensorFlow wrapper for JAX.
 Home-page: https://github.com/Impure-King/base-tensorwrap
 Author: Lelouch
 Author-email: ImpureK@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `tensorwrap-0.0.1.3/tensorwrap.egg-info/SOURCES.txt` & `tensorwrap-0.0.1.4/tensorwrap.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 tensorwrap/core/__init__.py
 tensorwrap/core/losses/__init__.py
 tensorwrap/core/losses/categorical.py
 tensorwrap/core/losses/mean.py
 tensorwrap/experimental/__init__.py
 tensorwrap/experimental/serialize.py
 tensorwrap/experimental/wrappers.py
+tensorwrap/experimental/data/__init__.py
+tensorwrap/experimental/data/arraybased.py
 tensorwrap/nn/__init__.py
 tensorwrap/nn/callbacks.py
 tensorwrap/nn/checkpoints.py
 tensorwrap/nn/activations/__init__.py
 tensorwrap/nn/activations/base.py
 tensorwrap/nn/initializers/__init__.py
 tensorwrap/nn/initializers/base.py
```

