# Comparing `tmp/waffle_hub-0.2.5.tar.gz` & `tmp/waffle_hub-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "waffle_hub-0.2.5.tar", last modified: Sat Jun 24 03:57:50 2023, max compression
+gzip compressed data, was "waffle_hub-0.2.6.tar", last modified: Mon Jul 17 01:46:18 2023, max compression
```

## Comparing `waffle_hub-0.2.5.tar` & `waffle_hub-0.2.6.tar`

### file list

```diff
@@ -1,86 +1,87 @@
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/LICENSE
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/MANIFEST.in
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3349 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/README.md
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-06-24 03:55:49.000000 waffle_hub-0.2.5/requirements.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/setup.cfg
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/setup.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/tests/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7833 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    14759 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/tests/test_dataset.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4581 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_ddp.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10437 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/tests/test_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2292 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/dataset/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/dataset/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/dataset/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      239 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3267 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/autocare_dlt.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2956 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/coco.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4859 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/transformers.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7226 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/adapter/yolo.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/dataset/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    59997 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/dataset/dataset.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/experimental/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7920 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/auto_label/grounding_dino.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/experimental/serve.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/hub/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/__init__.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10235 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4515 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/config.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5865 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2220 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     9156 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/train_input_helper.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    10577 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/transformers_hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4027 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/config.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    12669 2023-06-16 03:37:26.000000 waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.5/waffle_hub/hub/cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    49030 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/hub.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/hub/model/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/hub/model/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    13900 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/hub/model/wrapper.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/schema/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1169 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/base_schema.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1699 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/configs.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      785 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/schema/evaluate.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/schema/fields/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)    17217 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/annotation.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1455 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/base_field.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     7241 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/category.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2599 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/schema/fields/image.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      537 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/schema/result.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub/utils/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/__init__.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.5/waffle_hub/utils/base_cli.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/callback.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.5/waffle_hub/utils/conversion.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     5616 2023-06-24 03:11:53.000000 waffle_hub-0.2.5/waffle_hub/utils/data.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/draw.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/evaluate.py
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.5/waffle_hub/utils/process.py
-drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-06-24 03:57:50.953846 waffle_hub-0.2.5/waffle_hub.egg-info/
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     4430 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/PKG-INFO
--rw-rw-r--   0 lhj       (1002) lhj       (1003)     2242 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/SOURCES.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/dependency_links.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/entry_points.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/requires.txt
--rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-06-24 03:57:50.000000 waffle_hub-0.2.5/waffle_hub.egg-info/top_level.txt
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.114918 waffle_hub-0.2.6/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    35149 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/LICENSE
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/MANIFEST.in
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4422 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3341 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/README.md
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      386 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/requirements.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       38 2023-07-17 01:46:18.114918 waffle_hub-0.2.6/setup.cfg
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2935 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/setup.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.106917 waffle_hub-0.2.6/tests/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8844 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    18878 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_dataset.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4581 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/tests/test_ddp.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    12717 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/tests/test_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.106917 waffle_hub-0.2.6/waffle_hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2292 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/dataset/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       53 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/dataset/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/dataset/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      419 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7146 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/autocare_dlt.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6516 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/coco.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9006 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/transformers.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    14273 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/adapter/yolo.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      633 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/dataset/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    50432 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/dataset/dataset.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/experimental/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     8261 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/experimental/auto_label/grounding_dino.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2986 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/experimental/serve.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       39 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/hub/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/__init__.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       75 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10199 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4515 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/config.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      129 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1913 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5446 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       77 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2220 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     9156 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/train_input_helper.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    10543 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/transformers_hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       74 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6999 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/config.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13208 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      585 2023-06-16 03:34:36.000000 waffle_hub-0.2.6/waffle_hub/hub/cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    54492 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/hub/hub.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/hub/model/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/hub/model/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    13900 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/hub/model/wrapper.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/schema/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      345 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/schema/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1236 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/base_schema.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1731 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/configs.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      871 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      378 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/schema/evaluate.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/schema/fields/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      138 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)    17259 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/annotation.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1722 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/base_field.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     7283 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/category.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3137 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/schema/fields/image.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      537 2023-06-24 03:11:53.000000 waffle_hub-0.2.6/waffle_hub/schema/result.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub/utils/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        0 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/__init__.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3462 2023-06-16 03:34:37.000000 waffle_hub-0.2.6/waffle_hub/utils/base_cli.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     3694 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/callback.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     1686 2023-06-12 07:00:05.000000 waffle_hub-0.2.6/waffle_hub/utils/conversion.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     5752 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/utils/data.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4200 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/draw.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4420 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/evaluate.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     6049 2023-07-17 01:45:43.000000 waffle_hub-0.2.6/waffle_hub/utils/metric_logger.py
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      631 2023-06-12 07:51:09.000000 waffle_hub-0.2.6/waffle_hub/utils/process.py
+drwxrwxr-x   0 lhj       (1002) lhj       (1003)        0 2023-07-17 01:46:18.110918 waffle_hub-0.2.6/waffle_hub.egg-info/
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     4422 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/PKG-INFO
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)     2276 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/SOURCES.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)        1 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/dependency_links.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      224 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/entry_points.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)      308 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/requires.txt
+-rw-rw-r--   0 lhj       (1002) lhj       (1003)       11 2023-07-17 01:46:18.000000 waffle_hub-0.2.6/waffle_hub.egg-info/top_level.txt
```

### Comparing `waffle_hub-0.2.5/LICENSE` & `waffle_hub-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/PKG-INFO` & `waffle_hub-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle_hub
-Version: 0.2.5
+Version: 0.2.6
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -77,15 +77,15 @@
   name = "my_classifier",
   task = "classification",
   model_type = "yolov8",
   model_size = "n",
   categories = dataset.get_category_names(),
 )
 hub.train(
-  dataset_path = export_dir,
+  dataset = dataset,
   epochs = 30,
   batch_size = 64,
   image_size=64,
   device="cpu"
 )
 hub.inference(
   source=export_dir,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.5 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle_hub Version: 0.2.6 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -41,16 +41,16 @@
 both python module and CLI for Waffle Hub. Following examples do the exact same
 thing. ## Python Module ```python from waffle_hub.dataset import Dataset
 dataset = Dataset.sample( name = "mnist_classification", task =
 "classification", ) dataset.split( train_ratio = 0.8, val_ratio = 0.1,
 test_ratio = 0.1 ) export_dir = dataset.export("YOLO") from waffle_hub.hub
 import Hub hub = Hub.new( name = "my_classifier", task = "classification",
 model_type = "yolov8", model_size = "n", categories =
-dataset.get_category_names(), ) hub.train( dataset_path = export_dir, epochs =
-30, batch_size = 64, image_size=64, device="cpu" ) hub.inference
+dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
+batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
 train --name my_classifier --dataset-path datasets/mnist_classification/
 exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
```

### Comparing `waffle_hub-0.2.5/README.md` & `waffle_hub-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
   name = "my_classifier",
   task = "classification",
   model_type = "yolov8",
   model_size = "n",
   categories = dataset.get_category_names(),
 )
 hub.train(
-  dataset_path = export_dir,
+  dataset = dataset,
   epochs = 30,
   batch_size = 64,
   image_size=64,
   device="cpu"
 )
 hub.inference(
   source=export_dir,
```

#### html2text {}

```diff
@@ -26,16 +26,16 @@
 both python module and CLI for Waffle Hub. Following examples do the exact same
 thing. ## Python Module ```python from waffle_hub.dataset import Dataset
 dataset = Dataset.sample( name = "mnist_classification", task =
 "classification", ) dataset.split( train_ratio = 0.8, val_ratio = 0.1,
 test_ratio = 0.1 ) export_dir = dataset.export("YOLO") from waffle_hub.hub
 import Hub hub = Hub.new( name = "my_classifier", task = "classification",
 model_type = "yolov8", model_size = "n", categories =
-dataset.get_category_names(), ) hub.train( dataset_path = export_dir, epochs =
-30, batch_size = 64, image_size=64, device="cpu" ) hub.inference
+dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
+batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
 train --name my_classifier --dataset-path datasets/mnist_classification/
 exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
```

### Comparing `waffle_hub-0.2.5/setup.py` & `waffle_hub-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/tests/test_cli.py` & `waffle_hub-0.2.6/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,24 +42,25 @@
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_coco").exists()
 
 
 def test_dataset_from_yolo(test_dir: Path):
-    url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist_yolo_object_detection_splited.zip"
+    url = "https://raw.githubusercontent.com/snuailab/assets/main/waffle/sample_dataset/mnist_yolo_object_detection.zip"
     yolo_dir = test_dir / "datasets" / "mnist_yolo"
 
     get_file_from_url(url, str(test_dir), True)
-    unzip(str(test_dir / "mnist_yolo_object_detection_splited.zip"), yolo_dir)
+    unzip(str(test_dir / "mnist_yolo_object_detection.zip"), yolo_dir)
 
     cmd = f"python -m waffle_hub.dataset.cli from_yolo \
         --name from_yolo \
         --root-dir {test_dir / 'datasets'} \
         --task object_detection \
+        --yolo-root-dir {yolo_dir} \
         --yaml-path {yolo_dir / 'data.yaml'} \
     "
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "datasets" / "from_yolo").exists()
 
 
@@ -219,14 +220,50 @@
         --verbose \
     '
     ret = run_cli(cmd)
     assert ret.returncode == 0
     assert (test_dir / "hubs" / "test" / "artifacts").exists()
 
 
+def test_hub_train_advance_params(test_dir: Path):
+    cmd = f'python -m waffle_hub.hub.cli new \
+        --backend ultralytics \
+        --root-dir {test_dir / "hubs"} \
+        --name test_adv \
+        --task classification \
+        --model-type yolov8 \
+        --model-size n \
+        --categories [1,2] \
+    '
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+    assert (test_dir / "hubs" / "test").exists()
+
+    cmd = (
+        f'python -m waffle_hub.hub.cli train \
+        --root-dir {test_dir / "hubs"} \
+        --name test_adv \
+        --dataset {test_dir / "datasets" / "from_coco"} \
+        --epochs 1 \
+        --batch-size 4 \
+        --image-size 16 \
+        --learning-rate 0.001 \
+        --letter-box \
+        --device cpu \
+        --workers 0 \
+        --seed 0 \
+        --verbose \
+    '
+        + ' --advance_params "{box: 3}"'
+    )
+    ret = run_cli(cmd)
+    assert ret.returncode == 0
+    assert (test_dir / "hubs" / "test" / "artifacts").exists()
+
+
 def test_hub_inference(test_dir: Path):
     cmd = f'python -m waffle_hub.hub.cli inference \
         --root-dir {test_dir / "hubs"} \
         --name test \
         --source {test_dir / "datasets" / "mnist" / "exports" / "YOLO" / "test" / "images" } \
         --confidence-threshold 0.25 \
         --device cpu \
```

### Comparing `waffle_hub-0.2.5/tests/test_dataset.py` & `waffle_hub-0.2.6/tests/test_dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import Counter
 from pathlib import Path
 
 import pytest
 from waffle_utils.file.io import load_json, save_json
+from waffle_utils.file.search import get_image_files
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.schema.fields import Annotation, Category, Image
 from waffle_hub.utils.data import ImageDataset, LabeledDataset
 
 
@@ -164,50 +165,85 @@
 
 def _split(dataset_name, root_dir):
     dataset = Dataset.load(dataset_name, root_dir=root_dir)
 
     dataset.split(0.8)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) + len(val_ids) == len(dataset.get_images())
+    assert len(test_ids) == 0
 
     dataset.split(0.445446, 0.554554)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) + len(val_ids) == len(dataset.get_images())
