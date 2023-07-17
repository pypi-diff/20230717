# Comparing `tmp/pquisby-0.0.8.tar.gz` & `tmp/pquisby-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pquisby-0.0.8.tar", last modified: Thu Jun 22 11:39:52 2023, max compression
+gzip compressed data, was "pquisby-0.0.9.tar", last modified: Mon Jul 17 08:24:36 2023, max compression
```

## Comparing `pquisby-0.0.8.tar` & `pquisby-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.828084 pquisby-0.0.8/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 pquisby-0.0.8/LICENSE
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 pquisby-0.0.8/MANIFEST.in
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-22 11:39:52.828084 pquisby-0.0.8/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 pquisby-0.0.8/README.md
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 pquisby-0.0.8/requirements.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-06-22 11:39:52.828084 pquisby-0.0.8/setup.cfg
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      950 2023-06-22 11:39:52.000000 pquisby-0.0.8/setup.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.823084 pquisby-0.0.8/src/
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.824084 pquisby-0.0.8/src/pquisby/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.825084 pquisby-0.0.8/src/pquisby/command/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/command/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/command/compare_benchmark.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/command/main.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/command/process_benchmark.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.826084 pquisby-0.0.8/src/pquisby/lib/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.826084 pquisby-0.0.8/src/pquisby/lib/benchmarks/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/benchmarks/__init__.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.827084 pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/comparison.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/graph.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5430 2023-06-22 10:27:11.000000 pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/uperf.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/compare_sheets.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.827084 pquisby-0.0.8/src/pquisby/lib/credentials/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/credentials/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/credentials/creds.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2704 2023-06-22 11:39:43.000000 pquisby-0.0.8/src/pquisby/lib/post_processing.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.827084 pquisby-0.0.8/src/pquisby/lib/pricing/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/pricing/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/pricing/cloud_pricing.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/process_result.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.827084 pquisby-0.0.8/src/pquisby/lib/sheet/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/sheet/__init__.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/sheet/sheet_util.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/sheet/sheetapi.py
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 pquisby-0.0.8/src/pquisby/lib/util.py
-drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-06-22 11:39:52.825084 pquisby-0.0.8/src/pquisby.egg-info/
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/PKG-INFO
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1061 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/SOURCES.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/dependency_links.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/entry_points.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/requires.txt
--rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-06-22 11:39:52.000000 pquisby-0.0.8/src/pquisby.egg-info/top_level.txt
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.284159 pquisby-0.0.9/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)    35149 2023-06-13 14:39:53.000000 pquisby-0.0.9/LICENSE
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       39 2023-06-13 14:40:39.000000 pquisby-0.0.9/MANIFEST.in
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-07-17 08:24:36.284159 pquisby-0.0.9/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      940 2023-06-13 14:40:39.000000 pquisby-0.0.9/README.md
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3903 2023-06-13 14:40:39.000000 pquisby-0.0.9/requirements.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       38 2023-07-17 08:24:36.284159 pquisby-0.0.9/setup.cfg
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      950 2023-07-17 08:24:35.000000 pquisby-0.0.9/setup.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.278159 pquisby-0.0.9/src/
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.279159 pquisby-0.0.9/src/pquisby/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.281159 pquisby-0.0.9/src/pquisby/command/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/command/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      488 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/command/compare_benchmark.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      300 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/command/main.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     3382 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/command/process_benchmark.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.282159 pquisby-0.0.9/src/pquisby/lib/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.282159 pquisby-0.0.9/src/pquisby/lib/benchmarks/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/benchmarks/__init__.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.283159 pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1214 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/comparison.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5175 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/graph.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5430 2023-06-22 10:27:11.000000 pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/uperf.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1655 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/compare_sheets.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.283159 pquisby-0.0.9/src/pquisby/lib/credentials/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/credentials/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1119 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/credentials/creds.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2769 2023-07-17 08:20:47.000000 pquisby-0.0.9/src/pquisby/lib/post_processing.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.283159 pquisby-0.0.9/src/pquisby/lib/pricing/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/pricing/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     4728 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/pricing/cloud_pricing.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     6775 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/process_result.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.284159 pquisby-0.0.9/src/pquisby/lib/sheet/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        0 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/sheet/__init__.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     5692 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/sheet/sheet_util.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)      945 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/sheet/sheetapi.py
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     2370 2023-06-13 14:40:39.000000 pquisby-0.0.9/src/pquisby/lib/util.py
+drwxr-xr-x   0 siddardh  (1000) siddardh  (1000)        0 2023-07-17 08:24:36.280159 pquisby-0.0.9/src/pquisby.egg-info/
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1265 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/PKG-INFO
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1061 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/SOURCES.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        1 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/dependency_links.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)       54 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/entry_points.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)     1990 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/requires.txt
+-rw-r--r--   0 siddardh  (1000) siddardh  (1000)        8 2023-07-17 08:24:36.000000 pquisby-0.0.9/src/pquisby.egg-info/top_level.txt
```

### Comparing `pquisby-0.0.8/LICENSE` & `pquisby-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/PKG-INFO` & `pquisby-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.8/README.md` & `pquisby-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/requirements.txt` & `pquisby-0.0.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/setup.py` & `pquisby-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 README = (HERE / "README.md").read_text()
 
 # The text of the README file
 REQUIRE = (HERE / "requirements.txt").read_text()
 
 setup(
     name="pquisby",
-    version="0.0.8",
+    version="0.0.9",
     description="Quisby is a data processing and visualization tool for benchmark testing.",
     url = 'https://github.com/sousinha1997/Quisby',
     author = 'Soumya Sinha',
     author_email = 'sinhasoumya97@gmail.com',
     license = 'GPL v3.0',
     packages=find_packages("src"),
     package_dir={"":"src"},
```

### Comparing `pquisby-0.0.8/src/pquisby/command/process_benchmark.py` & `pquisby-0.0.9/src/pquisby/command/process_benchmark.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/comparison.py` & `pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/comparison.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/graph.py` & `pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/graph.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/benchmarks/uperf/uperf.py` & `pquisby-0.0.9/src/pquisby/lib/benchmarks/uperf/uperf.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/compare_sheets.py` & `pquisby-0.0.9/src/pquisby/lib/compare_sheets.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/credentials/creds.py` & `pquisby-0.0.9/src/pquisby/lib/credentials/creds.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/post_processing.py` & `pquisby-0.0.9/src/pquisby/lib/post_processing.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,32 +47,34 @@
                 "exception": str(exc),
                 "exception_type": exception_type,
             }
         return {"status": "success", "csv_data": ret_val, "json_data": json_data}
 
     def compare_csv_to_json(self, benchmark_name, input_type, data_stream):
         result_json = {}
