# Comparing `tmp/FinanceTrackerCLI-1.3.0.8.tar.gz` & `tmp/FinanceTrackerCLI-1.3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FinanceTrackerCLI-1.3.0.8.tar", last modified: Sun Jul 16 18:23:46 2023, max compression
+gzip compressed data, was "FinanceTrackerCLI-1.3.0.9.tar", last modified: Sun Jul 16 18:28:13 2023, max compression
```

## Comparing `FinanceTrackerCLI-1.3.0.8.tar` & `FinanceTrackerCLI-1.3.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:23:46.145181 FinanceTrackerCLI-1.3.0.8/
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.8/LICENSE
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:23:46.145076 FinanceTrackerCLI-1.3.0.8/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.8/README.md
--rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.8/pyproject.toml
--rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 18:23:46.145212 FinanceTrackerCLI-1.3.0.8/setup.cfg
--rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 18:23:41.000000 FinanceTrackerCLI-1.3.0.8/setup.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:23:46.142969 FinanceTrackerCLI-1.3.0.8/src/
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:23:46.144365 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/
--rw-r--r--   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:03:57.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/__init__.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3108 2023-07-16 18:23:41.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/finance_tracker.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/grouped_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/input_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/local_convertor.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/search_by_month_data.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/show_all_delete_string.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/terminal_name.py
--rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/text_prompts.py
-drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:23:46.144932 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/
--rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:23:46.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/PKG-INFO
--rw-r--r--   0 vladkobranov   (501) staff       (20)      626 2023-07-16 18:23:46.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/SOURCES.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 18:23:46.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/dependency_links.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:23:46.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/requires.txt
--rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:23:46.000000 FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/top_level.txt
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.617054 FinanceTrackerCLI-1.3.0.9/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1083 2023-07-16 13:30:44.000000 FinanceTrackerCLI-1.3.0.9/LICENSE
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:28:13.616950 FinanceTrackerCLI-1.3.0.9/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      292 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.9/README.md
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      124 2023-07-16 16:47:26.000000 FinanceTrackerCLI-1.3.0.9/pyproject.toml
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       38 2023-07-16 18:28:13.617089 FinanceTrackerCLI-1.3.0.9/setup.cfg
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      704 2023-07-16 18:28:09.000000 FinanceTrackerCLI-1.3.0.9/setup.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.614808 FinanceTrackerCLI-1.3.0.9/src/
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.616197 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:03:57.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/__init__.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3103 2023-07-16 18:27:06.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/finance_tracker.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     3273 2023-07-14 16:14:43.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/grouped_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1318 2023-07-14 16:47:58.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/input_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     1953 2023-07-14 16:18:24.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/local_convertor.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      885 2023-07-14 16:21:17.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/search_by_month_data.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      777 2023-07-14 15:39:26.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/show_all_delete_string.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      661 2023-07-12 16:42:26.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/terminal_name.py
+-rw-r--r--   0 vladkobranov   (501) staff       (20)     2536 2023-07-16 17:20:08.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/text_prompts.py
+drwxr-xr-x   0 vladkobranov   (501) staff       (20)        0 2023-07-16 18:28:13.616794 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      745 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/PKG-INFO
+-rw-r--r--   0 vladkobranov   (501) staff       (20)      626 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/SOURCES.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)        1 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/dependency_links.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/requires.txt
+-rw-r--r--   0 vladkobranov   (501) staff       (20)       18 2023-07-16 18:28:13.000000 FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/top_level.txt
```

### Comparing `FinanceTrackerCLI-1.3.0.8/LICENSE` & `FinanceTrackerCLI-1.3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/PKG-INFO` & `FinanceTrackerCLI-1.3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.8
+Version: 1.3.0.9
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.8/setup.py` & `FinanceTrackerCLI-1.3.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='FinanceTrackerCLI',
-    version='1.3.0.8',
+    version='1.3.0.9',
     author='Vladimir Kobranov',
     author_email='josephclturok@gmail.com',
     description='Finance tracker CLI app',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/VladimirKobranov/FinanceTrackerCLI',
     classifiers=[
```

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/finance_tracker.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/finance_tracker.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     availableCurrencies, currency_list
 
 new_title = 'Finance tracker'
 original_title = get_terminal_title()
 set_terminal_title(new_title)
 
 current_dir = os.path.dirname(os.path.abspath(__file__))
-file_path = os.path.join(current_dir, "data/FinanceList.json")
+file_path = os.path.join(current_dir, "FinanceList.json")
 
 
 def main():
     try:
         with open(file_path, "r") as infile:
             finances_list = json.load(infile)
     except FileNotFoundError:
```

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/grouped_data.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/grouped_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/input_data.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/input_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/local_convertor.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/local_convertor.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/search_by_month_data.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/search_by_month_data.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/show_all_delete_string.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/show_all_delete_string.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/terminal_name.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/terminal_name.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI/text_prompts.py` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI/text_prompts.py`

 * *Files identical despite different names*

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/PKG-INFO` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FinanceTrackerCLI
-Version: 1.3.0.8
+Version: 1.3.0.9
 Summary: Finance tracker CLI app
 Home-page: https://github.com/VladimirKobranov/FinanceTrackerCLI
 Author: Vladimir Kobranov
 Author-email: josephclturok@gmail.com
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
```

### Comparing `FinanceTrackerCLI-1.3.0.8/src/FinanceTrackerCLI.egg-info/SOURCES.txt` & `FinanceTrackerCLI-1.3.0.9/src/FinanceTrackerCLI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

