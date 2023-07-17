# Comparing `tmp/global_tonemapping-0.1.0.tar.gz` & `tmp/global_tonemapping-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_tonemapping-0.1.0.tar", last modified: Sat Jul 15 19:36:04 2023, max compression
+gzip compressed data, was "global_tonemapping-0.1.2.tar", last modified: Mon Jul 17 19:06:08 2023, max compression
```

## Comparing `global_tonemapping-0.1.0.tar` & `global_tonemapping-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 19:36:04.761202 global_tonemapping-0.1.0/
--rw-rw-rw-   0        0        0      208 2023-07-15 19:36:04.761202 global_tonemapping-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-15 11:18:12.000000 global_tonemapping-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 19:36:04.754377 global_tonemapping-0.1.0/global_tonemapping.egg-info/
--rw-rw-rw-   0        0        0      208 2023-07-15 19:36:04.000000 global_tonemapping-0.1.0/global_tonemapping.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      315 2023-07-15 19:36:04.000000 global_tonemapping-0.1.0/global_tonemapping.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 19:36:04.000000 global_tonemapping-0.1.0/global_tonemapping.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 19:36:04.000000 global_tonemapping-0.1.0/global_tonemapping.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 19:36:04.761202 global_tonemapping-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      346 2023-07-15 19:36:02.000000 global_tonemapping-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:36:04.761202 global_tonemapping-0.1.0/tests/
--rw-rw-rw-   0        0        0     1090 2023-07-15 11:54:54.000000 global_tonemapping-0.1.0/tests/test_crfio.py
--rw-rw-rw-   0        0        0      838 2023-07-15 19:03:56.000000 global_tonemapping-0.1.0/tests/test_merging.py
--rw-rw-rw-   0        0        0     1484 2023-07-15 19:26:49.000000 global_tonemapping-0.1.0/tests/test_processor.py
--rw-rw-rw-   0        0        0      667 2023-07-15 19:23:54.000000 global_tonemapping-0.1.0/tests/test_sharpen.py
--rw-rw-rw-   0        0        0     1560 2023-07-15 19:22:46.000000 global_tonemapping-0.1.0/tests/test_suit.py
--rw-rw-rw-   0        0        0      607 2023-07-15 19:23:39.000000 global_tonemapping-0.1.0/tests/test_tonemap.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:06:08.097828 global_tonemapping-0.1.2/
+-rw-rw-rw-   0        0        0      212 2023-07-17 19:06:08.097828 global_tonemapping-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-15 11:18:12.000000 global_tonemapping-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 19:06:08.097828 global_tonemapping-0.1.2/global_tonemapping.egg-info/
+-rw-rw-rw-   0        0        0      212 2023-07-17 19:06:08.000000 global_tonemapping-0.1.2/global_tonemapping.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-07-17 19:06:08.000000 global_tonemapping-0.1.2/global_tonemapping.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:06:08.000000 global_tonemapping-0.1.2/global_tonemapping.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-07-17 19:06:08.000000 global_tonemapping-0.1.2/global_tonemapping.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:06:08.000000 global_tonemapping-0.1.2/global_tonemapping.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:06:08.097828 global_tonemapping-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      409 2023-07-17 19:05:02.000000 global_tonemapping-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:06:08.097828 global_tonemapping-0.1.2/tests/
+-rw-rw-rw-   0        0        0      767 2023-07-17 18:33:06.000000 global_tonemapping-0.1.2/tests/test_crf_calc.py
+-rw-rw-rw-   0        0        0     1090 2023-07-15 11:54:54.000000 global_tonemapping-0.1.2/tests/test_crfio.py
+-rw-rw-rw-   0        0        0      828 2023-07-17 18:18:55.000000 global_tonemapping-0.1.2/tests/test_merging.py
+-rw-rw-rw-   0        0        0     2532 2023-07-17 18:27:43.000000 global_tonemapping-0.1.2/tests/test_processor.py
+-rw-rw-rw-   0        0        0      667 2023-07-15 19:23:54.000000 global_tonemapping-0.1.2/tests/test_sharpen.py
+-rw-rw-rw-   0        0        0      840 2023-07-17 18:11:51.000000 global_tonemapping-0.1.2/tests/test_suit.py
+-rw-rw-rw-   0        0        0      606 2023-07-17 18:19:08.000000 global_tonemapping-0.1.2/tests/test_tonemap.py
```

### Comparing `global_tonemapping-0.1.0/tests/test_crfio.py` & `global_tonemapping-0.1.2/tests/test_crfio.py`

 * *Files identical despite different names*

### Comparing `global_tonemapping-0.1.0/tests/test_merging.py` & `global_tonemapping-0.1.2/tests/test_merging.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,17 +11,17 @@
         return pickle.load(f)
 
 
 class TestMerging(unittest.TestCase):
 
     def test_merging(self):
         # Load the expected inputs and outputs
