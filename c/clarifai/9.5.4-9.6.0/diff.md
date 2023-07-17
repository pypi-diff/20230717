# Comparing `tmp/clarifai-9.5.4.tar.gz` & `tmp/clarifai-9.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clarifai-9.5.4.tar", last modified: Fri Jul  7 03:43:06 2023, max compression
+gzip compressed data, was "clarifai-9.6.0.tar", last modified: Mon Jul 17 14:39:44 2023, max compression
```

## Comparing `clarifai-9.5.4.tar` & `clarifai-9.6.0.tar`

### file list

```diff
@@ -1,222 +1,500 @@
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.687991 clarifai-9.5.4/
--rw-r--r--   0 zeiler     (503) staff       (20)      555 2021-12-09 18:28:59.000000 clarifai-9.5.4/LICENSE
--rw-r--r--   0 zeiler     (503) staff       (20)       21 2022-07-01 04:22:44.000000 clarifai-9.5.4/MANIFEST.in
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-07 03:43:06.687494 clarifai-9.5.4/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     2347 2023-01-03 21:48:03.000000 clarifai-9.5.4/README.md
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.086894 clarifai-9.5.4/clarifai/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.111755 clarifai-9.5.4/clarifai/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12447 2023-07-06 20:14:23.000000 clarifai-9.5.4/clarifai/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.131953 clarifai-9.5.4/clarifai/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.5.4/clarifai/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.151928 clarifai-9.5.4/clarifai/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/data_upload/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/convert_csv.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.163732 clarifai-9.5.4/clarifai/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10486 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2093 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.172579 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1606 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.074494 clarifai-9.5.4/clarifai/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.173216 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.175154 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.177317 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.178043 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.180432 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.207181 clarifai-9.5.4/clarifai/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.263748 clarifai-9.5.4/clarifai/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.269555 clarifai-9.5.4/clarifai/models/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     8691 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.297011 clarifai-9.5.4/clarifai/models/model_serving/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.346975 clarifai-9.5.4/clarifai/models/model_serving/cli/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3119 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/model_zip.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/cli/repository.py
--rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/constants.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076585 clarifai-9.5.4/clarifai/models/model_serving/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.075923 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076022 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.385846 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2021 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076307 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076416 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.401464 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1958 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076687 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.076799 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.427973 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 zeiler     (503) staff       (20)     2625 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.478042 clarifai-9.5.4/clarifai/models/model_serving/model_config/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1763 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/deploy.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/serializer.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.532663 clarifai-9.5.4/clarifai/models/model_serving/models/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1548 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3743 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/model_types.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/output.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/models/pb_model.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3408 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.562087 clarifai-9.5.4/clarifai/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:36:17.000000 clarifai-9.5.4/clarifai/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.564353 clarifai-9.5.4/clarifai/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.4/clarifai/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.5.4/clarifai/urls/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.096804 clarifai-9.5.4/clarifai.egg-info/
--rw-r--r--   0 zeiler     (503) staff       (20)     2882 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/PKG-INFO
--rw-r--r--   0 zeiler     (503) staff       (20)     7394 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/SOURCES.txt
--rw-r--r--   0 zeiler     (503) staff       (20)        1 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/dependency_links.txt
--rw-r--r--   0 zeiler     (503) staff       (20)      255 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/entry_points.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       52 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/requires.txt
--rw-r--r--   0 zeiler     (503) staff       (20)       24 2023-07-07 03:43:05.000000 clarifai-9.5.4/clarifai.egg-info/top_level.txt
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.565482 clarifai-9.5.4/clarifai_utils/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.568124 clarifai-9.5.4/clarifai_utils/auth/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/auth/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)    12447 2023-07-06 20:14:23.000000 clarifai-9.5.4/clarifai_utils/auth/helper.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.576809 clarifai-9.5.4/clarifai_utils/client/
--rw-r--r--   0 zeiler     (503) staff       (20)      121 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/client/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)      536 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/client/abc.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3606 2023-07-06 20:11:16.000000 clarifai-9.5.4/clarifai_utils/client/stub.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.581329 clarifai-9.5.4/clarifai_utils/data_upload/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/data_upload/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7331 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/convert_csv.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.586000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1693 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/base.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1289 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/features.py
--rw-r--r--   0 zeiler     (503) staff       (20)    10486 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/image.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2093 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/text.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.594900 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3651 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4856 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6196 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1606 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6451 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.079318 clarifai-9.5.4/clarifai_utils/data_upload/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.596226 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.597910 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1091 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.600318 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1195 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.602003 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.606551 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1049 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
--rw-r--r--   0 zeiler     (503) staff       (20)      540 2023-03-23 03:08:12.000000 clarifai-9.5.4/clarifai_utils/data_upload/examples.py
--rw-r--r--   0 zeiler     (503) staff       (20)    13040 2023-06-02 04:02:11.000000 clarifai-9.5.4/clarifai_utils/data_upload/upload.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.608606 clarifai-9.5.4/clarifai_utils/dataset_export/
--rw-r--r--   0 zeiler     (503) staff       (20)     7475 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/dataset_export/dataset_export_inputs.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.630441 clarifai-9.5.4/clarifai_utils/listing/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1169 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/concepts.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1184 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/datasets.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3632 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/inputs.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1466 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/installed_module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     7764 2023-05-01 19:51:07.000000 clarifai-9.5.4/clarifai_utils/listing/lister.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1506 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/listing/models.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1480 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/module_versions.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1170 2023-04-11 15:50:37.000000 clarifai-9.5.4/clarifai_utils/listing/modules.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.634556 clarifai-9.5.4/clarifai_utils/models/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     8691 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/api.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.637112 clarifai-9.5.4/clarifai_utils/models/model_serving/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/__init__.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.643938 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3119 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/deploy_cli.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1866 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/model_zip.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1947 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/cli/repository.py
--rw-r--r--   0 zeiler     (503) staff       (20)      112 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/constants.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081330 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080616 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080717 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.647383 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2021 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.080977 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081093 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.650612 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1958 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081435 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.081532 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.652647 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
--rw-r--r--   0 zeiler     (503) staff       (20)     2625 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.657629 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1763 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/deploy.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4231 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/serializer.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4489 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/triton_config.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.663741 clarifai-9.5.4/clarifai_utils/models/model_serving/models/
--rw-r--r--   0 zeiler     (503) staff       (20)      575 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1548 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/inference.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3743 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/model_types.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2334 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/output.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1955 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/models/pb_model.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3408 2023-07-06 20:12:20.000000 clarifai-9.5.4/clarifai_utils/models/model_serving/pb_model_repository.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.680353 clarifai-9.5.4/clarifai_utils/modules/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     2020 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/css.py
--rw-r--r--   0 zeiler     (503) staff       (20)     1383 2023-01-03 21:48:03.000000 clarifai-9.5.4/clarifai_utils/modules/pages.py
--rw-r--r--   0 zeiler     (503) staff       (20)     6003 2023-06-02 20:36:17.000000 clarifai-9.5.4/clarifai_utils/modules/style.css
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.683313 clarifai-9.5.4/clarifai_utils/urls/
--rw-r--r--   0 zeiler     (503) staff       (20)        0 2022-07-20 04:15:05.000000 clarifai-9.5.4/clarifai_utils/urls/__init__.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4276 2023-07-07 03:41:06.000000 clarifai-9.5.4/clarifai_utils/urls/helper.py
--rw-r--r--   0 zeiler     (503) staff       (20)       38 2023-07-07 03:43:06.688134 clarifai-9.5.4/setup.cfg
--rw-r--r--   0 zeiler     (503) staff       (20)     1297 2023-07-07 03:42:20.000000 clarifai-9.5.4/setup.py
-drwxr-xr-x   0 zeiler     (503) staff       (20)        0 2023-07-07 03:43:06.686764 clarifai-9.5.4/tests/
--rw-r--r--   0 zeiler     (503) staff       (20)     2300 2023-07-06 20:15:48.000000 clarifai-9.5.4/tests/test_auth.py
--rw-r--r--   0 zeiler     (503) staff       (20)     4771 2023-07-07 03:39:45.000000 clarifai-9.5.4/tests/test_modules.py
--rw-r--r--   0 zeiler     (503) staff       (20)     3716 2023-01-03 21:48:03.000000 clarifai-9.5.4/tests/test_stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.257110 clarifai-9.6.0/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      555 2023-06-01 21:00:24.000000 clarifai-9.6.0/LICENSE
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      119 2023-07-17 14:39:38.000000 clarifai-9.6.0/MANIFEST.in
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-07-17 14:39:44.256940 clarifai-9.6.0/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2347 2023-06-01 21:00:24.000000 clarifai-9.6.0/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.186212 clarifai-9.6.0/clarifai/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.187125 clarifai-9.6.0/clarifai/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12447 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.188476 clarifai-9.6.0/clarifai/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.190028 clarifai-9.6.0/clarifai/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3487 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7331 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/convert_csv.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.191163 clarifai-9.6.0/clarifai/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2546 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10249 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2074 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192201 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3961 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3684 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4894 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6291 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1605 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192340 clarifai-9.6.0/clarifai/data_upload/examples/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.192494 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.193192 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/cifar_small_test.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/cifar_small_train.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.194934 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      963 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_700.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      921 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_701.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      907 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_702.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      828 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_703.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      922 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_704.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      877 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_705.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      859 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_706.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      937 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_707.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      875 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_708.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/images/test_batch_709.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.195242 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.177597 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.198455 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    59900 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1036242.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1114182.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49005 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/1420783.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    63984 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/2012944.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    62530 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/2464389.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49264 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/3287885.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    43410 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/3617075.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    33826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/38052.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47755 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/39147.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/beignets/478632.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.202048 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    96729 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1061270.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    55702 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1202261.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    48391 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1381751.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    43856 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/139558.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47022 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    46176 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    63224 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3289634.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    37327 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    32557 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54823 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/hamburger/862025.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.205201 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    53968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/102197.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    26278 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    45386 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    40566 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    67808 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2749372.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47620 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    53419 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/2938268.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    52635 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    55723 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/3590861.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    56940 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/prime_rib/746716.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209134 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    44858 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/1545393.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49950 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/2427642.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    58221 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/2955110.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    64028 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3208966.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    62079 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3270629.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    58751 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3424562.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    51306 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/3520891.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    34567 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/377566.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    56869 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/503504.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    64261 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/images/ramen/544680.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209348 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.209548 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.211244 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      760 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2007_000464.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      572 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_000853.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1075 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_003182.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1319 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2008_008526.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2009_004315.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2009_004382.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      568 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_000430.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      874 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_001610.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2088 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2011_006412.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      914 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/annotations/2012_000690.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2692 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214274 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99806 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2007_000464.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99739 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_000853.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99737 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_003182.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99774 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2008_008526.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99802 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2009_004315.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99794 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2009_004382.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99823 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_000430.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99784 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_001610.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99748 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2011_006412.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99747 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_detection/voc/images/2012_000690.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214776 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.214994 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.215551 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/annotations/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   139780 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/annotations/instances_val2017_subset.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4235 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.219013 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101406 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000074646.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101836 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000086956.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101772 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000166563.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101669 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000176857.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101496 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000182202.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101592 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000193245.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101791 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000384850.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000409630.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101426 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000424349.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101539 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/examples/image_segmentation/coco/images/000000573008.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.220587 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.221922 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   237144 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/test.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   270347 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/train.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.222645 clarifai-9.6.0/clarifai/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7475 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.223832 clarifai-9.6.0/clarifai/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.224039 clarifai-9.6.0/clarifai/models/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     9555 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/api.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.224652 clarifai-9.6.0/clarifai/models/model_serving/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6903 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225139 clarifai-9.6.0/clarifai/models/model_serving/cli/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3825 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1866 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1947 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/cli/repository.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      112 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/constants.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225503 clarifai-9.6.0/clarifai/models/model_serving/docs/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1027 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/dependencies.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      943 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/model_types.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/docs/output.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225627 clarifai-9.6.0/clarifai/models/model_serving/envs/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1030 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/envs/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225753 clarifai-9.6.0/clarifai/models/model_serving/examples/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      623 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.225876 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      469 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.226522 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.226909 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2251 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227306 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      177 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      850 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      198 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      344 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       57 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227445 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.227987 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228328 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2173 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228725 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      588 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      841 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      151 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      326 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       26 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.228853 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      521 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.229354 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.229603 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2906 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      520 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      621 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      281 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.230087 clarifai-9.6.0/clarifai/models/model_serving/model_config/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1731 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4231 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4489 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.230684 clarifai-9.6.0/clarifai/models/model_serving/models/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1639 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3701 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/model_types.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2334 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/output.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/models/pb_model.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3411 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231247 clarifai-9.6.0/clarifai/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      367 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai/modules/pages.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6003 2023-06-02 20:18:09.000000 clarifai-9.6.0/clarifai/modules/style.css
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231466 clarifai-9.6.0/clarifai/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4276 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai/urls/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.186922 clarifai-9.6.0/clarifai.egg-info/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2882 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/PKG-INFO
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    27508 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/SOURCES.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        1 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/dependency_links.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      255 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/entry_points.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       52 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/requires.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       24 2023-07-17 14:39:44.000000 clarifai-9.6.0/clarifai.egg-info/top_level.txt
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231589 clarifai-9.6.0/clarifai_utils/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.231763 clarifai-9.6.0/clarifai_utils/auth/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/auth/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    12447 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/auth/helper.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.232096 clarifai-9.6.0/clarifai_utils/client/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      121 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      536 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/abc.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3606 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/client/stub.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.232614 clarifai-9.6.0/clarifai_utils/data_upload/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3487 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7331 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/convert_csv.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233134 clarifai-9.6.0/clarifai_utils/data_upload/datasets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2546 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/base.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1289 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/features.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    10249 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/image.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2074 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/text.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233887 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3961 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3684 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4894 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6291 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1605 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6451 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.233998 clarifai-9.6.0/clarifai_utils/data_upload/examples/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.234114 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.234526 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/cifar_small_test.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      299 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/cifar_small_train.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1091 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.235648 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      963 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_700.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      921 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_701.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      907 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_702.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      828 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_703.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      922 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_704.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      877 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_705.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      859 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_706.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      937 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_707.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      875 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_708.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/images/test_batch_709.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.235849 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1195 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.181226 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.237226 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    59900 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1036242.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54450 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1114182.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49005 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/1420783.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    63984 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/2012944.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    62530 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/2464389.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49264 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/3287885.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    43410 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/3617075.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    33826 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/38052.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47755 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/39147.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/beignets/478632.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.238749 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    96729 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1061270.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    55702 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1202261.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    48391 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1381751.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    43856 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/139558.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47022 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/1636096.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    46176 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/2480925.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    63224 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3289634.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    37327 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3385808.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    32557 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/3647386.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    54823 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/hamburger/862025.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.240185 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    53968 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/102197.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    26278 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/1826869.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    45386 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2243245.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    40566 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/259212.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    67808 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2749372.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    47620 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2842688.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    53419 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/2938268.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    52635 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/3035414.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    55723 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/3590861.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    56940 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/prime_rib/746716.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241596 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    44858 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/1545393.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    49950 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/2427642.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    58221 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/2955110.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    64028 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3208966.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    62079 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3270629.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    58751 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3424562.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    51306 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/3520891.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    34567 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/377566.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    56869 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/503504.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    64261 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/images/ramen/544680.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241739 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.241943 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.243046 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      760 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2007_000464.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      572 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_000853.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1075 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_003182.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1319 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2008_008526.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2009_004315.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      570 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2009_004382.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      568 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_000430.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      874 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_001610.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2088 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2011_006412.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      914 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/annotations/2012_000690.xml
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2692 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244595 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99806 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2007_000464.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99739 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_000853.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99737 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_003182.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99774 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2008_008526.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99802 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2009_004315.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99794 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2009_004382.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99823 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_000430.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99784 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_001610.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99748 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2011_006412.jpg
+-rwxr-xr-x   0 yvettezhang   (501) staff       (20)    99747 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_detection/voc/images/2012_000690.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244770 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.244982 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.245103 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/annotations/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   139780 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/annotations/instances_val2017_subset.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4235 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/dataset.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.246754 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101406 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000074646.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101836 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000086956.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101772 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000166563.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101669 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000176857.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101496 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000182202.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101592 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000193245.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101791 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000384850.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000409630.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101426 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000424349.jpg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   101539 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/image_segmentation/coco/images/000000573008.jpg
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.246907 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.247411 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1049 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   237144 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/test.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)   270347 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/train.csv
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      540 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/data_upload/examples.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)    13507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/data_upload/upload.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.247635 clarifai-9.6.0/clarifai_utils/dataset_export/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7475 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/dataset_export/dataset_export_inputs.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.248561 clarifai-9.6.0/clarifai_utils/listing/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1169 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/concepts.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1184 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/datasets.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3632 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/inputs.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1466 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/installed_module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     7764 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/lister.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1506 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/models.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1480 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/module_versions.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1170 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/listing/modules.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.248768 clarifai-9.6.0/clarifai_utils/models/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     9555 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/api.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249215 clarifai-9.6.0/clarifai_utils/models/model_serving/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6903 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/__init__.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249653 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3825 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/deploy_cli.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1866 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/model_zip.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1947 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/cli/repository.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      112 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/constants.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.249991 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1027 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/dependencies.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      943 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/model_types.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1507 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/docs/output.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250107 clarifai-9.6.0/clarifai_utils/models/model_serving/envs/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1030 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/envs/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250223 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      623 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250344 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      469 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.250806 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251133 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2251 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251513 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      177 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      850 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      198 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/vit-age-classifier/preprocessor_config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      344 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       57 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.251663 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      556 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.252473 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.252850 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2173 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.253290 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      588 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      841 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/config.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      151 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/twitter-xlm-roberta-base-sentiment/special_tokens_map.json
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      326 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       26 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      134 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.253416 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      521 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/README.md
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254016 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254296 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2906 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      520 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/config.pbtxt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      621 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/labels.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      281 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/requirements.txt
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       46 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/triton_conda.yaml
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.254861 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1731 2023-07-17 12:20:05.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/deploy.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4231 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/serializer.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4489 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/triton_config.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.255545 clarifai-9.6.0/clarifai_utils/models/model_serving/models/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      575 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1639 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/inference.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3701 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/model_types.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2334 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/output.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1941 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/models/pb_model.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3411 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/models/model_serving/pb_model_repository.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256116 clarifai-9.6.0/clarifai_utils/modules/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)      367 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/README.md
+-rw-r--r--   0 yvettezhang   (501) staff       (20)        0 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/__init__.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2020 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/css.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1383 2023-06-01 21:00:24.000000 clarifai-9.6.0/clarifai_utils/modules/pages.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     6003 2023-06-02 20:18:09.000000 clarifai-9.6.0/clarifai_utils/modules/style.css
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256232 clarifai-9.6.0/clarifai_utils/urls/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4276 2023-07-13 14:56:23.000000 clarifai-9.6.0/clarifai_utils/urls/helper.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)       38 2023-07-17 14:39:44.257149 clarifai-9.6.0/setup.cfg
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     1297 2023-07-17 14:37:15.000000 clarifai-9.6.0/setup.py
+drwxr-xr-x   0 yvettezhang   (501) staff       (20)        0 2023-07-17 14:39:44.256631 clarifai-9.6.0/tests/
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     2300 2023-07-13 14:56:23.000000 clarifai-9.6.0/tests/test_auth.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     4771 2023-07-13 14:56:23.000000 clarifai-9.6.0/tests/test_modules.py
+-rw-r--r--   0 yvettezhang   (501) staff       (20)     3716 2023-06-01 21:00:24.000000 clarifai-9.6.0/tests/test_stub.py
```

### Comparing `clarifai-9.5.4/LICENSE` & `clarifai-9.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/PKG-INFO` & `clarifai-9.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.4
+Version: 9.6.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.4/README.md` & `clarifai-9.6.0/README.md`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/auth/helper.py` & `clarifai-9.6.0/clarifai/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/client/abc.py` & `clarifai-9.6.0/clarifai/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/client/stub.py` & `clarifai-9.6.0/clarifai/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/convert_csv.py` & `clarifai-9.6.0/clarifai/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/features.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/image.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
-from typing import Iterator, List, Tuple, Union
+from typing import Iterator, List, Union
 
 from clarifai_grpc.grpc.api import resources_pb2
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
 
 from .base import ClarifaiDataset
 
 
 class VisualClassificationDataset(ClarifaiDataset):
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, labels: List[Union[str, int]], input_id: str,
                           dataset_id: str, geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -42,43 +43,40 @@
                   id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)\
                 for _label in labels
             ],
             metadata=metadata))
 
     return input_proto
 
-  def _get_input_protos(self) -> Iterator:
+  def _extract_protos(self) -> None:
     """
     Create input image protos for each data generator item.
-    Returns:
-      Input proto iterator
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       geo_info = item.geo_info
       metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
+      self.input_ids.append(input_id)
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
                                              geo_info, metadata)
-      self._all_input_protos.append(input_proto)
-
-    return iter(self._all_input_protos)
+      self._all_input_protos[input_id] = input_proto
 
 
 class VisualDetectionDataset(ClarifaiDataset):
   """
   Visual detection dataset proto class.
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
-    self._annotation_protos = []
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
                           geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -131,51 +129,48 @@
                     resources_pb2.Concept(
                         id=f"id-{''.join(label.split(' '))}", name=label, value=1.)
                 ]))
         ]))
 
     return input_annot_proto
 
-  def _get_input_protos(self) -> Tuple[Iterator, Iterator]:
+  def _extract_protos(self) -> None:
     """
     Create input image protos for each data generator item.
-    Returns:
-      Input and Annotation proto iterators.
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
+      self.input_ids.append(input_id)
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
-      self._all_input_protos.append(input_image_proto)
+      self._all_input_protos[input_id] = input_image_proto
 
       # iter over bboxes and classes
       # one id could have more than one bbox and label
       for i in range(len(bboxes)):
         input_annot_proto = self.create_annotation_proto(labels[i], bboxes[i], input_id,
                                                          self.dataset_id)
-        self._annotation_protos.append(input_annot_proto)
-
-    return iter(self._all_input_protos), iter(self._annotation_protos)
+        self._all_annotation_protos[input_id].append(input_annot_proto)
 
 
 class VisualSegmentationDataset(ClarifaiDataset):
   """
   Visual segmentation dataset proto class.
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
-    self._mask_protos = []  # mask or polygon protos
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
                           geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -226,36 +221,33 @@
                     resources_pb2.Concept(
                         id=f"id-{''.join(label.split(' '))}", name=label, value=1.)
                 ]))
         ]))
 
     return input_mask_proto
 
-  def _get_input_protos(self) -> Tuple[Iterator, Iterator]:
+  def _extract_protos(self) -> None:
     """
     Create input image and annotation protos for each data generator item.
-    Returns:
-      Input and Annotation proto iterators.
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
+      self.input_ids.append(input_id)
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
-      self._all_input_protos.append(input_image_proto)
+      self._all_input_protos[input_id] = input_image_proto
 
       ## Iterate over each masked image and create a proto for upload to clarifai
       ## The length of masks/polygons-list and labels must be equal
       for i, _polygon in enumerate(_polygons):
         try:
           input_mask_proto = self.create_mask_proto(labels[i], _polygon, input_id, self.dataset_id)
-          self._mask_protos.append(input_mask_proto)
+          self._all_annotation_protos[input_id].append(input_mask_proto)
         except IndexError:
           continue
-
-    return iter(self._all_input_protos), iter(self._mask_protos)
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/text.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class TextClassificationDataset(ClarifaiDataset):
   """
   Upload text classification datasets to clarifai datasets
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
+    self._extract_protos()
 
   def create_input_protos(self, text_input: str, labels: List[str], input_id: str, dataset_id: str,
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each text, label input pairs.
     Args:
     	`text_input`: text string.
@@ -38,25 +39,22 @@
                     id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)
                 for _label in labels
             ],
             metadata=metadata))
 
     return input_proto
 
-  def _get_input_protos(self) -> Iterator:
+  def _extract_protos(self) -> None:
     """
     Creates input protos for each data generator item.
-    Returns:
-    	A list of input protos
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Loading text data"):
       metadata = Struct()
       text = item.text
       labels = item.labels if isinstance(item.labels, list) else [item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"split": self.split})
 
+      self.input_ids.append(input_id)
       input_proto = self.create_input_protos(text, labels, input_id, self.dataset_id, metadata)
 
-      self._all_input_protos.append(input_proto)
-
-    return iter(self._all_input_protos)
+      self._all_input_protos[input_id] = input_proto
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_captions.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,38 +14,39 @@
 class COCOCaptionsDataset:
   """COCO 2017 Image Captioning Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory.
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train, val and annotation dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("Dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -70,30 +71,30 @@
   def dataloader(self):
     """
     Transform coco image captioning data into clarifai proto compatible
     format for upload.
     Returns:
       VisualClassificationFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:  #train, val, annotations
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:  #train, val, annotations
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 3 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 3 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" + f"captions_{self.split}*")[0]
     coco = COCO(annot_file)
     annot_ids = coco.getAnnIds()
     annotations = coco.loadAnns(annot_ids)
     for annot in annotations:
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(annot['image_id']).zfill(12)}*")[0]
       # image_captioning and image classification datasets have the same
       # image-label input feature formats
-      yield VisualClassificationFeatures(image_path, annot["caption"], annot["image_id"])
+      yield VisualClassificationFeatures(image_path, annot["caption"], id=annot["image_id"])
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 class COCODetectionDataset:
   """COCO 2017 Image Detection Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory.
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train*, val* and annotation* dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -71,25 +72,25 @@
   def dataloader(self):
     """
     Transform coco object detection data into clarifai proto compatible
     format for upload.
     Returns:
       VisualDetectionFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 2 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 2 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" +\
      f"instances_{self.split}*")[0]
     coco = COCO(annot_file)
     categories = coco.loadCats(coco.getCatIds())
     cat_id_map = {category["id"]: category["name"] for category in categories}
@@ -98,15 +99,15 @@
       cat_img_ids[cat_id] = coco.getImgIds(catIds=[cat_id])
 
     img_ids = []
     for i in list(cat_img_ids.values()):
       img_ids.extend(i)
 
     #get annotations for each image id
-    for _id in img_ids:
+    for _id in set(img_ids):
       annots = []  # bboxes
       class_names = []
       labels = [i for i in list(filter(lambda x: _id in cat_img_ids[x], cat_img_ids))]
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(_id).zfill(12)}*")[0]
 
       image_height, image_width = cv2.imread(image_path).shape[:2]
@@ -122,8 +123,8 @@
             y_max = (ann['bbox'][1] + ann['bbox'][3]) / image_height  #bottom_row
             annots.append([x_min, y_min, x_max, y_max])
         else:  # if no annotations for given image_id-cat_id pair
           continue
       assert len(class_names) == len(annots), f"Num classes must match num bbox annotations\
       for a single image. Found {len(class_names)} classes and {len(annots)} bboxes."
 
-      yield VisualDetectionFeatures(image_path, class_names, annots, _id)
+      yield VisualDetectionFeatures(image_path, class_names, annots, id=_id)
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,38 +19,39 @@
 class COCOSegmentationDataset:
   """COCO 2017 Image Segmentation Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage dir
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage dir
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train, val and annotation dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -74,25 +75,25 @@
 
   def dataloader(self):
     """
     Transform coco data into clarifai proto compatible format for upload.
     Returns:
       VisualSegmentationFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 3 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 3 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" +\
      f"instances_{self.split}*")[0]
     coco = COCO(annot_file)
     categories = coco.loadCats(coco.getCatIds())
     cat_id_map = {category["id"]: category["name"] for category in categories}
@@ -101,34 +102,34 @@
       cat_img_ids[cat_id] = coco.getImgIds(catIds=[cat_id])
 
     img_ids = []
     for i in list(cat_img_ids.values()):
       img_ids.extend(i)
 
     #get annotations for each image id
-    for _id in img_ids:
+    for _id in set(img_ids):
       annots = []  # polygons
       class_names = []
       labels = [i for i in list(filter(lambda x: _id in cat_img_ids[x], cat_img_ids))]
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(_id).zfill(12)}*")[0]
 
       image_height, image_width = cv2.imread(image_path).shape[:2]
       for cat_id in labels:
         annot_ids = coco.getAnnIds(imgIds=_id, catIds=[cat_id])
         if len(annot_ids) > 0:
           img_annotations = coco.loadAnns(annot_ids)
           for ann in img_annotations:
-            class_names.append(cat_id_map[cat_id])
             # get polygons
             if type(ann['segmentation']) == list:
               for seg in ann['segmentation']:
                 poly = np.array(seg).reshape((int(len(seg) / 2), 2))
                 poly[:, 0], poly[:, 1] = poly[:, 0] / image_width, poly[:, 1] / image_height
                 annots.append(poly.tolist())  #[[x=col, y=row],...]
+                class_names.append(cat_id_map[cat_id])
             else:  # seg: {"counts":[...]}
               if type(ann['segmentation']['counts']) == list:
                 rle = maskUtils.frPyObjects([ann['segmentation']], image_height, image_width)
               else:
                 rle = ann['segmentation']
               mask = maskUtils.decode(rle)  #binary mask
               #convert mask to polygons and add to annots
@@ -146,13 +147,14 @@
 
               polygons = np.array(polygons_flattened).reshape((int(len(polygons_flattened) / 2),
                                                                2))
               polygons[:, 0] = polygons[:, 0] / image_width
               polygons[:, 1] = polygons[:, 1] / image_height
 
               annots.append(polygons.tolist())  #[[x=col, y=row],...,[x=col, y=row]]
+              class_names.append(cat_id_map[cat_id])
         else:  # if no annotations for given image_id-cat_id pair
           continue
       assert len(class_names) == len(annots), f"Num classes must match num annotations\
       for a single image. Found {len(class_names)} classes and {len(annots)} polygons."
 
-      yield VisualSegmentationFeatures(image_path, class_names, annots, _id)
+      yield VisualSegmentationFeatures(image_path, class_names, annots, id=_id)
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Initialize dataset params.
     Args:
       data_dir: the local dataset directory.
       split: "train" or "test"
     """
     self.split = split
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.label_map = dict()
 
   def dataloader(self):
     """
     Transform text data into clarifai proto compatible
     format for upload.
     Returns:
```

