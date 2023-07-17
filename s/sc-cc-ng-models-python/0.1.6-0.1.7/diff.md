# Comparing `tmp/sc_cc_ng_models_python-0.1.6.tar.gz` & `tmp/sc_cc_ng_models_python-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc_cc_ng_models_python-0.1.6.tar", max compression
+gzip compressed data, was "sc_cc_ng_models_python-0.1.7.tar", max compression
```

## Comparing `sc_cc_ng_models_python-0.1.6.tar` & `sc_cc_ng_models_python-0.1.7.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.6/README.md
--rw-r--r--   0        0        0      425 2023-07-06 06:35:12.979496 sc_cc_ng_models_python-0.1.6/pyproject.toml
--rw-r--r--   0        0        0    10644 2023-07-06 21:56:38.261018 sc_cc_ng_models_python-0.1.6/sc_cc_ng_models_python/__init__.py
--rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      576 2023-06-26 14:02:21.217632 sc_cc_ng_models_python-0.1.7/README.md
+-rw-r--r--   0        0        0      425 2023-07-17 11:39:22.583170 sc_cc_ng_models_python-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0    10805 2023-07-17 11:39:12.751111 sc_cc_ng_models_python-0.1.7/sc_cc_ng_models_python/__init__.py
+-rw-r--r--   0        0        0      979 1970-01-01 00:00:00.000000 sc_cc_ng_models_python-0.1.7/PKG-INFO
```

### Comparing `sc_cc_ng_models_python-0.1.6/README.md` & `sc_cc_ng_models_python-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sc_cc_ng_models_python-0.1.6/sc_cc_ng_models_python/__init__.py` & `sc_cc_ng_models_python-0.1.7/sc_cc_ng_models_python/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,17 @@
 	MODEL = "MODEL"
 	MSRP = "MSRP"
 	NAME = "NAME"
 	NOX_EMISSION = "NOX_EMISSION"
 	NOX_EMISSION_SECONDARY = "NOX_EMISSION_SECONDARY"
 	PACKAGES = "PACKAGES"
 	POWERTRAIN_TYPE = "POWERTRAIN_TYPE"
+	PROCESSED_DESCRIPTION = "PROCESSED_DESCRIPTION"
+	PROCESSED_SHORT_DESCRIPTION = "PROCESSED_SHORT_DESCRIPTION"
+	PROCESSED_DISPLAY_NAME = "PROCESSED_DISPLAY_NAME"
 	ROOF_WEIGHT = "ROOF_WEIGHT"
 	SEAT_CAPACITY = "SEAT_CAPACITY"
 	SERVING_WEIGHT = "SERVING_WEIGHT"
 	SHORT_DESCRIPTION = "SHORT_DESCRIPTION"
 	SHORT_DISPLAY_NAME = "SHORT_DISPLAY_NAME"
 	SHOULDER_ROOM_FRONT = "SHOULDER_ROOM_FRONT"
 	SHOULDER_ROOM_REAR = "SHOULDER_ROOM_REAR"
```

### Comparing `sc_cc_ng_models_python-0.1.6/PKG-INFO` & `sc_cc_ng_models_python-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sc-cc-ng-models-python
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Rikard Olsson
 Author-email: rikard@thryselius.se
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

