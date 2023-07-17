# Comparing `tmp/x11-automation-0.3.4.tar.gz` & `tmp/x11-automation-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x11-automation-0.3.4.tar", last modified: Mon Jul 10 22:56:14 2023, max compression
+gzip compressed data, was "x11-automation-0.3.5.tar", last modified: Mon Jul 17 21:00:25 2023, max compression
```

## Comparing `x11-automation-0.3.4.tar` & `x11-automation-0.3.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-10 22:56:14.188129 x11-automation-0.3.4/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1071 2023-06-26 23:44:38.000000 x11-automation-0.3.4/LICENSE.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-10 22:56:14.188129 x11-automation-0.3.4/PKG-INFO
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      266 2023-06-26 23:44:01.000000 x11-automation-0.3.4/README.md
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      409 2023-07-10 22:56:14.192129 x11-automation-0.3.4/setup.cfg
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       37 2023-06-26 23:41:00.000000 x11-automation-0.3.4/setup.py
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-10 22:56:14.188129 x11-automation-0.3.4/x11_automation/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      361 2023-07-01 02:22:06.000000 x11-automation-0.3.4/x11_automation/__init__.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        0 2023-06-26 23:46:08.000000 x11-automation-0.3.4/x11_automation/__main__.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      619 2023-07-01 02:21:34.000000 x11-automation-0.3.4/x11_automation/get_win_geometry.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1214 2023-07-01 01:18:51.000000 x11-automation-0.3.4/x11_automation/move_mouse_to_new_window.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      536 2023-07-06 14:38:38.000000 x11-automation-0.3.4/x11_automation/send.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      122 2023-06-27 02:52:06.000000 x11-automation-0.3.4/x11_automation/win_activate.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      974 2023-07-10 22:54:15.000000 x11-automation-0.3.4/x11_automation/win_exists.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      209 2023-06-27 01:15:56.000000 x11-automation-0.3.4/x11_automation/win_get_process.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      499 2023-06-27 01:15:56.000000 x11-automation-0.3.4/x11_automation/win_wait_active.py
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       46 2023-06-27 01:13:09.000000 x11-automation-0.3.4/x11_automation/x11_automation.py
-drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-10 22:56:14.188129 x11-automation-0.3.4/x11_automation.egg-info/
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        2 2023-07-06 14:40:01.000000 x11-automation-0.3.4/x11_automation.egg-info/.gitignore
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-10 22:56:14.000000 x11-automation-0.3.4/x11_automation.egg-info/PKG-INFO
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      580 2023-07-10 22:56:14.000000 x11-automation-0.3.4/x11_automation.egg-info/SOURCES.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        1 2023-07-10 22:56:14.000000 x11-automation-0.3.4/x11_automation.egg-info/dependency_links.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       31 2023-07-10 22:56:14.000000 x11-automation-0.3.4/x11_automation.egg-info/requires.txt
--rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       15 2023-07-10 22:56:14.000000 x11-automation-0.3.4/x11_automation.egg-info/top_level.txt
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-17 21:00:25.358133 x11-automation-0.3.5/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1071 2023-06-26 23:44:38.000000 x11-automation-0.3.5/LICENSE.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-17 21:00:25.358133 x11-automation-0.3.5/PKG-INFO
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      266 2023-06-26 23:44:01.000000 x11-automation-0.3.5/README.md
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      409 2023-07-17 21:00:25.362133 x11-automation-0.3.5/setup.cfg
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       37 2023-06-26 23:41:00.000000 x11-automation-0.3.5/setup.py
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-17 21:00:25.358133 x11-automation-0.3.5/x11_automation/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      361 2023-07-01 02:22:06.000000 x11-automation-0.3.5/x11_automation/__init__.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        0 2023-06-26 23:46:08.000000 x11-automation-0.3.5/x11_automation/__main__.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      619 2023-07-01 02:21:34.000000 x11-automation-0.3.5/x11_automation/get_win_geometry.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1214 2023-07-01 01:18:51.000000 x11-automation-0.3.5/x11_automation/move_mouse_to_new_window.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      536 2023-07-06 14:38:38.000000 x11-automation-0.3.5/x11_automation/send.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      512 2023-07-17 20:59:24.000000 x11-automation-0.3.5/x11_automation/win_activate.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      974 2023-07-10 22:54:15.000000 x11-automation-0.3.5/x11_automation/win_exists.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      209 2023-06-27 01:15:56.000000 x11-automation-0.3.5/x11_automation/win_get_process.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      499 2023-06-27 01:15:56.000000 x11-automation-0.3.5/x11_automation/win_wait_active.py
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       46 2023-06-27 01:13:09.000000 x11-automation-0.3.5/x11_automation/x11_automation.py
+drwxrwxr-x   0 jok4r     (1000) jok4r     (1000)        0 2023-07-17 21:00:25.358133 x11-automation-0.3.5/x11_automation.egg-info/
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        2 2023-07-06 14:40:01.000000 x11-automation-0.3.5/x11_automation.egg-info/.gitignore
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)     1582 2023-07-17 21:00:25.000000 x11-automation-0.3.5/x11_automation.egg-info/PKG-INFO
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)      580 2023-07-17 21:00:25.000000 x11-automation-0.3.5/x11_automation.egg-info/SOURCES.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)        1 2023-07-17 21:00:25.000000 x11-automation-0.3.5/x11_automation.egg-info/dependency_links.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       31 2023-07-17 21:00:25.000000 x11-automation-0.3.5/x11_automation.egg-info/requires.txt
+-rw-rw-r--   0 jok4r     (1000) jok4r     (1000)       15 2023-07-17 21:00:25.000000 x11-automation-0.3.5/x11_automation.egg-info/top_level.txt
```

### Comparing `x11-automation-0.3.4/LICENSE.txt` & `x11-automation-0.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.4/PKG-INFO` & `x11-automation-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x11-automation
-Version: 0.3.4
+Version: 0.3.5
 Summary: X11-Automation
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: opensuse12@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `x11-automation-0.3.4/x11_automation/get_win_geometry.py` & `x11-automation-0.3.5/x11_automation/get_win_geometry.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.4/x11_automation/move_mouse_to_new_window.py` & `x11-automation-0.3.5/x11_automation/move_mouse_to_new_window.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.4/x11_automation/send.py` & `x11-automation-0.3.5/x11_automation/send.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.4/x11_automation/win_exists.py` & `x11-automation-0.3.5/x11_automation/win_exists.py`

 * *Files identical despite different names*

### Comparing `x11-automation-0.3.4/x11_automation.egg-info/PKG-INFO` & `x11-automation-0.3.5/x11_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x11-automation
-Version: 0.3.4
+Version: 0.3.5
 Summary: X11-Automation
 Home-page: 
 Author: Dmitry Yakovlev
 Author-email: opensuse12@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `x11-automation-0.3.4/x11_automation.egg-info/SOURCES.txt` & `x11-automation-0.3.5/x11_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

