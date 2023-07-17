# Comparing `tmp/fdfat-0.1.6.tar.gz` & `tmp/fdfat-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.6.tar", last modified: Mon Jul 17 04:03:55 2023, max compression
+gzip compressed data, was "fdfat-0.1.7.tar", last modified: Mon Jul 17 10:25:50 2023, max compression
```

## Comparing `fdfat-0.1.6.tar` & `fdfat-0.1.7.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.292769 fdfat-0.1.6/
--rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.6/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 04:03:55.292637 fdfat-0.1.6/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.6/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.287808 fdfat-0.1.6/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-17 04:03:13.000000 fdfat-0.1.6/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.288963 fdfat-0.1.6/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4734 2023-07-16 08:09:07.000000 fdfat-0.1.6/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1954 2023-07-17 03:59:33.000000 fdfat-0.1.6/fdfat/cfg/default.yaml
--rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.6/fdfat/cfg/default_data.yaml
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.6/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.289070 fdfat-0.1.6/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1337 2023-07-17 03:57:33.000000 fdfat-0.1.6/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.289300 fdfat-0.1.6/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.6/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.6/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.290160 fdfat-0.1.6/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.6/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3061 2023-07-17 03:59:04.000000 fdfat-0.1.6/fdfat/engine/base.py
--rw-r--r--   0 ryan       (501) staff       (20)     3359 2023-07-16 13:11:02.000000 fdfat-0.1.6/fdfat/engine/exporter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.290742 fdfat-0.1.6/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.6/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.6/fdfat/engine/loop/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.6/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.6/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.6/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.6/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.6/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.291002 fdfat-0.1.6/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.6/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.6/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.291521 fdfat-0.1.6/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.6/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3902 2023-07-16 08:24:43.000000 fdfat-0.1.6/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     5072 2023-07-16 08:30:38.000000 fdfat-0.1.6/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5929 2023-07-16 08:28:43.000000 fdfat-0.1.6/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.292423 fdfat-0.1.6/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.6/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.6/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7722 2023-07-16 08:36:19.000000 fdfat-0.1.6/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.6/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.6/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.288489 fdfat-0.1.6/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      918 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.6/requirements.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-17 04:03:55.292827 fdfat-0.1.6/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.6/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.897178 fdfat-0.1.7/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.7/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 10:25:50.897043 fdfat-0.1.7/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.7/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.890153 fdfat-0.1.7/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-17 10:25:10.000000 fdfat-0.1.7/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.891866 fdfat-0.1.7/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4734 2023-07-16 08:09:07.000000 fdfat-0.1.7/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1954 2023-07-17 03:59:33.000000 fdfat-0.1.7/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.7/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.7/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.892238 fdfat-0.1.7/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1337 2023-07-17 03:57:33.000000 fdfat-0.1.7/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.892504 fdfat-0.1.7/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.7/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4138 2023-07-17 08:12:15.000000 fdfat-0.1.7/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.893555 fdfat-0.1.7/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.7/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3109 2023-07-17 10:23:05.000000 fdfat-0.1.7/fdfat/engine/base.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3335 2023-07-17 09:38:40.000000 fdfat-0.1.7/fdfat/engine/exporter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.894339 fdfat-0.1.7/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.7/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.7/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2869 2023-07-17 09:49:49.000000 fdfat-0.1.7/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2317 2023-07-17 09:49:52.000000 fdfat-0.1.7/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.7/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6611 2023-07-17 09:54:14.000000 fdfat-0.1.7/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2169 2023-07-17 06:47:01.000000 fdfat-0.1.7/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.894649 fdfat-0.1.7/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.7/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.7/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.895522 fdfat-0.1.7/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.7/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3580 2023-07-17 10:21:41.000000 fdfat-0.1.7/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4444 2023-07-17 10:21:09.000000 fdfat-0.1.7/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5050 2023-07-17 09:44:34.000000 fdfat-0.1.7/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.896606 fdfat-0.1.7/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.7/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.7/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7948 2023-07-17 10:24:57.000000 fdfat-0.1.7/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.7/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.7/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 10:25:50.890854 fdfat-0.1.7/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      918 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-17 10:25:50.000000 fdfat-0.1.7/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.7/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-17 10:25:50.897230 fdfat-0.1.7/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.7/setup.py
```

### Comparing `fdfat-0.1.6/PKG-INFO` & `fdfat-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.6/README.md` & `fdfat-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/cfg/__init__.py` & `fdfat-0.1.7/fdfat/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/cfg/default.yaml` & `fdfat-0.1.7/fdfat/cfg/default.yaml`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.7/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/cli/__init__.py` & `fdfat-0.1.7/fdfat/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/data/dataloader.py` & `fdfat-0.1.7/fdfat/data/dataloader.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import torch
 from torch.utils.data import Dataset
 from torchvision import transforms
 import albumentations as A
 import cv2
 
 from fdfat.utils.pose_estimation import PoseEstimator
+from fdfat.utils.model_utils import normalize_tensor
 
 POSE_ROTAION_MED = np.array([-0.02234655,  0.28259986, -2.98499613])
 POSE_ROTATION_STD = np.array([0.87680358, 0.53386852, 0.25789746])
 
 def gen_bbox(lmk, scale=[1.4, 1.6], offset=0.2, square=True):
     bbox = np.array([np.min(lmk, 0), np.max(lmk, 0)])
     size = bbox[1, :] - bbox[0, :]
@@ -25,15 +26,15 @@
     offset_ab = (2*np.random.random(2)-1)*offset*size
 
     size = size*np.random.uniform(low=scale[0], high=scale[1], size=1)
     center = center + offset_ab
 
     return np.vstack([center-size/2, center+size/2])
 
-def read_data(img_path, lmk_scale=1.0, aug=None, imgsz=128, norm=True):
+def read_data(img_path, lmk_scale=1.0, aug=None, norm=True):
     img = Image.open(img_path)
     lmk_path = img_path.replace(".png", "_ldmks.txt")
     with open(lmk_path, 'r') as f:
         lmk = f.readlines()
         lmk = np.array([[float(n) for n in l.strip("\n").split(" ")] for l in lmk])
 
     bbox = gen_bbox(lmk)
@@ -45,33 +46,33 @@
     if aug is not None:
         transformed = aug(image=croped, keypoints=lmk)
         croped = transformed['image']
         lmk = transformed['keypoints']
         lmk = np.array(lmk)
 
     # normalize
-    lmk /= imgsz
+    lmk /= croped.shape[1]
     lmk -= 0.5
     lmk *= lmk_scale
     lmk = lmk.astype(np.float32)
 
     if norm:
-        croped = (croped / 127.5) - 1
+        croped = normalize_tensor(croped)
         croped = croped.astype(np.float32)
     else:
         croped.astype(np.uint8)
 
     return croped, lmk
 
 class LandmarkDataset(Dataset):
-    def __init__(self, cfgs, annotations_files, imgsz=128, aug=True, pose_rotation=False):
+    def __init__(self, cfgs, annotations_files, aug=True, pose_rotation=False):
         self.norm = cfgs.pre_norm
         self.img_paths = annotations_files
-        self.imgsz = imgsz
-        self.pose_rotation = pose_rotation
+        self.imgsz = cfgs.imgsz
+        self.pose_rotation = cfgs.aux_pose
 
         if aug:
             self.aug = A.Compose([
                 # A.HorizontalFlip(p=0.5), # wrong lmk idx
                 A.ToGray(p=0.2),
                 A.Rotate (limit=10, p=0.2),
                 A.RandomBrightnessContrast(p=0.2),
@@ -83,32 +84,32 @@
                     A.Defocus(p=0.1),
                     A.MotionBlur(p=.2),
                     A.MedianBlur(blur_limit=3, p=0.1),
                     A.Blur(blur_limit=3, p=0.1),
                 ], p=0.1),
                 A.ISONoise(p=0.2),
                 A.ImageCompression(quality_lower=50, quality_upper=90, p=0.5),
-                A.Resize(imgsz, imgsz)
+                A.Resize(self.imgsz, self.imgsz)
             ], keypoint_params=A.KeypointParams(format='xy', remove_invisible=False))
         else:
             self.aug = A.Compose([
-                A.Resize(imgsz, imgsz)
+                A.Resize(self.imgsz, self.imgsz)
             ], keypoint_params=A.KeypointParams(format='xy', remove_invisible=False))
         
         self.trans = transforms.ToTensor()
 
         print(f"Loaded {len(annotations_files)} samples")
 
     def __len__(self):
         return len(self.img_paths)
 
     def __getitem__(self, idx):
         img_path = self.img_paths[idx]
 
-        img, lmk = read_data(img_path, aug=self.aug, imgsz=self.imgsz, norm=self.norm)
+        img, lmk = read_data(img_path, aug=self.aug, norm=self.norm)
         
         if self.pose_rotation:
             estimator = PoseEstimator(self.imgsz, self.imgsz)
             lmk_denorm = (lmk + 0.5)*self.imgsz
             rot_vec, _ = estimator.solve(lmk_denorm[:68,:])
             rot_vec_norm = np.divide(rot_vec[:,0] - POSE_ROTAION_MED, POSE_ROTATION_STD*2)
```

