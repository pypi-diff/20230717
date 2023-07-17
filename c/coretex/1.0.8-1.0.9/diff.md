# Comparing `tmp/coretex-1.0.8.tar.gz` & `tmp/coretex-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coretex-1.0.8.tar", last modified: Mon Jul  3 08:16:20 2023, max compression
+gzip compressed data, was "coretex-1.0.9.tar", last modified: Thu Jul  6 13:36:35 2023, max compression
```

## Comparing `coretex-1.0.8.tar` & `coretex-1.0.9.tar`

### file list

```diff
@@ -1,191 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.575549 coretex-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-07-03 08:16:09.000000 coretex-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 08:16:20.571549 coretex-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-03 08:16:09.000000 coretex-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/cache/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/cache/cache_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/codable/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/codable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/codable/descriptor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/annotation/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/annotation/image/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/bbox.py
--rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/classes_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/annotation/image/coretex_format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex/coretex/conversion/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/base_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converter_processor_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/conversion/converters/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/city_scape_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/coco_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/create_ml_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/human_segmentation_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/label_me_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/instance_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/pascal/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/voc_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/conversion/converters/yolo_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.543548 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/image_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/local_image_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/local_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/network_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.547548 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/sequence_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/dataset/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.551548 coretex-1.0.8/coretex/coretex/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    16384 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/experiment_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.551548 coretex-1.0.8/coretex/coretex/experiment/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/metric_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/metrics/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/experiment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/model/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.555548 coretex-1.0.8/coretex/coretex/sample/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/any_local_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/custom_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/custom_sample/local_custom_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/image_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_sample/local_image_sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.559548 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/local_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/network_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/coretex/sample/sequence_sample/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/local_sequence_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/sequence_sample/sequence_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/sample/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/coretex/space/
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/coretex/space/space_task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/folder_management/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/folder_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/folder_management/folder_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.563549 coretex-1.0.8/coretex/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/log_severity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.567549 coretex-1.0.8/coretex/networking/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/chunk_upload_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/file_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_manager_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/network_response.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/request_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/requests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/networking/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.567549 coretex-1.0.8/coretex/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4308 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/calculate_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/project/remote.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/qiime2/
--rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/qiime2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/qiime2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/threading/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/threading/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/threading/threaded_data_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.571549 coretex-1.0.8/coretex/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/console_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-03 08:16:09.000000 coretex-1.0.8/coretex/utils/number.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 08:16:20.539548 coretex-1.0.8/coretex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-03 08:16:20.000000 coretex-1.0.8/coretex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-03 08:16:09.000000 coretex-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 08:16:20.575549 coretex-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.414537 coretex-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    31740 2023-07-06 13:36:19.000000 coretex-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-06 13:36:35.414537 coretex-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-07-06 13:36:19.000000 coretex-1.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.382537 coretex-1.0.9/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.382537 coretex-1.0.9/coretex/cache/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10306 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/cache/cache_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.386536 coretex-1.0.9/coretex/codable/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/codable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9139 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/codable/codable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1688 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/codable/descriptor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.386536 coretex-1.0.9/coretex/coretex/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.386536 coretex-1.0.9/coretex/coretex/annotation/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/annotation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.386536 coretex-1.0.9/coretex/coretex/annotation/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/annotation/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/annotation/image/bbox.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7629 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/annotation/image/classes_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/annotation/image/coretex_format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.386536 coretex-1.0.9/coretex/coretex/conversion/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converter_processor_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.390536 coretex-1.0.9/coretex/coretex/conversion/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/city_scape_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/coco_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/create_ml_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/human_segmentation_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/label_me_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.390536 coretex-1.0.9/coretex/coretex/conversion/converters/pascal/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/pascal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/pascal/instance_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/pascal/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/voc_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/conversion/converters/yolo_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.390536 coretex-1.0.9/coretex/coretex/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.390536 coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.394537 coretex-1.0.9/coretex/coretex/dataset/custom_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/custom_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/custom_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/custom_dataset/custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.394537 coretex-1.0.9/coretex/coretex/dataset/image_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_dataset/image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_dataset/local_image_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.394537 coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/local_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6060 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/network_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.394537 coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/sequence_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/dataset/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.394537 coretex-1.0.9/coretex/coretex/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15778 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/experiment_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.398537 coretex-1.0.9/coretex/coretex/experiment/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/metric_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/metric_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.398537 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/swap_usage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/metrics/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7663 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3121 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/experiment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.402537 coretex-1.0.9/coretex/coretex/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.402537 coretex-1.0.9/coretex/coretex/sample/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/any_local_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.402537 coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.402537 coretex-1.0.9/coretex/coretex/sample/custom_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/custom_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/custom_sample/custom_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/custom_sample/custom_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/custom_sample/local_custom_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/coretex/sample/image_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_sample/image_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3578 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_sample/image_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_sample/image_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_sample/local_image_sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/local_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/network_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/coretex/sample/sequence_sample/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/sequence_sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/sequence_sample/local_sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/sequence_sample/sequence_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/sample/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/coretex/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/space/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/space/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/space/space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/coretex/space/space_task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/folder_management/
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/folder_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/folder_management/folder_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.406537 coretex-1.0.9/coretex/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/logging/log_severity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.410537 coretex-1.0.9/coretex/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5024 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/chunk_upload_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/file_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/network_manager_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7892 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/network_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/network_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/request_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/requests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/networking/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.410537 coretex-1.0.9/coretex/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.410537 coretex-1.0.9/coretex/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/project/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4566 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/project/experiment_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/project/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/project/remote.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.414537 coretex-1.0.9/coretex/qiime2/
+-rw-r--r--   0 runner    (1001) docker     (123)     8821 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/qiime2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/qiime2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.414537 coretex-1.0.9/coretex/threading/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/threading/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/threading/threaded_data_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.414537 coretex-1.0.9/coretex/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/utils/console_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1433 2023-07-06 13:36:19.000000 coretex-1.0.9/coretex/utils/number.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 13:36:35.382537 coretex-1.0.9/coretex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5120 2023-07-06 13:36:35.000000 coretex-1.0.9/coretex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-06 13:36:35.000000 coretex-1.0.9/coretex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 13:36:35.000000 coretex-1.0.9/coretex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-06 13:36:35.000000 coretex-1.0.9/coretex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 13:36:35.000000 coretex-1.0.9/coretex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-06 13:36:19.000000 coretex-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 13:36:35.414537 coretex-1.0.9/setup.cfg
```

### Comparing `coretex-1.0.8/LICENSE` & `coretex-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/PKG-INFO` & `coretex-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.8/README.md` & `coretex-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/__init__.py` & `coretex-1.0.9/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/_configuration.py` & `coretex-1.0.9/coretex/_configuration.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/_logger.py` & `coretex-1.0.9/coretex/_logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/cache/__init__.py` & `coretex-1.0.9/coretex/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/cache/cache_module.py` & `coretex-1.0.9/coretex/cache/cache_module.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/codable/__init__.py` & `coretex-1.0.9/coretex/codable/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/codable/codable.py` & `coretex-1.0.9/coretex/codable/codable.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/codable/descriptor.py` & `coretex-1.0.9/coretex/codable/descriptor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/__init__.py` & `coretex-1.0.9/coretex/coretex/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/annotation/__init__.py` & `coretex-1.0.9/coretex/coretex/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/annotation/image/__init__.py` & `coretex-1.0.9/coretex/coretex/annotation/image/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/annotation/image/bbox.py` & `coretex-1.0.9/coretex/coretex/annotation/image/bbox.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/annotation/image/classes_format.py` & `coretex-1.0.9/coretex/coretex/annotation/image/classes_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/annotation/image/coretex_format.py` & `coretex-1.0.9/coretex/coretex/annotation/image/coretex_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/__init__.py` & `coretex-1.0.9/coretex/coretex/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/base_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/base_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converter_processor_factory.py` & `coretex-1.0.9/coretex/coretex/conversion/converter_processor_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/__init__.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/city_scape_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/city_scape_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/coco_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/coco_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/create_ml_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/create_ml_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/human_segmentation_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/human_segmentation_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/label_me_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/label_me_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/__init__.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/pascal/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/instance_extractor.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/pascal/instance_extractor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/pascal/pascal_2012_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/pascal/shared.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/pascal/shared.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/voc_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/voc_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/conversion/converters/yolo_converter.py` & `coretex-1.0.9/coretex/coretex/conversion/converters/yolo_converter.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/computer_vision_dataset/local_computer_vision_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/custom_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/base.py` & `coretex-1.0.9/coretex/coretex/dataset/custom_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/custom_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/custom_dataset/custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/custom_dataset/local_custom_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/image_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_dataset/base.py` & `coretex-1.0.9/coretex/coretex/dataset/image_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_dataset/image_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/image_dataset/image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_dataset/local_image_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/image_dataset/local_image_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py` & `coretex-1.0.9/coretex/coretex/dataset/image_dataset/synthetic_image_generator.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/image_segmentation_dataset/local_image_segmentation_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/local_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/local_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/network_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/network_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/__init__.py` & `coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/base.py` & `coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/local_sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/sequence_dataset/sequence_dataset.py` & `coretex-1.0.9/coretex/coretex/dataset/sequence_dataset/sequence_dataset.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/dataset/utils.py` & `coretex-1.0.9/coretex/coretex/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/__init__.py` & `coretex-1.0.9/coretex/coretex/experiment/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/artifact.py` & `coretex-1.0.9/coretex/coretex/experiment/artifact.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/experiment.py` & `coretex-1.0.9/coretex/coretex/experiment/experiment.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,14 @@
             name of project
         createdById : str
             id of created experiment
         useCachedEnv : bool
             if True chached env will be used, otherwise new environment will be created
     """
 
-    __statusUpdateLock: Final = Lock()
-
     name: str
     description: str
     meta: Dict[str, Any]
     status: ExperimentStatus
     spaceId: int
     spaceName: str
     spaceTask: SpaceTask
@@ -87,16 +85,14 @@
     useCachedEnv: bool
     metrics: List[Metric]
 
     def __init__(self) -> None:
         super(Experiment, self).__init__()
 
         self.metrics = []
-
-        self.__lastStatusMessage: Optional[str] = None
         self.__parameters: Dict[str, Any] = {}
 
     @property
     def parameters(self) -> Dict[str, Any]:
         """
             Returns
             -------
