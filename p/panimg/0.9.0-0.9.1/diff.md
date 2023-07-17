# Comparing `tmp/panimg-0.9.0.tar.gz` & `tmp/panimg-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panimg-0.9.0.tar", max compression
+gzip compressed data, was "panimg-0.9.1.tar", max compression
```

## Comparing `panimg-0.9.0.tar` & `panimg-0.9.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0    11363 2022-07-07 09:23:05.261732 panimg-0.9.0/LICENSE
--rw-r--r--   0        0        0     5537 2022-07-07 09:23:05.261732 panimg-0.9.0/README.md
--rw-r--r--   0        0        0      134 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/__init__.py
--rw-r--r--   0        0        0     1759 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/cli.py
--rw-r--r--   0        0        0        0 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/__init__.py
--rw-r--r--   0        0        0     1069 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/LICENSE
--rw-r--r--   0        0        0        0 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/__init__.py
--rw-r--r--   0        0        0      147 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/image_types/__init__.py
--rw-r--r--   0        0        0      534 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/image_types/fundus.py
--rw-r--r--   0        0        0      666 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/image_types/oct.py
--rw-r--r--   0        0        0       96 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/readers/__init__.py
--rw-r--r--   0        0        0     7782 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/readers/e2e.py
--rw-r--r--   0        0        0     5098 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/readers/fda.py
--rw-r--r--   0        0        0     5194 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/contrib/oct_converter/readers/fds.py
--rw-r--r--   0        0        0      492 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/exceptions.py
--rw-r--r--   0        0        0      963 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/__init__.py
--rw-r--r--   0        0        0    19421 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/dicom.py
--rw-r--r--   0        0        0     1914 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/fallback.py
--rw-r--r--   0        0        0     3911 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/metaio_mhd_mha.py
--rw-r--r--   0        0        0     1840 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/metaio_nifti.py
--rw-r--r--   0        0        0     4243 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/metaio_nrrd.py
--rw-r--r--   0        0        0     9377 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/metaio_utils.py
--rw-r--r--   0        0        0     7092 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/oct.py
--rw-r--r--   0        0        0    14254 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/image_builders/tiff.py
--rw-r--r--   0        0        0    12150 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/models.py
--rw-r--r--   0        0        0     6576 2022-07-07 09:23:05.261732 panimg-0.9.0/panimg/panimg.py
--rw-r--r--   0        0        0      154 2022-07-07 09:23:05.265732 panimg-0.9.0/panimg/post_processors/__init__.py
--rw-r--r--   0        0        0     2055 2022-07-07 09:23:05.265732 panimg-0.9.0/panimg/post_processors/tiff_to_dzi.py
--rw-r--r--   0        0        0       86 2022-07-07 09:23:05.265732 panimg-0.9.0/panimg/settings.py
--rw-r--r--   0        0        0      516 2022-07-07 09:23:05.265732 panimg-0.9.0/panimg/types.py
--rw-r--r--   0        0        0     1929 2022-07-07 09:23:05.265732 panimg-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     7064 2022-07-07 09:23:19.544195 panimg-0.9.0/setup.py
--rw-r--r--   0        0        0     6987 2022-07-07 09:23:19.544937 panimg-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11363 2022-07-12 08:54:00.450388 panimg-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5537 2022-07-12 08:54:00.450388 panimg-0.9.1/README.md
+-rw-r--r--   0        0        0      134 2022-07-12 08:54:00.450388 panimg-0.9.1/panimg/__init__.py
+-rw-r--r--   0        0        0     1759 2022-07-12 08:54:00.450388 panimg-0.9.1/panimg/cli.py
+-rw-r--r--   0        0        0        0 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/__init__.py
+-rw-r--r--   0        0        0     1069 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/LICENSE
+-rw-r--r--   0        0        0        0 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/__init__.py
+-rw-r--r--   0        0        0      147 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/image_types/__init__.py
+-rw-r--r--   0        0        0      534 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/image_types/fundus.py
+-rw-r--r--   0        0        0      666 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/image_types/oct.py
+-rw-r--r--   0        0        0       96 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/readers/__init__.py
+-rw-r--r--   0        0        0     7782 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/readers/e2e.py
+-rw-r--r--   0        0        0     5098 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/readers/fda.py
+-rw-r--r--   0        0        0     5194 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/contrib/oct_converter/readers/fds.py
+-rw-r--r--   0        0        0      492 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/exceptions.py
+-rw-r--r--   0        0        0      963 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/__init__.py
+-rw-r--r--   0        0        0    19421 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/dicom.py
+-rw-r--r--   0        0        0     1914 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/fallback.py
+-rw-r--r--   0        0        0     3911 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/metaio_mhd_mha.py
+-rw-r--r--   0        0        0     1840 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/metaio_nifti.py
+-rw-r--r--   0        0        0     4243 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/metaio_nrrd.py
+-rw-r--r--   0        0        0     9377 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/metaio_utils.py
+-rw-r--r--   0        0        0     7092 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/oct.py
+-rw-r--r--   0        0        0    14254 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/image_builders/tiff.py
+-rw-r--r--   0        0        0    12163 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/models.py
+-rw-r--r--   0        0        0     6576 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/panimg.py
+-rw-r--r--   0        0        0      154 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/post_processors/__init__.py
+-rw-r--r--   0        0        0     2055 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/post_processors/tiff_to_dzi.py
+-rw-r--r--   0        0        0       86 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/settings.py
+-rw-r--r--   0        0        0      516 2022-07-12 08:54:00.454388 panimg-0.9.1/panimg/types.py
+-rw-r--r--   0        0        0     1929 2022-07-12 08:54:00.454388 panimg-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     7064 2022-07-12 08:54:13.466955 panimg-0.9.1/setup.py
+-rw-r--r--   0        0        0     6987 2022-07-12 08:54:13.467974 panimg-0.9.1/PKG-INFO
```

### Comparing `panimg-0.9.0/LICENSE` & `panimg-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/README.md` & `panimg-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/cli.py` & `panimg-0.9.1/panimg/cli.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/LICENSE` & `panimg-0.9.1/panimg/contrib/oct_converter/LICENSE`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/image_types/fundus.py` & `panimg-0.9.1/panimg/contrib/oct_converter/image_types/fundus.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/image_types/oct.py` & `panimg-0.9.1/panimg/contrib/oct_converter/image_types/oct.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/readers/e2e.py` & `panimg-0.9.1/panimg/contrib/oct_converter/readers/e2e.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/readers/fda.py` & `panimg-0.9.1/panimg/contrib/oct_converter/readers/fda.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/contrib/oct_converter/readers/fds.py` & `panimg-0.9.1/panimg/contrib/oct_converter/readers/fds.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/__init__.py` & `panimg-0.9.1/panimg/image_builders/__init__.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/dicom.py` & `panimg-0.9.1/panimg/image_builders/dicom.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/fallback.py` & `panimg-0.9.1/panimg/image_builders/fallback.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/metaio_mhd_mha.py` & `panimg-0.9.1/panimg/image_builders/metaio_mhd_mha.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/metaio_nifti.py` & `panimg-0.9.1/panimg/image_builders/metaio_nifti.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/metaio_nrrd.py` & `panimg-0.9.1/panimg/image_builders/metaio_nrrd.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/metaio_utils.py` & `panimg-0.9.1/panimg/image_builders/metaio_utils.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/oct.py` & `panimg-0.9.1/panimg/image_builders/oct.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/image_builders/tiff.py` & `panimg-0.9.1/panimg/image_builders/tiff.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/models.py` & `panimg-0.9.1/panimg/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 import logging
 import re
 import shutil
 from enum import Enum
 from pathlib import Path
-from typing import Any, Dict, List, NamedTuple, Optional, Set, Tuple
+from typing import Any, Dict, FrozenSet, List, NamedTuple, Optional, Set, Tuple
 from uuid import UUID, uuid4
 
 import numpy as np
 import SimpleITK
 from pydantic import BaseModel, validator
 from pydantic.dataclasses import dataclass
 from SimpleITK import GetArrayViewFromImage, Image, WriteImage
@@ -151,15 +151,15 @@
     patient_age: str = ""
     patient_sex: PatientSex = PatientSex.EMPTY
     study_date: Optional[datetime.date] = None
     study_instance_uid: str = ""
     series_instance_uid: str = ""
     study_description: str = ""
     series_description: str = ""
-    segments: Optional[Tuple[int, ...]] = None
+    segments: Optional[FrozenSet[int]] = None
 
 
 @dataclass(frozen=True)
 class PanImgFile:
     image_id: UUID
     image_type: ImageType
     file: Path
@@ -270,22 +270,22 @@
         array = GetArrayViewFromImage(image)
         image.SetMetaData(smallest_tag, str(array.min()))
         image.SetMetaData(largest_tag, str(array.max()))
 
         return image
 
     @property
-    def segments(self) -> Optional[Tuple[int, ...]]:
+    def segments(self) -> Optional[FrozenSet[int]]:
         if self.image.GetPixelIDValue() not in MASK_TYPE_PIXEL_IDS:
             return None
 
         segments = np.unique(GetArrayViewFromImage(self.image))
 
         if len(segments) <= MAXIMUM_SEGMENTS_LENGTH:
-            return tuple(segments)
+            return frozenset(segments)
         else:
             return None
 
     @property
     def color_space(self) -> ColorSpace:
         return ITK_COLOR_SPACE_MAP[self.image.GetNumberOfComponentsPerPixel()]
```