### Comparing `fdfat-0.1.6/fdfat/engine/base.py` & `fdfat-0.1.7/fdfat/engine/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,18 +51,20 @@
 
     def load_database(self):
         raise NotImplementedError("Not implemented")
     
     def prepare(self):
         raise NotImplementedError("Not implemented")
 
-    def load_model(self, verbose=True, track_running_stats=False):
+    def load_model(self, verbose=True):
         LOGGER.info(f"Load model: {self.cfgs.model}")
-        self.net = getattr(model, self.cfgs.model)(imgz=self.cfgs.imgsz, muliplier=self.cfgs.muliplier, pose_rotation=self.cfgs.aux_pose, track_running_stats=track_running_stats).to(self.cfgs.device)
+        self.net = getattr(model, self.cfgs.model)(imgz=self.cfgs.imgsz, muliplier=self.cfgs.muliplier, pose_rotation=self.cfgs.aux_pose).to(self.cfgs.device)
         if verbose:
+            # need to call this before getting model info to prevent abnormal batchnorm
+            self.net.eval()
             _ = model_info(self.net, detailed=True, imgsz=self.cfgs.imgsz, device=self.cfgs.device)
 
     def load_checkpoint(self, checkpoint, map_location='cpu'):
         if isinstance(checkpoint, str) or isinstance(checkpoint, Path):
             checkpoint = torch.load(checkpoint, map_location=map_location)
         self.checkpoint = checkpoint
         self.net.load(checkpoint)
