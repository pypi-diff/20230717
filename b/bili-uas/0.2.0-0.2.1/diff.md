# Comparing `tmp/bili-uas-0.2.0.tar.gz` & `tmp/bili-uas-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bili-uas-0.2.0.tar", last modified: Mon Jul 17 13:31:23 2023, max compression
+gzip compressed data, was "bili-uas-0.2.1.tar", last modified: Mon Jul 17 14:01:55 2023, max compression
```

## Comparing `bili-uas-0.2.0.tar` & `bili-uas-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.720234 bili-uas-0.2.0/
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.712919 bili-uas-0.2.0/Bili_UAS/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.2.0/Bili_UAS/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2134 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/bili_config.py
--rw-r--r--   0 jhzg       (501) staff       (20)     5445 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/bili_live.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2875 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/bili_login.py
--rw-r--r--   0 jhzg       (501) staff       (20)     3350 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/bili_user.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2964 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/bili_video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.713982 bili-uas-0.2.0/Bili_UAS/cli/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-17 12:26:30.000000 bili-uas-0.2.0/Bili_UAS/cli/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4298 2023-07-17 12:47:31.000000 bili-uas-0.2.0/Bili_UAS/cli/live_cli.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1277 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/cli/user_cli.py
--rw-r--r--   0 jhzg       (501) staff       (20)     1502 2023-07-17 12:46:40.000000 bili-uas-0.2.0/Bili_UAS/cli/video_cli.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.714900 bili-uas-0.2.0/Bili_UAS/scripts/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.2.0/Bili_UAS/scripts/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2282 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/scripts/config.py
--rw-r--r--   0 jhzg       (501) staff       (20)    10584 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/scripts/log_in.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4670 2023-07-17 12:38:07.000000 bili-uas-0.2.0/Bili_UAS/scripts/video.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.717637 bili-uas-0.2.0/Bili_UAS/utils/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.2.0/Bili_UAS/utils/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2354 2023-07-15 12:39:12.000000 bili-uas-0.2.0/Bili_UAS/utils/config_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    63669 2023-07-17 12:17:57.000000 bili-uas-0.2.0/Bili_UAS/utils/live_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)     2224 2023-07-17 12:23:11.000000 bili-uas-0.2.0/Bili_UAS/utils/search_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.2.0/Bili_UAS/utils/train_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    18336 2023-07-17 12:53:20.000000 bili-uas-0.2.0/Bili_UAS/utils/user_utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-07-15 12:01:05.000000 bili-uas-0.2.0/Bili_UAS/utils/utils.py
--rw-r--r--   0 jhzg       (501) staff       (20)    22842 2023-07-15 13:04:58.000000 bili-uas-0.2.0/Bili_UAS/utils/video_utils.py
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.718931 bili-uas-0.2.0/Bili_UAS/writer/
--rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.2.0/Bili_UAS/writer/__init__.py
--rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.2.0/Bili_UAS/writer/abnormal_monitor.py
--rw-r--r--   0 jhzg       (501) staff       (20)     4148 2023-07-15 12:42:36.000000 bili-uas-0.2.0/Bili_UAS/writer/log_writer.py
--rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.2.0/LICENSE
--rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 13:31:23.720099 bili-uas-0.2.0/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.2.0/README.md
-drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 13:31:23.719904 bili-uas-0.2.0/bili_uas.egg-info/
--rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/PKG-INFO
--rw-r--r--   0 jhzg       (501) staff       (20)      890 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/SOURCES.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/dependency_links.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/entry_points.txt
--rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/requires.txt
--rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-17 13:31:23.000000 bili-uas-0.2.0/bili_uas.egg-info/top_level.txt
--rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-17 13:31:23.720284 bili-uas-0.2.0/setup.cfg
--rw-r--r--   0 jhzg       (501) staff       (20)     2042 2023-07-17 13:10:13.000000 bili-uas-0.2.0/setup.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.794275 bili-uas-0.2.1/
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.787826 bili-uas-0.2.1/Bili_UAS/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-30 10:47:09.000000 bili-uas-0.2.1/Bili_UAS/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2371 2023-07-17 13:47:56.000000 bili-uas-0.2.1/Bili_UAS/bili_config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     6867 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/bili_live.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3238 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/bili_login.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     3350 2023-07-17 12:53:20.000000 bili-uas-0.2.1/Bili_UAS/bili_user.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2964 2023-07-17 12:38:07.000000 bili-uas-0.2.1/Bili_UAS/bili_video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.788656 bili-uas-0.2.1/Bili_UAS/cli/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-07-17 12:26:30.000000 bili-uas-0.2.1/Bili_UAS/cli/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4298 2023-07-17 12:47:31.000000 bili-uas-0.2.1/Bili_UAS/cli/live_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1277 2023-07-17 12:46:40.000000 bili-uas-0.2.1/Bili_UAS/cli/user_cli.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     1502 2023-07-17 12:46:40.000000 bili-uas-0.2.1/Bili_UAS/cli/video_cli.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.789123 bili-uas-0.2.1/Bili_UAS/scripts/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-14 13:05:48.000000 bili-uas-0.2.1/Bili_UAS/scripts/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2886 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/scripts/config.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    13416 2023-07-17 14:01:28.000000 bili-uas-0.2.1/Bili_UAS/scripts/log_in.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4670 2023-07-17 12:38:07.000000 bili-uas-0.2.1/Bili_UAS/scripts/video.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.791877 bili-uas-0.2.1/Bili_UAS/utils/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-06-13 07:49:27.000000 bili-uas-0.2.1/Bili_UAS/utils/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2366 2023-07-17 13:38:58.000000 bili-uas-0.2.1/Bili_UAS/utils/config_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    63669 2023-07-17 12:17:57.000000 bili-uas-0.2.1/Bili_UAS/utils/live_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     2224 2023-07-17 12:23:11.000000 bili-uas-0.2.1/Bili_UAS/utils/search_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      359 2023-06-30 10:59:22.000000 bili-uas-0.2.1/Bili_UAS/utils/train_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    18336 2023-07-17 12:53:20.000000 bili-uas-0.2.1/Bili_UAS/utils/user_utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    11258 2023-07-15 12:01:05.000000 bili-uas-0.2.1/Bili_UAS/utils/utils.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    22842 2023-07-15 13:04:58.000000 bili-uas-0.2.1/Bili_UAS/utils/video_utils.py
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.793063 bili-uas-0.2.1/Bili_UAS/writer/
+-rw-r--r--   0 jhzg       (501) staff       (20)        0 2023-05-16 02:00:41.000000 bili-uas-0.2.1/Bili_UAS/writer/__init__.py
+-rw-r--r--   0 jhzg       (501) staff       (20)      488 2023-06-30 10:59:22.000000 bili-uas-0.2.1/Bili_UAS/writer/abnormal_monitor.py
+-rw-r--r--   0 jhzg       (501) staff       (20)     4148 2023-07-15 12:42:36.000000 bili-uas-0.2.1/Bili_UAS/writer/log_writer.py
+-rw-r--r--   0 jhzg       (501) staff       (20)    34523 2023-06-06 23:49:40.000000 bili-uas-0.2.1/LICENSE
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:01:55.794139 bili-uas-0.2.1/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)     3874 2023-07-08 12:32:56.000000 bili-uas-0.2.1/README.md
+drwxr-xr-x   0 jhzg       (501) staff       (20)        0 2023-07-17 14:01:55.793947 bili-uas-0.2.1/bili_uas.egg-info/
+-rw-r--r--   0 jhzg       (501) staff       (20)     4607 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/PKG-INFO
+-rw-r--r--   0 jhzg       (501) staff       (20)      890 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/SOURCES.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        1 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/dependency_links.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      226 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/entry_points.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)      245 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/requires.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)        9 2023-07-17 14:01:55.000000 bili-uas-0.2.1/bili_uas.egg-info/top_level.txt
+-rw-r--r--   0 jhzg       (501) staff       (20)       38 2023-07-17 14:01:55.794326 bili-uas-0.2.1/setup.cfg
+-rw-r--r--   0 jhzg       (501) staff       (20)     2042 2023-07-17 14:01:28.000000 bili-uas-0.2.1/setup.py
```

### Comparing `bili-uas-0.2.0/Bili_UAS/bili_config.py` & `bili-uas-0.2.1/Bili_UAS/bili_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         work_dir: working directory of program
         ffmpeg: the ffmpeg path in your computer
         mark: mark for marking live danmu, multiple marks need to be entered consecutive
         language: the language for program prompts
     """
     if not os.path.exists(work_dir):
         os.makedirs(work_dir, exist_ok=True)
-    sync(sc.save_work_dir_to_txt(work_dir))
+    sync(sc.save_work_dir_to_txt(work_dir, language))
 
     work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "config_log.txt")
 
     file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
@@ -44,25 +44,31 @@
     sys_handler.set_level("INFO", "WARNING")
 
     log: wlw.Logger = wlw.Logger()
     log.add_config(file_handler)
     log.add_config(sys_handler)
 
     if ffmpeg is not None:
-        sync(sc.save_ffmpeg_path_to_txt(ffmpeg, log))
+        sync(sc.save_ffmpeg_path_to_txt(ffmpeg, language))
     else:
-        log.warning("No ffmpeg path specified, video cannot be downloaded.")
+        if language == "en":
+            log.warning("No ffmpeg path specified, video cannot be downloaded.")
+        else:
+            log.warning("未指定ffmpeg路径，将无法下载视频。")
 
     if mark is not None:
         mark_list: list[str] = [m for m in mark]
-        sync(sc.save_danmu_mark_to_txt(mark_list, log))
+        sync(sc.save_danmu_mark_to_txt(mark_list, language))
     else:
-        log.warning("No danmu mark specified.")
+        if language == "en":
+            log.warning("No danmu mark specified.")
+        else:
+            log.warning("未指定弹幕标记。")
 
-    sync(sc.save_language_to_txt(language, log))
+    sync(sc.save_language_to_txt(language))
 
 
 def tyro_cli() -> None:
     """
     Command line interface
     """
     tyro.extras.set_accent_color("bright_yellow")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.2.0/Bili_UAS/bili_live.py` & `bili-uas-0.2.1/Bili_UAS/bili_live.py`

 * *Files 23% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 def sync_tyro_main(config: Union[clc.BiliLiveConfigAuto, clc.BiliLiveConfigMonitor, clc.BiliLiveConfigProcess]) -> None:
     """
     Main function for tyro command-line interface.
 
     Args:
         config: configuration
     """
+    language: str = ucu.load_language_from_txt()
     work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "live_log.txt")
 
     file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
@@ -42,25 +43,32 @@
     log.add_config(sys_handler)
 
     credential = sync(sli.load_credential_from_json(log_file))
     if credential is not None:
         credential = sync(sli.refresh_credential(credential, log_file))
 
     if isinstance(config, clc.BiliLiveConfigAuto):
-        log.warning("The setting mode is 'auto', and in this mode, 'auto_disconnect', 'danmu_disconnect', and "
-                    "'robust' are set to true, and data processing is automatically performed after disconnecting "
-                    "the live streaming connection!")
+        if language == "en":
+            log.warning("The setting mode is 'auto', and in this mode, 'auto_disconnect', 'danmu_disconnect', and "
+                        "'robust' are set to true, and data processing is automatically performed after disconnecting "
+                        "the live streaming connection!")
+        else:
+            log.warning("设置模式为 'auto'，在此模式下，'auto_disconnect'、'danmu_disconnect'、'robust' 被设置为True，"
+                        "且在断开直播连接后自动进行数据处理！")
 
         config.auto_disconnect = True
         config.danmu_disconnect = True
         config.robust = True
 
         if config.user_id is None:
             if config.live_id is None:
-                raise wam.ParameterInputError("user_id and live_id must be entered either!")
+                if language == "en":
+                    raise wam.ParameterInputError("user_id and live_id must be entered either!")
+                else:
+                    raise wam.ParameterInputError("user_id 和 live_id 必须输入其中之一！")
 
         if config.user_id is not None:
             user = uuu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
             config.live_id = user.room_id
 
         live_monitor = ulu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
                                            config.retry_after, credential)
@@ -69,46 +77,64 @@
 
         sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
         live_process = ulu.BiliLiveProcess(log_file, live_monitor.work_dir)
         sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                    config.robust_interval, mask))
 
         while config.forever:
-            log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
+            if language == "en":
+                log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
+            else:
+                log.warning("设置为长连直播间，要退出程序，请使用ctrl + c。")
             sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
             live_process = ulu.BiliLiveProcess(log_file, live_monitor.work_dir)
             sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
                                        config.robust_interval, mask))
 
     elif isinstance(config, clc.BiliLiveConfigMonitor):
-        log.warning("Set the mode to 'monitor', and in this mode, only data monitoring "
-                    "will be performed without data processing!")
+        if language == "en":
+            log.warning("Set the mode to 'monitor', and in this mode, only data monitoring "
+                        "will be performed without data processing!")
+        else:
+            log.warning("设置模式为 'monitor'，在此模式下，只进行数据监控，不进行数据处理！")
 
         if config.user_id is None:
             if config.live_id is None:
-                raise wam.ParameterInputError("user_id and live_id must be entered either!")
+                if language == "en":
+                    raise wam.ParameterInputError("user_id and live_id must be entered either!")
+                else:
+                    raise wam.ParameterInputError("user_id 和 live_id 必须输入其中之一！")
 
         if config.user_id is not None:
             user = uuu.BiliUser(uid=config.user_id, log=log_file, work_dir=work_dir, credential=credential)
             config.live_id = user.room_id
 
         live_monitor = ulu.BiliLiveMonitor(config.live_id, log_file, work_dir, config.max_retry,
                                            config.retry_after, credential)
         sync(live_monitor.load_danmu_mark())
 
         sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
         while config.forever:
-            log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
+            if language == "en":
+                log.warning("Long connecting live room. To exit the program, please use ctrl + c.")
+            else:
+                log.warning("设置为长连直播间，要退出程序，请使用ctrl + c。")
             sync(live_monitor.monitor(config.save_all_danmu, config.danmu_disconnect, config.auto_disconnect))
 
     elif isinstance(config, clc.BiliLiveConfigProcess):
-        log.warning("Set the mode to 'process', and in this mode, a data folder needs to be specified!")
+        if language == "en":
+            log.warning("Set the mode to 'process', and in this mode, a data folder needs to be specified!")
+        else:
+            log.warning("设置模式为 'process'，在此模式下，需要指定一个数据文件夹！")
 
         if config.data_dir is None:
-            raise wam.ParameterInputError("No data folder specified!")
+            if language == "en":
+                raise wam.ParameterInputError("No data folder specified!")
+            else:
+                raise wam.ParameterInputError("没有指定数据文件夹！")
 
         if config.mask is not None:
             mask: npt.NDArray = plt.imread(config.mask)
         else:
             mask = None
         live_process = ulu.BiliLiveProcess(log_file, config.data_dir)
         sync(live_process.analysis(config.revenue_interval, config.danmu_interval, config.robust,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.2.0/Bili_UAS/bili_login.py` & `bili-uas-0.2.1/Bili_UAS/bili_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
               specifying credential parameters
         sessdata: credential sessdata
         bili_jct: credential bili_jct
         buvid3: credential buvid3
         dedeuserid: credential dedeuserid
         ac_time_value: credential ac_time_value
     """
