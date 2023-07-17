# Comparing `tmp/visionai-data-format-1.0.5.tar.gz` & `tmp/visionai-data-format-1.0.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visionai-data-format-1.0.5.tar", last modified: Mon Jul 17 04:56:44 2023, max compression
+gzip compressed data, was "visionai-data-format-1.0.5a1.tar", last modified: Fri Jul 14 04:46:09 2023, max compression
```

## Comparing `visionai-data-format-1.0.5.tar` & `visionai-data-format-1.0.5a1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.903000 visionai-data-format-1.0.5/
--rw-r--r--   0 christian   (501) staff       (20)    16299 2023-07-17 04:56:44.902811 visionai-data-format-1.0.5/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)    16069 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/README.md
--rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-17 04:56:44.903055 visionai-data-format-1.0.5/setup.cfg
--rw-r--r--   0 christian   (501) staff       (20)      753 2023-07-17 04:56:27.000000 visionai-data-format-1.0.5/setup.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.898643 visionai-data-format-1.0.5/tests/
--rw-r--r--   0 christian   (501) staff       (20)     2176 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/tests/test_schemas.py
--rw-r--r--   0 christian   (501) staff       (20)     4731 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/tests/test_validators.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.899465 visionai-data-format-1.0.5/visionai_data_format/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     1400 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/bdd_to_vai.py
--rw-r--r--   0 christian   (501) staff       (20)     7775 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/coco_to_vai.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.901172 visionai-data-format-1.0.5/visionai_data_format/schemas/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)     2551 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/bdd_schema.py
--rw-r--r--   0 christian   (501) staff       (20)      679 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/coco_schema.py
--rw-r--r--   0 christian   (501) staff       (20)     1657 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/common.py
--rw-r--r--   0 christian   (501) staff       (20)      994 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/ontology.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.901437 visionai-data-format-1.0.5/visionai_data_format/schemas/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)    40508 2023-07-17 04:56:27.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/utils/validators.py
--rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/schemas/visionai_schema.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.902590 visionai-data-format-1.0.5/visionai_data_format/utils/
--rw-r--r--   0 christian   (501) staff       (20)        0 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/__init__.py
--rw-r--r--   0 christian   (501) staff       (20)      494 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/calculation.py
--rw-r--r--   0 christian   (501) staff       (20)    10506 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/checker.py
--rw-r--r--   0 christian   (501) staff       (20)      761 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/classes.py
--rw-r--r--   0 christian   (501) staff       (20)      335 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/common.py
--rw-r--r--   0 christian   (501) staff       (20)     7898 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/converter.py
--rw-r--r--   0 christian   (501) staff       (20)     4059 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/resize.py
--rw-r--r--   0 christian   (501) staff       (20)     1991 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/utils/validator.py
--rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/vai_to_bdd.py
--rw-r--r--   0 christian   (501) staff       (20)     6237 2023-07-17 04:56:18.000000 visionai-data-format-1.0.5/visionai_data_format/vai_to_coco.py
-drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-17 04:56:44.900318 visionai-data-format-1.0.5/visionai_data_format.egg-info/
--rw-r--r--   0 christian   (501) staff       (20)    16299 2023-07-17 04:56:44.000000 visionai-data-format-1.0.5/visionai_data_format.egg-info/PKG-INFO
--rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-17 04:56:44.000000 visionai-data-format-1.0.5/visionai_data_format.egg-info/SOURCES.txt
--rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-17 04:56:44.000000 visionai-data-format-1.0.5/visionai_data_format.egg-info/dependency_links.txt
--rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-17 04:56:44.000000 visionai-data-format-1.0.5/visionai_data_format.egg-info/requires.txt
--rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-17 04:56:44.000000 visionai-data-format-1.0.5/visionai_data_format.egg-info/top_level.txt
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.573661 visionai-data-format-1.0.5a1/
+-rw-r--r--   0 christian   (501) staff       (20)    16301 2023-07-14 04:46:09.573446 visionai-data-format-1.0.5a1/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)    16069 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/README.md
+-rw-r--r--   0 christian   (501) staff       (20)       38 2023-07-14 04:46:09.573712 visionai-data-format-1.0.5a1/setup.cfg
+-rw-r--r--   0 christian   (501) staff       (20)      755 2023-07-14 04:45:38.000000 visionai-data-format-1.0.5a1/setup.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.566645 visionai-data-format-1.0.5a1/tests/
+-rw-r--r--   0 christian   (501) staff       (20)     2176 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/tests/test_schemas.py
+-rw-r--r--   0 christian   (501) staff       (20)     4731 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/tests/test_validators.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.568143 visionai-data-format-1.0.5a1/visionai_data_format/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     1400 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/bdd_to_vai.py
+-rw-r--r--   0 christian   (501) staff       (20)     7775 2023-05-19 03:23:30.000000 visionai-data-format-1.0.5a1/visionai_data_format/coco_to_vai.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.570572 visionai-data-format-1.0.5a1/visionai_data_format/schemas/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)     2551 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/bdd_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)      679 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/coco_schema.py
+-rw-r--r--   0 christian   (501) staff       (20)     1657 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/common.py
+-rw-r--r--   0 christian   (501) staff       (20)      994 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/ontology.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.571120 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)    39993 2023-07-14 04:34:28.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/validators.py
+-rw-r--r--   0 christian   (501) staff       (20)    27992 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/schemas/visionai_schema.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.573153 visionai-data-format-1.0.5a1/visionai_data_format/utils/
+-rw-r--r--   0 christian   (501) staff       (20)        0 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/__init__.py
+-rw-r--r--   0 christian   (501) staff       (20)      494 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/calculation.py
+-rw-r--r--   0 christian   (501) staff       (20)    10506 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/checker.py
+-rw-r--r--   0 christian   (501) staff       (20)      761 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/classes.py
+-rw-r--r--   0 christian   (501) staff       (20)      335 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/common.py
+-rw-r--r--   0 christian   (501) staff       (20)     7898 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/converter.py
+-rw-r--r--   0 christian   (501) staff       (20)     4059 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/resize.py
+-rw-r--r--   0 christian   (501) staff       (20)     1991 2023-05-18 02:48:45.000000 visionai-data-format-1.0.5a1/visionai_data_format/utils/validator.py
+-rw-r--r--   0 christian   (501) staff       (20)     2308 2023-07-10 09:14:49.000000 visionai-data-format-1.0.5a1/visionai_data_format/vai_to_bdd.py
+-rw-r--r--   0 christian   (501) staff       (20)     6237 2023-05-18 02:48:43.000000 visionai-data-format-1.0.5a1/visionai_data_format/vai_to_coco.py
+drwxr-xr-x   0 christian   (501) staff       (20)        0 2023-07-14 04:46:09.569285 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/
+-rw-r--r--   0 christian   (501) staff       (20)    16301 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/PKG-INFO
+-rw-r--r--   0 christian   (501) staff       (20)     1122 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/SOURCES.txt
+-rw-r--r--   0 christian   (501) staff       (20)        1 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/dependency_links.txt
+-rw-r--r--   0 christian   (501) staff       (20)       45 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/requires.txt
+-rw-r--r--   0 christian   (501) staff       (20)       21 2023-07-14 04:46:09.000000 visionai-data-format-1.0.5a1/visionai_data_format.egg-info/top_level.txt
```

### Comparing `visionai-data-format-1.0.5/PKG-INFO` & `visionai-data-format-1.0.5a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: visionai-data-format
-Version: 1.0.5
-Summary: converter tool for visionai format
-Home-page: 
-Author: LinkerVision
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Provides-Extra: test
-
 # visionai-data-format
 
 `VisionAI` format is Dataverse["url"] standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
