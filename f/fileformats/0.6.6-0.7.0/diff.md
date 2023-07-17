# Comparing `tmp/fileformats-0.6.6.tar.gz` & `tmp/fileformats-0.7.0.tar.gz`

## Comparing `fileformats-0.6.6.tar` & `fileformats-0.7.0.tar`

### file list

```diff
@@ -1,53 +1,46 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/_version.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/converter.py
--rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/datatype.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/field.py
--rw-r--r--   0        0        0    42563 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/fileset.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/mark.py
--rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/mixin.py
--rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/utils.py
--rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_subpackages.py
--rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/document/__init__.py
--rw-r--r--   0        0        0     5127 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/__init__.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/basic.py
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/classifiers.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/converters.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/testing/headers.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.6/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.6/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.6/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.6/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.6/README.rst
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 fileformats-0.6.6/pyproject.toml
--rw-r--r--   0        0        0    22460 2020-02-02 00:00:00.000000 fileformats-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/_version.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/converter.py
+-rw-r--r--   0        0        0    10508 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/datatype.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/field.py
+-rw-r--r--   0        0        0    42563 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/fileset.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24544 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/mixin.py
+-rw-r--r--   0        0        0     7112 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8172 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     4312 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_subpackages.py
+-rw-r--r--   0        0        0    11427 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     8335 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/base.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/vector.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/__init__.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/basic.py
+-rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/classifiers.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/testing/headers.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.7.0/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.7.0/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.7.0/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.7.0/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.7.0/README.rst
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 fileformats-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    22316 2020-02-02 00:00:00.000000 fileformats-0.7.0/PKG-INFO
```

### Comparing `fileformats-0.6.6/fileformats/archive/__init__.py` & `fileformats-0.7.0/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/audio/__init__.py` & `fileformats-0.7.0/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/converter.py` & `fileformats-0.7.0/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/datatype.py` & `fileformats-0.7.0/fileformats/core/datatype.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/field.py` & `fileformats-0.7.0/fileformats/core/field.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/fileset.py` & `fileformats-0.7.0/fileformats/core/fileset.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/mark.py` & `fileformats-0.7.0/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/mixin.py` & `fileformats-0.7.0/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/utils.py` & `fileformats-0.7.0/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_classifiers.py` & `fileformats-0.7.0/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_converter.py` & `fileformats-0.7.0/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_detection.py` & `fileformats-0.7.0/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_general.py` & `fileformats-0.7.0/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_mime.py` & `fileformats-0.7.0/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_mixin.py` & `fileformats-0.7.0/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_subpackages.py` & `fileformats-0.7.0/fileformats/core/tests/test_subpackages.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/core/tests/test_utils.py` & `fileformats-0.7.0/fileformats/core/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/document/__init__.py` & `fileformats-0.7.0/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/field/__init__.py` & `fileformats-0.7.0/fileformats/field/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+"""Adds support for "field" data types
+
+While not "file-formats", in some workflows, particularly when interacting with a data
+store such as in Arcana, it is useful to interchangeably interact with file and field
+data, so the classes in this module are provided to support these use cases.
+"""
 import decimal
 import typing as ty
 import attrs
 from fileformats.core import Field
 from fileformats.core.mixin import WithClassifiers
 from fileformats.core.exceptions import FormatMismatchError
```

### Comparing `fileformats-0.6.6/fileformats/field/tests/test_fields.py` & `fileformats-0.7.0/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.7.0/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/generic/__init__.py` & `fileformats-0.7.0/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/image/raster.py` & `fileformats-0.7.0/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/image/tests/test_image_raster.py` & `fileformats-0.7.0/fileformats/image/tests/test_image_raster.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 @pytest.fixture(scope="session")
 def png_path():
     return get_remote_file("images/chelsea.png")
 
 
+@pytest.mark.xfail(reason="No converter between PNG and tiff")
 def test_tiff_endianness(png_path):
     png = Png(png_path)
     Tiff.convert(png)
 
 
 def test_tiff_fail(png_path, work_dir):
     bad_tiff_path = work_dir / "bad_tiff.tiff"
```

### Comparing `fileformats-0.6.6/fileformats/serialization/__init__.py` & `fileformats-0.7.0/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/testing/classifiers.py` & `fileformats-0.7.0/fileformats/testing/classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/testing/headers.py` & `fileformats-0.7.0/fileformats/testing/headers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/fileformats/text/__init__.py` & `fileformats-0.7.0/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/LICENSE` & `fileformats-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/README.rst` & `fileformats-0.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6.6/pyproject.toml` & `fileformats-0.7.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -45,37 +45,33 @@
 [project.optional-dependencies]
 dev = [
     "black",
     "pre-commit",
     "codespell",
     "flake8",
     "flake8-pyproject",
-    "fileformats[extended]",
     "fileformats[test]",
 ]
 test = [
     "pytest >=6.2.5",
     "pytest-env>=0.6.2",
     "pytest-cov>=2.12.1",
+    "imageio",
+    "pydra >=0.22",
 ]
 docs = [
     "packaging",
     "docutils>=0.10",
     "mock>1.0",
     "sphinx >=2.1.2",
     "sphinx-argparse>=0.2.0",
     "sphinx-click>=3.1",
     "furo>=2022.2.14.1",
     "numpydoc>=0.6.0",
 ]
-extended = [
-    "pydra >= 0.20.0",
-    "imageio >=2.24.0",
-    "PyYAML>=6.0",
-]
 
 [project.urls]
 repository = "https://github.com/ArcanaFramework/fileformats"
 
 
 [tool.hatch.version]
 source = "vcs"
```

### Comparing `fileformats-0.6.6/PKG-INFO` & `fileformats-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6.6
+Version: 0.7.0
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
         
@@ -113,33 +113,30 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: attrs>=22.1.0
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: codespell; extra == 'dev'
-Requires-Dist: fileformats[extended]; extra == 'dev'
 Requires-Dist: fileformats[test]; extra == 'dev'
 Requires-Dist: flake8; extra == 'dev'
 Requires-Dist: flake8-pyproject; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: docutils>=0.10; extra == 'docs'
 Requires-Dist: furo>=2022.2.14.1; extra == 'docs'
 Requires-Dist: mock>1.0; extra == 'docs'
 Requires-Dist: numpydoc>=0.6.0; extra == 'docs'
 Requires-Dist: packaging; extra == 'docs'
 Requires-Dist: sphinx-argparse>=0.2.0; extra == 'docs'
 Requires-Dist: sphinx-click>=3.1; extra == 'docs'
 Requires-Dist: sphinx>=2.1.2; extra == 'docs'
-Provides-Extra: extended
-Requires-Dist: imageio>=2.24.0; extra == 'extended'
-Requires-Dist: pydra>=0.20.0; extra == 'extended'
-Requires-Dist: pyyaml>=6.0; extra == 'extended'
 Provides-Extra: test
+Requires-Dist: imageio; extra == 'test'
+Requires-Dist: pydra>=0.22; extra == 'test'
 Requires-Dist: pytest-cov>=2.12.1; extra == 'test'
 Requires-Dist: pytest-env>=0.6.2; extra == 'test'
 Requires-Dist: pytest>=6.2.5; extra == 'test'
 Description-Content-Type: text/x-rst
 
 FileFormats
 ===========
```

