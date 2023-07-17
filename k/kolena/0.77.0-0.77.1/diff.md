# Comparing `tmp/kolena-0.77.0.tar.gz` & `tmp/kolena-0.77.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kolena-0.77.0.tar", max compression
+gzip compressed data, was "kolena-0.77.1.tar", max compression
```

## Comparing `kolena-0.77.0.tar` & `kolena-0.77.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
--rw-r--r--   0        0        0    11346 2023-07-12 00:24:31.058858 kolena-0.77.0/LICENSE
--rw-r--r--   0        0        0      556 2023-07-12 00:24:31.058858 kolena-0.77.0/LICENSE_HEADER
--rw-r--r--   0        0        0     1948 2023-07-12 00:24:31.058858 kolena-0.77.0/README.md
--rw-r--r--   0        0        0     1349 2023-07-12 00:24:31.118864 kolena-0.77.0/kolena/__init__.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.118864 kolena-0.77.0/kolena/_api/__init__.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.118864 kolena-0.77.0/kolena/_api/v1/__init__.py
--rw-r--r--   0        0        0     1737 2023-07-12 00:24:31.118864 kolena-0.77.0/kolena/_api/v1/batched_load.py
--rw-r--r--   0        0        0      878 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/client_log.py
--rw-r--r--   0        0        0     5111 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/core.py
--rw-r--r--   0        0        0     5320 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/detection.py
--rw-r--r--   0        0        0     7531 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/fr.py
--rw-r--r--   0        0        0     5597 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/generic.py
--rw-r--r--   0        0        0      778 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/repository.py
--rw-r--r--   0        0        0      833 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/token.py
--rw-r--r--   0        0        0      738 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_api/v1/workflow.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/__init__.py
--rw-r--r--   0        0        0     1117 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/__init__.py
--rw-r--r--   0        0        0     5654 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/evaluator.py
--rw-r--r--   0        0        0    15446 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/evaluator_multiclass.py
--rw-r--r--   0        0        0    10294 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/evaluator_single_class.py
--rw-r--r--   0        0        0    13260 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/utils.py
--rw-r--r--   0        0        0     5029 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_experimental/object_detection/workflow.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_extras/__init__.py
--rw-r--r--   0        0        0      676 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_extras/metrics/__init__.py
--rw-r--r--   0        0        0      783 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_extras/metrics/sklearn.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/__init__.py
--rw-r--r--   0        0        0     1616 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/asset_path_mapper.py
--rw-r--r--   0        0        0     5313 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/batched_load.py
--rw-r--r--   0        0        0     5608 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/cli.py
--rw-r--r--   0        0        0      921 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/consts.py
--rw-r--r--   0        0        0      579 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/dataframes/__init__.py
--rw-r--r--   0        0        0     2826 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/dataframes/validators.py
--rw-r--r--   0        0        0     1952 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/datatypes.py
--rw-r--r--   0        0        0     3403 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/endpoints.py
--rw-r--r--   0        0        0     1690 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/frozen.py
--rw-r--r--   0        0        0     1183 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/geometry.py
--rw-r--r--   0        0        0     1087 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/inference_validators.py
--rw-r--r--   0        0        0     2990 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/instrumentation.py
--rw-r--r--   0        0        0     5033 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/krequests.py
--rw-r--r--   0        0        0     3507 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/log.py
--rw-r--r--   0        0        0     1003 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/repository.py
--rw-r--r--   0        0        0     2494 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/serde.py
--rw-r--r--   0        0        0      889 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/serializable.py
--rw-r--r--   0        0        0     5450 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/state.py
--rw-r--r--   0        0        0     1942 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/uninstantiable.py
--rw-r--r--   0        0        0     1164 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/_utils/validators.py
--rw-r--r--   0        0        0     1272 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/metadata.py
--rw-r--r--   0        0        0     3512 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/model.py
--rw-r--r--   0        0        0     1213 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/multiclass/__init__.py
--rw-r--r--   0        0        0     3354 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/multiclass/_utils.py
--rw-r--r--   0        0        0    15698 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/multiclass/evaluator.py
--rw-r--r--   0        0        0     3573 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/multiclass/test_run.py
--rw-r--r--   0        0        0     3185 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/multiclass/workflow.py
--rw-r--r--   0        0        0     2694 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/test_case.py
--rw-r--r--   0        0        0     2372 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/test_config.py
--rw-r--r--   0        0        0     4480 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/test_image.py
--rw-r--r--   0        0        0     6013 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/test_run.py
--rw-r--r--   0        0        0     3180 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/classification/test_suite.py
--rw-r--r--   0        0        0     1477 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/__init__.py
--rw-r--r--   0        0        0     6819 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_datatypes.py
--rw-r--r--   0        0        0     1042 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/__init__.py
--rw-r--r--   0        0        0     1922 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/datatypes.py
--rw-r--r--   0        0        0      765 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/ground_truth.py
--rw-r--r--   0        0        0     1035 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/inference.py
--rw-r--r--   0        0        0     5470 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/metadata.py
--rw-r--r--   0        0        0     8995 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/model.py
--rw-r--r--   0        0        0    14122 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/test_case.py
--rw-r--r--   0        0        0     1201 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/test_config.py
--rw-r--r--   0        0        0     1761 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/test_image.py
--rw-r--r--   0        0        0    12390 2023-07-12 00:24:31.122865 kolena-0.77.0/kolena/detection/_internal/test_run.py
--rw-r--r--   0        0        0    13804 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/_internal/test_suite.py
--rw-r--r--   0        0        0     5867 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/ground_truth.py
--rw-r--r--   0        0        0     5435 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/inference.py
--rw-r--r--   0        0        0     1460 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/metadata.py
--rw-r--r--   0        0        0     3210 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/model.py
--rw-r--r--   0        0        0     2387 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/test_case.py
--rw-r--r--   0        0        0     3199 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/test_config.py
--rw-r--r--   0        0        0     5967 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/test_image.py
--rw-r--r--   0        0        0     5405 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/test_run.py
--rw-r--r--   0        0        0     2854 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/detection/test_suite.py
--rw-r--r--   0        0        0     2681 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/errors.py
--rw-r--r--   0        0        0     1400 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/__init__.py
--rw-r--r--   0        0        0     2171 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/_utils.py
--rw-r--r--   0        0        0    20960 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/datatypes.py
--rw-r--r--   0        0        0    10274 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/model.py
--rw-r--r--   0        0        0    14952 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/test_case.py
--rw-r--r--   0        0        0    12237 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/test_images.py
--rw-r--r--   0        0        0    16943 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/test_run.py
--rw-r--r--   0        0        0    16329 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/fr/test_suite.py
--rw-r--r--   0        0        0     3880 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/initialize.py
--rw-r--r--   0        0        0     2439 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/__init__.py
--rw-r--r--   0        0        0    13948 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/_datatypes.py
--rw-r--r--   0        0        0     6281 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/_validators.py
--rw-r--r--   0        0        0    10397 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/annotation.py
--rw-r--r--   0        0        0     4926 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/asset.py
--rw-r--r--   0        0        0     3469 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/define_workflow.py
--rw-r--r--   0        0        0    13854 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/evaluator.py
--rw-r--r--   0        0        0    11232 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/evaluator_function.py
--rw-r--r--   0        0        0     4421 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/ground_truth.py
--rw-r--r--   0        0        0     4334 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/inference.py
--rw-r--r--   0        0        0     1103 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/metrics/__init__.py
--rw-r--r--   0        0        0     2977 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/metrics/_formula.py
--rw-r--r--   0        0        0    16014 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/metrics/_geometry.py
--rw-r--r--   0        0        0     8459 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/model.py
--rw-r--r--   0        0        0    10261 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/plot.py
--rw-r--r--   0        0        0    18319 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/test_case.py
--rw-r--r--   0        0        0    22734 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/test_run.py
--rw-r--r--   0        0        0    10564 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/test_sample.py
--rw-r--r--   0        0        0    15455 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/test_suite.py
--rw-r--r--   0        0        0      792 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/visualization/__init__.py
--rw-r--r--   0        0        0     6145 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/visualization/_activation_map.py
--rw-r--r--   0        0        0     9419 2023-07-12 00:24:31.126865 kolena-0.77.0/kolena/workflow/workflow.py
--rw-r--r--   0        0        0     3027 2023-07-12 00:24:47.608370 kolena-0.77.0/pyproject.toml
--rw-r--r--   0        0        0     4316 1970-01-01 00:00:00.000000 kolena-0.77.0/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-07-17 18:15:30.569075 kolena-0.77.1/LICENSE
+-rw-r--r--   0        0        0      556 2023-07-17 18:15:30.569075 kolena-0.77.1/LICENSE_HEADER
+-rw-r--r--   0        0        0     1948 2023-07-17 18:15:30.569075 kolena-0.77.1/README.md
+-rw-r--r--   0        0        0     1349 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/__init__.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/__init__.py
+-rw-r--r--   0        0        0     1737 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/batched_load.py
+-rw-r--r--   0        0        0      878 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/client_log.py
+-rw-r--r--   0        0        0     5111 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/core.py
+-rw-r--r--   0        0        0     5320 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/detection.py
+-rw-r--r--   0        0        0     7531 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/fr.py
+-rw-r--r--   0        0        0     5597 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/generic.py
+-rw-r--r--   0        0        0      778 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/repository.py
+-rw-r--r--   0        0        0      833 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/token.py
+-rw-r--r--   0        0        0      738 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_api/v1/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/__init__.py
+-rw-r--r--   0        0        0     1117 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/object_detection/__init__.py
+-rw-r--r--   0        0        0     5654 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/object_detection/evaluator.py
+-rw-r--r--   0        0        0    15446 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/object_detection/evaluator_multiclass.py
+-rw-r--r--   0        0        0    10294 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/object_detection/evaluator_single_class.py
+-rw-r--r--   0        0        0    13260 2023-07-17 18:15:30.617075 kolena-0.77.1/kolena/_experimental/object_detection/utils.py
+-rw-r--r--   0        0        0     5029 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_experimental/object_detection/workflow.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_extras/__init__.py
+-rw-r--r--   0        0        0      676 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_extras/metrics/__init__.py
+-rw-r--r--   0        0        0      783 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_extras/metrics/sklearn.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/__init__.py
+-rw-r--r--   0        0        0     1616 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/asset_path_mapper.py
+-rw-r--r--   0        0        0     5313 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/batched_load.py
+-rw-r--r--   0        0        0     5608 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/cli.py
+-rw-r--r--   0        0        0      921 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/consts.py
+-rw-r--r--   0        0        0      579 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0     2826 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/dataframes/validators.py
+-rw-r--r--   0        0        0     1952 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/datatypes.py
+-rw-r--r--   0        0        0     3403 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/endpoints.py
+-rw-r--r--   0        0        0     1690 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/frozen.py
+-rw-r--r--   0        0        0     1183 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/geometry.py
+-rw-r--r--   0        0        0     1087 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/inference_validators.py
+-rw-r--r--   0        0        0     2990 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/instrumentation.py
+-rw-r--r--   0        0        0     5033 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/krequests.py
+-rw-r--r--   0        0        0     3507 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/log.py
+-rw-r--r--   0        0        0     1003 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/repository.py
+-rw-r--r--   0        0        0     2494 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/serde.py
+-rw-r--r--   0        0        0      889 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/serializable.py
+-rw-r--r--   0        0        0     5450 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/state.py
+-rw-r--r--   0        0        0     1942 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/uninstantiable.py
+-rw-r--r--   0        0        0     1164 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/_utils/validators.py
+-rw-r--r--   0        0        0     1272 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/metadata.py
+-rw-r--r--   0        0        0     3512 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/model.py
+-rw-r--r--   0        0        0     1213 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/multiclass/__init__.py
+-rw-r--r--   0        0        0     3354 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/multiclass/_utils.py
+-rw-r--r--   0        0        0    15698 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/multiclass/evaluator.py
+-rw-r--r--   0        0        0     3573 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/multiclass/test_run.py
+-rw-r--r--   0        0        0     3185 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/multiclass/workflow.py
+-rw-r--r--   0        0        0     2694 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/test_case.py
+-rw-r--r--   0        0        0     2372 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/test_config.py
+-rw-r--r--   0        0        0     4480 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/test_image.py
+-rw-r--r--   0        0        0     6013 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/test_run.py
+-rw-r--r--   0        0        0     3180 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/classification/test_suite.py
+-rw-r--r--   0        0        0     1477 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/__init__.py
+-rw-r--r--   0        0        0     6819 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_datatypes.py
+-rw-r--r--   0        0        0     1042 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/__init__.py
+-rw-r--r--   0        0        0     1922 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/datatypes.py
+-rw-r--r--   0        0        0      765 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/ground_truth.py
+-rw-r--r--   0        0        0     1035 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/inference.py
+-rw-r--r--   0        0        0     5470 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/metadata.py
+-rw-r--r--   0        0        0     8995 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/model.py
+-rw-r--r--   0        0        0    14122 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/test_case.py
+-rw-r--r--   0        0        0     1201 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/test_config.py
+-rw-r--r--   0        0        0     1761 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/test_image.py
+-rw-r--r--   0        0        0    12390 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/test_run.py
+-rw-r--r--   0        0        0    13804 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/_internal/test_suite.py
+-rw-r--r--   0        0        0     5867 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/ground_truth.py
+-rw-r--r--   0        0        0     5435 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/inference.py
+-rw-r--r--   0        0        0     1460 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/metadata.py
+-rw-r--r--   0        0        0     3210 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/model.py
+-rw-r--r--   0        0        0     2387 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/test_case.py
+-rw-r--r--   0        0        0     3199 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/test_config.py
+-rw-r--r--   0        0        0     5967 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/test_image.py
+-rw-r--r--   0        0        0     5405 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/test_run.py
+-rw-r--r--   0        0        0     2854 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/detection/test_suite.py
+-rw-r--r--   0        0        0     2681 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/errors.py
+-rw-r--r--   0        0        0     1400 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/__init__.py
+-rw-r--r--   0        0        0     2171 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/_utils.py
+-rw-r--r--   0        0        0    20960 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/datatypes.py
+-rw-r--r--   0        0        0    10274 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/model.py
+-rw-r--r--   0        0        0    14952 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/test_case.py
+-rw-r--r--   0        0        0    12237 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/test_images.py
+-rw-r--r--   0        0        0    16943 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/test_run.py
+-rw-r--r--   0        0        0    16329 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/fr/test_suite.py
+-rw-r--r--   0        0        0     3880 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/initialize.py
+-rw-r--r--   0        0        0     2439 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/workflow/__init__.py
+-rw-r--r--   0        0        0    13948 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/workflow/_datatypes.py
+-rw-r--r--   0        0        0     6281 2023-07-17 18:15:30.621075 kolena-0.77.1/kolena/workflow/_validators.py
+-rw-r--r--   0        0        0    10397 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/annotation.py
+-rw-r--r--   0        0        0     4926 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/asset.py
+-rw-r--r--   0        0        0     3469 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/define_workflow.py
+-rw-r--r--   0        0        0    13854 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/evaluator.py
+-rw-r--r--   0        0        0    11232 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/evaluator_function.py
+-rw-r--r--   0        0        0     4421 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/ground_truth.py
+-rw-r--r--   0        0        0     4334 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/inference.py
+-rw-r--r--   0        0        0     1103 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/metrics/__init__.py
+-rw-r--r--   0        0        0     2977 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/metrics/_formula.py
+-rw-r--r--   0        0        0    16014 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/metrics/_geometry.py
+-rw-r--r--   0        0        0     8459 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/model.py
+-rw-r--r--   0        0        0    10261 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/plot.py
+-rw-r--r--   0        0        0    18319 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/test_case.py
+-rw-r--r--   0        0        0    22734 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/test_run.py
+-rw-r--r--   0        0        0    10564 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/test_sample.py
+-rw-r--r--   0        0        0    15455 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/test_suite.py
+-rw-r--r--   0        0        0      792 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/visualization/__init__.py
+-rw-r--r--   0        0        0     6145 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/visualization/_activation_map.py
+-rw-r--r--   0        0        0     9419 2023-07-17 18:15:30.625075 kolena-0.77.1/kolena/workflow/workflow.py
+-rw-r--r--   0        0        0     3030 2023-07-17 18:15:44.293050 kolena-0.77.1/pyproject.toml
+-rw-r--r--   0        0        0     4319 1970-01-01 00:00:00.000000 kolena-0.77.1/PKG-INFO
```

### Comparing `kolena-0.77.0/LICENSE` & `kolena-0.77.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/LICENSE_HEADER` & `kolena-0.77.1/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/README.md` & `kolena-0.77.1/README.md`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/__init__.py` & `kolena-0.77.1/kolena/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/__init__.py` & `kolena-0.77.1/kolena/_api/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/__init__.py` & `kolena-0.77.1/kolena/_api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/batched_load.py` & `kolena-0.77.1/kolena/_api/v1/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/client_log.py` & `kolena-0.77.1/kolena/_api/v1/client_log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/core.py` & `kolena-0.77.1/kolena/_api/v1/core.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/detection.py` & `kolena-0.77.1/kolena/_api/v1/detection.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/fr.py` & `kolena-0.77.1/kolena/_api/v1/fr.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/generic.py` & `kolena-0.77.1/kolena/_api/v1/generic.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/repository.py` & `kolena-0.77.1/kolena/_api/v1/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/token.py` & `kolena-0.77.1/kolena/_api/v1/token.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_api/v1/workflow.py` & `kolena-0.77.1/kolena/_api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/__init__.py` & `kolena-0.77.1/kolena/_experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/__init__.py` & `kolena-0.77.1/kolena/_experimental/object_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/evaluator.py` & `kolena-0.77.1/kolena/_experimental/object_detection/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/evaluator_multiclass.py` & `kolena-0.77.1/kolena/_experimental/object_detection/evaluator_multiclass.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/evaluator_single_class.py` & `kolena-0.77.1/kolena/_experimental/object_detection/evaluator_single_class.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/utils.py` & `kolena-0.77.1/kolena/_experimental/object_detection/utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_experimental/object_detection/workflow.py` & `kolena-0.77.1/kolena/_experimental/object_detection/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_extras/__init__.py` & `kolena-0.77.1/kolena/_extras/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_extras/metrics/__init__.py` & `kolena-0.77.1/kolena/_extras/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_extras/metrics/sklearn.py` & `kolena-0.77.1/kolena/_extras/metrics/sklearn.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/__init__.py` & `kolena-0.77.1/kolena/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/asset_path_mapper.py` & `kolena-0.77.1/kolena/_utils/asset_path_mapper.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/batched_load.py` & `kolena-0.77.1/kolena/_utils/batched_load.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/cli.py` & `kolena-0.77.1/kolena/_utils/cli.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/consts.py` & `kolena-0.77.1/kolena/_utils/consts.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/dataframes/__init__.py` & `kolena-0.77.1/kolena/_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/dataframes/validators.py` & `kolena-0.77.1/kolena/_utils/dataframes/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/datatypes.py` & `kolena-0.77.1/kolena/_utils/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/endpoints.py` & `kolena-0.77.1/kolena/_utils/endpoints.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/frozen.py` & `kolena-0.77.1/kolena/_utils/frozen.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/geometry.py` & `kolena-0.77.1/kolena/_utils/geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/inference_validators.py` & `kolena-0.77.1/kolena/_utils/inference_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/instrumentation.py` & `kolena-0.77.1/kolena/_utils/instrumentation.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/krequests.py` & `kolena-0.77.1/kolena/_utils/krequests.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/log.py` & `kolena-0.77.1/kolena/_utils/log.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/repository.py` & `kolena-0.77.1/kolena/_utils/repository.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/serde.py` & `kolena-0.77.1/kolena/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/serializable.py` & `kolena-0.77.1/kolena/_utils/serializable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/state.py` & `kolena-0.77.1/kolena/_utils/state.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/uninstantiable.py` & `kolena-0.77.1/kolena/_utils/uninstantiable.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/_utils/validators.py` & `kolena-0.77.1/kolena/_utils/validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/__init__.py` & `kolena-0.77.1/kolena/classification/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/metadata.py` & `kolena-0.77.1/kolena/classification/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/model.py` & `kolena-0.77.1/kolena/classification/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/multiclass/__init__.py` & `kolena-0.77.1/kolena/classification/multiclass/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/multiclass/_utils.py` & `kolena-0.77.1/kolena/classification/multiclass/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/multiclass/evaluator.py` & `kolena-0.77.1/kolena/classification/multiclass/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/multiclass/test_run.py` & `kolena-0.77.1/kolena/classification/multiclass/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/multiclass/workflow.py` & `kolena-0.77.1/kolena/classification/multiclass/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/test_case.py` & `kolena-0.77.1/kolena/classification/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/test_config.py` & `kolena-0.77.1/kolena/classification/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/test_image.py` & `kolena-0.77.1/kolena/classification/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/test_run.py` & `kolena-0.77.1/kolena/classification/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/classification/test_suite.py` & `kolena-0.77.1/kolena/classification/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/__init__.py` & `kolena-0.77.1/kolena/detection/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_datatypes.py` & `kolena-0.77.1/kolena/detection/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/__init__.py` & `kolena-0.77.1/kolena/detection/_internal/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/datatypes.py` & `kolena-0.77.1/kolena/detection/_internal/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/ground_truth.py` & `kolena-0.77.1/kolena/detection/_internal/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/inference.py` & `kolena-0.77.1/kolena/detection/_internal/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/metadata.py` & `kolena-0.77.1/kolena/detection/_internal/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/model.py` & `kolena-0.77.1/kolena/detection/_internal/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/test_case.py` & `kolena-0.77.1/kolena/detection/_internal/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/test_config.py` & `kolena-0.77.1/kolena/detection/_internal/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/test_image.py` & `kolena-0.77.1/kolena/detection/_internal/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/test_run.py` & `kolena-0.77.1/kolena/detection/_internal/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/_internal/test_suite.py` & `kolena-0.77.1/kolena/detection/_internal/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/ground_truth.py` & `kolena-0.77.1/kolena/detection/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/inference.py` & `kolena-0.77.1/kolena/detection/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/metadata.py` & `kolena-0.77.1/kolena/detection/metadata.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/model.py` & `kolena-0.77.1/kolena/detection/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/test_case.py` & `kolena-0.77.1/kolena/detection/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/test_config.py` & `kolena-0.77.1/kolena/detection/test_config.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/test_image.py` & `kolena-0.77.1/kolena/detection/test_image.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/test_run.py` & `kolena-0.77.1/kolena/detection/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/detection/test_suite.py` & `kolena-0.77.1/kolena/detection/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/errors.py` & `kolena-0.77.1/kolena/errors.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/__init__.py` & `kolena-0.77.1/kolena/fr/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/_utils.py` & `kolena-0.77.1/kolena/fr/_utils.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/datatypes.py` & `kolena-0.77.1/kolena/fr/datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/model.py` & `kolena-0.77.1/kolena/fr/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/test_case.py` & `kolena-0.77.1/kolena/fr/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/test_images.py` & `kolena-0.77.1/kolena/fr/test_images.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/test_run.py` & `kolena-0.77.1/kolena/fr/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/fr/test_suite.py` & `kolena-0.77.1/kolena/fr/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/initialize.py` & `kolena-0.77.1/kolena/initialize.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/__init__.py` & `kolena-0.77.1/kolena/workflow/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/_datatypes.py` & `kolena-0.77.1/kolena/workflow/_datatypes.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/_validators.py` & `kolena-0.77.1/kolena/workflow/_validators.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/annotation.py` & `kolena-0.77.1/kolena/workflow/annotation.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/asset.py` & `kolena-0.77.1/kolena/workflow/asset.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/define_workflow.py` & `kolena-0.77.1/kolena/workflow/define_workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/evaluator.py` & `kolena-0.77.1/kolena/workflow/evaluator.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/evaluator_function.py` & `kolena-0.77.1/kolena/workflow/evaluator_function.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/ground_truth.py` & `kolena-0.77.1/kolena/workflow/ground_truth.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/inference.py` & `kolena-0.77.1/kolena/workflow/inference.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/metrics/__init__.py` & `kolena-0.77.1/kolena/workflow/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/metrics/_formula.py` & `kolena-0.77.1/kolena/workflow/metrics/_formula.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/metrics/_geometry.py` & `kolena-0.77.1/kolena/workflow/metrics/_geometry.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/model.py` & `kolena-0.77.1/kolena/workflow/model.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/plot.py` & `kolena-0.77.1/kolena/workflow/plot.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/test_case.py` & `kolena-0.77.1/kolena/workflow/test_case.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/test_run.py` & `kolena-0.77.1/kolena/workflow/test_run.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/test_sample.py` & `kolena-0.77.1/kolena/workflow/test_sample.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/test_suite.py` & `kolena-0.77.1/kolena/workflow/test_suite.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/visualization/__init__.py` & `kolena-0.77.1/kolena/workflow/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/visualization/_activation_map.py` & `kolena-0.77.1/kolena/workflow/visualization/_activation_map.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/kolena/workflow/workflow.py` & `kolena-0.77.1/kolena/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `kolena-0.77.0/pyproject.toml` & `kolena-0.77.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kolena"
-version = "0.77.0"  # version is automatically set to latest git tag during release process
+version = "0.77.1"  # version is automatically set to latest git tag during release process
 description = "Client for Kolena's machine learning testing platform."
 authors = ["Kolena Engineering <eng@kolena.io>"]
 homepage = "https://kolena.io"
 documentation = "https://docs.kolena.io"
 readme = "README.md"
 license = "Apache-2.0"
 keywords = ["Kolena", "ML", "testing"]