```

### Comparing `visionai-data-format-1.0.5/README.md` & `visionai-data-format-1.0.5a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: visionai-data-format
+Version: 1.0.5a1
+Summary: converter tool for visionai format
+Home-page: 
+Author: LinkerVision
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Provides-Extra: test
+
 # visionai-data-format
 
 `VisionAI` format is Dataverse["url"] standardized annotation format to label objects and sequences in the context of Autonomous Driving System(ADS). `VisionAI` provides consistent and effective driving environment description and categorization in the real-world case.
 
 This tool provides validator of `VisionAI` format schema. Currently, the library supports:
   - Validate created `VisionAI` data format
   - Validate `VisionAI` data attributes with given `Ontology` information.
```

### Comparing `visionai-data-format-1.0.5/setup.py` & `visionai-data-format-1.0.5a1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 AUTHOR = "LinkerVision"
 PACKAGE_NAME = "visionai-data-format"
-PACKAGE_VERSION = "1.0.5"
+PACKAGE_VERSION = "1.0.5a1"
 DESC = "converter tool for visionai format"
 REQUIRED = ["pydantic==1.*"]
 REQUIRES_PYTHON = ">=3.7, <4"
 EXTRAS = {
     "test": [
         "pytest",
         "mock",
```

### Comparing `visionai-data-format-1.0.5/tests/test_schemas.py` & `visionai-data-format-1.0.5a1/tests/test_schemas.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/tests/test_validators.py` & `visionai-data-format-1.0.5a1/tests/test_validators.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/bdd_to_vai.py` & `visionai-data-format-1.0.5a1/visionai_data_format/bdd_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/coco_to_vai.py` & `visionai-data-format-1.0.5a1/visionai_data_format/coco_to_vai.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/bdd_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/bdd_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/coco_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/coco_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/common.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/common.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/ontology.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/ontology.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/utils/validators.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/utils/validators.py`

 * *Files 1% similar despite different names*

```diff
@@ -725,49 +725,33 @@
                 )
 
     if msg:
         return False, msg
     return True, ""
 
 
-def generate_missing_attributes_error_message(
-    extra_attribute_names: Set[str],
-    missing_attribute_names: Set[str],
+def gen_missing_attributes_error_message(
+    extra_attributes_name: Set[str],
+    missing_attributes_name: Set[str],
     dynamic_attrs: dict,
 ) -> str:
-    """Generate error messages of extra or missing attributes from existing dynamic attributes
-
-    Parameters
-    ----------
-    extra_attribute_names : Set[str]
-        names of extra attributes, attributes that don't exist under visionai objects/contexts
-    missing_attribute_names : Set[str]
-        names of missing attributes, attributes that don't used under visionai frames
-    dynamic_attrs : dict
-        dynamic attributes data
-
-    Returns
-    -------
-    str
-        error message
-    """
     msg = ""
-    if extra_attribute_names:
+    if extra_attributes_name:
         msg += "Extra attributes from data pointers : \n"
-        for attr_name in extra_attribute_names:
+        for attr_name in extra_attributes_name:
             if attr_name in dynamic_attrs:
                 msg += (
                     f"{attr_name} with frames {list(dynamic_attrs[attr_name].keys())}\n"
                 )
             else:
                 msg += f"{attr_name} \n"
 
-    if missing_attribute_names:
-        msg += "Missing attributes from data pointers : \n"
-        for attr_name in missing_attribute_names:
+    if missing_attributes_name:
+        msg += "Missing attributes from data pointers : "
+        for attr_name in missing_attributes_name:
             if attr_name in dynamic_attrs:
                 msg += (
                     f"{attr_name} with frames {list(dynamic_attrs[attr_name].keys())}\n"
                 )
             else:
                 msg += f"{attr_name} \n"
     return msg
@@ -820,15 +804,15 @@
     )
 
     # validate if combinations of static and dynamic equals to data pointers
     combination_attrs = static_attrs_keys | dynamic_attrs_keys
     if combination_attrs ^ data_pointers_keys:
         extra_attributes_name: Set[str] = combination_attrs - data_pointers_keys
         missing_attributes_name: Set[str] = data_pointers_keys - combination_attrs
-        msg: str = generate_missing_attributes_error_message(
+        msg: str = gen_missing_attributes_error_message(
             extra_attributes_name=extra_attributes_name,
             missing_attributes_name=missing_attributes_name,
             dynamic_attrs=dynamic_attrs,
         )
 
         return False, msg
```

### Comparing `visionai-data-format-1.0.5/visionai_data_format/schemas/visionai_schema.py` & `visionai-data-format-1.0.5a1/visionai_data_format/schemas/visionai_schema.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/utils/checker.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/checker.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/utils/classes.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/classes.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/utils/converter.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/converter.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/utils/resize.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/resize.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/utils/validator.py` & `visionai-data-format-1.0.5a1/visionai_data_format/utils/validator.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/vai_to_bdd.py` & `visionai-data-format-1.0.5a1/visionai_data_format/vai_to_bdd.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format/vai_to_coco.py` & `visionai-data-format-1.0.5a1/visionai_data_format/vai_to_coco.py`

 * *Files identical despite different names*

### Comparing `visionai-data-format-1.0.5/visionai_data_format.egg-info/PKG-INFO` & `visionai-data-format-1.0.5a1/visionai_data_format.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visionai-data-format
-Version: 1.0.5
+Version: 1.0.5a1
 Summary: converter tool for visionai format
 Home-page: 
 Author: LinkerVision
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 Provides-Extra: test
```

### Comparing `visionai-data-format-1.0.5/visionai_data_format.egg-info/SOURCES.txt` & `visionai-data-format-1.0.5a1/visionai_data_format.egg-info/SOURCES.txt`

 * *Files identical despite different names*

