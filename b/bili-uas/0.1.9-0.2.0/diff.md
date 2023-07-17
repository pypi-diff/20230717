# Comparing `tmp/bili-uas-0.1.9.tar.gz` & `tmp/bili-uas-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.1.9.tar", last modified: Sun Jul  9 02:00:31 2023, max compression
+gzip compressed data, was "bili-uas-0.2.0.tar", last modified: Mon Jul 17 13:31:23 2023, max compression
```

## Comparing `bili-uas-0.1.9.tar` & `bili-uas-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,43 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.523998 bili-uas-0.1.9/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.518833 bili-uas-0.1.9/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.1.9/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1903 2023-07-03 09:43:52.000000 bili-uas-0.1.9/Bili_UAS/bili_config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5353 2023-07-09 02:00:21.000000 bili-uas-0.1.9/Bili_UAS/bili_live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2831 2023-07-03 09:35:16.000000 bili-uas-0.1.9/Bili_UAS/bili_login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2826 2023-07-03 09:35:16.000000 bili-uas-0.1.9/Bili_UAS/bili_user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2599 2023-07-09 02:00:21.000000 bili-uas-0.1.9/Bili_UAS/bili_video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.520040 bili-uas-0.1.9/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.1.9/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2368 2023-06-30 11:28:07.000000 bili-uas-0.1.9/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4270 2023-07-08 14:14:34.000000 bili-uas-0.1.9/Bili_UAS/scripts/live.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10541 2023-06-30 11:05:14.000000 bili-uas-0.1.9/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1366 2023-06-30 11:05:14.000000 bili-uas-0.1.9/Bili_UAS/scripts/user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5687 2023-06-30 11:44:32.000000 bili-uas-0.1.9/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.522131 bili-uas-0.1.9/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.1.9/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)    50170 2023-07-06 12:45:25.000000 bili-uas-0.1.9/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2186 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    15374 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18789 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.522739 bili-uas-0.1.9/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.1.9/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.1.9/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3575 2023-07-03 09:41:05.000000 bili-uas-0.1.9/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.1.9/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 02:00:31.523769 bili-uas-0.1.9/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.1.9/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-09 02:00:31.523507 bili-uas-0.1.9/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4599 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      808 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-09 02:00:31.000000 bili-uas-0.1.9/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-09 02:00:31.524061 bili-uas-0.1.9/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     2001 2023-07-09 02:00:28.000000 bili-uas-0.1.9/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.720234 bili-uas-0.2.0/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.712919 bili-uas-0.2.0/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.2.0/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2134 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     5445 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2875 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3350 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2964 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.713982 bili-uas-0.2.0/Bili_UAS/cli/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-17 12:26:30.000000 bili-uas-0.2.0/Bili_UAS/cli/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4298 2023-07-17 12:47:31.000000 bili-uas-0.2.0/Bili_UAS/cli/live_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1277 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/cli/user_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1502 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/cli/video_cli.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.714900 bili-uas-0.2.0/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.2.0/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2282 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    10584 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4670 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.717637 bili-uas-0.2.0/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.2.0/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2354 2023-07-15 12:39:12.000000 bili-uas-0.2.0/Bili_UAS/utils/config_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    63669 2023-07-17 12:17:57.000000 bili-uas-0.2.0/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2224 2023-07-17 12:23:11.000000 bili-uas-0.2.0/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.2.0/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18336 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-07-15 12:01:05.000000 bili-uas-0.2.0/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    22842 2023-07-15 13:04:58.000000 bili-uas-0.2.0/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.718931 bili-uas-0.2.0/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.2.0/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.2.0/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4148 2023-07-15 12:42:36.000000 bili-uas-0.2.0/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.2.0/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 13:31:23.720099 bili-uas-0.2.0/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.2.0/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.719904 bili-uas-0.2.0/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      890 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-17 13:31:23.720284 bili-uas-0.2.0/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     2042 2023-07-17 13:10:13.000000 bili-uas-0.2.0/setup.py
```

### Comparing `bili-uas-0.1.9/Bili_UAS/bili_live.py` & `bili-uas-0.2.0/Bili_UAS/bili_live.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,126 +2,128 @@
 Bili_UAS.bili_live
 
 This module provides a command line interface for monitoring the live broadcast room and processing data
 """
 
 
 from __future__ import annotations
-from Bili_UAS.utils import live_utils as lu, user_utils as uu
+from Bili_UAS.utils import config_utils as ucu
+from Bili_UAS.utils import live_utils as ulu, user_utils as uuu
 from typing import Union
-from Bili_UAS.writer import log_writer as lw, abnormal_monitor as am
+from Bili_UAS.writer import log_writer as wlw, abnormal_monitor as wam
 import os
 from bilibili_api import sync
-from Bili_UAS.scripts import config as sc, log_in as sli, live as sl
+from Bili_UAS.scripts import log_in as sli
+from Bili_UAS.cli import live_cli as clc
 import tyro
 import matplotlib.pyplot as plt
 from numpy import typing as npt
 
 
-def sync_tyro_main(config: Union[sl.BiliLiveConfigAuto, sl.BiliLiveConfigMonitor, sl.BiliLiveConfigProcess]) -> None:
+def sync_tyro_main(config: Union[clc.BiliLiveConfigAuto, clc.BiliLiveConfigMonitor, clc.BiliLiveConfigProcess]) -> None:
     """
     Main function for tyro command-line interface.
 
     Args:
         config: configuration
     """
-    work_dir: str = sync(sc.load_work_dir_from_txt())
+    work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "live_log.txt")
 
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     credential = sync(sli.load_credential_from_json(log_file))
     if credential is not None:
         credential = sync(sli.refresh_credential(credential, log_file))
 
-    if isinstance(config, sl.BiliLiveConfigAuto):
+    if isinstance(config, clc.BiliLiveConfigAuto):
         log.warning("The setting mode is 'auto', and in this mode, 'auto_disconnect', 'danmu_disconnect', and "
                     "'robust' are set to true, and data processing is automatically performed after disconnecting "
                     "the live streaming connection!")
 
         config.auto_disconnect = True
         config.danmu_disconnect = True
         config.robust = True
 
         if config.user_id is None:
             if config.live_id is None:
-                raise am.ParameterInputError("user_id and live_id must be entered either!")
+                raise wam.ParameterInputError("user_id and live_id must be entered either!")
 
         if config.user_id is not None:
-            user = uu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
+            user = uuu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
             config.live_id = user.room_id
 
-        live_monitor = lu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
-                                          config.retry_after, credential)
+        live_monitor = ulu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
+                                           config.retry_after, credential)
         sync(live_monitor.load_danmu_mark())
         mask: npt.NDArray = plt.imread(config.mask)
 
         sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
-        live_process = lu.BiliLiveProcess(log_file, live_monitor.work_dir)
+        live_process = ulu.BiliLiveProcess(log_file, live_monitor.work_dir)
         sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                    config.robust_interval, mask))
 
         while config.forever:
             log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
             sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
-            live_process = lu.BiliLiveProcess(log_file, live_monitor.work_dir)
+            live_process = ulu.BiliLiveProcess(log_file, live_monitor.work_dir)
             sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                        config.robust_interval, mask))
 
-    elif isinstance(config, sl.BiliLiveConfigMonitor):
+    elif isinstance(config, clc.BiliLiveConfigMonitor):
         log.warning("Set the mode to 'monitor', and in this mode, only data monitoring "
                     "will be performed without data processing!")
 
         if config.user_id is None:
             if config.live_id is None:
-                raise am.ParameterInputError("user_id and live_id must be entered either!")
+                raise wam.ParameterInputError("user_id and live_id must be entered either!")
 
         if config.user_id is not None:
-            user = uu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
+            user = uuu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
             config.live_id = user.room_id
 
-        live_monitor = lu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
-                                          config.retry_after, credential)
+        live_monitor = ulu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
+                                           config.retry_after, credential)
         sync(live_monitor.load_danmu_mark())
 
         sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
         while config.forever:
             log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
             sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
 
-    elif isinstance(config, sl.BiliLiveConfigProcess):
+    elif isinstance(config, clc.BiliLiveConfigProcess):
         log.warning("Set the mode to 'process', and in this mode, a data folder needs to be specified!")
 
         if config.data_dir is None:
-            raise am.ParameterInputError("No data folder specified!")
+            raise wam.ParameterInputError("No data folder specified!")
 
         if config.mask is not None:
             mask: npt.NDArray = plt.imread(config.mask)
         else:
             mask = None
-        live_process = lu.BiliLiveProcess(log_file, config.data_dir)
+        live_process = ulu.BiliLiveProcess(log_file, config.data_dir)
         sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                    config.robust_interval, mask))
 
 
 def tyro_cli() -> None:
     """
     Tyro command line interface.
     """
     tyro.extras.set_accent_color("bright_yellow")
     sync_tyro_main(
-        tyro.cli(sl.LiveConfigUnion, description="Monitor and process live broadcast room data.")
+        tyro.cli(clc.LiveConfigUnion, description="Monitor and process live broadcast room data.")
     )
 
 
 if __name__ == "__main__":
     tyro_cli()
```

### Comparing `bili-uas-0.1.9/Bili_UAS/bili_login.py` & `bili-uas-0.2.0/Bili_UAS/bili_login.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 Bili_UAS.bili_login
 
 This module provides a command line interface for logining to bilibili.
 """
 
 
 from __future__ import annotations
-from Bili_UAS.scripts import log_in as sli, config as sc
+from Bili_UAS.utils import config_utils as ucu
+from Bili_UAS.scripts import log_in as sli
 from bilibili_api import sync
 import os
 from typing import Literal, Union
 import tyro
-from Bili_UAS.writer import log_writer as lw, abnormal_monitor as am
+from Bili_UAS.writer import log_writer as wlw, abnormal_monitor as wam
 
 
 def sync_tyro_main(mode: Literal[1, 2, 3, 4] = 1,
                    sessdata: Union[str, None] = None,
                    bili_jct: Union[str, None] = None,
                    buvid3: Union[str, None] = None,
                    dedeuserid: Union[str, None] = None,
@@ -28,38 +29,38 @@
               specifying credential parameters
         sessdata: credential sessdata
         bili_jct: credential bili_jct
         buvid3: credential buvid3
         dedeuserid: credential dedeuserid
         ac_time_value: credential ac_time_value
     """
-    work_dir: str = sync(sc.load_work_dir_from_txt())
+    work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "login_log.txt")
 
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING", "ERROR")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     m = sli.LoginMode(mode)
 
     if m == sli.LoginMode.PARAMETER:
         if sessdata is not None and bili_jct is not None and buvid3 is not None \
                 and dedeuserid is not None and ac_time_value is not None:
             pass
         else:
-            raise am.ParameterInputError("Select the login method with the specified parameters,"
-                                         "but the input parameters are missing!")
+            raise wam.ParameterInputError("Select the login method with the specified parameters,"
+                                          "but the input parameters are missing!")
 
     if m == sli.LoginMode.QR:
         flag = sync(sli.log_in_by_QR_code(log_file))
     elif m == sli.LoginMode.PASSWORD:
         flag = sync(sli.log_in_by_password(log_file))
     elif m == sli.LoginMode.VERIFICATION:
         flag = sync(sli.log_in_by_verification_code(log_file))
```

### Comparing `bili-uas-0.1.9/Bili_UAS/bili_user.py` & `bili-uas-0.2.0/Bili_UAS/bili_user.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,83 +2,94 @@
 Bili_UAS.bili_user
 
 This module provides a command line interface for collecting user information and performing user operations.
 """
 
 
 from __future__ import annotations
-from Bili_UAS.utils import user_utils as uu
+from Bili_UAS.utils import config_utils as ucu, user_utils as uuu
+from Bili_UAS.cli import user_cli as cuc
 from typing import Union
 from bilibili_api import sync, user as bau
-from Bili_UAS.writer import log_writer as lw, abnormal_monitor as am
+from Bili_UAS.writer import log_writer as wlw, abnormal_monitor as wam
 import os
-from Bili_UAS.scripts import config as sc, log_in as sli, user as su
+from Bili_UAS.scripts import log_in as sli
 import tyro
 
 
-def sync_tyro_main(config: Union[su.BiliUserConfigUpdate, su.BiliUserConfigAddress]) -> None:
+language: str = ucu.load_language_from_txt()
+
+
+def sync_tyro_main(config: Union[cuc.BiliUserConfigUpdate, cuc.BiliUserConfigAddress]) -> None:
     """
     Main function for tyro command-line interface.
 
     Args:
         config: configuration
     """
-    work_dir: str = sync(sc.load_work_dir_from_txt())
+    work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "../test")
     log_file: str = os.path.join(log_output, "user_log.txt")
 
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING", "ERROR")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     credential = sync(sli.load_credential_from_json(log_file))
     if credential is not None:
         credential = sync(sli.refresh_credential(credential, log_file))
 
     if config.name is None:
         if config.uid is None:
-            raise am.ParameterInputError("name and uid must be entered either!")
+            if language == "en":
+                raise wam.ParameterInputError("name and uid must be entered either!")
+            else:
+                raise wam.ParameterInputError("用户名和uid必须输入其中之一！")
 
     if config.uid is None:
         try:
             uid_info: dict = sync(bau.name2uid(config.name))
             config.uid = uid_info['uid_list'][0]['uid']
         except KeyError:
-            log.error("Unable to query the uid of this user, the user may not exist or there may be "
-                      "unresolved characters in the username!")
-            log.warning("Please re-enter the username or directly enter the uid!")
+            if language == "en":
+                log.error("Unable to query the uid of this user, the user may not exist or there may be "
+                          "unresolved characters in the username!")
+                log.warning("Please re-enter the username or directly enter the uid!")
+            else:
+                log.error("无法查询到该用户的uid，该用户可能不存在或者用户名中存在无法解析的字符！")
+                log.warning("请重新输入用户名或直接输入uid！")
             return
 
-    user = uu.BiliUser(config.uid, log=log_file, work_dir=work_dir, credential=credential)
+    user = uuu.BiliUser(config.uid, log=log_file, work_dir=work_dir, credential=credential)
 
-    if isinstance(config, su.BiliUserConfigUpdate):
+    if isinstance(config, cuc.BiliUserConfigUpdate):
         sync(user.update_fans_number())
         sync(user.update_guard_number())
         sync(user.update_charge_number())
     else:
-        mode = su.AddressProcessType(config.mode)
-        if mode == su.AddressProcessType.SEND:
+        mode = uuu.AddressProcessType(config.mode)
+        if mode == uuu.AddressProcessType.SEND:
             sync(user.guard_address_stat_send())
