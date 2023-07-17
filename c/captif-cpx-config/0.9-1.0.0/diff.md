# Comparing `tmp/captif_cpx_config-0.9.tar.gz` & `tmp/captif_cpx_config-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.9.tar", max compression
+gzip compressed data, was "captif_cpx_config-1.0.0.tar", max compression
```

## Comparing `captif_cpx_config-0.9.tar` & `captif_cpx_config-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/LICENSE
--rw-r--r--   0        0        0       19 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/README.md
--rw-r--r--   0        0        0       44 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     4335 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      523 2023-06-23 02:06:00.030631 captif_cpx_config-0.9/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-17 09:50:11.936602 captif_cpx_config-1.0.0/LICENSE
+-rw-r--r--   0        0        0       19 2023-07-17 09:50:11.936602 captif_cpx_config-1.0.0/README.md
+-rw-r--r--   0        0        0       46 2023-07-17 09:50:11.936602 captif_cpx_config-1.0.0/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     4562 2023-07-17 09:50:11.936602 captif_cpx_config-1.0.0/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      525 2023-07-17 09:50:11.936602 captif_cpx_config-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 captif_cpx_config-1.0.0/PKG-INFO
```

### Comparing `captif_cpx_config-0.9/LICENSE` & `captif_cpx_config-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.9/captif_cpx_config/metadata.py` & `captif_cpx_config-1.0.0/captif_cpx_config/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,14 +115,21 @@
             "to convert the data back into volts."
         ),
     )
     notes: Optional[str] = Field(
         default=None,
         description="any additional notes",
     )
+    measurement_group_date: Optional[date_] = Field(
+        default=None,
+        description=(
+            "date used for grouping repeat runs performed across difference "
+            "measurement sessions"
+        ),
+    )
     gis_check_complete: Optional[bool] = Field(
         default=False,
         description="tracks whether the manual GIS check has been done",
     )
 
     wheel_bay_details: list["WheelBayDetails"] = []
```

### Comparing `captif_cpx_config-0.9/pyproject.toml` & `captif_cpx_config-1.0.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-config"
-version = "0.9"
+version = "1.0.0"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "captif_cpx_config"}]
 
 [tool.poetry.dependencies]
@@ -14,12 +14,12 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.1.0"
 pytest-randomly = "^3.12.0"
 black = "^23.3.0"
 flake8 = "^6.0.0"
-captif-cpx-db = ">=0.10"
+captif-cpx-db = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `captif_cpx_config-0.9/PKG-INFO` & `captif_cpx_config-1.0.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.9
+Version: 1.0.0
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

