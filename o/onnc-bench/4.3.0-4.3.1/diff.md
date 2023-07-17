# Comparing `tmp/onnc-bench-4.3.0.tar.gz` & `tmp/onnc-bench-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnc-bench-4.3.0.tar", last modified: Wed Jul 12 05:14:26 2023, max compression
+gzip compressed data, was "onnc-bench-4.3.1.tar", last modified: Mon Jul 17 03:39:53 2023, max compression
```

## Comparing `onnc-bench-4.3.0.tar` & `onnc-bench-4.3.1.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1070 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      784 2023-07-05 02:46:47.000000 onnc-bench-4.3.0/README.md
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.447508 onnc-bench-4.3.0/onnc/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)      863 2023-02-07 10:13:51.000000 onnc-bench-4.3.0/onnc/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      794 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc/bench/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1213 2023-06-01 09:39:05.000000 onnc-bench-4.3.0/onnc/bench/config.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       92 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/benchmark.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      515 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/bench/core/common.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/compiler/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1811 2023-07-06 03:40:40.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1843 2023-07-06 03:49:30.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/builder.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4319 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2129 2022-09-22 04:18:54.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe_docker.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)    11826 2023-06-20 04:57:49.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/onnc_saas.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1009 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/bench/core/compiler/saas_config.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/dataset/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3072 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/dataset.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      661 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/layout.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2220 2022-10-19 15:48:12.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/operation.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1508 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/preprocessor.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     8208 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/serializer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2419 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/dataset/transformer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4005 2023-05-22 10:27:59.000000 onnc-bench-4.3.0/onnc/bench/core/deployment.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/evaluator/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      697 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/evaluator/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/bench/core/model/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/bench/core/model/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3912 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/model/model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6987 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/core/model/serializer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      577 2022-05-19 06:51:56.000000 onnc-bench-4.3.0/onnc/bench/core/model/transformer.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     7409 2023-07-12 04:29:20.000000 onnc-bench-4.3.0/onnc/bench/core/modelpackage.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6963 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/bench/project.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      279 2022-07-28 03:03:26.000000 onnc-bench-4.3.0/onnc/bench/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      295 2022-07-28 03:03:26.000000 onnc-bench-4.3.0/onnc/forest/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/core/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/core/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      748 2022-09-21 03:34:59.000000 onnc-bench-4.3.0/onnc/forest/core/binding_helper.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1618 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/core/options.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4144 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/core/runtime.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/proxies/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1663 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2066 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2334 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime_server.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      482 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/__init__.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-02-07 10:13:51.000000 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2072 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/onnx/runtime.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.451508 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4823 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     6455 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/forest/runtimes/openvino/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3627 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/runtime.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2930 2022-07-26 09:00:19.000000 onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/utils.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc/forest/utils/
--rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.0/onnc/forest/utils/__init__.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      510 2022-07-05 06:10:59.000000 onnc-bench-4.3.0/onnc/forest/utils/load_img.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/onnc_bench.egg-info/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1070 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/PKG-INFO
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2052 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/SOURCES.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        1 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/dependency_links.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      211 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/requires.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)        5 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/onnc_bench.egg-info/top_level.txt
--rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/setup.cfg
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     1278 2023-07-12 05:14:26.000000 onnc-bench-4.3.0/setup.py
-drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-12 05:14:26.455508 onnc-bench-4.3.0/tests/
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      721 2023-06-07 17:45:11.000000 onnc-bench-4.3.0/tests/test_core_compiler.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     2207 2022-10-25 06:18:30.000000 onnc-bench-4.3.0/tests/test_core_dataset_operation.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     4576 2023-07-12 04:28:10.000000 onnc-bench-4.3.0/tests/test_core_model.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3379 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_core_modelpackage.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3936 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_onnc_saas_builder.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)      398 2023-07-07 02:25:54.000000 onnc-bench-4.3.0/tests/test_options_factory.py
--rw-rw-r--   0 fuji      (1010) fuji      (1010)     3389 2022-09-19 02:11:04.000000 onnc-bench-4.3.0/tests/test_runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.412953 onnc-bench-4.3.1/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1313 2023-07-17 03:39:53.412953 onnc-bench-4.3.1/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1027 2023-07-17 03:34:15.000000 onnc-bench-4.3.1/README.md
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.404954 onnc-bench-4.3.1/onnc/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)      863 2023-02-07 10:13:51.000000 onnc-bench-4.3.1/onnc/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.404954 onnc-bench-4.3.1/onnc/bench/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      794 2023-07-17 03:39:07.000000 onnc-bench-4.3.1/onnc/bench/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1213 2023-06-01 09:39:05.000000 onnc-bench-4.3.1/onnc/bench/config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.404954 onnc-bench-4.3.1/onnc/bench/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       92 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/benchmark.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      515 2022-07-05 06:10:59.000000 onnc-bench-4.3.1/onnc/bench/core/common.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/bench/core/compiler/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1811 2023-07-06 03:40:40.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1843 2023-07-06 03:49:30.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/builder.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4319 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/nnuxe.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2129 2022-09-22 04:18:54.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/nnuxe_docker.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)    11826 2023-06-20 04:57:49.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/onnc_saas.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1009 2022-07-05 06:10:59.000000 onnc-bench-4.3.1/onnc/bench/core/compiler/saas_config.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/bench/core/dataset/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       51 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3072 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/dataset.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      661 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/layout.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2220 2022-10-19 15:48:12.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/operation.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1508 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/preprocessor.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     8208 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2419 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/dataset/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4005 2023-05-22 10:27:59.000000 onnc-bench-4.3.1/onnc/bench/core/deployment.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/bench/core/evaluator/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      697 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/evaluator/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/bench/core/model/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/bench/core/model/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3912 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/model/model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6987 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/model/serializer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      577 2022-05-19 06:51:56.000000 onnc-bench-4.3.1/onnc/bench/core/model/transformer.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     7409 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/core/modelpackage.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6963 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/bench/project.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      279 2022-07-28 03:03:26.000000 onnc-bench-4.3.1/onnc/bench/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      295 2022-07-28 03:03:26.000000 onnc-bench-4.3.1/onnc/forest/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/core/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.1/onnc/forest/core/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      748 2022-09-21 03:34:59.000000 onnc-bench-4.3.1/onnc/forest/core/binding_helper.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1618 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/forest/core/options.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4144 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/forest/core/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/proxies/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1663 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/forest/proxies/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2022-09-19 02:11:04.000000 onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2066 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2334 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/runtime_server.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      482 2022-09-19 02:11:04.000000 onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/runtimes/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.1/onnc/forest/runtimes/__init__.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/runtimes/onnx/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        0 2023-02-07 10:13:51.000000 onnc-bench-4.3.1/onnc/forest/runtimes/onnx/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2072 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/forest/runtimes/onnx/runtime.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/runtimes/openvino/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.1/onnc/forest/runtimes/openvino/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4823 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/forest/runtimes/openvino/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     6455 2022-07-05 06:10:59.000000 onnc-bench-4.3.1/onnc/forest/runtimes/openvino/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3627 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/runtime.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2930 2022-07-26 09:00:19.000000 onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/utils.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc/forest/utils/
+-rwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2022-07-22 10:02:31.000000 onnc-bench-4.3.1/onnc/forest/utils/__init__.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      510 2022-07-05 06:10:59.000000 onnc-bench-4.3.1/onnc/forest/utils/load_img.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.408954 onnc-bench-4.3.1/onnc_bench.egg-info/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1313 2023-07-17 03:39:53.000000 onnc-bench-4.3.1/onnc_bench.egg-info/PKG-INFO
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2052 2023-07-17 03:39:53.000000 onnc-bench-4.3.1/onnc_bench.egg-info/SOURCES.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        1 2023-07-17 03:39:53.000000 onnc-bench-4.3.1/onnc_bench.egg-info/dependency_links.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      211 2023-07-17 03:39:53.000000 onnc-bench-4.3.1/onnc_bench.egg-info/requires.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)        5 2023-07-17 03:39:53.000000 onnc-bench-4.3.1/onnc_bench.egg-info/top_level.txt
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)       38 2023-07-17 03:39:53.412953 onnc-bench-4.3.1/setup.cfg
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     1278 2023-07-17 03:39:02.000000 onnc-bench-4.3.1/setup.py
+drwxrwxr-x   0 fuji      (1010) fuji      (1010)        0 2023-07-17 03:39:53.412953 onnc-bench-4.3.1/tests/
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      721 2023-06-07 17:45:11.000000 onnc-bench-4.3.1/tests/test_core_compiler.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     2207 2022-10-25 06:18:30.000000 onnc-bench-4.3.1/tests/test_core_dataset_operation.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     4576 2023-07-12 05:30:20.000000 onnc-bench-4.3.1/tests/test_core_model.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3379 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/tests/test_core_modelpackage.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3936 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/tests/test_onnc_saas_builder.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)      398 2023-07-07 02:25:54.000000 onnc-bench-4.3.1/tests/test_options_factory.py
+-rw-rw-r--   0 fuji      (1010) fuji      (1010)     3389 2022-09-19 02:11:04.000000 onnc-bench-4.3.1/tests/test_runtime.py
```

### Comparing `onnc-bench-4.3.0/PKG-INFO` & `onnc-bench-4.3.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 Metadata-Version: 2.1
 Name: onnc-bench