+    language: str = ucu.load_language_from_txt()
     work_dir: str = sync(ucu.load_work_dir_from_txt())
     log_output: str = os.path.join(work_dir, "log")
     log_file: str = os.path.join(log_output, "login_log.txt")
 
     file_handler: wlw.Handler = wlw.Handler("file")
     file_handler.set_level("WARNING", "ERROR")
     file_handler.set_file(log_file)
@@ -51,29 +52,35 @@
     m = sli.LoginMode(mode)
 
     if m == sli.LoginMode.PARAMETER:
         if sessdata is not None and bili_jct is not None and buvid3 is not None \
                 and dedeuserid is not None and ac_time_value is not None:
             pass
         else:
-            raise wam.ParameterInputError("Select the login method with the specified parameters,"
-                                          "but the input parameters are missing!")
+            if language == "en":
+                raise wam.ParameterInputError("Select the login method with the specified parameters,"
+                                              "but the input parameters are missing!")
+            else:
+                raise wam.ParameterInputError("选择指定参数登录方式，但输入参数缺失！")
 
     if m == sli.LoginMode.QR:
         flag = sync(sli.log_in_by_QR_code(log_file))
     elif m == sli.LoginMode.PASSWORD:
         flag = sync(sli.log_in_by_password(log_file))
     elif m == sli.LoginMode.VERIFICATION:
         flag = sync(sli.log_in_by_verification_code(log_file))
     else:
         flag = sync(sli.save_credential_by_parm_to_json(sessdata, bili_jct, buvid3,
                                                         dedeuserid, ac_time_value, log_file))
 
     if not flag:
-        log.error("Login failed, please try logging in again! (priority is to scan QR code or specify parameters)")
+        if language == "en":
+            log.error("Login failed, please try logging in again! (priority is to scan QR code or specify parameters)")
+        else:
+            log.error("登录失败，请重试登录！（优先扫描二维码或指定参数）")
 
 
 def tyro_cli() -> None:
     """
     Command line interface
     """
     tyro.extras.set_accent_color("bright_yellow")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.2.0/Bili_UAS/bili_user.py` & `bili-uas-0.2.1/Bili_UAS/bili_user.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/bili_video.py` & `bili-uas-0.2.1/Bili_UAS/bili_video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/cli/live_cli.py` & `bili-uas-0.2.1/Bili_UAS/cli/live_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/cli/user_cli.py` & `bili-uas-0.2.1/Bili_UAS/cli/user_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/cli/video_cli.py` & `bili-uas-0.2.1/Bili_UAS/cli/video_cli.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/scripts/config.py` & `bili-uas-0.2.1/Bili_UAS/scripts/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,22 @@
 
 
 from __future__ import annotations
 from Bili_UAS.writer import log_writer as wlw
 import os
 
 
-async def save_work_dir_to_txt(work_dir: str) -> None:
+@wlw.async_separate()
+async def save_work_dir_to_txt(work_dir: str, language: str) -> None:
     """
     Save working path to file.
+
+    Args:
+        work_dir: working directory of program
+        language: the language of program prompts
     """
     work_dir_file: str = ".work_dir.txt"
     output_dir: str = os.path.join(os.path.abspath(work_dir), "Bili_UAS_Output")
     if not os.path.exists(output_dir):
         os.mkdir(output_dir)
     with open(work_dir_file, "w") as f:
         f.write(output_dir + "\n")
