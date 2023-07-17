# Comparing `tmp/bioval-0.1.1.6a0.tar.gz` & `tmp/bioval-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioval-0.1.1.6a0.tar", max compression
+gzip compressed data, was "bioval-0.1.1a0.tar", last modified: Mon Jun 19 17:27:25 2023, max compression
```

## Comparing `bioval-0.1.1.6a0.tar` & `bioval-0.1.1a0.tar`

### file list

```diff
@@ -1,22 +1,13 @@
--rw-r--r--   0        0        0     1073 2023-06-19 17:23:24.232839 bioval-0.1.1.6a0/LICENSE.txt
--rw-r--r--   0        0        0    11879 2023-06-19 18:47:57.081259 bioval-0.1.1.6a0/Readme.md
--rw-r--r--   0        0        0     6148 2023-02-22 10:13:08.338375 bioval-0.1.1.6a0/bioval/.DS_Store
--rw-r--r--   0        0        0     4096 2023-02-22 10:13:08.342375 bioval-0.1.1.6a0/bioval/._.DS_Store
--rw-r--r--   0        0        0        8 2023-02-17 13:44:38.645154 bioval-0.1.1.6a0/bioval/Readme.md
--rw-r--r--   0        0        0        0 2023-06-19 19:04:55.434787 bioval-0.1.1.6a0/bioval/__init__.py
--rw-r--r--   0        0        0        0 2023-02-17 13:44:38.693155 bioval-0.1.1.6a0/bioval/metrics/__init__.py
--rw-r--r--   0        0        0    46777 2023-07-17 13:55:11.685260 bioval-0.1.1.6a0/bioval/metrics/conditional_evaluation.py
--rw-r--r--   0        0        0        0 2023-02-17 13:44:38.737156 bioval-0.1.1.6a0/bioval/tests/__init__.py
--rw-r--r--   0        0        0     4627 2023-03-02 17:29:56.264221 bioval-0.1.1.6a0/bioval/tests/test_conditional_evaluation.py
--rw-r--r--   0        0        0     6148 2023-02-22 10:13:08.350375 bioval-0.1.1.6a0/bioval/tutorials/.DS_Store
--rw-r--r--   0        0        0     4096 2023-02-22 10:13:08.350375 bioval-0.1.1.6a0/bioval/tutorials/._.DS_Store
--rw-r--r--   0        0        0     8251 2023-02-22 10:13:08.354375 bioval-0.1.1.6a0/bioval/tutorials/conditional_gan.py
--rw-r--r--   0        0        0        0 2023-02-22 10:13:08.354375 bioval-0.1.1.6a0/bioval/tutorials/data/.placeholder
--rw-r--r--   0        0        0        1 2023-02-22 10:13:08.446376 bioval-0.1.1.6a0/bioval/tutorials/images/.placeholder
--rw-r--r--   0        0        0        0 2023-02-17 13:44:38.829157 bioval-0.1.1.6a0/bioval/utils/__init__.py
--rw-r--r--   0        0        0     2345 2023-03-02 17:29:56.348222 bioval-0.1.1.6a0/bioval/utils/aggregation.py
--rw-r--r--   0        0        0     6262 2023-04-19 18:03:39.266180 bioval-0.1.1.6a0/bioval/utils/distance.py
--rw-r--r--   0        0        0     1617 2023-03-02 17:29:56.428223 bioval-0.1.1.6a0/bioval/utils/gpu_manager.py
--rw-r--r--   0        0        0      678 2023-07-17 13:56:04.754021 bioval-0.1.1.6a0/pyproject.toml
--rw-r--r--   0        0        0    13157 1970-01-01 00:00:00.000000 bioval-0.1.1.6a0/setup.py
--rw-r--r--   0        0        0    12752 1970-01-01 00:00:00.000000 bioval-0.1.1.6a0/PKG-INFO
+drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 17:27:25.080159 bioval-0.1.1a0/
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1073 2023-06-19 17:23:24.000000 bioval-0.1.1a0/LICENSE.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1053 2023-06-19 17:27:25.080159 bioval-0.1.1a0/PKG-INFO
+-rw-rw----   0 bendidi   (5571) biofid   (50425)    10685 2023-06-19 17:23:24.000000 bioval-0.1.1a0/README.md
+drwxrwx---   0 bendidi   (5571) biofid   (50425)        0 2023-06-19 17:27:25.080159 bioval-0.1.1a0/bioval.egg-info/
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1053 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/PKG-INFO
+-rw-rw----   0 bendidi   (5571) biofid   (50425)      204 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/SOURCES.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)        1 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/dependency_links.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)       65 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/requires.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)        7 2023-06-19 17:27:24.000000 bioval-0.1.1a0/bioval.egg-info/top_level.txt
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     1460 2023-06-19 17:02:02.000000 bioval-0.1.1a0/pyproject.toml
+-rw-rw----   0 bendidi   (5571) biofid   (50425)       79 2023-06-19 17:27:25.084159 bioval-0.1.1a0/setup.cfg
+-rw-rw----   0 bendidi   (5571) biofid   (50425)     2078 2023-06-19 17:27:20.000000 bioval-0.1.1a0/setup.py
```

### Comparing `bioval-0.1.1.6a0/LICENSE.txt` & `bioval-0.1.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bioval-0.1.1.6a0/Readme.md` & `bioval-0.1.1a0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,26 @@
 # Bioval
 Bioval is a Python package made to provide a wrapper and an easy access to a collection of evaluation metrics for comparing the similarity of two tensors, adapted to different evaluation processes of generative models applied to biological images, and by extension to natural images. The package support unconditional comparison cases, in which we have no labels separating different classes/conditions, and also supports conditional comparisons, with metrics adapted to evaluating the appropriateness of the generated images to all the distributions of real conditions. The package also supports distance of generated conditions from the real negative control condition, used in most biological contexts.
 
 The package supports both images (with any number of channels) and encoded features of images. The compared tensors need to have the same shape. This package performs encoding of images using the InceptionV3 encoder pretrained on ImageNet dataset, but can also handle features encoded using different encoders.
 