-        elif mode == su.AddressProcessType.RECEIVE:
+        elif mode == uuu.AddressProcessType.RECEIVE:
             sync(user.guard_address_stat_receive())
 
 
 def tyro_cli() -> None:
     """
     Tyro command line interface.
     """
     tyro.extras.set_accent_color("bright_yellow")
     sync_tyro_main(
-        tyro.cli(su.UserConfigUnion, description="Update user fan number, guard number, "
+        tyro.cli(cuc.UserConfigUnion, description="Update user fan number, guard number, "
                                                  "charging number, and count guard addresses.")
     )
 
 
 if __name__ == "__main__":
     tyro_cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.1.9/Bili_UAS/bili_video.py` & `bili-uas-0.2.0/Bili_UAS/bili_video.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,74 +4,84 @@
 This module provides a command line interface for downloading videos, audio or generating word image.
 """
 
 
 from __future__ import annotations
 import matplotlib.pyplot as plt
 import tyro
-from Bili_UAS.scripts import video as sv, log_in as sli, config as sc
-from Bili_UAS.utils import video_utils as vu
+from Bili_UAS.utils import config_utils as ucu, video_utils as uvu
+from Bili_UAS.scripts import video as sv, log_in as sli
+from Bili_UAS.cli import video_cli as cvc
+from Bili_UAS.writer import log_writer as wlw, abnormal_monitor as wam
 from bilibili_api import sync
-from Bili_UAS.writer import log_writer as lw, abnormal_monitor as am
 import os
 from typing import Union
 from numpy import typing as npt
 
 
-def sync_tyro_main(config: Union[sv.BiliVideoConfigWordCloud, sv.BiliVideoConfigDownload]) -> None:
+language: str = ucu.load_language_from_txt()
+
+
+def sync_tyro_main(config: Union[cvc.BiliVideoConfigWordCloud, cvc.BiliVideoConfigDownload]) -> None:
     """
     Main function for tyro command-line interface.
 
     Args:
         config: configuration
     """
-    work_dir: str = sync(sc.load_work_dir_from_txt())
+    work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "video_log.txt")
 
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     credential = sync(sli.load_credential_from_json(log_file))
     if credential is not None:
         credential = sync(sli.refresh_credential(credential, log_file))
 
-    if isinstance(config, sv.BiliVideoConfigWordCloud):
+    if isinstance(config, cvc.BiliVideoConfigWordCloud):
         if config.video_id is None:
-            raise am.ParameterInputError("Video ID not entered!")
+            if language == "en":
+                raise wam.ParameterInputError("Video ID not entered!")
+            else:
+                raise wam.ParameterInputError("未输入视频ID！")
         wm = sv.WordCloudContent(config.mode)
         if config.mask is not None:
             word_cloud_mask: npt.NDArray = plt.imread(config.mask)
         else:
             word_cloud_mask = None
         sync(sv.word_cloud(config.video_id, credential, wm, config.sec, word_cloud_mask, log_file, work_dir))
     else:
         if config.video_id is None:
-            raise am.ParameterInputError("Video ID not entered!")
-        dm = vu.VideoDownloadMode(config.mode)
+            if language == "en":
+                raise wam.ParameterInputError("Video ID not entered!")
+            else:
+                raise wam.ParameterInputError("未输入视频ID！")
+        dm = uvu.VideoDownloadMode(config.mode)
         if isinstance(config.video_id, int):
-            video = vu.BiliVideo(log=log_file, aid=config.video_id, credential=credential, work_dir=work_dir)
+            video = uvu.BiliVideo(log=log_file, aid=config.video_id, credential=credential, work_dir=work_dir)
         else:
-            video = vu.BiliVideo(log=log_file, bvid=config.video_id, credential=credential, work_dir=work_dir)
+            video = uvu.BiliVideo(log=log_file, bvid=config.video_id, credential=credential, work_dir=work_dir)
         sync(video.download(dm))
 
 
 def tyro_cli() -> None:
     """
     Tyro command line interface.
     """
     tyro.extras.set_accent_color("bright_yellow")
     sync_tyro_main(
-        tyro.cli(sv.VideoConfigUnion, description="Download videos, audio or generate word image.")
+        tyro.cli(cvc.VideoConfigUnion, description="Download videos, audio or generate word image.")
     )
 
 
 if __name__ == "__main__":
     tyro_cli()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.1.9/Bili_UAS/scripts/config.py` & `bili-uas-0.2.0/Bili_UAS/scripts/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Bili_UAS.scripts.config
 
 This module provides the function to save and read working path and danmu mark.
 """
 
 
 from __future__ import annotations
-from Bili_UAS.writer import abnormal_monitor as am
+from Bili_UAS.writer import log_writer as wlw
 import os
 
 
 async def save_work_dir_to_txt(work_dir: str) -> None:
     """
     Save working path to file.
     """
@@ -33,49 +33,48 @@
     log_out_dir: str = os.path.join(output_dir, "log")
     if not os.path.exists(log_out_dir):
         os.mkdir(log_out_dir)
 
     print("Working path saved successfully.")
 
 
-async def load_work_dir_from_txt() -> str:
-    """
-    Load a working path from file.
-
-    Returns:
-        the work directory
-    """
-    config_file: str = ".work_dir.txt"
-    if not os.path.exists(config_file):
-        raise am.FileMissError("No historical working path found, please specify the working path.")
-    else:
-        with open(config_file, "r") as f:
-            work_dir: str = f.readline().removesuffix("\n")
-        print("Historical working path found, using historical working path.")
-        return work_dir
-
-
-async def save_danmu_mark_to_txt(danmu_mark: list[str]) -> None:
+async def save_danmu_mark_to_txt(danmu_mark: list[str], log: wlw.Logger) -> None:
     """
     Save danmu mark to file.
 
     Args:
         danmu_mark: danmu mark list
+        log: logger
     """
     danmu_mark_file: str = ".danmu_mark.txt"
     with open(danmu_mark_file, "w") as f:
         for mark in danmu_mark:
             f.write(mark + "\n")
-    print("Danmu mark saved successfully.")
+    log.info("Danmu mark saved successfully.")
 
 
-async def save_ffmpeg_path_to_txt(ffmpeg_path: str) -> None:
+async def save_ffmpeg_path_to_txt(ffmpeg_path: str, log: wlw.Logger) -> None:
     """
     Save ffmpeg path to file.
 
     Args:
         ffmpeg_path: the path of ffmpeg
+        log: logger
     """
     ffmpeg_file: str = ".ffmpeg.txt"
     with open(ffmpeg_file, "w") as f:
         f.write(ffmpeg_path + "\n")
-    print("Ffmpeg path saved successfully.")
+    log.info("Ffmpeg path saved successfully.")
+
+
+async def save_language_to_txt(language: str, log: wlw.Logger) -> None:
+    """
+    Save language to file.
+
+    Args:
+        language: the language of program prompts
+        log: logger
+    """
+    language_file: str = ".language.txt"
+    with open(language_file, "w") as f:
+        f.write(language + "\n")
+    log.info("Language configuration saved successfully.")
```

### Comparing `bili-uas-0.1.9/Bili_UAS/scripts/live.py` & `bili-uas-0.2.0/Bili_UAS/cli/live_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
-Bili_UAS.scripts.live
+Bili_UAS.cli.live_cli
 
-This module provides classes for configuring live-streaming data monitoring.
+This module provides command line interface configuration for monitoring and processing live broadcasts.
 """
 
 
 from typing import Union
 from dataclasses import dataclass
 import tyro
```

### Comparing `bili-uas-0.1.9/Bili_UAS/scripts/log_in.py` & `bili-uas-0.2.0/Bili_UAS/scripts/log_in.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from bilibili_api import login, user, Credential
 from bilibili_api import settings
 from bilibili_api.exceptions import (CredentialNoBiliJctException, CredentialNoSessdataException,
                                      CredentialNoBuvid3Exception, CredentialNoDedeUserIDException)
 import sys
 import json
 import os
-from Bili_UAS.writer import log_writer as lw
+from Bili_UAS.writer import log_writer as wlw
 import enum
 from typing import Union
 
 
 class LoginMode(enum.Enum):
     """
     Login method Enumeration Class
@@ -31,22 +31,22 @@
 async def load_credential_from_json(log_file: str) -> Union[Credential, None]:
     """
     Load credential from json file.
 
     Args:
         log_file: the log file
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     config_file: str = ".config.json"
     if not os.path.exists(config_file):
         log.warning("No historical login records found, using empty credential!")
         return None
@@ -66,22 +66,22 @@
     """
     Save credential to json file.
 
     Args:
         credential: logon credentials
         log_file: the log file
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     config_file: str = ".config.json"
     credential_dict: dict = {"sessdata": credential.sessdata,
                              "bili_jct": credential.bili_jct,
                              "buvid3": credential.buvid3,
@@ -105,22 +105,22 @@
         sessdata: credential sessdata
         bili_jct: credential bili_jct
         buvid3: credential buvid3
         dedeuserid: credential dedeuserid
         ac_time_value: credential ac_time_value
         log_file: the log file
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     config_file: str = ".config.json"
     credential_dict: dict = {"sessdata": sessdata,
                              "bili_jct": bili_jct,
                              "buvid3": buvid3,
@@ -137,22 +137,22 @@
 
     Args:
         log_file: the log file
 
     Returns:
         True if login successfully, False otherwise.
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     log.info("Please scan the QR code.")
     credential: Credential = login.login_with_qrcode()
 
     try:
@@ -191,22 +191,22 @@
 
     Args:
         log_file: the log file
 
     Returns:
         True if login successfully, False otherwise.
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     log.info("Please enter your username (phone number/email):\n")
     user_name: str = str(sys.stdin.readline())
     log.info("Please enter password:\n")
     password: str = str(sys.stdin.readline())
@@ -255,22 +255,22 @@
 
     Args:
         log_file: the log file
 
     Returns:
         True if login successfully, False otherwise.
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     settings.geetest_auto_open = False
     log.info("Please enter your phone number:\n")
     phone_number: str = str(sys.stdin.readline())
     log.info("Please wait for receiving the verification code...")
@@ -322,22 +322,22 @@
     Args:
         credential: logon credentials
         log_file: the log file
 
     Returns:
         refreshed credential
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     if credential.chcek_refresh():
         await credential.refresh()
         log.info("Credential refreshed successfully.")
     else:
```

### Comparing `bili-uas-0.1.9/Bili_UAS/scripts/user.py` & `bili-uas-0.2.0/Bili_UAS/cli/user_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,17 @@
 """
-Bili_UAS.scripts.user
+Bili_UAS.cli.user_cli
 
-This module provides classes for configuring user data.
+This module provides user command line interface configuration.
 """
 
 
 import tyro
 from typing import Union, Literal
 from dataclasses import dataclass
-import enum
-
-
-class AddressProcessType(enum.Enum):
-    """
-
-    """
-    SEND = 1
-    RECEIVE = 2
 
 
 @dataclass
 class BiliUserConfigUpdate(object):
     """
 
     """
```

### Comparing `bili-uas-0.1.9/Bili_UAS/scripts/video.py` & `bili-uas-0.2.0/Bili_UAS/scripts/video.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 Bili_UAS.scripts.video
 
 This module provides the function to obtain video data and generate word cloud images.
 """
 
 
 from __future__ import annotations
-from typing import Union, Literal
+from typing import Union
 import jieba
 import wordcloud
 import pandas as pd
-from Bili_UAS.utils import video_utils as vu
+from Bili_UAS.utils import video_utils as uvu
 from numpy import typing as npt
 from bilibili_api import Credential
-from Bili_UAS.writer import log_writer as lw
+from Bili_UAS.utils.config_utils import load_language_from_txt
+from Bili_UAS.writer import log_writer as wlw
 import enum
 import os
 from dataclasses import dataclass
 import tyro
 
 
+language: str = load_language_from_txt()
+
+
 class WordCloudContent(enum.Enum):
     """
     Word Cloud Content Enumeration Class
     """
     REPLY = 1
     DANMU = 2
     BOTH = 3
@@ -44,31 +48,34 @@
         credential: logon credentials
         mode: 0 represents only processing comments, 1 represents only processing danmu, and 2 represents both processing
         sec: whether to process secondary replies
         mask: word cloud mask, filling the white pixel with word clouds
         log_file: the log file
         work_dir: working directory
     """
-    file_handler: lw.Handler = lw.Handler("file")
+    file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
 
-    sys_handler: lw.Handler = lw.Handler("sys")
+    sys_handler: wlw.Handler = wlw.Handler("sys")
     sys_handler.set_level("INFO", "WARNING")
 
-    log: lw.Logger = lw.Logger()
+    log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     if isinstance(video_id, int):
-        video = vu.BiliVideo(log=log_file, aid=video_id, credential=credential, work_dir=work_dir)
+        video = uvu.BiliVideo(log=log_file, aid=video_id, credential=credential, work_dir=work_dir)
     else:
-        video = vu.BiliVideo(log=log_file, bvid=video_id, credential=credential, work_dir=work_dir)
+        video = uvu.BiliVideo(log=log_file, bvid=video_id, credential=credential, work_dir=work_dir)
 
-    log.info("Starting to generate word cloud image...")
+    if language == "en":
+        log.info("Starting to generate word cloud image...")
+    else:
+        log.info("开始生成词云图片...")
     if mode == WordCloudContent.REPLY:
         save_path: str = os.path.join(video.work_dir, "reply_word_cloud.jpg")
 
         reply_content: str = ""
         await video.get_replies(sec=sec)
         await video.reply_robust_process()
         for elem in video.robust_replies:
@@ -115,60 +122,19 @@
         words: list[str] = jieba.lcut(content)
         word_freq = pd.Series(words).value_counts()
         wc = wordcloud.WordCloud(font_path='PingFang.ttc', background_color='white', mask=mask)
         wc.generate_from_frequencies(word_freq)
         image = wc.to_image()
         image.save(save_path, quality=100)
 
-    log.info(f"Word cloud image generated successfully! Saved in {save_path}.")
+    if language == "en":
+        log.info(f"Word cloud image generated successfully! Saved in {save_path}.")
+    else:
+        log.info(f"词云图片生成成功！保存在 {save_path} 。")
 
 
 # TODO: Effective Chinese sentiment analysis tool
 # def _sentiment_analysis() -> None:
 #     """
 #     Conduct emotional analysis on video comments and barrage, and generate emotional statistical charts.
 #     """
 #     pass
-
-
-@dataclass
-class BiliVideoConfigWordCloud(object):
-    """
-    Bilibili Video Configuration Class: Word Cloud.
-    """
-    video_id: Union[str, int, None] = None
-    """video's aid or bvid"""
-    mode: Literal[1, 2, 3] = 1
-    """word cloud content, 1 represents comments, 2 represents barrage, and 3 represents both"""
-    sec: bool = True
-    """whether to process secondary replies"""
-    mask: Union[str, None] = None
-    """word cloud mask, filling the white pixel with word clouds"""
-
-
-@dataclass
-class BiliVideoConfigDownload(object):
-    """
-    Bilibili Video Configuration Class: Download.
-    """
-    video_id: Union[str, int, None] = None
-    """video's aid or bvid"""
-    mode: Literal[1, 2] = 1
-    """video download type, 1 represents video and 2 represents audio"""
-
-
-mode_configs: dict[str, Union[BiliVideoConfigWordCloud, BiliVideoConfigDownload]] = {}
-
-descriptions: dict[str, str] = {
-    "word_cloud": "Generate word cloud images of video replies or danmu.",
-    "download": "Download video or audio."
-}
-
-mode_configs["word_cloud"] = BiliVideoConfigWordCloud()
-mode_configs["download"] = BiliVideoConfigDownload()
-
-VideoConfigUnion = tyro.conf.SuppressFixed[
-    tyro.conf.FlagConversionOff[
-        tyro.extras.subcommand_type_from_defaults(defaults=mode_configs, descriptions=descriptions)
-    ]
-]
-
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.1.9/Bili_UAS/utils/live_utils.py` & `bili-uas-0.2.0/Bili_UAS/utils/live_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 # within this time period after streaming cannot be recorded.
 
 
 from __future__ import annotations
 from bilibili_api import live as bal, sync, Credential
 from matplotlib import pyplot as plt
 from .utils import BiliLiveDanmu, BiliLiveGift, BiliLiveSC, BiliLiveGuard
-from Bili_UAS.writer import log_writer as lw
+from .config_utils import load_language_from_txt
+from Bili_UAS.writer import log_writer as wlw
 import os
 import datetime
 import time
 import pandas as pd
 from pandas import DataFrame
 import numpy as np
 import scipy.interpolate as spi
 from typing import Union
 from numpy import typing as npt
 import jieba
 import wordcloud
 
 
+language: str = load_language_from_txt()
 danmu_warning_mark: list[str] = ["@", "。", "？", "！", "，", ".", "?", "!", ","]
 
 
 class BiliLiveMonitor(bal.LiveRoom, bal.LiveDanmaku):
     """
     Bilibili live monitor class.
     """
@@ -89,31 +91,31 @@
         self.guard_excel: Union[DataFrame, None] = None
         self.guard_excel_file: Union[str, None] = None
         self.view_txt_file: Union[str, None] = None
         self.live_info_txt_file: Union[str, None] = None
         self.todo_txt_file: Union[str, None] = None
 
         self.log_file: str = log
-        self.log: Union[lw.Logger, None] = None
+        self.log: Union[wlw.Logger, None] = None
         self.__set_log()
         self.__init_live_room_info()
         self.__load_work_dir(work_dir)
 
     def __set_log(self) -> None:
         """
         Set up logs.
         """
-        file_handler: lw.Handler = lw.Handler("file")
+        file_handler: wlw.Handler = wlw.Handler("file")
         file_handler.set_level("WARNING", "ERROR")
         file_handler.set_file(self.log_file)
 
-        sys_handler: lw.Handler = lw.Handler("sys")
+        sys_handler: wlw.Handler = wlw.Handler("sys")
         sys_handler.set_level("INFO", "WARNING")
 
-        self.log: lw.Logger = lw.Logger()
+        self.log: wlw.Logger = wlw.Logger()
         self.log.add_config(file_handler)
         self.log.add_config(sys_handler)
 
     def __init_live_room_info(self) -> None:
         """
         Initialize live room information.
         """
@@ -145,43 +147,51 @@
         live_play_info: dict = await self.get_room_play_info_v2()
         self.live_status: int = live_play_info['live_status']
         if self.live_status == 1:
             return True
         else:
             return False
 
+    @wlw.async_separate()
     async def get_live_info(self) -> None:
         """
         Get live information.
         """
+        if language == "en":
+            self.log.info("Getting live information...")
+        else:
+            self.log.info("正在获取直播信息...")
         live_play_info: dict = await self.get_room_play_info_v2()
-        if live_play_info:
-            self.is_hidden: bool = live_play_info['is_hidden']
-            self.is_locked: bool = live_play_info['is_locked']
-            self.is_portrait: bool = live_play_info['is_portrait']
-            self.hidden_till: Union[int, None] = live_play_info['hidden_till'] if live_play_info[
-                                                                                      'hidden_till'] != 0 else None
-            self.lock_till: Union[int, None] = live_play_info['lock_till'] if live_play_info['lock_till'] != 0 else None
-            self.encrypted: bool = live_play_info['encrypted']
-            self.pwd_verified: Union[bool, None] = live_play_info['pwd_verified'] if self.encrypted else None
-            self.live_start_time: int = live_play_info['live_time']
+        self.is_hidden: bool = live_play_info['is_hidden']
+        self.is_locked: bool = live_play_info['is_locked']
+        self.is_portrait: bool = live_play_info['is_portrait']
+        self.hidden_till: Union[int, None] = live_play_info['hidden_till'] if live_play_info[
+                                                                                  'hidden_till'] != 0 else None
+        self.lock_till: Union[int, None] = live_play_info['lock_till'] if live_play_info['lock_till'] != 0 else None
+        self.encrypted: bool = live_play_info['encrypted']
+        self.pwd_verified: Union[bool, None] = live_play_info['pwd_verified'] if self.encrypted else None
+        self.live_start_time: int = live_play_info['live_time']
 
         live_info: dict = await self.get_room_info()
-        if live_info:
-            self.area_id: int = live_info['room_info']['area_id']
-            self.area_name: str = live_info['room_info']['area_name']
-            self.parent_area_id: int = live_info['room_info']['parent_area_id']
-            self.parent_area_name: str = live_info['room_info']['parent_area_name']
-            self.title: str = live_info['room_info']['title']
-            self.introduction: str = live_info['news_info']['content']
+        self.area_id: int = live_info['room_info']['area_id']
+        self.area_name: str = live_info['room_info']['area_name']
+        self.parent_area_id: int = live_info['room_info']['parent_area_id']
+        self.parent_area_name: str = live_info['room_info']['parent_area_name']
+        self.title: str = live_info['room_info']['title']
+        self.introduction: str = live_info['news_info']['content']
 
+    @wlw.async_separate()
     async def live_info_to_txt(self) -> None:
         """
         Write live information to txt.
         """
+        if language == "en":
+            self.log.info("Writing live information to txt...")
+        else:
+            self.log.info("正在将直播信息写入文件...")
         with open(self.live_info_txt_file, "a") as f:
             f.write("\n")
             f.write(f"title: {self.title}\n")
             f.write(f"live_start_time: {datetime.datetime.fromtimestamp(self.live_start_time)}\n")
             f.write(f"is_hidden: {self.is_hidden}\n")
             f.write(f"is_locked: {self.is_locked}\n")
             f.write(f"is_portrait: {self.is_portrait}\n")
@@ -191,14 +201,18 @@
             if self.encrypted:
                 f.write(f"pwd_verified: {self.pwd_verified}\n")
             f.write(f"introduction: {self.introduction if self.introduction else 'None'}\n")
             f.write(f"area_id: {self.area_id}\n")
             f.write(f"area_name: {self.area_name}\n")
             f.write(f"parent_area_id: {self.parent_area_id}\n")
             f.write(f"parent_area_name: {self.parent_area_name}\n")
+        if language == "en":
+            self.log.info("Live information has been written to txt.")
+        else:
+            self.log.info("直播信息已写入文件。")
 
     async def __load_output_file(self) -> None:
         """
         Load the test_output file.
         Includes Excel files for storing danmu, gifts,
         guards and SCs as well as txt files for storing popularity values.
         """
@@ -261,41 +275,50 @@
 
     async def load_danmu_mark(self) -> None:
         """
         Load the marked
         """
         danmu_mark_txt_file: str = ".danmu_mark.txt"
         if not os.path.exists(danmu_mark_txt_file):
-            self.log.warning("The danmu mark file does not exist. Use the default mark.")
+            if language == "en":
+                self.log.warning("The danmu mark file does not exist. Use the default mark.")
+            else:
+                self.log.warning("弹幕标记文件不存在。使用默认标记。")
         else:
             self.mark: list = []
             with open(danmu_mark_txt_file, "r") as f:
                 for elem in f.readlines():
                     self.mark.append(elem.removesuffix("\n"))
             for m in self.mark:
                 if m in danmu_warning_mark:
-                    self.log.warning(f"{m}: This mark is a symbol that might be used in a normal unmarked danmu and "
-                                     f"may cause confusion!")
-            self.log.info("Load the danmu mark successful.")
+                    if language == "en":
+                        self.log.warning(f"{m}: This mark is a symbol that might be used in a normal unmarked danmu and "
+                                         f"may cause confusion!")
+                    else:
+                        self.log.warning(f"{m}: 此标记是未标记弹幕中可能会使用的符号，可能会造成混淆！")
+            if language == "en":
+                self.log.info("Load the danmu mark successful.")
+            else:
+                self.log.info("弹幕标记加载成功。")
 
     async def monitor(self, save_all_danmu: bool, danmu_disconnect: bool, auto_disconnect: bool) -> None:
         """
         Monitor live broadcast.
 
         Args:
             save_all_danmu: whether to save all live danmu, default is True
             danmu_disconnect: whether to disconnect from the live broadcast room by entering "###disconnect###"
             auto_disconnect: whether to disconnect from the live room automatically when the live broadcast ends
         """
         live_start: bool = False
-        live_flag: bool = True
+        live_sta_flag: bool = True
         force_flag: bool = await self.__check_live_sta()
         if force_flag:
             live_start = True
-            live_flag = False
+            live_sta_flag = False
             await self.get_live_info()
             await self.__load_output_file()
             await self.live_info_to_txt()
 
         @self.on("DANMU_MSG")
         async def __disconnect_live_room(event: dict) -> None:
             """
@@ -303,14 +326,18 @@
 
             Args:
                  event: API returns data
             """
             if danmu_disconnect:
                 flag: str = event['data']['info'][1]
                 if flag == "###disconnect###":
+                    if language == "en":
+                        self.log.info("Received the stop command and disconnect from the live broadcast room.")
+                    else:
+                        self.log.info("收到停止指令，断开直播间连接。")
                     await self.disconnect()
 
         @self.on("DANMU_MSG")
         async def __danmu_record(event: dict) -> None:
             """
             Record danmaku.
 
@@ -320,58 +347,70 @@
             if live_start:
                 danmu: BiliLiveDanmu = BiliLiveDanmu(log=self.log_file)
                 await danmu.load_from_api(event)
                 if save_all_danmu:
                     await danmu.to_excel(self.danmu_excel_file, self.danmu_excel)
                     self.danmu_excel = pd.read_excel(self.danmu_excel_file)
                 if danmu.content[0] in self.mark or danmu.content[-1] in self.mark:
-                    self.log.info("Get a marked danmu.")
+                    if language == "en":
+                        self.log.info("Get a marked danmu.")
+                    else:
+                        self.log.info("获取到一个标记弹幕。")
                     await danmu.to_excel(self.marked_danmu_file, self.marked_danmu_excel)
                     self.marked_danmu_excel = pd.read_excel(self.marked_danmu_file)
 
         @self.on("SEND_GIFT")
         async def __gift_record(event: dict) -> None:
             """
             Record gifts.
 
             Args:
                 event: API returns data
             """
             if live_start:
-                self.log.info("Get a gift.")
+                if language == "en":
+                    self.log.info("Get a gift.")
+                else:
+                    self.log.info("获取到一个礼物。")
                 gift: BiliLiveGift = BiliLiveGift(log=self.log_file)
                 await gift.load_from_api(event)
                 await gift.to_excel(self.gift_excel_file, self.gift_excel)
                 self.gift_excel = pd.read_excel(self.gift_excel_file)
 
         @self.on("GUARD_BUY")
         async def __guard_record(event: dict) -> None:
             """
             Record guard.
 
             Args:
                 event: API returns data
             """
             if live_start:
-                self.log.info("Get a guard.")
+                if language == "en":
+                    self.log.info("Get a guard.")
+                else:
+                    self.log.info("获取到一个舰长。")
                 guard: BiliLiveGuard = BiliLiveGuard(log=self.log_file)
                 await guard.load_from_api(event)
                 await guard.to_excel(self.guard_excel_file, self.guard_excel)
                 self.guard_excel = pd.read_excel(self.guard_excel_file)
 
         @self.on("SUPER_CHAT_MESSAGE_JPN")
         async def __sc_record(event: dict) -> None:
             """
             Record sc.
 
             Args:
                 event: API returns data
             """
             if live_start:
-                self.log.info("Get a sc.")
+                if language == "en":
+                    self.log.info("Get a sc.")
+                else:
+                    self.log.info("获取到一个SC。")
                 sc: BiliLiveSC = BiliLiveSC(log=self.log_file)
                 await sc.load_from_api(event)
                 await sc.to_excel(self.sc_excel_file, self.sc_excel)
                 self.sc_excel = pd.read_excel(self.sc_excel_file)
 
         @self.on("VIEW")
         async def __view_record(event: dict) -> None:
@@ -379,48 +418,60 @@
             Record the popularity of the live broadcast room.
 
             Args:
                 event: API returns data
             """
             t: str = str(int(time.time()))
             if live_start:
-                self.log.info("Popularity update.")
+                if language == "en":
+                    self.log.info("Popularity update.")
+                else:
+                    self.log.info("人气更新。")
                 with open(self.view_txt_file, "a") as f:
                     f.write(t + "," + str(event['data']))
                     f.write("\n")
 
         @self.on("LIVE")
         async def __live_stat_record(event: dict) -> None:
             """
             Record live status.
 
             Args:
                 event: API returns data
             """
-            nonlocal live_start, live_flag
+            nonlocal live_start, live_sta_flag
             live_start = True
-            if live_flag:
+            if live_sta_flag:
                 self.live_start_time = event['data']['live_time']
                 await self.__load_output_file()
                 await self.get_live_info()
                 await self.live_info_to_txt()
-                self.log.info("Live start.")
-                live_flag = False
+                if language == "en":
+                    self.log.info("Live start.")
+                else:
+                    self.log.info("直播开始。")
+                live_sta_flag = False
 
         @self.on("PREPARING")
         async def __monitor_live_end() -> None:
             """
             Check if the live broadcast has ended.
             """
             self.live_end_time = time.time()
-            self.log.warning("Live broadcast has ended.")
+            if language == "en":
+                self.log.warning("Live broadcast has ended.")
+            else:
+                self.log.warning("直播已结束。")
             with open(self.live_info_txt_file, "a") as f:
                 f.write(f"live_end_time: {datetime.datetime.fromtimestamp(self.live_end_time)}\n")
             if auto_disconnect:
-                self.log.warning("Auto disconnect.")
+                if language == "en":
+                    self.log.warning("Auto disconnect.")
+                else:
+                    self.log.warning("自动断开连接。")
                 await self.disconnect()
 
         await self.connect()
 
 
 class BiliLiveProcess(object):
     """
@@ -448,43 +499,45 @@
         self.view: list[int] = []
         self.view_time: list[int] = []
 
         self.complete_suggestion_txt_file: Union[str, None] = None
         self.sparse_suggestion_txt_file: Union[str, None] = None
 
         self.log_file: str = log
-        self.log: Union[lw.Logger, None] = None
+        self.log: Union[wlw.Logger, None] = None
         self.__set_log()
         self.__load_work_dir(work_dir)
 
     def __set_log(self) -> None:
         """
         Set up logs.
         """
-        file_handler: lw.Handler = lw.Handler("file")
+        file_handler: wlw.Handler = wlw.Handler("file")
         file_handler.set_level("WARNING", "ERROR")
         file_handler.set_file(self.log_file)
 
-        sys_handler: lw.Handler = lw.Handler("sys")
+        sys_handler: wlw.Handler = wlw.Handler("sys")
         sys_handler.set_level("INFO", "WARNING")
 
-        self.log: lw.Logger = lw.Logger()
+        self.log: wlw.Logger = wlw.Logger()
         self.log.add_config(file_handler)
         self.log.add_config(sys_handler)
 
     def __load_work_dir(self, work_dir: str) -> None:
         """
         Load the working directory.
 
         Args:
             work_dir: the working directory path
         """
         dir_name: str = os.path.split(work_dir)[-1]
         if not dir_name.isdigit():
             self.work_dir.append(os.path.abspath(work_dir))
+            temp: str = os.path.split(os.path.abspath(work_dir))[0]
+            self.todo_txt_file: str = os.path.join(temp, ".todo.txt")
             if os.path.exists(self.todo_txt_file):
                 todo_list: list[str] = []
                 with open(self.todo_txt_file, "r") as f:
                     for live_dir in f.readlines():
                         temp: str = live_dir.removesuffix("\n")
                         if temp not in todo_list:
                             todo_list.append(temp)
@@ -509,139 +562,201 @@
     async def __load_danmu(self, live_dir: str) -> None:
         """
         Load the danmu.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Loading the complete danmu data and the marked danmu...")
+        if language == "en":
+            self.log.info("Loading the complete danmu data and the marked danmu data...")
+        else:
+            self.log.info("正在加载完整弹幕数据和标记弹幕数据...")
         danmu_excel_file: str = os.path.join(live_dir, "danmu.xlsx")
         if not os.path.exists(danmu_excel_file):
-            self.log.warning("The live broadcast did not save the complete danmu data, so frequency analysis cannot be "
-                             "conducted!")
+            if language == "en":
+                self.log.warning("The live broadcast did not save the complete danmu data, which may affect "
+                                 "subsequent operations!")
+            else:
+                self.log.warning("直播间没有保存完整弹幕数据，这可能会影响后续操作！")
         else:
             danmu_excel: DataFrame = pd.read_excel(danmu_excel_file)
             if danmu_excel.empty:
-                self.log.warning(
-                    "The live broadcast did not save the complete danmu data, so frequency analysis cannot "
-                    "be conducted!")
+                if language == "en":
+                    self.log.warning(
+                        "The live broadcast did not save the complete danmu data, which may affect subsequent!")
+                else:
+                    self.log.warning("直播间没有保存完整弹幕数据，这可能会影响后续操作！")
             else:
                 danmu_data_list: list[dict] = danmu_excel.to_dict(orient="records")
                 for elem in danmu_data_list:
                     danmu: BiliLiveDanmu = BiliLiveDanmu(log=self.log_file)
                     await danmu.load_from_excel(elem)
                     self.danmu.append(danmu)
-                self.log.info("Load the danmu successful.")
+                if language == "en":
+                    self.log.info("Load the complete danmu successful.")
+                else:
+                    self.log.info("成功加载完整弹幕数据。")
 
         marked_danmu_excel_file: str = os.path.join(live_dir, "marked_danmu.xlsx")
         if not os.path.exists(marked_danmu_excel_file):
-            self.log.warning("There is no marked danmu!")
+            if language == "en":
+                self.log.warning("There is no marked danmu data, which may affect subsequent!")
+            else:
+                self.log.warning("没有被标记弹幕数据，这可能会影响后续操作！")
         else:
             marked_danmu_excel: DataFrame = pd.read_excel(marked_danmu_excel_file)
             if marked_danmu_excel.empty:
-                self.log.warning("There is no marked danmu!")
+                if language == "en":
+                    self.log.warning("There is no marked danmu data, which may affect subsequent!")
+                else:
+                    self.log.warning("没有被标记弹幕数据，这可能会影响后续操作！")
             else:
                 marked_danmu_data_list: list[dict] = marked_danmu_excel.to_dict(orient="records")
                 for elem in marked_danmu_data_list:
                     danmu: BiliLiveDanmu = BiliLiveDanmu(log=self.log_file)
                     await danmu.load_from_excel(elem)
                     self.marked_danmu.append(danmu)
-                self.log.info("Load the marked danmu successful.")
+                if language == "en":
+                    self.log.info("Load the marked danmu data successful.")
+                else:
+                    self.log.info("成功加载标被记弹幕数据。")
 
     async def __load_gift(self, live_dir: str) -> None:
         """
         Load the gift.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Loading the gift...")
+        if language == "en":
+            self.log.info("Loading the gift data...")
+        else:
+            self.log.info("正在加载礼物数据...")
         gift_excel_file: str = os.path.join(live_dir, "gift.xlsx")
         if not os.path.join(gift_excel_file):
-            self.log.warning("The gift data file does not exist!")
+            if language == "en":
+                self.log.warning("There is no gifts data, which may affect subsequent!")
+            else:
+                self.log.warning("没有礼物数据，这可能会影响后续操作！")
         else:
             gift_excel: DataFrame = pd.read_excel(gift_excel_file)
             if gift_excel.empty:
-                self.log.warning("There is no gift!")
+                if language == "en":
+                    self.log.warning("There is no gifts data, which may affect subsequent!")
+                else:
+                    self.log.warning("没有礼物数据，这可能会影响后续操作！")
             else:
                 gift_list: [dict] = gift_excel.to_dict(orient="records")
                 for elem in gift_list:
                     if elem["gift_id"] == 31531:
                         continue
                     gift: BiliLiveGift = BiliLiveGift(log=self.log_file)
                     await gift.load_from_excel(elem)
                     self.gift.append(gift)
-                self.log.info("Load the gift successful.")
+                if language == "en":
+                    self.log.info("Load the gift data successful.")
+                else:
+                    self.log.info("成功加载礼物数据。")
 
     async def __load_sc(self, live_dir: str) -> None:
         """
         Load the sc.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Loading the sc...")
+        if language == "en":
+            self.log.info("Loading the sc data...")
+        else:
+            self.log.info("正在加载sc数据...")
         sc_excel_file: str = os.path.join(live_dir, "sc.xlsx")
         if not os.path.join(sc_excel_file):
-            self.log.warning("The sc data file does not exist!")
+            if language == "en":
+                self.log.warning("There is no sc data, which may affect subsequent!")
+            else:
+                self.log.warning("没有sc数据，这可能会影响后续操作！")
         else:
             sc_excel: DataFrame = pd.read_excel(sc_excel_file)
             if sc_excel.empty:
-                self.log.warning("There is no gift!")
+                if language == "en":
+                    self.log.warning("There is no sc data, which may affect subsequent!")
+                else:
+                    self.log.warning("没有sc数据，这可能会影响后续操作！")
             else:
                 sc_list: list[dict] = sc_excel.to_dict(orient="records")
                 for elem in sc_list:
                     sc: BiliLiveSC = BiliLiveSC(log=self.log_file)
                     await sc.load_from_excel(elem)
                     self.sc.append(sc)
-                self.log.info("Load the sc successful.")
+                if language == "en":
+                    self.log.info("Load the sc data successful.")
+                else:
+                    self.log.info("成功加载sc数据。")
 
     async def __load_guard(self, live_dir: str) -> None:
         """
         Load the guard.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Load the guard...")
+        self.log.info("Load the guard data...")
         guard_excel_file: str = os.path.join(live_dir, "guard.xlsx")
         if not os.path.exists(guard_excel_file):
-            self.log.warning("The guard data file not exist!")
+            if language == "en":
+                self.log.warning("There is no guard data, which may affect subsequent!")
+            else:
+                self.log.warning("没有舰长数据，这可能会影响后续操作！")
         else:
             guard_excel: DataFrame = pd.read_excel(guard_excel_file)
             if guard_excel.empty:
-                self.log.warning("There is no guard!")
+                if language == "en":
+                    self.log.warning("There is no guard data, which may affect subsequent!")
+                else:
+                    self.log.warning("没有舰长数据，这可能会影响后续操作！")
             else:
                 guard_list: list[dict] = guard_excel.to_dict(orient="records")
                 for elem in guard_list:
                     guard: BiliLiveGuard = BiliLiveGuard(log=self.log_file)
                     await guard.load_from_excel(elem)
                     self.guard.append(guard)
-                self.log.info("Load the guard successful.")
+                if language == "en":
+                    self.log.info("Load the guard data successful.")
+                else:
+                    self.log.info("成功加载舰长数据。")
 
     async def __load_view(self, live_dir: str) -> None:
         """
         Load the popularity.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Loading the popularity data...")
+        if language == "en":
+            self.log.info("Loading the popularity data...")
+        else:
+            self.log.info("正在加载人气数据...")
         view_txt_file: str = os.path.join(live_dir, "view.txt")
         if not os.path.exists(view_txt_file):
-            self.log.warning("The popularity data file not exist!")
+            if language == "en":
+                self.log.warning("There is no popularity data, which may affect subsequent!")
+            else:
+                self.log.warning("没有人气数据，这可能会影响后续操作！")
         else:
             with open(view_txt_file, "r") as f:
                 for elem in f.readlines():
                     content: list[str] = elem.removesuffix("\n").split(",")
                     if len(content) == 2:
                         if content[0].isdigit() and content[1].isdigit():
                             self.view.append(int(content[1]))
                             self.view_time.append(int(content[0]))
-            self.log.info("Load the popularity data successful.")
+            if language == "en":
+                self.log.info("Load the popularity data successful.")
+            else:
+                self.log.info("成功加载人气数据。")
 
     async def __load_output_dir(self, live_dir: str) -> None:
         """
         Load the test_output directory.
 
         Args:
             live_dir: directory for storing single live-streaming data
@@ -656,45 +771,57 @@
                 f.write("seconds from the start of the live, suggested content\n")
 
         self.sparse_suggestion_txt_file: str = os.path.join(self.output_dir, "sparse_suggestion.txt")
         if not os.path.exists(self.sparse_suggestion_txt_file):
             with open(self.sparse_suggestion_txt_file, "a") as f:
                 f.write("seconds from the start of the live, suggested content\n")
 
+    @wlw.async_separate()
     async def __load_data(self, live_dir: str) -> None:
         """
         Load the data of the live room from the work directory.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info(f"Loading data from {live_dir}...")
+        if language == "en":
+            self.log.info(f"Loading data from {live_dir}...")
+        else:
+            self.log.info(f"正在从{live_dir}加载数据...")
         st: str = os.path.split(live_dir)[-1]
         t = time.mktime(time.strptime(st, "%Y-%m-%d_%H-%M-%S"))
         self.start_time = int(t)
         await self.__load_danmu(live_dir)
         await self.__load_gift(live_dir)
         await self.__load_sc(live_dir)
         await self.__load_guard(live_dir)
         await self.__load_view(live_dir)
         await self.__load_output_dir(live_dir)
 
+    @wlw.async_separate()
     async def __danmu_robust_process(self, interval: float, live_dir: str) -> None:
         """
         Selecting marking danmu with a certain frequency.
 
         Args:
             interval: the minimum minute interval between two selected danmu
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info(f"Selecting the marked danmu every {interval} minute...")
+        if language == "en":
+            self.log.info(f"Selecting the marked danmu every {interval} minute...")
+        else:
+            self.log.info(f"每隔 {interval} 分钟选择被标记弹幕...")
         if not self.marked_danmu:
-            self.log.warning("There is no marked danmu and cannot be robust processed!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'marked_danmu.xlsx')} "
-                           f"exists and is not empty.")
+            if language == "en":
+                self.log.warning("There is no marked danmu and cannot be robust processed!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'marked_danmu.xlsx')} "
+                               f"exists and is not empty.")
+            else:
+                self.log.warning("没有被标记弹幕，无法筛选！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'marked_danmu.xlsx')} 是否存在且不为空。")
             return
 
         robust_danmu_excel_file: str = os.path.join(live_dir, "robust_danmu.xlsx")
         if not os.path.exists(robust_danmu_excel_file):
             temp_excel: DataFrame = pd.DataFrame()
             temp_excel.to_excel(robust_danmu_excel_file, index=False)
         robust_danmu_excel: DataFrame = pd.read_excel(robust_danmu_excel_file)
@@ -708,59 +835,93 @@
                 if danmu.time <= flag + interval * 60:
                     pass
                 else:
                     flag = danmu.time
                     self.robust_danmu.append(danmu)
                     await danmu.to_excel(robust_danmu_excel_file, robust_danmu_excel)
                     robust_danmu_excel = pd.read_excel(robust_danmu_excel_file)
-        self.log.info(f"Selecting the marked danmu successful. The result is saved in {robust_danmu_excel_file}.")
+        if language == "en":
+            self.log.info(f"Selecting the marked danmu successful. The result is saved in {robust_danmu_excel_file}.")
+        else:
+            self.log.info(f"被标记弹幕筛选成功。结果保存在 {robust_danmu_excel_file} 。")
 
+    @wlw.async_separate()
     async def __editing_suggestions(self) -> None:
         """
         Suggest the editing of the video, according to the danmu.
         """
         if not self.marked_danmu:
-            self.log.warning(
-                "No useful marked danmu sequence found, unable to provide complete suggestions for editing!")
+            if language == "en":
+                self.log.warning(
+                    "There is no complete marked danmu data, unable to provide complete suggestions for editing!")
+            else:
+                self.log.warning("没有完整的被标记弹幕数据，无法提供完整的剪辑建议！")
         else:
-            self.log.info("Providing complete suggestions for editing...")
+            if language == "en":
+                self.log.info("Providing complete suggestions for editing...")
+            else:
+                self.log.info("正在提供完整的剪辑建议...")
             for elem in self.marked_danmu:
                 with open(self.complete_suggestion_txt_file, "a") as f:
                     sug = str(elem.time - self.start_time) + ", " + elem.content + "\n"
                     f.write(sug)
-            self.log.info(f"Providing complete suggestions for editing successful. The result is saved in "
-                          f"{self.complete_suggestion_txt_file}.")
+            if language == "en":
+                self.log.info(f"Providing complete suggestions for editing successful. The result is saved in "
+                              f"{self.complete_suggestion_txt_file}.")
+            else:
+                self.log.info(f"成功提供完整的剪辑建议。结果保存在 {self.complete_suggestion_txt_file} 。")
 
         if not self.robust_danmu:
-            self.log.warning("No useful robust danmu sequence found, unable to provide sparse suggestions for editing!")
+            if language == "en":
+                self.log.warning("There is no robust marked danmu data found, "
+                                 "unable to provide sparse suggestions for editing!")
+            else:
+                self.log.warning("没有找到筛选后的被标记弹幕数据，无法提供稀疏的剪辑建议！")
         else:
-            self.log.info("Providing sparse suggestions for editing...")
+            if language == "en":
+                self.log.info("Providing sparse suggestions for editing...")
+            else:
+                self.log.info("正在提供稀疏的剪辑建议...")
             for elem in self.robust_danmu:
                 with open(self.sparse_suggestion_txt_file, "a") as f:
                     sug = str(elem.time - self.start_time) + ", " + elem.content + "\n"
                     f.write(sug)
-            self.log.info(f"Providing sparse suggestions for editing successful. The result is saved in "
-                          f"{self.sparse_suggestion_txt_file}.")
+            if language == "en":
+                self.log.info(f"Providing sparse suggestions for editing successful. The result is saved in "
+                              f"{self.sparse_suggestion_txt_file}.")
+            else:
+                self.log.info(f"成功提供稀疏的剪辑建议。结果保存在 {self.sparse_suggestion_txt_file} 。")
 
+    @wlw.async_separate()
     async def __complete_danmu_frequency_analysis(self, interval: float, live_dir: str) -> None:
         """
         Analyze the frequency of complete danmu.
 
         Args:
             interval: the second interval for danmu frequency analysis
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info(f"Analyzing the frequency of complete danmu...")
+        if language == "en":
+            self.log.info(f"Analyzing the frequency of complete danmu...")
+        else:
+            self.log.info("正在分析完整弹幕的频率...")
         if interval < 30:
-            self.log.warning("The interval is too small, it may cause the result image to fluctuate "
-                             "too much and reduce the perception.")
+            if language == "en":
+                self.log.warning("The interval is too small, it may cause the result image to fluctuate "
+                                 "too much and reduce the perception.")
+            else:
+                self.log.warning("间隔过小，可能导致结果图像波动过大，降低感知。")
         if not self.danmu:
-            self.log.warning("There is no complete danmu data, and frequency could not be performed!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'danmu.xlsx')} "
-                           f"exists and is not empty.")
+            if language == "en":
+                self.log.warning("There is no complete danmu data, and frequency could not be performed!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'danmu.xlsx')} "
+                               f"exists and is not empty.")
+            else:
+                self.log.warning("没有完整弹幕数据，无法进行频率分析！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'danmu.xlsx')} 是否存在且不为空。")
         else:
             count_list: list[int] = []
             count: int = 1
             time_list: list[int] = []
             time_flag: int = self.danmu[0].time
             time_list.append(time_flag)
             if len(self.danmu) > 1:
@@ -775,58 +936,89 @@
                 count_list.append(count)
             else:
                 count_list.append(count)
             time_list = [time_list[i] - self.start_time for i in range(len(time_list))]
 
             plt.figure(figsize=(1080 / 200, 720 / 200), dpi=200)
             plt.plot(time_list, count_list)
-            plt.xlabel("Time")
-            plt.ylabel("Count")
-            plt.title("Complete Danmu Frequency Analysis (Original)")
+            if language == "en":
+                plt.xlabel("Time")
+                plt.ylabel("Count")
+                plt.title("Complete Danmu Frequency Analysis (Original)")
+            else:
+                plt.xlabel("时间")
+                plt.ylabel("数量")
+                plt.title("完整弹幕频率分析（原始）")
             original_name: str = os.path.join(self.output_dir, "complete_danmu_frequency_analysis_original.jpg")
             plt.savefig(original_name)
 
-            if len(time_list) > 3:
+            if len(time_list) > 30:
                 x_new = np.linspace(time_list[0], time_list[-1], 500)
                 y_new = spi.make_interp_spline(time_list, count_list)(x_new)
                 plt.figure(figsize=(2160 / 200, 1440 / 200), dpi=200)
                 plt.plot(x_new, y_new)
-                plt.xlabel("Time")
-                plt.ylabel("Count")
-                plt.title("Complete Danmu Frequency Analysis (Smooth)")
+                if language == "en":
+                    plt.xlabel("Time")
+                    plt.ylabel("Count")
+                    plt.title("Complete Danmu Frequency Analysis (Smooth)")
+                else:
+                    plt.xlabel("时间")
+                    plt.ylabel("数量")
+                    plt.title("完整弹幕频率分析（平滑）")
                 smooth_name: Union[str, None] = os.path.join(self.output_dir,
                                                              "complete_danmu_frequency_analysis_smooth.jpg")
                 plt.savefig(smooth_name)
             else:
-                self.log.warning("There is too little data to smooth out the complete danmu frequency analysis!")
+                if language == "en":
+                    self.log.warning("There is too little data to smooth out the complete danmu frequency analysis!")
+                else:
+                    self.log.warning("数据量太少，无法对完整弹幕频率分析进行平滑化！")
                 smooth_name = None
 
             if smooth_name is not None:
-                self.log.info(f"The analysis of complete danmu frequency is completed, and the original result graph is "
-                              f"saved as {original_name} while the smoothing result map is saved as {smooth_name}.")
+                if language == "en":
+                    self.log.info(f"The analysis of complete danmu frequency is completed, and the original result "
+                                  f"graph is saved as {original_name} while the smoothing result map is saved "
+                                  f"as {smooth_name}.")
+                else:
+                    self.log.info(f"完成完整弹幕频率分析，原始结果图保存为 {original_name} ，平滑结果图保存为 {smooth_name} 。")
             else:
-                self.log.info(f"The analysis of complete danmu frequency is completed, and the original result graph is "
-                              f"saved as {original_name}.")
+                if language == "en":
+                    self.log.info(f"The analysis of complete danmu frequency is completed, and the original result "
+                                  f"graph is saved as {original_name}.")
+                else:
+                    self.log.info(f"完成完整弹幕频率分析，结果图保存为 {original_name} 。")
 
+    @wlw.async_separate()
     async def __marked_danmu_frequency_analysis(self, interval: float, live_dir: str) -> None:
         """
         Analyze the frequency of marked danmu.
 
         Args:
             interval: the second interval for danmu frequency analysis
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Analyzing the frequency of marked danmu...")
+        if language == "en":
+            self.log.info("Analyzing the frequency of marked danmu...")
+        else:
+            self.log.info("正在分析被标记弹幕的频率...")
         if interval < 30:
-            self.log.warning("The interval is too small, it may cause the result image to fluctuate "
-                             "too much and reduce the perception.")
+            if language == "en":
+                self.log.warning("The interval is too small, it may cause the result image to fluctuate "
+                                 "too much and reduce the perception.")
+            else:
+                self.log.warning("间隔过小，可能导致结果图像波动过大，降低感知。")
         if not self.marked_danmu:
-            self.log.warning("There is no marked danmu data, and frequency could not be performed!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'marked_danmu.xlsx')} "
-                           f"exists and is not empty.")
+            if language == "en":
+                self.log.warning("There is no marked danmu data, and frequency could not be performed!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'marked_danmu.xlsx')} "
+                               f"exists and is not empty.")
+            else:
+                self.log.warning("没有被标记弹幕数据，无法进行频率分析！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'marked_danmu.xlsx')} 是否存在且不为空。")
         else:
             count_mark_list: list[int] = []
             count: int = 1
             time_list: list[int] = []
             time_flag: int = self.marked_danmu[0].time
             time_list.append(time_flag)
             if len(self.marked_danmu) > 1:
@@ -841,79 +1033,110 @@
                 count_mark_list.append(count)
             else:
                 count_mark_list.append(count)
             time_list = [time_list[i] - self.start_time for i in range(len(time_list))]
 
             plt.figure(figsize=(2160 / 200, 1440 / 200), dpi=200)
             plt.plot(time_list, count_mark_list)
-            plt.xlabel("Time")
-            plt.ylabel("Count")
-            plt.title("Marked Danmu Frequency Analysis (Original)")
+            if language == "en":
+                plt.xlabel("Time")
+                plt.ylabel("Count")
+                plt.title("Marked Danmu Frequency Analysis (Original)")
+            else:
+                plt.xlabel("时间")
+                plt.ylabel("数量")
+                plt.title("被标记弹幕频率分析（原始）")
             original_name: str = os.path.join(self.output_dir, "marked_danmu_frequency_analysis_original.jpg")
             plt.savefig(original_name)
 
-            if len(time_list) > 3:
+            if len(time_list) > 30:
                 x_new = np.linspace(time_list[0], time_list[-1], 500)
                 y_new = spi.make_interp_spline(time_list, count_mark_list)(x_new)
                 plt.figure(figsize=(2160 / 200, 1440 / 200), dpi=200)
                 plt.plot(x_new, y_new)
-                plt.xlabel("Time")
-                plt.ylabel("Count")
-                plt.title("Marked Danmu Frequency Analysis (Smooth)")
+                if language == "en":
+                    plt.xlabel("Time")
+                    plt.ylabel("Count")
+                    plt.title("Marked Danmu Frequency Analysis (Smooth)")
+                else:
+                    plt.xlabel("时间")
+                    plt.ylabel("数量")
+                    plt.title("被标记弹幕频率分析（平滑）")
                 smooth_name: Union[str, None] = os.path.join(self.output_dir,
                                                              "marked_danmu_frequency_analysis_smooth.jpg")
                 plt.savefig(smooth_name)
             else:
-                self.log.warning("There is too little data to smooth out the marbled danmu frequency analysis!")
+                if language == "en":
+                    self.log.warning("There is too little data to smooth out the marbled danmu frequency analysis!")
+                else:
+                    self.log.warning("数据量太少，无法对被标记弹幕频率分析进行平滑化！")
                 smooth_name = None
 
             if smooth_name is not None:
-                self.log.info(f"The analysis of marked danmu frequency is completed, and the original result graph is "
-                              f"saved as {original_name} while the smoothing result map is saved as {smooth_name}.")
+                if language == "en":
+                    self.log.info(f"The analysis of marked danmu frequency is completed, and the original result "
+                                  f"graph is saved as {original_name} while the smoothing result map is saved "
+                                  f"as {smooth_name}.")
+                else:
+                    self.log.info(f"完成被标记弹幕频率分析，原始结果图保存为 {original_name} ，平滑结果图保存为 {smooth_name} 。")
             else:
-                self.log.info(f"The analysis of marked danmu frequency is completed, and the original result graph is "
-                              f"saved as {original_name}.")
+                if language == "en":
+                    self.log.info(f"The analysis of marked danmu frequency is completed, and the original result "
+                                  f"graph is saved as {original_name}.")
+                else:
+                    self.log.info(f"完成被标记弹幕频率分析，结果图保存为 {original_name} 。")
 
     async def __danmu_frequency_analysis(self, interval: float, live_dir: str) -> None:
         """
         Analyze the frequency of danmu.
 
         Args:
             interval: the second interval for danmu frequency analysis
             live_dir: directory for storing single live-streaming data
         """
         await self.__complete_danmu_frequency_analysis(interval, live_dir)
         await self.__marked_danmu_frequency_analysis(interval, live_dir)
 
+    @wlw.async_separate()
     async def __danmu_word_cloud(self, live_dir: str, mask: Union[npt.NDArray, None]) -> None:
         """
         Generate word cloud of danmu.
 
         Args:
             live_dir: directory for storing single live-streaming data
             mask: mask for word cloud
         """
         if self.danmu:
-            self.log.info("Generating word cloud of complete danmu...")
+            if language == "en":
+                self.log.info("Generating word cloud of complete danmu...")
+            else:
+                self.log.info("正在生成完整弹幕词云...")
             danmu_content: str = ""
             for elem in self.danmu:
                 danmu_content += elem.content
                 danmu_content += " "
             words: list[str] = jieba.lcut(danmu_content)
             word_freq = pd.Series(words).value_counts()
             wc = wordcloud.WordCloud(font_path='PingFang.ttc', background_color='white', mask=mask)
             wc.generate_from_frequencies(word_freq)
             image = wc.to_image()
             save_path: str = os.path.join(self.output_dir, "complete_danmu_word_cloud.jpg")
             image.save(save_path, quality=100)
-            self.log.info(f"The word cloud image of complete danmu is generated and saved as {save_path}.")
+            if language == "en":
+                self.log.info(f"Word cloud image of complete danmu generation completed and saved as {save_path}.")
+            else:
+                self.log.info(f"完整弹幕词云图生成完成，保存为 {save_path} 。")
         else:
-            self.log.warning("There is no complete danmu data, and word cloud could not be generated!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'complete_danmu.xlsx')} "
-                           f"exists and is not empty.")
+            if language == "en":
+                self.log.warning("There is no complete danmu data, and word cloud could not be generated!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'complete_danmu.xlsx')} "
+                               f"exists and is not empty.")
+            else:
+                self.log.warning("没有完整弹幕数据，无法生成词云！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'complete_danmu.xlsx')} 是否存在且不为空。")
 
     async def __merge_revenue(self) -> None:
         """
         Merge the gift, sc, guard of live-streaming rooms.
         """
         gift = self.gift.copy()
         sc = self.sc.copy()
@@ -944,30 +1167,40 @@
                 self.revenue += guard
             else:
                 self.revenue += guard
         else:
             if temp:
                 self.revenue += temp
 
+    @wlw.async_separate()
     async def __revenue_stat_by_time(self, interval: float, live_dir: str) -> None:
         """
         Analyze revenue from live-streaming rooms by time.
 
         Args:
             interval: the minute interval for gift analysis
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Analyzing revenue from live-streaming rooms by time...")
+        if language == "en":
+            self.log.info("Analyzing revenue from live-streaming rooms by time...")
+        else:
+            self.log.info("正在分析直播间收益按时间分布...")
         await self.__merge_revenue()
         if not self.revenue:
-            self.log.warning("There is no revenue data!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'gift.xlsx')}"
-                           f", {os.path.join(live_dir, 'sc.xlsx')} "
-                           f"and {os.path.join(live_dir, 'guard.xlsx')} "
-                           f"exist and are not empty.")
+            if language == "en":
+                self.log.warning("There is no revenue data!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'gift.xlsx')}"
+                               f", {os.path.join(live_dir, 'sc.xlsx')} "
+                               f"and {os.path.join(live_dir, 'guard.xlsx')} "
+                               f"exist and are not empty.")
+            else:
+                self.log.warning("没有收益数据！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'gift.xlsx')}、"
+                               f"{os.path.join(live_dir, 'sc.xlsx')} 和 "
+                               f"{os.path.join(live_dir, 'guard.xlsx')} 是否存在且不为空。")
         else:
             count_list: list[int] = []
             count: int = 1
             time_list: list[int] = []
             time_flag: int = self.revenue[0].time
             time_list.append(time_flag)
             if len(self.revenue) > 1:
@@ -982,27 +1215,39 @@
                 count_list.append(count)
             else:
                 count_list.append(count)
             time_list = [time_list[i] - self.start_time for i in range(len(time_list))]
 
             plt.figure(figsize=(2160 / 200, 1440 / 200), dpi=200)
             plt.plot(time_list, count_list)
-            plt.xlabel("Time")
-            plt.ylabel("Count")
-            plt.title("Revenue Analysis (Original)")
+            if language == "en":
+                plt.xlabel("Time")
+                plt.ylabel("Count")
+                plt.title("Revenue Analysis (Original)")
+            else:
+                plt.xlabel("时间")
+                plt.ylabel("数量")
+                plt.title("收益分析（原始）")
             original_name: str = os.path.join(self.output_dir, "revenue_analysis_original.jpg")
             plt.savefig(original_name)
-            self.log.info(f"The analysis of revenue by time is completed, and the original result graph is "
-                          f"saved as {original_name}.")
+            if language == "en":
+                self.log.info(f"The analysis of revenue by time is completed, and the original result graph is "
+                              f"saved as {original_name}.")
+            else:
+                self.log.info(f"直播间收益按时间分布分析完成，原始结果图保存为 {original_name} 。")
 
-    async def _revenue_stat_by_price(self) -> None:
+    @wlw.async_separate()
+    async def _revenue_stat_by_user(self) -> None:
         """
-        Analyze the situation of live-streaming gifts by price.
+        Analyze the situation of live-streaming gifts by user.
         """
-        self.log.info("Analyzing the situation of live-streaming gifts by price...")
+        if language == "en":
+            self.log.info("Analyzing revenue from live-streaming room by user...")
+        else:
+            self.log.info("正在按用户分析直播间收益...")
         revenue: dict[int, float] = {}
         if self.gift:
             for elem in self.gift:
                 if elem.user_uid not in revenue:
                     revenue[elem.user_uid] = elem.price
                 else:
                     revenue[elem.user_uid] += elem.price
@@ -1032,19 +1277,26 @@
             else:
                 count_list[4] += 1
         label_list: list[str] = ["0-50", "50-200", "200-500", "500-2000", "2000+"]
         idx: npt.NDArray = np.nonzero(count_list)[0]
         plt.pie(np.array(count_list)[idx], labels=np.array(label_list, dtype=str)[idx], autopct='%1.2f%%',
                 explode=[0.1 for _ in range(len(np.array(count_list)[idx]))], shadow=False, labeldistance=1.06)
         plt.axis("equal")
-        plt.title("Revenue Analysis by Price")
-        name: str = os.path.join(self.output_dir, "revenue_analysis_by_price.jpg")
+        if language == "en":
+            plt.title("Revenue Analysis by User")
+        else:
+            plt.title("收益分析（按用户）")
+        name: str = os.path.join(self.output_dir, "revenue_analysis_by_user.jpg")
         plt.savefig(name, dpi=300)
-        self.log.info(f"The analysis of revenue by price is completed, and the result graph is saved as {name}.")
+        if language == "en":
+            self.log.info(f"The analysis of revenue by user is completed, and the result graph is saved as {name}.")
+        else:
+            self.log.info(f"直播间收益按用户分布分析完成，结果图保存为 {name} 。")
 
+    @wlw.async_separate()
     async def __revenue_stat_by_type(self) -> None:
         """
         Analyze the situation of live-streaming gifts by type.
         """
         gift_total_price: float = 0
         sc_total_price: float = 0
         guard_total_price: float = 0
@@ -1055,58 +1307,80 @@
             for sc in self.sc:
                 sc_total_price += sc.price
         if self.guard:
             for guard in self.guard:
                 guard_total_price += guard.price
 
         price_list: list[float] = [gift_total_price, sc_total_price, guard_total_price]
-        label_list: list[str] = ["Gift", "Super Chat", "Guard"]
+        if language == "en":
+            label_list: list[str] = ["Gift", "Super Chat", "Guard"]
+        else:
+            label_list: list[str] = ["礼物", "SC", "舰长"]
         idx: npt.NDArray = np.nonzero(price_list)[0]
         plt.pie(np.array(price_list)[idx], labels=np.array(label_list, dtype=str)[idx], autopct='%1.2f%%',
                 explode=[0.1 for _ in range(len(np.array(price_list)[idx]))], shadow=False, labeldistance=1.06)
         plt.axis("equal")
-        plt.title("Revenue Analysis by Type")
+        if language == "en":
+            plt.title("Revenue Analysis by Type")
+        else:
+            plt.title("收益分析（按类型）")
         name: str = os.path.join(self.output_dir, "revenue_analysis_by_type.jpg")
         plt.savefig(name, dpi=300)
         self.log.info(f"The analysis of revenue by type is completed, and the result graph is saved as {name}.")
 
     async def __revenue_stat(self, interval: float, live_dir: str) -> None:
         """
         Analyze revenue from live-streaming rooms.
 
         Args:
             interval: the minute interval for revenue analysis
             live_dir: directory for storing single live-streaming data
         """
         await self.__revenue_stat_by_time(interval, live_dir)
-        # await self._revenue_stat_by_price()  # TODO: Waiting for interface modification of bilibili-api-python
+        # await self._revenue_stat_by_user()  # TODO: Waiting for interface modification of bilibili-api-python
         await self.__revenue_stat_by_type()
 
+    @wlw.async_separate()
     async def __view_stat(self, live_dir: str) -> None:
         """
         Analyze the number of viewers in live-streaming rooms.
 
         Args:
             live_dir: directory for storing single live-streaming data
         """
-        self.log.info("Analyzing the popularity of the live broadcast room...")
+        if language == "en":
+            self.log.info("Analyzing the popularity of the live broadcast room...")
+        else:
+            self.log.info("正在分析直播间人气...")
         if not self.view:
-            self.log.warning("There is no popularity data!")
-            self.log.error(f"Please check that {os.path.join(live_dir, 'view.txt')} "
-                           f"exists and is not empty.")
+            if language == "en":
+                self.log.warning("There is no popularity data!")
+                self.log.error(f"Please check that {os.path.join(live_dir, 'view.txt')} "
+                               f"exists and is not empty.")
+            else:
+                self.log.warning("没有人气数据！")
+                self.log.error(f"请检查 {os.path.join(live_dir, 'view.txt')} 是否存在且不为空。")
         else:
             view_time: list[int] = [self.view_time[i] - self.start_time for i in range(len(self.view_time))]
             plt.figure(figsize=(2160 / 200, 1440 / 200), dpi=200)
             plt.plot(view_time, self.view)
-            plt.xlabel("Time")
-            plt.ylabel("Popularity")
-            plt.title("Popularity Analysis")
+            if language == "en":
+                plt.xlabel("Time")
+                plt.ylabel("Popularity")
+                plt.title("Popularity Analysis")
+            else:
+                plt.xlabel("时间")
+                plt.ylabel("人气")
+                plt.title("人气分析")
             name: str = os.path.join(self.output_dir, "popularity_analysis.jpg")
             plt.savefig(name)
-            self.log.info(f"The analysis of popularity is completed, and the result graph is saved as {name}.")
+            if language == "en":
+                self.log.info(f"The analysis of popularity is completed, and the result graph is saved as {name}.")
+            else:
+                self.log.info(f"人气分析完成，结果图保存为 {name} 。")
 
     async def analysis(self, revenue_interval: float, danmu_interval: float, robust: bool,
                        robust_interval: float, mask: Union[npt.NDArray, None]) -> None:
         """
         Analyze the live-streaming room.
 
         Args:
@@ -1123,8 +1397,11 @@
                     await self.__danmu_robust_process(robust_interval, live_dir)
                 await self.__revenue_stat(revenue_interval, live_dir)
                 await self.__view_stat(live_dir)
                 await self.__danmu_frequency_analysis(danmu_interval, live_dir)
                 await self.__editing_suggestions()
                 await self.__danmu_word_cloud(live_dir, mask)
         else:
-            self.log.warning("No unprocessed data!")
+            if language == "en":
+                self.log.warning("No unprocessed data!")
+            else:
+                self.log.warning("没有未处理的数据！")
```

### Comparing `bili-uas-0.1.9/Bili_UAS/utils/search_utils.py` & `bili-uas-0.2.0/Bili_UAS/utils/search_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,25 @@
 """
 
 
 from __future__ import annotations
 from bilibili_api import search as bas
 from Bili_UAS.writer import log_writer as lw
 import time
+from typing import Union
 
 
 class BiliSearch(object):
     """
     Bilibili Search Class
     """
     def __init__(self, keywords: list[str], log: str) -> None:
         self.keywords: list[str] = keywords
         self.log_file: str = log
-        self.log: lw.Logger = None
+        self.log: Union[lw.Logger, None] = None
         self.__set_log()
 
         self.video_id: list[str] = []
 
     def __set_log(self) -> None:
         """
         Set up logs.
```

### Comparing `bili-uas-0.1.9/Bili_UAS/utils/user_utils.py` & `bili-uas-0.2.0/Bili_UAS/utils/user_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,26 +8,39 @@
 # data test_output path template: user_output/{user_id}/file_name: {fans_num.txt, guard_num.txt, charge_num.txt,
 #                                                             address.xlsx, address_unreceived.txt}
 # fans_num.txt content format: {time},{fans_num}
 # guard_num.txt content format: {time},{guard_total_num},{governor_num},{supervisor_num},{captain_num}
 
 
 from __future__ import annotations
+import enum
 from bilibili_api import user as bau, live as bal, sync
-from Bili_UAS.writer import log_writer as lw
+from .config_utils import load_language_from_txt
+from Bili_UAS.writer import log_writer as wlw
 from bilibili_api import Credential, session
 import os
 import time
 from bilibili_api.exceptions import (CredentialNoBiliJctException, CredentialNoSessdataException,
                                      CredentialNoBuvid3Exception, CredentialNoDedeUserIDException)
 import pandas as pd
 from pandas import DataFrame
 from typing import Union
 
 
+language: str = load_language_from_txt()
+
+
+class AddressProcessType(enum.Enum):
+    """
+
+    """
+    SEND = 1
+    RECEIVE = 2
+
+
 async def _address_mag_simple_check(msg: list[str]) -> bool:
     """
     Check if it is address information.
 
     Args:
         msg: message list
 
@@ -56,15 +69,15 @@
         """
         Args:
             uid: user ID
             log: log file path
             credential: logon credentials
         """
         self.log_file: str = log
-        self.log: Union[lw.Logger, None] = None
+        self.log: Union[wlw.Logger, None] = None
         self.__set_log()
 
         bau.User.__init__(self, uid, credential)
         self.uid: int = uid
         self.room_id: Union[int, None] = None
         self.work_dir: Union[str, None] = None
         self.__live_init()
@@ -81,22 +94,22 @@
         self.__load_work_dir(work_dir)
         sync(self.__load_output_file())
 
     def __set_log(self) -> None:
         """
         Set up logs.
         """
-        file_handler: lw.Handler = lw.Handler("file")
+        file_handler: wlw.Handler = wlw.Handler("file")
         file_handler.set_level("WARNING", "ERROR")
         file_handler.set_file(self.log_file)
 
-        sys_handler: lw.Handler = lw.Handler("sys")
+        sys_handler: wlw.Handler = wlw.Handler("sys")
         sys_handler.set_level("INFO", "WARNING")
 
-        self.log: lw.Logger = lw.Logger()
+        self.log: wlw.Logger = wlw.Logger()
         self.log.add_config(file_handler)
         self.log.add_config(sys_handler)
 
     def __load_work_dir(self, work_dir: str) -> None:
         """
         Load the working directory.
 
@@ -113,48 +126,63 @@
 
     def __live_init(self) -> None:
         """
         Initialize live room.
         """
         live_info: dict = sync(self.get_live_info())
         if live_info['live_room'] is None:
-            self.log.warning("The user has not opened a live streaming room!")
+            if language == "en":
+                self.log.warning("The user has not opened a live streaming room!")
+            else:
+                self.log.warning("用户未开通直播间！")
             return
         self.room_id = live_info['live_room']['roomid']
         bal.LiveRoom.__init__(self, self.room_id, self.credential)
 
     async def __check_credentials(self) -> bool:
         """
         Check if the credentials are valid.
 
         Returns:
             True if the credentials are valid, False otherwise.
         """
         try:
             await self.credential.raise_for_no_sessdata()
         except CredentialNoSessdataException:
-            self.log.warning("Credential missing SESSDATA!")
+            if language == "en":
+                self.log.warning("Credential missing SESSDATA!")
+            else:
+                self.log.warning("登录信息缺少SESSDATA！")
             return False
 
         try:
             await self.credential.raise_for_no_bili_jct()
         except CredentialNoBiliJctException:
-            self.log.warning("Credential missing bili_jct!")
+            if language == "en":
+                self.log.warning("Credential missing bili_jct!")
+            else:
+                self.log.warning("登录信息缺少bili_jct！")
             return False
 
         try:
             await self.credential.raise_for_no_buvid3()
         except CredentialNoBuvid3Exception:
-            self.log.warning("Credential missing buvid3!")
+            if language == "en":
+                self.log.warning("Credential missing buvid3!")
+            else:
+                self.log.warning("登录信息缺少buvid3！")
             return False
 
         try:
             await self.credential.raise_for_no_dedeuserid()
         except CredentialNoDedeUserIDException:
-            self.log.warning("Credential missing DedeUserID!")
+            if language == "en":
+                self.log.warning("Credential missing DedeUserID!")
+            else:
+                self.log.warning("登录信息缺少DedeUserID！")
             return False
 
         return True
 
     async def __load_output_file(self) -> None:
         """
         Load the test_output file.
@@ -181,57 +209,74 @@
         self.address_excel: DataFrame = pd.read_excel(self.address_excel_file)
 
         self.address_unreceived_txt_file: str = os.path.join(self.work_dir, "address_unreceived.txt")
         if not os.path.exists(self.address_unreceived_txt_file):
             with open(self.address_unreceived_txt_file, "a") as f:
                 f.write("uid,bili_name\n\n")
 
+    @wlw.async_separate()
     async def get_upload_videos(self):
         """
         Get all videos uploaded by this user.
         """
-        self.log.info(f"Start getting all videos uploaded by user {self.uid}...")
+        if language == "en":
+            self.log.info(f"Start getting all videos uploaded by user {self.uid}...")
+        else:
+            self.log.info(f"开始获取用户 {self.uid} 上传的所有视频...")
         page: int = 1
         count: int = 0
         while True:
             video_data: dict = await self.get_videos(pn=page)
-            if video_data:
-                if video_data['list']['vlist']:
-                    for video in video_data['list']['vlist']:
-                        self.video_id.append(video['bvid'])
-                        count += 1
-                else:
-                    break
-                if count >= video_data['page']['count']:
-                    break
-                page += 1
+            if video_data['list']['vlist']:
+                for video in video_data['list']['vlist']:
+                    self.video_id.append(video['bvid'])
+                    count += 1
             else:
                 break
-        self.log.info(f"A total of {len(self.video_id)} videos were obtained.")
+            if count >= video_data['page']['count']:
+                break
+            page += 1
+        if language == "en":
+            self.log.info(f"A total of {len(self.video_id)} videos were obtained.")
+        else:
+            self.log.info(f"共获取到 {len(self.video_id)} 个视频。")
 
+    @wlw.async_separate()
     async def update_fans_number(self) -> None:
         """
         Update the number of fans.
         """
         now_time: int = int(time.time())
+        if language == "en":
+            self.log.info(f"Start getting the number of fans of user {self.uid}...")
+        else:
+            self.log.info(f"开始获取用户 {self.uid} 的粉丝数...")
         relation_info: dict = await self.get_relation_info()
-        if relation_info:
-            fans_num = relation_info['follower']
+        fans_num = relation_info['follower']
+        if fans_num:
             with open(self.fans_num_txt_file, "a") as f:
                 f.write(f"{time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime(now_time))},{fans_num}\n")
         else:
-            self.log.warning("Failed to update fans number!")
+            if language == "en":
+                self.log.warning("Failed to get the number of fans!")
+            else:
+                self.log.warning("获取粉丝数失败！")
 
+    @wlw.async_separate()
     async def update_guard_number(self) -> None:
         """
         Update the number of guards.
         """
         now_time: int = int(time.time())
+        if language == "en":
+            self.log.info(f"Start getting the number of guards of user {self.uid}...")
+        else:
+            self.log.info(f"开始获取用户 {self.uid} 的舰长数...")
         guard_info: dict = await self.get_dahanghai(page=1)
-        total_page: int = guard_info['info']['page']
+        total_page: int = guard_info['info']['page']  # TODO: need to check guard_info is not empty
         guard_num: int = guard_info['info']['num']
         governor_num: int = 0
         supervisor_num: int = 0
         flag: bool = True
         for elem in guard_info['top3']:
             if elem['guard_level'] == 1:
                 governor_num += 1
@@ -251,61 +296,80 @@
                     elif elem['guard_level'] == 3:
                         break
         captain_num: int = guard_num - governor_num - supervisor_num
         with open(self.guard_num_txt_file, "a") as f:
             f.write(f"{time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime(now_time))},{guard_num},{governor_num},"
                     f"{supervisor_num},{captain_num}\n")
 
+    @wlw.async_separate()
     async def update_charge_number(self) -> None:
         """
         Update the number of charges.
         """
         now_time: int = int(time.time())
-        charge_info: dict = await self.get_elec_user_monthly()
-        if charge_info:
-            charge_num: int = charge_info['total_count']
-            with open(self.charge_num_txt_file, "a") as f:
-                f.write(f"{time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime(now_time))},{charge_num}\n")
+        if language == "en":
+            self.log.info(f"Start getting the number of charging member of user {self.uid}...")
         else:
-            self.log.warning("Failed to update charge number!")
+            self.log.info(f"开始获取用户 {self.uid} 的充电人数...")
+        charge_info: dict = await self.get_elec_user_monthly()
+        charge_num: int = charge_info['total_count']
+        with open(self.charge_num_txt_file, "a") as f:
+            f.write(f"{time.strftime('%Y-%m-%d_%H-%M-%S', time.localtime(now_time))},{charge_num}\n")
 
+    @wlw.async_separate()
     async def guard_address_stat_send(self) -> None:
         """
         Send address statistics to the guard.
         """
-        self.log.info(f"Start sending address statistics to the guard...")
+        if language == "en":
+            self.log.info(f"Start sending address statistics to the guard...")
+        else:
+            self.log.info(f"开始向舰长发送地址统计信息...")
         if not await self.__check_credentials():
-            self.log.warning("Credential error, unable to perform address statistics!")
+            if language == "en":
+                self.log.warning("Credential error, unable to perform address statistics!")
+            else:
+                self.log.warning("登录信息错误，无法进行地址统计！")
             return
 
         msg: str = "请按以下顺序输入地址信息：收件人，电话，地址。每项之间换行。示例：\n收件人：图图\n电话：123456\n地址：翻斗花园"
         guard_info: dict = await self.get_dahanghai(page=1)
         total_page: int = guard_info['info']['page']
         for elem in guard_info['top3']:
             target_uid: int = elem['uid']
             await session.send_msg(self.credential, target_uid, "1", msg)
         for i in range(1, total_page + 1):
-            guard_info: dict = await self.get_dahanghai(page=i)
+            guard_info: dict = await self.get_dahanghai(page=i)  # TODO: need to check guard_info is not empty
             for elem in guard_info['list']:
                 target_uid: int = elem['uid']
                 await session.send_msg(self.credential, target_uid, "1", msg)
-        self.log.info(f"Send successfully.")
+        if language == "en":
+            self.log.info(f"Send successfully.")
+        else:
+            self.log.info(f"发送成功。")
 
+    @wlw.async_separate()
     async def guard_address_stat_receive(self) -> None:
         """
         Receive address statistics from the guard.
         """
-        self.log.info("Start receiving address statistics to the guard")
+        if language == "en":
+            self.log.info("Start receiving address statistics to the guard")
+        else:
+            self.log.info("开始接收舰长的地址统计信息")
         if not await self.__check_credentials():
-            self.log.warning("Credential error, unable to receive address statistics!")
+            if language == "en":
+                self.log.warning("Credential error, unable to receive address statistics!")
+            else:
+                self.log.warning("登录信息错误，无法接收地址信息！")
             return
 
         receive_flag: bool = False
         count: int = 0
-        guard_info: dict = await self.get_dahanghai(page=1)
+        guard_info: dict = await self.get_dahanghai(page=1)  # TODO: need to check guard_info is not empty
         total_page: int = guard_info['info']['page']
         guard_num: int = guard_info['info']['num']
         for elem in guard_info['top3']:
             target_uid: int = elem['uid']
             target_name: str = elem['username']
             receive_info = await session.fetch_session_msgs(target_uid, self.credential)
             msg_list: list[dict] = receive_info['messages']
@@ -353,12 +417,19 @@
                         receive_flag = True
                         break
                 if not receive_flag:
                     with open(self.address_unreceived_txt_file, "a") as f:
                         f.write(f"{target_uid},{target_name}\n")
                 receive_flag = False
         if count == guard_num:
-            self.log.info(f"Receive successfully. All addresses have been received, but may still contain invalid "
-                          f"addresses that require manual inspection.")
+            if language == "en":
+                self.log.info(f"Receive successfully. All addresses have been received, but may still contain invalid "
+                              f"addresses that require manual inspection.")
+            else:
+                self.log.info(f"接收成功。已经接收到所有地址，但仍可能需要人工检查是否含有无效地址。")
         else:
-            self.log.warning(f"Receive successfully. But only {count} address messages were received in total. "
-                             f"Guard whose address is not receives are recorded in {self.address_unreceived_txt_file}.")
+            if language == "en":
+                self.log.warning(f"Receive successfully. But only {count} address messages were received in total. "
+                                 f"Guard whose address is not receives are recorded in {self.address_unreceived_txt_file}.")
+            else:
+                self.log.warning(f"接收成功。但总共只接收到了{count}个地址信息。"
+                                 f"未接收到地址信息的舰长记录在 {self.address_unreceived_txt_file} 中。")
```

### Comparing `bili-uas-0.1.9/Bili_UAS/utils/utils.py` & `bili-uas-0.2.0/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.9/Bili_UAS/utils/video_utils.py` & `bili-uas-0.2.0/Bili_UAS/utils/video_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,76 +4,70 @@
 This module provides the BiliVideo class, which is used to get video information, danmu, replies and tags.
 """
 
 
 from __future__ import annotations
 import numpy as np
 from .utils import BiliVideoReply, BiliVideoDanmu, BiliVideoTag
-from Bili_UAS.writer import log_writer as lw, abnormal_monitor as am
+from .config_utils import load_language_from_txt, load_ffmpeg_path_from_txt
+from Bili_UAS.writer import log_writer as wlw
 import time
 import copy
 import re
 from bilibili_api import Credential, video as bav, sync, Danmaku, comment as bac, HEADERS
 import pandas as pd
 from pandas import DataFrame
 import os
 from typing import Union
 import httpx
 import enum
 
 
+language: str = load_language_from_txt()
+
+
+@wlw.async_separate()
 async def _download_video_from_url(video_url: str,
                                    output_file: str,
                                    video_pid: int,
-                                   log: lw.Logger,
+                                   log: wlw.Logger,
                                    prompt_prefix: str) -> None:
     """
     Download video through url.
 
     Args:
         video_url: download url for video
         output_file: the path to save the video
         video_pid: pid of video
         log: the log class
     """
-    log.info(f"{video_pid} {prompt_prefix} downloading...")
+    if language == "en":
+        log.info(f"{video_pid} {prompt_prefix} downloading...")
+    else:
+        log.info(f"{video_pid} {prompt_prefix} 正在下载...")
     async with httpx.AsyncClient(headers=HEADERS) as sess:
         resp = await sess.get(video_url)
         length = resp.headers.get('content-length')
 
         with open(output_file, 'wb') as f:
             process = 0
             for chunk in resp.iter_bytes(1024):
                 if not chunk:
                     break
                 process += len(chunk)
-                log.info(f"{video_pid} {prompt_prefix} downloading... {process} / {length}")
+                if language == "en":
+                    log.info(f"{video_pid} {prompt_prefix} downloading... {process} / {length}")
+                else:
+                    log.info(f"{video_pid} {prompt_prefix} 正在下载... {process} / {length}")
                 f.write(chunk)
 
-    log.info(f"{video_pid} {prompt_prefix} download successfully.")
-
-
-async def _load_ffmpeg_path_from_txt(log: lw.Logger) -> str:
-    """
-    Load the ffmpeg path.
-
-    Args:
-        log: the log class
-
-    Returns:
-        the path of ffmpeg
-    """
-    ffmpeg_file: str = ".ffmpeg.txt"
-    if not os.path.exists(ffmpeg_file):
-        raise am.FileMissError("No file found to record ffmpeg path, please specify the ffmpeg path.")
+    if language == "en":
+        log.info(f"{video_pid} {prompt_prefix} download successfully.")
     else:
-        with open(ffmpeg_file, "r") as f:
-            ffmpeg: str = f.readline().removesuffix("\n")
-        log.info("Historical ffmpeg path found, using historical ffmpeg path.")
-        return ffmpeg
+        log.info(f"{video_pid} {prompt_prefix} 下载成功.")
 
 
 class VideoDownloadMode(enum.Enum):
     """
     Video Download Type Enumeration Class
     """
     VIDEO = 1
@@ -133,208 +127,276 @@
         self.tags: list[BiliVideoTag] = []
 
         self.work_dir: Union[str, None] = None
         self.info_excel_file: Union[str, None] = None
         self.info_excel: Union[DataFrame, None] = None
 
         self.log_file: str = log
-        self.log: Union[lw.Logger, None] = None
+        self.log: Union[wlw.Logger, None] = None
         self.__set_log()
         self.__p_video_init()
         self.__load_work_dir(work_dir)
 
     def __set_log(self) -> None:
         """
         Set up logs.
         """
-        file_handler: lw.Handler = lw.Handler("file")
+        file_handler: wlw.Handler = wlw.Handler("file")
         file_handler.set_level("WARNING", "ERROR")
         file_handler.set_file(self.log_file)
 
-        sys_handler: lw.Handler = lw.Handler("sys")
+        sys_handler: wlw.Handler = wlw.Handler("sys")
         sys_handler.set_level("INFO", "WARNING")
 
-        self.log: lw.Logger = lw.Logger()
+        self.log: wlw.Logger = wlw.Logger()
         self.log.add_config(file_handler)
         self.log.add_config(sys_handler)
 
     def __p_video_init(self) -> None:
         """
         Obtain sub video information, including id and video time.
         """
         p_info: list[dict] = sync(self.get_pages())
         if p_info:
             for page in p_info:
                 self.p_cid.append(page['cid'])
                 self.p_time.append(page['duration'])
         else:
-            self.log.warning("Failed to obtain sub video ID, which may affect subsequent operations!")
+            if language == "en":
+                self.log.warning("Failed to obtain sub video ID, which may affect subsequent operations!")
+            else:
+                self.log.warning("未获取到分P视频ID, 这可能会影响后续操作!")
 
     def __load_work_dir(self, work_dir: str) -> None:
         """
         Load the working directory.
 
         Args:
             work_dir: working directory
         """
         video_output_dir: str = os.path.join(work_dir, "video_output")
         self.work_dir: str = os.path.join(video_output_dir, self.bvid)
         if not os.path.exists(self.work_dir):
             os.mkdir(self.work_dir)
 
+    @wlw.async_separate()
     async def video_info_statistics(self) -> None:
         """
         Obtain current video data information.
         """
-        self.log.info(f"Start acquiring video information for {self.bvid}...")
-        video_info: dict = await self.get_info()
-        if video_info:
-            self.publish_time = video_info['pubdate']
-            self.total_time = video_info['duration']
-            self.view = video_info['stat']['view']
-            self.like = video_info['stat']['like']
-            self.coin = video_info['stat']['coin']
-            self.favorite = video_info['stat']['favorite']
-            self.share = video_info['stat']['share']
-            self.history_rank = video_info['stat']['his_rank']
-            self.reply_num = video_info['stat']['reply']
-            self.danmu_num = video_info['stat']['danmaku']
-            self.copyright = video_info['copyright']  # copyright: copyright mark, 1: homemade, 2: reprint
-            self.up_uid = video_info['owner']['mid']
+        if language == "en":
+            self.log.info(f"Start acquiring video information for {self.bvid}...")
         else:
-            self.log.warning("Failed to obtain video information, which may affect subsequent operations!")
+            self.log.info(f"开始获取 {self.bvid} 的视频信息...")
+
+        video_info: dict = await self.get_info()
+        self.publish_time = video_info['pubdate']
+        self.total_time = video_info['duration']
+        self.view = video_info['stat']['view']
+        self.like = video_info['stat']['like']
+        self.coin = video_info['stat']['coin']
+        self.favorite = video_info['stat']['favorite']
+        self.share = video_info['stat']['share']
+        self.history_rank = video_info['stat']['his_rank']
+        self.reply_num = video_info['stat']['reply']
+        self.danmu_num = video_info['stat']['danmaku']
+        self.copyright = video_info['copyright']  # copyright: copyright mark, 1: homemade, 2: reprint
+        self.up_uid = video_info['owner']['mid']
 
         video_stst: dict = await self.get_stat()
-        if video_stst:
-            self.reprint_sign = video_stst[
-                'no_reprint']  # reprint_sign: prohibition of reprinting sign, 0: none, 1: prohibition
-        else:
-            self.log.warning("Failed to obtain video reprint information, which may affect subsequent operations!")
+        self.reprint_sign = video_stst[
+            'no_reprint']  # reprint_sign: prohibition of reprinting sign, 0: none, 1: prohibition
 
-        self.log.info(f"Video information acquisition completed for {self.bvid}.")
+        if language == "en":
+            self.log.info(f"Video information acquisition completed for {self.bvid}.")
+        else:
+            self.log.info(f"{self.bvid} 的视频信息获取完成.")
 
+    @wlw.async_separate()
     async def get_replies(self, sec: bool) -> None:
         """
         Obtain first level (second level) replies of videos.
 
         Args:
             sec: whether to obtain the second level reply
         """
-        self.log.info(f"Start acquiring replies for {self.bvid}...")
+        if language == "en":
+            self.log.info(f"Start acquiring replies for {self.bvid}...")
+        else:
+            self.log.info(f"开始获取 {self.bvid} 的评论...")
         page: int = 1
         count: int = 0
         while True:
-            self.log.info(f"Start acquiring page {page} of replies for {self.bvid}.")
+            if language == "en":
+                self.log.info(f"Start acquiring page {page} of replies for {self.bvid}.")
+            else:
+                self.log.info(f"开始获取 {self.bvid} 第 {page} 页评论.")
             page_reply_info: dict = await bac.get_comments(self.aid, bac.CommentResourceType.VIDEO, page,
                                                            credential=self.credential)
-            if page_reply_info:
-                count += page_reply_info['page']['size']
-                if page_reply_info['replies']:
-                    for r in page_reply_info['replies']:
-                        reply: BiliVideoReply = BiliVideoReply(r, log=self.log_file)
-                        self.replies.append(reply)
-                        if sec:
-                            if r['replies']:
-                                for sub_r in r['replies']:
-                                    sub_reply: BiliVideoReply = BiliVideoReply(sub_r, log=self.log_file)
-                                    self.replies.append(sub_reply)
-                    page += 1
-                    time.sleep(0.2)
-                    if count >= page_reply_info['page']['count']:
-                        break
-                else:
+            count += page_reply_info['page']['size']
+            if page_reply_info['replies']:
+                for r in page_reply_info['replies']:
+                    reply: BiliVideoReply = BiliVideoReply(r, log=self.log_file)
+                    self.replies.append(reply)
+                    if sec:
+                        if r['replies']:
+                            for sub_r in r['replies']:
+                                sub_reply: BiliVideoReply = BiliVideoReply(sub_r, log=self.log_file)
+                                self.replies.append(sub_reply)
+                page += 1
+                time.sleep(0.2)
+                if count >= page_reply_info['page']['count']:
                     break
             else:
                 break
         if sec:
-            self.log.info(
-                f"A total of {len(self.replies)} replies have been collected successfully. "
-                f"(With second level replies)")
-        else:
-            self.log.info(
-                f"A total of {len(self.replies)} replies have been collected successfully. "
-                f"(Without second level replies)")
+            if language == "en":
+                self.log.info(
+                    f"A total of {len(self.replies)} replies have been collected successfully. "
+                    f"(With second level replies)")
+            else:
+                self.log.info(
+                    f"一共成功获取了 {len(self.replies)} 条评论. (包含二级评论)")
+        else:
+            if language == "en":
+                self.log.info(
+                    f"A total of {len(self.replies)} replies have been collected successfully. "
+                    f"(Without second level replies)")
+            else:
+                self.log.info(
+                    f"一共成功获取了 {len(self.replies)} 条评论. (不包含二级评论)")
 
+    @wlw.async_separate()
     async def get_danmu(self) -> None:
         """
         Obtain all current danmu in the video.
         """
-        self.log.info(f"Start acquiring danmu for {self.bvid}...")
+        if language == "en":
+            self.log.info(f"Start acquiring danmu for {self.bvid}...")
+        else:
+            self.log.info(f"开始获取 {self.bvid} 的弹幕...")
         if self.p_cid:
             for p_id in self.p_cid:
-                self.log.info(f"Start acquiring danmu for sub video: {p_id}.")
+                if language == "en":
+                    self.log.info(f"Start acquiring danmu for sub video: {p_id}...")
+                else:
+                    self.log.info(f"开始获取分P: {p_id} 的弹幕...")
                 danmu_list_info: list[Danmaku] = await self.get_danmakus(cid=p_id)
                 if danmu_list_info:
                     for danmu_info in danmu_list_info:
                         danmu: BiliVideoDanmu = BiliVideoDanmu(danmu_info, log=self.log_file)
                         self.danmu.append(danmu)
                 time.sleep(0.2)
-            self.log.info(f"A total of {len(self.danmu)} danmu have been collected successfully.")
+            if language == "en":
+                self.log.info(f"A total of {len(self.danmu)} danmu have been collected successfully.")
+            else:
+                self.log.info(f"一共成功获取了 {len(self.danmu)} 条弹幕.")
         else:
-            self.log.warning("The sub video id is missing, and the danmu cannot be obtained!")
+            if language == "en":
+                self.log.warning("The sub video id is missing, and the danmu cannot be obtained!")
+            else:
+                self.log.warning("缺少分P视频id, 无法获取弹幕!")
 
+    @wlw.async_separate()
     async def reply_robust_process(self) -> None:
         """
         Robust processing of replies. Remove emoticon frame.
         """
-        self.log.info(f"Start robust processing of replies for {self.bvid}...")
+        if language == "en":
+            self.log.info(f"Start robust processing of replies for {self.bvid}...")
+        else:
+            self.log.info(f"开始处理 {self.bvid} 的评论内容...")
         if self.replies:
             for elem in self.replies:
                 rb_reply: BiliVideoReply = copy.deepcopy(elem)
                 rb_reply.content = re.sub(r"\[.*?]", ",", rb_reply.content)
                 self.robust_replies.append(rb_reply)
-            self.log.info(f"Robust processing of replies for {self.bvid} completed.")
+            if language == "en":
+                self.log.info(f"Robust processing of replies for {self.bvid} completed.")
+            else:
+                self.log.info(f"完成对 {self.bvid} 评论内容的处理.")
         else:
-            self.log.warning("The reply is empty, and the robust processing cannot be performed!")
+            if language == "en":
+                self.log.warning("The reply is empty, and the robust processing cannot be performed!")
+            else:
+                self.log.warning("评论为空, 无法进行处理!")
 
+    @wlw.async_separate()
     async def get_tag(self) -> None:
         """
         Obtain video tag information.
         """
-        self.log.info(f"Start acquiring tags for {self.bvid}...")
+        if language == "en":
+            self.log.info(f"Start acquiring tags for {self.bvid}...")
+        else:
+            self.log.info(f"开始获取 {self.bvid} 的标签...")
         if self.p_cid:
             for p_id in self.p_cid:
-                self.log.info(f"Start acquiring tags for sub video: {p_id}.")
+                if language == "en":
+                    self.log.info(f"Start acquiring tags for sub video: {p_id}.")
+                else:
+                    self.log.info(f"开始获取分P: {p_id} 的标签...")
                 tag_info_list: list[dict] = await self.get_tags(cid=p_id)
                 if tag_info_list:
                     for tag_info in tag_info_list:
                         tag: BiliVideoTag = BiliVideoTag(tag_info, log=self.log_file)
                         self.tags.append(tag)
                 time.sleep(0.2)
             if len(self.tags) > 0:
-                self.log.info(f"A total of {len(self.tags)} tags have been collected successfully.")
+                if language == "en":
+                    self.log.info(f"A total of {len(self.tags)} tags have been collected successfully.")
+                else:
+                    self.log.info(f"一共成功获取了 {len(self.tags)} 个标签.")
             else:
-                self.log.warning(f"{self.bvid} did not add a tag, which may affect subsequent operations!")
+                if language == "en":
+                    self.log.warning(f"{self.bvid} did not add a tag, which may affect subsequent operations!")
+                else:
+                    self.log.warning(f"{self.bvid} 没有添加标签, 这可能会影响后续操作!")
         else:
-            self.log.warning("The sub video id is missing, and the tag cannot be obtained!")
+            if language == "en":
+                self.log.warning("The sub video id is missing, and the tag cannot be obtained!")
+            else:
+                self.log.warning("缺少分P视频id, 无法获取标签!")
 
+    @wlw.async_separate()
     async def tag_process(self) -> None:
         """
         Calculate the mean, maximum and minimum values of video tag popularity.
         """
+        if language == "en":
+            self.log.info(f"Start processing tags for {self.bvid}...")
+        else:
+            self.log.info(f"开始处理 {self.bvid} 的标签...")
         tag_use: list[int] = []
         tag_follow: list[int] = []
         if self.tags:
             for elem in self.tags:
                 tag_use.append(elem.use_num)
                 tag_follow.append(elem.follow_num)
             self.tag_use_mean: float = sum(tag_use) / len(tag_use)
             self.tag_use_max: int = np.max(tag_use)
             self.tag_use_min: int = np.min(tag_use)
             self.tag_follow_mean: float = sum(tag_follow) / len(tag_follow)
             self.tag_follow_max: int = np.max(tag_follow)
             self.tag_follow_min: int = np.min(tag_follow)
+            if language == "en":
+                self.log.info(f"Processing tags for {self.bvid} completed.")
+            else:
+                self.log.info(f"完成对 {self.bvid} 标签的处理.")
         else:
             self.tag_follow_mean: float = -1
             self.tag_follow_max: int = -1
             self.tag_follow_min: int = -1
             self.tag_use_mean: float = -1
             self.tag_use_max: int = -1
             self.tag_use_min: int = -1
-            self.log.warning("The tag is empty!")
+            if language == "en":
+                self.log.warning("The tag is empty!")
+            else:
+                self.log.warning("标签为空!")
 
     async def __load_info_excel(self, excel_file: str) -> None:
         """
         Load the Excel file to save the video information.
 
         Args:
             excel_file: excel file path
@@ -369,77 +431,105 @@
                                         "reprint_sign": self.reprint_sign,
                                         "tag_use_mean": self.tag_use_mean,
                                         "tag_use_max": self.tag_use_max,
                                         "tag_use_min": self.tag_use_min,
                                         "tag_follow_mean": self.tag_follow_mean,
                                         "tag_follow_max": self.tag_follow_max,
                                         "tag_follow_min": self.tag_follow_min},
-                                        index=[0])
+                                       index=[0])
         pd.concat([self.info_excel, line], axis=0, ignore_index=True).to_excel(excel_file, index=False)
