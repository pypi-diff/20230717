# Comparing `tmp/comet_mpm-0.4.1.tar.gz` & `tmp/comet_mpm-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "comet_mpm-0.4.1.tar", last modified: Mon Jul  3 14:16:00 2023, max compression
+gzip compressed data, was "comet_mpm-0.4.2.tar", last modified: Mon Jul 17 11:28:24 2023, max compression
```

## Comparing `comet_mpm-0.4.1.tar` & `comet_mpm-0.4.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.606959 comet_mpm-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/_json/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_json/numpy_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/batch_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9865 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/comet_mpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/data_series.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/events/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/base_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/events_from_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/label_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/events/prediction_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/logging_messages.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/optional_update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm/sender/
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/asyncio_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/sender/thread_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-03 14:15:50.000000 comet_mpm-0.4.1/src/comet_mpm/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 14:16:00.610959 comet_mpm-0.4.1/src/comet_mpm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-03 14:16:00.000000 comet_mpm-0.4.1/src/comet_mpm.egg-info/SOURCES.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.266476 comet_mpm-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.270477 comet_mpm-0.4.2/src/comet_mpm/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.270477 comet_mpm-0.4.2/src/comet_mpm/_json/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/_json/numpy_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/batch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/comet_mpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/data_series.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/src/comet_mpm/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/events/base_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2631 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/events/events_from_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/events/label_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/events/prediction_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/logging_messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/optional_update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/src/comet_mpm/sender/
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9727 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/sender/asyncio_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/sender/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8239 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/sender/thread_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-07-17 11:28:11.000000 comet_mpm-0.4.2/src/comet_mpm/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:28:24.274477 comet_mpm-0.4.2/src/comet_mpm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-17 11:28:24.000000 comet_mpm-0.4.2/src/comet_mpm.egg-info/SOURCES.txt
```

### Comparing `comet_mpm-0.4.1/MANIFEST.in` & `comet_mpm-0.4.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/PKG-INFO` & `comet_mpm-0.4.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comet_mpm
-Version: 0.4.1
+Version: 0.4.2
 Summary: Comet MPM SDK
 Home-page: https://www.comet.ml
 Author: Comet ML Inc.
 Author-email: mail@comet.ml
 License: Proprietary
 Keywords: comet_mpm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `comet_mpm-0.4.1/setup.py` & `comet_mpm-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,11 +52,11 @@
     long_description_content_type="text/markdown",
     include_package_data=True,
     keywords="comet_mpm",
     name="comet_mpm",
     packages=find_packages("src"),
     package_dir={"": "src"},
     url="https://www.comet.ml",
-    version="0.4.1",
+    version="0.4.2",
     zip_safe=False,
     license="Proprietary",
 )
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/__init__.py` & `comet_mpm-0.4.2/src/comet_mpm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,14 @@
 #  Copyright (C) 2021 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 
 __author__ = """Comet ML Inc."""
 __email__ = "mail@comet.ml"
-__version__ = "0.4.1"
+__version__ = "0.4.2"
 __all__ = ["CometMPM"]
 
 from ._logging import _setup_comet_mpm_logging
 from .comet_mpm import CometMPM
 
 _setup_comet_mpm_logging()
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/_json/__init__.py` & `comet_mpm-0.4.2/src/comet_mpm/_json/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/_json/numpy_encoder.py` & `comet_mpm-0.4.2/src/comet_mpm/_json/numpy_encoder.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/_logging.py` & `comet_mpm-0.4.2/src/comet_mpm/_logging.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/batch_utils.py` & `comet_mpm-0.4.2/src/comet_mpm/batch_utils.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/cli.py` & `comet_mpm-0.4.2/src/comet_mpm/cli.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/comet_mpm.py` & `comet_mpm-0.4.2/src/comet_mpm/comet_mpm.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,59 +101,61 @@
 
     def log_event(
         self,
         prediction_id: str,
         input_features: Optional[Dict[str, Any]] = None,
         output_value: Optional[Any] = None,
         output_probability: Optional[Any] = None,
+        timestamp: Optional[float] = None,
     ) -> Optional[Awaitable[None]]:
         """
-        Log a single event asynchronously to MPM. Events are identified by the
-        mandatory prediction_id parameter. You can send multiple events with the
-        same prediction_id, events will be merged on the backend side
-        automatically.
+        Asynchronously log a single event to MPM. Events are identified by the
+        mandatory prediction_id parameter. You can send multiple events with
+        the same prediction_id, and the events will be automatically merged
+        on the backend side.
+
         Args:
-            prediction_id: The unique prediction ID, could be provided by the
-                framework, you or a random unique value could be provided like
-                str(uuid4())
-            input_features: If provided must be a flat Dictionary where the
-                keys are the feature name and the value are native Python
-                scalars, int, floats, booleans or strings. For example:
-                `{“age”: 42, “income”: 42894.89}`
-            output_value: The prediction as a native Python scalar, int,
-                float, boolean or string.
-            output_probability: If provided, must be a float between 0 and 1
-                indicating the confidence of the model in the prediction
-        """
+            prediction_id: The unique prediction ID. It can be provided by the
+                framework, you, or a random unique value such as str(uuid4()).
+            input_features: If provided, it must be a flat dictionary where the
+                keys are the feature names, and the values are native Python
+                scalars, such as integers, floats, booleans, or strings. For
+                example: `{"age": 42, "income": 42894.89}`.
+            output_value: The prediction as a native Python scalar, such as an
+                 integer, float, boolean, or string.
+            output_probability: If provided, it must be a float between 0 and
+                 1, indicating the model's confidence in the prediction.
+            timestamp: An optional timestamp to associate with the event
+                (seconds since epoch in UTC timezone). If not provided, the
+                 current time will be used."""
         if self.disabled:
             if self._asyncio is False:
                 return None
             else:
                 return asyncio_module.sleep(0)
 
         event = PredictionEvent(
             workspace=self._settings.mpm_workspace_name,
             model_name=self._settings.mpm_model_name,
             model_version=self._settings.mpm_model_version,
             prediction_id=prediction_id,
             input_features=input_features,
             output_value=output_value,
             output_probability=output_probability,
+            timestamp=timestamp,
         )
         return self._log_event(event)
 
     def log_label(self, prediction_id: str, label: Any) -> Optional[Awaitable[None]]:
         """
         Send an MPM event containing the ground truth value for a prediction whose input and output
         features are already stored in Comet.
         Args:
-            prediction_id: The unique prediction ID, could be provided by the
-                framework, you or a random unique value could be provided like
-                str(uuid4())
-            label: the ground truth value for a prediction
+            prediction_id: The unique prediction ID
+            label: The ground truth value for the prediction
         """
         if self.disabled:
             if self._asyncio is False:
                 return None
             else:
                 return asyncio_module.sleep(0)
 
@@ -169,42 +171,44 @@
     def log_dataframe(  # type: ignore[no-untyped-def]
         self,
         dataframe,
         prediction_id_column: str,
         feature_columns: Optional[List[str]] = None,
         output_value_column: Optional[str] = None,
         output_probability_column: Optional[str] = None,
+        timestamp_column: Optional[str] = None,
     ) -> LogEventsResult:
         """
-        Log a pandas DataFrame to MPM.
-        Every row in the dataframe will be interpreted as an event to be logged.
-
-        Events are structured as described in .log_event() method, please refer to it
-        to have the full context.
+        This function logs each row of a Pandas DataFrame as an MPM event. The
+        events are structured as described in the [log_event]
+        (#cometmpmlog_event) method, so please refer to it for full context.
 
         Args:
-            dataframe: the pandas DataFrame to be logged.
-            prediction_id_column: this column should have the prediction_id
-                values for the events.
-            feature_columns: if provided, this column will be used as the
-                input_features parameter for the events.
-            output_value_column: if provided, this column will be used as the
-                output_value for the events.
-            output_probability_column: if provided, this column will be used as
-                the output_probability for the events.
+            dataframe: The Pandas DataFrame to be logged.
+            prediction_id_column: This column should contain the prediction_id values for the
+                events.
+            feature_columns: If provided, these columns will be used as the input_features parameter
+                for the events.
+            output_value_column: If provided, this column will be used as the output_value for the
+                events.
+            output_probability_column: If provided, this column will be used as the
+                output_probability for the events.
+            timestamp_column: If provided, this column will be used as the timestamp (seconds since
+                epoch start in UTC timezone) for the events.
         """
         events = events_from_dataframe.generate(
             workspace=self._settings.mpm_workspace_name,
             model_name=self._settings.mpm_model_name,
             model_version=self._settings.mpm_model_version,
             dataframe=dataframe,
             prediction_id_column=prediction_id_column,
             feature_columns=feature_columns,
             output_value_column=output_value_column,
             output_probability_column=output_probability_column,
+            timestamp_column=timestamp_column,
         )
 
         return self._log_events(events)
 
     def connect(self) -> None:
         """
         When using CometMPM in asyncio mode, this coroutine needs to be awaited
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/connection.py` & `comet_mpm-0.4.2/src/comet_mpm/connection.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/constants.py` & `comet_mpm-0.4.2/src/comet_mpm/constants.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/data_series.py` & `comet_mpm-0.4.2/src/comet_mpm/data_series.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/events/__init__.py` & `comet_mpm-0.4.2/src/comet_mpm/events/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/events/base_event.py` & `comet_mpm-0.4.2/src/comet_mpm/events/base_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,34 +10,40 @@
 #  Copyright (C) 2021-2023 Comet ML INC
 #  This file can not be copied and/or distributed without the express
 #  permission of Comet ML Inc.
 # *******************************************************
 import abc
 import calendar
 from datetime import datetime
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 from comet_mpm.constants import (
     EVENT_MODEL_NAME,
     EVENT_MODEL_VERSION,
     EVENT_PREDICTION_ID,
     EVENT_TIMESTAMP,
     EVENT_WORKSPACE_NAME,
 )
 
 
 class BaseEvent(abc.ABC):
     def __init__(
-        self, workspace: str, model_name: str, model_version: str, prediction_id: str
+        self,
+        workspace: str,
+        model_name: str,
+        model_version: str,
+        prediction_id: str,
+        timestamp: Optional[float] = None,
     ):
         self.workspace = workspace
         self.model_name = model_name
         self.model_version = model_version
         self.prediction_id = prediction_id
-        self.timestamp = local_timestamp()
+
+        self.timestamp = local_timestamp(timestamp)
 
     def create_event_dict(self) -> Dict[str, Any]:
         base_dict = {
             EVENT_MODEL_NAME: self.model_name,
             EVENT_MODEL_VERSION: self.model_version,
             EVENT_WORKSPACE_NAME: self.workspace,
             EVENT_PREDICTION_ID: self.prediction_id,
@@ -47,13 +53,18 @@
         return base_dict
 
     @abc.abstractmethod
     def _get_event_dict(self) -> Dict[str, Any]:
         ...
 
 
-def local_timestamp() -> int:
+def local_timestamp(timestamp: Optional[float] = None) -> int:
     """Return a timestamp in a format expected by the backend (milliseconds)"""
-    now = datetime.utcnow()
-    timestamp_in_seconds = calendar.timegm(now.timetuple()) + (now.microsecond / 1e6)
+    if timestamp is None:
+        now = datetime.utcnow()
+        timestamp_in_seconds = calendar.timegm(now.timetuple()) + (
+            now.microsecond / 1e6
+        )
+    else:
+        timestamp_in_seconds = timestamp
     timestamp_in_milliseconds = int(timestamp_in_seconds * 1000)
     return timestamp_in_milliseconds
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/events/events_from_dataframe.py` & `comet_mpm-0.4.2/src/comet_mpm/events/events_from_dataframe.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,48 +21,63 @@
     model_name: str,
     model_version: str,
     dataframe,
     prediction_id_column: str,
     feature_columns: Optional[List[str]] = None,
     output_value_column: Optional[str] = None,
     output_probability_column: Optional[str] = None,
+    timestamp_column: Optional[str] = None,
 ):
     return (
         _event(
             workspace=workspace,
             model_name=model_name,
             model_version=model_version,
             row=row,
             prediction_id_column=prediction_id_column,
             feature_columns=feature_columns,
             output_value_column=output_value_column,
             output_probability_column=output_probability_column,
+            timestamp_column=timestamp_column,
         )
         for row in dataframe.to_dict(orient="records")
     )
 
 
 def _event(  # type: ignore[no-untyped-def]
     workspace: str,
     model_name: str,
     model_version: str,
     row,
     prediction_id_column,
     feature_columns,
     output_value_column,
     output_probability_column,
+    timestamp_column: Optional[str] = None,
 ) -> PredictionEvent:
     prediction_id = str(row[prediction_id_column])
-    event = PredictionEvent(
+    input_features = None
+    if feature_columns is not None:
+        input_features = {key: row[key] for key in feature_columns}
+
+    output_value = None
+    if output_value_column is not None:
+        output_value = row[output_value_column]
+
+    output_probability = None
+    if output_probability_column is not None:
+        output_probability = row[output_probability_column]
+
+    timestamp = None
+    if timestamp_column is not None:
+        timestamp = row[timestamp_column]
+
+    return PredictionEvent(
         workspace=workspace,
         model_name=model_name,
         model_version=model_version,
         prediction_id=prediction_id,
+        input_features=input_features,
+        output_value=output_value,
+        output_probability=output_probability,
+        timestamp=timestamp,
     )
-    if feature_columns is not None:
-        event.input_features = {key: row[key] for key in feature_columns}
-    if output_value_column is not None:
-        event.output_value = row[output_value_column]
-    if output_probability_column is not None:
-        event.output_probability = row[output_probability_column]
-
-    return event
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/events/label_event.py` & `comet_mpm-0.4.2/src/comet_mpm/events/label_event.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/events/prediction_event.py` & `comet_mpm-0.4.2/src/comet_mpm/events/prediction_event.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,20 +51,22 @@
         workspace: str,
         model_name: str,
         model_version: str,
         prediction_id: str,
         input_features: Optional[Dict[str, Any]] = None,
         output_value: Any = None,
         output_probability: Optional[float] = None,
+        timestamp: Optional[float] = None,
     ):
         super(PredictionEvent, self).__init__(
             workspace=workspace,
             model_name=model_name,
             model_version=model_version,
             prediction_id=prediction_id,
+            timestamp=timestamp,
         )
         self.input_features = input_features
         self.output_value = output_value
         self.output_probability = output_probability
 
     def _get_event_dict(self) -> Dict[str, Any]:
         prediction: Dict[str, Any] = {}
```

### Comparing `comet_mpm-0.4.1/src/comet_mpm/exceptions.py` & `comet_mpm-0.4.2/src/comet_mpm/exceptions.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/logging_messages.py` & `comet_mpm-0.4.2/src/comet_mpm/logging_messages.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/optional_update.py` & `comet_mpm-0.4.2/src/comet_mpm/optional_update.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/sender/__init__.py` & `comet_mpm-0.4.2/src/comet_mpm/sender/__init__.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/sender/asyncio_sender.py` & `comet_mpm-0.4.2/src/comet_mpm/sender/asyncio_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/sender/base.py` & `comet_mpm-0.4.2/src/comet_mpm/sender/base.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/sender/thread_sender.py` & `comet_mpm-0.4.2/src/comet_mpm/sender/thread_sender.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm/settings.py` & `comet_mpm-0.4.2/src/comet_mpm/settings.py`

 * *Files identical despite different names*

### Comparing `comet_mpm-0.4.1/src/comet_mpm.egg-info/SOURCES.txt` & `comet_mpm-0.4.2/src/comet_mpm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