### Comparing `clarifai-9.5.4/clarifai/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.0/clarifai/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.0/clarifai/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.0/clarifai/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.0/clarifai/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/examples.py` & `clarifai-9.6.0/clarifai/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/data_upload/upload.py` & `clarifai-9.6.0/clarifai/data_upload/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #! Clarifai data upload
 
 import importlib
 import inspect
 import os
 import sys
+import time
+import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
 from typing import Iterator, List, Optional, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2, service_pb2_grpc
-from clarifai_grpc.grpc.api.status import status_code_pb2
+from clarifai_grpc.grpc.api.status import status_code_pb2, status_pb2
+from google.protobuf.json_format import MessageToDict
 from tqdm import tqdm
 
 from clarifai.client import create_stub
 from clarifai.data_upload.datasets.base import Chunker
 from clarifai.data_upload.datasets.image import (VisualClassificationDataset,
                                                  VisualDetectionDataset, VisualSegmentationDataset)
 from clarifai.data_upload.datasets.text import TextClassificationDataset
@@ -112,14 +115,16 @@
     self.dataset_id = dataset_id
     self.task = task
     self.module_dir = from_module
     self.zoo_dataset = from_zoo
     self.split = split
     self.chunk_size = min(128, chunk_size)  # limit max protos in a req
     self.num_workers: int = min(10, cpu_count())  #15 req/sec rate limit