```

### Comparing `fdfat-0.1.6/fdfat/engine/exporter.py` & `fdfat-0.1.7/fdfat/engine/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from fdfat.utils.model_utils import preprocess, get_latest_opset
 from fdfat.utils.utils import render_lmk
 
 class ExportEngine(BaseEngine):
 
     def __init__(self, cfg_: Union[str, Path, Dict, SimpleNamespace]):
         super().__init__(cfg_)
-        self.load_model(track_running_stats=True) # prevent miss behaviour with batchnorm not in eval mode
+        self.load_model() # prevent miss behaviour with batchnorm not in eval mode
 
         self.target_checkpoint_path = self.cfgs.checkpoint if self.cfgs.checkpoint is not None else self.save_best
         self.load_checkpoint(self.target_checkpoint_path)
 
         self.net.eval()
 
     def export(self):
```

### Comparing `fdfat-0.1.6/fdfat/engine/loop/tester.py` & `fdfat-0.1.7/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/engine/loop/trainer.py` & `fdfat-0.1.7/fdfat/engine/loop/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from collections import defaultdict
 
 import torch
 
 from fdfat.utils.utils import LMK_PARTS, LMK_PART_NAMES, render_batch
 from fdfat import TQDM_BAR_FORMAT
 from fdfat.metric.metric import nme