@@ -29,52 +34,65 @@
         os.mkdir(user_out_dir)
     video_out_dir: str = os.path.join(output_dir, "video_output")
     if not os.path.exists(video_out_dir):
         os.mkdir(video_out_dir)
     log_out_dir: str = os.path.join(output_dir, "log")
     if not os.path.exists(log_out_dir):
         os.mkdir(log_out_dir)
+    if language == "en":
+        print("INFO: Working path saved successfully.")
+    else:
+        print("INFO: 工作路径保存成功。")
 
-    print("Working path saved successfully.")
 
-
-async def save_danmu_mark_to_txt(danmu_mark: list[str], log: wlw.Logger) -> None:
+@wlw.async_separate()
+async def save_danmu_mark_to_txt(danmu_mark: list[str], language: str) -> None:
     """
     Save danmu mark to file.
 
     Args:
         danmu_mark: danmu mark list
-        log: logger
+        language: the language of program prompts
     """
     danmu_mark_file: str = ".danmu_mark.txt"
     with open(danmu_mark_file, "w") as f:
         for mark in danmu_mark:
             f.write(mark + "\n")
-    log.info("Danmu mark saved successfully.")
+    if language == "en":
+        print("INFO: Danmu mark saved successfully.")
+    else:
+        print("INFO: 弹幕标记保存成功。")
 
 
-async def save_ffmpeg_path_to_txt(ffmpeg_path: str, log: wlw.Logger) -> None:
+@wlw.async_separate()
+async def save_ffmpeg_path_to_txt(ffmpeg_path: str, language: str) -> None:
     """
     Save ffmpeg path to file.
 
     Args:
         ffmpeg_path: the path of ffmpeg
-        log: logger
+        language: the language of program prompts
     """
     ffmpeg_file: str = ".ffmpeg.txt"
     with open(ffmpeg_file, "w") as f:
         f.write(ffmpeg_path + "\n")