-
-## Table of Content
-- [Bioval](#bioval)
-  * [Installation](#installation)
-    + [Installation from Pypip](#installation-from-pypip)
-    + [Installation from source](#installation-from-source)
-  * [Available Metrics](#available-metrics)
-    + [Overall KID/FID](#overall-kid-fid)
-    + [Intraclass KID/FID](#intraclass-kid-fid)
-    + [IntraClass Conditional Evaluation](#intraclass-conditional-evaluation)
-    + [InterClass Conditional Evaluation](#interclass-conditional-evaluation)
-    + [Distance from Control](#distance-from-control)
-  * [Usage settings](#usage-settings)
-    + [Aggregated](#aggregated)
-    + [Distributed](#distributed)
-  * [Quick Usage](#quick-usage)
-    + [Object Instanciation](#object-instanciation)
-    + [Input tensors](#input-tensors)
-    + [Aggregated Usage of the metrics](#aggregated-usage-of-the-metrics)
-  * [Contributing](#contributing)
-  * [License](#license)
-
 ## Installation
 
-### Installation from Pypip
-
-You can install the current alpha version through the command :
-
-```bash
-pip install bioval
-```
-
 ### Installation from source
 Bioval can be built using the following command (from the root of this package):
 
 ```bash
 poetry build
-pip install dist/bioval-{version_number}.tar.gz
+pip3 install dist/bioval-{version_number}.tar.gz
 ```
 
+### Installation from Pypip
+
+Pypip installation will be supported soon.
+
 ## Available Metrics
 The following evaluation metrics are available in Bioval:
 
 ### Overall KID/FID
 This metric measures the KID/FID between two tensors, while being agnostic to the classes and conditions. this metric returns the overall KID/FID score.
 
 ### Intraclass KID/FID
@@ -158,17 +132,14 @@
 # (H, W, C) or (I, F) or (F), where C is the number of channels, 
 # H is the height, and W is the width of the input image, and 
 # I the number of instances, and F is the number of features.
 
 # control array with 10 images and 3 channels
 control = torch.randn(10, 256, 256, 3)
 
-# control array with 10 images and 5 channels
-control = torch.randn(10, 256, 256, 5) # If control has 5 channels, array_1 and array_2 must also have 5 channels
-
 # control array with 1 image and 3 channels
 control = torch.randn(256, 256, 3)
 
 # control array with 10 images and an embedding of size 1024
 control = torch.randn(10, 1024)
 
 # control array with 1 image and an embedding of size 1024
@@ -177,26 +148,26 @@
 ```
 
 In the case where nb of channels in input images differs from 3 channels, each channel is encoded separately, and the embeddings of each channel are concatenated into one embedding. For example, if the input images have 5 channels, the output embedding will be of size 5*embedding_size.
 
 
 ### Aggregated Usage of the metrics
 
-Computing all the metrics for our input tensors can be done using our created instance of our object, and passing the input tensors to it. The first and second arrays are mandatory inputs with no default values.
+Computing all the metrics for our input tensors can be done using our created instance of our object, and passing the input tensors to it. 
 
 ```python
 
-output = topk(arr1, arr2)
+output = topk(arr1, arr2, k_range=[1, 5, 10, 20, 50, 100])
 ```
 
 The Object instance can be called with the following parameters:
 
-- arr1: The first input tensor, and a mandatory input. Can be of shape (N, I, H, W, C) or (N, H, W, C) or (N, I, F) or (N, F), where N is the number of classes/conditions, I is the number of instances, H is the height, W is the width, C is the number of channels, and F is the number of features.
+- arr1: The first input tensor. Can be of shape (N, I, H, W, C) or (N, H, W, C) or (N, I, F) or (N, F), where N is the number of classes/conditions, I is the number of instances, H is the height, W is the width, C is the number of channels, and F is the number of features.
 
-- arr2: The second input tensor, and a mandatory input. Can be of shape (N, I, H, W, C) or (N, H, W, C) or (N, I, F) or (N, F), where N is the number of classes/conditions, I is the number of instances, H is the height, W is the width, C is the number of channels, and F is the number of features. Array 1 and Array 2 must have the same shape.
+- arr2: The second input tensor. Can be of shape (N, I, H, W, C) or (N, H, W, C) or (N, I, F) or (N, F), where N is the number of classes/conditions, I is the number of instances, H is the height, W is the width, C is the number of channels, and F is the number of features. Array 1 and Array 2 must have the same shape.
 
 - control: The control tensor. Default is None when the distance from control metric is not of desired. When not None, it is a torch.Tensor object of shape (I, H, W, C) or (H, W, C) or (I, F) or (F), where C is the number of channels, H is the height, and W is the width of the input image, and I the number of instances, and F is the number of features.
 
 - k_range: The range of k values to use for the top-k similarity metrics. Default is [1, 5, 10]. If the range is bigger than the number of conditions, the range is truncated to the number of conditions. 
 
 - aggregated : Whether to use the aggregated (if True) or distributed metrics (if False). Default is True.
```