+from fdfat.utils.model_utils import normalize_tensor
 
 def train_loop(cfgs, current_epoch, dataloader, model, loss_fn, optimizer, name="Train"):
     loss_dict = defaultdict(lambda: 0)
 
     if cfgs.lossw_enabled:
         loss_weight = torch.zeros((cfgs.batch_size, 70))
         all_weights = [
@@ -26,15 +27,15 @@
     num_batches = len(dataloader)
     pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
 
     model.train()
     for batch, (x, y) in pbar:
         x_device = x.to(cfgs.device, non_blocking=True)
         if not cfgs.pre_norm:
-            x_device = ((x_device / 127.5) - 1).type(torch.float32)
+            x_device = normalize_tensor(x_device).type(torch.float32)
         y_device = y.to(cfgs.device, non_blocking=True)
 
         pred = model(x_device)
 
         if cfgs.aux_pose:
             loss = loss_fn(pred, y_device[:,:-1])
```

### Comparing `fdfat-0.1.6/fdfat/engine/loop/validator.py` & `fdfat-0.1.7/fdfat/engine/loop/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 import tqdm
 import torch
 from collections import defaultdict
 
 from fdfat.utils.utils import LMK_PARTS, LMK_PART_NAMES, render_batch
 from fdfat import TQDM_BAR_FORMAT
 from fdfat.metric.metric import nme
+from fdfat.utils.model_utils import normalize_tensor
 
 def val_loop(cfgs, current_epoch, dataloader, model, loss_fn, name="Valid"):
-    loss_dict = defaultdict(lambda: 0)
 
-    num_batches = len(dataloader)
-    pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
-
-    model.eval()
     with torch.no_grad():
+        loss_dict = defaultdict(lambda: 0)
+
+        num_batches = len(dataloader)
+        pbar = tqdm.tqdm(enumerate(dataloader), total=num_batches, bar_format=TQDM_BAR_FORMAT)
+
+        model.eval()
         for batch, (x, y) in pbar:
             x_device = x.to(cfgs.device, non_blocking=True)
             if not cfgs.pre_norm:
-                x_device = ((x_device / 127.5) - 1).type(torch.float32)
+                x_device = normalize_tensor(x_device).type(torch.float32)
             y_device = y.to(cfgs.device, non_blocking=True)
 
             pred = model(x_device)
 
             if cfgs.aux_pose:
                 loss = loss_fn(pred, y_device[:,:-1])
                 pose_weight = y_device[:,-1:]
@@ -46,11 +48,11 @@
 
             pbar.set_description(f"{name} epoch [{current_epoch+1:3d}/{cfgs.epoch:3d}] {losses_str}")
 
             if current_epoch == 0 and batch < cfgs.dump_batch:
                 save_batch_png = cfgs.save_dir / f'{name}_batch{batch}.png'
                 render_batch(x_device.cpu().detach().numpy(), y_device[:,:70*2].cpu().detach().numpy(), save_batch_png)
 
-    for k in loss_dict.keys():
-        loss_dict[k] /= num_batches
+        for k in loss_dict.keys():
+            loss_dict[k] /= num_batches
 
-    return loss_dict
+        return loss_dict
```

### Comparing `fdfat-0.1.6/fdfat/engine/tester.py` & `fdfat-0.1.7/fdfat/engine/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/engine/trainer.py` & `fdfat-0.1.7/fdfat/engine/trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,28 +24,23 @@
     def __init__(self, cfg_: Union[str, Path, Dict, SimpleNamespace]):
         super().__init__(cfg_)
         self.load_database()
         self.load_model()
 
     def load_database(self):
         LOGGER.info("Load Train data")
-        self.dataset = LandmarkDataset(self.cfgs, read_file_list(self.cfgs.data.train, base_path=self.cfgs.data.base_path), 
-                                    imgsz=self.cfgs.imgsz, 
-                                    pose_rotation=self.cfgs.aux_pose)
+        self.dataset = LandmarkDataset(self.cfgs, read_file_list(self.cfgs.data.train, base_path=self.cfgs.data.base_path))
         self.train_dataloader = DataLoader(self.dataset, batch_size=self.cfgs.batch_size, shuffle=True, 
                                         pin_memory=self.cfgs.pin_memory,
                                         num_workers=self.cfgs.workers,
                                         persistent_workers=True,
                                         multiprocessing_context="spawn")
 
         LOGGER.info("Load Val data")
-        self.dataset_test = LandmarkDataset(self.cfgs, read_file_list(self.cfgs.data.val, base_path=self.cfgs.data.base_path), 
-                                        imgsz=self.cfgs.imgsz, 
-                                        pose_rotation=self.cfgs.aux_pose, 
-                                        aug=False)
+        self.dataset_test = LandmarkDataset(self.cfgs, read_file_list(self.cfgs.data.val, base_path=self.cfgs.data.base_path), aug=False)
         self.test_dataloader = DataLoader(self.dataset_test, batch_size=self.cfgs.batch_size, shuffle=False,
                                         pin_memory=self.cfgs.pin_memory,
                                         num_workers=self.cfgs.workers,
                                         persistent_workers=True,
                                         multiprocessing_context="spawn")
```

### Comparing `fdfat-0.1.6/fdfat/engine/validator.py` & `fdfat-0.1.7/fdfat/engine/validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,18 +27,15 @@
         if self.cfgs.validation == "train":
             self.target_data_path = self.cfgs.data.train
         elif self.cfgs.validation == "test":
             self.target_data_path = self.cfgs.data.test
 
         LOGGER.info(f"Load {self.cfgs.validation} data")
 
-        self.dataset = LandmarkDataset(self.cfgs, read_file_list(self.target_data_path, base_path=self.cfgs.data.base_path), 
-                                        imgsz=self.cfgs.imgsz, 
-                                        pose_rotation=self.cfgs.aux_pose, 
-                                        aug=False)
+        self.dataset = LandmarkDataset(self.cfgs, read_file_list(self.target_data_path, base_path=self.cfgs.data.base_path), aug=False)
         self.dataloader = DataLoader(self.dataset, batch_size=self.cfgs.batch_size, shuffle=False,
                                         pin_memory=self.cfgs.pin_memory,
                                         num_workers=self.cfgs.workers,
                                         persistent_workers=True,
                                         multiprocessing_context="spawn")
         
         LOGGER.info("Load database DONE")
```

### Comparing `fdfat-0.1.6/fdfat/metric/metric.py` & `fdfat-0.1.7/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/nn/conv.py` & `fdfat-0.1.7/fdfat/nn/conv.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 def initialize_weights(model):
     """Initialize model weights to random values."""
     for m in model.modules():
         t = type(m)
         if t is nn.Conv2d:
             pass  # nn.init.kaiming_normal_(m.weight, mode='fan_out', nonlinearity='relu')
         elif t is nn.BatchNorm2d:
-            m.eps = 1e-3
+            m.eps = 1e-5
             m.momentum = 0.03
-            m.track_running_stats=False
         elif t in [nn.Hardswish, nn.LeakyReLU, nn.ReLU, nn.ReLU6, nn.SiLU]:
             m.inplace = True
 
 def autopad(k, p=None, d=1):  # kernel, padding, dilation
     """Pad to 'same' shape outputs."""
     if d > 1:
         k = d * (k - 1) + 1 if isinstance(k, int) else [d * (x - 1) + 1 for x in k]  # actual kernel-size
@@ -26,36 +25,36 @@
         p = k // 2 if isinstance(k, int) else [x // 2 for x in k]  # auto-pad
     return p
 
 class Conv(nn.Module):
     """Standard convolution with args(ch_in, ch_out, kernel, stride, padding, groups, dilation, activation)."""
     default_act = nn.SiLU()  # default activation
 
-    def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True, track_running_stats=False):
+    def __init__(self, c1, c2, k=1, s=1, p=None, g=1, d=1, act=True):
         """Initialize Conv layer with given arguments including activation."""
         super().__init__()
         self.conv = nn.Conv2d(c1, c2, k, s, autopad(k, p, d), groups=g, dilation=d, bias=False)
