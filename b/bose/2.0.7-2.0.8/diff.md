# Comparing `tmp/bose-2.0.7.tar.gz` & `tmp/bose-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-2.0.7.tar", last modified: Thu Jul 13 15:37:04 2023, max compression
+gzip compressed data, was "bose-2.0.8.tar", last modified: Mon Jul 17 03:57:16 2023, max compression
```

## Comparing `bose-2.0.7.tar` & `bose-2.0.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:37:04.916600 bose-2.0.7/
--rw-rw-rw-   0        0        0    14120 2023-07-13 15:37:04.916600 bose-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.7/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-13 15:37:04.916600 bose-2.0.7/bose/
--rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.7/bose/__init__.py
--rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.7/bose/account_generator.py
--rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.7/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.7/bose/base_data.py
--rw-rw-rw-   0        0        0     8287 2023-07-01 12:32:35.823549 bose-2.0.7/bose/base_task.py
--rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.7/bose/beep_utils.py
--rw-rw-rw-   0        0        0    10586 2023-07-13 15:33:35.445633 bose-2.0.7/bose/bose_driver.py
--rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.7/bose/bose_undetected_driver.py
--rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.7/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.7/bose/download_driver.py
--rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.7/bose/ip_utils.py
--rw-rw-rw-   0        0        0     3040 2023-07-09 14:30:45.891095 bose-2.0.7/bose/launch_tasks.py
--rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.7/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.7/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.7/bose/opponent.py
--rw-rw-rw-   0        0        0     3130 2023-07-11 16:45:26.788592 bose-2.0.7/bose/output.py
--rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.7/bose/profile.py
--rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.7/bose/schedule_utils.py
--rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.7/bose/task_config.py
--rw-rw-rw-   0        0        0     1375 2023-07-01 09:14:29.721606 bose-2.0.7/bose/task_info.py
--rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.7/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.7/bose/user_agent.py
--rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.7/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.7/bose/wait.py
--rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.7/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2312 2023-07-13 15:36:43.101330 bose-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:57:16.158173 bose-2.0.8/
+-rw-rw-rw-   0        0        0    14120 2023-07-17 03:57:16.158173 bose-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    10357 2023-07-06 11:59:35.580609 bose-2.0.8/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-17 03:57:16.158173 bose-2.0.8/bose/
+-rw-rw-rw-   0        0        0      452 2023-06-30 14:14:28.791702 bose-2.0.8/bose/__init__.py
+-rw-rw-rw-   0        0        0     4160 2023-07-01 09:12:23.121716 bose-2.0.8/bose/account_generator.py
+-rw-rw-rw-   0        0        0      707 2023-06-30 05:04:43.924597 bose-2.0.8/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-2.0.8/bose/base_data.py
+-rw-rw-rw-   0        0        0     8356 2023-07-17 03:55:40.349391 bose-2.0.8/bose/base_task.py
+-rw-rw-rw-   0        0        0      317 2023-06-29 11:53:16.211079 bose-2.0.8/bose/beep_utils.py
+-rw-rw-rw-   0        0        0    10586 2023-07-13 15:33:35.445633 bose-2.0.8/bose/bose_driver.py
+-rw-rw-rw-   0        0        0    10384 2023-07-06 11:56:35.717259 bose-2.0.8/bose/bose_undetected_driver.py
+-rw-rw-rw-   0        0        0     7884 2023-07-01 17:18:08.107702 bose-2.0.8/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-2.0.8/bose/download_driver.py
+-rw-rw-rw-   0        0        0      993 2023-07-06 10:42:02.261172 bose-2.0.8/bose/ip_utils.py
+-rw-rw-rw-   0        0        0     3040 2023-07-09 14:30:45.891095 bose-2.0.8/bose/launch_tasks.py
+-rw-rw-rw-   0        0        0     3185 2023-06-29 08:54:46.918966 bose-2.0.8/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-2.0.8/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-2.0.8/bose/opponent.py
+-rw-rw-rw-   0        0        0     3130 2023-07-11 16:45:26.788592 bose-2.0.8/bose/output.py
+-rw-rw-rw-   0        0        0     4600 2023-07-01 06:42:54.180748 bose-2.0.8/bose/profile.py
+-rw-rw-rw-   0        0        0      853 2023-06-29 11:00:24.518432 bose-2.0.8/bose/schedule_utils.py
+-rw-rw-rw-   0        0        0      460 2023-06-29 10:04:53.656427 bose-2.0.8/bose/task_config.py
+-rw-rw-rw-   0        0        0     1859 2023-07-17 03:55:54.165141 bose-2.0.8/bose/task_info.py
+-rw-rw-rw-   0        0        0     5429 2023-06-26 10:10:30.768354 bose-2.0.8/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7480 2023-07-03 07:28:55.309830 bose-2.0.8/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6210 2023-07-01 09:18:35.128413 bose-2.0.8/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-2.0.8/bose/wait.py
+-rw-rw-rw-   0        0        0     1222 2023-07-01 17:18:01.675976 bose-2.0.8/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-07-17 03:56:45.238680 bose-2.0.8/setup.py
```

### Comparing `bose-2.0.7/PKG-INFO` & `bose-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 2.0.7
+Version: 2.0.8
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-2.0.7/README.rst` & `bose-2.0.8/README.rst`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/account_generator.py` & `bose-2.0.8/bose/account_generator.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/analytics.py` & `bose-2.0.8/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/base_data.py` & `bose-2.0.8/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/base_task.py` & `bose-2.0.8/bose/base_task.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         return create_driver(config)
     
     def begin_task(self, data, task_config:TaskConfig):
         def create_directories(task_path):
 
             driver_path =  relative_path(get_driver_path(), 0)
             if not os.path.isfile(driver_path):
-                print('Downloading Driver in build/ directory ...')
+                print('[INFO] Downloading Chrome Driver in build/ directory. This is a one-time process. Download in progress...')
                 _download_driver()
 
             tasks_path =  relative_path('tasks/', 0)
             if not os.path.exists(tasks_path):
                 os.makedirs(tasks_path)
 
             output_path =  relative_path('output/', 0)
@@ -144,15 +144,15 @@
             task_name = self.__class__.__name__
             task.set_task_name(task_name)
 
             final_image = "final.png"
             def end_task(driver:BoseDriver):
                 task.end()
                 task.set_ip()
-                data = task.data
+                data = task.get_data()
                 driver.save_screenshot(final_image)
                 
                 html_path  = f'{self.task_path}/page.html'
                 source = get_page_source_safe(driver)
                 write_html(source, html_path)
 
                 data["last_url"] = get_driver_url_safe(driver)
```

