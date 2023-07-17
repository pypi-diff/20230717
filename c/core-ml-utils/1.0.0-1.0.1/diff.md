# Comparing `tmp/core-ml-utils-1.0.0.tar.gz` & `tmp/core-ml-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core-ml-utils-1.0.0.tar", last modified: Sat Jul 15 09:03:30 2023, max compression
+gzip compressed data, was "core-ml-utils-1.0.1.tar", last modified: Mon Jul 17 07:35:28 2023, max compression
```

## Comparing `core-ml-utils-1.0.0.tar` & `core-ml-utils-1.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:03:30.315609 core-ml-utils-1.0.0/
--rw-rw-rw-   0        0        0     1080 2023-07-09 05:25:39.000000 core-ml-utils-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      253 2023-07-15 09:03:30.314609 core-ml-utils-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       18 2023-07-15 09:02:56.000000 core-ml-utils-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 09:03:30.296610 core-ml-utils-1.0.0/cmu/
--rw-rw-rw-   0        0        0      364 2023-07-10 06:19:10.000000 core-ml-utils-1.0.0/cmu/__init__.py
--rw-rw-rw-   0        0        0     2456 2023-07-10 06:05:13.000000 core-ml-utils-1.0.0/cmu/config_parser.py
--rw-rw-rw-   0        0        0     7220 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/distributed.py
--rw-rw-rw-   0        0        0     1468 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/history_buffer.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:03:30.306612 core-ml-utils-1.0.0/cmu/hooks/
--rw-rw-rw-   0        0        0      296 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/__init__.py
--rw-rw-rw-   0        0        0     1770 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/checkpoint_hook.py
--rw-rw-rw-   0        0        0      558 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/distributed_hook.py
--rw-rw-rw-   0        0        0     1304 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/eval_hook.py
--rw-rw-rw-   0        0        0     3170 2023-07-15 09:02:28.000000 core-ml-utils-1.0.0/cmu/hooks/hookbase.py
--rw-rw-rw-   0        0        0     4106 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/logger_hook.py
--rw-rw-rw-   0        0        0     1651 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/hooks/lr_update_hook.py
--rw-rw-rw-   0        0        0     2926 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/logger.py
--rw-rw-rw-   0        0        0     7612 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/lr_scheduler.py
--rw-rw-rw-   0        0        0     3103 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/cmu/misc.py
--rw-rw-rw-   0        0        0    21480 2023-07-10 06:06:18.000000 core-ml-utils-1.0.0/cmu/trainer.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:03:30.313609 core-ml-utils-1.0.0/core_ml_utils.egg-info/
--rw-rw-rw-   0        0        0      253 2023-07-15 09:03:30.000000 core-ml-utils-1.0.0/core_ml_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      545 2023-07-15 09:03:30.000000 core-ml-utils-1.0.0/core_ml_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:03:30.000000 core-ml-utils-1.0.0/core_ml_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2023-07-15 09:03:30.000000 core-ml-utils-1.0.0/core_ml_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-07-15 09:03:30.000000 core-ml-utils-1.0.0/core_ml_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       70 2023-06-28 08:32:01.000000 core-ml-utils-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 09:03:30.315609 core-ml-utils-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      943 2023-07-15 09:03:13.000000 core-ml-utils-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:35:28.850463 core-ml-utils-1.0.1/
+-rw-rw-rw-   0        0        0     1080 2023-07-09 05:25:39.000000 core-ml-utils-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      253 2023-07-17 07:35:28.850463 core-ml-utils-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       18 2023-07-15 09:02:56.000000 core-ml-utils-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 07:35:28.833462 core-ml-utils-1.0.1/cmu/
+-rw-rw-rw-   0        0        0      364 2023-07-17 07:35:16.000000 core-ml-utils-1.0.1/cmu/__init__.py
+-rw-rw-rw-   0        0        0     2456 2023-07-10 06:05:13.000000 core-ml-utils-1.0.1/cmu/config_parser.py
+-rw-rw-rw-   0        0        0     7220 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/distributed.py
+-rw-rw-rw-   0        0        0     1468 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/history_buffer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:35:28.841462 core-ml-utils-1.0.1/cmu/hooks/
+-rw-rw-rw-   0        0        0      296 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/__init__.py
+-rw-rw-rw-   0        0        0     1770 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/checkpoint_hook.py
+-rw-rw-rw-   0        0        0      558 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/distributed_hook.py
+-rw-rw-rw-   0        0        0     1304 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/eval_hook.py
+-rw-rw-rw-   0        0        0     3170 2023-07-15 09:02:28.000000 core-ml-utils-1.0.1/cmu/hooks/hookbase.py
+-rw-rw-rw-   0        0        0     4106 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/logger_hook.py
+-rw-rw-rw-   0        0        0     1651 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/hooks/lr_update_hook.py
+-rw-rw-rw-   0        0        0     2926 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/logger.py
+-rw-rw-rw-   0        0        0     7612 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/lr_scheduler.py
+-rw-rw-rw-   0        0        0     3103 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/cmu/misc.py
+-rw-rw-rw-   0        0        0    21588 2023-07-16 09:29:58.000000 core-ml-utils-1.0.1/cmu/trainer.py
+drwxrwxrwx   0        0        0        0 2023-07-17 07:35:28.848463 core-ml-utils-1.0.1/core_ml_utils.egg-info/
+-rw-rw-rw-   0        0        0      253 2023-07-17 07:35:28.000000 core-ml-utils-1.0.1/core_ml_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2023-07-17 07:35:28.000000 core-ml-utils-1.0.1/core_ml_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 07:35:28.000000 core-ml-utils-1.0.1/core_ml_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2023-07-17 07:35:28.000000 core-ml-utils-1.0.1/core_ml_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-07-17 07:35:28.000000 core-ml-utils-1.0.1/core_ml_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       70 2023-06-28 08:32:01.000000 core-ml-utils-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 07:35:28.850463 core-ml-utils-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-07-15 09:03:13.000000 core-ml-utils-1.0.1/setup.py
```

### Comparing `core-ml-utils-1.0.0/LICENSE` & `core-ml-utils-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/config_parser.py` & `core-ml-utils-1.0.1/cmu/config_parser.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/distributed.py` & `core-ml-utils-1.0.1/cmu/distributed.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/history_buffer.py` & `core-ml-utils-1.0.1/cmu/history_buffer.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/checkpoint_hook.py` & `core-ml-utils-1.0.1/cmu/hooks/checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/distributed_hook.py` & `core-ml-utils-1.0.1/cmu/hooks/distributed_hook.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/eval_hook.py` & `core-ml-utils-1.0.1/cmu/hooks/eval_hook.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/hookbase.py` & `core-ml-utils-1.0.1/cmu/hooks/hookbase.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/logger_hook.py` & `core-ml-utils-1.0.1/cmu/hooks/logger_hook.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/hooks/lr_update_hook.py` & `core-ml-utils-1.0.1/cmu/hooks/lr_update_hook.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/logger.py` & `core-ml-utils-1.0.1/cmu/logger.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/lr_scheduler.py` & `core-ml-utils-1.0.1/cmu/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/misc.py` & `core-ml-utils-1.0.1/cmu/misc.py`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/cmu/trainer.py` & `core-ml-utils-1.0.1/cmu/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,14 +75,15 @@
         trainer.train()
     """
 
     def __init__(
         self,
         model: nn.Module,
         optimizer: optim.Optimizer,
+        criterion,
         lr_scheduler: optim.lr_scheduler._LRScheduler,
         data_loader: DataLoader,
         max_epochs: int,
         work_dir: str = "work_dir",
         max_num_checkpoints: int = None,
         checkpoint_period: int = 1,
         log_period: int = 50,
@@ -100,15 +101,15 @@
         self.optimizer = optimizer
         self.lr_scheduler = LRWarmupScheduler(lr_scheduler, by_epoch, len(data_loader), warmup_t,
                                               warmup_by_epoch, warmup_mode, warmup_init_lr,
                                               warmup_factor)
         self.data_loader = data_loader
         self.work_dir = work_dir
         self.metric_storage = MetricStorage()
-
+        self.criterion = criterion
         # counters
         self.inner_iter: int  # [0, epoch_len - 1]
         self.epoch: int  # [0, max_epochs - 1]
         self.start_epoch = 0  # [0, max_epochs - 1]
         self.max_epochs = max_epochs
 
         self._hooks: List[HookBase] = []
@@ -298,15 +299,16 @@
         #####################
         # 2. Calculate loss #
         #####################
         # If self._enable_amp=False, autocast and GradScaler’s calls become no-ops.
         # This allows switching between default precision and mixed precision
         # without if-else statements.
         with autocast(enabled=self._enable_amp):
-            loss_dict = self.model(batch)
+            data, label = batch
+            loss_dict = self.criterion(self.model(data), label) 
             if isinstance(loss_dict, torch.Tensor):
                 losses = loss_dict
                 loss_dict = {"total_loss": loss_dict}
             else:
                 losses = sum(loss_dict.values())
 
         ##########################
```

### Comparing `core-ml-utils-1.0.0/core_ml_utils.egg-info/SOURCES.txt` & `core-ml-utils-1.0.1/core_ml_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `core-ml-utils-1.0.0/setup.py` & `core-ml-utils-1.0.1/setup.py`

 * *Files identical despite different names*