### Comparing `panimg-0.9.0/panimg/panimg.py` & `panimg-0.9.1/panimg/panimg.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/post_processors/tiff_to_dzi.py` & `panimg-0.9.1/panimg/post_processors/tiff_to_dzi.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/panimg/types.py` & `panimg-0.9.1/panimg/types.py`

 * *Files identical despite different names*

### Comparing `panimg-0.9.0/pyproject.toml` & `panimg-0.9.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "panimg"
-version = "0.9.0"
+version = "0.9.1"
 description = "Conversion of medical images to MHA and TIFF."
 license = "Apache-2.0"
 authors = ["James Meakin <panimg@jmsmkn.com>"]
 readme = "README.md"
 repository = "https://github.com/DIAGNijmegen/rse-panimg"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `panimg-0.9.0/setup.py` & `panimg-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  ':python_version >= "3.8" and python_version < "4.0"': ['numpy>=1.22,<2.0']}
 
 entry_points = \
 {'console_scripts': ['panimg = panimg.cli:cli']}
 
 setup_kwargs = {
     'name': 'panimg',
-    'version': '0.9.0',
+    'version': '0.9.1',
     'description': 'Conversion of medical images to MHA and TIFF.',
     'long_description': '# panimg\n\n[![CI](https://github.com/DIAGNijmegen/rse-panimg/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/DIAGNijmegen/rse-panimg/actions/workflows/ci.yml?query=branch%3Amain)\n[![PyPI](https://img.shields.io/pypi/v/panimg)](https://pypi.org/project/panimg/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/panimg)](https://pypi.org/project/panimg/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![DOI](https://zenodo.org/badge/344730308.svg)](https://zenodo.org/badge/latestdoi/344730308)\n\n**NOT FOR CLINICAL USE**\n\nConversion of medical images to MHA and TIFF.\nRequires Python 3.7, 3.8, 3.9 or 3.10.\n`libvips-dev` and `libopenslide-dev` must be installed on your system.\n\nUnder the hood we use:\n\n* `SimpleITK`\n* `pydicom`\n* `pylibjpeg`\n* `Pillow`\n* `openslide-python`\n* `pyvips`\n* `oct-converter`\n\n## Usage\n\n`panimg` takes a folder and tries to convert the containing files to MHA or TIFF.\nBy default, it will try to convert files from subdirectories as well.\nTo only convert files in the top level directory, set `recurse_subdirectories` to `False`.\nIt will try several strategies for loading the contained files, and if an image is found it will output it to the output folder.\nIt will return a structure containing information about what images were produced, what images were used to form the new images, image metadata, and any errors from any of the strategies.\n\n\n**NOTE: Alpha software, do not run this on folders you do not have a backup of.**\n\n```python\nfrom pathlib import Path\nfrom panimg import convert\n\nresult = convert(\n    input_directory=Path("/path/to/files/"),\n    output_directory=Path("/where/files/will/go/"),\n)\n```\n\n### Command Line Interface\n\n`panimg` is also accessible from the command line.\nInstall the package from pip as before, then you can use:\n\n**NOTE: Alpha software, do not run this on folders you do not have a backup of.**\n\n```shell\npanimg convert /path/to/files/ /where/files/will/go/\n```\n\nTo access the help test you can use `panimg -h`.\n\n### Supported Formats\n\n| Input                               | Output  | Strategy   | Notes                      |\n| ----------------------------------- | --------| ---------- | -------------------------- |\n| `.mha`                              | `.mha`  | `metaio`   |                            |\n| `.mhd` with `.raw` or `.zraw`       | `.mha`  | `metaio`   |                            |\n| `.dcm`                              | `.mha`  | `dicom`    |                            |\n| `.nii`                              | `.mha`  | `nifti`    |                            |\n| `.nii.gz`                           | `.mha`  | `nifti`    |                            |\n| `.nrrd`                             | `.mha`  | `nrrd`     | <sup>[1](#footnote1)</sup> |\n| `.e2e`                              | `.mha`  | `oct`      | <sup>[2](#footnote2)</sup> |\n| `.fds`                              | `.mha`  | `oct`      | <sup>[2](#footnote2)</sup> |\n| `.fda`                              | `.mha`  | `oct`      | <sup>[2](#footnote2)</sup> |\n| `.png`                              | `.mha`  | `fallback` | <sup>[3](#footnote3)</sup> |\n| `.jpeg`                             | `.mha`  | `fallback` | <sup>[3](#footnote3)</sup> |\n| `.tiff`                             | `.tiff` | `tiff`     |                            |\n| `.svs` (Aperio)                     | `.tiff` | `tiff`     |                            |\n| `.vms`, `.vmu`, `.ndpi` (Hamamatsu) | `.tiff` | `tiff`     |                            |\n| `.scn` (Leica)                      | `.tiff` | `tiff`     |                            |\n| `.mrxs` (MIRAX)                     | `.tiff` | `tiff`     |                            |\n| `.biff` (Ventana)                   | `.tiff` | `tiff`     |                            |\n\n<a name="footnote1">1</a>: Detached headers are not supported.\n\n<a name="footnote2">2</a>: Only OCT volume(s), no fundus image(s) will be extracted.\n\n<a name="footnote3">3</a>: 2D only, unitary dimensions\n\n#### Post Processors\n\nYou can also define a set of post processors that will operate on each output file.\nPost processors will not produce any new image entities, but rather add additional representations of an image, such as DZI or thumbnails.\nWe provide a `dzi_to_tiff` post processor that is enabled by default, which will produce a DZI file if it is able to.\nTo customise the post processors that run you can do this with\n\n```python\nresult = convert(..., post_processors=[...])\n```\n\nYou are able to run the post processors directly with\n\n```python\nfrom panimg import post_process\nfrom panimg.models import PanImgFile\n\nresult = post_process(image_files={PanImgFile(...), ...}, post_processors=[...])\n```\n\n#### Using Strategies Directly\n\nIf you want to run a particular strategy directly which returns a generator of images for a set of files you can do this with\n\n```python\nfiles = {f for f in Path("/foo/").glob("*.dcm") if f.is_file()}\n\ntry:\n    for result in image_builder_dicom(files=files):\n        sitk_image = result.image\n        process(sitk_image)  # etc. you can also look at result.name for the name of the file,\n                             # and result.consumed_files to see what files were used for this image\nexcept UnconsumedFilesException as e:\n    # e.errors is keyed with a Path to a file that could not be consumed,\n    # with a list of all the errors found with loading it,\n    # the user can then choose what to do with that information\n    ...\n```\n',
     'author': 'James Meakin',
     'author_email': 'panimg@jmsmkn.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/DIAGNijmegen/rse-panimg',
```

### Comparing `panimg-0.9.0/PKG-INFO` & `panimg-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panimg
-Version: 0.9.0
+Version: 0.9.1
 Summary: Conversion of medical images to MHA and TIFF.
 Home-page: https://github.com/DIAGNijmegen/rse-panimg
 License: Apache-2.0
 Author: James Meakin
 Author-email: panimg@jmsmkn.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
```