@@ -143,15 +139,14 @@
         descriptors["spaceId"] = KeyDescriptor("project_id")
         descriptors["spaceName"] = KeyDescriptor("project_name")
         descriptors["spaceTask"] = KeyDescriptor("project_task", SpaceTask)
         descriptors["projectId"] = KeyDescriptor("sub_project_id")
         descriptors["projectName"] = KeyDescriptor("sub_project_name")
 
         # private properties of the object should not be encoded
-        descriptors["__lastStatusMessage"] = KeyDescriptor(isEncodable = False)
         descriptors["__parameters"] = KeyDescriptor(isEncodable = False)
 
         return descriptors
 
     @classmethod
     def _endpoint(cls) -> str:
         return "model-queue"
@@ -164,68 +159,73 @@
 
         if not isinstance(self.meta["parameters"], list):
             raise ValueError(">> [Coretex] Invalid parameters")
 
         parameters = [ExperimentParameter.decode(value) for value in self.meta["parameters"]]
         self.__parameters = parseParameters(parameters, self.spaceTask)
 
-    def updateStatus(self, status: ExperimentStatus, message: Optional[str] = None, notifyServer: bool = True) -> bool:
+    def updateStatus(
+        self,
+        status: Optional[ExperimentStatus] = None,
+        message: Optional[str] = None,
+        notifyServer: bool = True
+    ) -> bool:
+
         """
             Updates Experiment status, if message parameter is None
             default message value will be used\n
             Some Experiment statuses do not have default message
 
             Parameters
             ----------
-            status : ExperimentStatus
-                ExperimentStatus type
+            status : Optional[ExperimentStatus]
+                Status to which the experiment will be updated to
             message : Optional[str]
-                Descriptive message for experiment status
+                Descriptive message for experiment status, it is diplayed
+                when the status is hovered on the Coretex Web App
             notifyServer : bool
                 if True update request will be sent to Coretex.ai
 
             Example
             -------
             >>> from coretex import ExecutingExperiment, ExperimentStatus
             \b
             >>> ExecutingExperiment.current().updateStatus(
                     ExperimentStatus.completedWithSuccess
                 )
             True
         """
 