+    self.annot_num_workers = 4
+    self.max_retires = 10
     self.__base: str = ""
     if portal == "dev":
       self.__base = "https://api-dev.clarifai.com"
     elif portal == "staging":
       self.__base = "https://api-staging.clarifai.com"
     else:  #prod
       self.__base = "https://api.clarifai.com"
@@ -130,144 +135,204 @@
     os.environ["CLARIFAI_API_BASE"] = self.__base
     os.environ["CLARIFAI_PAT"] = self.PAT
 
     self.STUB: service_pb2_grpc.V2Stub = create_stub()
     self.metadata: Tuple = (('authorization', 'Key ' + self.PAT),)
     self.user_app_id = resources_pb2.UserAppIDSet(user_id=self.USER_ID, app_id=self.APP_ID)
 
-  def _upload_inputs(self, batch_input: List[resources_pb2.Input]
-                    ) -> Union[List[resources_pb2.Input], List[None]]:
+  def _upload_inputs(self, batch_input: List[resources_pb2.Input]) -> str:
     """
     Upload inputs to clarifai platform dataset.
     Args:
       batch_input: input batch protos
     Returns:
-      retry_upload: failed input upload
+      input_job_id: Upload Input Job ID
     """
-    retry_upload = []  # those that fail to upload are stored for retries
+    input_job_id = uuid.uuid4().hex  # generate a unique id for this job
     response = self.STUB.PostInputs(
-        service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=batch_input),)
-
-    MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
+        service_pb2.PostInputsRequest(
+            user_app_id=self.user_app_id, inputs=batch_input, inputs_add_job_id=input_job_id),)
     if response.status.code != status_code_pb2.SUCCESS:
       try:
-        if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
-          retry_upload.extend(batch_input)
-        print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
+        print(f"Post inputs failed, status: {response.inputs[0].status.details}")
       except:
-        if "Duplicated inputs ID" not in response.status.details:
-          retry_upload.extend(batch_input)
-        print(f"Post inputs failed, status: {response.status.details}\n")
+        print(f"Post inputs failed, status: {response.status.details}")
 
-    return retry_upload
+    return input_job_id
 
-  def upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
-                        ) -> Union[List[resources_pb2.Annotation], List[None]]:
+  def _upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
+                         ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Upload image annotations to clarifai detection dataset
     Args:
       batch_annot: annot batch protos
     Returns:
       retry_upload: failed annot upload
     """
     retry_upload = []  # those that fail to upload are stored for retries
     response = self.STUB.PostAnnotations(
         service_pb2.PostAnnotationsRequest(user_app_id=self.user_app_id, annotations=batch_annot),)
 
     if response.status.code != status_code_pb2.SUCCESS:
       try:
-        print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
+        print(f"Post annotations failed, status: {response.annotations[0].status.details}")
       except:
-        print(f"Post annotations failed, status:\n{response.status.details}\n")
+        print(f"Post annotations failed, status: {response.status.details}")
       finally:
         retry_upload.extend(batch_annot)
 
     return retry_upload
 
-  def concurrent_inp_upload(
-      self,
-      inputs: List[List[resources_pb2.Input]],
-      chunks: int,
-      desc: str = "uploading inputs...") -> Union[List[resources_pb2.Input], List[None]]:
+  def _concurrent_annot_upload(self, annots: List[List[resources_pb2.Annotation]]
+                              ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
-    Upload images concurrently.
+    Uploads annotations concurrently.
     Args:
-      inputs: input protos
-      chunks: number of inputs chunks
+      annots: annot protos
     Returns:
-      retry_upload: All failed input protos during upload
+      retry_annot_upload: All failed annot protos during upload
     """
-    inp_threads = []
-    retry_upload = []
+    annot_threads = []
+    retry_annot_upload = []
 
-    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      with tqdm(total=chunks, desc=desc) as progress:
-        # Submit all jobs to the executor and store the returned futures
-        inp_threads = [executor.submit(self._upload_inputs, inp_batch) for inp_batch in inputs]
+    with ThreadPoolExecutor(max_workers=self.annot_num_workers) as executor:  # limit annot workers
+      annot_threads = [
+          executor.submit(self._upload_annotations, inp_batch) for inp_batch in annots
+      ]
+
+      for job in as_completed(annot_threads):
+        result = job.result()
+        if result:
+          retry_annot_upload.extend(result)
 
-        for job in as_completed(inp_threads):
-          result = job.result()
-          if result:
-            retry_upload.extend(result)
-          progress.update()
+    return retry_annot_upload
 
-    return retry_upload
+  def _backoff_iterator(self) -> None:
+    """
+    Return iterator for exponential backoff intervals.
+    """
+    yield 0.1
+    for i in range(5, 11):
+      yield 0.01 * (2**i)
+    while True:
+      yield 0.01 * (2**10)  #10 sec
 
-  def concurrent_annot_upload(
-      self,
-      annots: List[List[resources_pb2.Annotation]],
-      chunks: int,
-      desc: str = "uploading annotations...") -> Union[List[resources_pb2.Annotation], List[None]]:
+  def _wait_for_inputs(self, input_job_id: str) -> bool:
     """
-    Uploads annotations concurrently.
+    Wait for inputs to be processed. Cancel Job if timeout > 30 minutes.
     Args:
-      annots: annot protos
-      chunks: number of annots chunks
+      input_job_id: Upload Input Job ID
     Returns:
-      retry_annot_upload: All failed annot protos during upload
+      True if inputs are processed, False otherwise
     """
-    annot_threads = []
-    retry_annot_upload = []
+    backoff_iterator = self._backoff_iterator()
+    max_retries = self.max_retires
+    start_time = time.time()
+    while True:
+      response = self.STUB.GetInputsAddJob(
+          service_pb2.GetInputsAddJobRequest(user_app_id=self.user_app_id, id=input_job_id),)
+
+      if time.time() - start_time > 60 * 30 or max_retries == 0:  # 30 minutes timeout
+        self.STUB.CancelInputsAddJob(
+            service_pb2.CancelInputsAddJobRequest(user_app_id=self.user_app_id, id=input_job_id),
+        )  #Cancel Job
+        return False
+      if response.status.code != status_code_pb2.SUCCESS:
+        max_retries -= 1
+        print(f"Get input job failed, status: {response.status.details}\n")
+        continue
+      if response.inputs_add_job.progress.in_progress_count == 0 and response.inputs_add_job.progress.pending_count == 0:
+        return True
+      else:
+        time.sleep(next(backoff_iterator))
 
-    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      with tqdm(total=chunks, desc=desc) as progress:
-        # Submit all jobs to the executor and store the returned futures
-        annot_threads = [
-            executor.submit(self.upload_annotations, inp_batch) for inp_batch in annots
-        ]
+  def _delete_failed_inputs(self, input_ids: List[str]) -> Tuple[List[str], List[str]]:
+    """
+    Delete failed input ids from clarifai platform dataset.
+    Args:
+      input_ids: batch input ids
+    Returns:
+      success_inputs: upload success input ids
+      failed_inputs: upload failed input ids
+    """
+    success_status = status_pb2.Status(code=status_code_pb2.INPUT_DOWNLOAD_SUCCESS)
+    response = self.STUB.ListInputs(
+        service_pb2.ListInputsRequest(
+            ids=input_ids,
+            per_page=len(input_ids),
+            user_app_id=self.user_app_id,
+            status=success_status),)
+    response_dict = MessageToDict(response)
+    success_inputs = response_dict.get('inputs', [])
+
+    success_input_ids = [input.get('id') for input in success_inputs]
+    failed_input_ids = list(set(input_ids) - set(success_input_ids))
+    #delete failed inputs
+    self.STUB.DeleteInputs(
+        service_pb2.DeleteInputsRequest(user_app_id=self.user_app_id, ids=failed_input_ids),)
 
-        for job in as_completed(annot_threads):
-          result = job.result()
-          if result:
-            retry_annot_upload.extend(result)
-          progress.update()
+    return success_input_ids, failed_input_ids
 
-    return retry_annot_upload
+  def _upload_inputs_annotations(
+      self, batch_input_ids: List[str]) -> Tuple[List[str], List[resources_pb2.Annotation]]:
+    """
+    Uploads batch of inputs and annotations concurrently to clarifai platform dataset.
+    Args:
+      batch_input_ids: batch input ids
+    Returns:
+      failed_input_ids: failed input ids
+      retry_annot_protos: failed annot protos
+    """
+    input_protos, _ = self.dataset_obj.get_protos(batch_input_ids)
+    input_job_id = self._upload_inputs(input_protos)
+    retry_annot_protos = []
 
-  def retry_concurrent_uploads(
-      self,
-      retry_upload_protos: Union[List[resources_pb2.Input], List[resources_pb2.Annotation]],
-      upload_type: str = "input") -> None:
+    self._wait_for_inputs(input_job_id)
+    success_input_ids, failed_input_ids = self._delete_failed_inputs(batch_input_ids)
+
+    if self.task in ["visual_detection", "visual_segmentation"]:
+      _, annotation_protos = self.dataset_obj.get_protos(success_input_ids)
+      chunked_annotation_protos = Chunker(annotation_protos, self.chunk_size).chunk()
+      retry_annot_protos.extend(self._concurrent_annot_upload(chunked_annotation_protos))
+
+    return failed_input_ids, retry_annot_protos
+
+  def _retry_uploads(self, failed_input_ids: List[str],
+                     retry_annot_protos: List[resources_pb2.Annotation]) -> None:
+    """
+    Retry failed uploads.
+    Args:
+      failed_input_ids: failed input ids
+      retry_annot_protos: failed annot protos
+    """
+    if failed_input_ids:
+      self._upload_inputs_annotations(failed_input_ids)
+    if retry_annot_protos:
+      chunked_annotation_protos = Chunker(retry_annot_protos, self.chunk_size).chunk()
+      _ = self._concurrent_annot_upload(chunked_annotation_protos)
+
+  def _data_upload(self, input_ids: List[str]) -> None:
     """
-    Retry Uploads of inputs/annotations.
+    Uploads inputs and annotations to clarifai platform dataset.
     Args:
-      retry_upload_protos: upload protos for retry
-      upload_type: input/annot protos type
+      input_ids: input ids
     """
-    retry_chunked_upload_protos = Chunker(retry_upload_protos, self.chunk_size).chunk()
-    if len(retry_upload_protos) > 0 and upload_type == "input":
-      _ = self.concurrent_inp_upload(
-          retry_chunked_upload_protos,
-          len(retry_chunked_upload_protos),
-          desc="retry uploading failed input protos...")
-    elif len(retry_upload_protos) > 0 and upload_type == "annot":
-      _ = self.concurrent_annot_upload(
-          retry_chunked_upload_protos,
-          len(retry_chunked_upload_protos),
-          desc="retry uploading failed annotation protos...")
+    chunk_input_ids = Chunker(input_ids, self.chunk_size).chunk()
+    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
+      with tqdm(total=len(chunk_input_ids), desc='Uploading Dataset') as progress:
+        # Submit all jobs to the executor and store the returned futures
+        futures = [
+            executor.submit(self._upload_inputs_annotations, batch_input_ids)
+            for batch_input_ids in chunk_input_ids
+        ]
+
+        for job in as_completed(futures):
+          retry_input_proto, retry_annot_protos = job.result()
+          self._retry_uploads(retry_input_proto, retry_annot_protos)
+          progress.update()
 
   def upload_to_clarifai(self):
     """
     Execute data upload.
     """
     datagen_object = None
     if self.module_dir is None and self.zoo_dataset is None:
@@ -278,62 +343,21 @@
       but NOT both.")
     elif self.module_dir is not None:
       datagen_object = load_dataset(self.module_dir, self.split)
     else:
       datagen_object = load_zoo_dataset(self.zoo_dataset, self.split)
 
     if self.task == "text_clf":
-      dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
-      text_protos = dataset_obj._get_input_protos()
-      text_protos = dataset_obj._to_list(text_protos)
-
-      # Upload text
-      chunked_text_protos = Chunker(text_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_text_protos,
-                                                       len(chunked_text_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
+      self.dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
 
     elif self.task == "visual_detection":
-      dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
-      img_protos, annotation_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
-
-      # Upload annotations:
-      print("Uploading annotations.......")
-      annotation_protos = dataset_obj._to_list(annotation_protos)
-      chunked_annot_protos = Chunker(annotation_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_annot_upload(chunked_annot_protos,
-                                                         len(chunked_annot_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "annot")
+      self.dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)  # TODO: get_img_ids or get_input_ids
 
     elif self.task == "visual_segmentation":
-      dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
-      img_protos, mask_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-      mask_protos = dataset_obj._to_list(mask_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
-
-      # Upload masks:
-      print("Uploading masks.......")
-      chunked_mask_protos = Chunker(mask_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_annot_upload(chunked_mask_protos,
-                                                         len(chunked_mask_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "annot")
+      self.dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
 
     else:  # visual-classification & visual-captioning
-      dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
-      img_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
+      self.dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
```

### Comparing `clarifai-9.5.4/clarifai/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.0/clarifai/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/concepts.py` & `clarifai-9.6.0/clarifai/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/datasets.py` & `clarifai-9.6.0/clarifai/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/inputs.py` & `clarifai-9.6.0/clarifai/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/installed_module_versions.py` & `clarifai-9.6.0/clarifai/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/lister.py` & `clarifai-9.6.0/clarifai/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/models.py` & `clarifai-9.6.0/clarifai/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/module_versions.py` & `clarifai-9.6.0/clarifai/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/listing/modules.py` & `clarifai-9.6.0/clarifai/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/api.py` & `clarifai-9.6.0/clarifai/models/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Interface to Clarifai Models API."""
 
-from typing import Dict, List, Type
+from typing import Dict, Type
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Struct
 
 from clarifai.auth.helper import ClarifaiAuthHelper
 from clarifai.client import create_stub
@@ -96,92 +96,117 @@
 
     return {
         "Model Types": model_types,
         "Input Metadata": in_dims_dtype,
         "Output Metadata": out_dims_dtype
     }
 
-  def post_model(
+  def init_model(
       self,
       model_id: str,
-      model_zip_url: str,
       model_type: str,
-      input: List,
-      outputs: List,
       description: str = "",
   ):
-    """Post a new trained model to the Clarifai platform.
+    """Init a new model on Clarifai platform.
 
     Args:
         model_id (str): Clarifai model id
-        model_zip_url (str): url of zip of model
         model_type (str): Clarifai model type
-        input (List): list of a pair of clarifai input field and triton model input,
-            [clarifai_input_field, triton_input_filed]
-        outputs (List): list of pairs of clarifai output fields and triton model outputs,
-            [[clarifai_output_field1, triton_output_filed1],[clarifai_output_field2, triton_output_filed2],...]
         description (str, optional): a description of the model. Defaults to "".
 
     Returns:
         dict: Clarifai api response
     """
-
-    def _parse_fields_map(x):
-      """parse input, outputs to Struct"""
-      _fields_map = Struct()
-      if not isinstance(x[0], list):
-        x = [x]
-      for field, mapping in x:
-        _fields_map.update({field: mapping})
-      return _fields_map
-
-    input_fields_map = _parse_fields_map(input)
-    output_fields_map = _parse_fields_map(outputs)
     user_data_object = self.auth.get_user_app_id_proto()
     post_models_response = self.stub.PostModels(
         service_pb2.PostModelsRequest(
             user_app_id=user_data_object,
-            models=[
-                resources_pb2.Model(
-                    id=model_id,
-                    notes=description,
-                    model_type_id=model_type,
-                    model_version=resources_pb2.ModelVersion(
-                        pretrained_model_config=resources_pb2.PretrainedModelConfig(
-                            model_zip_url=model_zip_url,
-                            input_fields_map=input_fields_map,
-                            output_fields_map=output_fields_map)))
-            ]),
+            models=[resources_pb2.Model(id=model_id, notes=description,
+                                        model_type_id=model_type)]),
         metadata=self.auth.metadata)
 
     return MessageToDict(post_models_response, preserving_proto_field_name=True)
 
-  def post_model_version(self, model_id: str, model_zip_url: str):
+  def post_model_version(
+      self,
+      model_id: str,
+      model_zip_url: str,
+      input: dict,
+      outputs: dict,
+  ):
     """Post a new version of an existing model in the Clarifai platform.
 
     Args:
         model_id (str): Clarifai model id
         model_zip_url (str]): url of zip of model
+        model_zip_url (str): url of zip of model
+        input (dict): a dict where the key is clarifai input field and the value is triton model input,
+            {clarifai_input_field: triton_input_filed}.
+        outputs (dict): a dict where the keys are clarifai output fields and the values are triton model outputs,
+            {clarifai_output_field1: triton_output_filed1, clarifai_output_field2: triton_output_filed2,...}.
 
     Returns:
         dict: clarifai api response
     """
     user_data_object = self.auth.get_user_app_id_proto()
+
+    def _parse_fields_map(x):
+      """parse input, outputs to Struct"""
+      _fields_map = Struct()
+      _fields_map.update(x)
+      return _fields_map
+
+    input_fields_map = _parse_fields_map(input)
+    output_fields_map = _parse_fields_map(outputs)
     post_model_versions = self.stub.PostModelVersions(
         service_pb2.PostModelVersionsRequest(
             user_app_id=user_data_object,
             model_id=model_id,
             model_versions=[
-                resources_pb2.ModelVersion(pretrained_model_config=resources_pb2.
-                                           PretrainedModelConfig(model_zip_url=model_zip_url))
+                resources_pb2.ModelVersion(
+                    pretrained_model_config=resources_pb2.PretrainedModelConfig(
+                        model_zip_url=model_zip_url,
+                        input_fields_map=input_fields_map,
+                        output_fields_map=output_fields_map))
             ]),
         metadata=self.auth.metadata)
 
     return MessageToDict(post_model_versions, preserving_proto_field_name=True)
 
+  def upload_model(
+      self,
+      model_id: str,
+      model_zip_url: str,
+      input: dict,
+      outputs: dict,
+      model_type: str,
+      description: str = "",
+  ):
+    """Doing 2 requests for initializing and creating version for a new trained model to the Clarifai platform.
+
+    Args:
+        model_id (str): Clarifai model id
+        model_zip_url (str): url of zip of model
+        input (dict): a dict where the key is clarifai input field and the value is triton model input,
+            {clarifai_input_field: triton_input_filed}
+        outputs (dict): a dict where the keys are clarifai output fields and the values are triton model outputs,
+            {clarifai_output_field1: triton_output_filed1, clarifai_output_field2: triton_output_filed2,...}
+        model_type (str): Clarifai model type.
+        description (str, optional): a description of the model. Defaults to "".
+
+    Returns:
+        dict: Clarifai api response
+    """
+    init_resp = self.init_model(model_id, model_type, description)
+    if init_resp["status"]["code"] != "SUCCESS":
+      return init_resp
+    version_resp = self.post_model_version(model_id, model_zip_url, input, outputs)
+
+    return version_resp
+
   def delete_model(self, model_id: str):
     """Delete model api by model id
 
     Args:
         model_id (str): Clarifai model id
 
     Returns:
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/__init__.py` & `clarifai-9.6.0/clarifai/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/cli/__init__.py` & `clarifai-9.6.0/clarifai/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.0/clarifai/models/model_serving/cli/deploy_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,46 +15,65 @@
 
 from clarifai.auth.helper import ClarifaiAuthHelper
 from clarifai.models.api import Models
 from clarifai.models.model_serving.constants import MODEL_TYPES
 from clarifai.models.model_serving.model_config.deploy import ClarifaiFieldsMap
 
 
-def deploy(model_url, model_id: str = None, model_type: str = None, desc: str = ""):
+def deploy(model_url,
+           model_id: str = None,
+           model_type: str = None,
+           desc: str = "",
+           update_version: bool = False):
   # init Auth from env vars
   auth = ClarifaiAuthHelper.from_env()
+  # init api
+  model_api = Models(auth)
+
   # parsing model name/type.
   # if filename having this format: <model_id>_<model-type>
   # e.i yolov5s_coco_visual-dectector
   # else user has to input model_type and model_id
   zip_filename = model_url.split('/')[-1]
   zip_filename = zip_filename.split('.')[0]
 
   def _parse_name(name):
     *id_, type_ = name.split('_')
     return "_".join(id_), type_
 
+  # parse model_id
   if not model_id and "_" in zip_filename:
     model_id = _parse_name(zip_filename)[0]
+  assert model_id, "Can not parse model_id from url, please input it directly"
+  # parse model_type
   if not model_type and "_" in zip_filename:
     model_type = _parse_name(zip_filename)[-1]
-  assert model_id or model_type, "Can not parse model_type or model_id from url, please input them directly"
+  assert model_type, "Can not parse model_type from url, please input it directly"
   # key map
   assert model_type in MODEL_TYPES, f"model_type should be one of {MODEL_TYPES}"
   clarifai_key_map = ClarifaiFieldsMap(model_type=model_type)
-  # init api
-  model_api = Models(auth)
-  # post model
-  resp = model_api.post_model(
-      model_id=model_id,
-      model_zip_url=model_url,
-      model_type=model_type,
-      input=clarifai_key_map.input_fields_map,
-      outputs=clarifai_key_map.output_fields_map,
-      description=desc)
+  # if updating new version of existing model
+  if update_version:
+    resp = model_api.post_model_version(
+        model_id=model_id,
+        model_zip_url=model_url,
+        input=clarifai_key_map.input_fields_map,
+        outputs=clarifai_key_map.output_fields_map,
+    )
+  # creating new model
+  else:
+    # post model
+    resp = model_api.upload_model(
+        model_id=model_id,
+        model_zip_url=model_url,
+        model_type=model_type,
+        input=clarifai_key_map.input_fields_map,
+        outputs=clarifai_key_map.output_fields_map,
+        description=desc,
+    )
   # response
   if resp["status"]["code"] != "SUCCESS":
     raise Exception("Post models failed, details: {}, {}".format(resp["status"]["description"],
                                                                  resp["status"]["details"]))
   else:
     print("Success!")
 
@@ -66,16 +85,26 @@
   parser.add_argument("--model_id", type=str, required=False, default="", help="Custom model id.")
   parser.add_argument(
       "--model_type",
       type=str,
       required=False,
       choices=MODEL_TYPES,
       default="",
-      help="Short description of model")
+      help="Clarifai model type")
   parser.add_argument(
       "--desc", type=str, required=False, default="", help="Short desccription of model")
+  parser.add_argument(
+      "--update_version",
+      action="store_true",
+      required=False,
+      help="Update exist model with new version")
   args = parser.parse_args()
-  deploy(model_url=args.url, model_id=args.model_id, desc=args.desc, model_type=args.model_type)
+  deploy(
+      model_url=args.url,
+      model_id=args.model_id,
+      desc=args.desc,
+      model_type=args.model_type,
+      update_version=args.update_version)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/cli/model_zip.py` & `clarifai-9.6.0/clarifai/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/cli/repository.py` & `clarifai-9.6.0/clarifai/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.0/clarifai/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.0/clarifai/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.0/clarifai/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/model_config/__init__.py` & `clarifai-9.6.0/clarifai/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/model_config/deploy.py` & `clarifai-9.6.0/clarifai/models/model_serving/model_config/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,17 +33,19 @@
   output_fields_map: List = field(default_factory=list)
 
   def __post_init__(self):
     """
     Set mapping of clarifai in/output vs triton in/output
     """
     if self.model_type == "visual-detector":
-      self.input_fields_map = ["image", "image"]
-      self.output_fields_map = [["regions[...].region_info.bounding_box", "predicted_bboxes"],
-                                ["regions[...].data.concepts[...].id", "predicted_labels"],
-                                ["regions[...].data.concepts[...].value", "predicted_scores"]]
+      self.input_fields_map = {"image": "image"}
+      self.output_fields_map = {
+          "regions[...].region_info.bounding_box": "predicted_bboxes",
+          "regions[...].data.concepts[...].id": "predicted_labels",
+          "regions[...].data.concepts[...].value": "predicted_scores"
+      }
     elif self.model_type == "visual-classifier":
-      self.input_fields_map = ["image", "image"]
-      self.output_fields_map = ["concepts", "softmax_predictions"]
+      self.input_fields_map = {"image": "image"}
+      self.output_fields_map = {"concepts": "softmax_predictions"}
     elif self.model_type == "text-classifier":
-      self.input_fields_map = ["text", "text"]
-      self.output_fields_map = ["concepts", "softmax_predictions"]
+      self.input_fields_map = {"text": "text"}
+      self.output_fields_map = {"concepts": "softmax_predictions"}
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/model_config/serializer.py` & `clarifai-9.6.0/clarifai/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/model_config/triton_config.py` & `clarifai-9.6.0/clarifai/models/model_serving/model_config/triton_config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/models/__init__.py` & `clarifai-9.6.0/clarifai/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/models/inference.py` & `clarifai-9.6.0/clarifai/models/model_serving/models/inference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 # This file contains boilerplate code to allow users write their model
 # inference code that will then interact with the Triton Inference Server
 # Python backend to serve end user requests.
-# The module name, module path and the setup() & predict() function names MUST be maintained as is
-# but other functions may be added within this module as deemed fit provided
-# they are invoked within the main predict() function if they play a role any
-# step of model inference
+# The module name, module path, class name & get_predictions() method names MUST be maintained as is
+# but other methods may be added within the class as deemed fit provided
+# they are invoked within the main get_predictions() inference method
+# if they play a role in any step of model inference
 """User model inference script."""
 
 import os
-from typing import Callable
+from pathlib import Path
 
-BASE_PATH = os.path.dirname(__file__)
 
+class InferenceModel:
+  """User model inference class."""
 
-def setup():
-  """
-  Load inference model.
-  The model checkpoint(s) should be saved in the same directory and directory
-  level as this inference.py module.
-
-  Returns:
-  --------
-    Inference Model Callable
-  """
-  # sample model loading code:
-  # checkpoint_path = os.path.join(BASE_PATH, your_checkpoint_name)
-  # model = <load model from checkpoint_path>
-  # return model
-
-  # Delete/Comment out line below and add your code
-  raise NotImplementedError()
-
-
-def predict(input_data, model: Callable):
-  """
-  Main model inference function.
-
-  Args:
-  -----
-    input_data: A single input data item to predict on.
-      Input data can be an image or text, etc depending on the model type.
-    model: Inference model callable as returned by setup() above.
-
-  Returns:
-  --------
-    One of the clarifai.model_serving.models.output types. Refer to the README/docs
-  """
-  # Delete/Comment out line below and add your inference code
-  raise NotImplementedError()
+  def __init__(self) -> None:
+    """
+    Load inference time artifacts that are called frequently .e.g. models, tokenizers, etc.
+    in this method so they are loaded only once for faster inference.
+    """
+    self.base_path: Path = os.path.dirname(__file__)
+    ## sample model loading code:
+    #self.checkpoint_path: Path = os.path.join(self.base_path, "your checkpoint filename/path")
+    #self.model: Callable = <load_your_model_here from checkpoint or folder>
+
+  #Add relevant model type decorator to the method below (see docs/model_types for ref.)
+  def get_predictions(self, input_data):
+    """
+    Main model inference method.
+
+    Args:
+    -----
+      input_data: A single input data item to predict on.
+        Input data can be an image or text, etc depending on the model type.
+
+    Returns:
+    --------
+      One of the clarifai.models.model_serving.models.output types. Refer to the README/docs
+    """
+    # Delete/Comment out line below and add your inference code
+    raise NotImplementedError()
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/models/model_types.py` & `clarifai-9.6.0/clarifai/models/model_serving/models/model_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # limitations under the License.
 """
 Parse inference model predictions to triton inference responses
 per model type.
 """
 
 from functools import wraps
-from typing import Callable, List
+from typing import Callable
 
 import numpy as np
 
 try:
   import triton_python_backend_utils as pb_utils
 except ModuleNotFoundError:
   pass
@@ -28,23 +28,23 @@
 
 def visual_detector(func: Callable):
   """
   Visual detector type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_bboxes = []
     out_labels = []
     out_scores = []
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_bboxes.append(preds.predicted_bboxes)
       out_labels.append(preds.predicted_labels)
       out_scores.append(preds.predicted_scores)
 
     if len(out_bboxes) < 1 or len(out_labels) < 1:
       out_tensor_bboxes = pb_utils.Tensor("predicted_bboxes", np.zeros((0, 4), dtype=np.float32))
       out_tensor_labels = pb_utils.Tensor("predicted_labels", np.zeros((0, 1), dtype=np.int32))
@@ -67,21 +67,21 @@
 
 def visual_classifier(func: Callable):
   """
   Visual classifier type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_scores = []
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_scores.append(preds.predicted_scores)
 
     out_tensor_scores = pb_utils.Tensor("softmax_predictions",
                                         np.asarray(out_scores, dtype=np.float32))
     inference_response = pb_utils.InferenceResponse(output_tensors=[out_tensor_scores])
 
     return inference_response
@@ -91,22 +91,22 @@
 
 def text_classifier(func: Callable):
   """
   Text classifier type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_scores = []
     input_data = [in_elem[0].decode() for in_elem in input_data]
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_scores.append(preds.predicted_scores)
 
     out_tensor_scores = pb_utils.Tensor("softmax_predictions",
                                         np.asarray(out_scores, dtype=np.float32))
     inference_response = pb_utils.InferenceResponse(output_tensors=[out_tensor_scores])
 
     return inference_response
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/models/output.py` & `clarifai-9.6.0/clarifai/models/model_serving/models/output.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/models/pb_model.py` & `clarifai-9.6.0/clarifai/models/model_serving/models/pb_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai/models/model_serving/pb_model_repository.py` & `clarifai-9.6.0/clarifai/models/model_serving/pb_model_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if hasattr(out_field, "label_filename"):
           with open(os.path.join(repository_path, "labels.txt"), "w"):
             pass
         else:
           continue
       # gen requirements & conda yaml
       with open(os.path.join(repository_path, "requirements.txt"), "w") as f:
-        f.write("clarifai\ntritonclient==2.34.0")  # for model upload utils
+        f.write("clarifai>9.5.3\ntritonclient[all]")  # for model upload utils
       with open(os.path.join(repository_path, "triton_conda.yaml"), "w") as conda_env:
         conda_env.write("name: triton_conda-cp3.8-torch1.13.1-19f97078")
 
     if not os.path.isdir(model_version_path):
       os.mkdir(model_version_path)
     if not os.path.exists(os.path.join(model_version_path, "__init__.py")):
       with open(os.path.join(model_version_path, "__init__.py"), "w"):
```

### Comparing `clarifai-9.5.4/clarifai/modules/css.py` & `clarifai-9.6.0/clarifai/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/modules/pages.py` & `clarifai-9.6.0/clarifai/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/modules/style.css` & `clarifai-9.6.0/clarifai/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai/urls/helper.py` & `clarifai-9.6.0/clarifai/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai.egg-info/PKG-INFO` & `clarifai-9.6.0/clarifai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clarifai
-Version: 9.5.4
+Version: 9.6.0
 Summary: Clarifai Python Utilities
 Home-page: https://github.com/Clarifai/clarifai-python-utils
 Author: Clarifai
 Author-email: support@clarifai.com
 License: Apache 2.0
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Programming Language :: Python :: 3
```

### Comparing `clarifai-9.5.4/clarifai_utils/auth/helper.py` & `clarifai-9.6.0/clarifai_utils/auth/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/client/abc.py` & `clarifai-9.6.0/clarifai_utils/client/abc.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/client/stub.py` & `clarifai-9.6.0/clarifai_utils/client/stub.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/convert_csv.py` & `clarifai-9.6.0/clarifai_utils/data_upload/convert_csv.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/features.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/features.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/image.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/image.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import os
-from typing import Iterator, List, Tuple, Union
+from typing import Iterator, List, Union
 
 from clarifai_grpc.grpc.api import resources_pb2
 from google.protobuf.struct_pb2 import Struct
 from tqdm import tqdm
 
 from .base import ClarifaiDataset
 
 
 class VisualClassificationDataset(ClarifaiDataset):
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, labels: List[Union[str, int]], input_id: str,
                           dataset_id: str, geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -42,43 +43,40 @@
                   id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)\
                 for _label in labels
             ],
             metadata=metadata))
 
     return input_proto
 
-  def _get_input_protos(self) -> Iterator:
+  def _extract_protos(self) -> None:
     """
     Create input image protos for each data generator item.
-    Returns:
-      Input proto iterator
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image_path = item.image_path
       label = item.label if isinstance(item.label, list) else [item.label]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       geo_info = item.geo_info
       metadata.update({"filename": os.path.basename(image_path), "split": self.split})
 
+      self.input_ids.append(input_id)
       input_proto = self.create_input_protos(image_path, label, input_id, self.dataset_id,
                                              geo_info, metadata)
-      self._all_input_protos.append(input_proto)
-
-    return iter(self._all_input_protos)
+      self._all_input_protos[input_id] = input_proto
 
 
 class VisualDetectionDataset(ClarifaiDataset):
   """
   Visual detection dataset proto class.
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
-    self._annotation_protos = []
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
                           geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -131,51 +129,48 @@
                     resources_pb2.Concept(
                         id=f"id-{''.join(label.split(' '))}", name=label, value=1.)
                 ]))
         ]))
 
     return input_annot_proto
 