@@ -30,15 +30,15 @@
     { version = ">=1.19", python = ">=3.7,<3.11" },
     { version = ">=1.23", python = ">=3.11" },
 ]
 pandas = [
     { version = ">=1.1,<1.6", python = ">=3.7,<3.11" },
     { version = ">=1.5,<1.6", python = ">=3.11" },
 ]
-pandera = ">=0.9.0,<1"
+pandera = ">=0.9.0,<0.16"
 pydantic = ">=1.8,<2"
 dacite = ">=1.6,<2"
 requests = ">=2.20,<2.30" # TODO: revert upper bound when urllib3 situation sorts out: https://github.com/psf/requests/issues/6432
 requests-toolbelt = "*"
 importlib-metadata = { version = "<5.0", python = "<3.8" }
 tqdm = ">=4,<5"
 Pillow = "^9.1.1"
```

### Comparing `kolena-0.77.0/PKG-INFO` & `kolena-0.77.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolena
-Version: 0.77.0
+Version: 0.77.1
 Summary: Client for Kolena's machine learning testing platform.
 Home-page: https://kolena.io
 License: Apache-2.0
 Keywords: Kolena,ML,testing
 Author: Kolena Engineering
 Author-email: eng@kolena.io
 Requires-Python: >=3.7.1,<3.12