-        self.bn = nn.BatchNorm2d(c2, track_running_stats=track_running_stats)
+        self.bn = nn.BatchNorm2d(c2)
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
 
-        initialize_weights(self)
+        # initialize_weights(self)
 
     def forward(self, x):
         """Apply convolution, batch normalization and activation to input tensor."""
         return self.act(self.bn(self.conv(x)))
 
     def forward_fuse(self, x):
         """Perform transposed convolution of 2D data."""
         return self.act(self.conv(x))
     
 class DWConv(Conv):
     """Depth-wise convolution."""
 
-    def __init__(self, c1, c2, k=1, s=1, d=1, act=True, track_running_stats=False):  # ch_in, ch_out, kernel, stride, dilation, activation
-        super().__init__(c1, c2, k, s, g=math.gcd(c1, c2), d=d, act=act, track_running_stats=track_running_stats)
+    def __init__(self, c1, c2, k=1, s=1, d=1, act=True):  # ch_in, ch_out, kernel, stride, dilation, activation
+        super().__init__(c1, c2, k, s, g=math.gcd(c1, c2), d=d, act=act)
 
 class Concat(nn.Module):
     """Concatenate a list of tensors along dimension."""
 
     def __init__(self, dimension=1):
         """Concatenates a list of tensors along a specified dimension."""
         super().__init__()