-Version: 4.3.0
+Version: 4.3.1
 Summary: ONNC-bench is a Python wrapper of ONNC
 Home-page: https://www.skymizer.com
 Author: The Skymizer Team
 Author-email: hello@skymizer.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+# WARNING: This repository is no longer maintained ⚠️
+
+This repository has been moved to:
+
+- https://github.com/skymizer/oasis-api-client
+- https://pypi.org/project/oasis-api-client/
+
+Make sure you have permission to view this repository
+
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
 ### Developer install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `onnc-bench-4.3.0/README.md` & `onnc-bench-4.3.1/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+# WARNING: This repository is no longer maintained ⚠️
+
+This repository has been moved to:
+
+- https://github.com/skymizer/oasis-api-client
+- https://pypi.org/project/oasis-api-client/
+
+Make sure you have permission to view this repository
+
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
 ### Developer install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `onnc-bench-4.3.0/onnc/__init__.py` & `onnc-bench-4.3.1/onnc/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/__init__.py` & `onnc-bench-4.3.1/onnc/bench/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,8 +24,8 @@
              level="INFO")
 
 sentry_sdk.init(
     "https://da9cdf5759874504940714a91657de21@o304393.ingest.sentry.io/5901378",
     traces_sample_rate=1.0)
 fpath = os.path.dirname(os.path.abspath(__file__))
 