-  def _get_input_protos(self) -> Tuple[Iterator, Iterator]:
+  def _extract_protos(self) -> None:
     """
     Create input image protos for each data generator item.
-    Returns:
-      Input and Annotation proto iterators.
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path
       labels = item.classes  # list:[l1,...,ln]
       bboxes = item.bboxes  # [[xmin,ymin,xmax,ymax],...,[xmin,ymin,xmax,ymax]]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
+      self.input_ids.append(input_id)
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
-      self._all_input_protos.append(input_image_proto)
+      self._all_input_protos[input_id] = input_image_proto
 
       # iter over bboxes and classes
       # one id could have more than one bbox and label
       for i in range(len(bboxes)):
         input_annot_proto = self.create_annotation_proto(labels[i], bboxes[i], input_id,
                                                          self.dataset_id)
-        self._annotation_protos.append(input_annot_proto)
-
-    return iter(self._all_input_protos), iter(self._annotation_protos)
+        self._all_annotation_protos[input_id].append(input_annot_proto)
 
 
 class VisualSegmentationDataset(ClarifaiDataset):
   """
   Visual segmentation dataset proto class.
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
-    self._mask_protos = []  # mask or polygon protos
+    self._extract_protos()
 
   def create_input_protos(self, image_path: str, input_id: str, dataset_id: str,
                           geo_info: Union[List[float], None],
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each image, label input pair.
     Args:
@@ -226,36 +221,33 @@
                     resources_pb2.Concept(
                         id=f"id-{''.join(label.split(' '))}", name=label, value=1.)
                 ]))
         ]))
 
     return input_mask_proto
 
-  def _get_input_protos(self) -> Tuple[Iterator, Iterator]:
+  def _extract_protos(self) -> None:
     """
     Create input image and annotation protos for each data generator item.
-    Returns:
-      Input and Annotation proto iterators.
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Creating input protos..."):
       metadata = Struct()
       image = item.image_path  # image path
       labels = item.classes  # list of class labels
       _polygons = item.polygons  # list of polygons: [[[x,y],...,[x,y]],...]
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"filename": os.path.basename(image), "split": self.split})
       geo_info = item.geo_info
 
+      self.input_ids.append(input_id)
       input_image_proto = self.create_input_protos(image, input_id, self.dataset_id, geo_info,
                                                    metadata)
-      self._all_input_protos.append(input_image_proto)
+      self._all_input_protos[input_id] = input_image_proto
 
       ## Iterate over each masked image and create a proto for upload to clarifai
       ## The length of masks/polygons-list and labels must be equal
       for i, _polygon in enumerate(_polygons):
         try:
           input_mask_proto = self.create_mask_proto(labels[i], _polygon, input_id, self.dataset_id)
-          self._mask_protos.append(input_mask_proto)
+          self._all_annotation_protos[input_id].append(input_mask_proto)
         except IndexError:
           continue
-
-    return iter(self._all_input_protos), iter(self._mask_protos)
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/text.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/text.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class TextClassificationDataset(ClarifaiDataset):
   """
   Upload text classification datasets to clarifai datasets
   """
 
   def __init__(self, datagen_object: Iterator, dataset_id: str, split: str) -> None:
     super().__init__(datagen_object, dataset_id, split)
+    self._extract_protos()
 
   def create_input_protos(self, text_input: str, labels: List[str], input_id: str, dataset_id: str,
                           metadata: Struct) -> resources_pb2.Input:
     """
     Create input protos for each text, label input pairs.
     Args:
     	`text_input`: text string.
@@ -38,25 +39,22 @@
                     id=f"id-{''.join(_label.split(' '))}", name=_label, value=1.)
                 for _label in labels
             ],
             metadata=metadata))
 
     return input_proto
 
-  def _get_input_protos(self) -> Iterator:
+  def _extract_protos(self) -> None:
     """
     Creates input protos for each data generator item.
-    Returns:
-    	A list of input protos
     """
     for i, item in tqdm(enumerate(self.datagen_object), desc="Loading text data"):
       metadata = Struct()
       text = item.text
       labels = item.labels if isinstance(item.labels, list) else [item.labels]  # clarifai concept
       input_id = f"{self.dataset_id}-{self.split}-{i}" if item.id is None else f"{self.split}-{str(item.id)}"
       metadata.update({"split": self.split})
 
+      self.input_ids.append(input_id)
       input_proto = self.create_input_protos(text, labels, input_id, self.dataset_id, metadata)
 
-      self._all_input_protos.append(input_proto)
-
-    return iter(self._all_input_protos)
+      self._all_input_protos[input_id] = input_proto
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_captions.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_captions.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,38 +14,39 @@
 class COCOCaptionsDataset:
   """COCO 2017 Image Captioning Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory.
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train, val and annotation dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("Dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -70,30 +71,30 @@
   def dataloader(self):
     """
     Transform coco image captioning data into clarifai proto compatible
     format for upload.
     Returns:
       VisualClassificationFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:  #train, val, annotations
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:  #train, val, annotations
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 3 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 3 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" + f"captions_{self.split}*")[0]
     coco = COCO(annot_file)
     annot_ids = coco.getAnnIds()
     annotations = coco.loadAnns(annot_ids)
     for annot in annotations:
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(annot['image_id']).zfill(12)}*")[0]
       # image_captioning and image classification datasets have the same
       # image-label input feature formats
-      yield VisualClassificationFeatures(image_path, annot["caption"], annot["image_id"])
+      yield VisualClassificationFeatures(image_path, annot["caption"], id=annot["image_id"])
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_detection.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_detection.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,39 @@
 class COCODetectionDataset:
   """COCO 2017 Image Detection Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory.
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train*, val* and annotation* dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -71,25 +72,25 @@
   def dataloader(self):
     """
     Transform coco object detection data into clarifai proto compatible
     format for upload.
     Returns:
       VisualDetectionFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 2 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 2 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" +\
      f"instances_{self.split}*")[0]
     coco = COCO(annot_file)
     categories = coco.loadCats(coco.getCatIds())
     cat_id_map = {category["id"]: category["name"] for category in categories}
@@ -98,15 +99,15 @@
       cat_img_ids[cat_id] = coco.getImgIds(catIds=[cat_id])
 
     img_ids = []
     for i in list(cat_img_ids.values()):
       img_ids.extend(i)
 
     #get annotations for each image id
-    for _id in img_ids:
+    for _id in set(img_ids):
       annots = []  # bboxes
       class_names = []
       labels = [i for i in list(filter(lambda x: _id in cat_img_ids[x], cat_img_ids))]
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(_id).zfill(12)}*")[0]
 
       image_height, image_width = cv2.imread(image_path).shape[:2]
