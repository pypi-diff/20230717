# Comparing `tmp/processview-1.3.0.tar.gz` & `tmp/processview-1.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "processview-1.3.0.tar", last modified: Mon Jul 17 11:46:58 2023, max compression
+gzip compressed data, was "processview-1.3.0a0.tar", last modified: Thu Jul 13 11:01:37 2023, max compression
```

## Comparing `processview-1.3.0.tar` & `processview-1.3.0a0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0/LICENSE
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-07-17 11:46:58.985711 processview-1.3.0/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.3.0/README.md
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview/
--rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.3.0/processview/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview/core/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/dataset.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/helpers.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview/core/manager/
--rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/manager/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    13705 2023-07-17 11:46:44.000000 processview-1.3.0/processview/core/manager/manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview/core/manager/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/manager/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/manager/test/test_manager.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/setup.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/sorting.py
--rw-r--r--   0 payno     (1001) payno     (1001)     5392 2023-07-17 11:46:44.000000 processview-1.3.0/processview/core/superviseprocess.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview/core/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.3.0/processview/core/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/gui/
--rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0/processview/gui/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.3.0/processview/gui/icons.py
--rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.3.0/processview/gui/messagebox.py
--rw-r--r--   0 payno     (1001) payno     (1001)    26706 2023-07-17 11:46:44.000000 processview-1.3.0/processview/gui/processmanager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/gui/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.3.0/processview/gui/test/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.3.0/processview/gui/test/test_process_manager.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/resources/
--rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.3.0/processview/resources/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.977711 processview-1.3.0/processview/resources/gui/
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/resources/gui/icons/
--rw-r--r--   0 payno     (1001) payno     (1001)      729 2023-06-21 09:33:50.000000 processview-1.3.0/processview/resources/gui/icons/advancement.png
--rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 09:33:50.000000 processview-1.3.0/processview/resources/gui/icons/advancement.svg
--rw-r--r--   0 payno     (1001) payno     (1001)      926 2023-06-21 09:33:50.000000 processview-1.3.0/processview/resources/gui/icons/magnifying_glass.png
--rw-r--r--   0 payno     (1001) payno     (1001)     4631 2023-06-21 09:33:50.000000 processview-1.3.0/processview/resources/gui/icons/magnifying_glass.svg
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/test/
--rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.3.0/processview/test/__init__.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.985711 processview-1.3.0/processview/utils/
--rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.3.0/processview/utils/__init__.py
--rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.3.0/processview/utils/singleton.py
--rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-07-17 11:46:44.000000 processview-1.3.0/processview/version.py
-drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-17 11:46:58.981711 processview-1.3.0/processview.egg-info/
--rw-r--r--   0 payno     (1001) payno     (1001)     1063 2023-07-17 11:46:58.000000 processview-1.3.0/processview.egg-info/PKG-INFO
--rw-r--r--   0 payno     (1001) payno     (1001)     1179 2023-07-17 11:46:58.000000 processview-1.3.0/processview.egg-info/SOURCES.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-07-17 11:46:58.000000 processview-1.3.0/processview.egg-info/dependency_links.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-07-17 11:46:58.000000 processview-1.3.0/processview.egg-info/requires.txt
--rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-07-17 11:46:58.000000 processview-1.3.0/processview.egg-info/top_level.txt
--rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.3.0/processview.egg-info/zip-safe
--rw-r--r--   0 payno     (1001) payno     (1001)     1196 2023-07-17 11:46:58.985711 processview-1.3.0/setup.cfg
--rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.3.0/setup.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/LICENSE
+-rw-r--r--   0 payno     (1001) payno     (1001)     1065 2023-07-13 11:01:37.750609 processview-1.3.0a0/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)      767 2023-06-21 09:33:50.000000 processview-1.3.0a0/README.md
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.742609 processview-1.3.0a0/processview/
+-rw-r--r--   0 payno     (1001) payno     (1001)       91 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3289 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/dataset.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2350 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/helpers.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/manager/
+-rw-r--r--   0 payno     (1001) payno     (1001)       23 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    13677 2023-07-13 11:00:07.000000 processview-1.3.0a0/processview/core/manager/manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/manager/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1534 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4823 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/manager/test/test_manager.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1745 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/setup.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1067 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/sorting.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     5128 2023-07-13 11:00:07.000000 processview-1.3.0a0/processview/core/superviseprocess.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/core/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1561 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/core/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/gui/
+-rw-r--r--   0 payno     (1001) payno     (1001)        0 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    12926 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/icons.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     2296 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/messagebox.py
+-rw-r--r--   0 payno     (1001) payno     (1001)    26124 2023-07-13 11:00:09.000000 processview-1.3.0a0/processview/gui/processmanager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/gui/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1584 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/test/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     3666 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/gui/test/test_process_manager.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/resources/
+-rw-r--r--   0 payno     (1001) payno     (1001)    10757 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.738609 processview-1.3.0a0/processview/resources/gui/
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.746609 processview-1.3.0a0/processview/resources/gui/icons/
+-rw-r--r--   0 payno     (1001) payno     (1001)      729 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/advancement.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     5781 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/advancement.svg
+-rw-r--r--   0 payno     (1001) payno     (1001)      926 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.png
+-rw-r--r--   0 payno     (1001) payno     (1001)     4631 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.svg
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/processview/test/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1695 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/test/__init__.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.750609 processview-1.3.0a0/processview/utils/
+-rw-r--r--   0 payno     (1001) payno     (1001)     2565 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/utils/__init__.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     1559 2023-06-21 09:33:50.000000 processview-1.3.0a0/processview/utils/singleton.py
+-rw-r--r--   0 payno     (1001) payno     (1001)     4411 2023-07-13 11:00:41.000000 processview-1.3.0a0/processview/version.py
+drwxr-xr-x   0 payno     (1001) payno     (1001)        0 2023-07-13 11:01:37.742609 processview-1.3.0a0/processview.egg-info/
+-rw-r--r--   0 payno     (1001) payno     (1001)     1065 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/PKG-INFO
+-rw-r--r--   0 payno     (1001) payno     (1001)     1179 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/SOURCES.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/dependency_links.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       94 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/requires.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)       12 2023-07-13 11:01:37.000000 processview-1.3.0a0/processview.egg-info/top_level.txt
+-rw-r--r--   0 payno     (1001) payno     (1001)        1 2023-06-21 09:48:11.000000 processview-1.3.0a0/processview.egg-info/zip-safe
+-rw-r--r--   0 payno     (1001) payno     (1001)     1196 2023-07-13 11:01:37.750609 processview-1.3.0a0/setup.cfg
+-rw-r--r--   0 payno     (1001) payno     (1001)       69 2023-06-21 09:33:50.000000 processview-1.3.0a0/setup.py
```

### Comparing `processview-1.3.0/PKG-INFO` & `processview-1.3.0a0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.3.0/README.md` & `processview-1.3.0a0/README.md`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/dataset.py` & `processview-1.3.0a0/processview/core/dataset.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/helpers.py` & `processview-1.3.0a0/processview/core/helpers.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/manager/manager.py` & `processview-1.3.0a0/processview/core/manager/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 
     ON_GOING = "on going"
     SUCCEED = "succeed"
     FAILED = "failed"
     PENDING = "pending"
     SKIPPED = "skipped"
     WAIT_USER_VALIDATION = "waiting user validation"
-    CANCELLED = "cancelled"
 
 
 @singleton
 class ProcessManager:
     """
     Manager to register and observe `SuperviseProcess`.
     """
```