-        self.log.info(f"Video information has been saved to {excel_file}.")
+        if language == "en":
+            self.log.info(f"Video information has been saved to {excel_file}.")
+        else:
+            self.log.info(f"视频信息已保存至 {excel_file}.")
 
+    @wlw.async_separate()
     async def download(self, mode: VideoDownloadMode) -> None:
         """
         Download all videos or audio.
 
         Args:
             mode: 0 for downloading videos, 1 for downloading audio.
         """
         if self.p_cid:
-            ffmpeg_path = await _load_ffmpeg_path_from_txt(self.log)
+            ffmpeg_path = await load_ffmpeg_path_from_txt()
             for pid in self.p_cid:
                 p_url_info: dict = await self.get_download_url(cid=pid)
                 detector = bav.VideoDownloadURLDataDetecter(data=p_url_info)
                 streams = detector.detect_best_streams()
 
                 if detector.check_flv_stream():
                     if mode == VideoDownloadMode.VIDEO:
                         temp_flv: str = os.path.join(self.work_dir, f"{pid}_flv_temp.flv")
                         mp4_video_out: str = os.path.join(self.work_dir, f"{pid}.mp4")
 
                         await _download_video_from_url(streams[0].url, temp_flv, pid, self.log, "flv video streaming")
 
-                        self.log.info("Converting video format...")
+                        if language == "en":
+                            self.log.info("Converting video format...")
+                        else:
+                            self.log.info("正在转换视频格式...")
                         os.system(f"{ffmpeg_path} -i {temp_flv} {mp4_video_out}")
 
                         os.remove(temp_flv)