@@ -122,8 +123,8 @@
             y_max = (ann['bbox'][1] + ann['bbox'][3]) / image_height  #bottom_row
             annots.append([x_min, y_min, x_max, y_max])
         else:  # if no annotations for given image_id-cat_id pair
           continue
       assert len(class_names) == len(annots), f"Num classes must match num bbox annotations\
       for a single image. Found {len(class_names)} classes and {len(annots)} bboxes."
 
-      yield VisualDetectionFeatures(image_path, class_names, annots, _id)
+      yield VisualDetectionFeatures(image_path, class_names, annots, id=_id)
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/coco_segmentation.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,38 +19,39 @@
 class COCOSegmentationDataset:
   """COCO 2017 Image Segmentation Dataset."""
 
   def __init__(self, split: str = "train"):
     """
     Initialize coco dataset.
     Args:
-      filenames: the coco zip filenames: List[str] to be downloaded if download=True,
+      filenames: the coco zip filenames: Dict[str, str] to be downloaded if download=True,
       data_dir: the local coco dataset directory
       split: "train" or "val"
     """
     self.filenames = {
         "train": "train2017.zip",
         "val": "val2017.zip",
         "annotations": "annotations_trainval2017.zip"
     }
     self.split = split
     self.url = "http://images.cocodataset.org/zips/"  # coco base image-zip url
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage dir
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage dir
     self.extracted_coco_dirs = {"train": None, "val": None, "annotations": None}
 
   def coco_download(self, save_dir):
     """Download coco dataset."""
     if not os.path.exists(save_dir):
       os.mkdir(save_dir)
 
     #check if train, val and annotation dirs exist
     #so that the coco2017 data isn't downloaded
     for key, filename in self.filenames.items():
-      if os.path.exists(glob(f"{save_dir}/{key}*")[0]):
-        print("dataset already downloded and extracted")
+      existing_files = glob(f"{save_dir}/{key}*")
+      if existing_files:
+        print(f"{key} dataset already downloded and extracted")
         continue
 
       print("-" * 80)
       print(f"Downloading {filename}")
       print("-" * 80)
 
       if "annotations" in filename:
@@ -74,25 +75,25 @@
 
   def dataloader(self):
     """
     Transform coco data into clarifai proto compatible format for upload.
     Returns:
       VisualSegmentationFeatures type generator.
     """
-    if isinstance(self.filenames, list) and len(self.filenames) == 3:
+    if isinstance(self.filenames, dict) and len(self.filenames) == 3:
       self.coco_download(self.data_dir)
       self.extracted_coco_dirs["train"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "train" in i][0]
       self.extracted_coco_dirs["val"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "val" in i][0]
 
       self.extracted_coco_dirs["annotations"] = [os.path.join(self.data_dir, i) \
       for i in os.listdir(self.data_dir) if "annotations" in i][0]
     else:
