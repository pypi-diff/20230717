# Comparing `tmp/com.castsoftware.uc.oneclick-0.2.3.2b0.tar.gz` & `tmp/com.castsoftware.uc.oneclick-0.2.3.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.3.2b0.tar", last modified: Thu Jun 29 23:50:51 2023, max compression
+gzip compressed data, was "com.castsoftware.uc.oneclick-0.2.3.3b0.tar", last modified: Mon Jul 17 18:00:19 2023, max compression
```

## Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0.tar` & `com.castsoftware.uc.oneclick-0.2.3.3b0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-06-29 23:50:51.158737 com.castsoftware.uc.oneclick-0.2.3.2b0/
--rw-rw-rw-   0        0        0      519 2023-06-29 23:50:51.150525 com.castsoftware.uc.oneclick-0.2.3.2b0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.619769 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/
--rw-rw-rw-   0        0        0      519 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      836 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      179 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-29 23:50:50.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.745750 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/
--rw-rw-rw-   0        0        0        2 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:50:50.978145 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/
--rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/__init__.py
--rw-rw-rw-   0        0        0     2745 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/aip_analysis.py
--rw-rw-rw-   0        0        0     1231 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/analysis.py
--rw-rw-rw-   0        0        0     4068 2023-06-29 19:27:55.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/highlight_analysis.py
--rw-rw-rw-   0        0        0     4706 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/trackAnalysis.py
--rw-rw-rw-   0        0        0    24987 2023-06-29 16:00:26.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/config.py
-drwxrwxrwx   0        0        0        0 2023-06-29 23:50:51.139469 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/
--rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/__init__.py
--rw-rw-rw-   0        0        0     4740 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cleanup.py
--rw-rw-rw-   0        0        0     7274 2023-06-29 23:42:53.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cloc.py
--rw-rw-rw-   0        0        0     9130 2023-06-28 22:43:16.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/discoveryReport.py
--rw-rw-rw-   0        0        0     2893 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/prep.py
--rw-rw-rw-   0        0        0      491 2023-06-29 11:52:29.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sourceValidation.py
--rw-rw-rw-   0        0        0     6835 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sqlDiscovery.py
--rw-rw-rw-   0        0        0     2740 2023-06-29 17:12:02.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/unzip.py
--rw-rw-rw-   0        0        0      305 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/exceptions.py
--rw-rw-rw-   0        0        0    10978 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/main.py
--rw-rw-rw-   0        0        0     2152 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/runArg.py
--rw-rw-rw-   0        0        0     2098 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/sendEmail.py
--rw-rw-rw-   0        0        0     3947 2023-06-28 21:49:06.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/setup.py
--rw-rw-rw-   0        0        0      779 2023-06-29 23:50:33.000000 com.castsoftware.uc.oneclick-0.2.3.2b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-29 23:50:51.158737 com.castsoftware.uc.oneclick-0.2.3.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 18:00:19.607748 com.castsoftware.uc.oneclick-0.2.3.3b0/
+-rw-rw-rw-   0        0        0      519 2023-07-17 18:00:19.600664 com.castsoftware.uc.oneclick-0.2.3.3b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-17 18:00:19.386350 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-07-17 18:00:19.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      836 2023-07-17 18:00:19.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 18:00:19.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      179 2023-07-17 18:00:19.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-17 18:00:19.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 18:00:19.452935 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/
+-rw-rw-rw-   0        0        0        2 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:00:19.492505 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/__init__.py
+-rw-rw-rw-   0        0        0     2745 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/aip_analysis.py
+-rw-rw-rw-   0        0        0     1231 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/analysis.py
+-rw-rw-rw-   0        0        0     4068 2023-06-29 19:27:55.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/highlight_analysis.py
+-rw-rw-rw-   0        0        0     4706 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/trackAnalysis.py
+-rw-rw-rw-   0        0        0    24987 2023-06-29 16:00:26.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/config.py
+drwxrwxrwx   0        0        0        0 2023-07-17 18:00:19.594520 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/
+-rw-rw-rw-   0        0        0        0 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/__init__.py
+-rw-rw-rw-   0        0        0     4740 2023-06-28 21:49:05.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/cleanup.py
+-rw-rw-rw-   0        0        0     8404 2023-07-17 17:44:07.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/cloc.py
+-rw-rw-rw-   0        0        0     9130 2023-06-28 22:43:16.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/discoveryReport.py
+-rw-rw-rw-   0        0        0     2893 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/prep.py
+-rw-rw-rw-   0        0        0      491 2023-06-29 11:52:29.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/sourceValidation.py
+-rw-rw-rw-   0        0        0     6835 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/sqlDiscovery.py
+-rw-rw-rw-   0        0        0     3255 2023-07-10 18:56:26.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/unzip.py
+-rw-rw-rw-   0        0        0      305 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/exceptions.py
+-rw-rw-rw-   0        0        0    10978 2023-06-06 12:30:59.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/main.py
+-rw-rw-rw-   0        0        0     2152 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/runArg.py
+-rw-rw-rw-   0        0        0     2098 2023-05-30 12:14:01.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/sendEmail.py
+-rw-rw-rw-   0        0        0     3947 2023-07-10 18:51:38.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/setup.py
+-rw-rw-rw-   0        0        0      779 2023-07-17 17:59:56.000000 com.castsoftware.uc.oneclick-0.2.3.3b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 18:00:19.607748 com.castsoftware.uc.oneclick-0.2.3.3b0/setup.cfg
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.3.2b0
+Version: 0.2.3.3b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO` & `com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.castsoftware.uc.oneclick
-Version: 0.2.3.2b0
+Version: 0.2.3.3b0
 Summary: Assessment Generator
 Project-URL: Homepage, https://github.com/CAST-Extend/com.castsoftware.uc.arg
 Project-URL: Bug Tracker, https://github.com/CAST-Extend/com.castsoftware.uc.arg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt` & `com.castsoftware.uc.oneclick-0.2.3.3b0/com.castsoftware.uc.oneclick.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/aip_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/aip_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/highlight_analysis.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/highlight_analysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/analysis/trackAnalysis.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/analysis/trackAnalysis.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/config.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/config.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cleanup.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/cleanup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/cloc.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/cloc.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from oneclick.config import Config
 from cast_common.logger import Logger,INFO
 from cast_common.util import run_process,check_process,format_table,create_folder
 from oneclick.discovery.sourceValidation import SourceValidation 
 from time import sleep
 
-from os import getcwd
+from platform import system
 from os.path import exists,abspath,getsize
 from re import findall
 from pandas import DataFrame,ExcelWriter
 
+from string import ascii_uppercase
+from win32api import GetLogicalDriveStrings
+from win32wnet import WNetOpenEnum,WNetEnumResource
+from win32netcon import RESOURCE_REMEMBERED,RESOURCETYPE_DISK
+
 from ctypes import windll, c_int, c_wchar_p
 
 #TODO: Convert total line to formulas (d1-SHP)
 #TODO: Format all numbers as integers not text (d1-SHP)
 #TODO: Group tabs in pairs (before, after) then by application (d2)
 
 class ClocPreCleanup(SourceValidation):
@@ -39,14 +44,31 @@
     def cloc_project(cls):
         return f'{cls.cloc_base}\\{cls.config.project_name}'
 
     @property
     def cloc_results(cls):
         return cls._df
 
+    def _get_free_drive(cls):
+        drives = set(ascii_uppercase[2:])
+        for d in GetLogicalDriveStrings().split(':\\\x00'):
+            drives.discard(d)
+        # Discard persistent network drives, even if not connected.
+        henum = WNetOpenEnum(RESOURCE_REMEMBERED, 
+            RESOURCETYPE_DISK, 0, None)
+        while True:
+            result = WNetEnumResource(henum)
+            if not result:
+                break
+            for r in result:
+                if len(r.lpLocalName) == 2 and r.lpLocalName[1] == ':':
+                    drives.discard(r.lpLocalName[0])
+        if drives:
+            return sorted(drives)[-1] + ':'
+
     def _run_cloc(cls,work_folder:str,cloc_output:str,cloc_output_ignored:str):
         args = [cls.cloc_path,work_folder,"--report-file",cloc_output,"--ignored",cloc_output_ignored,"--quiet"]
         cls._log.info(' '.join(args))
         proc = run_process(args,False)
 
         sleep(10)
         if proc.poll() is not None and exists(cloc_output):
@@ -68,36 +90,38 @@
         cloc_run=False
 
         DefineDosDevice = windll.kernel32.DefineDosDeviceW
         DefineDosDevice.argtypes = [ c_int, c_wchar_p, c_wchar_p ]
 
         project_folder=abspath(f'{config.work}/AIP/{config.project_name}')
         # Create a subst. Check the return for non-zero to mean success
-        if DefineDosDevice(0, "F:", project_folder ) == 0:
-            raise RuntimeError("Subst failed")
+        drive=project_folder
+        platform = system()
+        if platform == 'Windows':
+            drive = cls._get_free_drive()
+            if DefineDosDevice(0, drive, project_folder ) == 0:
+                raise RuntimeError("Subst failed")
 
         for appl in config.application:
             cls._log.info(f'Running {config.project_name}/{appl}')
             create_folder(f'{config.report}/{config.project_name}/{appl}')
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
             cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt')
-#            work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
-            work_folder = abspath(f'F:/{appl}')
+            if platform == 'Windows':            
+                work_folder = abspath(f'{drive}/{appl}')
+            else:
+                work_folder = abspath(f'{config.work}/AIP/{config.project_name}/{appl}')
 
             #if the report is already out there - no need to continue
             if exists(cloc_output):
                 process[appl]=None
                 continue 
             cloc_run=True
             process[appl] = cls._run_cloc(work_folder,cloc_output,cloc_output_ignored)
 
-        # Delete the subst.
-        if DefineDosDevice(2, "F:", project_folder ) == 0:
-            raise RuntimeError("Subst failed")
-
         #has all cloc processing completed
         all_done=False
         while (not all_done):
             all_done=True
             for p in process:
                 if process[p]=='DONE':
                     continue
@@ -115,14 +139,18 @@
                             cls._log.error(f'Error running cloc on {cloc_output} ({ret})')
 
                 if exists(cloc_output):
                     process[p]='DONE'
             if cloc_run:
                 sleep(60)
 
+        # Delete the subst.
+        if platform == 'Windows' and DefineDosDevice(2, drive, project_folder ) == 0:
+            raise RuntimeError("Subst failed")
+
         for appl in config.application:
             #reading cloc_output.txt file
             cloc_output = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-{cls.phase}.txt')
             cloc_output_ignored = abspath(f'{config.report}/{config.project_name}/{appl}/{appl}-cloc-ignored-{cls.phase}.txt') 
             cls._log.info(f'Processing {cloc_output}')
             with open(cloc_output, 'r') as f:
                 content = f.read()
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/discoveryReport.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/discoveryReport.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/prep.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/prep.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/sqlDiscovery.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/sqlDiscovery.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/discovery/unzip.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/discovery/unzip.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,74 +1,94 @@
 from os import walk,remove
-from os.path import abspath
+from os.path import abspath,exists
 
 #from shutil import unpack_archive
 from pyunpack import Archive
+from gzip import open as gz
+from tarfile import open as tar, TarError
+from shutil import copyfileobj
+
+from cast_common.util import create_folder
 
 from oneclick.discovery.sourceValidation import SourceValidation 
 from oneclick.config import Config
 
 class Unzip(SourceValidation):
+   skip = ['__MACOSX','.DS_Store']
 
    def __init__(cls, config:Config, log_level:int):
         super().__init__(config,cls.__class__.__name__,log_level)
 
+   def unzip(cls,src_fldr) -> bool:
+      error = False
+      found = False
+      for root, dirs, files in walk(src_fldr):
+         try:
+            if '__MACOSX' in root or '.DS_Store' in files:
+               continue
+            for file in files:
+               full_name = abspath(f'{root.strip()}\\{file}')
+               dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
+
+               found=False
+               if file.endswith(".gz"):
+                  found = True
+                  with gz(full_name, 'rb') as f_in:
+                     if not exists(dest):
+                        with open(dest, 'wb') as f_out:
+                           copyfileobj(f_in, f_out)               
+
+               elif file.endswith(".tar") or file.endswith(".gztar") or file.endswith(".bztar"):
+                  with tar(full_name) as f_in:
+                     found = True
+                     create_folder(dest)
+                     f_in.extractall(dest)
+
+               elif file.endswith(".7z") or file.endswith(".zip") :
+                  found = True
+                  full_name = abspath(f'{root.strip()}\\{file}')
+                  Archive(full_name).extractall(dest,auto_create_dir=True)
+
+               if found:     
+                  cls._log.info(f'Unpacked: {full_name}')  
+                  remove(full_name)
+
+         except (TarError, ValueError, Exception) as ex:
+            cls._log.error(str(ex))
+            error = True
+
+      #terminate on error 
+      if error: 
+         raise
+
+      return found
 
    def run(cls,config:Config):
+      cls._log.info(f'Running {cls.__class__.__name__} for all applications')
       cls._log.debug('Running unzip step')
 
       #scan delivery folder for application folders
       apps= config.application
       # for (dirpath,dirnames,filenames) in walk(work_folder):
       #    apps.extend(dirnames)
 
       found = True
-      cls._log.info(f'Running {cls.__class__.__name__} for all applications')
       while found:
          found = False
          for app in apps:
-            app_folder_aip = f'{config.work}\\AIP\\{config.project_name}\\{app}'
-            for root, dirs, files in walk(app_folder_aip):
-               if '__MACOSX' in root or '.DS_Store' in files:
-                  continue
-               for file in files:
-                  if file.endswith(".zip") or \
-                     file.endswith(".7z") or \
-                     file.endswith(".tar") or \
-                     file.endswith(".gztar") or \
-                     file.endswith(".bztar"):
-                     found = True
-                     
-                     full_name = abspath(f'{root.strip()}\\{file}')
-                     dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
-                     cls._log.info(f'Unzipping {full_name}')
-
-                     Archive(full_name).extractall(dest,auto_create_dir=True)
-                     
-                     remove(full_name)
-
-            app_folder_hl = f'{config.work}\\HL\\{config.project_name}\\{app}'
-            for root, dirs, files in walk(app_folder_hl):
-               if '__MACOSX' in root:
-                  continue
-               for file in files:
-                  if file.endswith(".zip") or \
-                     file.endswith(".7z") or \
-                     file.endswith(".tar") or \
-                     file.endswith(".gztar") or \
-                     file.endswith(".bztar"):
-                     found = True
+            found = cls.unzip(abspath(f'{config.work}\\AIP\\{config.project_name}\\{app}'))
+            found = cls.unzip(abspath(f'{config.work}\\HL\\{config.project_name}\\{app}'))
                      
-                     full_name = abspath(f'{root.strip()}\\{file}')
-                     dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
-                     cls._log.info(f'Unzipping {full_name}')
+            #          full_name = abspath(f'{root.strip()}\\{file}')
+            #          dest = full_name.replace(f".{full_name.split('.')[-1]}",'')
+            #          cls._log.info(f'Unzipping {full_name}')
 
-                     Archive(full_name).extractall(dest,auto_create_dir=True)
+            #          Archive(full_name).extractall(dest,auto_create_dir=True)
                      
-                     remove(full_name)
+            #          remove(full_name)
 
       cls._log.info('Unzip step complete')
```

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/main.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/main.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/runArg.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/runArg.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/sendEmail.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/sendEmail.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/oneclick/setup.py` & `com.castsoftware.uc.oneclick-0.2.3.3b0/oneclick/setup.py`

 * *Files identical despite different names*

### Comparing `com.castsoftware.uc.oneclick-0.2.3.2b0/pyproject.toml` & `com.castsoftware.uc.oneclick-0.2.3.3b0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name='com.castsoftware.uc.oneclick'
 description="Assessment Generator"
-version='0.2.3.2-beta' #prod version
+version='0.2.3.3-beta' #prod version
 dependencies = [
     'pandas','python-pptx==0.6.18','python-docx',
     'argparse_formatter','django','pyunpack',
     'patool','archive',
     'com.castsoftware.uc.python.common',
     'com.castsoftware.uc.action-plan',
     'com.castsoftware.uc.arg'
```

