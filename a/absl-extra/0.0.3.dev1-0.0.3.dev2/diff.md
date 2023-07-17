# Comparing `tmp/absl_extra-0.0.3.dev1.tar.gz` & `tmp/absl_extra-0.0.3.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.3.dev1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.3.dev2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.3.dev1.tar` & `absl_extra-0.0.3.dev2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1521 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/Readme.md
--rw-r--r--   0        0        0       74 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/__init__.py
--rw-r--r--   0        0        0     1945 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/callbacks.py
--rw-r--r--   0        0        0    16818 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/flax_utils.py
--rw-r--r--   0        0        0     5411 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/jax_utils.py
--rw-r--r--   0        0        0     1605 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/logging_utils.py
--rw-r--r--   0        0        0     3238 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/notifier.py
--rw-r--r--   0        0        0       64 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/py.typed
--rw-r--r--   0        0        0     5702 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/tasks.py
--rw-r--r--   0        0        0        0 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/testing/__init__.py
--rw-r--r--   0        0        0     2301 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/testing/lifted_variants.py
--rw-r--r--   0        0        0     4623 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/absl_extra/tf_utils.py
--rw-r--r--   0        0        0     1071 2023-07-17 08:37:47.932638 absl_extra-0.0.3.dev1/pyproject.toml
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 absl_extra-0.0.3.dev1/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/Readme.md
+-rw-r--r--   0        0        0       74 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/__init__.py
+-rw-r--r--   0        0        0     1945 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/callbacks.py
+-rw-r--r--   0        0        0    17373 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/flax_utils.py
+-rw-r--r--   0        0        0     5411 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/jax_utils.py
+-rw-r--r--   0        0        0     1605 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/logging_utils.py
+-rw-r--r--   0        0        0     3238 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/notifier.py
+-rw-r--r--   0        0        0       64 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/py.typed
+-rw-r--r--   0        0        0     5702 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2301 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/testing/lifted_variants.py
+-rw-r--r--   0        0        0     4623 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/absl_extra/tf_utils.py
+-rw-r--r--   0        0        0     1071 2023-07-17 09:51:24.083073 absl_extra-0.0.3.dev2/pyproject.toml
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 absl_extra-0.0.3.dev2/PKG-INFO
```

### Comparing `absl_extra-0.0.3.dev1/Readme.md` & `absl_extra-0.0.3.dev2/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/callbacks.py` & `absl_extra-0.0.3.dev2/absl_extra/callbacks.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/flax_utils.py` & `absl_extra-0.0.3.dev2/absl_extra/flax_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -340,17 +340,17 @@
     for epoch in range(epochs):
         if verbose:
             logging.info(f"Epoch {epoch + 1}/{epochs}...")
 
         for hook in hooks.on_epoch_begin:
             hook(int(training_state.step))
 
-        training_dataset = prefetch_to_device(
-            training_dataset_factory(), prefetch_buffer_size
-        )
+        training_dataset = training_dataset_factory()
+        if prefetch_buffer_size != 0:
+            prefetch_to_device(training_dataset, prefetch_buffer_size)
         training_metrics = metrics_container_type.empty()
 
         for x_batch, y_batch in training_dataset:
             for hook in hooks.on_step_begin:
                 hook(int(training_state.step))
 
             training_state, training_metrics = training_step_func(
@@ -365,17 +365,17 @@
                 )
         if verbose:
             logging.info(
                 {f"train_{k}": f"{float(v):.3f}"}
                 for k, v in training_metrics.compute().items()
             )
 
-        validation_dataset = prefetch_to_device(
-            validation_dataset_factory(), prefetch_buffer_size
-        )
+        validation_dataset = validation_dataset_factory()
+        if prefetch_buffer_size != 0:
+            validation_dataset = prefetch_to_device(validation_dataset, prefetch_buffer_size)
         validation_metrics = metrics_container_type.empty()
 
         for x_batch, y_batch in validation_dataset:
             validation_metrics = validation_step_func(
                 training_state, x_batch, y_batch, validation_metrics
             )
 
@@ -414,35 +414,41 @@
     prefetch_buffer_size: int,
     verbose: bool,
 ) -> MetricsAndParams:
     # How do we handle prngKey or batch stats?
     training_state = jax_utils.replicate(training_state)
     if hasattr(training_state, "dropout_key"):
         training_state.replace(
-            dropout_key=common_utils.shard_prng_key(training_state.dropout_key)
+            dropout_key=common_utils.shard_prng_key(
+                jax_utils.unreplicate(training_state.dropout_key)
+            )
         )
 
     def step_number():
         return int(jax_utils.unreplicate(training_state.step))
 
     for epoch in range(epochs):
         if verbose:
             logging.info(f"Epoch {epoch + 1}/{epochs}...")
 
         for hook in hooks.on_epoch_begin:
             hook(step_number())
 
-        training_dataset = jax_utils.prefetch_to_device(
-            training_dataset_factory(), prefetch_buffer_size
-        )
+        training_dataset = training_dataset_factory()
+        if prefetch_buffer_size != 0:
+            training_dataset = jax_utils.prefetch_to_device(training_dataset, prefetch_buffer_size)
+        
         training_metrics = jax_utils.replicate(metrics_container_type.empty())
 
         for x_batch, y_batch in training_dataset:
             for hook in hooks.on_step_begin:
                 hook(step_number())
+            
+            x_batch = common_utils.shard(x_batch)
+            y_batch = common_utils.shard(y_batch)
 
             training_state, training_metrics = training_step_func(
                 training_state, x_batch, y_batch, training_metrics
             )
 
             for hook in hooks.on_step_end:  # type: ignore
                 hook(  # type: ignore
@@ -452,20 +458,25 @@
                 )
         if verbose:
             logging.info(
                 {f"train_{k}": f"{float(v):.3f}"}
                 for k, v in training_metrics.unreplicate().compute().items()
             )
 
-        validation_dataset = jax_utils.prefetch_to_device(
-            validation_dataset_factory(), prefetch_buffer_size
-        )
+        validation_dataset = validation_dataset_factory()
+        if prefetch_buffer_size != 0:
+            validation_dataset = jax_utils.prefetch_to_device(validation_dataset, prefetch_buffer_size)
+        
         validation_metrics = jax_utils.replicate(metrics_container_type.empty())
 
         for x_batch, y_batch in validation_dataset:
+            
+            x_batch = common_utils.shard(x_batch)
+            y_batch = common_utils.shard(y_batch)
+            
             validation_metrics = validation_step_func(
                 training_state, x_batch, y_batch, validation_metrics
             )
 
         if verbose:
             logging.info(
                 {f"val_{k}": f"{float(v):.3f}"}
```

### Comparing `absl_extra-0.0.3.dev1/absl_extra/jax_utils.py` & `absl_extra-0.0.3.dev2/absl_extra/jax_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/logging_utils.py` & `absl_extra-0.0.3.dev2/absl_extra/logging_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/notifier.py` & `absl_extra-0.0.3.dev2/absl_extra/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/tasks.py` & `absl_extra-0.0.3.dev2/absl_extra/tasks.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/testing/lifted_variants.py` & `absl_extra-0.0.3.dev2/absl_extra/testing/lifted_variants.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/absl_extra/tf_utils.py` & `absl_extra-0.0.3.dev2/absl_extra/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev1/pyproject.toml` & `absl_extra-0.0.3.dev2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.3dev1"
+version = "0.0.3dev2"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.3.dev1/PKG-INFO` & `absl_extra-0.0.3.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.3.dev1
+Version: 0.0.3.dev2
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