-      raise Exception(f"`filenames` must be a list of atleast 3 coco zip file names; \
+      raise Exception(f"`filenames` must be a dict of atleast 3 coco zip file names; \
       train, val and annotations. Found {len(self.filenames)} items instead.")
 
     annot_file = glob(self.extracted_coco_dirs["annotations"] + "/" +\
      f"instances_{self.split}*")[0]
     coco = COCO(annot_file)
     categories = coco.loadCats(coco.getCatIds())
     cat_id_map = {category["id"]: category["name"] for category in categories}
@@ -101,34 +102,34 @@
       cat_img_ids[cat_id] = coco.getImgIds(catIds=[cat_id])
 
     img_ids = []
     for i in list(cat_img_ids.values()):
       img_ids.extend(i)
 
     #get annotations for each image id
-    for _id in img_ids:
+    for _id in set(img_ids):
       annots = []  # polygons
       class_names = []
       labels = [i for i in list(filter(lambda x: _id in cat_img_ids[x], cat_img_ids))]
       image_path = glob(self.extracted_coco_dirs[self.split]+"/"+\
       f"{str(_id).zfill(12)}*")[0]
 
       image_height, image_width = cv2.imread(image_path).shape[:2]
       for cat_id in labels:
         annot_ids = coco.getAnnIds(imgIds=_id, catIds=[cat_id])
         if len(annot_ids) > 0:
           img_annotations = coco.loadAnns(annot_ids)
           for ann in img_annotations:
-            class_names.append(cat_id_map[cat_id])
             # get polygons
             if type(ann['segmentation']) == list:
               for seg in ann['segmentation']:
                 poly = np.array(seg).reshape((int(len(seg) / 2), 2))
                 poly[:, 0], poly[:, 1] = poly[:, 0] / image_width, poly[:, 1] / image_height
                 annots.append(poly.tolist())  #[[x=col, y=row],...]
+                class_names.append(cat_id_map[cat_id])
             else:  # seg: {"counts":[...]}
               if type(ann['segmentation']['counts']) == list:
                 rle = maskUtils.frPyObjects([ann['segmentation']], image_height, image_width)
               else:
                 rle = ann['segmentation']
               mask = maskUtils.decode(rle)  #binary mask
               #convert mask to polygons and add to annots
@@ -146,13 +147,14 @@
 
               polygons = np.array(polygons_flattened).reshape((int(len(polygons_flattened) / 2),
                                                                2))
               polygons[:, 0] = polygons[:, 0] / image_width
               polygons[:, 1] = polygons[:, 1] / image_height
 
               annots.append(polygons.tolist())  #[[x=col, y=row],...,[x=col, y=row]]
+              class_names.append(cat_id_map[cat_id])
         else:  # if no annotations for given image_id-cat_id pair
           continue
       assert len(class_names) == len(annots), f"Num classes must match num annotations\
       for a single image. Found {len(class_names)} classes and {len(annots)} polygons."
 
-      yield VisualSegmentationFeatures(image_path, class_names, annots, _id)
+      yield VisualSegmentationFeatures(image_path, class_names, annots, id=_id)
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/imagenet_classification.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Initialize dataset params.
     Args:
       data_dir: the local dataset directory.
       split: "train" or "test"
     """
     self.split = split
-    self.data_dir = os.path.join(os.curdir, ".data")  # data storage directory
+    self.data_dir = os.path.join(os.curdir, "data")  # data storage directory
     self.label_map = dict()
 
   def dataloader(self):
     """
     Transform text data into clarifai proto compatible
     format for upload.
     Returns:
```

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/datasets/zoo/xview_detection.py` & `clarifai-9.6.0/clarifai_utils/data_upload/datasets/zoo/xview_detection.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py` & `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/cifar10/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py` & `clarifai-9.6.0/clarifai_utils/data_upload/examples/image_classification/food-101/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py` & `clarifai-9.6.0/clarifai_utils/data_upload/examples/text_classification/imdb_dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/examples.py` & `clarifai-9.6.0/clarifai_utils/data_upload/examples.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/data_upload/upload.py` & `clarifai-9.6.0/clarifai_utils/data_upload/upload.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 #! Clarifai data upload
 
 import importlib
 import inspect
 import os
 import sys
+import time
+import uuid
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from multiprocessing import cpu_count
 from typing import Iterator, List, Optional, Tuple, Union
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2, service_pb2_grpc
-from clarifai_grpc.grpc.api.status import status_code_pb2
+from clarifai_grpc.grpc.api.status import status_code_pb2, status_pb2
+from google.protobuf.json_format import MessageToDict
 from tqdm import tqdm
 
 from clarifai.client import create_stub
 from clarifai.data_upload.datasets.base import Chunker
 from clarifai.data_upload.datasets.image import (VisualClassificationDataset,
                                                  VisualDetectionDataset, VisualSegmentationDataset)
 from clarifai.data_upload.datasets.text import TextClassificationDataset
@@ -112,14 +115,16 @@
     self.dataset_id = dataset_id
     self.task = task
     self.module_dir = from_module
     self.zoo_dataset = from_zoo
     self.split = split
     self.chunk_size = min(128, chunk_size)  # limit max protos in a req
     self.num_workers: int = min(10, cpu_count())  #15 req/sec rate limit
+    self.annot_num_workers = 4
+    self.max_retires = 10
     self.__base: str = ""
     if portal == "dev":
       self.__base = "https://api-dev.clarifai.com"
     elif portal == "staging":
       self.__base = "https://api-staging.clarifai.com"
     else:  #prod
       self.__base = "https://api.clarifai.com"
@@ -130,144 +135,204 @@
     os.environ["CLARIFAI_API_BASE"] = self.__base
     os.environ["CLARIFAI_PAT"] = self.PAT
 
     self.STUB: service_pb2_grpc.V2Stub = create_stub()
     self.metadata: Tuple = (('authorization', 'Key ' + self.PAT),)
     self.user_app_id = resources_pb2.UserAppIDSet(user_id=self.USER_ID, app_id=self.APP_ID)
 
-  def _upload_inputs(self, batch_input: List[resources_pb2.Input]
-                    ) -> Union[List[resources_pb2.Input], List[None]]:
+  def _upload_inputs(self, batch_input: List[resources_pb2.Input]) -> str:
     """
     Upload inputs to clarifai platform dataset.
     Args:
       batch_input: input batch protos
     Returns:
-      retry_upload: failed input upload
+      input_job_id: Upload Input Job ID
     """
-    retry_upload = []  # those that fail to upload are stored for retries
+    input_job_id = uuid.uuid4().hex  # generate a unique id for this job
     response = self.STUB.PostInputs(
-        service_pb2.PostInputsRequest(user_app_id=self.user_app_id, inputs=batch_input),)
-
-    MESSAGE_DUPLICATE_ID = "Input has a duplicate ID."
+        service_pb2.PostInputsRequest(
+            user_app_id=self.user_app_id, inputs=batch_input, inputs_add_job_id=input_job_id),)
     if response.status.code != status_code_pb2.SUCCESS:
       try:
-        if response.inputs[0].status.details != MESSAGE_DUPLICATE_ID:
-          retry_upload.extend(batch_input)
-        print(f"Post inputs failed, status: {response.inputs[0].status.details}\n")
+        print(f"Post inputs failed, status: {response.inputs[0].status.details}")
       except:
-        if "Duplicated inputs ID" not in response.status.details:
-          retry_upload.extend(batch_input)
-        print(f"Post inputs failed, status: {response.status.details}\n")
+        print(f"Post inputs failed, status: {response.status.details}")
 
-    return retry_upload
+    return input_job_id
 
-  def upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
-                        ) -> Union[List[resources_pb2.Annotation], List[None]]:
+  def _upload_annotations(self, batch_annot: List[resources_pb2.Annotation]
+                         ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
     Upload image annotations to clarifai detection dataset
     Args:
       batch_annot: annot batch protos
     Returns:
       retry_upload: failed annot upload
     """
     retry_upload = []  # those that fail to upload are stored for retries
     response = self.STUB.PostAnnotations(
         service_pb2.PostAnnotationsRequest(user_app_id=self.user_app_id, annotations=batch_annot),)
 
     if response.status.code != status_code_pb2.SUCCESS:
       try:
-        print(f"Post annotations failed, status:\n{response.annotations[0].status.details}\n")
+        print(f"Post annotations failed, status: {response.annotations[0].status.details}")
       except:
-        print(f"Post annotations failed, status:\n{response.status.details}\n")
+        print(f"Post annotations failed, status: {response.status.details}")
       finally:
         retry_upload.extend(batch_annot)
 
     return retry_upload
 
-  def concurrent_inp_upload(
-      self,
-      inputs: List[List[resources_pb2.Input]],
-      chunks: int,
-      desc: str = "uploading inputs...") -> Union[List[resources_pb2.Input], List[None]]:
+  def _concurrent_annot_upload(self, annots: List[List[resources_pb2.Annotation]]
+                              ) -> Union[List[resources_pb2.Annotation], List[None]]:
     """
-    Upload images concurrently.
+    Uploads annotations concurrently.
     Args:
-      inputs: input protos
-      chunks: number of inputs chunks
+      annots: annot protos
     Returns:
-      retry_upload: All failed input protos during upload
+      retry_annot_upload: All failed annot protos during upload
     """
-    inp_threads = []
-    retry_upload = []
+    annot_threads = []
+    retry_annot_upload = []
 
-    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      with tqdm(total=chunks, desc=desc) as progress:
-        # Submit all jobs to the executor and store the returned futures
-        inp_threads = [executor.submit(self._upload_inputs, inp_batch) for inp_batch in inputs]
+    with ThreadPoolExecutor(max_workers=self.annot_num_workers) as executor:  # limit annot workers
+      annot_threads = [
+          executor.submit(self._upload_annotations, inp_batch) for inp_batch in annots
+      ]
+
+      for job in as_completed(annot_threads):
+        result = job.result()
+        if result:
+          retry_annot_upload.extend(result)
 
-        for job in as_completed(inp_threads):
-          result = job.result()
-          if result:
-            retry_upload.extend(result)
-          progress.update()
+    return retry_annot_upload
 
-    return retry_upload
+  def _backoff_iterator(self) -> None:
+    """
+    Return iterator for exponential backoff intervals.
+    """
+    yield 0.1
+    for i in range(5, 11):
+      yield 0.01 * (2**i)
+    while True:
+      yield 0.01 * (2**10)  #10 sec
 
-  def concurrent_annot_upload(
-      self,
-      annots: List[List[resources_pb2.Annotation]],
-      chunks: int,
-      desc: str = "uploading annotations...") -> Union[List[resources_pb2.Annotation], List[None]]:
+  def _wait_for_inputs(self, input_job_id: str) -> bool:
     """
-    Uploads annotations concurrently.
+    Wait for inputs to be processed. Cancel Job if timeout > 30 minutes.
     Args:
-      annots: annot protos
-      chunks: number of annots chunks
+      input_job_id: Upload Input Job ID
     Returns:
-      retry_annot_upload: All failed annot protos during upload
+      True if inputs are processed, False otherwise
     """
-    annot_threads = []
-    retry_annot_upload = []
+    backoff_iterator = self._backoff_iterator()
+    max_retries = self.max_retires
+    start_time = time.time()
+    while True:
+      response = self.STUB.GetInputsAddJob(
+          service_pb2.GetInputsAddJobRequest(user_app_id=self.user_app_id, id=input_job_id),)
+
+      if time.time() - start_time > 60 * 30 or max_retries == 0:  # 30 minutes timeout
+        self.STUB.CancelInputsAddJob(
+            service_pb2.CancelInputsAddJobRequest(user_app_id=self.user_app_id, id=input_job_id),
+        )  #Cancel Job
+        return False
+      if response.status.code != status_code_pb2.SUCCESS:
+        max_retries -= 1
+        print(f"Get input job failed, status: {response.status.details}\n")
+        continue
+      if response.inputs_add_job.progress.in_progress_count == 0 and response.inputs_add_job.progress.pending_count == 0:
+        return True
+      else:
+        time.sleep(next(backoff_iterator))
 
-    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
-      with tqdm(total=chunks, desc=desc) as progress:
-        # Submit all jobs to the executor and store the returned futures
-        annot_threads = [
-            executor.submit(self.upload_annotations, inp_batch) for inp_batch in annots
-        ]
+  def _delete_failed_inputs(self, input_ids: List[str]) -> Tuple[List[str], List[str]]:
+    """
+    Delete failed input ids from clarifai platform dataset.
+    Args:
+      input_ids: batch input ids
+    Returns:
+      success_inputs: upload success input ids
+      failed_inputs: upload failed input ids
+    """
+    success_status = status_pb2.Status(code=status_code_pb2.INPUT_DOWNLOAD_SUCCESS)
+    response = self.STUB.ListInputs(
+        service_pb2.ListInputsRequest(
+            ids=input_ids,
+            per_page=len(input_ids),
+            user_app_id=self.user_app_id,
+            status=success_status),)
+    response_dict = MessageToDict(response)
+    success_inputs = response_dict.get('inputs', [])
+
+    success_input_ids = [input.get('id') for input in success_inputs]
+    failed_input_ids = list(set(input_ids) - set(success_input_ids))
+    #delete failed inputs
+    self.STUB.DeleteInputs(
+        service_pb2.DeleteInputsRequest(user_app_id=self.user_app_id, ids=failed_input_ids),)
 
-        for job in as_completed(annot_threads):
-          result = job.result()
-          if result:
-            retry_annot_upload.extend(result)
-          progress.update()
+    return success_input_ids, failed_input_ids
 
-    return retry_annot_upload
+  def _upload_inputs_annotations(
+      self, batch_input_ids: List[str]) -> Tuple[List[str], List[resources_pb2.Annotation]]:
+    """
+    Uploads batch of inputs and annotations concurrently to clarifai platform dataset.
+    Args:
+      batch_input_ids: batch input ids
+    Returns:
+      failed_input_ids: failed input ids
+      retry_annot_protos: failed annot protos
+    """
+    input_protos, _ = self.dataset_obj.get_protos(batch_input_ids)
+    input_job_id = self._upload_inputs(input_protos)
+    retry_annot_protos = []
 
-  def retry_concurrent_uploads(
-      self,
-      retry_upload_protos: Union[List[resources_pb2.Input], List[resources_pb2.Annotation]],
-      upload_type: str = "input") -> None:
+    self._wait_for_inputs(input_job_id)
+    success_input_ids, failed_input_ids = self._delete_failed_inputs(batch_input_ids)
+
+    if self.task in ["visual_detection", "visual_segmentation"]:
+      _, annotation_protos = self.dataset_obj.get_protos(success_input_ids)
+      chunked_annotation_protos = Chunker(annotation_protos, self.chunk_size).chunk()
+      retry_annot_protos.extend(self._concurrent_annot_upload(chunked_annotation_protos))
+
+    return failed_input_ids, retry_annot_protos
+
+  def _retry_uploads(self, failed_input_ids: List[str],
+                     retry_annot_protos: List[resources_pb2.Annotation]) -> None:
+    """
+    Retry failed uploads.
+    Args:
+      failed_input_ids: failed input ids
+      retry_annot_protos: failed annot protos
+    """
+    if failed_input_ids:
+      self._upload_inputs_annotations(failed_input_ids)
+    if retry_annot_protos:
+      chunked_annotation_protos = Chunker(retry_annot_protos, self.chunk_size).chunk()
+      _ = self._concurrent_annot_upload(chunked_annotation_protos)
+
+  def _data_upload(self, input_ids: List[str]) -> None:
     """
-    Retry Uploads of inputs/annotations.
+    Uploads inputs and annotations to clarifai platform dataset.
     Args:
-      retry_upload_protos: upload protos for retry
-      upload_type: input/annot protos type
+      input_ids: input ids
     """
-    retry_chunked_upload_protos = Chunker(retry_upload_protos, self.chunk_size).chunk()
-    if len(retry_upload_protos) > 0 and upload_type == "input":
-      _ = self.concurrent_inp_upload(
-          retry_chunked_upload_protos,
-          len(retry_chunked_upload_protos),
-          desc="retry uploading failed input protos...")
-    elif len(retry_upload_protos) > 0 and upload_type == "annot":
-      _ = self.concurrent_annot_upload(
-          retry_chunked_upload_protos,
-          len(retry_chunked_upload_protos),
-          desc="retry uploading failed annotation protos...")
+    chunk_input_ids = Chunker(input_ids, self.chunk_size).chunk()
+    with ThreadPoolExecutor(max_workers=self.num_workers) as executor:
+      with tqdm(total=len(chunk_input_ids), desc='Uploading Dataset') as progress:
+        # Submit all jobs to the executor and store the returned futures
+        futures = [
+            executor.submit(self._upload_inputs_annotations, batch_input_ids)
+            for batch_input_ids in chunk_input_ids
+        ]
+
+        for job in as_completed(futures):
+          retry_input_proto, retry_annot_protos = job.result()
+          self._retry_uploads(retry_input_proto, retry_annot_protos)
+          progress.update()
 
   def upload_to_clarifai(self):
     """
     Execute data upload.
     """
     datagen_object = None
     if self.module_dir is None and self.zoo_dataset is None:
@@ -278,62 +343,21 @@
       but NOT both.")
     elif self.module_dir is not None:
       datagen_object = load_dataset(self.module_dir, self.split)
     else:
       datagen_object = load_zoo_dataset(self.zoo_dataset, self.split)
 
     if self.task == "text_clf":
-      dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
-      text_protos = dataset_obj._get_input_protos()
-      text_protos = dataset_obj._to_list(text_protos)
-
-      # Upload text
-      chunked_text_protos = Chunker(text_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_text_protos,
-                                                       len(chunked_text_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
+      self.dataset_obj = TextClassificationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
 
     elif self.task == "visual_detection":
-      dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
-      img_protos, annotation_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
-
-      # Upload annotations:
-      print("Uploading annotations.......")
-      annotation_protos = dataset_obj._to_list(annotation_protos)
-      chunked_annot_protos = Chunker(annotation_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_annot_upload(chunked_annot_protos,
-                                                         len(chunked_annot_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "annot")
+      self.dataset_obj = VisualDetectionDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)  # TODO: get_img_ids or get_input_ids
 
     elif self.task == "visual_segmentation":
-      dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
-      img_protos, mask_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-      mask_protos = dataset_obj._to_list(mask_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
-
-      # Upload masks:
-      print("Uploading masks.......")
-      chunked_mask_protos = Chunker(mask_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_annot_upload(chunked_mask_protos,
-                                                         len(chunked_mask_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "annot")
+      self.dataset_obj = VisualSegmentationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
 
     else:  # visual-classification & visual-captioning
-      dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
-      img_protos = dataset_obj._get_input_protos()
-      img_protos = dataset_obj._to_list(img_protos)
-
-      # Upload images
-      chunked_img_protos = Chunker(img_protos, self.chunk_size).chunk()
-      retry_upload_protos = self.concurrent_inp_upload(chunked_img_protos, len(chunked_img_protos))
-      self.retry_concurrent_uploads(retry_upload_protos, "input")
+      self.dataset_obj = VisualClassificationDataset(datagen_object, self.dataset_id, self.split)
+      self._data_upload(self.dataset_obj.input_ids)
```

### Comparing `clarifai-9.5.4/clarifai_utils/dataset_export/dataset_export_inputs.py` & `clarifai-9.6.0/clarifai_utils/dataset_export/dataset_export_inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/concepts.py` & `clarifai-9.6.0/clarifai_utils/listing/concepts.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/datasets.py` & `clarifai-9.6.0/clarifai_utils/listing/datasets.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/inputs.py` & `clarifai-9.6.0/clarifai_utils/listing/inputs.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/installed_module_versions.py` & `clarifai-9.6.0/clarifai_utils/listing/installed_module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/lister.py` & `clarifai-9.6.0/clarifai_utils/listing/lister.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/models.py` & `clarifai-9.6.0/clarifai_utils/listing/models.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/module_versions.py` & `clarifai-9.6.0/clarifai_utils/listing/module_versions.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/listing/modules.py` & `clarifai-9.6.0/clarifai_utils/listing/modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/api.py` & `clarifai-9.6.0/clarifai_utils/models/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Interface to Clarifai Models API."""
 
-from typing import Dict, List, Type
+from typing import Dict, Type
 
 from clarifai_grpc.grpc.api import resources_pb2, service_pb2
 from google.protobuf.json_format import MessageToDict
 from google.protobuf.struct_pb2 import Struct
 
 from clarifai.auth.helper import ClarifaiAuthHelper
 from clarifai.client import create_stub
@@ -96,92 +96,117 @@
 
     return {
         "Model Types": model_types,
         "Input Metadata": in_dims_dtype,
         "Output Metadata": out_dims_dtype
     }
 
-  def post_model(
+  def init_model(
       self,
       model_id: str,
-      model_zip_url: str,
       model_type: str,
-      input: List,
-      outputs: List,
       description: str = "",
   ):
-    """Post a new trained model to the Clarifai platform.
+    """Init a new model on Clarifai platform.
 
     Args:
         model_id (str): Clarifai model id
-        model_zip_url (str): url of zip of model
         model_type (str): Clarifai model type
-        input (List): list of a pair of clarifai input field and triton model input,
-            [clarifai_input_field, triton_input_filed]
-        outputs (List): list of pairs of clarifai output fields and triton model outputs,
-            [[clarifai_output_field1, triton_output_filed1],[clarifai_output_field2, triton_output_filed2],...]
         description (str, optional): a description of the model. Defaults to "".
 
     Returns:
         dict: Clarifai api response
     """
-
-    def _parse_fields_map(x):
-      """parse input, outputs to Struct"""
-      _fields_map = Struct()
-      if not isinstance(x[0], list):
-        x = [x]
-      for field, mapping in x:
-        _fields_map.update({field: mapping})
-      return _fields_map
-
-    input_fields_map = _parse_fields_map(input)
-    output_fields_map = _parse_fields_map(outputs)
     user_data_object = self.auth.get_user_app_id_proto()
     post_models_response = self.stub.PostModels(
         service_pb2.PostModelsRequest(
             user_app_id=user_data_object,
-            models=[
-                resources_pb2.Model(
-                    id=model_id,
-                    notes=description,
-                    model_type_id=model_type,
-                    model_version=resources_pb2.ModelVersion(
-                        pretrained_model_config=resources_pb2.PretrainedModelConfig(
-                            model_zip_url=model_zip_url,
-                            input_fields_map=input_fields_map,
-                            output_fields_map=output_fields_map)))
-            ]),
+            models=[resources_pb2.Model(id=model_id, notes=description,
+                                        model_type_id=model_type)]),
         metadata=self.auth.metadata)
 
     return MessageToDict(post_models_response, preserving_proto_field_name=True)
 
-  def post_model_version(self, model_id: str, model_zip_url: str):
+  def post_model_version(
+      self,
+      model_id: str,
+      model_zip_url: str,
+      input: dict,
+      outputs: dict,
+  ):
     """Post a new version of an existing model in the Clarifai platform.
 
     Args:
         model_id (str): Clarifai model id
         model_zip_url (str]): url of zip of model
+        model_zip_url (str): url of zip of model
+        input (dict): a dict where the key is clarifai input field and the value is triton model input,
+            {clarifai_input_field: triton_input_filed}.
+        outputs (dict): a dict where the keys are clarifai output fields and the values are triton model outputs,
+            {clarifai_output_field1: triton_output_filed1, clarifai_output_field2: triton_output_filed2,...}.
 
     Returns:
         dict: clarifai api response
     """
     user_data_object = self.auth.get_user_app_id_proto()
+
+    def _parse_fields_map(x):
+      """parse input, outputs to Struct"""
+      _fields_map = Struct()
+      _fields_map.update(x)
+      return _fields_map
+
+    input_fields_map = _parse_fields_map(input)
+    output_fields_map = _parse_fields_map(outputs)
     post_model_versions = self.stub.PostModelVersions(
         service_pb2.PostModelVersionsRequest(
             user_app_id=user_data_object,
             model_id=model_id,
             model_versions=[
-                resources_pb2.ModelVersion(pretrained_model_config=resources_pb2.
-                                           PretrainedModelConfig(model_zip_url=model_zip_url))
+                resources_pb2.ModelVersion(
+                    pretrained_model_config=resources_pb2.PretrainedModelConfig(
+                        model_zip_url=model_zip_url,
+                        input_fields_map=input_fields_map,
+                        output_fields_map=output_fields_map))
             ]),
         metadata=self.auth.metadata)
 
     return MessageToDict(post_model_versions, preserving_proto_field_name=True)
 
+  def upload_model(
+      self,
+      model_id: str,
+      model_zip_url: str,
+      input: dict,
+      outputs: dict,
+      model_type: str,
+      description: str = "",
+  ):
+    """Doing 2 requests for initializing and creating version for a new trained model to the Clarifai platform.
+
+    Args:
+        model_id (str): Clarifai model id
+        model_zip_url (str): url of zip of model
+        input (dict): a dict where the key is clarifai input field and the value is triton model input,
+            {clarifai_input_field: triton_input_filed}
+        outputs (dict): a dict where the keys are clarifai output fields and the values are triton model outputs,
+            {clarifai_output_field1: triton_output_filed1, clarifai_output_field2: triton_output_filed2,...}
+        model_type (str): Clarifai model type.
+        description (str, optional): a description of the model. Defaults to "".
+
+    Returns:
+        dict: Clarifai api response
+    """
+    init_resp = self.init_model(model_id, model_type, description)
+    if init_resp["status"]["code"] != "SUCCESS":
+      return init_resp
+    version_resp = self.post_model_version(model_id, model_zip_url, input, outputs)
+
+    return version_resp
+
   def delete_model(self, model_id: str):
     """Delete model api by model id
 
     Args:
         model_id (str): Clarifai model id
 
     Returns:
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/__init__.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/cli/__init__.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/cli/deploy_cli.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/deploy_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,46 +15,65 @@
 
 from clarifai.auth.helper import ClarifaiAuthHelper
 from clarifai.models.api import Models
 from clarifai.models.model_serving.constants import MODEL_TYPES
 from clarifai.models.model_serving.model_config.deploy import ClarifaiFieldsMap
 
 
-def deploy(model_url, model_id: str = None, model_type: str = None, desc: str = ""):
+def deploy(model_url,
+           model_id: str = None,
+           model_type: str = None,
+           desc: str = "",
+           update_version: bool = False):
   # init Auth from env vars
   auth = ClarifaiAuthHelper.from_env()
+  # init api
+  model_api = Models(auth)
+
   # parsing model name/type.
   # if filename having this format: <model_id>_<model-type>
   # e.i yolov5s_coco_visual-dectector
   # else user has to input model_type and model_id
   zip_filename = model_url.split('/')[-1]
   zip_filename = zip_filename.split('.')[0]
 
   def _parse_name(name):
     *id_, type_ = name.split('_')
     return "_".join(id_), type_
 
+  # parse model_id
   if not model_id and "_" in zip_filename:
     model_id = _parse_name(zip_filename)[0]
+  assert model_id, "Can not parse model_id from url, please input it directly"
+  # parse model_type
   if not model_type and "_" in zip_filename:
     model_type = _parse_name(zip_filename)[-1]
-  assert model_id or model_type, "Can not parse model_type or model_id from url, please input them directly"
+  assert model_type, "Can not parse model_type from url, please input it directly"
   # key map
   assert model_type in MODEL_TYPES, f"model_type should be one of {MODEL_TYPES}"
   clarifai_key_map = ClarifaiFieldsMap(model_type=model_type)
-  # init api
-  model_api = Models(auth)
-  # post model
-  resp = model_api.post_model(
-      model_id=model_id,
-      model_zip_url=model_url,
-      model_type=model_type,
-      input=clarifai_key_map.input_fields_map,
-      outputs=clarifai_key_map.output_fields_map,
-      description=desc)
+  # if updating new version of existing model
+  if update_version:
+    resp = model_api.post_model_version(
+        model_id=model_id,
+        model_zip_url=model_url,
+        input=clarifai_key_map.input_fields_map,
+        outputs=clarifai_key_map.output_fields_map,
+    )
+  # creating new model
+  else:
+    # post model
+    resp = model_api.upload_model(
+        model_id=model_id,
+        model_zip_url=model_url,
+        model_type=model_type,
+        input=clarifai_key_map.input_fields_map,
+        outputs=clarifai_key_map.output_fields_map,
+        description=desc,
+    )
   # response
   if resp["status"]["code"] != "SUCCESS":
     raise Exception("Post models failed, details: {}, {}".format(resp["status"]["description"],
                                                                  resp["status"]["details"]))
   else:
     print("Success!")
 
@@ -66,16 +85,26 @@
   parser.add_argument("--model_id", type=str, required=False, default="", help="Custom model id.")
   parser.add_argument(
       "--model_type",
       type=str,
       required=False,
       choices=MODEL_TYPES,
       default="",
-      help="Short description of model")
+      help="Clarifai model type")
   parser.add_argument(
       "--desc", type=str, required=False, default="", help="Short desccription of model")