-                        self.log.info(f"{pid} video download successfully.")
+                        if language == "en":
+                            self.log.info(f"{pid} video download successfully.")
+                        else:
+                            self.log.info(f"{pid} 视频下载成功.")
 
                     elif mode == VideoDownloadMode.AUDIO:
                         temp_flv: str = os.path.join(self.work_dir, f"{pid}_flv_temp.flv")
                         mp3_audio_out: str = os.path.join(self.work_dir, f"{pid}.mp3")
 
                         await _download_video_from_url(streams[0].url, temp_flv, pid, self.log, "flv video streaming")
 
-                        self.log.info("Converting audio format...")
+                        if language == "en":
+                            self.log.info("Converting audio format...")
+                        else:
+                            self.log.info("正在转换音频格式...")
                         os.system(f"{ffmpeg_path} -i {temp_flv} -vn -acodec copy {mp3_audio_out}")
 
                         os.remove(temp_flv)
-                        self.log.info(f"{pid} audio download successfully.")
+                        if language == "en":
+                            self.log.info(f"{pid} audio download successfully.")
+                        else:
+                            self.log.info(f"{pid} 音频下载成功.")
                 else:
                     if mode == VideoDownloadMode.VIDEO:
                         temp_m4s_video: str = os.path.join(self.work_dir, f"{pid}_video_mp4_temp.m4s")
                         temp_m4s_audio: str = os.path.join(self.work_dir, f"{pid}_audio_mp4_temp.m4s")
                         mp4_video_out: str = os.path.join(self.work_dir, f"{pid}.mp4")
 
                         await _download_video_from_url(streams[0].url, temp_m4s_video, pid, self.log, "video streaming")
                         await _download_video_from_url(streams[1].url, temp_m4s_audio, pid, self.log, "audio streaming")
 