@@ -31,15 +31,15 @@
 Requires-Dist: dacite (>=1.6,<2)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: importlib-metadata (<5.0) ; python_version < "3.8"
 Requires-Dist: numpy (>=1.19) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: numpy (>=1.23) ; python_version >= "3.11"
 Requires-Dist: pandas (>=1.1,<1.6) ; python_version >= "3.7" and python_version < "3.11"
 Requires-Dist: pandas (>=1.5,<1.6) ; python_version >= "3.11"
-Requires-Dist: pandera (>=0.9.0,<1)
+Requires-Dist: pandera (>=0.9.0,<0.16)
 Requires-Dist: pyarrow (>=8)
 Requires-Dist: pydantic (>=1.8,<2)
 Requires-Dist: requests (>=2.20,<2.30)
 Requires-Dist: requests-toolbelt
 Requires-Dist: retrying (>=1.3.3,<2.0.0)
 Requires-Dist: scikit-learn (>=1.0,<1.0.3) ; (python_full_version >= "3.7.1" and python_version < "3.8") and (extra == "metrics")
 Requires-Dist: scikit-learn (>=1.2,<2) ; (python_version >= "3.8") and (extra == "metrics")
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kolena Version: 0.77.0 Summary: Client for Kolena's
+Metadata-Version: 2.1 Name: kolena Version: 0.77.1 Summary: Client for Kolena's
 machine learning testing platform. Home-page: https://kolena.io License:
 Apache-2.0 Keywords: Kolena,ML,testing Author: Kolena Engineering Author-email:
 eng@kolena.io Requires-Python: >=3.7.1,<3.12 Classifier: Development Status ::
 4 - Beta Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Natural Language :: English Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -16,15 +16,15 @@
 Extra: metrics Requires-Dist: Pillow (>=9.1.1,<10.0.0) Requires-Dist: Shapely
 (>=1.8.5,<2.0.0) Requires-Dist: click (>=8.1.3,<9.0.0) Requires-Dist: dacite
 (>=1.6,<2) Requires-Dist: deprecation (>=2.1.0,<3.0.0) Requires-Dist:
 importlib-metadata (<5.0) ; python_version < "3.8" Requires-Dist: numpy
 (>=1.19) ; python_version >= "3.7" and python_version < "3.11" Requires-Dist:
 numpy (>=1.23) ; python_version >= "3.11" Requires-Dist: pandas (>=1.1,<1.6) ;
 python_version >= "3.7" and python_version < "3.11" Requires-Dist: pandas
-(>=1.5,<1.6) ; python_version >= "3.11" Requires-Dist: pandera (>=0.9.0,<1)
+(>=1.5,<1.6) ; python_version >= "3.11" Requires-Dist: pandera (>=0.9.0,<0.16)
 Requires-Dist: pyarrow (>=8) Requires-Dist: pydantic (>=1.8,<2) Requires-Dist:
 requests (>=2.20,<2.30) Requires-Dist: requests-toolbelt Requires-Dist:
 retrying (>=1.3.3,<2.0.0) Requires-Dist: scikit-learn (>=1.0,<1.0.3) ;
 (python_full_version >= "3.7.1" and python_version < "3.8") and (extra ==
 "metrics") Requires-Dist: scikit-learn (>=1.2,<2) ; (python_version >= "3.8")
 and (extra == "metrics") Requires-Dist: termcolor (>=1.1.0,<2.0.0) Requires-
 Dist: tqdm (>=4,<5) Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) ;
```