-        comp_dataset_name = ""
+        comp_dataset_name = "result"
         flag = 0
         for dataset_name, data in data_stream.items():
-            comp_dataset_name = comp_dataset_name + "&" + dataset_name
-            json_res = self.extract_data(benchmark_name, dataset_name, input_type, data)
+            json_res = self.extract_data(self,benchmark_name, dataset_name, input_type, data)
             if json_res["status"] != "success":
                 return json_res
 
             if json_res["json_data"]:
                 json_data = json_res["json_data"]
             if flag == 0:
+                comp_dataset_name = dataset_name
                 result_json = json_data
                 flag = flag + 1
             else:
+                comp_dataset_name = comp_dataset_name + "&" + dataset_name
                 for i in result_json["data"]:
                     metric_unit = i["metrics_unit"]
                     test_name = i["test_name"]
                     for j in json_data["data"]:
                         if (
                             metric_unit == j["metrics_unit"]
                             and test_name == j["test_name"]
                         ):
                             i["instances"].extend(j["instances"])
         result_json["dataset_name"] = comp_dataset_name
         return {"status": "success", "json_data": result_json}
+
```

### Comparing `pquisby-0.0.8/src/pquisby/lib/pricing/cloud_pricing.py` & `pquisby-0.0.9/src/pquisby/lib/pricing/cloud_pricing.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/process_result.py` & `pquisby-0.0.9/src/pquisby/lib/process_result.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/sheet/sheet_util.py` & `pquisby-0.0.9/src/pquisby/lib/sheet/sheet_util.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/sheet/sheetapi.py` & `pquisby-0.0.9/src/pquisby/lib/sheet/sheetapi.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby/lib/util.py` & `pquisby-0.0.9/src/pquisby/lib/util.py`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby.egg-info/PKG-INFO` & `pquisby-0.0.9/src/pquisby.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pquisby
-Version: 0.0.8
+Version: 0.0.9
 Summary: Quisby is a data processing and visualization tool for benchmark testing.
 Home-page: https://github.com/sousinha1997/Quisby
 Author: Soumya Sinha
 Author-email: sinhasoumya97@gmail.com
 License: GPL v3.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pquisby-0.0.8/src/pquisby.egg-info/SOURCES.txt` & `pquisby-0.0.9/src/pquisby.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pquisby-0.0.8/src/pquisby.egg-info/requires.txt` & `pquisby-0.0.9/src/pquisby.egg-info/requires.txt`

 * *Files identical despite different names*