-                        self.log.info("Converting video format...")
+                        if language == "en":
+                            self.log.info("Converting video format...")
+                        else:
+                            self.log.info("正在转换视频格式...")
                         os.system(f"{ffmpeg_path} -i {temp_m4s_video} -i {temp_m4s_audio} "
                                   f"-vcodec copy -acodec copy {mp4_video_out}")
 
                         os.remove(temp_m4s_video)
                         os.remove(temp_m4s_audio)
-                        self.log.info(f"{pid} video download successfully.")
+                        if language == "en":
+                            self.log.info(f"{pid} video download successfully.")
+                        else:
+                            self.log.info(f"{pid} 视频下载成功.")
 
                     elif mode == VideoDownloadMode.AUDIO:
                         temp_m4s_audio: str = os.path.join(self.work_dir, f"{pid}_audio_mp4_temp.m4s")
                         mp3_audio_out: str = os.path.join(self.work_dir, f"{pid}.mp3")
 
                         await _download_video_from_url(streams[1].url, temp_m4s_audio, pid, self.log, "audio streaming")
 
-                        self.log.info("Converting audio format...")
+                        if language == "en":
+                            self.log.info("Converting audio format...")
+                        else:
+                            self.log.info("正在转换音频格式...")
                         os.system(f"{ffmpeg_path} -i {temp_m4s_audio} -acodec copy {mp3_audio_out}")
 
                         os.remove(temp_m4s_audio)
