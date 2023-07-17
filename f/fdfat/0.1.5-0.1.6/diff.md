# Comparing `tmp/fdfat-0.1.5.tar.gz` & `tmp/fdfat-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdfat-0.1.5.tar", last modified: Sun Jul 16 09:11:33 2023, max compression
+gzip compressed data, was "fdfat-0.1.6.tar", last modified: Mon Jul 17 04:03:55 2023, max compression
```

## Comparing `fdfat-0.1.5.tar` & `fdfat-0.1.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.531662 fdfat-0.1.5/
--rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.5/MANIFEST.in
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 09:11:33.531529 fdfat-0.1.5/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.5/README.md
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.527149 fdfat-0.1.5/fdfat/
--rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-16 09:11:32.000000 fdfat-0.1.5/fdfat/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528472 fdfat-0.1.5/fdfat/cfg/
--rw-r--r--   0 ryan       (501) staff       (20)     4734 2023-07-16 08:09:07.000000 fdfat-0.1.5/fdfat/cfg/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1986 2023-07-16 08:08:53.000000 fdfat-0.1.5/fdfat/cfg/default.yaml
--rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.5/fdfat/cfg/default_data.yaml
--rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.5/fdfat/cfg/yaml_utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528586 fdfat-0.1.5/fdfat/cli/
--rw-r--r--   0 ryan       (501) staff       (20)     1153 2023-07-16 08:01:18.000000 fdfat-0.1.5/fdfat/cli/__init__.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.528792 fdfat-0.1.5/fdfat/data/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.5/fdfat/data/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.5/fdfat/data/dataloader.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.529467 fdfat-0.1.5/fdfat/engine/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.5/fdfat/engine/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3014 2023-07-16 08:26:08.000000 fdfat-0.1.5/fdfat/engine/base.py
--rw-r--r--   0 ryan       (501) staff       (20)     3359 2023-07-16 08:36:51.000000 fdfat-0.1.5/fdfat/engine/exporter.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.529917 fdfat-0.1.5/fdfat/engine/loop/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.5/fdfat/engine/loop/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.5/fdfat/engine/loop/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.5/fdfat/engine/loop/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.5/fdfat/engine/loop/validator.py
--rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.5/fdfat/engine/tester.py
--rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.5/fdfat/engine/trainer.py
--rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.5/fdfat/engine/validator.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.530125 fdfat-0.1.5/fdfat/metric/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.5/fdfat/metric/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.5/fdfat/metric/metric.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.530617 fdfat-0.1.5/fdfat/nn/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.5/fdfat/nn/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     3902 2023-07-16 08:24:43.000000 fdfat-0.1.5/fdfat/nn/conv.py
--rw-r--r--   0 ryan       (501) staff       (20)     5072 2023-07-16 08:30:38.000000 fdfat-0.1.5/fdfat/nn/model.py
--rw-r--r--   0 ryan       (501) staff       (20)     5929 2023-07-16 08:28:43.000000 fdfat-0.1.5/fdfat/nn/module.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.531306 fdfat-0.1.5/fdfat/utils/
--rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.5/fdfat/utils/__init__.py
--rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.5/fdfat/utils/logger.py
--rw-r--r--   0 ryan       (501) staff       (20)     7722 2023-07-16 08:36:19.000000 fdfat-0.1.5/fdfat/utils/model_utils.py
--rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.5/fdfat/utils/pose_estimation.py
--rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.5/fdfat/utils/utils.py
-drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-16 09:11:33.527970 fdfat-0.1.5/fdfat.egg-info/
--rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/PKG-INFO
--rw-r--r--   0 ryan       (501) staff       (20)      918 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/SOURCES.txt
--rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/dependency_links.txt
--rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/entry_points.txt
--rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/requires.txt
--rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-16 09:11:33.000000 fdfat-0.1.5/fdfat.egg-info/top_level.txt
--rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.5/requirements.txt
--rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-16 09:11:33.531707 fdfat-0.1.5/setup.cfg
--rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.5/setup.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.292769 fdfat-0.1.6/
+-rw-r--r--   0 ryan       (501) staff       (20)      118 2023-07-16 04:39:56.000000 fdfat-0.1.6/MANIFEST.in
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 04:03:55.292637 fdfat-0.1.6/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)     2067 2023-07-13 09:39:58.000000 fdfat-0.1.6/README.md
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.287808 fdfat-0.1.6/fdfat/
+-rw-r--r--   0 ryan       (501) staff       (20)      239 2023-07-17 04:03:13.000000 fdfat-0.1.6/fdfat/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.288963 fdfat-0.1.6/fdfat/cfg/
+-rw-r--r--   0 ryan       (501) staff       (20)     4734 2023-07-16 08:09:07.000000 fdfat-0.1.6/fdfat/cfg/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1954 2023-07-17 03:59:33.000000 fdfat-0.1.6/fdfat/cfg/default.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)      116 2023-07-06 09:39:01.000000 fdfat-0.1.6/fdfat/cfg/default_data.yaml
+-rw-r--r--   0 ryan       (501) staff       (20)     3934 2023-07-11 11:08:58.000000 fdfat-0.1.6/fdfat/cfg/yaml_utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.289070 fdfat-0.1.6/fdfat/cli/
+-rw-r--r--   0 ryan       (501) staff       (20)     1337 2023-07-17 03:57:33.000000 fdfat-0.1.6/fdfat/cli/__init__.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.289300 fdfat-0.1.6/fdfat/data/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:58.000000 fdfat-0.1.6/fdfat/data/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4086 2023-07-16 06:03:32.000000 fdfat-0.1.6/fdfat/data/dataloader.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.290160 fdfat-0.1.6/fdfat/engine/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:52:47.000000 fdfat-0.1.6/fdfat/engine/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3061 2023-07-17 03:59:04.000000 fdfat-0.1.6/fdfat/engine/base.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3359 2023-07-16 13:11:02.000000 fdfat-0.1.6/fdfat/engine/exporter.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.290742 fdfat-0.1.6/fdfat/engine/loop/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-16 02:56:31.000000 fdfat-0.1.6/fdfat/engine/loop/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1922 2023-07-11 13:22:27.000000 fdfat-0.1.6/fdfat/engine/loop/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2814 2023-07-16 06:06:48.000000 fdfat-0.1.6/fdfat/engine/loop/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2233 2023-07-16 06:07:42.000000 fdfat-0.1.6/fdfat/engine/loop/validator.py
+-rw-r--r--   0 ryan       (501) staff       (20)     1532 2023-07-16 06:07:55.000000 fdfat-0.1.6/fdfat/engine/tester.py
+-rw-r--r--   0 ryan       (501) staff       (20)     6922 2023-07-16 03:23:10.000000 fdfat-0.1.6/fdfat/engine/trainer.py
+-rw-r--r--   0 ryan       (501) staff       (20)     2349 2023-07-16 03:16:12.000000 fdfat-0.1.6/fdfat/engine/validator.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.291002 fdfat-0.1.6/fdfat/metric/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:58:57.000000 fdfat-0.1.6/fdfat/metric/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)      809 2023-07-09 04:19:57.000000 fdfat-0.1.6/fdfat/metric/metric.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.291521 fdfat-0.1.6/fdfat/nn/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:57:26.000000 fdfat-0.1.6/fdfat/nn/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     3902 2023-07-16 08:24:43.000000 fdfat-0.1.6/fdfat/nn/conv.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5072 2023-07-16 08:30:38.000000 fdfat-0.1.6/fdfat/nn/model.py
+-rw-r--r--   0 ryan       (501) staff       (20)     5929 2023-07-16 08:28:43.000000 fdfat-0.1.6/fdfat/nn/module.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.292423 fdfat-0.1.6/fdfat/utils/
+-rw-r--r--   0 ryan       (501) staff       (20)        0 2023-07-02 01:59:34.000000 fdfat-0.1.6/fdfat/utils/__init__.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4013 2023-07-11 13:22:27.000000 fdfat-0.1.6/fdfat/utils/logger.py
+-rw-r--r--   0 ryan       (501) staff       (20)     7722 2023-07-16 08:36:19.000000 fdfat-0.1.6/fdfat/utils/model_utils.py
+-rw-r--r--   0 ryan       (501) staff       (20)     8029 2023-07-07 05:05:30.000000 fdfat-0.1.6/fdfat/utils/pose_estimation.py
+-rw-r--r--   0 ryan       (501) staff       (20)     4857 2023-07-13 08:42:53.000000 fdfat-0.1.6/fdfat/utils/utils.py
+drwxr-xr-x   0 ryan       (501) staff       (20)        0 2023-07-17 04:03:55.288489 fdfat-0.1.6/fdfat.egg-info/
+-rw-r--r--   0 ryan       (501) staff       (20)     3348 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/PKG-INFO
+-rw-r--r--   0 ryan       (501) staff       (20)      918 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/SOURCES.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        1 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/dependency_links.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       48 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/entry_points.txt
+-rw-r--r--   0 ryan       (501) staff       (20)      179 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/requires.txt
+-rw-r--r--   0 ryan       (501) staff       (20)        6 2023-07-17 04:03:55.000000 fdfat-0.1.6/fdfat.egg-info/top_level.txt
+-rw-r--r--   0 ryan       (501) staff       (20)     1110 2023-06-29 01:21:18.000000 fdfat-0.1.6/requirements.txt
+-rw-r--r--   0 ryan       (501) staff       (20)       38 2023-07-17 04:03:55.292827 fdfat-0.1.6/setup.cfg
+-rw-r--r--   0 ryan       (501) staff       (20)     2119 2023-07-16 05:53:56.000000 fdfat-0.1.6/setup.py
```

### Comparing `fdfat-0.1.5/PKG-INFO` & `fdfat-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.5/README.md` & `fdfat-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/cfg/__init__.py` & `fdfat-0.1.6/fdfat/cfg/__init__.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/cfg/default.yaml` & `fdfat-0.1.6/fdfat/cfg/default.yaml`

 * *Files 9% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 
 # data
 data: # path to dataset file, ie. face_synth.yaml
 workers: 8 # number of workers for dataloader
 aug: 0.5 # aug
 input: # input file path/url for prediction
 validation: val # validation target set in the data yaml, one of train, val, test
-pre_norm: true # normalize data in dataloader instead of normalizing right before feeding to model 
+pre_norm: True # normalize data in dataloader instead of normalizing right before feeding to model 
 
 # model
-model: # modelname
+model: LightWeightModel # modelname
 imgsz: 128 # size of input image as integer
-aux_pose: False # model with auxiliary pose esimation
+aux_pose: True # model with auxiliary pose esimation
 muliplier: 1.0 # model depth multiplier
 checkpoint: # target checkpoint to load
 
 # training
 resume: False # resume training
-epoch: 100 # number of training epoch
-patience: 15 # number of epoch to adjust lr if val loss is not improve
+epoch: 500 # number of training epoch
+patience: 10 # number of epoch to adjust lr if val loss is not improve
 warmup_epoch: 2 # number of epoch to warmup model using lr0, after that use lr
-optimizer: SGD # torch.optim class
+optimizer: NAdam # torch.optim class
 loss: L1Loss # torch.nn class
-lr: 0.01  # main learning rate (i.e. SGD=1E-2, Adam=1E-3)
-batch_size: 32 # batchsize
+lr: 0.001  # main learning rate (i.e. SGD=1E-2, Adam=1E-3)
+batch_size: 64 # batchsize
 lr0_factor: 0.01  # initial learning rate factor
 lre_factor: 0.1 # end_lr = current_lr*lr_factor at the end of the trainning
 device: cpu # target device, ie. cuda device=0 or device=0,1,2,3 or device=cpu
 dump_batch: 5 # write sample batch for debug
 save: True # save checkpoint and stats
 pin_memory: False # use pin memory for dataloader
 aux_pose_weight: 0.5 # loss weight for auxiliary pose esimation
@@ -49,10 +49,9 @@
 w_mount: 1.0
 w_purpil: 1.0
 
 # testing
 test_warmup: True # warming up model when testing
 
 # export
-export_format: onnx # torchscript, onnx, saved_model, tflite
-export_pose: false # export with aux pose estimation
-export_simplify: true # simplify onnx model using onnxsim
+export_format: tflite # torchscript, onnx, saved_model, tflite
+export_simplify: True # simplify onnx model using onnxsim
```