-        images_w_exposure = load_pickle('examplers/pickles/image_w_exposure.pkl')
-        expected_output = load_pickle('examplers/pickles/merged.pkl')
-        crf = CRF_importer("../config/crf_bottom.npy")
+        images_w_exposure = load_pickle('examplers/pickles/list_10.pkl')
+        expected_output = load_pickle('examplers/pickles/merge.pkl')
+        crf = load_pickle('examplers/pickles/crf.pkl')
 
         # Call the function with the expected inputs
         result = merging(images_w_exposure, crf)
 
         # Check the function output
         self.assertTrue(numpy.array_equal(result, expected_output))
```

### Comparing `global_tonemapping-0.1.0/tests/test_processor.py` & `global_tonemapping-0.1.2/tests/test_processor.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,28 +14,49 @@
 
 def load_pickle(file_name):
     with open(file_name, 'rb') as f:
         return pickle.load(f)
 
 class TestProcessor(unittest.TestCase):
     def test_processor_b(self):
-        input = load_pickle('./examplers/pickles/image_w_exposure.pkl')
+        input = load_pickle('./examplers/pickles/list_10.pkl')
         expected_output = load_pickle('./examplers/pickles/sharpen.pkl')
         # Call the function with the expected inputs
-        result = processor(input, selector="B", gb=1.4, sb=2.0, sharpening_itteration=3, s=20, r=0.1)
+        result = processor(input, selector="B", gamma=1.4, saturation=2.0, sharpening_iteration=3, s=20, r=0.1)
 
         # Check the function output
         self.assertTrue(numpy.array_equal(result, expected_output))
 
 
     def test_processor_b_v2(self):
-        input = load_pickle('./examplers/pickles/dict.pkl')
+        input = load_pickle('./examplers/pickles/dict_10.pkl')
         expected_output = load_pickle('./examplers/pickles/sharpen.pkl')
         # Call the function with the expected inputs
-        result = processor(input, selector="B", gb=1.4, sb=2.0, sharpening_itteration=3, s=20, r=0.1)
+        result = processor(input, selector="B", gamma=1.4, saturation=2.0, sharpening_iteration=3, s=20, r=0.1)
+
+        try:
+            npt.assert_array_equal(result, expected_output)
+        except AssertionError as e:
+            print(f'Test_processor_b failed with difference: {e}')
+            raise
+
+    def test_processor_b_crf(self):
+        input = load_pickle('./examplers/pickles/list_100.pkl')
+        expected_output = load_pickle('./examplers/pickles/crf.pkl')
+        # Call the function with the expected inputs
+        result = processor(input, selector="B", gamma=1.4, saturation=2.0, sharpening_iteration=3, s=20, r=0.1, mode="calibration")
+
+        # Check the function output
+        self.assertTrue(numpy.array_equal(result, expected_output))
+
+    def test_processor_b_v2_crf(self):
+        input = load_pickle('./examplers/pickles/list_100.pkl')
+        expected_output = load_pickle('./examplers/pickles/crf.pkl')
+        # Call the function with the expected inputs
+        result = processor(input, selector="B", gamma=1.4, saturation=2.0, sharpening_iteration=3, s=20, r=0.1, mode="calibration")
 
         try:
             npt.assert_array_equal(result, expected_output)
         except AssertionError as e:
             print(f'Test_processor_b failed with difference: {e}')
             raise
```

### Comparing `global_tonemapping-0.1.0/tests/test_sharpen.py` & `global_tonemapping-0.1.2/tests/test_sharpen.py`

 * *Files identical despite different names*

### Comparing `global_tonemapping-0.1.0/tests/test_tonemap.py` & `global_tonemapping-0.1.2/tests/test_tonemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 def load_pickle(file_name):
     with open(file_name, 'rb') as f:
         return pickle.load(f)
 
 class TestTonemap(unittest.TestCase):
     def test_tonemap(self):
-        tonemap = load_pickle("examplers/pickles/merged.pkl")
+        tonemap = load_pickle("examplers/pickles/merge.pkl")
         expected_output = load_pickle("examplers/pickles/tonemap.pkl")
 
         result = tonemaping.tonemaping(tonemap)
 
         # Check the function output
         self.assertTrue(numpy.array_equal(result, expected_output))
 if __name__ == '__main__':
```