@@ -66,36 +65,36 @@
         return torch.cat(x, self.d)
 
 
 class IdentifyBlock(nn.Module):
 
     default_act = nn.ReLU6()  # default activation
 
-    def __init__(self, in_ch, out_ch, expand, k=3, act=True, stride=1, dilation_rate=1, track_running_stats=False):
+    def __init__(self, in_ch, out_ch, expand, k=3, act=True, stride=1, dilation_rate=1):
         super().__init__()
 
         self.act = self.default_act if act is True else act if isinstance(act, nn.Module) else nn.Identity()
         
         expand_ch = int(expand*in_ch)
 
         # expansion
-        self.conv1 = Conv(in_ch, expand_ch, k=1, act=self.act, track_running_stats=track_running_stats)
+        self.conv1 = Conv(in_ch, expand_ch, k=1, act=self.act)
 
         # depthwise
-        self.conv2 = DWConv(expand_ch, expand_ch, k=k, s=stride, d=dilation_rate, act=self.act, track_running_stats=track_running_stats)
+        self.conv2 = DWConv(expand_ch, expand_ch, k=k, s=stride, d=dilation_rate, act=self.act)
 
         # squeeze
-        self.conv3 = Conv(expand_ch, out_ch, k=1, act=False, track_running_stats=track_running_stats)
+        self.conv3 = Conv(expand_ch, out_ch, k=1, act=False)
 
         self.need_fuse = in_ch == out_ch
         self.need_pool = stride == 2
         if self.need_fuse and self.need_pool:
             self.pool = nn.MaxPool2d(2, stride=2)
 
-        initialize_weights(self)
+        # initialize_weights(self)
 
     def forward(self, x):
         
         ex = self.conv1(x)
         de = self.conv2(ex)
         sq = self.conv3(de)
```

### Comparing `fdfat-0.1.6/fdfat/utils/logger.py` & `fdfat-0.1.7/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/utils/model_utils.py` & `fdfat-0.1.7/fdfat/utils/model_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,15 @@
     #     return 0
     
 def init_seeds(seed=0, deterministic=False):
     """Initialize random number generator (RNG) seeds https://pytorch.org/docs/stable/notes/randomness.html."""
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
+    torch.mps.manual_seed(seed)  # for Multi-GPU, exception safe
     torch.cuda.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)  # for Multi-GPU, exception safe
     # torch.backends.cudnn.benchmark = True  # AutoBatch problem https://github.com/ultralytics/yolov5/issues/9287
     if deterministic:  # https://github.com/ultralytics/yolov5/pull/8213
         if TORCH_2_0:
             torch.use_deterministic_algorithms(True)
             torch.backends.cudnn.deterministic = True
@@ -143,14 +144,19 @@
 
 def intersect_dicts(da, db, exclude=()):
     """Returns a dictionary of intersecting keys with matching shapes, excluding 'exclude' keys, using da values."""
     return {k: v for k, v in da.items() if k in db and all(x not in k for x in exclude) and v.shape == db[k].shape}
 
 def preprocess(img_pil, imgsz):
     img_pil = img_pil.resize((imgsz, imgsz))
-    img_np = np.array(img_pil)/127.5 - 1
+    img_np = normalize_tensor(np.array(img_pil))
     img_np = np.transpose(img_np, [2, 0, 1])[np.newaxis, ...]
     return img_np
 
+def normalize_tensor(tensor):
+    return tensor/127.5 - 1
+    # return tensor/255
+    # return (tensor/255 - 0.44531356896770125 ) / 0.2692461874154524
+
 def get_latest_opset():
     """Return second-most (for maturity) recently supported ONNX opset by this version of torch."""
     return max(int(k[14:]) for k in vars(torch.onnx) if 'symbolic_opset' in k) - 1  # opset
```

### Comparing `fdfat-0.1.6/fdfat/utils/pose_estimation.py` & `fdfat-0.1.7/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat/utils/utils.py` & `fdfat-0.1.7/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.7/fdfat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.6
+Version: 0.1.7
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.6/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.7/fdfat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/requirements.txt` & `fdfat-0.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.6/setup.py` & `fdfat-0.1.7/setup.py`

 * *Files identical despite different names*