### Comparing `processview-1.3.0/processview/core/manager/test/__init__.py` & `processview-1.3.0a0/processview/core/manager/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/manager/test/test_manager.py` & `processview-1.3.0a0/processview/core/manager/test/test_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/setup.py` & `processview-1.3.0a0/processview/core/setup.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/sorting.py` & `processview-1.3.0a0/processview/core/sorting.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/core/superviseprocess.py` & `processview-1.3.0a0/processview/core/superviseprocess.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,21 +24,18 @@
 # ###########################################################################*/
 
 __authors__ = ["H. Payno"]
 __license__ = "MIT"
 __date__ = "29/01/2021"
 
 
-import logging
 from .manager import ProcessManager
 from .manager import DatasetState
 from .dataset import Dataset
 
-_logger = logging.getLogger(__name__)
-
 
 class SuperviseProcess:
     """
     Supervise process are processes with a state.
     They are decoupled of BaseProcess because a SuperviseProcess can be
     a group of BaseProcess. This is more dedicated to users.
     For example Axis is a Base process that could only 'Suceed' or 'Failed'
@@ -125,19 +122,10 @@
             dataset=dataset, state=state, process=self, details=details
         )
 
     def reprocess(self, dataset):
         """
         Reprocess a dataset.
 
-        :param Dataset dataset: dataset to reprocess
+        :param Dataset: dataset to reprocess
         """
         raise NotImplementedError("Base class")
-
-    def cancel(self):
-        """
-        cancel (abort) current processing
-
-        """
-        _logger.warning(
-            f"process cancellation haven't been implemented for {self.name}"
-        )
```

### Comparing `processview-1.3.0/processview/core/test/__init__.py` & `processview-1.3.0a0/processview/core/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/gui/icons.py` & `processview-1.3.0a0/processview/gui/icons.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/gui/messagebox.py` & `processview-1.3.0a0/processview/gui/messagebox.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/gui/processmanager.py` & `processview-1.3.0a0/processview/gui/processmanager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,14 @@
 _DATASET_STATE_BACKGROUND = {
     DatasetState.ON_GOING: qt.QColor("#839684"),  # light blue
     DatasetState.SUCCEED: qt.QColor("#068c0c"),  # green
     DatasetState.FAILED: qt.QColor("#f52718"),  # red
     DatasetState.PENDING: qt.QColor("#609ab3"),  # blue gray
     DatasetState.SKIPPED: qt.QColor("#f08e0e"),  # light orange
     DatasetState.WAIT_USER_VALIDATION: qt.QColor("#cb34c1"),  # pink
-    DatasetState.CANCELLED: qt.QColor("#a4a8a2"),  # light black
 }
 
 
 class ProcessManagerWindow(qt.QMainWindow):
     """
     Main window of the process manager
     """
@@ -85,29 +84,26 @@
         self._clearAction = qt.QAction("clear")
         self.dataset_menu.addAction(self._clearAction)
 
         # QMenu for cell from on dataset and one process
         self.menu_dataset_vs_process = qt.QMenu()
         self._reprocessAction = qt.QAction("reprocess")
         self.menu_dataset_vs_process.addAction(self._reprocessAction)
-        self._cancelAction = qt.QAction("cancel")
-        self.menu_dataset_vs_process.addAction(self._cancelAction)
         self._infoAction = qt.QAction("info")
         self.menu_dataset_vs_process.addAction(self._infoAction)
         self.menu_dataset_vs_process.addAction(self._clearAction)
 
         self._target = (None, None)
         # register target of the last menu (process, DatasetIdentifier)
 
         # connect signal / slot
         self._copyAction.triggered.connect(self._requestDatasetIdCopy)
         self._clearAction.triggered.connect(self._requestClearDataset)
         self._reprocessAction.triggered.connect(self._requestReprocessing)
         self._infoAction.triggered.connect(self._requestInfo)
-        self._cancelAction.triggered.connect(self._requestCancelProcessing)
 
     def _processAt(self, x_pos):
         column = self.columnAt(x_pos)
         if column >= 1:
             processes = self.model()._processes
             process_idx = column - 1
             if process_idx < len(processes):
@@ -145,21 +141,14 @@
         process, dataset = self._target
 
         if process is not None and dataset is not None:
             assert isinstance(process, SuperviseProcess)
             assert isinstance(dataset, DatasetIdentifier)
             process.reprocess(dataset.recreate_dataset())
 
-    def _requestCancelProcessing(self, *args, **kwargs):
-        process, dataset = self._target
-        if process is not None and dataset is not None:
-            assert isinstance(process, SuperviseProcess)
-            assert isinstance(dataset, DatasetIdentifier)
-            process.cancel(dataset.recreate_dataset())
-
     def _requestDatasetIdCopy(self, *args, **kwargs):
         _, dataset = self._target
         if dataset is not None:
             clipboard = qt.QGuiApplication.clipboard()
             clipboard.setText(dataset.to_str())
 
     def _requestClearDataset(self, *args, **kwargs):
```

### Comparing `processview-1.3.0/processview/gui/test/__init__.py` & `processview-1.3.0a0/processview/gui/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/gui/test/test_process_manager.py` & `processview-1.3.0a0/processview/gui/test/test_process_manager.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/resources/__init__.py` & `processview-1.3.0a0/processview/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/resources/gui/icons/advancement.png` & `processview-1.3.0a0/processview/resources/gui/icons/advancement.png`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/resources/gui/icons/advancement.svg` & `processview-1.3.0a0/processview/resources/gui/icons/advancement.svg`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/resources/gui/icons/magnifying_glass.png` & `processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.png`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/resources/gui/icons/magnifying_glass.svg` & `processview-1.3.0a0/processview/resources/gui/icons/magnifying_glass.svg`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/test/__init__.py` & `processview-1.3.0a0/processview/test/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/utils/__init__.py` & `processview-1.3.0a0/processview/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/utils/singleton.py` & `processview-1.3.0a0/processview/utils/singleton.py`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/processview/version.py` & `processview-1.3.0a0/processview/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     "rc": 12,
     "final": 15,
 }
 
 MAJOR = 1
 MINOR = 3
 MICRO = 0
-RELEV = "final"  # <16
+RELEV = "alpha"  # <16
 SERIAL = 0  # <16
 
 date = __date__
 
 from collections import namedtuple
 
 _version_info = namedtuple(
```

### Comparing `processview-1.3.0/processview.egg-info/PKG-INFO` & `processview-1.3.0a0/processview.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: processview
-Version: 1.3.0
+Version: 1.3.0a0
 Summary: Simple helper to provide user feedback about dataset processing
 Author: data analysis unit
 Author-email: henri.payno@esrf.fr
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
```

### Comparing `processview-1.3.0/processview.egg-info/SOURCES.txt` & `processview-1.3.0a0/processview.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `processview-1.3.0/setup.cfg` & `processview-1.3.0a0/setup.cfg`

 * *Files identical despite different names*