### Comparing `bose-2.0.7/bose/bose_driver.py` & `bose-2.0.8/bose/bose_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/bose_undetected_driver.py` & `bose-2.0.8/bose/bose_undetected_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/create_driver.py` & `bose-2.0.8/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/download_driver.py` & `bose-2.0.8/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/ip_utils.py` & `bose-2.0.8/bose/ip_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/launch_tasks.py` & `bose-2.0.8/bose/launch_tasks.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/local_storage.py` & `bose-2.0.8/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/local_storage_driver.py` & `bose-2.0.8/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/output.py` & `bose-2.0.8/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/profile.py` & `bose-2.0.8/bose/profile.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/schedule_utils.py` & `bose-2.0.8/bose/schedule_utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/task_info.py` & `bose-2.0.8/bose/task_info.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,14 @@
-import requests
 from datetime import datetime
-import traceback
-
 from .ip_utils import find_ip_details
-
 from .utils import pretty_format_time
 
 
-def format_time_diff(start_time, end_time):
-    time_diff = end_time - start_time
+def format_time_diff(start_time_datetime, end_time_datetime):
+    time_diff = end_time_datetime - start_time_datetime
     total_seconds = int(time_diff.total_seconds())
 
     minutes, seconds = divmod(total_seconds, 60)
 
     # Format the time difference as a string
     time_str = ""
     if minutes > 0:
@@ -20,38 +16,51 @@
     if seconds >= 0:
         if time_str:
             time_str += " "
         time_str += f"{seconds} {'seconds' if seconds > 1 else 'second'}"
 
     return time_str
 
+def copy_and_remove_keys(input_dict):
+    # Make a shallow copy of the input dictionary
+    new_dict = input_dict.copy()
+
+    # Remove the specified keys if they exist in the dictionary
+    keys_to_remove = ['end_time_datetime', 'start_time_datetime']
+    for key in keys_to_remove:
+        new_dict.pop(key, None)
+
+    return new_dict
 
 class TaskInfo():
   data = {}
   
   def start(self):
-    self.data["start_time"] = datetime.now()
+    self.data["start_time_datetime"] = datetime.now()
     pass
   
+  def get_data(self):
+     return copy_and_remove_keys(self.data)
   
   def end(self):
-    self.data["end_time"] = datetime.now()
-    self.data["duration"] = format_time_diff(self.data["start_time"],self.data["end_time"])
+    self.data["end_time_datetime"] = datetime.now()
+    self.data["duration"] = format_time_diff(self.data["start_time_datetime"],self.data["end_time_datetime"])
     
 
-    self.data["start_time"] = pretty_format_time(self.data["start_time"])
-    self.data["end_time"] = pretty_format_time(self.data["end_time"])
+    self.data["start_time"] = pretty_format_time(self.data["start_time_datetime"])
+    self.data["end_time"] = pretty_format_time(self.data["end_time_datetime"])
 
 
   def set_ip(self):
     self.data["ip_details"] = find_ip_details()
 
   def set_task_name(self, task_name):
     self.data["task_name"] = task_name
 
 
 if __name__ == "__main__":
     t = TaskInfo()
     t.start()
     t.end()
+    t.end()
     t.set_ip()
-    print(t.data)
+    print(t.get_data())
```

### Comparing `bose-2.0.7/bose/temp_mail.py` & `bose-2.0.8/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/user_agent.py` & `bose-2.0.8/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/utils.py` & `bose-2.0.8/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/bose/window_size.py` & `bose-2.0.8/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-2.0.7/setup.py` & `bose-2.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     except:
       return None
     
             
 setup(
     name='bose',
     packages=['bose'],
-    version='2.0.7',
+    version='2.0.8',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/",
         "Source": "https://github.com/omkarcloud/bose",
         "Tracker": "https://github.com/omkarcloud/bose/issues",
     },
```