### Comparing `fdfat-0.1.5/fdfat/cfg/yaml_utils.py` & `fdfat-0.1.6/fdfat/cfg/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/data/dataloader.py` & `fdfat-0.1.6/fdfat/data/dataloader.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/base.py` & `fdfat-0.1.6/fdfat/engine/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
     def load_model(self, verbose=True, track_running_stats=False):
         LOGGER.info(f"Load model: {self.cfgs.model}")
         self.net = getattr(model, self.cfgs.model)(imgz=self.cfgs.imgsz, muliplier=self.cfgs.muliplier, pose_rotation=self.cfgs.aux_pose, track_running_stats=track_running_stats).to(self.cfgs.device)
         if verbose:
             _ = model_info(self.net, detailed=True, imgsz=self.cfgs.imgsz, device=self.cfgs.device)
 
-    def load_checkpoint(self, checkpoint):
+    def load_checkpoint(self, checkpoint, map_location='cpu'):
         if isinstance(checkpoint, str) or isinstance(checkpoint, Path):
-            checkpoint = torch.load(checkpoint)
+            checkpoint = torch.load(checkpoint, map_location=map_location)
         self.checkpoint = checkpoint
         self.net.load(checkpoint)
         self.start_epoch = checkpoint['epoch']
         self.best_epoch_loss = checkpoint['best_fit']
         self.best_epoch_no = checkpoint['best_epoch']
         LOGGER.info(f"Loaded checkpoint epoch {checkpoint['epoch']}")