-        with Experiment.__statusUpdateLock:
-            if message is None:
-                message = status.defaultMessage
-
-            assert(len(message) > 10)  # Some information needs to be sent to Coretex.ai
+        if status is not None:
             self.status = status
-            self.__lastStatusMessage = message
+
+        if notifyServer:
+            if status is not None and message is None:
+                message = status.defaultMessage
 
             parameters: Dict[str, Any] = {
-                "id": self.id,
-                "status": status.value,
-                "status_message": message
+                "id": self.id
             }
 
-            if notifyServer:
-                # TODO: Should API rename this too?
-                endpoint = "model-queue/job-status-update"
-                response = networkManager.genericJSONRequest(
-                    endpoint = endpoint,
-                    requestType = RequestType.post,
-                    parameters = parameters
-                )
+            if status is not None:
+                parameters["status"] = status
+
+            if message is not None:
+                parameters["message"] = message
 
-                if response.hasFailed():
-                    logging.getLogger("coretexpylib").error(">> [Coretex] Error while updating experiment status")
+            # TODO: Should API rename this too?
+            endpoint = "model-queue/job-status-update"
+            response = networkManager.genericJSONRequest(endpoint, RequestType.post, parameters)
 
-                return not response.hasFailed()
+            if response.hasFailed():
+                logging.getLogger("coretexpylib").error(">> [Coretex] Error while updating experiment status")
 
