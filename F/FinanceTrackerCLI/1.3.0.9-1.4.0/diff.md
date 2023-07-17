# Comparing `tmp/FinanceTrackerCLI-1.3.0.9.tar.gz` & `tmp/FinanceTrackerCLI-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinanceTrackerCLI-1.3.0.9.tar", last modified: Sun Jul 16 18:28:13 2023, max compression
+gzip compressed data, was "FinanceTrackerCLI-1.4.0.tar", last modified: Mon Jul 17 05:14:14 2023, max compression
```

## Comparing `FinanceTrackerCLI-1.3.0.9.tar` & `FinanceTrackerCLI-1.4.0.tar`

### file list

```diff
@@ -1,24 +1,27 @@
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.617054 FinanceTrackerCLI-1.3.0.9/
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.9/LICENSE
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:28:13.616950 FinanceTrackerCLI-1.3.0.9/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.9/README.md
--rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.9/pyproject.toml
--rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 18:28:13.617089 FinanceTrackerCLI-1.3.0.9/setup.cfg
--rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 18:28:09.000000 FinanceTrackerCLI-1.3.0.9/setup.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.614808 FinanceTrackerCLI-1.3.0.9/src/
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.616197 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/
--rw-r--r--   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:03:57.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3103 2023-07-16 18:27:06.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/finance_tracker.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/grouped_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/input_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/local_convertor.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/search_by_month_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/show_all_delete_string.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/terminal_name.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/text_prompts.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.616794 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      626 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/SOURCES.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/dependency_links.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/requires.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/top_level.txt
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-17 05:14:14.423135 FinanceTrackerCLI-1.4.0/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.4.0/LICENSE
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1032 2023-07-17 05:14:14.422983 FinanceTrackerCLI-1.4.0/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      564 2023-07-17 04:34:47.000000 FinanceTrackerCLI-1.4.0/README.md
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      299 2023-07-17 05:00:38.000000 FinanceTrackerCLI-1.4.0/pyproject.toml
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-17 05:14:14.423184 FinanceTrackerCLI-1.4.0/setup.cfg
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      733 2023-07-17 05:00:38.000000 FinanceTrackerCLI-1.4.0/setup.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-17 05:14:14.419220 FinanceTrackerCLI-1.4.0/src/
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-17 05:14:14.419932 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:03:57.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3145 2023-07-16 18:33:17.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/finance_tracker.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-17 05:14:14.422655 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      209 2023-07-16 18:36:04.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/grouped_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/input_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/local_convertor.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/search_by_month_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/show_all_delete_string.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/terminal_name.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     2534 2023-07-17 03:59:48.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/text_prompts.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-17 05:14:14.420682 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1032 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      756 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       59 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/entry_points.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/requires.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-17 05:14:14.000000 FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/top_level.txt
```

### Comparing `FinanceTrackerCLI-1.3.0.9/LICENSE` & `FinanceTrackerCLI-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/setup.py` & `FinanceTrackerCLI-1.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FinanceTrackerCLI',
-    version='1.3.0.9',
+    version='1.4.0',
     author='Vladimir Kobranov',
     author_email='josephclturok@gmail.com',
     description='Finance tracker CLI app',
     long_description=open('README.md').read(),
+    include_package_data=True,
     long_description_content_type='text/markdown',
     url='https://github.com/VladimirKobranov/FinanceTrackerCLI',
     classifiers=[
         'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
         'Operating System :: MacOS',
     ],
```

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/finance_tracker.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/finance_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import json
 import os
 import os.path
 
-from grouped_data import grouped_final
-from input_data import input_string
-from local_convertor import local_convertor
-from search_by_month_data import search_by_month
-from show_all_delete_string import delete_string
-from terminal_name import set_terminal_title, get_terminal_title
-from text_prompts import mainMessage, helpMessage, creditsMessage, \
+from logic.grouped_data import grouped_final
+from logic.input_data import input_string
+from logic.local_convertor import local_convertor
+from logic.search_by_month_data import search_by_month
+from logic.show_all_delete_string import delete_string
+from logic.terminal_name import set_terminal_title, get_terminal_title
+from logic.text_prompts import mainMessage, helpMessage, creditsMessage, \
     availableCurrencies, currency_list
 
 new_title = 'Finance tracker'
 original_title = get_terminal_title()
 set_terminal_title(new_title)
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
```

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/grouped_data.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/grouped_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/input_data.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/input_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/local_convertor.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/local_convertor.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/search_by_month_data.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/search_by_month_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/show_all_delete_string.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/show_all_delete_string.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/terminal_name.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/terminal_name.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/text_prompts.py` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI/logic/text_prompts.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ------------------------------------------
   Expense tracker python CLI app made by
             Vladimir Kobranov
             
     https://github.com/VladimirKobranov
 ------------------------------------------
         Release Date: 2023-07-10
-          Version Number: 1.3.0.0
+          Version Number: 1.4.0
              Release Notes:
 --added conversion at Forex Exchange Market
 --added local currency convertor
 --added input checks
 --added program name title
 --added delete string functionality 
 --overhaul, fixes
```

### Comparing `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/SOURCES.txt` & `FinanceTrackerCLI-1.4.0/src/FinanceTrackerCLI.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/FinanceTrackerCLI/__init__.py
 src/FinanceTrackerCLI/finance_tracker.py
-src/FinanceTrackerCLI/grouped_data.py
-src/FinanceTrackerCLI/input_data.py
-src/FinanceTrackerCLI/local_convertor.py
-src/FinanceTrackerCLI/search_by_month_data.py
-src/FinanceTrackerCLI/show_all_delete_string.py
-src/FinanceTrackerCLI/terminal_name.py
-src/FinanceTrackerCLI/text_prompts.py
 src/FinanceTrackerCLI.egg-info/PKG-INFO
 src/FinanceTrackerCLI.egg-info/SOURCES.txt
 src/FinanceTrackerCLI.egg-info/dependency_links.txt
+src/FinanceTrackerCLI.egg-info/entry_points.txt
 src/FinanceTrackerCLI.egg-info/requires.txt
-src/FinanceTrackerCLI.egg-info/top_level.txt
+src/FinanceTrackerCLI.egg-info/top_level.txt
+src/FinanceTrackerCLI/logic/__init__.py
+src/FinanceTrackerCLI/logic/grouped_data.py
+src/FinanceTrackerCLI/logic/input_data.py
+src/FinanceTrackerCLI/logic/local_convertor.py
+src/FinanceTrackerCLI/logic/search_by_month_data.py
+src/FinanceTrackerCLI/logic/show_all_delete_string.py
+src/FinanceTrackerCLI/logic/terminal_name.py
+src/FinanceTrackerCLI/logic/text_prompts.py
```