+    assert len(test_ids) == 0
 
     dataset.split(0.4, 0.4, 0.2)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(train_ids) + len(val_ids) + len(test_ids) == len(dataset.get_images())
 
     dataset.split(0.99999999999999, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
-    assert len(dataset.get_categories()) == len(val_ids) == len(test_ids)
+    assert len(dataset.get_categories()) == len(val_ids)
+    assert len(test_ids) == 0
 
     dataset.split(0.00000000000001, 0.0)
     train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
     assert len(dataset.get_categories()) == len(train_ids)
+    assert len(test_ids) == 0
 
     with pytest.raises(ValueError):
         dataset.split(0.0, 0.2)
 
     with pytest.raises(ValueError):
         dataset.split(0.9, 0.2)
 
 
 def _export(dataset_name, task: TaskType, root_dir):
     dataset = Dataset.load(dataset_name, root_dir=root_dir)
     dataset.split(0.05)
 
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
-        dataset.export("coco")
+        export_dir = Path(dataset.export("coco"))
+        import_ds = Dataset.from_coco(
+            name=f"{task}_import_coco",
+            task=task,
+            coco_file=list(export_dir.glob("*.json")),
+            coco_root_dir=export_dir / "images",
+            root_dir=root_dir,
+        )
+        assert len(dataset.get_images()) == len(import_ds.get_images())
     if task in [TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION, TaskType.CLASSIFICATION]:
-        dataset.export("yolo")
+        export_dir = Path(dataset.export("yolo"))
+        import_ds = Dataset.from_yolo(
+            name=f"{task}_import_yolo",
+            task=task,
+            yolo_root_dir=export_dir,
+            yaml_path=export_dir / "data.yaml" if task != TaskType.CLASSIFICATION else None,
+            root_dir=root_dir,
+        )
+        assert len(dataset.get_images()) == len(import_ds.get_images())
     if task in [TaskType.OBJECT_DETECTION, TaskType.CLASSIFICATION]:
-        dataset.export("transformers")
+        export_dir = Path(dataset.export("transformers"))
+        import_ds = Dataset.from_transformers(
+            name=f"{task}_import_transformers",
+            task=task,
+            dataset_dir=export_dir,
+            root_dir=root_dir,
+        )
+        assert len(dataset.get_images()) == len(import_ds.get_images())
     if task in [TaskType.OBJECT_DETECTION, TaskType.TEXT_RECOGNITION, TaskType.CLASSIFICATION]:
-        dataset.export("autocare_dlt")
+        export_dir = Path(dataset.export("autocare_dlt"))
+        import_ds = Dataset.from_autocare_dlt(
+            name=f"{task}_import_autocare_dlt",
+            task=task,
+            coco_file=list(export_dir.glob("*.json")),
+            coco_root_dir=export_dir / "images",
+            root_dir=root_dir,
+        )
+        assert len(dataset.get_images()) == len(import_ds.get_images())
 
 
 # test dummy
 def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
     dataset = Dataset.dummy(
         name=dataset_name,
         task=task,
@@ -240,47 +276,14 @@
     ]:
         _total_dummy(f"dummy_{task}", task, 100, 5, 10, tmpdir)
 
     with pytest.raises(ValueError):
         _total_dummy("dummy", TaskType.CLASSIFICATION, 3, 3, 0, tmpdir)
 
 
-# test dummy
-def _dummy(dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir):
-    dataset = Dataset.dummy(
-        name=dataset_name,
-        task=task,
-        image_num=image_num,
-        category_num=category_num,
-        unlabeled_image_num=unlabeled_image_num,
-        root_dir=root_dir,
-    )
-    assert len(dataset.get_images()) == image_num
-    assert len(dataset.get_categories()) == category_num
-    assert len(dataset.get_images(labeled=False)) == unlabeled_image_num
-
-
-def _total_dummy(
-    dataset_name, task: TaskType, image_num, category_num, unlabeled_image_num, root_dir
-):
-    _dummy(dataset_name, task, image_num, category_num, unlabeled_image_num, root_dir)
-    _load(dataset_name, root_dir)
-    _clone(dataset_name, root_dir)
-    _split(dataset_name, root_dir)
-    _export(dataset_name, task, root_dir)
-
-
-def test_dummy(tmpdir):
-    for task in [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]:
-        _total_dummy(f"dummy_{task}", task, 100, 5, 10, tmpdir)
-
-    with pytest.raises(ValueError):
-        _total_dummy("dummy", TaskType.CLASSIFICATION, 3, 3, 0, tmpdir)
-
-
 # test coco
 def _from_coco(dataset_name, task: TaskType, coco_path, root_dir):
     dataset = Dataset.from_coco(
         name=dataset_name,
         task=task,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
@@ -326,14 +329,83 @@
 @pytest.mark.parametrize(
     "task", [TaskType.CLASSIFICATION, TaskType.OBJECT_DETECTION, TaskType.INSTANCE_SEGMENTATION]
 )
 def test_coco(coco_path, tmpdir, task):
     _total_coco(f"coco_{task}", task, coco_path, tmpdir)
 
 
+# test ultralytics
+def test_yolo_classification(yolo_classification_path: Path, tmpdir: Path):
+    dataset_name = "yolo_classification"
+    root_dir = tmpdir
+
+    dataset = Dataset.from_yolo(
+        name=dataset_name,
+        task=TaskType.CLASSIFICATION,
+        yolo_root_dir=yolo_classification_path,
+        root_dir=root_dir,
+    )
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 60
+    assert len(val_ids) == 20
+    assert len(test_ids) == 20
+    assert len(dataset.get_images()) == 100
+
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, TaskType.CLASSIFICATION, root_dir)
+
+
+def test_yolo_object_detection(yolo_object_detection_path: Path, tmpdir: Path):
+    dataset_name = "yolo_object_detection"
+    root_dir = tmpdir
+
+    dataset = Dataset.from_yolo(
+        name=dataset_name,
+        task=TaskType.OBJECT_DETECTION,
+        yolo_root_dir=yolo_object_detection_path,
+        yaml_path=yolo_object_detection_path / "data.yaml",
+        root_dir=root_dir,
+    )
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 60
+    assert len(val_ids) == 20
+    assert len(test_ids) == 20
+    assert len(dataset.get_images()) == 100
+
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, TaskType.OBJECT_DETECTION, root_dir)
+
+
+def test_yolo_instance_segmentation(yolo_instance_segmentation_path: Path, tmpdir: Path):
+    dataset_name = "yolo_instance_segmentation"
+    root_dir = tmpdir
+
+    dataset = Dataset.from_yolo(
+        name=dataset_name,
+        task=TaskType.INSTANCE_SEGMENTATION,
+        yolo_root_dir=yolo_instance_segmentation_path,
+        yaml_path=yolo_instance_segmentation_path / "data.yaml",
+        root_dir=root_dir,
+    )
+    train_ids, val_ids, test_ids, unlabeled_ids = dataset.get_split_ids()
+    assert len(train_ids) == 60
+    assert len(val_ids) == 20
+    assert len(test_ids) == 20
+    assert len(dataset.get_images()) == 100
+
+    _load(dataset_name, root_dir)
+    _clone(dataset_name, root_dir)
+    _split(dataset_name, root_dir)
+    _export(dataset_name, TaskType.INSTANCE_SEGMENTATION, root_dir)
+
+
 # test autocare_dlt
 def _from_autocare_dlt(dataset_name, task: TaskType, coco_path, root_dir):
     dataset = Dataset.from_autocare_dlt(
         name=dataset_name,
         task=task,
         coco_file=coco_path / "coco.json",
         coco_root_dir=coco_path / "images",
@@ -496,7 +568,69 @@
     assert len(ds.get_images()) == 100
     assert len(ds.get_annotations()) == 100 + category_1_num
     assert len(ds.get_categories()) == 3
 
     assert category_counts[1] == category_1_num
     assert category_counts[2] == category_2_num
     assert category_counts[3] == category_1_num
+
+
+def test_extract_by_images_ids(tmpdir):
+    ds = Dataset.dummy(
+        name="dummy_for_extract_by_image_ids",
+        root_dir=tmpdir,
+        task=TaskType.OBJECT_DETECTION,
+        image_num=10,
+        category_num=3,
+    )
+
+    extracted_ds = ds.extract_by_image_ids(
+        name="extracted_by_image_ids",
+        root_dir=tmpdir,
+        image_ids=[1, 2],
+    )
+
+    assert extracted_ds.dataset_dir.exists()
+    assert len(extracted_ds.get_images()) == 2
+
+
+def test_extract_by_categories(tmpdir):
+    ds = Dataset.dummy(
+        name="dummy_for_extract_by_categories",
+        root_dir=tmpdir,
+        task=TaskType.OBJECT_DETECTION,
+        image_num=10,
+        category_num=3,
+    )
+
+    extracted_ds = ds.extract_by_categories(
+        name="extracted_by_categories",
+        root_dir=tmpdir,
+        category_ids=[1, 2],
+    )
+
+    assert extracted_ds.dataset_dir.exists()
+    assert len(extracted_ds.get_categories()) == 2
+
+
+@pytest.mark.parametrize(
+    "task",
+    [
+        TaskType.OBJECT_DETECTION,
+        TaskType.CLASSIFICATION,
+        TaskType.INSTANCE_SEGMENTATION,
+        TaskType.TEXT_RECOGNITION,
+    ],
+)
+def test_draw_annotations(tmpdir, task):
+    image_num = 5
+    ds = Dataset.dummy(
+        name=f"dummy_for_draw_annotations_{task}",
+        root_dir=tmpdir,
+        task=task,
+        image_num=image_num,
+        category_num=1,
+    )
+
+    ds.draw_annotations([1, 2])
+    assert ds.draw_dir.exists()
+    assert len(get_image_files(ds.draw_dir)) == 2
```

### Comparing `waffle_hub-0.2.5/tests/test_ddp.py` & `waffle_hub-0.2.6/tests/test_ddp.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/tests/test_hub.py` & `waffle_hub-0.2.6/tests/test_hub.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+import json
+import tempfile
 import time
 from pathlib import Path
 
+import pytest
 import torch
 
 from waffle_hub import TaskType
 from waffle_hub.dataset import Dataset
 from waffle_hub.hub import Hub
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 
 
-def _train(hub, dataset: Dataset, image_size: int, hold: bool = True):
+def _train(hub, dataset: Dataset, image_size: int, advance_params: dict = None, hold: bool = True):
     result: TrainResult = hub.train(
         dataset=dataset,
         epochs=1,
         image_size=image_size,
         batch_size=4,
         pretrained_model=None,
         device="cpu",
         workers=0,
+        advance_params=advance_params,
         hold=hold,
     )
 
     if not hold:
         assert hasattr(result, "callback")
         while not result.callback.is_finished() and not result.callback.is_failed():
             time.sleep(1)
@@ -132,17 +136,17 @@
     hub_class = Hub.get_hub_class(backend)
     assert hub_class == type(hub)
 
     hub_loaded = Hub.load(name, root_dir)
     assert isinstance(hub_loaded, type(hub))
 
 
-def _total(hub, dataset: Dataset, image_size: int, hold: bool = True):
+def _total(hub, dataset: Dataset, image_size: int, advance_params: dict = None, hold: bool = True):
 
-    _train(hub, dataset, image_size, hold=hold)
+    _train(hub, dataset, image_size, advance_params=advance_params, hold=hold)
     _evaluate(hub, dataset, hold=hold)
     _inference(hub, dataset.raw_image_dir, hold=hold)
     _export(hub, half=False, hold=hold)
     # _export(hub, half=True, hold=hold)  # cpu cannot be half
     _feature_extraction(hub, image_size)
     _benchmark(hub, image_size)
     _util(hub)
@@ -194,77 +198,90 @@
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-def test_ultralytics_classification(classification_dataset: Dataset, tmpdir: Path):
+def test_ultralytics_object_detection_advance_params(
+    object_detection_dataset: Dataset, tmpdir: Path
+):
     image_size = 32
-    dataset = classification_dataset
+    dataset = object_detection_dataset
 
     # test hub
-    name = "test_cls"
+    name = "test_det_adv"
     hub = Hub.new(
         name=name,
         backend="ultralytics",
-        task=TaskType.CLASSIFICATION,
+        task=TaskType.OBJECT_DETECTION,
         model_type="yolov8",
         model_size="n",
-        categories=classification_dataset.get_category_names(),
+        categories=dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = Hub.load(name=name, root_dir=tmpdir)
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
-    _total(hub, dataset, image_size)
+    hub.get_default_advance_train_params()
 
+    _total(hub, dataset, image_size, {"box": 4, "cls": 1})
+    hub.delete_artifact()
 
-def test_transformers_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+    with open(str(tmpdir / "adv.json"), "w") as f:
+        json.dump({"box": 4, "cls": 2}, f)
+    _total(hub, dataset, image_size, str(tmpdir / "adv.json"))
+    hub.delete_artifact()
+
+    with pytest.raises(ValueError):
+        _total(hub, dataset, image_size, {"box": 4, "dummy_adv_param": 2})
+
+
+def test_ultralytics_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
-    dataset = object_detection_dataset
+    dataset = classification_dataset
 
     # test hub
-    name = "test_det"
+    name = "test_cls"
     hub = Hub.new(
         name=name,
-        backend="transformers",
-        task=TaskType.OBJECT_DETECTION,
-        model_type="YOLOS",
-        model_size="tiny",
-        categories=object_detection_dataset.get_category_names(),
+        backend="ultralytics",
+        task=TaskType.CLASSIFICATION,
+        model_type="yolov8",
+        model_size="n",
+        categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = Hub.load(name=name, root_dir=tmpdir)
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
     )
 
     _total(hub, dataset, image_size)
 
 
-def test_transformers_classification(classification_dataset: Dataset, tmpdir: Path):
-    image_size = 224
-    dataset = classification_dataset
+def test_transformers_object_detection(object_detection_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = object_detection_dataset
 
     # test hub
-    name = "test_cls"
+    name = "test_det"
     hub = Hub.new(
         name=name,
         backend="transformers",
-        task=TaskType.CLASSIFICATION,
-        model_type="ViT",
+        task=TaskType.OBJECT_DETECTION,
+        model_type="YOLOS",
         model_size="tiny",
-        categories=classification_dataset.get_category_names(),
+        categories=object_detection_dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = Hub.load(name=name, root_dir=tmpdir)
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -323,35 +340,23 @@
     _total(hub, dataset, image_size)
 
 
 def test_autocare_dlt_classification(classification_dataset: Dataset, tmpdir: Path):
     image_size = 32
     dataset = classification_dataset
 
-    # temporal solution
-    super_cat = [[c.supercategory, c.name] for c in dataset.get_categories()]
-    super_cat_dict = {}
-    for super_cat, cat in super_cat:
-        if super_cat not in super_cat_dict:
-            super_cat_dict[super_cat] = []
-        super_cat_dict[super_cat].append(cat)
-    super_cat_dict_list = []
-
-    for super_cat, cat in super_cat_dict.items():
-        super_cat_dict_list.append({super_cat: cat})
-
     # test hub
     name = "test_cls"
     hub = Hub.new(
         name=name,
         backend="autocare_dlt",
         task=TaskType.CLASSIFICATION,
         model_type="Classifier",
         model_size="s",
-        categories=super_cat_dict_list,
+        categories=dataset.get_categories(),
         root_dir=tmpdir,
     )
     hub = Hub.load(name=name, root_dir=tmpdir)
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
@@ -368,15 +373,90 @@
     name = "test_ocr"
     hub = Hub.new(
         name=name,
         backend="autocare_dlt",
         task=TaskType.TEXT_RECOGNITION,
         model_type="TextRecognition",
         model_size="s",
-        categories=dataset.get_category_names(),
+        categories=dataset.get_categories(),
+        root_dir=tmpdir,
+    )
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_ultralytics_classification_without_category(classification_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = classification_dataset
+
+    # test hub
+    name = "test_cls"
+    hub = Hub.new(
+        name=name,
+        backend="ultralytics",
+        task=TaskType.CLASSIFICATION,
+        model_type="yolov8",
+        model_size="n",
+        # categories=classification_dataset.get_category_names(),  # auto detect
+        root_dir=tmpdir,
+    )
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_autocare_dlt_classification_without_category(classification_dataset: Dataset, tmpdir: Path):
+    image_size = 32
+    dataset = classification_dataset
+
+    # test hub
+    name = "test_cls"
+    hub = Hub.new(
+        name=name,
+        backend="autocare_dlt",
+        task=TaskType.CLASSIFICATION,
+        model_type="Classifier",
+        model_size="s",
+        # categories=dataset.get_categories(),
+        root_dir=tmpdir,
+    )
+    hub = Hub.load(name=name, root_dir=tmpdir)
+    hub: Hub = Hub.from_model_config(
+        name=name + "_from_model_config",
+        model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
+        root_dir=tmpdir,
+    )
+
+    _total(hub, dataset, image_size)
+
+
+def test_transformers_classification(classification_dataset: Dataset, tmpdir: Path):
+    image_size = 224
+    dataset = classification_dataset
+
+    # test hub
+    name = "test_cls"
+    hub = Hub.new(
+        name=name,
+        backend="transformers",
+        task=TaskType.CLASSIFICATION,
+        model_type="ViT",
+        model_size="tiny",
+        # categories=classification_dataset.get_category_names(),
         root_dir=tmpdir,
     )
     hub = Hub.load(name=name, root_dir=tmpdir)
     hub: Hub = Hub.from_model_config(
         name=name + "_from_model_config",
         model_config_file=tmpdir / name / Hub.MODEL_CONFIG_FILE,
         root_dir=tmpdir,
```

### Comparing `waffle_hub-0.2.5/waffle_hub/__init__.py` & `waffle_hub-0.2.6/waffle_hub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.5"
+__version__ = "0.2.6"
 
 import enum
 from collections import OrderedDict
 
 BACKEND_MAP = OrderedDict(
     {
         "ultralytics": {
```

### Comparing `waffle_hub-0.2.5/waffle_hub/dataset/adapter/yolo.py` & `waffle_hub-0.2.6/waffle_hub/dataset/adapter/coco.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,225 +1,192 @@
+import logging
 import warnings
 from pathlib import Path
 from typing import Union
 
+import tqdm
+from pycocotools.coco import COCO
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
-from waffle_hub.schema.fields.image import Image
-from waffle_hub.utils.conversion import merge_multi_segment
+from waffle_hub.schema.fields import Annotation, Category, Image
+from waffle_hub.utils.conversion import convert_rle_to_polygon
 
 
-def _check_valid_file_paths(images: list[Image]) -> bool:
-    """Check file paths are valid
-    If the file name includes the words "images" or "labels," an error occurs during training
-
-    Args:
-        images (list[Image]): List of Image
-
-    Returns:
-        bool: True if valid
-    """
-    for image in images:
-        file_path = Path(image.file_name)
-        if "images" in file_path.parts:
-            raise ValueError(
-                f"The file path '{file_path}' is not allowed. Please choose a file path that does not contain the word 'images'"
-            )
-        if "labels" in file_path.parts:
-            raise ValueError(
-                f"The file path '{file_path}' is not allowed. Please choose a file path that does not contain the word 'labels'"
-            )
-    else:
-        return True
-
-
-def _export_yolo_classification(
-    self,
-    export_dir: Path,
-    train_ids: list,
-    val_ids: list,
-    test_ids: list,
-    unlabeled_ids: list,
-):
-    """Export dataset to YOLO format for classification task
-
-    Args:
-        export_dir (Path): Path to export directory
-        train_ids (list): List of train ids
-        val_ids (list): List of validation ids
-        test_ids (list): List of test ids
-        unlabeled_ids (list): List of unlabeled ids
-    """
-    io.make_directory(export_dir)
-
-    for split, image_ids in zip(
-        ["train", "val", "test", "unlabeled"],
-        [train_ids, val_ids, test_ids, unlabeled_ids],
-    ):
-        if len(image_ids) == 0:
-            continue
-
-        split_dir = export_dir / split
-        io.make_directory(split_dir)
-
-        category_names = {c.category_id: c.name for c in self.get_categories()}
-        for image in self.get_images(image_ids):
-            image_path = self.raw_image_dir / image.file_name
-
-            annotations = self.get_annotations(image.image_id)
-            if len(annotations) > 1:
-                warnings.warn(f"Multi label does not support yet. Skipping {image_path}.")
-                continue
-            category_id = annotations[0].category_id
-
-            image_dst_path = split_dir / category_names[category_id] / image.file_name
-            io.copy_file(image_path, image_dst_path, create_directory=True)
-
-
-def _export_yolo_detection(
+def _export_coco(
     self,
     export_dir: Path,
     train_ids: list,
     val_ids: list,
     test_ids: list,
     unlabeled_ids: list,
 ):
-    """Export dataset to YOLO format for detection task
+    """Export dataset to COCO format
 
     Args:
         export_dir (Path): Path to export directory
         train_ids (list): List of train ids
         val_ids (list): List of validation ids
         test_ids (list): List of test ids
         unlabeled_ids (list): List of unlabeled ids
     """
     io.make_directory(export_dir)
 
-    for split, image_ids in zip(
-        ["train", "val", "test", "unlabeled"],
-        [train_ids, val_ids, test_ids, unlabeled_ids],
-    ):
-        if len(image_ids) == 0:
-            continue
-
-        image_dir = export_dir / split / "images"
-        label_dir = export_dir / split / "labels"
-
-        io.make_directory(image_dir)
-        io.make_directory(label_dir)
-
-        for image in self.get_images(image_ids):
-            image_path = self.raw_image_dir / image.file_name
-            image_dst_path = image_dir / image.file_name
-            label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
-            io.copy_file(image_path, image_dst_path, create_directory=True)
-
-            W = image.width
-            H = image.height
-
-            annotations = self.get_annotations(image.image_id)
-            label_txts = []
-            for annotation in annotations:
-                x1, y1, w, h = annotation.bbox
-                x1, w = x1 / W, w / W
-                y1, h = y1 / H, h / H
-                cx, cy = x1 + w / 2, y1 + h / 2
-
-                category_id = annotation.category_id - 1
-
-                label_txts.append(f"{category_id} {cx} {cy} {w} {h}")
-
-            io.make_directory(label_dst_path.parent)
-            with open(label_dst_path, "w") as f:
-                f.write("\n".join(label_txts))
-
-
-def _export_yolo_segmentation(
-    self,
-    export_dir: Path,
-    train_ids: list,
-    val_ids: list,
-    test_ids: list,
-    unlabeled_ids: list,
-):
-    io.make_directory(export_dir)
+    image_dir = export_dir / "images"
 
     for split, image_ids in zip(
         ["train", "val", "test", "unlabeled"],
         [train_ids, val_ids, test_ids, unlabeled_ids],
     ):
         if len(image_ids) == 0:
             continue
 
-        image_dir = export_dir / split / "images"
-        label_dir = export_dir / split / "labels"
-
-        io.make_directory(image_dir)
-        io.make_directory(label_dir)
+        coco = {
+            "categories": [
+                {
+                    "id": category.category_id,
+                    "name": category.name,
+                    "supercategory": category.supercategory,
+                }
+                for category in self.get_categories()
+            ],
+            "images": [],
+            "annotations": [],
+        }
 
         for image in self.get_images(image_ids):
             image_path = self.raw_image_dir / image.file_name
             image_dst_path = image_dir / image.file_name
-            label_dst_path = (label_dir / image.file_name).with_suffix(".txt")
             io.copy_file(image_path, image_dst_path, create_directory=True)
 
-            W = image.width
-            H = image.height
+            d = image.to_dict()
+            image_id = d.pop("image_id")
+            coco["images"].append({"id": image_id, **d})
 
-            annotations = self.get_annotations(image.image_id)
-            label_txts = []
+            annotations = self.get_annotations(image_id)
             for annotation in annotations:
-                x1, y1, w, h = annotation.bbox
-                x1, w = x1 / W, w / W
-                y1, h = y1 / H, h / H
-
-                category_id = annotation.category_id - 1
-
-                segment = merge_multi_segment(annotation.segmentation, (W, H))
-                segment[0::2] = [x / W for x in segment[0::2]]
-                segment[1::2] = [y / H for y in segment[1::2]]
-                segment = " ".join(map(str, segment))
+                d = annotation.to_dict()
+                if d.get("segmentation", None):
+                    if isinstance(d["segmentation"], dict):
+                        d["segmentation"] = convert_rle_to_polygon(d["segmentation"])
+                annotation_id = d.pop("annotation_id")
+                coco["annotations"].append({"id": annotation_id, **d})
 
-                label_txts.append(f"{category_id} {segment}")
+        io.save_json(coco, export_dir / f"{split}.json", create_directory=True)
 
-            io.make_directory(label_dst_path.parent)
-            with open(label_dst_path, "w") as f:
-                f.write("\n".join(label_txts))
 
-
-def export_yolo(self, export_dir: Union[str, Path]) -> str:
-    """Export dataset to YOLO format
+def export_coco(self, export_dir: Union[str, Path]) -> str:
+    """Export dataset to COCO format
 
     Args:
-        export_dir (Union[str, Path]): Path to export directory
+        export_dir (str): Path to export directory
 
     Returns:
         str: Path to export directory
     """
-    _check_valid_file_paths(self.get_images())
-
     export_dir = Path(export_dir)
 
     train_ids, val_ids, test_ids, _ = self.get_split_ids()
 
     if self.task == TaskType.CLASSIFICATION:
-        _export_yolo_classification(self, export_dir, train_ids, val_ids, test_ids, [])
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.OBJECT_DETECTION:
-        _export_yolo_detection(self, export_dir, train_ids, val_ids, test_ids, [])
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     elif self.task == TaskType.INSTANCE_SEGMENTATION:
-        _export_yolo_segmentation(self, export_dir, train_ids, val_ids, test_ids, [])
+        _export_coco(self, export_dir, train_ids, val_ids, test_ids, [])
     else:
         raise ValueError(f"Unsupported task type: {self.task}")
 
-    io.save_yaml(
-        {
-            "path": str(export_dir.absolute()),
-            "train": "train",
-            "val": "val",
-            "test": "test",
-            "names": {category.category_id - 1: category.name for category in self.get_categories()},
-        },
-        export_dir / "data.yaml",
-    )
-
     return str(export_dir)
+
+
+def import_coco(self, coco_files: list[str], coco_root_dirs: list[str]):
+    """
+    Import coco dataset
+
+    Args:
+        coco_files (list[str]): List of coco annotation files
+        coco_root_dirs (list[str]): List of coco root directories
+    """
+    if len(coco_files) == 1:
+        set_names = [None]
+    elif len(coco_files) == 2:
+        set_names = ["train", "val"]
+    elif len(coco_files) == 3:
+        set_names = ["train", "val", "test"]
+    else:
+        raise ValueError("coco_file should have 1, 2, or 3 files.")
+
+    cocos = [COCO(coco_file) for coco_file in coco_files]
+
+    # categories should be same between coco files
+    categories = cocos[0].loadCats(cocos[0].getCatIds())
+    for coco in cocos[1:]:
+        if categories != coco.loadCats(coco.getCatIds()):
+            raise ValueError("categories should be same between coco files.")
+
+    coco_cat_id_to_waffle_cat_id = {}
+    for i, category in enumerate(categories, start=1):
+        coco_category_id = category.pop("id")
+        coco_cat_id_to_waffle_cat_id[coco_category_id] = i
+        self.add_categories([Category.from_dict({**category, "category_id": i}, task=self.task)])
+
+    # import coco dataset
+    total_length = sum([len(coco.getImgIds()) for coco in cocos])
+    logging.info(f"Importing coco dataset. Total length: {total_length}")
+    pgbar = tqdm.tqdm(total=total_length, desc="Importing coco dataset")
+
+    image_id = 1
+    annotation_id = 1
+
+    # parse coco annotation file
+    for coco, coco_root_dir, set_name in tqdm.tqdm(zip(cocos, coco_root_dirs, set_names)):
+
+        image_ids = []
+        for coco_image_id, annotation_dicts in coco.imgToAnns.items():
+            if len(annotation_dicts) == 0:
+                warnings.warn(f"image_id {coco_image_id} has no annotations.")
+                continue
+
+            image_dict = coco.loadImgs(coco_image_id)[0]
+            image_dict.pop("id")
+
+            file_name = image_dict.pop("file_name")
+            image_path = Path(coco_root_dir) / file_name
+            if not image_path.exists():
+                raise FileNotFoundError(f"{image_path} does not exist.")
+
+            if set_name:
+                file_name = f"{set_name}/{file_name}"
+
+            self.add_images(
+                [Image.from_dict({**image_dict, "image_id": image_id, "file_name": file_name})]
+            )
+            io.copy_file(image_path, self.raw_image_dir / file_name, create_directory=True)
+
+            for annotation_dict in annotation_dicts:
+                annotation_dict.pop("id")
+                self.add_annotations(
+                    [
+                        Annotation.from_dict(
+                            {
+                                **annotation_dict,
+                                "image_id": image_id,
+                                "annotation_id": annotation_id,
+                                "category_id": coco_cat_id_to_waffle_cat_id[
+                                    annotation_dict["category_id"]
+                                ],
+                            },
+                            task=self.task,
+                        )
+                    ]
+                )
+                annotation_id += 1
+
+            image_ids.append(image_id)
+            image_id += 1
+            pgbar.update(1)
+
+        if set_name:
+            io.save_json(image_ids, self.set_dir / f"{set_name}.json", create_directory=True)
+
+    pgbar.close()
```

### Comparing `waffle_hub-0.2.5/waffle_hub/dataset/cli.py` & `waffle_hub-0.2.6/waffle_hub/dataset/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/dataset/dataset.py` & `waffle_hub-0.2.6/waffle_hub/dataset/dataset.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,33 +6,34 @@
 import warnings
 from collections import Counter, defaultdict
 from functools import cached_property
 from pathlib import Path
 from tempfile import mkdtemp
 from typing import Union
 
-import cv2
 import PIL.Image
 import tqdm
-from pycocotools.coco import COCO
 from waffle_utils.file import io, network
-from waffle_utils.file.search import get_files, get_image_files
+from waffle_utils.image.io import load_image, save_image
 from waffle_utils.log import datetime_now
 from waffle_utils.utils import type_validator
 
-from datasets import Dataset as HFDataset
-from datasets import DatasetDict, load_from_disk
 from waffle_hub import EXPORT_MAP, DataType, SplitMethod, TaskType
 from waffle_hub.dataset.adapter import (
     export_autocare_dlt,
     export_coco,
     export_transformers,
     export_yolo,
+    import_autocare_dlt,
+    import_coco,
+    import_transformers,
+    import_yolo,
 )
 from waffle_hub.schema import Annotation, Category, DatasetInfo, Image
+from waffle_hub.utils.draw import draw_results
 
 logger = logging.getLogger(__name__)
 
 
 class Dataset:
     DEFAULT_DATASET_ROOT_DIR = Path("./datasets")
     DATASET_INFO_FILE_NAME = Path("info.yaml")
@@ -40,35 +41,44 @@
     RAW_IMAGE_DIR = Path("raw")
     IMAGE_DIR = Path("images")
     ANNOTATION_DIR = Path("annotations")
     CATEGORY_DIR = Path("categories")
     PREDICTION_DIR = Path("predictions")
     EXPORT_DIR = Path("exports")
     SET_DIR = Path("sets")
+    DRAW_DIR = Path("draws")
 
     TRAIN_SET_FILE_NAME = Path("train.json")
     VAL_SET_FILE_NAME = Path("val.json")
     TEST_SET_FILE_NAME = Path("test.json")
     UNLABELED_SET_FILE_NAME = Path("unlabeled.json")
 
     MINIMUM_TRAINABLE_IMAGE_NUM_PER_CATEGORY = 3
 
     def __init__(
         self,
         name: str,
         task: Union[str, TaskType],
+        categories: list[Union[str, int, float, dict, Category]] = None,
         created: str = None,
         root_dir: str = None,
     ):
         self.name = name
         self.task = task
         self.created = created
 
         self.root_dir = root_dir
 
+        if not self.initialized():
+            self.initialize()
+            self.set_categories(categories)
+            self.save_dataset_info()
+        else:  # for backward compatibility
+            self.save_dataset_info()
+
     def __repr__(self):
         return self.get_dataset_info().__repr__()
 
     # properties
     @property
     def name(self):
         return self.__name
@@ -86,14 +96,132 @@
     def task(self, v):
         v = str(v).upper()
         if v not in TaskType:
             raise ValueError(f"Invalid task type: {v}" f"Available task types: {list(TaskType)}")
         self.__task = v
 
     @property
+    def categories(self) -> list[Category]:
+        return self.get_categories()
+
+    def set_categories(self, v):
+        if v is None or len(v) == 0:
+            v = []
+        elif isinstance(v[0], dict):
+            v = [
+                getattr(Category, self.task.lower())(
+                    **{
+                        **category,
+                        "category_id": category.get("category_id", i),
+                    }
+                )
+                for i, category in enumerate(v, start=1)
+            ]
+        elif isinstance(v[0], (str, int, float)):
+            v = [
+                getattr(Category, self.task.lower())(
+                    category_id=i,
+                    supercategory="object",
+                    name=str(category),
+                )
+                for i, category in enumerate(v, start=1)
+            ]
+        elif isinstance(v[0], Category):
+            pass
+
+        self.add_categories(v)
+
+    def extract_by_image_ids(
+        self, name: str, image_ids: list[int], root_dir: str = None
+    ) -> "Dataset":
+        """
+        Extract a new dataset by image ids
+
+        Args:
+            name (str): Name of the new dataset
+            image_ids (list[int]): Image ids to extract
+            root_dir (str, optional): Root directory of the new dataset. Defaults to None.
+
+        Returns:
+            Dataset: Extracted dataset
+
+        """
+        ds = Dataset.new(
+            name=name,
+            task=self.task,
+            root_dir=root_dir,
+        )
+
+        try:
+            ds.add_categories(self.get_categories())
+            for image in self.get_images(image_ids):
+                annotations = self.get_annotations(image.image_id)
+                io.copy_file(
+                    self.raw_image_dir / image.file_name, ds.raw_image_dir / image.file_name
+                )
+                ds.add_images([image])
+                ds.add_annotations(annotations)
+
+        except Exception as e:
+            ds.delete()
+            raise e
+
+        return ds
+
+    def extract_by_categories(
+        self, name: str, category_ids: list[int], root_dir: str = None
+    ) -> "Dataset":
+        """
+        Extract a new dataset by categories
+
+        Args:
+            name (str): Name of the new dataset
+            category_ids (list[int]): Category IDs to extract
+            root_dir (str, optional): Root directory of the new dataset. Defaults to None.
+
+        Returns (Dataset): New dataset
+        """
+        ds = Dataset.new(
+            name=name,
+            task=self.task,
+            root_dir=root_dir,
+        )
+        try:
+            category_old2new = {}
+            for new_category_id, category_id in enumerate(category_ids, start=1):
+                category_old2new[category_id] = new_category_id
+                categories = self.get_categories([category_id])
+                for category in categories:
+                    category.category_id = new_category_id
+                ds.add_categories(categories)
+
+            for image in self.get_images():
+                annotations = list(
+                    filter(
+                        lambda ann: ann.category_id in category_ids,
+                        self.get_annotations(image.image_id),
+                    )
+                )
+                for annotation in annotations:
+                    annotation.category_id = category_old2new[annotation.category_id]
+
+                if annotations:
+                    io.copy_file(
+                        self.raw_image_dir / image.file_name, ds.raw_image_dir / image.file_name
+                    )
+                    ds.add_images([image])
+                    ds.add_annotations(annotations)
+
+        except Exception as e:
+            ds.delete()
+            raise e
+
+        return ds
+
+    @property
     def created(self):
         return self.__created
 
     @created.setter
     def created(self, v):
         self.__created = v or datetime_now()
 
@@ -150,14 +278,18 @@
         return self.dataset_dir / Dataset.EXPORT_DIR
 
     @cached_property
     def set_dir(self) -> Path:
         return self.dataset_dir / Dataset.SET_DIR
 
     @cached_property
+    def draw_dir(self) -> Path:
+        return self.dataset_dir / Dataset.DRAW_DIR
+
+    @cached_property
     def train_set_file(self) -> Path:
         return self.set_dir / Dataset.TRAIN_SET_FILE_NAME
 
     @cached_property
     def val_set_file(self) -> Path:
         return self.set_dir / Dataset.VAL_SET_FILE_NAME
 
@@ -166,15 +298,15 @@
         return self.set_dir / Dataset.TEST_SET_FILE_NAME
 
     @cached_property
     def unlabeled_set_file(self) -> Path:
         return self.set_dir / Dataset.UNLABELED_SET_FILE_NAME
 
     def get_category_names(self) -> list[str]:
-        return [c.name for c in sorted(self.get_categories(), key=lambda c: c.category_id)]
+        return [category.name for category in self.categories]
 
     def get_image_to_annotations(self) -> dict[int, list[Annotation]]:
         image_to_annotations = defaultdict(list)
         for annotation in self.get_annotations():
             image_to_annotations[annotation.image_id].append(annotation)
         return dict(image_to_annotations)
 
@@ -222,23 +354,30 @@
             category_id: len(annotations)
             for category_id, annotations in self.get_category_to_annotations().items()
         }
         return num_annotations_per_category
 
     # factories
     @classmethod
-    def new(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
+    def new(
+        cls,
+        name: str,
+        task: str,
+        categories: list[Union[str, int, float, dict, Category]] = None,
+        root_dir: str = None,
+    ) -> "Dataset":
         """
         Create New Dataset.
         This method creates a new dataset directory and initialize dataset info file.
         If you have other types of data, you can use from_* methods to create a dataset.
 
         Args:
             name (str): Dataset name
             task (str): Dataset task
+            categories (list[Union[str, int, float, dict, Category]]): Dataset categories
             root_dir (str, optional): Dataset root directory. Defaults to None.
 
         Raises:
             FileExistsError: if dataset name already exists
 
         Examples:
             >>> ds = Dataset.new("my_dataset", "CLASSIFICATION")
@@ -246,21 +385,25 @@
             'my_dataset'  # dataset name
             >>> ds.task  # dataset task
             'CLASSIFICATION'
 
         Returns:
             Dataset: Dataset Class
         """
-        ds = cls(name=name, task=task, root_dir=root_dir)
-        if ds.initialized():
-            raise FileExistsError(
-                f'{ds.dataset_dir} already exists. try another name or Dataset.load("{name}")'
-            )
-        ds.initialize()
-        return ds
+        root_dir = Dataset.parse_root_dir(root_dir)
+
+        if name in Dataset.get_dataset_list(root_dir):
+            raise FileExistsError(f"Dataset {name} already exists.")
+
+        try:
+            return cls(name=name, task=task, categories=categories, root_dir=root_dir)
+        except Exception as e:
+            if (root_dir / name).exists():
+                io.remove_directory(root_dir / name)
+            raise e
 
     @classmethod
     def clone(
         cls,
         src_name: str,
         name: str,
         src_root_dir: str = None,
@@ -288,23 +431,28 @@
             'my_dataset_clone'  # cloned dataset name
             >>> ds.task
             'CLASSIFICATION'   # original dataset task
 
         Returns:
             Dataset: Dataset Class
         """
-        src_ds = Dataset.load(src_name, src_root_dir)
-        if not src_ds.initialized():
-            raise FileNotFoundError(f"{src_ds.dataset_dir} has not been created by Waffle.")
-
-        ds = Dataset.new(name, src_ds.task, root_dir)
-        io.copy_files_to_directory(src_ds.dataset_dir, ds.dataset_dir, create_directory=True)
-        ds.initialize()
+        root_dir = Dataset.parse_root_dir(root_dir)
 
-        return ds
+        try:
+            src_ds = Dataset.load(src_name, src_root_dir)
+
+            ds = Dataset.new(name=name, task=src_ds.task, root_dir=root_dir)
+            io.copy_files_to_directory(src_ds.dataset_dir, ds.dataset_dir, create_directory=True)
+            ds.save_dataset_info()
+
+            return ds
+        except Exception as e:
+            if (root_dir / name).exists():
+                io.remove_directory(root_dir / name)
+            raise e
 
     @classmethod
     def dummy(
         cls,
         name: str,
         task: str,
         image_num: int = 100,
@@ -329,15 +477,15 @@
         Examples:
             >>> ds = Dataset.dummy("my_dataset", "CLASSIFICATION", image_num=100, category_num=10)
             >>> len(ds.get_images())
             100
             >>> len(ds.get_categories())
             10
         """
-        ds = Dataset.new(name, task, root_dir)
+        ds = Dataset.new(name=name, task=task, root_dir=root_dir)
 
         try:
             for category_id in range(1, category_num + 1):
 
                 if task == TaskType.CLASSIFICATION:
                     category = Category.classification(
                         category_id=category_id,
@@ -614,122 +762,44 @@
             # You can give coco_file as list.
             # Given coco files are regarded as [train, [val, [test]]] json files.
             >>> ds = Dataset.from_coco("my_dataset", "object_detection", ["coco_train.json", "coco_val.json"], ["coco_train_root", "coco_val_root"])
 
         Returns:
             Dataset: Dataset Class
         """
-        ds = Dataset.new(name, task, root_dir)
-        ds.initialize()
-
-        if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
-            if len(coco_file) != len(coco_root_dir):
-                raise ValueError("coco_file and coco_root_dir should have same length.")
-        if not isinstance(coco_file, list) and isinstance(coco_root_dir, list):
-            raise ValueError(
-                "ambiguous input. The number of coco_file should be same or greater than coco_root_dir."
-            )
-        if not isinstance(coco_file, list):
-            coco_file = [coco_file]
-        if not isinstance(coco_root_dir, list):
-            coco_root_dir = [coco_root_dir] * len(coco_file)
-
-        coco_files = coco_file
-        coco_root_dirs = coco_root_dir
-
-        if len(coco_files) == 1:
-            set_names = [None]
-        elif len(coco_files) == 2:
-            set_names = ["train", "val"]
-        elif len(coco_files) == 3:
-            set_names = ["train", "val", "test"]
-        else:
-            raise ValueError("coco_file should have 1, 2, or 3 files.")
-
-        cocos = [COCO(coco_file) for coco_file in coco_files]
-
-        # categories should be same between coco files
-        categories = cocos[0].loadCats(cocos[0].getCatIds())
-        for coco in cocos[1:]:
-            if categories != coco.loadCats(coco.getCatIds()):
-                raise ValueError("categories should be same between coco files.")
-
-        coco_cat_id_to_waffle_cat_id = {}
-        for i, category in enumerate(categories, start=1):
-            coco_category_id = category.pop("id")
-            coco_cat_id_to_waffle_cat_id[coco_category_id] = i
-            ds.add_categories([Category.from_dict({**category, "category_id": i}, task=ds.task)])
-
-        # import coco dataset
-        total_length = sum([len(coco.getImgIds()) for coco in cocos])
-        logging.info(f"Importing coco dataset. Total length: {total_length}")
-        pgbar = tqdm.tqdm(total=total_length, desc="Importing coco dataset")
-
-        image_id = 1
-        annotation_id = 1
-
-        # parse coco annotation file
-        for coco, coco_root_dir, set_name in tqdm.tqdm(zip(cocos, coco_root_dirs, set_names)):
-
-            image_ids = []
-            for coco_image_id, annotation_dicts in coco.imgToAnns.items():
-                if len(annotation_dicts) == 0:
-                    warnings.warn(f"image_id {coco_image_id} has no annotations.")
-                    continue
-
-                image_dict = coco.loadImgs(coco_image_id)[0]
-                image_dict.pop("id")
-
-                file_name = image_dict.pop("file_name")
-                image_path = Path(coco_root_dir) / file_name
-                if not image_path.exists():
-                    raise FileNotFoundError(f"{image_path} does not exist.")
+        ds = Dataset.new(name=name, task=task, root_dir=root_dir)
 
-                if set_name:
-                    file_name = f"{set_name}/{file_name}"
-
-                ds.add_images(
-                    [Image.from_dict({**image_dict, "image_id": image_id, "file_name": file_name})]
+        try:
+            if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+                if len(coco_file) != len(coco_root_dir):
+                    raise ValueError("coco_file and coco_root_dir should have same length.")
+            if not isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+                raise ValueError(
+                    "ambiguous input. The number of coco_file should be same or greater than coco_root_dir."
                 )
-                io.copy_file(image_path, ds.raw_image_dir / file_name, create_directory=True)
-
-                for annotation_dict in annotation_dicts:
-                    annotation_dict.pop("id")
-                    ds.add_annotations(
-                        [
-                            Annotation.from_dict(
-                                {
-                                    **annotation_dict,
-                                    "image_id": image_id,
-                                    "annotation_id": annotation_id,
-                                    "category_id": coco_cat_id_to_waffle_cat_id[
-                                        annotation_dict["category_id"]
-                                    ],
-                                },
-                                task=ds.task,
-                            )
-                        ]
-                    )
-                    annotation_id += 1
-
-                image_ids.append(image_id)
-                image_id += 1
-                pgbar.update(1)
-
-            if set_name:
-                io.save_json(image_ids, ds.set_dir / f"{set_name}.json", create_directory=True)
-
-        pgbar.close()
+            if not isinstance(coco_file, list):
+                coco_file = [coco_file]
+            if not isinstance(coco_root_dir, list):
+                coco_root_dir = [coco_root_dir] * len(coco_file)
+
+            coco_files = coco_file
+            coco_root_dirs = coco_root_dir
+
+            import_coco(ds, coco_files, coco_root_dirs)
+
+            if len(coco_files) == 2:
+                logger.info("copying val set to test set")
+                io.copy_file(ds.val_set_file, ds.test_set_file, create_directory=True)
 
-        if len(coco_files) == 2:
-            logging.info("copying val set to test set")
-            io.copy_file(ds.val_set_file, ds.test_set_file, create_directory=True)
+            # TODO: add unlabeled set
+            io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
-        # TODO: add unlabeled set
-        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+        except Exception as e:
+            ds.delete()
+            raise e
 
         return ds
 
     @classmethod
     def from_autocare_dlt(
         cls,
         name: str,
@@ -763,299 +833,82 @@
             {<Category: 1>, <Category: 2>, <Category: 3>, <Category: 4>, <Category: 5>}
             >>> ds.get_category_names()
             ['person', 'bicycle', 'car', 'motorcycle', 'airplane']
 
         Returns:
             Dataset: Dataset Class.
         """
-        ds = Dataset.new(name, task, root_dir)
-        ds.initialize()
-
-        if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
-            if len(coco_file) != len(coco_root_dir):
-                raise ValueError("coco_file and coco_root_dir should have same length.")
-        if not isinstance(coco_file, list) and isinstance(coco_root_dir, list):
-            raise ValueError(
-                "ambiguous input. The number of coco_file should be same or greater than coco_root_dir."
-            )
-        if not isinstance(coco_file, list):
-            coco_file = [coco_file]
-        if not isinstance(coco_root_dir, list):
-            coco_root_dir = [coco_root_dir] * len(coco_file)
-
-        coco_files = coco_file
-        coco_root_dirs = coco_root_dir
-
-        if len(coco_files) == 1:
-            set_names = [None]
-        elif len(coco_files) == 2:
-            set_names = ["train", "val"]
-        elif len(coco_files) == 3:
-            set_names = ["train", "val", "test"]
-        else:
-            raise ValueError("coco_file should have 1, 2, or 3 files.")
-
-        cocos = []
-        for coco_file in coco_files:
-            coco_dict = io.load_json(coco_file)
-            for ann in coco_dict["annotations"]:
-                if "category_id" not in ann:
-                    ann["category_id"] = -1  # dummy category_id to use COCO
-            coco = COCO()
-            coco.dataset = coco_dict
-            coco.createIndex()
-            cocos.append(coco)
-
-        # categories should be same between coco files
-        categories = cocos[0].loadCats(cocos[0].getCatIds())
-        for coco in cocos[1:]:
-            if categories != coco.loadCats(coco.getCatIds()):
-                raise ValueError("categories should be same between coco files.")
-
-        coco_cat_id_to_waffle_cat_id = {}
-        for i, category in enumerate(categories, start=1):
-            coco_category_id = category.pop("id")
-            coco_cat_id_to_waffle_cat_id[coco_category_id] = i
-            ds.add_categories([Category.from_dict({**category, "category_id": i}, task=ds.task)])
-
-        # import coco dataset
-        total_length = sum([len(coco.getImgIds()) for coco in cocos])
-        logging.info(f"Importing coco dataset. Total length: {total_length}")
-        pgbar = tqdm.tqdm(total=total_length, desc="Importing coco dataset")
-
-        image_id = 1
-        annotation_id = 1
-
-        # parse coco annotation file
-        for coco, coco_root_dir, set_name in tqdm.tqdm(zip(cocos, coco_root_dirs, set_names)):
-
-            image_ids = []
-            for coco_image_id, annotation_dicts in coco.imgToAnns.items():
-                if len(annotation_dicts) == 0:
-                    warnings.warn(f"image_id {coco_image_id} has no annotations.")
-                    continue
-
-                image_dict = coco.loadImgs(coco_image_id)[0]
-                image_dict.pop("id")
-
-                file_name = image_dict.pop("file_name")
-                image_path = Path(coco_root_dir) / file_name
-                if not image_path.exists():
-                    raise FileNotFoundError(f"{image_path} does not exist.")
-
-                if set_name:
-                    file_name = f"{set_name}/{file_name}"
+        ds = Dataset.new(name=name, task=task, root_dir=root_dir)
 
-                ds.add_images(
-                    [Image.from_dict({**image_dict, "image_id": image_id, "file_name": file_name})]
+        try:
+            if isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+                if len(coco_file) != len(coco_root_dir):
+                    raise ValueError("coco_file and coco_root_dir should have same length.")
+            if not isinstance(coco_file, list) and isinstance(coco_root_dir, list):
+                raise ValueError(
+                    "ambiguous input. The number of coco_file should be same or greater than coco_root_dir."
                 )
-                io.copy_file(image_path, ds.raw_image_dir / file_name, create_directory=True)
+            if not isinstance(coco_file, list):
+                coco_file = [coco_file]
+            if not isinstance(coco_root_dir, list):
+                coco_root_dir = [coco_root_dir] * len(coco_file)
+
+            coco_files = coco_file
+            coco_root_dirs = coco_root_dir
+
+            import_autocare_dlt(ds, coco_files, coco_root_dirs)
+
+            if len(coco_files) == 2:
+                logging.info("copying val set to test set")
+                io.copy_file(ds.val_set_file, ds.test_set_file, create_directory=True)
 
-                for annotation_dict in annotation_dicts:
-                    annotation_dict.pop("id")
-                    ds.add_annotations(
-                        [
-                            Annotation.from_dict(
-                                {
-                                    **annotation_dict,
-                                    "image_id": image_id,
-                                    "annotation_id": annotation_id,
-                                    "category_id": coco_cat_id_to_waffle_cat_id[
-                                        annotation_dict["category_id"]
-                                    ],
-                                },
-                                task=ds.task,
-                            )
-                        ]
-                    )
-                    annotation_id += 1
+            # TODO: add unlabeled set
+            io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
-                image_ids.append(image_id)
-                image_id += 1
-                pgbar.update(1)
-
-            if set_name:
-                io.save_json(image_ids, ds.set_dir / f"{set_name}.json", create_directory=True)
-
-        pgbar.close()
-
-        if len(coco_files) == 2:
-            logging.info("copying val set to test set")
-            io.copy_file(ds.val_set_file, ds.test_set_file, create_directory=True)
-
-        # TODO: add unlabeled set
-        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+        except Exception as e:
+            ds.delete()
+            raise e
 
         return ds
 
     @classmethod
     def from_yolo(
         cls,
         name: str,
         task: str,
-        yaml_path: str,
+        yolo_root_dir: str,
+        yaml_path: str = None,
         root_dir: str = None,
     ) -> "Dataset":
         """
         Import Dataset from yolo format.
         This method imports dataset from yolo(ultralytics) yaml file.
 
         Args:
             name (str): Dataset name.
             task (str): Dataset task.
-            yaml_path (str): Yolo yaml file path.
+            yolo_root_dir (str): Yolo dataset root directory.
+            yaml_path (str): Yolo yaml file path. when task is classification, yaml_path is not required.
             root_dir (str, optional): Dataset root directory. Defaults to None.
 
         Example:
             >>> ds = Dataset.from_yolo("yolo", "classification", "path/to/yolo.yaml")
 
         Returns:
             Dataset: Imported dataset.
         """
 
-        ds = Dataset.new(name, task, root_dir)
-        ds.initialize()
-
-        def _import_classification(set_dir: Path, image_ids: list[int]):
-            # categories
-            for category_id, category_name in info["names"].items():
-                ds.add_categories(
-                    [
-                        Category.classification(
-                            category_id=category_id + 1,
-                            name=category_name,
-                        )
-                    ]
-                )
-            name2id = {v: k for k, v in info["names"].items()}
-
-            for image_id, image_path in zip(image_ids, get_image_files(set_dir)):
-                category_name_index = image_path.parts.index(set_dir.stem) + 1
-                category_name = image_path.parts[category_name_index]
-                category_id = name2id[category_name] + 1
-
-                # image
-                img = cv2.imread(str(image_path))
-                height, width, _ = img.shape
-                image = Image.new(
-                    image_id=image_id,
-                    file_name=f"{image_id}{image_path.suffix}",
-                    width=width,
-                    height=height,
-                )
-                ds.add_images([image])
-
-                # annotation
-                annotation = Annotation.classification(
-                    annotation_id=image_id,
-                    image_id=image_id,
-                    category_id=category_id,
-                )
-                ds.add_annotations([annotation])
-
-                # raw
-                dst = ds.raw_image_dir / f"{image_id}{image_path.suffix}"
-                io.copy_file(image_path, dst)
-
-        def _import_object_detection(set_dir: Path, image_ids: list[int]):
-            image_dir = set_dir / "images"
-            label_dir = set_dir / "labels"
-
-            if not image_dir.exists():
-                warnings.warn(f"{image_dir} does not exist.")
-                return
-            if not label_dir.exists():
-                warnings.warn(f"{label_dir} does not exist.")
-                return
-
-            # categories
-            for category_id, category_name in info["names"].items():
-                ds.add_categories(
-                    [
-                        Category.object_detection(
-                            category_id=category_id + 1,
-                            name=category_name,
-                        )
-                    ]
-                )
-
-            for image_id, image_path, label_path in zip(
-                image_ids,
-                get_image_files(image_dir),
-                get_files(label_dir, "txt"),
-            ):
-                # image
-                img = cv2.imread(str(image_path))
-                height, width, _ = img.shape
-                image = Image.new(
-                    image_id=image_id,
-                    file_name=f"{image_id}{image_path.suffix}",
-                    width=width,
-                    height=height,
-                )
-                ds.add_images([image])
-
-                # annotation
-                with open(label_path) as f:  # TODO: use load_txt of waffle_utils after implementing
-                    txt = f.readlines()
-
-                current_annotation_id = len(ds.get_annotations())
-                for i, t in enumerate(txt, start=1):
-                    category_id, x, y, w, h = list(map(float, t.split()))
-                    category_id = int(category_id) + 1
-                    x *= width
-                    y *= height
-                    w *= width
-                    h *= height
-
-                    x -= w / 2
-                    y -= h / 2
-
-                    x, y, w, h = int(x), int(y), int(w), int(h)
-                    annotation = Annotation.object_detection(
-                        annotation_id=current_annotation_id + i,
-                        image_id=image_id,
-                        category_id=category_id,
-                        bbox=[x, y, w, h],
-                        area=w * h,
-                    )
-                    ds.add_annotations([annotation])
-
-                # raw
-                dst = ds.raw_image_dir / f"{image_id}{image_path.suffix}"
-                io.copy_file(image_path, dst)
-
-        if task == TaskType.OBJECT_DETECTION:
-            _import = _import_object_detection
-        elif task == TaskType.CLASSIFICATION:
-            _import = _import_classification
-        else:
-            raise ValueError(f"Unsupported task: {task}")
-
-        info = io.load_yaml(yaml_path)
-        yolo_root_dir = Path(info["path"])
-
-        current_image_id = 1
-        for set_type in ["train", "val", "test"]:
-            if set_type not in info.keys():
-                continue
-
-            # sets
-            set_dir = Path(yolo_root_dir) / set_type
-            image_num = len(get_image_files(set_dir))
-            image_ids = list(range(current_image_id, image_num + current_image_id))
+        ds = Dataset.new(name=name, task=task, root_dir=root_dir)
 
-            io.save_json(image_ids, ds.set_dir / f"{set_type}.json", True)
-            current_image_id += image_num
-
-            # import other field
-            _import(set_dir, image_ids)
+        try:
+            import_yolo(ds, yolo_root_dir, yaml_path)
 
-        # TODO: add unlabeled set
-        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+        except Exception as e:
+            ds.delete()
+            raise e
 
         return ds
 
     @classmethod
     def from_transformers(
         cls,
         name: str,
@@ -1079,112 +932,25 @@
 
         Examples:
             >>> ds = Dataset.from_transformers("transformers", "object_detection", "path/to/transformers/dataset")
 
         Returns:
             Dataset: Dataset Class
         """
-        ds = Dataset.new(name, task, root_dir)
-        ds.initialize()
-
-        dataset = load_from_disk(dataset_dir)
-
-        if isinstance(dataset, DatasetDict):
-            is_splited = True
-        elif isinstance(dataset, HFDataset):
-            is_splited = False
-        else:
-            raise ValueError("dataset should be Dataset or DatasetDict")
-
-        def _import(dataset: HFDataset, task: str, image_ids: list[int]):
-            if task == TaskType.OBJECT_DETECTION:
-                if not ds.get_categories():
-                    categories = dataset.features["objects"].feature["category"].names
-                    for category_id, category_name in enumerate(categories):
-                        category = Category.object_detection(
-                            category_id=category_id + 1,
-                            supercategory="object",
-                            name=category_name,
-                        )
-                        ds.add_categories([category])
-
-                for data in dataset:
-                    data["image"].save(f"{ds.raw_image_dir}/{data['image_id']}.jpg")
-                    image = Image.new(
-                        image_id=data["image_id"],
-                        file_name=f"{data['image_id']}.jpg",
-                        width=data["width"],
-                        height=data["height"],
-                    )
-                    ds.add_images([image])
-
-                    annotation_ids = data["objects"]["id"]
-                    areas = data["objects"]["area"]
-                    category_ids = data["objects"]["category"]
-                    bboxes = data["objects"]["bbox"]
-
-                    for annotation_id, area, category_id, bbox in zip(
-                        annotation_ids, areas, category_ids, bboxes
-                    ):
-                        annotation = Annotation.object_detection(
-                            annotation_id=annotation_id,
-                            image_id=image.image_id,
-                            category_id=category_id + 1,
-                            area=area,
-                            bbox=bbox,
-                        )
-                        ds.add_annotations([annotation])
-
-            elif task == TaskType.CLASSIFICATION:
-                if not ds.get_categories():
-                    categories = dataset.features["label"].names
-                    for category_id, category_name in enumerate(categories):
-                        category = Category.classification(
-                            category_id=category_id + 1,
-                            supercategory="object",
-                            name=category_name,
-                        )
-                        ds.add_categories([category])
-
-                for image_id, data in zip(image_ids, dataset):
-                    image_save_path = f"{ds.raw_image_dir}/{image_id}.jpg"
-                    data["image"].save(image_save_path)
-                    pil_image = PIL.Image.open(image_save_path)
-                    width, height = pil_image.size
-                    image = Image.new(
-                        image_id=image_id,
-                        file_name=f"{image_id}.jpg",
-                        width=width,
-                        height=height,
-                    )
-                    ds.add_images([image])
-
-                    annotation = Annotation.classification(
-                        annotation_id=image_id,
-                        image_id=image.image_id,
-                        category_id=data["label"] + 1,
-                    )
-                    ds.add_annotations([annotation])
+        ds = Dataset.new(name=name, task=task, root_dir=root_dir)
 
-            else:
-                raise ValueError("task should be one of ['classification', 'object_detection']")
+        try:
+            import_transformers(ds, dataset_dir)
 
-        if is_splited:
-            start_num = 1
-            for set_type, set in dataset.items():
-                image_ids = list(range(start_num, set.num_rows + start_num))
-                start_num += set.num_rows
-                io.save_json(image_ids, ds.set_dir / f"{set_type}.json", True)
-                _import(set, task, image_ids)
-        else:
-            image_ids = list(range(1, dataset.num_rows + 1))
-            _import(dataset, task, image_ids)
+            # TODO: add unlabeled set
+            io.save_json([], ds.unlabeled_set_file, create_directory=True)
 
-        # TODO: add unlabeled set
-        io.save_json([], ds.unlabeled_set_file, create_directory=True)
+        except Exception as e:
+            ds.delete()
+            raise e
 
         return ds
 
     @classmethod
     def sample(cls, name: str, task: str, root_dir: str = None) -> "Dataset":
         """
         Import sample Dataset.
@@ -1252,35 +1018,42 @@
                     dataset_name_list.append(dataset_dir.name)
         return dataset_name_list
 
     def initialize(self):
         """Initialize Dataset.
         It creates necessary directories under {dataset_root_dir}/{dataset_name}.
         """
+
+        if self.initialized():
+            raise FileExistsError(f"{self.name} is already initialized.")
+
         io.make_directory(self.raw_image_dir)
         io.make_directory(self.image_dir)
         io.make_directory(self.annotation_dir)
         io.make_directory(self.category_dir)
 
-        # create dataset_info.yaml
-        io.save_yaml(
-            DatasetInfo(name=self.name, task=self.task, created=self.created).to_dict(),
-            self.dataset_info_file,
-        )
-
     def initialized(self) -> bool:
         """Check if Dataset has been initialized or not.
 
         Returns:
             bool:
                 initialized -> True
                 not initialized -> False
         """
         return self.dataset_info_file.exists()
 
+    def save_dataset_info(self):
+        """Save DatasetInfo."""
+        DatasetInfo(
+            name=self.name,
+            task=self.task,
+            categories=list(map(lambda x: x.to_dict(), self.categories)),
+            created=self.created,
+        ).save_yaml(self.dataset_info_file)
+
     def trainable(self) -> bool:
         """Check if Dataset is trainable or not.
 
         Returns:
             bool:
                 trainable -> True
                 not trainable -> False
@@ -1313,15 +1086,19 @@
 
     def get_dataset_info(self) -> DatasetInfo:
         """Get DatasetInfo.
 
         Returns:
             DatasetInfo: DatasetInfo
         """
-        return DatasetInfo.load(self.dataset_info_file)
+        dataset_info = DatasetInfo.load(self.dataset_info_file)
+        if not hasattr(dataset_info, "categories"):
+            dataset_info.categories = self.get_categories()
+            self.save_dataset_info()
+        return dataset_info
 
     # get
     def get_images(self, image_ids: list[int] = None, labeled: bool = True) -> list[Image]:
         """Get "Image"s.
 
         Args:
             image_ids (list[int], optional): id list. None for all "Image"s. Defaults to None.
@@ -1432,14 +1209,16 @@
             raise ValueError("Category names should be unique")
 
         for item in categories:
             item_id = item.category_id
             item_path = self.category_dir / f"{item_id}.json"
             io.save_json(item.to_dict(), item_path)
 
+        self.save_dataset_info()
+
     def add_annotations(self, annotations: list[Annotation]):
         """Add "Annotation"s to dataset.
 
         Args:
             annotations (list[Annotation]): list of "Annotation"s
         """
         categories = self.get_category_names()
@@ -1522,15 +1301,14 @@
                 # flatten images to one list [cat]
                 train_num = max(int(image_num * train_ratio), 1)
                 val_num = max(int(image_num * val_ratio), 1)
 
                 if test_ratio == 0.0:
                     train_ids.extend(image_ids[:train_num])
                     val_ids.extend(image_ids[train_num:])
-                    test_ids = val_ids
                 else:
                     train_ids.extend(image_ids[:train_num])
                     val_ids.extend(image_ids[train_num : train_num + val_num])
                     test_ids.extend(image_ids[train_num + val_num :])
 
         else:
             raise ValueError(f"Unknown split method: {method}")
@@ -1570,18 +1348,22 @@
 
         Returns:
             list[list[int]]: split ids
         """
         if not self.train_set_file.exists():
             raise FileNotFoundError("There is no set files. Please run ds.split() first")
 
-        train_ids: list[int] = io.load_json(self.train_set_file)
-        val_ids: list[int] = io.load_json(self.val_set_file)
-        test_ids: list[int] = io.load_json(self.test_set_file)
-        unlabeled_ids: list[int] = io.load_json(self.unlabeled_set_file)
+        train_ids: list[int] = (
+            io.load_json(self.train_set_file) if self.train_set_file.exists() else []
+        )
+        val_ids: list[int] = io.load_json(self.val_set_file) if self.val_set_file.exists() else []
+        test_ids: list[int] = io.load_json(self.test_set_file) if self.test_set_file.exists() else []
+        unlabeled_ids: list[int] = (
+            io.load_json(self.unlabeled_set_file) if self.unlabeled_set_file.exists() else []
+        )
 
         return [train_ids, val_ids, test_ids, unlabeled_ids]
 
     def export(self, data_type: Union[str, DataType]) -> str:
         """
         Export Dataset to Specific data formats
 
@@ -1632,7 +1414,28 @@
                 io.remove_directory(export_dir)
             raise e
 
     def delete(self):
         """Delete Dataset"""
         io.remove_directory(self.dataset_dir)
         del self
+
+    def draw_annotations(self, image_ids=None):
+        """
+        Draw annotations on images
+        Save drawn images to draw_dir
+
+        Args:
+            image_ids (list[int], optional): image ids to draw. Defaults to None.
+
+        """
+        if not self.draw_dir.exists():
+            self.draw_dir.mkdir(parents=True)
+
+        images = self.get_images(image_ids)
+        names = self.get_category_names()
+
+        for image in tqdm.tqdm(images):
+            np_image = load_image(self.raw_image_dir / image.file_name)
+            annotations = self.get_annotations(image.image_id)
+            drawn_image = draw_results(np_image, annotations, names)
+            save_image(self.draw_dir / image.file_name, drawn_image)
```

### Comparing `waffle_hub-0.2.5/waffle_hub/experimental/auto_label/grounding_dino.py` & `waffle_hub-0.2.6/waffle_hub/experimental/auto_label/grounding_dino.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 import argparse
 from pathlib import Path
 
 import cv2
 import torch
 import torchvision.transforms as T
-
 import tqdm
-
 from groundingdino.models import build_model
 from groundingdino.util.slconfig import SLConfig
 from groundingdino.util.utils import clean_state_dict, get_phrases_from_posmap
-
-from waffle_utils.dataset import Dataset
 from waffle_utils.file import io
 from waffle_utils.log import initialize_logger
 
+from waffle_hub.dataset import Dataset
+
 initialize_logger("logs/auto_label.log")
 
-from waffle_hub.utils.data import ImageDataset
-from waffle_hub.utils.draw import draw_results
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation
+from waffle_hub.utils.data import ImageDataset
+from waffle_hub.utils.draw import draw_results
 
 
-def parse_results(bboxes: torch.Tensor, confs: list[float], labels: list[str], image_info: ImageInfo, class2id: dict):
+def parse_results(
+    bboxes: torch.Tensor,
+    confs: list[float],
+    labels: list[str],
+    image_info: ImageInfo,
+    class2id: dict,
+):
 
     W, H = image_info.input_shape
     left_pad, top_pad = image_info.pad
     ori_w, ori_h = image_info.ori_shape
     new_w, new_h = image_info.new_shape
 
     # cx cy w h (0~1) -> x1 y1 x2 y2 (0~1)
@@ -35,17 +39,15 @@
     x1 = cx - w / 2
     y1 = cy - h / 2
     x2 = cx + w / 2
     y2 = cy + h / 2
     bboxes = torch.stack([x1, y1, x2, y2], dim=-1)
 
     parsed = []
-    for (x1, y1, x2, y2), conf, label in zip(
-        bboxes, confs, labels
-    ):
+    for (x1, y1, x2, y2), conf, label in zip(bboxes, confs, labels):
 
         x1 = max(float((x1 * W - left_pad) / new_w * ori_w), 0)
         y1 = max(float((y1 * H - top_pad) / new_h * ori_h), 0)
         x2 = min(float((x2 * W - left_pad) / new_w * ori_w), ori_w)
         y2 = min(float((y2 * H - top_pad) / new_h * ori_h), ori_h)
 
         parsed.append(
@@ -65,15 +67,18 @@
     model = build_model(args)
     checkpoint = torch.load(model_checkpoint_path, map_location="cpu")
     load_res = model.load_state_dict(clean_state_dict(checkpoint["model"]), strict=False)
     print(load_res)
     _ = model.eval()
     return model
 
-def get_grounding_output(model, image, caption, box_threshold, text_threshold, device, with_logits=True):
+
+def get_grounding_output(
+    model, image, caption, box_threshold, text_threshold, device, with_logits=True
+):
     caption = caption.lower()
     caption = caption.strip()
     if not caption.endswith("."):
         caption = caption + "."
     model = model.to(device)
     image = image.to(device)
     with torch.no_grad():
@@ -105,46 +110,57 @@
 
     return torch.tensor(boxes), confs, labels
 
 
 if __name__ == "__main__":
 
     parser = argparse.ArgumentParser("Grounding DINO example", add_help=True)
-    parser.add_argument("--config_file", "-c", type=str, default="autolabel_tmp/GroundingDINO_SwinT_OGC.py", help="path to config file")
     parser.add_argument(
-        "--checkpoint_path", "-p", type=str, default="autolabel_tmp/groundingdino_swint_ogc.pth", help="path to checkpoint file"
+        "--config_file",
+        "-c",
+        type=str,
+        default="autolabel_tmp/GroundingDINO_SwinT_OGC.py",
+        help="path to config file",
+    )
+    parser.add_argument(
+        "--checkpoint_path",
+        "-p",
+        type=str,
+        default="autolabel_tmp/groundingdino_swint_ogc.pth",
+        help="path to checkpoint file",
     )
-    parser.add_argument("--source", "-s", type=str, required=True, help="path to image file or directory")
-    parser.add_argument("--image_size", "-i", type=int, default=640, help="image size")
-    parser.add_argument("--text_prompt", "-t", type=str, required=True, help="text prompt")
     parser.add_argument(
-        "--output_dir", "-o", type=str, default="outputs", help="output directory"
+        "--source", "-s", type=str, required=True, help="path to image file or directory"
     )
+    parser.add_argument("--image_size", "-i", type=int, default=640, help="image size")
+    parser.add_argument("--text_prompt", "-t", type=str, required=True, help="text prompt")
+    parser.add_argument("--class_name", type=str, required=True, help="class name")
+    parser.add_argument("--output_dir", "-o", type=str, default="outputs", help="output directory")
 
     parser.add_argument("--box_threshold", type=float, default=0.3, help="box threshold")
     parser.add_argument("--text_threshold", type=float, default=0.25, help="text threshold")
 
     parser.add_argument("--draw", action="store_true", help="draw bounding boxes")
+    parser.add_argument("--recursive", action="store_true", help="load image recursively")
 
     parser.add_argument("--waffle_dataset_name", default=None, type=str, help="waffle dataset name")
 
-    parser.add_argument(
-        "--device", default="0", type=str, help="cuda device id or cpu"
-    )
+    parser.add_argument("--device", default="0", type=str, help="cuda device id or cpu")
     args = parser.parse_args()
 
     # cfg
     config_file = args.config_file  # change the path of the model config file
     checkpoint_path = args.checkpoint_path  # change the path of the model
 
     # text_prompt = args.text_prompt
     text_prompt = args.text_prompt
-    classes = [text_prompt]
-    class2id = {name: i for i, name in enumerate(classes)}
-    id2class = {i: name for i, name in enumerate(classes)}
+    class_name = args.class_name
+    class2id = {name: i for i, name in enumerate([class_name])}
+    id2class = {i: name for name, i in class2id.items()}
+    
     box_threshold = args.box_threshold
     text_threshold = args.text_threshold
 
     # device
     device = "cpu" if args.device == "cpu" else f"cuda:{args.device}"
 
     # directory
@@ -152,40 +168,44 @@
     output_dir = Path(args.output_dir)
     draw_dir = output_dir / "draw"
 
     # load model
     model = load_model(config_file, checkpoint_path, device)
 
     # get dataloader
-    dl = ImageDataset(image_dir=source_dir, image_size=args.image_size, letter_box=True).get_dataloader(1, 1)
+    dl = ImageDataset(
+        image_dir=source_dir, image_size=args.image_size, letter_box=True, recursive=args.recursive
+    ).get_dataloader(1, 1)
     preprocess = T.Normalize([0.485, 0.456, 0.406], [0.229, 0.224, 0.225])
 
     # coco format
     coco = {
-        "categories": [{"id": i+1, "name": c, "supercategory": "object"} for i, c in id2class.items()],
+        "categories": [
+            {"id": i + 1, "name": c, "supercategory": "object"} for i, c in id2class.items()
+        ],
         "images": [],
         "annotations": [],
     }
     image_id = 1
     annotation_id = 1
 
     for images, image_infos in tqdm.tqdm(dl, total=len(dl)):
 
         images = preprocess(images)
-        
+
         # run model
         boxes, confs, labels = get_grounding_output(
             model, images, text_prompt, box_threshold, text_threshold, device
         )
         image_info = image_infos[0]  # TODO: batch
         if len(boxes) > 0:
-            results = parse_results(boxes, confs, labels, image_info, class2id)
+            results = parse_results(boxes, confs, [class_name] * len(labels), image_info, class2id)
         else:
             results = []
-        
+
         # save result as coco format
         file_name = Path(image_info.image_path).relative_to(source_dir)
         coco["images"].append(
             {
                 "id": image_id,
                 "file_name": str(file_name),
                 "width": image_info.ori_shape[0],
@@ -193,27 +213,27 @@
             }
         )
         for result in results:
             coco["annotations"].append(
                 {
                     "id": annotation_id,
                     "image_id": image_id,
-                    "category_id": result.category_id+1,
+                    "category_id": result.category_id + 1,
                     "bbox": result.bbox,
                     "score": result.score,
                 }
             )
             annotation_id += 1
         image_id += 1
 
         if args.draw:
             draw = draw_results(
                 image_info.image_path,
                 results,
-                names=classes,
+                names=[class_name],
             )
             draw_path = draw_dir / file_name.with_suffix(".png")
             io.make_directory(draw_path.parent)
             cv2.imwrite(str(draw_path), draw)
 
     # save coco format
     io.save_json(coco, output_dir / "coco.json", create_directory=True)
```

### Comparing `waffle_hub-0.2.5/waffle_hub/experimental/serve.py` & `waffle_hub-0.2.6/waffle_hub/experimental/serve.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/autocare_dlt_hub.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 class AutocareDLTHub(Hub):
     BACKEND_NAME = "autocare_dlt"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = False
     DEFAULT_PARAMS = DEFAULT_PARAMS
+    DEFAULT_ADVANCE_PARAMS = {}
 
     DATA_TYPE_MAP = DATA_TYPE_MAP
     WEIGHT_PATH = WEIGHT_PATH
 
     def __init__(
         self,
         name: str,
@@ -104,32 +105,14 @@
             task=task,
             model_type=model_type,
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
-    @property
-    def categories(self) -> list[dict]:
-        return self.__categories
-
-    @categories.setter
-    @type_validator(list)
-    def categories(self, v):
-        if isinstance(v[0], str):
-            v = [{"supercategory": "object", "name": n} for n in v]
-        elif isinstance(v[0], dict) and "supercategory" not in v[0]:
-            # TODO: Temporal solution for DLT classification: Not supported multi-task yet.
-            v_ = []
-            for k, cls in v[0].items():
-                for c in cls:
-                    v_.append({"supercategory": k, "name": c})
-            v = v_
-        self.__categories = v
-
     # Hub Utils
     def get_preprocess(self, *args, **kwargs):
 
         if self.task == TaskType.OBJECT_DETECTION:
             normalize = T.Normalize([0, 0, 0], [1, 1, 1], inplace=True)
 
             def preprocess(x, *args, **kwargs):
@@ -208,36 +191,49 @@
 
         return metrics
 
     # Train Hook
     def on_train_start(self, cfg: TrainConfig):
         # set data
         cfg.dataset_path: Path = Path(cfg.dataset_path)
+        train_coco_file = cfg.dataset_path / "train.json"
+        val_coco_file = cfg.dataset_path / "val.json"
+        test_coco_file = cfg.dataset_path / "test.json"
         data_config = get_data_config(
             self.DATA_TYPE_MAP[self.task],
             cfg.image_size if isinstance(cfg.image_size, list) else [cfg.image_size, cfg.image_size],
             cfg.batch_size,
             cfg.workers,
-            str(cfg.dataset_path / "train.json"),
+            str(train_coco_file),
             str(cfg.dataset_path / "images"),
-            str(cfg.dataset_path / "val.json"),
+            str(val_coco_file),
             str(cfg.dataset_path / "images"),
-            str(cfg.dataset_path / "test.json"),
+            str(test_coco_file) if test_coco_file.exists() else str(val_coco_file),
             str(cfg.dataset_path / "images"),
         )
         if self.model_type == "LicencePlateRecognition":
             data_config["data"]["mode"] = "lpr"
 
         cfg.data_config = self.artifact_dir / "data.json"
         io.save_json(data_config, cfg.data_config, create_directory=True)
-        categories = (
-            self.categories
-            if self._Hub__task == TaskType.CLASSIFICATION
-            else [x["name"] for x in self.categories]
-        )
+
+        if self.task == TaskType.CLASSIFICATION:
+            super_cat = [[c.supercategory, c.name] for c in self.categories]
+            super_cat_dict = {}
+            for super_cat, cat in super_cat:
+                if super_cat not in super_cat_dict:
+                    super_cat_dict[super_cat] = []
+                super_cat_dict[super_cat].append(cat)
+
+            categories = []
+            for super_cat, cat in super_cat_dict.items():
+                categories.append({super_cat: cat})
+
+        else:
+            categories = self.get_category_names()
 
         model_config = get_model_config(
             self.model_type,
             self.model_size,
             categories,
             cfg.seed,
             cfg.learning_rate,
```

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/config.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/data_cfg.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/autocare_dlt/configs/model_cfg.py`

 * *Files 6% similar despite different names*

```diff
@@ -92,16 +92,16 @@
                 "momentum": 0.9,
                 "weight_decay": 0.0001,
             },
             "lr_cfg": {"type": "cosine"},
             "use_model_ema": True,
             "max_epoch": epochs,
             "seed": seed,
-            "classes": get_multi_task_categories(categories),
-            "num_classes": len(categories),
+            "classes": categories,
+            "num_classes": sum([len(list(category.values())[0]) for category in categories]),
         }
 
     elif model_type == "TextRecognition":
         if model_size == "s":
             backbone = "resnet18"
         elif model_size == "m":
             backbone = "resnet34"
@@ -150,22 +150,7 @@
             "max_epoch": epochs,
             "seed": seed,
             "classes": categories,
             "num_classes": len(categories),
         }
     else:
         raise NotImplementedError(f"Model type {model_type} not implemented.")
-
-
-def get_multi_task_categories(categories: list[dict]):
-    multi_task_categories = []
-    cat_dict = {}
-    for category in categories:
-        sup = category["supercategory"]
-        name = category["name"]
-        if sup not in cat_dict:
-            cat_dict[sup] = [name]
-        else:
-            cat_dict[sup].append(name)
-    for k, v in cat_dict.items():
-        multi_task_categories.append({k: v})
-    return multi_task_categories
```

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/config.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/config.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/train_input_helper.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/train_input_helper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/transformers/transformers_hub.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/transformers/transformers_hub.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """
 Transformers Hub
 See Hub documentation for more details about usage.
 """
 
 import os
 import warnings
-from copy import deepcopy
+from collections import defaultdict
 from functools import cached_property
 from pathlib import Path
 from typing import Callable, Union
 
 import torch
 import transformers
 from torchvision import transforms as T
 from transformers import (
     AutoImageProcessor,
     AutoModelForImageClassification,
     AutoModelForObjectDetection,
     Trainer,
     TrainerCallback,
 )
+from transformers.trainer_callback import TrainerControl, TrainerState
+from transformers.training_args import TrainingArguments
 from transformers.utils import ModelOutput
 from waffle_utils.file import io
 
 from datasets import load_from_disk
 from waffle_hub import TaskType
 from waffle_hub.hub import Hub
 from waffle_hub.hub.adapter.transformers.train_input_helper import (
@@ -39,33 +41,37 @@
 
 
 class CustomCallback(TrainerCallback):
     """
     This class is necessary to obtain logs for the training.
     """
 
-    def __init__(self, trainer) -> None:
+    def __init__(self, trainer, metric_file: Union[Path, str]) -> None:
         super().__init__()
         self._trainer = trainer
+        self.metric_file = metric_file
 
-    def on_epoch_end(self, args, state, control, **kwargs):
-        if control.should_evaluate:
-            control_copy = deepcopy(control)
-            self._trainer.evaluate(
-                eval_dataset=self._trainer.train_dataset,
-                metric_key_prefix="train",
-            )
-            return control_copy
+    def on_train_end(
+        self, args: TrainingArguments, state: TrainerState, control: TrainerControl, **kwargs
+    ):
+        epoch_metric = defaultdict(list)
+        for metric in state.log_history:
+            epoch = int(metric.get("epoch"))
+            for key, value in metric.items():
+                epoch_metric[epoch].append({"tag": key, "value": value})
+        io.save_json(list(epoch_metric.values()), self.metric_file)
+        return control
 
 
 class TransformersHub(Hub):
     BACKEND_NAME = "transformers"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = False
     DEFAULT_PARAMS = DEFAULT_PARAMS
+    DEFAULT_ADVANCE_PARAMS = {}
 
     # Override
     LAST_CKPT_FILE = "weights/last_ckpt"
     BEST_CKPT_FILE = "weights/best_ckpt"
 
     def __init__(
         self,
@@ -205,38 +211,24 @@
             args=cfg.train_input.training_args,
             data_collator=cfg.train_input.collator,
             train_dataset=cfg.train_input.dataset["train"],
             eval_dataset=cfg.train_input.dataset["val"],
             tokenizer=cfg.train_input.image_processor,
             compute_metrics=cfg.train_input.compute_metrics,
         )
-        trainer.add_callback(CustomCallback(trainer))
+        trainer.add_callback(CustomCallback(trainer, self.metric_file))
         trainer.train()
         trainer.save_model(str(self.artifact_dir / "weights" / "last_ckpt"))
         trainer._load_best_model()
         trainer.save_model(str(self.artifact_dir / "weights" / "best_ckpt"))
 
         self.train_log = trainer.state.log_history
 
     def get_metrics(self) -> list[list[dict]]:
-        metrics = []
-
-        for epoch in range(0, len(self.train_log) - 1, 3):  # last is runtime info
-
-            current_epoch_log = self.train_log[epoch]
-
-            current_epoch_log.update(self.train_log[epoch + 1])
-            current_epoch_log.update(self.train_log[epoch + 2])
-
-            epoch_metrics = []
-            for key, value in current_epoch_log.items():
-                epoch_metrics.append({"tag": key, "value": value})
-            metrics.append(epoch_metrics)
-
-        return metrics
+        return io.load_json(self.metric_file) if self.metric_file.exists() else []
 
     def on_train_end(self, cfg: TrainConfig):
         io.copy_files_to_directory(
             self.artifact_dir / "weights" / "best_ckpt",
             self.best_ckpt_file,
             create_directory=True,
         )
```

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py` & `waffle_hub-0.2.6/waffle_hub/hub/adapter/ultralytics/ultralytics_hub.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,34 +7,35 @@
 from pathlib import Path
 from typing import Union
 
 import torch
 import ultralytics
 from torchvision import transforms as T
 from ultralytics import YOLO
+from ultralytics.yolo.utils import DEFAULT_CFG as YOLO_DEFAULT_ADVANCE_PARAMS
 from waffle_utils.file import io
 
 from waffle_hub import TaskType
 from waffle_hub.hub import Hub
 from waffle_hub.hub.model.wrapper import ModelWrapper
 from waffle_hub.schema.configs import TrainConfig
 from waffle_hub.utils.callback import TrainCallback
 from waffle_hub.utils.process import run_python_file
 
-from .config import DEFAULT_PARAMS, MODEL_TYPES, TASK_MAP, TASK_SUFFIX
+from .config import DEFAULT_PARAMS, MODEL_TYPES, TASK_MAP
 
 
 class UltralyticsHub(Hub):
     BACKEND_NAME = "ultralytics"
     MODEL_TYPES = MODEL_TYPES
     MULTI_GPU_TRAIN = True
     DEFAULT_PARAMS = DEFAULT_PARAMS
+    DEFAULT_ADVANCE_PARAMS = dict(YOLO_DEFAULT_ADVANCE_PARAMS)
 
     TASK_MAP = TASK_MAP
-    TASK_SUFFIX = TASK_SUFFIX
 
     def __init__(
         self,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
@@ -65,14 +66,19 @@
             model_size=model_size,
             categories=categories,
             root_dir=root_dir,
         )
 
         self.backend_task_name = self.TASK_MAP[self.task]
 
+    def get_default_advance_train_params(
+        cls, task: str = None, model_type: str = None, model_size: str = None
+    ) -> dict:
+        return cls.DEFAULT_ADVANCE_PARAMS
+
     @classmethod
     def new(
         cls,
         name: str,
         task: str = None,
         model_type: str = None,
         model_size: str = None,
@@ -260,37 +266,46 @@
             cfg.dataset_path = cfg.dataset_path.absolute()
         cfg.dataset_path = str(cfg.dataset_path)
 
         # pretrained model
         cfg.pretrained_model = (
             cfg.pretrained_model
             if cfg.pretrained_model
-            else self.model_type + self.model_size + self.TASK_SUFFIX[self.backend_task_name] + ".pt"
+            else self.MODEL_TYPES[self.task][self.model_type][self.model_size]
         )
 
+        # other
+        cfg.letter_box = False if "," in cfg.device else cfg.letter_box
+
     def training(self, cfg: TrainConfig, callback: TrainCallback):
 
         code = f"""if __name__ == "__main__":
         from ultralytics import YOLO
-        model = YOLO("{cfg.pretrained_model}", task="{self.backend_task_name}")
-        model.train(
-            data="{cfg.dataset_path}",
-            epochs={cfg.epochs},
-            batch={cfg.batch_size},
-            imgsz={cfg.image_size},
-            lr0={cfg.learning_rate},
-            lrf={cfg.learning_rate},
-            rect={cfg.letter_box},
-            device="{cfg.device}",
-            workers={cfg.workers},
-            seed={cfg.seed},
-            verbose={cfg.verbose},
-            project="{self.hub_dir}",
-            name="{self.ARTIFACT_DIR}",
-        )"""
+        try:
+            model = YOLO("{cfg.pretrained_model}", task="{self.backend_task_name}")
+            model.train(
+                data="{cfg.dataset_path}",
+                epochs={cfg.epochs},
+                batch={cfg.batch_size},
+                imgsz={cfg.image_size},
+                lr0={cfg.learning_rate},
+                lrf={cfg.learning_rate},
+                rect={cfg.letter_box},
+                device="{cfg.device}",
+                workers={cfg.workers},
+                seed={cfg.seed},
+                verbose={cfg.verbose},
+                project="{self.hub_dir}",
+                name="{self.ARTIFACT_DIR}",
+                **{cfg.advance_params}
+            )
+        except Exception as e:
+            print(e)
+            raise e
+        """
 
         script_file = str((self.hub_dir / "train.py").absolute())
         with open(script_file, "w") as f:
             f.write(code)
 
         run_python_file(script_file)
```

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/cli.py` & `waffle_hub-0.2.6/waffle_hub/hub/cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/hub.py` & `waffle_hub-0.2.6/waffle_hub/hub/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import importlib
 import logging
 import os
 import threading
 import time
 import warnings
 from functools import cached_property
-from pathlib import Path
+from pathlib import Path, PurePath
 from typing import Union
 
 import cpuinfo
 import cv2
 import numpy as np
 import torch
 import tqdm
@@ -32,14 +32,15 @@
     EvaluateConfig,
     ExportConfig,
     InferenceConfig,
     ModelConfig,
     TrainConfig,
 )
 from waffle_hub.schema.data import ImageInfo
+from waffle_hub.schema.fields import Category
 from waffle_hub.schema.result import (
     EvaluateResult,
     ExportResult,
     InferenceResult,
     TrainResult,
 )
 from waffle_hub.utils.callback import (
@@ -47,14 +48,15 @@
     ExportCallback,
     InferenceCallback,
     TrainCallback,
 )
 from waffle_hub.utils.data import ImageDataset, LabeledDataset, get_image_transform
 from waffle_hub.utils.draw import draw_results
 from waffle_hub.utils.evaluate import evaluate_function
+from waffle_hub.utils.metric_logger import MetricLogger
 
 logger = logging.getLogger(__name__)
 
 
 class Hub:
     # Hub Spec. must have
     BACKEND_NAME = None
@@ -68,14 +70,16 @@
     ARTIFACT_DIR = Path("artifacts")
 
     INFERENCE_DIR = Path("inferences")
     EXPORT_DIR = Path("exports")
 
     DRAW_DIR = Path("draws")
 
+    TRAIN_LOG_DIR = Path("logs")
+
     # config files
     CONFIG_DIR = Path("configs")
     MODEL_CONFIG_FILE = CONFIG_DIR / "model.yaml"
     TRAIN_CONFIG_FILE = CONFIG_DIR / "train.yaml"
 
     # train results
     LAST_CKPT_FILE = "weights/last_ckpt.pt"
@@ -95,15 +99,15 @@
         self,
         name: str,
         backend: str = None,
         version: str = None,
         task: Union[str, TaskType] = None,
         model_type: str = None,
         model_size: str = None,
-        categories: Union[list[dict], list] = None,
+        categories: list[Union[str, int, float, dict, Category]] = None,
         root_dir: str = None,
     ):
         if self.BACKEND_NAME is None:
             raise AttributeError("BACKEND_NAME must be specified.")
 
         if self.MODEL_TYPES is None:
             raise AttributeError("MODEL_TYPES must be specified.")
@@ -114,39 +118,21 @@
         if self.DEFAULT_PARAMS is None:
             raise AttributeError("DEFAULT_PARAMS must be specified.")
 
         self.name: str = name
         self.task: str = task
         self.model_type: str = model_type
         self.model_size: str = model_size
-        self.categories: list[dict] = categories
+        self.categories: list[Category] = categories
         self.root_dir: Path = root_dir
 
         self.backend: str = backend
         self.version: str = version
 
-        # check task supports
-        if self.task not in self.MODEL_TYPES:
-            io.remove_directory()
-            raise ValueError(f"{self.task} is not supported with {self.backend}")
-
-        try:
-            # save model config
-            model_config = ModelConfig(
-                name=self.name,
-                backend=self.backend,
-                version=self.version,
-                task=self.task,
-                model_type=self.model_type,
-                model_size=self.model_size,
-                categories=self.categories,
-            )
-            model_config.save_yaml(self.model_config_file)
-        except Exception as e:
-            raise e
+        self.save_model_config()
 
     def __repr__(self):
         return self.get_model_config().__repr__()
 
     @classmethod
     def get_hub_class(cls, backend: str = None) -> "Hub":
         """
@@ -238,15 +224,16 @@
         """
         backend = backend if backend else cls.BACKEND_NAME
         hub = cls.get_hub_class(backend)
         if task not in hub.MODEL_TYPES:
             raise ValueError(f"{task} is not supported with {backend}")
         if model_type not in hub.MODEL_TYPES[task]:
             raise ValueError(f"{model_type} is not supported with {backend}")
-        return hub.MODEL_TYPES[task][model_type]
+        model_sizes = hub.MODEL_TYPES[task][model_type]
+        return model_sizes if isinstance(model_sizes, list) else list(model_sizes.keys())
 
     @classmethod
     def get_default_train_params(
         cls, backend: str = None, task: str = None, model_type: str = None, model_size: str = None
     ) -> dict:
         """
         Get default train params
@@ -296,32 +283,43 @@
             model_size (str, optional): Model Size. See Hub.MODEL_SIZES. Defaults to None.
             categories (Union[list[dict], list]): class dictionary or list. [{"supercategory": "name"}, ] or ["name",].
             root_dir (str, optional): Root directory of hub repository. Defaults to None.
 
         Returns:
             Hub: Hub instance
         """
+        root_dir = Hub.parse_root_dir(root_dir)
+
         if name in cls.get_hub_list(root_dir):
-            raise ValueError(f"{name} already exists. Try another name.")
+            raise FileExistsError(f"{name} already exists. Try another name.")
 
-        backend = backend if backend else cls.get_available_backends()[0]
-        task = str(task).upper() if task else cls.get_available_tasks(backend)[0]
-        model_type = model_type if model_type else cls.get_available_model_types(backend, task)[0]
-        model_size = (
-            model_size if model_size else cls.get_available_model_sizes(backend, task, model_type)[0]
-        )
+        try:
+            backend = backend if backend else cls.get_available_backends()[0]
+            task = str(task).upper() if task else cls.get_available_tasks(backend)[0]
+            model_type = (
+                model_type if model_type else cls.get_available_model_types(backend, task)[0]
+            )
+            model_size = (
+                model_size
+                if model_size
+                else cls.get_available_model_sizes(backend, task, model_type)[0]
+            )
 
-        return cls.get_hub_class(backend)(
-            name=name,
-            task=task,
-            model_type=model_type,
-            model_size=model_size,
-            categories=categories,
-            root_dir=root_dir,
-        )
+            return cls.get_hub_class(backend)(
+                name=name,
+                task=task,
+                model_type=model_type,
+                model_size=model_size,
+                categories=categories,
+                root_dir=root_dir,
+            )
+        except Exception as e:
+            if (root_dir / name).exists():
+                io.remove_directory(root_dir / name)
+            raise e
 
     @classmethod
     def load(cls, name: str, root_dir: str = None) -> "Hub":
         """Load Hub by name.
 
         Args:
             name (str): hub name.
@@ -353,25 +351,31 @@
             name (str): hub name.
             model_config_file (str): model config yaml file.
             root_dir (str, optional): hub root directory. Defaults to None.
 
         Returns:
             Hub: New Hub instance
         """
-        if name in cls.get_hub_list(root_dir):
-            raise ValueError(f"{name} already exists. Try another name.")
+        root_dir = Hub.parse_root_dir(root_dir)
+        try:
+            if name in cls.get_hub_list(root_dir):
+                raise ValueError(f"{name} already exists. Try another name.")
 
-        model_config = io.load_yaml(model_config_file)
-        return cls.new(
-            **{
-                **model_config,
-                "name": name,
-                "root_dir": root_dir,
-            }
-        )
+            model_config = io.load_yaml(model_config_file)
+            return cls.new(
+                **{
+                    **model_config,
+                    "name": name,
+                    "root_dir": root_dir,
+                }
+            )
+        except Exception as e:
+            if (root_dir / name).exists():
+                io.remove_directory(root_dir / name)
+            raise e
 
     @classmethod
     def get_hub_list(cls, root_dir: str = None) -> list[str]:
         """
         Get hub name list in root_dir.
 
         Args:
@@ -481,24 +485,52 @@
 
     @version.setter
     @type_validator(str)
     def version(self, v):
         self.__version = v
 
     @property
-    def categories(self) -> list[dict]:
+    def categories(self) -> list[Category]:
         return self.__categories
 
     @categories.setter
     @type_validator(list)
     def categories(self, v):
-        if v is None:
-            raise ValueError("Categories must be specified.")
-        if not isinstance(v[0], dict):
-            v = [{"supercategory": "object", "name": str(n)} for n in v]
+        if v is None or len(v) == 0:
+            warnings.warn(
+                "Categories is not specified.\n"
+                + "It follows the categories of Dataset when the training starts."
+            )
+            v = []
+        elif isinstance(v[0], dict):
+            v = [
+                getattr(Category, self.task.lower())(
+                    **{
+                        **category,
+                        "category_id": category.get("category_id", i),
+                    }
+                )
+                for i, category in enumerate(v, start=1)
+            ]
+        elif isinstance(v[0], (str, int, float)):
+            v = [
+                getattr(Category, self.task.lower())(
+                    category_id=i,
+                    supercategory="object",
+                    name=str(category),
+                )
+                for i, category in enumerate(v, start=1)
+            ]
+            warnings.warn(
+                "Super category is not specified. It may cause unexpected errors in some backends.\n"
+                + "To avoid this warning, please specify category as a list of dictionary or Category"
+            )
+        elif isinstance(v[0], Category):
+            pass
+
         self.__categories = v
 
     @cached_property
     def hub_dir(self) -> Path:
         """Hub(Model) Directory"""
         return self.root_dir / self.name
 
@@ -524,14 +556,19 @@
 
     @cached_property
     def draw_dir(self) -> Path:
         """Draw Results Directory"""
         return self.inference_dir / Hub.DRAW_DIR
 
     @cached_property
+    def train_log_dir(self) -> Path:
+        """Train Logs Directory"""
+        return self.hub_dir / Hub.TRAIN_LOG_DIR
+
+    @cached_property
     def train_config_file(self) -> Path:
         """Train Config yaml File"""
         return self.hub_dir / Hub.TRAIN_CONFIG_FILE
 
     @cached_property
     def best_ckpt_file(self) -> Path:
         """Best Checkpoint File"""
@@ -597,14 +634,51 @@
         """Get model config from model config file.
 
         Returns:
             ModelConfig: model config
         """
         return ModelConfig.load(self.model_config_file)
 
+    def save_model_config(self):
+        """Save ModelConfig."""
+        ModelConfig(
+            name=self.name,
+            backend=self.backend,
+            version=self.version,
+            task=self.task,
+            model_type=self.model_type,
+            model_size=self.model_size,
+            categories=list(map(lambda x: x.to_dict(), self.categories)),
+        ).save_yaml(self.model_config_file)
+
+    def get_default_advance_train_params(
+        self, task: str = None, model_type: str = None, model_size: str = None
+    ) -> dict:
+        """
+        Get default train advance params
+
+        Args:
+            task (str): Task name
+            model_type (str): Model type
+            model_size (str): Model size
+
+        Raises:
+            ModuleNotFoundError: If backend is not supported
+
+        Returns:
+            dict: Default train advance params
+        """
+        raise NotImplementedError(f"{self.backend} does not support advance_params argument.")
+
+    def get_categories(self) -> list[Category]:
+        return self.categories
+
+    def get_category_names(self) -> list[str]:
+        return [category.name for category in self.categories]
+
     # get results
     def get_metrics(self) -> list[list[dict]]:
         """Get metrics per epoch from metric file.
 
         Example:
             >>> hub.get_metrics()
             [
@@ -774,14 +848,15 @@
         image_size: Union[int, list[int]] = None,
         learning_rate: float = None,
         letter_box: bool = None,
         pretrained_model: str = None,
         device: str = "0",
         workers: int = 2,
         seed: int = 0,
+        advance_params: Union[dict, str] = None,
         verbose: bool = True,
         hold: bool = True,
     ) -> TrainResult:
         """Start Train
 
         Args:
             dataset (Union[Dataset, str]): Waffle Dataset object or path or name.
@@ -792,14 +867,15 @@
             learning_rate (float, optional): learning rate. None to use default. Defaults to None.
             letter_box (bool, optional): letter box. None to use default. Defaults to None.
             pretrained_model (str, optional): pretrained model. None to use default. Defaults to None.
             device (str, optional):
                 "cpu" or "gpu_id" or comma seperated "gpu_ids". Defaults to "0".
             workers (int, optional): number of workers. Defaults to 2.
             seed (int, optional): random seed. Defaults to 0.
+            advance_params (Union[dict, str], optional): advance params dictionary or file (yaml, json) path. Defaults to None.
             verbose (bool, optional): verbose. Defaults to True.
             hold (bool, optional): hold process. Defaults to True.
 
         Raises:
             FileExistsError: if trained artifact exists.
             FileNotFoundError: if can not detect appropriate dataset.
             ValueError: if can not detect appropriate dataset.
@@ -826,83 +902,142 @@
 
         Returns:
             TrainResult: train result
         """
 
         def inner(callback: TrainCallback, result: TrainResult):
             try:
+                metric_logger = MetricLogger(
+                    name=self.name,
+                    log_dir=self.train_log_dir,
+                    func=self.get_metrics,
+                    interval=10,
+                    prefix="waffle",
+                )
+                metric_logger.start()
                 self.before_train(cfg)
                 self.on_train_start(cfg)
                 self.save_train_config(cfg)
                 self.training(cfg, callback)
                 self.on_train_end(cfg)
                 self.evaluate(
                     dataset=dataset,
                     batch_size=cfg.batch_size,
                     image_size=cfg.image_size,
                     letter_box=cfg.letter_box,
                     device=cfg.device,
                     workers=cfg.workers,
                 )
                 self.after_train(cfg, result)
+                metric_logger.stop()
+
+                callback.force_finish()
+            except FileExistsError as e:
                 callback.force_finish()
+                callback.set_failed()
+                raise e
             except Exception as e:
                 if self.artifact_dir.exists():
                     io.remove_directory(self.artifact_dir)
                 callback.force_finish()
                 callback.set_failed()
                 raise e
 
+        # parse dataset
         if isinstance(dataset, (str, Path)):
             if Path(dataset).exists():
                 dataset = Path(dataset)
                 dataset = Dataset.load(
                     name=dataset.parts[-1], root_dir=dataset.parents[0].absolute()
                 )
             elif dataset in Dataset.get_dataset_list(dataset_root_dir):
                 dataset = Dataset.load(name=dataset, root_dir=dataset_root_dir)
             else:
                 raise FileNotFoundError(f"Dataset {dataset} is not exist.")
 
+        ## check task match
         if dataset.task.upper() != self.task.upper():
             raise ValueError(
                 f"Dataset task is not matched with hub task. Dataset task: {dataset.task}, Hub task: {self.task}"
             )
 
+        ## check category match
+        if not self.categories:
+            self.categories = dataset.get_categories()
+            self.save_model_config()
+        elif set(dataset.get_category_names()) != set(self.get_category_names()):
+            raise ValueError(
+                "Dataset categories are not matched with hub categories. \n"
+                + f"Dataset categories: {dataset.get_category_names()}, Hub categories: {self.get_category_names()}"
+            )
+
+        ## convert dataset to backend format if not exist
         export_dir = dataset.export_dir / EXPORT_MAP[self.backend.upper()]
         if not export_dir.exists():
+            logger.info(f"[Dataset] Exporting dataset to {self.backend} format...")
             export_dir = dataset.export(self.backend)
-            logger.info(f"Dataset exported to {export_dir}")
+            logger.info("[Dataset] Exporting done.")
 
+        # parse train config
         cfg = TrainConfig(
             dataset_path=export_dir,
             epochs=epochs,
             batch_size=batch_size,
             image_size=image_size,
             learning_rate=learning_rate,
             letter_box=letter_box,
             pretrained_model=pretrained_model,
             device=device,
             workers=workers,
             seed=seed,
+            advance_params=advance_params if advance_params else {},
             verbose=verbose,
         )
 
-        # overwrite train config with default config
+        ## overwrite train config with default config
         for k, v in cfg.to_dict().items():
             if v is None:
                 field_value = getattr(
                     self.DEFAULT_PARAMS[self.task][self.model_type][self.model_size], k
                 )
                 setattr(cfg, k, field_value)
 
+        ## overwrite train advance config
+        if cfg.advance_params:
+            if isinstance(cfg.advance_params, (str, PurePath)):
+                # check if it is yaml or json
+                if Path(cfg.advance_params).exists():
+                    if Path(cfg.advance_params).suffix in [".yaml", ".yml"]:
+                        cfg.advance_params = io.load_yaml(cfg.advance_params)
+                    elif Path(cfg.advance_params).suffix in [".json"]:
+                        cfg.advance_params = io.load_json(cfg.advance_params)
+                    else:
+                        raise ValueError(
+                            f"Advance parameter file should be yaml or json. {cfg.advance_params}"
+                        )
+                else:
+                    raise FileNotFoundError(f"Advance parameter file is not exist.")
+            elif not isinstance(cfg.advance_params, dict):
+                raise ValueError(
+                    f"Advance parameter should be dictionary or file path. {cfg.advance_params}"
+                )
+
+            default_advance_param = self.get_default_advance_train_params()
+            for key in cfg.advance_params.keys():
+                if key not in default_advance_param:
+                    raise ValueError(
+                        f"Advance parameter {key} is not supported.\n"
+                        + f"Supported parameters: {list(default_advance_param.keys())}"
+                    )
+
         callback = TrainCallback(cfg.epochs + 1, self.get_metrics)
         result = TrainResult()
         result.callback = callback
 
+        # TODO: hold arguemnt will be deprecated
         if hold:
             inner(callback, result)
         else:
             thread = threading.Thread(target=inner, args=(callback, result), daemon=True)
             callback.register_thread(thread)
             callback.start()
```

### Comparing `waffle_hub-0.2.5/waffle_hub/hub/model/wrapper.py` & `waffle_hub-0.2.6/waffle_hub/hub/model/wrapper.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/base_schema.py` & `waffle_hub-0.2.6/waffle_hub/schema/base_schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,7 +40,10 @@
     def load(cls, load_path):
         load_path = Path(load_path)
         if load_path.suffix == ".json":
             config = io.load_json(load_path)
         elif load_path.suffix == ".yaml":
             config = io.load_yaml(load_path)
         return cls(**config)
+
+    def __getitem__(self, key):
+        return getattr(self, key)
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/configs.py` & `waffle_hub-0.2.6/waffle_hub/schema/configs.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     image_size: Union[int, list[int]] = None
     learning_rate: float = None
     letter_box: bool = None
     pretrained_model: str = None
     device: str = None
     workers: int = None
     seed: int = None
+    advance_params: dict = None
     verbose: bool = None
 
 
 @dataclass
 class EvaluateConfig(BaseSchema):
     dataset_name: str = None
     set_name: str = None
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/data.py` & `waffle_hub-0.2.6/waffle_hub/schema/data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from dataclasses import dataclass
 
-from waffle_hub.schema.base_schema import BaseSchema
 from waffle_utils.log import datetime_now
 
+from waffle_hub.schema.base_schema import BaseSchema
+from waffle_hub.schema.fields import Category
+
+
 @dataclass
 class DatasetInfo(BaseSchema):
     name: str
     task: str
+    categories: list[Category] = None
     created: str = None
 
     def __post_init__(self):
         self.created = self.created or datetime_now()
 
 
 @dataclass
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/fields/annotation.py` & `waffle_hub-0.2.6/waffle_hub/schema/fields/annotation.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             iscrowd (int, optional): is crowd or not. Default to None.
             score (float, optional): prediction score. Default to None.
             task (Union[str, TaskType], optional): task type. Default to None.
 
         Returns:
             Annotation: annotation class
         """
-        return cls(
+        return (getattr(cls, task.lower()) if task else cls)(
             annotation_id=annotation_id,
             image_id=image_id,
             category_id=category_id,
             bbox=bbox,
             segmentation=segmentation,
             area=area,
             keypoints=keypoints,
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/fields/base_field.py` & `waffle_hub-0.2.6/waffle_hub/schema/fields/base_field.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from waffle_hub import TaskType
 
 
 class BaseField(ABC):
     def __init__(self):
         pass
 
+    def __repr__(self) -> str:
+        return f"{self.__class__.__name__}({', '.join([f'{k}={v}' for k, v in self.to_dict().items()])})"
+
+    def __str__(self) -> str:
+        return self.__repr__()
+
     @abstractmethod
     def to_dict(self):
         pass
 
     @classmethod
     @abstractmethod
     def new(cls):
@@ -47,7 +53,10 @@
             task (str, optional): task name. Default to None.
 
         Returns:
             Field Object: Field Object.
         """
         d: dict = io.load_json(f)
         return cls.from_dict(d, task)
+
+    def __getitem__(self, key):
+        return getattr(self, key)
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/fields/category.py` & `waffle_hub-0.2.6/waffle_hub/schema/fields/category.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,15 @@
             keypoints (list[str]): category name.
             skeleton (list[list[int]]): skeleton edges.
             task (Union[str, TaskType], optional): task type. Default to None.
 
         Returns:
             Category: category class
         """
-        return cls(
+        return (getattr(cls, task.lower()) if task else cls)(
             category_id=category_id,
             name=name,
             supercategory=supercategory,
             keypoints=keypoints,
             skeleton=skeleton,
             task=task,
         )
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/fields/image.py` & `waffle_hub-0.2.6/waffle_hub/schema/fields/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,21 +9,23 @@
         self,
         # required
         image_id: int,
         file_name: str,
         width: int,
         height: int,
         # optional
+        original_file_name: str = None,
         date_captured: str = None,
     ):
 
         self.image_id = image_id
         self.file_name = file_name
         self.width = width
         self.height = height
+        self.original_file_name = original_file_name
         self.date_captured = date_captured
 
     # properties
     @property
     def image_id(self):
         return self.__image_id
 
@@ -35,15 +37,15 @@
         self.__image_id = v
 
     @property
     def file_name(self):
         return self.__file_name
 
     @file_name.setter
-    @type_validator(str)
+    @type_validator(str, strict=False)
     def file_name(self, v):
         self.__file_name = v
 
     @property
     def width(self):
         return self.__width
 
@@ -58,14 +60,23 @@
 
     @height.setter
     @type_validator(int)
     def height(self, v):
         self.__height = v
 
     @property
+    def original_file_name(self):
+        return self.__original_file_name
+
+    @original_file_name.setter
+    @type_validator(str, strict=False)
+    def original_file_name(self, v):
+        self.__original_file_name = v or self.file_name
+
+    @property
     def date_captured(self):
         return self.__date_captured
 
     @date_captured.setter
     @type_validator(str)
     def date_captured(self, v):
         if v is None:
@@ -76,24 +87,26 @@
     @classmethod
     def new(
         cls,
         image_id: int,
         file_name: str,
         width: int,
         height: int,
+        original_file_name: str = None,
         date_captured: str = None,
         **kwargs,
     ) -> "Image":
         """Image Format
 
         Args:
             image_id (int): image id. natural number.
             file_name (str): file name. relative file path.
             width (int): image width.
             height (int): image height.
+            original_file_name (str): original file name. relative file path.
             date_captured (str): date_captured string. "%Y-%m-%d %H:%M:%S"
 
         Returns:
             Image: image class
         """
         return cls(image_id, file_name, width, height, date_captured)
 
@@ -105,11 +118,12 @@
         """
 
         cat = {
             "image_id": self.image_id,
             "file_name": self.file_name,
             "width": self.width,
             "height": self.height,
+            "original_file_name": self.original_file_name,
             "date_captured": self.date_captured,
         }
 
         return cat
```

### Comparing `waffle_hub-0.2.5/waffle_hub/schema/result.py` & `waffle_hub-0.2.6/waffle_hub/schema/result.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/base_cli.py` & `waffle_hub-0.2.6/waffle_hub/utils/base_cli.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/callback.py` & `waffle_hub-0.2.6/waffle_hub/utils/callback.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/conversion.py` & `waffle_hub-0.2.6/waffle_hub/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/data.py` & `waffle_hub-0.2.6/waffle_hub/utils/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from pathlib import Path
 from typing import Union
 
 import cv2
 import numpy as np
 import torch
+from natsort import natsorted
 from torchvision import transforms as T
 from waffle_utils.file import io
 
 from waffle_hub.dataset import Dataset
 from waffle_hub.schema.data import ImageInfo
 from waffle_hub.schema.fields import Annotation, Category, Image
 
 
 def get_images(d, recursive: bool = True) -> list[str]:
     exp = "**/*" if recursive else "*"
     image_paths = []
     for ext in ["png", "jpg", "jpeg", "bmp", "tif", "tiff"]:
         image_paths += list(Path(d).glob(exp.lower() + "." + ext))
         image_paths += list(Path(d).glob(exp.upper() + "." + ext))
-    return list(
-        set(
-            map(
-                str,
-                image_paths,
+    return natsorted(
+        list(
+            set(
+                map(
+                    str,
+                    image_paths,
+                )
             )
         )
     )
 
 
 def resize_image(
     image: np.ndarray, image_size: list[int], letter_box: bool = False
@@ -99,20 +102,21 @@
 
 class ImageDataset:
     def __init__(
         self,
         image_dir: str,
         image_size: Union[int, list[int]],
         letter_box: bool = False,
+        recursive: bool = True,
     ):
         self.image_dir = image_dir
         if Path(self.image_dir).is_file():
             self.image_paths = [self.image_dir]
         else:
-            self.image_paths = get_images(self.image_dir)
+            self.image_paths = get_images(self.image_dir, recursive=recursive)
 
         self.transform = get_image_transform(image_size, letter_box)
 
     def __len__(self):
         return len(self.image_paths)
 
     def __getitem__(self, idx):
```

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/draw.py` & `waffle_hub-0.2.6/waffle_hub/utils/draw.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/evaluate.py` & `waffle_hub-0.2.6/waffle_hub/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub/utils/process.py` & `waffle_hub-0.2.6/waffle_hub/utils/process.py`

 * *Files identical despite different names*

### Comparing `waffle_hub-0.2.5/waffle_hub.egg-info/PKG-INFO` & `waffle_hub-0.2.6/waffle_hub.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: waffle-hub
-Version: 0.2.5
+Version: 0.2.6
 Summary: Waffle hub
 Home-page: https://github.com/snuailab/waffle_hub
 Author: SNUAILAB
 Author-email: huijae.lee@snuailab.ai
 License: GPL-3.0
 Project-URL: Bug Reports, https://github.com/snuailab/waffle_hub/issues
 Project-URL: Source, https://github.com/snuailab/waffle_hub
@@ -77,15 +77,15 @@
   name = "my_classifier",
   task = "classification",
   model_type = "yolov8",
   model_size = "n",
   categories = dataset.get_category_names(),
 )
 hub.train(
-  dataset_path = export_dir,
+  dataset = dataset,
   epochs = 30,
   batch_size = 64,
   image_size=64,
   device="cpu"
 )
 hub.inference(
   source=export_dir,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.5 Summary: Waffle hub Home-
+Metadata-Version: 2.1 Name: waffle-hub Version: 0.2.6 Summary: Waffle hub Home-
 page: https://github.com/snuailab/waffle_hub Author: SNUAILAB Author-email:
 huijae.lee@snuailab.ai License: GPL-3.0 Project-URL: Bug Reports, https://
 github.com/snuailab/waffle_hub/issues Project-URL: Source, https://github.com/
 snuailab/waffle_hub Keywords: machine-learning,deep-
 learning,vision,ML,DL,AI,YOLO,Ultralytics,SNUAILAB Classifier: Development
 Status :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
@@ -41,16 +41,16 @@
 both python module and CLI for Waffle Hub. Following examples do the exact same
 thing. ## Python Module ```python from waffle_hub.dataset import Dataset
 dataset = Dataset.sample( name = "mnist_classification", task =
 "classification", ) dataset.split( train_ratio = 0.8, val_ratio = 0.1,
 test_ratio = 0.1 ) export_dir = dataset.export("YOLO") from waffle_hub.hub
 import Hub hub = Hub.new( name = "my_classifier", task = "classification",
 model_type = "yolov8", model_size = "n", categories =
-dataset.get_category_names(), ) hub.train( dataset_path = export_dir, epochs =
-30, batch_size = 64, image_size=64, device="cpu" ) hub.inference
+dataset.get_category_names(), ) hub.train( dataset = dataset, epochs = 30,
+batch_size = 64, image_size=64, device="cpu" ) hub.inference
 ( source=export_dir, draw=True, device="cpu" ) ``` ## CLI ```bash wd sample --
 name mnist_classification --task classification wd split --name
 mnist_classification --train-ratio 0.8 --val-ratio 0.1 --test-ratio 0.1 wd
 export --name mnist_classification --data-type YOLO wh new --name my_classifier
 --task classification --model-type yolov8 --model-size n --categories [1,2] wh
 train --name my_classifier --dataset-path datasets/mnist_classification/
 exports/YOLO --epochs 30 --batch-size 64 --image-size 64 --device cpu wh
```

### Comparing `waffle_hub-0.2.5/waffle_hub.egg-info/SOURCES.txt` & `waffle_hub-0.2.6/waffle_hub.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -59,8 +59,9 @@
 waffle_hub/utils/__init__.py
 waffle_hub/utils/base_cli.py
 waffle_hub/utils/callback.py
 waffle_hub/utils/conversion.py
 waffle_hub/utils/data.py
 waffle_hub/utils/draw.py
 waffle_hub/utils/evaluate.py
+waffle_hub/utils/metric_logger.py
 waffle_hub/utils/process.py
```