+  parser.add_argument(
+      "--update_version",
+      action="store_true",
+      required=False,
+      help="Update exist model with new version")
   args = parser.parse_args()
-  deploy(model_url=args.url, model_id=args.model_id, desc=args.desc, model_type=args.model_type)
+  deploy(
+      model_url=args.url,
+      model_id=args.model_id,
+      desc=args.desc,
+      model_type=args.model_type,
+      update_version=args.update_version)
 
 
 if __name__ == "__main__":
   main()
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/cli/model_zip.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/model_zip.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/cli/repository.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/cli/repository.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/image_classification/age_vit/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/text_classification/xlm-roberta/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/examples/visual_detection/yolov5x/1/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/__init__.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/deploy.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/deploy.py`

 * *Files 22% similar despite different names*

```diff
@@ -33,17 +33,19 @@
   output_fields_map: List = field(default_factory=list)
 
   def __post_init__(self):
     """
     Set mapping of clarifai in/output vs triton in/output
     """
     if self.model_type == "visual-detector":
-      self.input_fields_map = ["image", "image"]
-      self.output_fields_map = [["regions[...].region_info.bounding_box", "predicted_bboxes"],
-                                ["regions[...].data.concepts[...].id", "predicted_labels"],
-                                ["regions[...].data.concepts[...].value", "predicted_scores"]]
+      self.input_fields_map = {"image": "image"}
+      self.output_fields_map = {
+          "regions[...].region_info.bounding_box": "predicted_bboxes",
+          "regions[...].data.concepts[...].id": "predicted_labels",
+          "regions[...].data.concepts[...].value": "predicted_scores"
+      }
     elif self.model_type == "visual-classifier":
-      self.input_fields_map = ["image", "image"]
-      self.output_fields_map = ["concepts", "softmax_predictions"]
+      self.input_fields_map = {"image": "image"}
+      self.output_fields_map = {"concepts": "softmax_predictions"}
     elif self.model_type == "text-classifier":
-      self.input_fields_map = ["text", "text"]
-      self.output_fields_map = ["concepts", "softmax_predictions"]
+      self.input_fields_map = {"text": "text"}
+      self.output_fields_map = {"concepts": "softmax_predictions"}
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/serializer.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/serializer.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/model_config/triton_config.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/model_config/triton_config.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/models/__init__.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/models/__init__.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/models/inference.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/models/inference.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 # This file contains boilerplate code to allow users write their model
 # inference code that will then interact with the Triton Inference Server
 # Python backend to serve end user requests.
-# The module name, module path and the setup() & predict() function names MUST be maintained as is
-# but other functions may be added within this module as deemed fit provided
-# they are invoked within the main predict() function if they play a role any
-# step of model inference
+# The module name, module path, class name & get_predictions() method names MUST be maintained as is
+# but other methods may be added within the class as deemed fit provided
+# they are invoked within the main get_predictions() inference method
+# if they play a role in any step of model inference
 """User model inference script."""
 
 import os
-from typing import Callable
+from pathlib import Path
 
-BASE_PATH = os.path.dirname(__file__)
 
+class InferenceModel:
+  """User model inference class."""
 
-def setup():
-  """
-  Load inference model.
-  The model checkpoint(s) should be saved in the same directory and directory
-  level as this inference.py module.
-
-  Returns:
-  --------
-    Inference Model Callable
-  """
-  # sample model loading code:
-  # checkpoint_path = os.path.join(BASE_PATH, your_checkpoint_name)
-  # model = <load model from checkpoint_path>
-  # return model
-
-  # Delete/Comment out line below and add your code
-  raise NotImplementedError()
-
-
-def predict(input_data, model: Callable):
-  """
-  Main model inference function.
-
-  Args:
-  -----
-    input_data: A single input data item to predict on.
-      Input data can be an image or text, etc depending on the model type.
-    model: Inference model callable as returned by setup() above.
-
-  Returns:
-  --------
-    One of the clarifai.model_serving.models.output types. Refer to the README/docs
-  """
-  # Delete/Comment out line below and add your inference code
-  raise NotImplementedError()
+  def __init__(self) -> None:
+    """
+    Load inference time artifacts that are called frequently .e.g. models, tokenizers, etc.
+    in this method so they are loaded only once for faster inference.
+    """
+    self.base_path: Path = os.path.dirname(__file__)
+    ## sample model loading code:
+    #self.checkpoint_path: Path = os.path.join(self.base_path, "your checkpoint filename/path")
+    #self.model: Callable = <load_your_model_here from checkpoint or folder>
+
+  #Add relevant model type decorator to the method below (see docs/model_types for ref.)
+  def get_predictions(self, input_data):
+    """
+    Main model inference method.
+
+    Args:
+    -----
+      input_data: A single input data item to predict on.
+        Input data can be an image or text, etc depending on the model type.
+
+    Returns:
+    --------
+      One of the clarifai.models.model_serving.models.output types. Refer to the README/docs
+    """
+    # Delete/Comment out line below and add your inference code
+    raise NotImplementedError()
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/models/model_types.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/models/model_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # limitations under the License.
 """
 Parse inference model predictions to triton inference responses
 per model type.
 """
 
 from functools import wraps
-from typing import Callable, List
+from typing import Callable
 
 import numpy as np
 
 try:
   import triton_python_backend_utils as pb_utils
 except ModuleNotFoundError:
   pass
@@ -28,23 +28,23 @@
 
 def visual_detector(func: Callable):
   """
   Visual detector type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_bboxes = []
     out_labels = []
     out_scores = []
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_bboxes.append(preds.predicted_bboxes)
       out_labels.append(preds.predicted_labels)
       out_scores.append(preds.predicted_scores)
 
     if len(out_bboxes) < 1 or len(out_labels) < 1:
       out_tensor_bboxes = pb_utils.Tensor("predicted_bboxes", np.zeros((0, 4), dtype=np.float32))
       out_tensor_labels = pb_utils.Tensor("predicted_labels", np.zeros((0, 1), dtype=np.int32))
@@ -67,21 +67,21 @@
 
 def visual_classifier(func: Callable):
   """
   Visual classifier type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_scores = []
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_scores.append(preds.predicted_scores)
 
     out_tensor_scores = pb_utils.Tensor("softmax_predictions",
                                         np.asarray(out_scores, dtype=np.float32))
     inference_response = pb_utils.InferenceResponse(output_tensors=[out_tensor_scores])
 
     return inference_response
@@ -91,22 +91,22 @@
 
 def text_classifier(func: Callable):
   """
   Text classifier type output parser.
   """
 
   @wraps(func)
-  def parse_predictions(input_data: List[List], model: Callable):
+  def parse_predictions(self, input_data: np.ndarray):
     """
     Format predictions and return clarifai compatible output.
     """
     out_scores = []
     input_data = [in_elem[0].decode() for in_elem in input_data]
     for item in input_data:
-      preds = func(item, model)
+      preds = func(self, item)
       out_scores.append(preds.predicted_scores)
 
     out_tensor_scores = pb_utils.Tensor("softmax_predictions",
                                         np.asarray(out_scores, dtype=np.float32))
     inference_response = pb_utils.InferenceResponse(output_tensors=[out_tensor_scores])
 
     return inference_response
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/models/output.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/models/output.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/models/pb_model.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/models/pb_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,18 +30,17 @@
 
   def initialize(self, args):
     """
     Triton server init.
     """
     args["model_repository"] = args["model_repository"].replace("/1/model.py", "")
     sys.path.append(os.path.dirname(__file__))
-    from inference import predict, setup
+    from inference import InferenceModel
 
-    self.inference_func = predict
-    self.model = setup()
+    self.inference_obj = InferenceModel()
     self.device = "cuda:0" if "GPU" in args["model_instance_kind"] else "cpu"
 
     # Read input_name from config file
     self.config_msg = ModelConfig()
     with open(os.path.join(args["model_repository"], "config.pbtxt"), "r") as f:
       cfg = f.read()
     text_format.Merge(cfg, self.config_msg)
@@ -52,11 +51,11 @@
     Serve model inference requests.
     """
     responses = []
 
     for request in requests:
       in_batch = pb_utils.get_input_tensor_by_name(request, self.input_name)
       in_batch = in_batch.as_numpy()
-      inference_response = self.inference_func(in_batch, self.model)
+      inference_response = self.inference_obj.get_predictions(in_batch)
       responses.append(inference_response)
 
     return responses
```

### Comparing `clarifai-9.5.4/clarifai_utils/models/model_serving/pb_model_repository.py` & `clarifai-9.6.0/clarifai_utils/models/model_serving/pb_model_repository.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         if hasattr(out_field, "label_filename"):
           with open(os.path.join(repository_path, "labels.txt"), "w"):
             pass
         else:
           continue
       # gen requirements & conda yaml
       with open(os.path.join(repository_path, "requirements.txt"), "w") as f:
-        f.write("clarifai\ntritonclient==2.34.0")  # for model upload utils
+        f.write("clarifai>9.5.3\ntritonclient[all]")  # for model upload utils
       with open(os.path.join(repository_path, "triton_conda.yaml"), "w") as conda_env:
         conda_env.write("name: triton_conda-cp3.8-torch1.13.1-19f97078")
 
     if not os.path.isdir(model_version_path):
       os.mkdir(model_version_path)
     if not os.path.exists(os.path.join(model_version_path, "__init__.py")):
       with open(os.path.join(model_version_path, "__init__.py"), "w"):
```

### Comparing `clarifai-9.5.4/clarifai_utils/modules/css.py` & `clarifai-9.6.0/clarifai_utils/modules/css.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/modules/pages.py` & `clarifai-9.6.0/clarifai_utils/modules/pages.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/modules/style.css` & `clarifai-9.6.0/clarifai_utils/modules/style.css`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/clarifai_utils/urls/helper.py` & `clarifai-9.6.0/clarifai_utils/urls/helper.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/setup.py` & `clarifai-9.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 packages = setuptools.find_namespace_packages(include=["clarifai*"])
 
 setuptools.setup(
     name="clarifai",
-    version="9.5.4",
+    version="9.6.0",
     author="Clarifai",
     author_email="support@clarifai.com",
     description="Clarifai Python Utilities",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Clarifai/clarifai-python-utils",
     packages=packages,
@@ -20,15 +20,15 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     license="Apache 2.0",
     python_requires='>=3.8',
     install_requires=[
-        "clarifai-grpc>=9.5.0",
+        "clarifai-grpc>=9.6.0",
         "tritonclient==2.34.0",
         "packaging",
     ],
     entry_points={
         "console_scripts": [
             "clarifai-model-upload-init = clarifai.models.model_serving.cli.repository:model_upload_init",
             "clarifai-triton-zip = clarifai.models.model_serving.cli.model_zip:main",
```

### Comparing `clarifai-9.5.4/tests/test_auth.py` & `clarifai-9.6.0/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/tests/test_modules.py` & `clarifai-9.6.0/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `clarifai-9.5.4/tests/test_stub.py` & `clarifai-9.6.0/tests/test_stub.py`

 * *Files identical despite different names*

