# Comparing `tmp/ngff_zarr-0.4.4.tar.gz` & `tmp/ngff_zarr-0.4.5.tar.gz`

## Comparing `ngff_zarr-0.4.4.tar` & `ngff_zarr-0.4.5.tar`

### file list

```diff
@@ -1,48 +1,59 @@
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.github/workflows/test.yml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/__about__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/__init__.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/_array_split.py
--rwxr-xr-x   0        0        0    10939 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/cli.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/config.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/detect_cli_io_backend.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/from_ngff_zarr.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/memory_usage.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/multiscales.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/ngff_image.py
--rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/ngff_image_to_itk_image.py
--rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/rich_dask_progress.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/task_count.py
--rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/to_multiscales.py
--rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/to_ngff_image.py
--rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/to_ngff_zarr.py
--rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/zarr_metadata.py
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/methods/__init__.py
--rw-r--r--   0        0        0    16129 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/methods/_dask_image.py
--rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/methods/_itk.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/ngff_zarr/methods/_support.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/__init__.py
--rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/_data.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_cli_input_to_ngff_image.py
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_detect_cli_input_backend.py
--rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_from_ngff_zarr.py
--rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_itk_image_to_ngff_image.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_large_serialization.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_memory_usage.py
--rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_ngff_image_scale_factors.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_ngff_image_to_itk_image.py
--rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_task_count.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_to_ngff_zarr_dask_image.py
--rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/test/test_to_ngff_zarr_itk.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/LICENSE.txt
--rw-r--r--   0        0        0     3375 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/README.md
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/pyproject.toml
--rw-r--r--   0        0        0     5188 2020-02-02 00:00:00.000000 ngff_zarr-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.readthedocs.yaml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.github/workflows/test.yml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/.gitignore
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/Makefile
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/cli.md
+-rw-r--r--   0        0        0     1511 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/conf.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/development.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/index.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/make.bat
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/requirements.txt
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/_static/favicon.png
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/docs/_static/logo.png
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/__about__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/__init__.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/_array_split.py
+-rwxr-xr-x   0        0        0    10939 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/cli.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/config.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/detect_cli_io_backend.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/from_ngff_zarr.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/memory_usage.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/multiscales.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/ngff_image.py
+-rw-r--r--   0        0        0     2470 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/rich_dask_progress.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/task_count.py
+-rw-r--r--   0        0        0    13466 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_multiscales.py
+-rw-r--r--   0        0        0     3200 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_ngff_image.py
+-rw-r--r--   0        0        0    10321 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/to_ngff_zarr.py
+-rw-r--r--   0        0        0     3360 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/zarr_metadata.py
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/__init__.py
+-rw-r--r--   0        0        0    16279 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_dask_image.py
+-rw-r--r--   0        0        0    18392 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_itk.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/ngff_zarr/methods/_support.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/__init__.py
+-rw-r--r--   0        0        0     3263 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/_data.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_cli_input_to_ngff_image.py
+-rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_detect_cli_input_backend.py
+-rw-r--r--   0        0        0     1584 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_from_ngff_zarr.py
+-rw-r--r--   0        0        0     3341 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_itk_image_to_ngff_image.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_large_serialization.py
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_memory_usage.py
+-rw-r--r--   0        0        0      878 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_ngff_image_scale_factors.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_ngff_image_to_itk_image.py
+-rw-r--r--   0        0        0      894 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_task_count.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_to_ngff_zarr_dask_image.py
+-rw-r--r--   0        0        0     4917 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/test/test_to_ngff_zarr_itk.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/LICENSE.txt
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/README.md
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0     3478 2020-02-02 00:00:00.000000 ngff_zarr-0.4.5/PKG-INFO
```