```

### Comparing `fdfat-0.1.5/fdfat/engine/exporter.py` & `fdfat-0.1.6/fdfat/engine/exporter.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/loop/tester.py` & `fdfat-0.1.6/fdfat/engine/loop/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/loop/trainer.py` & `fdfat-0.1.6/fdfat/engine/loop/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/loop/validator.py` & `fdfat-0.1.6/fdfat/engine/loop/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/tester.py` & `fdfat-0.1.6/fdfat/engine/tester.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/trainer.py` & `fdfat-0.1.6/fdfat/engine/trainer.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/engine/validator.py` & `fdfat-0.1.6/fdfat/engine/validator.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/metric/metric.py` & `fdfat-0.1.6/fdfat/metric/metric.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/nn/conv.py` & `fdfat-0.1.6/fdfat/nn/conv.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/nn/model.py` & `fdfat-0.1.6/fdfat/nn/model.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/nn/module.py` & `fdfat-0.1.6/fdfat/nn/module.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/utils/logger.py` & `fdfat-0.1.6/fdfat/utils/logger.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/utils/model_utils.py` & `fdfat-0.1.6/fdfat/utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/utils/pose_estimation.py` & `fdfat-0.1.6/fdfat/utils/pose_estimation.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat/utils/utils.py` & `fdfat-0.1.6/fdfat/utils/utils.py`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/fdfat.egg-info/PKG-INFO` & `fdfat-0.1.6/fdfat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdfat
-Version: 0.1.5
+Version: 0.1.6
 Summary: Fast 6DoF Face Alignment and Tracking
 Home-page: https://github.com/RyanDam/Fast-6DoF-Face-Alignment-and-Tracking
 Author: RyanDam
 License: GPL-3.0
 Keywords: machine-learning,deep-learning,vision,ML,DL,AI
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fdfat-0.1.5/fdfat.egg-info/SOURCES.txt` & `fdfat-0.1.6/fdfat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/requirements.txt` & `fdfat-0.1.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `fdfat-0.1.5/setup.py` & `fdfat-0.1.6/setup.py`

 * *Files identical despite different names*

