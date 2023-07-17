# Comparing `tmp/lightningdata-modules-0.1.8.tar.gz` & `tmp/lightningdata-modules-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightningdata-modules-0.1.8.tar", last modified: Mon Jun 12 08:28:01 2023, max compression
+gzip compressed data, was "lightningdata-modules-0.1.9.tar", last modified: Mon Jul 17 10:01:41 2023, max compression
```

## Comparing `lightningdata-modules-0.1.8.tar` & `lightningdata-modules-0.1.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.194669 lightningdata-modules-0.1.8/
--rw-rw-rw-   0        0        0     2468 2023-06-12 08:28:01.193669 lightningdata-modules-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1799 2023-06-12 08:20:57.000000 lightningdata-modules-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.078671 lightningdata-modules-0.1.8/lightningdata/
--rw-rw-rw-   0        0        0     1461 2023-04-17 07:40:15.000000 lightningdata-modules-0.1.8/lightningdata/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.084668 lightningdata-modules-0.1.8/lightningdata/common/
--rw-rw-rw-   0        0        0        0 2022-02-02 14:20:15.000000 lightningdata-modules-0.1.8/lightningdata/common/__init__.py
--rw-rw-rw-   0        0        0      550 2023-04-17 07:36:40.000000 lightningdata-modules-0.1.8/lightningdata/common/config.py
--rw-rw-rw-   0        0        0     4976 2023-04-18 12:22:44.000000 lightningdata-modules-0.1.8/lightningdata/common/folder2lmdb.py
--rw-rw-rw-   0        0        0     8727 2022-02-14 12:32:07.000000 lightningdata-modules-0.1.8/lightningdata/common/pre_process.py
--rw-rw-rw-   0        0        0     2395 2022-02-15 15:32:32.000000 lightningdata-modules-0.1.8/lightningdata/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.086669 lightningdata-modules-0.1.8/lightningdata/modules/
--rw-rw-rw-   0        0        0        0 2022-02-11 08:08:08.000000 lightningdata-modules-0.1.8/lightningdata/modules/__init__.py
--rw-rw-rw-   0        0        0     2241 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/modules/datamodule_base.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.095667 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/
--rw-rw-rw-   0        0        0        0 2022-02-09 11:07:33.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/__init__.py
--rw-rw-rw-   0        0        0     1346 2022-02-21 13:22:43.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/digit5_datamodule.py
--rw-rw-rw-   0        0        0     8577 2023-04-18 12:36:07.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
--rw-rw-rw-   0        0        0     1394 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
--rw-rw-rw-   0        0        0     1363 2023-04-18 12:39:48.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/office31_datamodule.py
--rw-rw-rw-   0        0        0     1405 2022-02-21 13:22:15.000000 lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.098668 lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/
--rw-rw-rw-   0        0        0        0 2022-02-10 14:34:26.000000 lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/__init__.py
--rw-rw-rw-   0        0        0     1048 2022-02-11 09:46:51.000000 lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/emnist_datamodule.py
--rw-rw-rw-   0        0        0     3966 2022-11-09 12:58:43.000000 lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/federatedLearning_base.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.103669 lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/
--rw-rw-rw-   0        0        0        0 2022-04-12 08:56:02.000000 lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/__init__.py
--rw-rw-rw-   0        0        0     3378 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/metaLearning_base.py
--rw-rw-rw-   0        0        0     2181 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
--rw-rw-rw-   0        0        0     2156 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/omiglot_datamodule.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.104670 lightningdata-modules-0.1.8/lightningdata/thirdparty/
--rw-rw-rw-   0        0        0        0 2022-11-09 14:16:25.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.106670 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/
--rw-rw-rw-   0        0        0      352 2022-11-09 14:09:26.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.129669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/
--rw-rw-rw-   0        0        0     1620 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/__init__.py
--rw-rw-rw-   0        0        0    19222 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/bach.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.133669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/
--rw-rw-rw-   0        0        0      195 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
--rw-rw-rw-   0        0        0     6861 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
--rw-rw-rw-   0        0        0     5332 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
--rw-rw-rw-   0        0        0     5708 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
--rw-rw-rw-   0        0        0    10048 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cub.py
--rw-rw-rw-   0        0        0    10334 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
--rw-rw-rw-   0        0        0    14448 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/helpers.py
--rw-rw-rw-   0        0        0     6522 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
--rw-rw-rw-   0        0        0    11646 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/letter.py
--rw-rw-rw-   0        0        0     9242 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
--rw-rw-rw-   0        0        0    11285 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
--rw-rw-rw-   0        0        0    14763 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
--rw-rw-rw-   0        0        0    14686 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
--rw-rw-rw-   0        0        0    14786 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
--rw-rw-rw-   0        0        0    10004 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
--rw-rw-rw-   0        0        0    21872 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/tcga.py
--rw-rw-rw-   0        0        0    10696 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
--rw-rw-rw-   0        0        0    10345 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
--rw-rw-rw-   0        0        0     1975 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.146669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/
--rw-rw-rw-   0        0        0     1100 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/__init__.py
--rw-rw-rw-   0        0        0     2576 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/activation.py
--rw-rw-rw-   0        0        0     2301 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
--rw-rw-rw-   0        0        0      736 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/container.py
--rw-rw-rw-   0        0        0     1149 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/conv.py
--rw-rw-rw-   0        0        0      786 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/linear.py
--rw-rw-rw-   0        0        0     2437 2022-11-09 13:14:11.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/module.py
--rw-rw-rw-   0        0        0      555 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/normalization.py
--rw-rw-rw-   0        0        0     2091 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/parallel.py
--rw-rw-rw-   0        0        0     1084 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/sparse.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.151670 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/
--rw-rw-rw-   0        0        0      345 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/__init__.py
--rw-rw-rw-   0        0        0     5592 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/harmonic.py
--rw-rw-rw-   0        0        0     4121 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/helpers.py
--rw-rw-rw-   0        0        0     4744 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
--rw-rw-rw-   0        0        0     6312 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.162669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/
--rw-rw-rw-   0        0        0      556 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/__init__.py
--rw-rw-rw-   0        0        0     2589 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
--rw-rw-rw-   0        0        0     2748 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/categorical.py
--rw-rw-rw-   0        0        0    16328 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/splitters.py
--rw-rw-rw-   0        0        0      555 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
--rw-rw-rw-   0        0        0     1325 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
--rw-rw-rw-   0        0        0     1139 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.168669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/
--rw-rw-rw-   0        0        0      843 2022-11-09 14:09:46.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.175669 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/
--rw-rw-rw-   0        0        0      818 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
--rw-rw-rw-   0        0        0     2651 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
--rw-rw-rw-   0        0        0    13806 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
--rw-rw-rw-   0        0        0     2113 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
--rw-rw-rw-   0        0        0     2190 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/task.py
--rw-rw-rw-   0        0        0     3129 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
--rw-rw-rw-   0        0        0     2330 2022-11-09 14:09:55.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
--rw-rw-rw-   0        0        0     7624 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/matching.py
--rw-rw-rw-   0        0        0     4277 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/metrics.py
--rw-rw-rw-   0        0        0     2832 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/prototype.py
--rw-rw-rw-   0        0        0     4966 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/r2d2.py
--rw-rw-rw-   0        0        0       17 2022-11-09 13:14:09.000000 lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/version.py
-drwxrwxrwx   0        0        0        0 2023-06-12 08:28:01.192667 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/
--rw-rw-rw-   0        0        0     2468 2023-06-12 08:28:00.000000 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4581 2023-06-12 08:28:01.000000 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 08:28:00.000000 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      100 2023-06-12 08:28:00.000000 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 08:28:00.000000 lightningdata-modules-0.1.8/lightningdata_modules.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 08:28:01.194669 lightningdata-modules-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1175 2023-06-12 08:27:56.000000 lightningdata-modules-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.558100 lightningdata-modules-0.1.9/
+-rw-rw-rw-   0        0        0     2468 2023-07-17 10:01:41.557099 lightningdata-modules-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1799 2023-06-12 08:20:57.000000 lightningdata-modules-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.457097 lightningdata-modules-0.1.9/lightningdata/
+-rw-rw-rw-   0        0        0     1461 2023-04-17 07:40:15.000000 lightningdata-modules-0.1.9/lightningdata/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.463099 lightningdata-modules-0.1.9/lightningdata/common/
+-rw-rw-rw-   0        0        0        0 2022-02-02 14:20:15.000000 lightningdata-modules-0.1.9/lightningdata/common/__init__.py
+-rw-rw-rw-   0        0        0      550 2023-04-17 07:36:40.000000 lightningdata-modules-0.1.9/lightningdata/common/config.py
+-rw-rw-rw-   0        0        0     4976 2023-04-18 12:22:44.000000 lightningdata-modules-0.1.9/lightningdata/common/folder2lmdb.py
+-rw-rw-rw-   0        0        0     8727 2022-02-14 12:32:07.000000 lightningdata-modules-0.1.9/lightningdata/common/pre_process.py
+-rw-rw-rw-   0        0        0     2395 2022-02-15 15:32:32.000000 lightningdata-modules-0.1.9/lightningdata/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.465101 lightningdata-modules-0.1.9/lightningdata/modules/
+-rw-rw-rw-   0        0        0        0 2022-02-11 08:08:08.000000 lightningdata-modules-0.1.9/lightningdata/modules/__init__.py
+-rw-rw-rw-   0        0        0     2241 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/modules/datamodule_base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.471103 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/
+-rw-rw-rw-   0        0        0        0 2022-02-09 11:07:33.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/__init__.py
+-rw-rw-rw-   0        0        0     1346 2022-02-21 13:22:43.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/digit5_datamodule.py
+-rw-rw-rw-   0        0        0     8577 2023-04-18 12:36:07.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/domainAdaptation_base.py
+-rw-rw-rw-   0        0        0     1394 2022-02-21 13:23:46.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/domainNet_datamodule.py
+-rw-rw-rw-   0        0        0     1363 2023-04-18 12:39:48.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/office31_datamodule.py
+-rw-rw-rw-   0        0        0     1405 2022-02-21 13:22:15.000000 lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/officeHome_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.475101 lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/
+-rw-rw-rw-   0        0        0        0 2022-02-10 14:34:26.000000 lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/__init__.py
+-rw-rw-rw-   0        0        0     1048 2022-02-11 09:46:51.000000 lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/emnist_datamodule.py
+-rw-rw-rw-   0        0        0     3966 2022-11-09 12:58:43.000000 lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/federatedLearning_base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.480103 lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/
+-rw-rw-rw-   0        0        0        0 2022-04-12 08:56:02.000000 lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/__init__.py
+-rw-rw-rw-   0        0        0     3378 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/metaLearning_base.py
+-rw-rw-rw-   0        0        0     2181 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py
+-rw-rw-rw-   0        0        0     2156 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/omiglot_datamodule.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.481104 lightningdata-modules-0.1.9/lightningdata/thirdparty/
+-rw-rw-rw-   0        0        0        0 2022-11-09 14:16:25.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.483103 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/
+-rw-rw-rw-   0        0        0      352 2022-11-09 14:09:26.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.504100 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/
+-rw-rw-rw-   0        0        0     1620 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/__init__.py
+-rw-rw-rw-   0        0        0    19222 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/bach.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.509101 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/
+-rw-rw-rw-   0        0        0      195 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/__init__.py
+-rw-rw-rw-   0        0        0     6861 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py
+-rw-rw-rw-   0        0        0     5332 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py
+-rw-rw-rw-   0        0        0     5708 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py
+-rw-rw-rw-   0        0        0    10048 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cub.py
+-rw-rw-rw-   0        0        0    10334 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py
+-rw-rw-rw-   0        0        0    14448 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/helpers.py
+-rw-rw-rw-   0        0        0     6522 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py
+-rw-rw-rw-   0        0        0    11646 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/letter.py
+-rw-rw-rw-   0        0        0     9242 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py
+-rw-rw-rw-   0        0        0    11285 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/omniglot.py
+-rw-rw-rw-   0        0        0    14763 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py
+-rw-rw-rw-   0        0        0    14686 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py
+-rw-rw-rw-   0        0        0    14786 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py
+-rw-rw-rw-   0        0        0    10004 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py
+-rw-rw-rw-   0        0        0    21872 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/tcga.py
+-rw-rw-rw-   0        0        0    10696 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py
+-rw-rw-rw-   0        0        0    10345 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py
+-rw-rw-rw-   0        0        0     1975 2023-04-17 07:35:57.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.521099 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/
+-rw-rw-rw-   0        0        0     1100 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/__init__.py
+-rw-rw-rw-   0        0        0     2576 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/activation.py
+-rw-rw-rw-   0        0        0     2301 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/batchnorm.py
+-rw-rw-rw-   0        0        0      736 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/container.py
+-rw-rw-rw-   0        0        0     1149 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/conv.py
+-rw-rw-rw-   0        0        0      786 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/linear.py
+-rw-rw-rw-   0        0        0     2437 2022-11-09 13:14:11.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/module.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/normalization.py
+-rw-rw-rw-   0        0        0     2091 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/parallel.py
+-rw-rw-rw-   0        0        0     1084 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/sparse.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.526100 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/
+-rw-rw-rw-   0        0        0      345 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/__init__.py
+-rw-rw-rw-   0        0        0     5592 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/harmonic.py
+-rw-rw-rw-   0        0        0     4121 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/helpers.py
+-rw-rw-rw-   0        0        0     4744 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/sinusoid.py
+-rw-rw-rw-   0        0        0     6312 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.534100 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/
+-rw-rw-rw-   0        0        0      556 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/__init__.py
+-rw-rw-rw-   0        0        0     2589 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/augmentations.py
+-rw-rw-rw-   0        0        0     2748 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/categorical.py
+-rw-rw-rw-   0        0        0    16328 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/splitters.py
+-rw-rw-rw-   0        0        0      555 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py
+-rw-rw-rw-   0        0        0     1325 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py
+-rw-rw-rw-   0        0        0     1139 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.541101 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/
+-rw-rw-rw-   0        0        0      843 2022-11-09 14:09:46.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.548098 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/
+-rw-rw-rw-   0        0        0      818 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/__init__.py
+-rw-rw-rw-   0        0        0     2651 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py
+-rw-rw-rw-   0        0        0    13806 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/dataset.py
+-rw-rw-rw-   0        0        0     2113 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/sampler.py
+-rw-rw-rw-   0        0        0     2190 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/task.py
+-rw-rw-rw-   0        0        0     3129 2022-11-09 14:04:34.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py
+-rw-rw-rw-   0        0        0     2330 2022-11-09 14:09:55.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/gradient_based.py
+-rw-rw-rw-   0        0        0     7624 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/matching.py
+-rw-rw-rw-   0        0        0     4277 2022-11-09 14:10:27.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/metrics.py
+-rw-rw-rw-   0        0        0     2832 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/prototype.py
+-rw-rw-rw-   0        0        0     4966 2022-11-09 13:14:12.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/r2d2.py
+-rw-rw-rw-   0        0        0       17 2022-11-09 13:14:09.000000 lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/version.py
+drwxrwxrwx   0        0        0        0 2023-07-17 10:01:41.556100 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/
+-rw-rw-rw-   0        0        0     2468 2023-07-17 10:01:41.000000 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4581 2023-07-17 10:01:41.000000 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 10:01:41.000000 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      117 2023-07-17 10:01:41.000000 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 10:01:41.000000 lightningdata-modules-0.1.9/lightningdata_modules.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 10:01:41.558100 lightningdata-modules-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-07-17 09:55:14.000000 lightningdata-modules-0.1.9/setup.py
```

### Comparing `lightningdata-modules-0.1.8/PKG-INFO` & `lightningdata-modules-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.8/README.md` & `lightningdata-modules-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/common/config.py` & `lightningdata-modules-0.1.9/lightningdata/common/config.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/common/folder2lmdb.py` & `lightningdata-modules-0.1.9/lightningdata/common/folder2lmdb.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/common/pre_process.py` & `lightningdata-modules-0.1.9/lightningdata/common/pre_process.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/common/utils.py` & `lightningdata-modules-0.1.9/lightningdata/common/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/datamodule_base.py` & `lightningdata-modules-0.1.9/lightningdata/modules/datamodule_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/digit5_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/digit5_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/domainAdaptation_base.py` & `lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/domainAdaptation_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/domainNet_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/domainNet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/office31_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/office31_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/domain_adaptation/officeHome_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/domain_adaptation/officeHome_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/emnist_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/emnist_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/federated_learning/federatedLearning_base.py` & `lightningdata-modules-0.1.9/lightningdata/modules/federated_learning/federatedLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/metaLearning_base.py` & `lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/metaLearning_base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/mini_imagenet_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/modules/meta_learning/omiglot_datamodule.py` & `lightningdata-modules-0.1.9/lightningdata/modules/meta_learning/omiglot_datamodule.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/bach.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/bach.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/base.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/cifar_fs.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cifar100/fc100.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/cub.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/cub.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/doublemnist.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/helpers.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/helpers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/helpers_tabular.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/letter.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/letter.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/miniimagenet.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/omniglot.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/omniglot.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_margin.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_shape.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/one_hundred_plants_texture.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/pascal5i.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/tcga.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/tcga.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/tieredimagenet.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/triplemnist.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/datasets/utils.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/activation.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/activation.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/batchnorm.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/container.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/container.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/conv.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/conv.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/linear.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/linear.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/module.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/module.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/normalization.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/normalization.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/parallel.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/parallel.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/modules/sparse.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/modules/sparse.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/harmonic.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/harmonic.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/helpers.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/helpers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/sinusoid.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/sinusoid.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/toy/sinusoid_line.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/augmentations.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/augmentations.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/categorical.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/categorical.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/splitters.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/splitters.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/tabular_transforms.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/target_transforms.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/transforms/utils.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/transforms/utils.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/__init__.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/dataset.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/dataset.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/sampler.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/sampler.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/task.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/task.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/data/wrappers.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/gradient_based.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/gradient_based.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/matching.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/matching.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/metrics.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/prototype.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/prototype.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata/thirdparty/torchmeta/utils/r2d2.py` & `lightningdata-modules-0.1.9/lightningdata/thirdparty/torchmeta/utils/r2d2.py`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/lightningdata_modules.egg-info/PKG-INFO` & `lightningdata-modules-0.1.9/lightningdata_modules.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightningdata-modules
-Version: 0.1.8
+Version: 0.1.9
 Summary: Pre-packages Pytorch-Lightning datasets
 Home-page: https://github.com/ManuelRoeder/lightningdata-modules
 Author: Manuel Roeder
 Author-email: manuel.roeder@web.de
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lightningdata-modules-0.1.8/lightningdata_modules.egg-info/SOURCES.txt` & `lightningdata-modules-0.1.9/lightningdata_modules.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightningdata-modules-0.1.8/setup.py` & `lightningdata-modules-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 required_packages = [
     "getfilelistpy", "lmdb", "matplotlib", "numpy", "Pillow", "pytorch_lightning", "setuptools",
-    "six", "torch", "torchvision", "py7zr"
+    "six", "torch", "torchvision", "py7zr", "h5py", "ordered-set"
 ]
 
 setup(
     name="lightningdata-modules",
-    version="0.1.8",
+    version="0.1.9",
     description="Pre-packages Pytorch-Lightning datasets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ManuelRoeder/lightningdata-modules",
     author="Manuel Roeder",
     author_email="manuel.roeder@web.de",
     license="MIT",
```