-    log.info("Ffmpeg path saved successfully.")
+    if language == "en":
+        print("INFO: ffmpeg path saved successfully.")
+    else:
+        print("INFO: ffmpeg路径保存成功。")
 
 
-async def save_language_to_txt(language: str, log: wlw.Logger) -> None:
+@wlw.async_separate()
+async def save_language_to_txt(language: str) -> None:
     """
     Save language to file.
 
     Args:
         language: the language of program prompts
-        log: logger
     """
     language_file: str = ".language.txt"
     with open(language_file, "w") as f:
         f.write(language + "\n")
-    log.info("Language configuration saved successfully.")
+    if language == "en":
+        print("INFO: Language configuration saved successfully.")
+    else:
+        print("INFO: 语言配置保存成功。")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `bili-uas-0.2.0/Bili_UAS/scripts/video.py` & `bili-uas-0.2.1/Bili_UAS/scripts/video.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/config_utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/config_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,17 +18,17 @@
     config_file: str = ".language.txt"
     if not os.path.exists(config_file):
         return "en"
     else:
         with open(config_file, "r") as f:
             language: str = f.readline().removesuffix("\n")
         if language == "en":
-            print("Historical language found, using historical language.")
+            print("INFO: Historical language found, using historical language.")
         else:
-            print("找到历史语言设置, 使用历史语言.")
+            print("INFO: 找到历史语言设置, 使用历史语言.")
         return language
 
 
 async def load_work_dir_from_txt() -> str:
     """
     Load a working path from file.
```

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/live_utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/live_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/search_utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/search_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/user_utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/user_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/utils/video_utils.py` & `bili-uas-0.2.1/Bili_UAS/utils/video_utils.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/Bili_UAS/writer/log_writer.py` & `bili-uas-0.2.1/Bili_UAS/writer/log_writer.py`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/LICENSE` & `bili-uas-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/PKG-INFO` & `bili-uas-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.2.0
+Version: 0.2.1
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.2.0/README.md` & `bili-uas-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/bili_uas.egg-info/PKG-INFO` & `bili-uas-0.2.1/bili_uas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bili-uas
-Version: 0.2.0
+Version: 0.2.1
 Summary: Assist up in personal, live, and video data analysis and prediction.
 Home-page: https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System
 Author: jhzg
 Author-email: jhzg02200059@163.com
 License: GPLv3
 Keywords: BiliBili,auxiliary,analysis,live,video,word_cloud,monitor
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `bili-uas-0.2.0/bili_uas.egg-info/SOURCES.txt` & `bili-uas-0.2.1/bili_uas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bili-uas-0.2.0/setup.py` & `bili-uas-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'apscheduler~=3.10.1',
     'requests~=2.31.0',
     'httpx~=0.24.1',
     'openpyxl~=3.1.2']
 
 setup(
     name='bili-uas',
-    version='0.2.0',
+    version='0.2.1',
     license='GPLv3',
     author='jhzg',
     author_email='jhzg02200059@163.com',
     url='https://github.com/jhzgjhzg/BiliBili-UP-Auxiliary-System',
     description='Assist up in personal, live, and video data analysis and prediction.',
     long_description=long_description,
     long_description_content_type='text/markdown',
```