-__version__= "4.3.0"
+__version__= "4.3.1"
```

### Comparing `onnc-bench-4.3.0/onnc/bench/config.py` & `onnc-bench-4.3.1/onnc/bench/config.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/common.py` & `onnc-bench-4.3.1/onnc/bench/core/common.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/__init__.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/builder.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/builder.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/nnuxe.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/nnuxe_docker.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/nnuxe_docker.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/onnc_saas.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/onnc_saas.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/compiler/saas_config.py` & `onnc-bench-4.3.1/onnc/bench/core/compiler/saas_config.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/dataset.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/layout.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/layout.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/operation.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/operation.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/preprocessor.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/preprocessor.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/serializer.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/serializer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/dataset/transformer.py` & `onnc-bench-4.3.1/onnc/bench/core/dataset/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/deployment.py` & `onnc-bench-4.3.1/onnc/bench/core/deployment.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/evaluator/__init__.py` & `onnc-bench-4.3.1/onnc/bench/core/evaluator/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/model/model.py` & `onnc-bench-4.3.1/onnc/bench/core/model/model.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/model/serializer.py` & `onnc-bench-4.3.1/onnc/bench/core/model/serializer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/model/transformer.py` & `onnc-bench-4.3.1/onnc/bench/core/model/transformer.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/core/modelpackage.py` & `onnc-bench-4.3.1/onnc/bench/core/modelpackage.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/bench/project.py` & `onnc-bench-4.3.1/onnc/bench/project.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/core/binding_helper.py` & `onnc-bench-4.3.1/onnc/forest/core/binding_helper.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/core/options.py` & `onnc-bench-4.3.1/onnc/forest/core/options.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/core/runtime.py` & `onnc-bench-4.3.1/onnc/forest/core/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/proxies/__init__.py` & `onnc-bench-4.3.1/onnc/forest/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime.py` & `onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/proxies/zerorpc/runtime_server.py` & `onnc-bench-4.3.1/onnc/forest/proxies/zerorpc/runtime_server.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/runtimes/onnx/runtime.py` & `onnc-bench-4.3.1/onnc/forest/runtimes/onnx/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/runtimes/openvino/runtime.py` & `onnc-bench-4.3.1/onnc/forest/runtimes/openvino/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/runtimes/openvino/utils.py` & `onnc-bench-4.3.1/onnc/forest/runtimes/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/runtime.py` & `onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/runtime.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc/forest/runtimes/tensorrt/utils.py` & `onnc-bench-4.3.1/onnc/forest/runtimes/tensorrt/utils.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/onnc_bench.egg-info/PKG-INFO` & `onnc-bench-4.3.1/onnc_bench.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,27 @@
 Metadata-Version: 2.1
 Name: onnc-bench