### Comparing `ngff_zarr-0.4.4/.github/workflows/test.yml` & `ngff_zarr-0.4.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/.pytest_cache/v/cache/nodeids` & `ngff_zarr-0.4.5/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/__init__.py` & `ngff_zarr-0.4.5/ngff_zarr/__init__.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/_array_split.py` & `ngff_zarr-0.4.5/ngff_zarr/_array_split.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/cli.py` & `ngff_zarr-0.4.5/ngff_zarr/cli.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/cli_input_to_ngff_image.py` & `ngff_zarr-0.4.5/ngff_zarr/cli_input_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/config.py` & `ngff_zarr-0.4.5/ngff_zarr/config.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/detect_cli_io_backend.py` & `ngff_zarr-0.4.5/ngff_zarr/detect_cli_io_backend.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/from_ngff_zarr.py` & `ngff_zarr-0.4.5/ngff_zarr/from_ngff_zarr.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/itk_image_to_ngff_image.py` & `ngff_zarr-0.4.5/ngff_zarr/itk_image_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/memory_usage.py` & `ngff_zarr-0.4.5/ngff_zarr/memory_usage.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/multiscales.py` & `ngff_zarr-0.4.5/ngff_zarr/multiscales.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/ngff_image_to_itk_image.py` & `ngff_zarr-0.4.5/ngff_zarr/ngff_image_to_itk_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/rich_dask_progress.py` & `ngff_zarr-0.4.5/ngff_zarr/rich_dask_progress.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/to_multiscales.py` & `ngff_zarr-0.4.5/ngff_zarr/to_multiscales.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/to_ngff_image.py` & `ngff_zarr-0.4.5/ngff_zarr/to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/to_ngff_zarr.py` & `ngff_zarr-0.4.5/ngff_zarr/to_ngff_zarr.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/zarr_metadata.py` & `ngff_zarr-0.4.5/ngff_zarr/zarr_metadata.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/methods/_dask_image.py` & `ngff_zarr-0.4.5/ngff_zarr/methods/_dask_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,20 @@
     import dask_image.ndinterp
 
     multiscales = [
         ngff_image,
     ]
     previous_image = ngff_image
     dims = ngff_image.dims
-    previous_dim_factors = {d: 1 for d in dims}
+    previous_absolute_dim_factors = {d: 1 for d in dims}
+    previous_scale_factor = 1
     for scale_factor in scale_factors:
-        dim_factors = _dim_scale_factors(dims, scale_factor, previous_dim_factors)
-        previous_dim_factors = dim_factors
+        dim_factors = _dim_scale_factors(dims, scale_factor, previous_absolute_dim_factors)
+        previous_absolute_dim_factors = {d:v*previous_scale_factor for d, v in dim_factors.items()}
+        previous_scale_factor = scale_factor
         previous_image = _align_chunks(previous_image, default_chunks, dim_factors)
 
         shrink_factors = []
         for dim in dims:
             if dim in dim_factors:
                 shrink_factors.append(dim_factors[dim])
             else:
```

### Comparing `ngff_zarr-0.4.4/ngff_zarr/methods/_itk.py` & `ngff_zarr-0.4.5/ngff_zarr/methods/_itk.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/ngff_zarr/methods/_support.py` & `ngff_zarr-0.4.5/ngff_zarr/methods/_support.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/_data.py` & `ngff_zarr-0.4.5/test/_data.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_cli_input_to_ngff_image.py` & `ngff_zarr-0.4.5/test/test_cli_input_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_detect_cli_input_backend.py` & `ngff_zarr-0.4.5/test/test_detect_cli_input_backend.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_from_ngff_zarr.py` & `ngff_zarr-0.4.5/test/test_from_ngff_zarr.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_itk_image_to_ngff_image.py` & `ngff_zarr-0.4.5/test/test_itk_image_to_ngff_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_large_serialization.py` & `ngff_zarr-0.4.5/test/test_large_serialization.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_memory_usage.py` & `ngff_zarr-0.4.5/test/test_memory_usage.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_ngff_image_scale_factors.py` & `ngff_zarr-0.4.5/test/test_ngff_image_scale_factors.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_ngff_image_to_itk_image.py` & `ngff_zarr-0.4.5/test/test_ngff_image_to_itk_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_task_count.py` & `ngff_zarr-0.4.5/test/test_task_count.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_to_ngff_zarr_dask_image.py` & `ngff_zarr-0.4.5/test/test_to_ngff_zarr_dask_image.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/test/test_to_ngff_zarr_itk.py` & `ngff_zarr-0.4.5/test/test_to_ngff_zarr_itk.py`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/LICENSE.txt` & `ngff_zarr-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ngff_zarr-0.4.4/pyproject.toml` & `ngff_zarr-0.4.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 cli = [
     "dask-image",
     "dask[distributed]",
     "itk-filtering>=5.3.0",
     "itk-io>=5.3.0",
     "imageio",
     "tifffile",
+    "imagecodecs",
 ]
 test = [
     "pytest",
     "pooch",
     "itkwasm",
     "itk-io>=5.3.0",
     "itk-filtering>=5.3.0",
```