-                        self.log.info(f"{pid} audio download successfully.")
+                        if language == "en":
+                            self.log.info(f"{pid} audio download successfully.")
+                        else:
+                            self.log.info(f"{pid} 音频下载成功.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.1.9/Bili_UAS/writer/log_writer.py` & `bili-uas-0.2.0/Bili_UAS/writer/log_writer.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 """
 
 
 from __future__ import annotations
 import datetime
 from Bili_UAS.writer import abnormal_monitor as am
 from typing import Union
+from functools import wraps
+import asyncio
 
 
 class Handler:
     """
     Log test_output configuration class. Set the destination for log test_output and what level of log to test_output.
     """
     def __init__(self, output_mode: str) -> None:
@@ -112,7 +114,27 @@
         Logs a message with level ERROR.
 
         Args:
             message: log information
         """
         for handler in self.config:
             handler.log_print("ERROR", message)
+
+
+def async_separate(number: int = 50) -> callable:
+    """
+    Separate program output.
+
+    Args:
+        number: the number of separator characters
+    """
+    def decorator(func):
+        @wraps(func)
+        async def wrapper(*args, **kwargs):
+            print("\n")
+            print("\033[32m" + "-" * number + "\033[0m")
+            result = await func(*args, **kwargs)
+            print("\033[32m" + "-" * number + "\033[0m")
+            print("\n")
+            return result
+        return wrapper
+    return decorator
```

### Comparing `bili-uas-0.1.9/LICENSE` & `bili-uas-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.9/PKG-INFO` & `bili-uas-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.9
+Version: 0.2.0
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
-Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
+Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.9
```

### Comparing `bili-uas-0.1.9/README.md` & `bili-uas-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.1.9/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.2.0/bili_uas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.1.9
+Version: 0.2.0
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
-Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud
+Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.9
```

### Comparing `bili-uas-0.1.9/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.2.0/bili_uas.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 setup.py
 Bili_UAS/__init__.py
 Bili_UAS/bili_config.py
 Bili_UAS/bili_live.py
 Bili_UAS/bili_login.py
 Bili_UAS/bili_user.py
 Bili_UAS/bili_video.py
+Bili_UAS/cli/__init__.py
+Bili_UAS/cli/live_cli.py
+Bili_UAS/cli/user_cli.py
+Bili_UAS/cli/video_cli.py
 Bili_UAS/scripts/__init__.py
 Bili_UAS/scripts/config.py
-Bili_UAS/scripts/live.py
 Bili_UAS/scripts/log_in.py
-Bili_UAS/scripts/user.py
 Bili_UAS/scripts/video.py
 Bili_UAS/utils/__init__.py
+Bili_UAS/utils/config_utils.py
 Bili_UAS/utils/live_utils.py
 Bili_UAS/utils/search_utils.py
 Bili_UAS/utils/train_utils.py
 Bili_UAS/utils/user_utils.py
 Bili_UAS/utils/utils.py
 Bili_UAS/utils/video_utils.py
 Bili_UAS/writer/__init__.py
```

### Comparing `bili-uas-0.1.9/setup.py` & `bili-uas-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,45 +5,46 @@
 
 requirements = [
     'bilibili-api-python~=15.5.1',
     'setuptools~=68.0.0',
     'wordcloud~=1.9.2',
     'jieba~=0.42.1',
     'scipy~=1.11.1',
-    'numpy~=1.25.0',
-    'tyro~=0.5.3',
+    'numpy~=1.25.1',
+    'tyro~=0.5.4',
     'pandas~=2.0.3',
     'tqdm~=4.65.0',
-    'matplotlib~=3.7.1',
+    'matplotlib~=3.7.2',
     'asyncio~=3.4.3',
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1',
     'openpyxl~=3.1.2']
 
 setup(
     name='bili-uas',
-    version='0.1.9',
+    version='0.2.0',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
-    keywords=["BiliBili", "auxiliary", "analysis", "live", "video", "word_cloud"],
+    keywords=["BiliBili", "auxiliary", "analysis", "live", "video", "word_cloud", "monitor"],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'Topic :: Software Development :: Build Tools',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)"
     ],
     packages=['Bili_UAS',
+              'Bili_UAS.cli',
               'Bili_UAS.utils',
               'Bili_UAS.writer',
               'Bili_UAS.scripts'],
     package_data={'': ['*.txt', '*.md', 'LICENSE', 'setup.py', 'requirements.txt', '.gitignore']},
     exclude_package_data={'': ['test/*.py', 'test']},
     include_package_data=True,
     python_requires='>=3.9',
```