-Version: 4.3.0
+Version: 4.3.1
 Summary: ONNC-bench is a Python wrapper of ONNC
 Home-page: https://www.skymizer.com
 Author: The Skymizer Team
 Author-email: hello@skymizer.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
+# WARNING: This repository is no longer maintained ⚠️
+
+This repository has been moved to:
+
+- https://github.com/skymizer/oasis-api-client
+- https://pypi.org/project/oasis-api-client/
+
+Make sure you have permission to view this repository
+
 # ONNC-bench
 
 ONNC-bench is a Python wrapper of ONNC
 
 ## Installation
 
 ### Developer install
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `onnc-bench-4.3.0/onnc_bench.egg-info/SOURCES.txt` & `onnc-bench-4.3.1/onnc_bench.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/setup.py` & `onnc-bench-4.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
                 requirements[i] = requirements[i].replace("{CWD}", os.getcwd())
     return [r for r in requirements if r and r[0] != '#']
 
 
 # This call to setup() does all the work
 setup(
     name="onnc-bench",
-    version="4.3.0",
+    version="4.3.1",
     description="ONNC-bench is a Python wrapper of ONNC",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.skymizer.com",
     author="The Skymizer Team",
     author_email="hello@skymizer.com",
     license="Apache License 2.0",
```

### Comparing `onnc-bench-4.3.0/tests/test_core_compiler.py` & `onnc-bench-4.3.1/tests/test_core_compiler.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/tests/test_core_dataset_operation.py` & `onnc-bench-4.3.1/tests/test_core_dataset_operation.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/tests/test_core_model.py` & `onnc-bench-4.3.1/tests/test_core_model.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/tests/test_core_modelpackage.py` & `onnc-bench-4.3.1/tests/test_core_modelpackage.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/tests/test_onnc_saas_builder.py` & `onnc-bench-4.3.1/tests/test_onnc_saas_builder.py`

 * *Files identical despite different names*

### Comparing `onnc-bench-4.3.0/tests/test_runtime.py` & `onnc-bench-4.3.1/tests/test_runtime.py`

 * *Files identical despite different names*