-            return True
+            return not response.hasFailed()
+
+        return True
 
     def createMetrics(self, metrics: List[Metric]) -> None:
         """
             Creates specified metrics for the experiment
 
             Parameters
             ----------
@@ -307,29 +307,14 @@
             "model-queue/metrics",
             RequestType.post,
             parameters
         )
 
         return not response.hasFailed()
 
-    def sendHeartbeat(self) -> bool:
-        """
-            Sends an update status request with the status and the
-            status message of the previous status update
-
-            Returns
-            -------
-            bool -> True if success, False otherwise
-        """
-
-        if self.__lastStatusMessage:
-            return False
-
-        return self.updateStatus(self.status, self.__lastStatusMessage)
-
     def downloadProject(self) -> bool:
         """
             Downloads project snapshot linked to the experiment
 
             Returns
             -------
             bool -> True if project downloaded successfully, False if project download has failed
```

### Comparing `coretex-1.0.8/coretex/coretex/experiment/experiment_builder.py` & `coretex-1.0.9/coretex/coretex/experiment/experiment_builder.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/__init__.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/metric.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/metric_factory.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/metric_factory.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/metric_type.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/metric_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/cpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/disk_read.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/disk_write.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/download_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/gpu_temperature.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/gpu_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/ram_usage.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/predefined_metrics/upload_speed.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/metrics/utils.py` & `coretex-1.0.9/coretex/coretex/experiment/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/parameters.py` & `coretex-1.0.9/coretex/coretex/experiment/parameters.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/status.py` & `coretex-1.0.9/coretex/coretex/experiment/status.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/experiment/utils.py` & `coretex-1.0.9/coretex/coretex/experiment/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/model/__init__.py` & `coretex-1.0.9/coretex/coretex/model/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/model/model.py` & `coretex-1.0.9/coretex/coretex/model/model.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/any_local_sample.py` & `coretex-1.0.9/coretex/coretex/sample/any_local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py` & `coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py` & `coretex-1.0.9/coretex/coretex/sample/computer_vision_sample/local_computer_vision_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/custom_sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/custom_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample.py` & `coretex-1.0.9/coretex/coretex/sample/custom_sample/custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/custom_sample/custom_sample_data.py` & `coretex-1.0.9/coretex/coretex/sample/custom_sample/custom_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/custom_sample/local_custom_sample.py` & `coretex-1.0.9/coretex/coretex/sample/custom_sample/local_custom_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/image_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_sample/image_format.py` & `coretex-1.0.9/coretex/coretex/sample/image_sample/image_format.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample.py` & `coretex-1.0.9/coretex/coretex/sample/image_sample/image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_sample/image_sample_data.py` & `coretex-1.0.9/coretex/coretex/sample/image_sample/image_sample_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_sample/local_image_sample.py` & `coretex-1.0.9/coretex/coretex/sample/image_sample/local_image_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py` & `coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py` & `coretex-1.0.9/coretex/coretex/sample/image_segmentation_sample/local_image_segmentation_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/local_sample.py` & `coretex-1.0.9/coretex/coretex/sample/local_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/network_sample.py` & `coretex-1.0.9/coretex/coretex/sample/network_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/sample.py` & `coretex-1.0.9/coretex/coretex/sample/sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/sequence_sample/__init__.py` & `coretex-1.0.9/coretex/coretex/sample/sequence_sample/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/sequence_sample/local_sequence_sample.py` & `coretex-1.0.9/coretex/coretex/sample/sequence_sample/local_sequence_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/sequence_sample/sequence_sample.py` & `coretex-1.0.9/coretex/coretex/sample/sequence_sample/sequence_sample.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/sample/utils.py` & `coretex-1.0.9/coretex/coretex/sample/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/space/__init__.py` & `coretex-1.0.9/coretex/coretex/space/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/space/base.py` & `coretex-1.0.9/coretex/coretex/space/base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/space/project.py` & `coretex-1.0.9/coretex/coretex/space/project.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/space/space.py` & `coretex-1.0.9/coretex/coretex/space/space.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/coretex/space/space_task.py` & `coretex-1.0.9/coretex/coretex/space/space_task.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/folder_management/__init__.py` & `coretex-1.0.9/coretex/folder_management/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/folder_management/folder_manager.py` & `coretex-1.0.9/coretex/folder_management/folder_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
             with cls.__instanceLock:
                 if cls.__instance is None:
                     cls.__instance = cls()
 
         return cls.__instance
 
     def __init__(self) -> None:
-        self.__root: Final = Path(os.environ["CTX_STORAGE_PATH"]).expanduser()
+        self._root: Final = Path(os.environ["CTX_STORAGE_PATH"]).expanduser()
 
         # These paths are str paths for backwards compatibility
         self.samplesFolder: Final = str(self.__createFolder("samples"))
         self.modelsFolder: Final = str(self.__createFolder("models"))
         self.temp: Final = str(self.__createFolder("temp"))
 
         # These paths are pathlib.Paths
@@ -171,15 +171,15 @@
             Deletes all temp files and folders (including artifacts)
         """
 
         self.__clearDirectory(self.temp)
         self.__clearDirectory(self.__artifactsFolder)
 
     def __createFolder(self, name: str) -> Path:
-        path = self.__root / name
+        path = self._root / name
 
         if not path.exists():
             path.mkdir(parents = True, exist_ok = True)
 
         return path
 
     def __clearDirectory(self, path: Union[Path, str]) -> None:
```

### Comparing `coretex-1.0.8/coretex/logging/__init__.py` & `coretex-1.0.9/coretex/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/logging/log.py` & `coretex-1.0.9/coretex/logging/log.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/logging/log_severity.py` & `coretex-1.0.9/coretex/logging/log_severity.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/logging/logger.py` & `coretex-1.0.9/coretex/logging/logger.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/__init__.py` & `coretex-1.0.9/coretex/networking/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/chunk_upload_session.py` & `coretex-1.0.9/coretex/networking/chunk_upload_session.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/file_data.py` & `coretex-1.0.9/coretex/networking/file_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/network_manager.py` & `coretex-1.0.9/coretex/networking/network_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/network_manager_base.py` & `coretex-1.0.9/coretex/networking/network_manager_base.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/network_object.py` & `coretex-1.0.9/coretex/networking/network_object.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/network_response.py` & `coretex-1.0.9/coretex/networking/network_response.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/request_type.py` & `coretex-1.0.9/coretex/networking/request_type.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/requests_manager.py` & `coretex-1.0.9/coretex/networking/requests_manager.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/networking/user_data.py` & `coretex-1.0.9/coretex/networking/user_data.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/__init__.py` & `coretex-1.0.9/coretex/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/text.py` & `coretex-1.0.9/coretex/nlp/text.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/token.py` & `coretex-1.0.9/coretex/nlp/token.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/transcriber.py` & `coretex-1.0.9/coretex/nlp/transcriber.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/transcription.py` & `coretex-1.0.9/coretex/nlp/transcription.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/nlp/utils.py` & `coretex-1.0.9/coretex/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/project/__init__.py` & `coretex-1.0.9/coretex/project/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/project/base.py` & `coretex-1.0.9/coretex/project/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,36 +22,37 @@
 import logging
 import multiprocessing
 
 from ..coretex import Experiment
 from ..folder_management import FolderManager
 from ..logging import LogHandler
 
-from .calculate_metrics import uploadMetricsWorker
+from .experiment_worker import experimentWorker
 
 
 class ProjectCallback:
 
     def __init__(self, experiment: Experiment, refreshToken: str) -> None:
         self._experiment: Final = experiment
 
         self.__outputStream, self.__inputStream = multiprocessing.Pipe()
 
-        self.process = multiprocessing.Process(
-            target = uploadMetricsWorker,
+        self.workerProcess = multiprocessing.Process(
+            name = f"Experiment {experiment.id} worker process",
+            target = experimentWorker,
             args = (self.__outputStream, refreshToken, self._experiment.id),
             daemon = True
         )
 
     @classmethod
     def create(cls, experimentId: int, refreshToken: str) -> Self:
         return cls(Experiment.fetchById(experimentId), refreshToken)
 
     def onStart(self) -> None:
-        self.process.start()
+        self.workerProcess.start()
 
         result = self.__inputStream.recv()
         if result["code"] != 0:
             raise RuntimeError(result["message"])
 
         logging.getLogger("coretexpylib").info(result["message"])
 
@@ -69,16 +70,16 @@
         FolderManager.instance().clearTempFiles()
 
         sys.exit(1)
 
     def onCleanUp(self) -> None:
         logging.getLogger("coretexpylib").info("Experiment execution finished")
 
-        self.process.kill()
-        self.process.join()
+        self.workerProcess.kill()
+        self.workerProcess.join()
 
         try:
             from py3nvml import py3nvml
             py3nvml.nvmlShutdown()
         except:
             pass
```

### Comparing `coretex-1.0.8/coretex/project/calculate_metrics.py` & `coretex-1.0.9/coretex/project/experiment_worker.py`

 * *Files 11% similar despite different names*

```diff
@@ -65,50 +65,65 @@
             createMetric("gpu_usage", "time (s)", MetricType.interval, "usage (%)", MetricType.percent, None, [0, 100]),
             createMetric("gpu_temperature", "time (s)", MetricType.interval, "usage (%)", MetricType.percent)
         ])
     except:
         pass
 
 
-def uploadMetricsWorker(outputStream: Connection, refreshToken: str, experimentId: int) -> None:
+def _isAlive(output: Connection) -> bool:
+    try:
+        # If parent process gets killed with SIGKILL there
+        # is no guarantee that the child process will get
+        # closed so we ping the parent process to check if
+        # the pipe is available or not
+        output.send(None)
+    except BrokenPipeError:
+        output.close()
+        return False
+
+    return output.writable and not output.closed
+
+
+def _heartbeat(experiment: Experiment) -> None:
+    # Update status without parameters is considered experiment hearbeat
+    experiment.updateStatus()
+
+
+def _uploadMetrics(experiment: Experiment) -> None:
+    x = time.time()
+    metricValues: Dict[str, Tuple[float, float]] = {}
+
+    for metric in experiment.metrics:
+        metricValue = metric.extract()
+
+        if metricValue is not None:
+            metricValues[metric.name] = x, metricValue
+
+    experiment.submitMetrics(metricValues)
+
+
+def experimentWorker(outputStream: Connection, refreshToken: str, experimentId: int) -> None:
     setupGPUMetrics()
 
     response = networkManager.authenticateWithRefreshToken(refreshToken)
     if response.hasFailed():
         sendFailure(outputStream, "Failed to authenticate with refresh token")
         return
 
     try:
         experiment: Experiment = Experiment.fetchById(experimentId)
     except NetworkRequestError:
-        sendFailure(outputStream, f"Failed to fetch experiment with id: {experimentId}")
+        sendFailure(outputStream, f"Failed to fetch experiment with id \"{experimentId}\"")
         return
 
     try:
         experiment.createMetrics(METRICS)
     except NetworkRequestError:
         sendFailure(outputStream, "Failed to create metrics")
 
-    sendSuccess(outputStream, "Metrics worker succcessfully started")
-
-    while outputStream.writable and not outputStream.closed:
-        try:
-            # If parent process gets killed with SIGKILL there
-            # is no guarantee that the child process will get
-            # closed so we ping the parent process to check if
-            # the pipe is available or not
-            outputStream.send(None)
-        except BrokenPipeError:
-            outputStream.close()
-            break
-
-        startTime = time.time()
-        metricValues: Dict[str, Tuple[float, float]] = {}
-
-        for metric in experiment.metrics:
-            metricValue = metric.extract()
+    sendSuccess(outputStream, "Experiment worker succcessfully started")
 
-            if metricValue is not None:
-                metricValues[metric.name] = startTime, metricValue
+    while _isAlive(outputStream):
+        _heartbeat(experiment)
+        _uploadMetrics(experiment)
 
-        experiment.submitMetrics(metricValues)
         time.sleep(5)  # delay between sending generic metrics
```

### Comparing `coretex-1.0.8/coretex/project/local.py` & `coretex-1.0.9/coretex/project/local.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,34 +21,28 @@
 import logging
 import os
 
 from tap import Tap
 
 import psutil
 
-from .heartbeat import Heartbeat
 from .base import ProjectCallback
 from ..coretex import Experiment, ExperimentStatus
 from ..folder_management import FolderManager
 from ..networking import networkManager
 from ..coretex.experiment.parameters import ExperimentParameter
 
 
 class LocalProjectCallback(ProjectCallback):
 
     def onStart(self) -> None:
         super().onStart()
 
         FolderManager.instance().clearTempFiles()
 
-        logging.getLogger("coretexpylib").info("Heartbeat started")
-
-        heartbeat = Heartbeat(self._experiment)
-        heartbeat.start()
-
     def onSuccess(self) -> None:
         super().onSuccess()
 
         self._experiment.updateStatus(ExperimentStatus.completedWithSuccess)
 
     def onKeyboardInterrupt(self) -> None:
         super().onKeyboardInterrupt()
```

### Comparing `coretex-1.0.8/coretex/project/remote.py` & `coretex-1.0.9/coretex/project/remote.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/qiime2/__init__.py` & `coretex-1.0.9/coretex/qiime2/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/qiime2/utils.py` & `coretex-1.0.9/coretex/qiime2/utils.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/threading/__init__.py` & `coretex-1.0.9/coretex/threading/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/threading/threaded_data_processor.py` & `coretex-1.0.9/coretex/threading/threaded_data_processor.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/utils/__init__.py` & `coretex-1.0.9/coretex/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/utils/console_progress_bar.py` & `coretex-1.0.9/coretex/utils/console_progress_bar.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/utils/date.py` & `coretex-1.0.9/coretex/utils/date.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/utils/file.py` & `coretex-1.0.9/coretex/utils/file.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex/utils/number.py` & `coretex-1.0.9/coretex/utils/number.py`

 * *Files identical despite different names*

### Comparing `coretex-1.0.8/coretex.egg-info/PKG-INFO` & `coretex-1.0.9/coretex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coretex
-Version: 1.0.8
+Version: 1.0.9
 Summary: A package for AI experiment tracking, infrastructure and dataset management using Coretex.ai platform.
 Author-email: Duško Mirković <dmirkovic@coretex.ai>
 Maintainer-email: Duško Mirković <dmirkovic@coretex.ai>, Igor Perić <igor@coretex.ai>, Jovica Zarić <jzaric@coretex.ai>, Darko Zarić <dzaric@coretex.ai>, Bogdan Tintor <btintor@coretex.ai>, Alex Maslennikov <alex@coretex.ai>
 Project-URL: Homepage, https://coretex.ai
 Project-URL: Documentation, https://docs.coretex.ai/
 Project-URL: Python API, https://coretexpylib.coretex.ai/
 Project-URL: Source, https://github.com/coretex-ai/coretexpylib
```

### Comparing `coretex-1.0.8/coretex.egg-info/SOURCES.txt` & `coretex-1.0.9/coretex.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,15 @@
 coretex/nlp/text.py
 coretex/nlp/token.py
 coretex/nlp/transcriber.py
 coretex/nlp/transcription.py
 coretex/nlp/utils.py
 coretex/project/__init__.py
 coretex/project/base.py
-coretex/project/calculate_metrics.py
-coretex/project/heartbeat.py
+coretex/project/experiment_worker.py
 coretex/project/local.py
 coretex/project/remote.py
 coretex/qiime2/__init__.py
 coretex/qiime2/utils.py
 coretex/threading/__init__.py
 coretex/threading/threaded_data_processor.py
 coretex/utils/__init__.py
```

### Comparing `coretex-1.0.8/pyproject.toml` & `coretex-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "coretex"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" }
 ]
 maintainers = [
   { name="Duško Mirković", email="dmirkovic@coretex.ai" },
   { name="Igor Perić", email="igor@coretex.ai" },
   { name="Jovica Zarić", email="jzaric@coretex.ai" },
```

