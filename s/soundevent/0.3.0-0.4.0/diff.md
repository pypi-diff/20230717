# Comparing `tmp/soundevent-0.3.0.tar.gz` & `tmp/soundevent-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soundevent-0.3.0.tar", last modified: Sun Jul  9 15:05:39 2023, max compression
+gzip compressed data, was "soundevent-0.4.0.tar", last modified: Sun Jul 16 22:12:27 2023, max compression
```

## Comparing `soundevent-0.3.0.tar` & `soundevent-0.4.0.tar`

### file list

```diff
@@ -1,37 +1,48 @@
--rw-r--r--   0        0        0     1084 2023-07-09 15:05:30.648328 soundevent-0.3.0/LICENSE
--rw-r--r--   0        0        0     3164 2023-07-09 15:05:30.648328 soundevent-0.3.0/README.md
--rw-r--r--   0        0        0     1328 2023-07-09 15:05:39.128515 soundevent-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1134 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/__init__.py
--rw-r--r--   0        0        0       60 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/__version__.py
--rw-r--r--   0        0        0      323 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/__init__.py
--rw-r--r--   0        0        0     2939 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/chunks.py
--rw-r--r--   0        0        0     3893 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/io.py
--rw-r--r--   0        0        0     2461 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/media_info.py
--rw-r--r--   0        0        0     2495 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/audio/spectrograms.py
--rw-r--r--   0        0        0     3037 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/__init__.py
--rw-r--r--   0        0        0     2523 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotation_projects.py
--rw-r--r--   0        0        0     3077 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotation_tasks.py
--rw-r--r--   0        0        0     3287 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/annotations.py
--rw-r--r--   0        0        0     2993 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/clips.py
--rw-r--r--   0        0        0     2854 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/dataset.py
--rw-r--r--   0        0        0     2424 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/features.py
--rw-r--r--   0        0        0    17278 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/geometries.py
--rw-r--r--   0        0        0     2102 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/matches.py
--rw-r--r--   0        0        0     2261 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/model_run.py
--rw-r--r--   0        0        0     3002 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/notes.py
--rw-r--r--   0        0        0     2638 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/predicted_sound_events.py
--rw-r--r--   0        0        0     1531 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/predicted_tags.py
--rw-r--r--   0        0        0     2590 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/processed_clip.py
--rw-r--r--   0        0        0     5531 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/recordings.py
--rw-r--r--   0        0        0     2935 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/sequences.py
--rw-r--r--   0        0        0     2574 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/sound_events.py
--rw-r--r--   0        0        0     2624 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/data/tags.py
--rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/src/soundevent/py.typed
--rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/__init__.py
--rw-r--r--   0        0        0      989 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/conftest.py
--rw-r--r--   0        0        0     4678 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/test_audio.py
--rw-r--r--   0        0        0     2691 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_audio/test_spectrograms.py
--rw-r--r--   0        0        0        0 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_data/__init__.py
--rw-r--r--   0        0        0      183 2023-07-09 15:05:30.652328 soundevent-0.3.0/tests/test_soundevent.py
--rw-r--r--   0        0        0     3714 1970-01-01 00:00:00.000000 soundevent-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-16 22:12:17.686308 soundevent-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3805 2023-07-16 22:12:17.686308 soundevent-0.4.0/README.md
+-rw-r--r--   0        0        0     1328 2023-07-16 22:12:27.482298 soundevent-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1134 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/__init__.py
+-rw-r--r--   0        0        0       60 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/__version__.py
+-rw-r--r--   0        0        0      323 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/audio/__init__.py
+-rw-r--r--   0        0        0     2939 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/audio/chunks.py
+-rw-r--r--   0        0        0     3893 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/audio/io.py
+-rw-r--r--   0        0        0     2461 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/audio/media_info.py
+-rw-r--r--   0        0        0     2495 2023-07-16 22:12:17.690308 soundevent-0.4.0/src/soundevent/audio/spectrograms.py
+-rw-r--r--   0        0        0     3037 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/__init__.py
+-rw-r--r--   0        0        0     2680 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/annotation_projects.py
+-rw-r--r--   0        0        0     3458 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/annotation_tasks.py
+-rw-r--r--   0        0        0     3449 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/annotations.py
+-rw-r--r--   0        0        0     3120 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/clips.py
+-rw-r--r--   0        0        0     2878 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/dataset.py
+-rw-r--r--   0        0        0     2424 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/features.py
+-rw-r--r--   0        0        0    17475 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/geometries.py
+-rw-r--r--   0        0        0     2102 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/matches.py
+-rw-r--r--   0        0        0     2261 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/model_run.py
+-rw-r--r--   0        0        0     3002 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/notes.py
+-rw-r--r--   0        0        0     2761 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/predicted_sound_events.py
+-rw-r--r--   0        0        0     1531 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/predicted_tags.py
+-rw-r--r--   0        0        0     2838 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/processed_clip.py
+-rw-r--r--   0        0        0     5665 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/recordings.py
+-rw-r--r--   0        0        0     2935 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/sequences.py
+-rw-r--r--   0        0        0     2762 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/sound_events.py
+-rw-r--r--   0        0        0     2757 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/data/tags.py
+-rw-r--r--   0        0        0      538 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/__init__.py
+-rw-r--r--   0        0        0     3732 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/annotation_projects.py
+-rw-r--r--   0        0        0     4097 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/datasets.py
+-rw-r--r--   0        0        0      764 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/formats/__init__.py
+-rw-r--r--   0        0        0    33111 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/formats/aoef.py
+-rw-r--r--   0        0        0     4135 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/model_runs.py
+-rw-r--r--   0        0        0      913 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/io/types.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:12:17.694308 soundevent-0.4.0/src/soundevent/py.typed
+-rw-r--r--   0        0        0        0 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_audio/__init__.py
+-rw-r--r--   0        0        0      989 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_audio/conftest.py
+-rw-r--r--   0        0        0     4707 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_audio/test_audio.py
+-rw-r--r--   0        0        0     2677 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_audio/test_spectrograms.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_data/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_io/__init__.py
+-rw-r--r--   0        0        0    16187 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_io/test_annotation_projects.py
+-rw-r--r--   0        0        0    10337 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_io/test_datasets.py
+-rw-r--r--   0        0        0     8248 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_io/test_model_runs.py
+-rw-r--r--   0        0        0      183 2023-07-16 22:12:17.694308 soundevent-0.4.0/tests/test_soundevent.py
+-rw-r--r--   0        0        0     4355 1970-01-01 00:00:00.000000 soundevent-0.4.0/PKG-INFO
```

### Comparing `soundevent-0.3.0/LICENSE` & `soundevent-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/README.md` & `soundevent-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,34 @@
+Metadata-Version: 2.1
+Name: soundevent
+Version: 0.4.0
+Summary: soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management.
+Author-Email: Santiago Martinez <santiago.balvanera.20@ucl.ac.uk>
+License: MIT
+Requires-Python: >=3.8
+Requires-Dist: pydantic>=2.0
+Requires-Dist: shapely>=2.0.1
+Requires-Dist: scipy>=1.6.1
+Requires-Dist: xarray>=0.20.2
+Requires-Dist: matplotlib>=3.5.3
+Requires-Dist: cython>=0.29.36
+Description-Content-Type: text/markdown
+
 # soundevent
 
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/soundevent.svg)](https://badge.fury.io/py/soundevent)
+![tests](https://github.com/mbsantiago/soundevent/actions/workflows/test.yml/badge.svg)
+[![docs](https://github.com/mbsantiago/soundevent/actions/workflows/docs.yml/badge.svg)](https://mbsantiago.github.io/soundevent/)
+![Python 3.8 +](https://img.shields.io/badge/python->=_3.8-blue.svg)
+![Static Badge](https://img.shields.io/badge/formatting-black-black)
+[![codecov](https://codecov.io/gh/mbsantiago/soundevent/branch/main/graph/badge.svg?token=42kVE87avA)](https://codecov.io/gh/mbsantiago/soundevent)
+
 > **Warning**
-> This package is under active development use with caution. 
-> However, most of the data definitions are not expected to change. 
-> Will be adding data loading/exporting and prediction evaluation functions soon. 
+> This package is under active development, use with caution.
 
 `soundevent` is an open-source Python package that aims to support the
 computational biocoustic community in developing well-tested, coherent, and
 standardized software tools for bioacoustic analysis. The main goal of the
 package is to provide a flexible yet consistent definition of what a sound event
 is in a computational sense, along with a set of tools to easily work with this
 definition. The package comprises three key components:
@@ -25,18 +46,20 @@
 valid and meaningful. Specifically, it defines objects related to sound events,
 such as user annotations and model predictions.
 
 ### 2. Serialization, Storage, and Reading Functions
 
 To promote standardized data formats for storing annotated datasets and other
 information about sounds in recordings, the `soundevent` package provides
-several functions for serialization, storage, and reading of the different data
-classes offered. These functions enable easy sharing of information about common
-objects in bioacoustic research. By employing a consistent data format,
-researchers can exchange data more efficiently and collaborate seamlessly.
+[several
+functions](https://mbsantiago.github.io/soundevent/generated/gallery/1_saving_and_loading/)
+for serialization, storage, and reading of the different data classes offered.
+These functions enable easy sharing of information about common objects in
+bioacoustic research. By employing a consistent data format, researchers can
+exchange data more efficiently and collaborate seamlessly.
 
 ### 3. Handling Functions for Sound Events
 
 The `soundevent` package also includes a variety of functions that facilitate
 the handling of sound event objects. These functions serve multiple purposes,
 such as matching sound events for model prediction evaluation, transforming
 sound events, and managing metadata and labels. By offering a comprehensive set
```

### Comparing `soundevent-0.3.0/pyproject.toml` & `soundevent-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 profile = "black"
 
 [tool.mypy]
 ignore_missing_imports = true
 
 [project]
 name = "soundevent"
-version = "0.3.0"
+version = "0.4.0"
 description = "soundevent is an open-source Python package for the computational biocoustic community, providing standardized tools for sound event analysis and data management."
 authors = [
     { name = "Santiago Martinez", email = "santiago.balvanera.20@ucl.ac.uk" },
 ]
 dependencies = [
     "pydantic>=2.0",
     "shapely>=2.0.1",
```

### Comparing `soundevent-0.3.0/src/soundevent/__init__.py` & `soundevent-0.4.0/src/soundevent/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
     Geometry,
     GeometryType,
     LineString,
     Match,
     ModelRun,
     MultiLineString,
     MultiPoint,
-    Sequence,
     MultiPolygon,
     Note,
     Point,
     Polygon,
     PredictedSoundEvent,
     PredictedTag,
     ProcessedClip,
     Recording,
+    Sequence,
     SoundEvent,
     Tag,
     Time,
     TimeInterval,
     TimeStamp,
 )
```

### Comparing `soundevent-0.3.0/src/soundevent/audio/chunks.py` & `soundevent-0.4.0/src/soundevent/audio/chunks.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/audio/io.py` & `soundevent-0.4.0/src/soundevent/audio/io.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/audio/media_info.py` & `soundevent-0.4.0/src/soundevent/audio/media_info.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/audio/spectrograms.py` & `soundevent-0.4.0/src/soundevent/audio/spectrograms.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/__init__.py` & `soundevent-0.4.0/src/soundevent/data/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
 
 from soundevent.data.annotation_projects import AnnotationProject
 from soundevent.data.annotation_tasks import AnnotationTask
 from soundevent.data.annotations import Annotation
 from soundevent.data.clips import Clip
 from soundevent.data.dataset import Dataset
 from soundevent.data.features import Feature
-from soundevent.data.sequences import Sequence
 from soundevent.data.geometries import (
     MAX_FREQUENCY,
     BoundingBox,
     Frequency,
     Geometry,
     GeometryType,
     LineString,
@@ -56,14 +55,15 @@
 from soundevent.data.matches import Match
 from soundevent.data.model_run import ModelRun
 from soundevent.data.notes import Note
 from soundevent.data.predicted_sound_events import PredictedSoundEvent
 from soundevent.data.predicted_tags import PredictedTag
 from soundevent.data.processed_clip import ProcessedClip
 from soundevent.data.recordings import Recording
+from soundevent.data.sequences import Sequence
 from soundevent.data.sound_events import SoundEvent
 from soundevent.data.tags import Tag
 
 __all__ = [
     "Annotation",
     "AnnotationProject",
     "AnnotationTask",
```

### Comparing `soundevent-0.3.0/src/soundevent/data/annotation_projects.py` & `soundevent-0.4.0/src/soundevent/data/annotation_projects.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,18 +44,21 @@
 
 from soundevent.data.annotation_tasks import AnnotationTask
 
 
 class AnnotationProject(BaseModel):
     """Annotation collection."""
 
-    id: UUID = Field(default_factory=uuid4)
+    id: UUID = Field(default_factory=uuid4, repr=False)
     """Unique identifier for the annotation collection."""
 
     name: str
     """Name of the annotation project."""
 
-    description: Optional[str] = None
+    description: Optional[str] = Field(default=None, repr=False)
     """Description of the annotation collection."""
 
-    tasks: List[AnnotationTask] = Field(default_factory=list)
+    tasks: List[AnnotationTask] = Field(default_factory=list, repr=False)
     """List of annotation tasks in the project."""
+
+    instructions: Optional[str] = Field(default=None, repr=False)
+    """Instructions for annotators."""
```

### Comparing `soundevent-0.3.0/src/soundevent/data/annotation_tasks.py` & `soundevent-0.4.0/src/soundevent/data/annotation_tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,37 +43,49 @@
 tasks, extract relevant information, and perform analyses based on the
 completed annotations. Utilizing the `AnnotationTask` class facilitates
 effective management and processing of annotation tasks, ultimately
 enabling comprehensive analysis of audio recordings in bioacoustic
 research projects.
 
 """
+import datetime
 from typing import List, Optional
+from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.annotations import Annotation
 from soundevent.data.clips import Clip
 from soundevent.data.notes import Note
 from soundevent.data.tags import Tag
 
 
 class AnnotationTask(BaseModel):
     """Annotation task."""
 
+    id: UUID = Field(default_factory=uuid4)
+    """Unique identifier for the annotation task."""
+
     clip: Clip
     """The annotated clip."""
 
     annotations: List[Annotation] = Field(default_factory=list)
     """List of annotations in the created during the annotation task."""
 
     completed_by: Optional[str] = None
     """The user who completed the annotation task."""
 
+    completed_on: Optional[datetime.datetime] = None
+    """The date and time when the annotation task was completed."""
+
     notes: List[Note] = Field(default_factory=list)
     """Notes associated with the annotation task."""
 
     tags: List[Tag] = Field(default_factory=list)
     """User provided tags to the annotated clip."""
 
     completed: bool = False
     """Whether the annotation task has been completed."""
+
+    def __hash__(self):
+        """Compute the hash value for the annotation task."""
+        return hash(self.id)
```

### Comparing `soundevent-0.3.0/src/soundevent/data/annotations.py` & `soundevent-0.4.0/src/soundevent/data/annotations.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,29 +58,33 @@
     "Annotation",
 ]
 
 
 class Annotation(BaseModel):
     """Annotation."""
 
-    id: UUID = Field(default_factory=uuid4)
+    id: UUID = Field(default_factory=uuid4, repr=False)
     """A unique identifier for the annotation."""
 
     created_by: Optional[str] = None
     """The user who created the annotation."""
 
     sound_event: SoundEvent
     """The sound event being annotated."""
 
-    notes: List[Note] = Field(default_factory=list)
+    notes: List[Note] = Field(default_factory=list, repr=False)
     """Notes associated with the annotation."""
 
-    tags: List[Tag] = Field(default_factory=list)
+    tags: List[Tag] = Field(default_factory=list, repr=False)
     """User provided tags to the annotated sound event."""
 
-    created_on: datetime.datetime = Field(
-        default_factory=datetime.datetime.now
+    created_on: Optional[datetime.datetime] = Field(
+        default_factory=datetime.datetime.now, repr=False
     )
     """The time at which the annotation was created.
 
     Important for tracking the progress of an annotation task.
     """
+
+    def __hash__(self):
+        """Compute the hash of the annotation."""
+        return hash(self.id)
```

### Comparing `soundevent-0.3.0/src/soundevent/data/clips.py` & `soundevent-0.4.0/src/soundevent/data/clips.py`

 * *Files 3% similar despite different names*

```diff
@@ -53,31 +53,35 @@
     "Clip",
 ]
 
 
 class Clip(BaseModel):
     """Clip model."""
 
+    uuid: UUID = Field(default_factory=uuid4)
+    """The unique identifier of the clip."""
+
     recording: Recording
     """The recording that the clip belongs to."""
 
     start_time: float
     """The start time of the clip in seconds."""
 
     end_time: float
     """The end time of the clip in seconds."""
 
-    uuid: UUID = Field(default_factory=uuid4)
-    """The unique identifier of the clip."""
-
     tags: List[Tag] = Field(default_factory=list)
     """List of tags associated with the clip."""
 
     features: List[Feature] = Field(default_factory=list)
     """List of features associated with the clip."""
 
     @model_validator(mode="before")
     def validate_times(cls, values):
         """Validate that start_time < end_time."""
         if values["start_time"] > values["end_time"]:
             raise ValueError("start_time must be less than end_time")
         return values
+
+    def __hash__(self):
+        """Hash clip object."""
+        return hash((self.recording, self.start_time, self.end_time))
```

### Comparing `soundevent-0.3.0/src/soundevent/data/dataset.py` & `soundevent-0.4.0/src/soundevent/data/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,18 +58,18 @@
 
 from soundevent.data.recordings import Recording
 
 
 class Dataset(BaseModel):
     """Datasets."""
 
-    id: UUID = Field(default_factory=uuid4)
+    id: UUID = Field(default_factory=uuid4, repr=False)
     """The unique identifier of the dataset."""
 
     name: str
     """The name of the dataset."""
 
     description: Optional[str] = None
     """A description of the dataset."""
 
-    recordings: List[Recording] = Field(default_factory=list)
+    recordings: List[Recording] = Field(default_factory=list, repr=False)
     """List of recordings associated with the dataset."""
```

### Comparing `soundevent-0.3.0/src/soundevent/data/features.py` & `soundevent-0.4.0/src/soundevent/data/features.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/geometries.py` & `soundevent-0.4.0/src/soundevent/data/geometries.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,19 +49,19 @@
 
 By offering these geometry types, the soundevent package provides a
 comprehensive framework for accurately and flexibly describing the
 location and extent of sound events within a recording.
 """
 import sys
 from abc import ABC, abstractmethod
-from typing import List, Tuple
+from typing import List, Tuple, Union
 
-from pydantic import BaseModel, ConfigDict, Field, PrivateAttr, field_validator
+from pydantic import BaseModel, Field, PrivateAttr, field_validator
 from shapely import geometry
-from shapely.geometry.base import BaseGeometry
+import shapely.geometry.base as shapely
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 __all__ = [
@@ -99,34 +99,36 @@
 Frequency = float
 """Frequency in Hertz."""
 
 MAX_FREQUENCY = 5_000_000
 """The absolute maximum frequency that can be used in a geometry."""
 
 
-class Geometry(BaseModel, ABC):
+class BaseGeometry(BaseModel, ABC):
     """Base class for geometries.
 
     Notes
     -----
     Mutation of geometry objects is not allowed. This is to ensure that the
     geometry object is always in sync with the Shapely geometry object.
     """
 
-    model_config = ConfigDict(
-        arbitrary_types_allowed=True,
+    type: str = Field(
+        description="the type of geometry used to locate the sound event.",
         frozen=True,
+        include=True,
     )
 
-    type: GeometryType = Field(
-        ...,
-        description="the type of geometry used to locate the sound event.",
+    coordinates: Union[float, List, Tuple] = Field(
+        description="the coordinates of the geometry.",
+        frozen=True,
+        include=True,
     )
 
-    _geom: BaseGeometry = PrivateAttr()
+    _geom: shapely.BaseGeometry = PrivateAttr()
     """The Shapely geometry object representing the geometry."""
 
     @classmethod
     def geom_type(cls) -> str:
         """Get the geometry type.
 
         Returns
@@ -134,15 +136,15 @@
         str
             The Shapely geometry type.
         """
         type_field = cls.model_fields["type"]
         return type_field.default
 
     @property
-    def geom(self) -> BaseGeometry:
+    def geom(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return self._geom
@@ -160,70 +162,69 @@
 
     def __init__(self, **data):
         """Initialize the geometry."""
         super().__init__(**data)
         self._geom = self._get_shapely_geometry()
 
     @abstractmethod
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         raise NotImplementedError
 
 
-class TimeStamp(Geometry):
+class TimeStamp(BaseGeometry):
     """TimeStamp geometry type.
 
     This geometry type is used to locate a sound event with a single time stamp.
     Useful for very short sound events that are not well represented by a
     time interval.
     """
 
-    type: Literal["TimeStamp"] = "TimeStamp"
+    type: str = "TimeStamp"
 
     coordinates: Time = Field(
         ...,
         description="The time stamp of the sound event.",
     )
     """The time stamp of the sound event.
 
     The time stamp is relative to the start of the recording.
     """
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return geometry.box(
             self.coordinates,
             0,
             self.coordinates,
             MAX_FREQUENCY,
         )
 
 
-class TimeInterval(Geometry):
+class TimeInterval(BaseGeometry):
     """TimeInterval geometry type.
 
     This geometry type is used to locate a sound event with a time interval.
     Useful for sound events that have a clear start and end time, but that do
     not have a clear frequency range.
     """
 
-    type: Literal["TimeInterval"] = "TimeInterval"
+    type: str = "TimeInterval"
 
     coordinates: Tuple[Time, Time] = Field(
-        ...,
         description="The time interval of the sound event.",
     )
     """The time interval of the sound event.
 
     The time interval is relative to the start of the recording.
     """
 
@@ -245,75 +246,75 @@
             ValueError: If the time interval is invalid (i.e. the start time is
                 after the end time).
         """
         if v[0] > v[1]:
             raise ValueError("The start time must be before the end time.")
         return v
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the sound event.
 
         Returns
         -------
             The Shapely geometry object representing the sound event.
         """
         start_time, end_time = self.coordinates
         return geometry.box(start_time, 0, end_time, MAX_FREQUENCY)
 
 
-class Point(Geometry):
+class Point(BaseGeometry):
     """Point geometry type.
 
     This geometry type is used to locate a sound event with a single point in
     time and frequency.
     """
 
-    type: Literal["Point"] = "Point"
+    type: str = "Point"
 
     coordinates: Tuple[Time, Frequency] = Field(
         ...,
         description="The points of the sound event.",
     )
     """The points of the sound event.
 
     The time is relative to the start of the recording.
 
     """
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return geometry.Point(self.coordinates)
 
 
-class LineString(Geometry):
+class LineString(BaseGeometry):
     """LineString geometry type.
 
     This geometry type is used to locate a sound event with a line in time and
     frequency. Useful to lcoate with detail sounds that have a clear frequency
     trajectory.
     """
 
-    type: Literal["LineString"] = "LineString"
+    type: str = "LineString"
 
     coordinates: List[Tuple[Time, Frequency]] = Field(
         ...,
         description="The line of the sound event.",
     )
     """The line of the sound event.
 
     Each line should be ordered by time.
 
     All times are relative to the start of the recording."""
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return geometry.LineString(self.coordinates)
@@ -333,23 +334,23 @@
     ) -> List[Tuple[Time, Frequency]]:
         """Validate that the line is ordered by time."""
         if not all(v[i][0] <= v[i + 1][0] for i in range(len(v) - 1)):
             raise ValueError("The line must be ordered by time.")
         return v
 
 
-class Polygon(Geometry):
+class Polygon(BaseGeometry):
     """Polygon geometry type.
 
     This geometry type is used to locate a sound event with a polygon in time
     and frequency. Useful to locate with detail sounds that have a clear
     frequency trajectory and that are bounded by a clear start and end time.
     """
 
-    type: Literal["Polygon"] = "Polygon"
+    type: str = "Polygon"
 
     coordinates: List[List[Tuple[Time, Frequency]]] = Field(
         ...,
         description="The polygon of the sound event.",
     )
     """The polygon of the sound event.
 
@@ -360,35 +361,35 @@
         cls, v: List[List[Tuple[Time, Frequency]]]
     ) -> List[List[Tuple[Time, Frequency]]]:
         """Validate that the polygon has at least one ring."""
         if len(v) == 0:
             raise ValueError("The polygon must have at least one ring.")
         return v
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         shell = self.coordinates[0]
         holes = self.coordinates[1:]
         return geometry.Polygon(shell, holes)
 
 
-class BoundingBox(Geometry):
+class BoundingBox(BaseGeometry):
     """BoundingBox geometry type.
 
     This geometry type is used to locate a sound event with a bounding box in
     time and frequency. Useful to locate sounds that have a clear frequency
     range and start and stop times.
     """
 
-    type: Literal["BoundingBox"] = "BoundingBox"
+    type: str = "BoundingBox"
 
     coordinates: Tuple[Time, Frequency, Time, Frequency] = Field(
         ...,
         description="The bounding box of the sound event.",
     )
     """The bounding box of the sound event.
 
@@ -408,73 +409,73 @@
         if v[1] > v[3]:
             raise ValueError(
                 "The start frequency must be before the end frequency."
             )
 
         return v
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry."""
         start_time, start_frequency, end_time, end_frequency = self.coordinates
         return geometry.box(
             start_time,
             start_frequency,
             end_time,
             end_frequency,
         )
 
 
-class MultiPoint(Geometry):
+class MultiPoint(BaseGeometry):
     """MultiPoint geometry type.
 
     This geometry type is used to locate a sound event with multiple points in
     time and frequency. Useful to locate multiple interesting points that
     together form a sound event.
     """
 
-    type: Literal["MultiPoint"] = "MultiPoint"
+    type: str = "MultiPoint"
 
     coordinates: List[Tuple[Time, Frequency]] = Field(
         ...,
         description="The points of the sound event.",
     )
     """The points of the sound event.
 
     All times are relative to the start of the recording."""
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return geometry.MultiPoint(self.coordinates)
 
 
-class MultiLineString(Geometry):
+class MultiLineString(BaseGeometry):
     """MultiLineString geometry type.
 
     This geometry type is used to locate a sound event with multiple lines in
     time and frequency. Useful to locate multiple interesting lines that
     together form a sound event. For example, a sound event that has multiple
     harmonics.
     """
 
-    type: Literal["MultiLineString"] = "MultiLineString"
+    type: str = "MultiLineString"
 
     coordinates: List[List[Tuple[Time, Frequency]]] = Field(
         ...,
         description="The lines of the sound event.",
     )
     """The lines of the sound event.
 
     All times are relative to the start of the recording."""
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         return geometry.MultiLineString(self.coordinates)
@@ -506,25 +507,25 @@
             if not all(
                 line[i][0] <= line[i + 1][0] for i in range(len(line) - 1)
             ):
                 raise ValueError("Each line must be ordered by time.")
         return v
 
 
-class MultiPolygon(Geometry):
+class MultiPolygon(BaseGeometry):
     """MultiPolygon geometry type.
 
     This geometry type is used to locate a sound event with multiple polygons in
     time and frequency. Useful to locate multiple interesting polygons that
     together form a sound event. For example sound events that have been
     occluded by other sound events and that are therefore split into multiple
     polygons.
     """
 
-    type: Literal["MultiPolygon"] = "MultiPolygon"
+    type: str = "MultiPolygon"
 
     coordinates: List[List[List[Tuple[Time, Frequency]]]] = Field(
         ...,
         description="The polygons of the sound event.",
     )
     """The polygons of the sound event.
 
@@ -547,21 +548,34 @@
     ) -> List[List[List[Tuple[Time, Frequency]]]]:
         """Validate that each polygon has at least one ring."""
         for polygon in v:
             if len(polygon) == 0:
                 raise ValueError("Each polygon must have at least one ring.")
         return v
 
-    def _get_shapely_geometry(self) -> BaseGeometry:
+    def _get_shapely_geometry(self) -> shapely.BaseGeometry:
         """Get the Shapely geometry object representing the geometry.
 
         Returns
         -------
             The Shapely geometry object representing the geometry.
         """
         polgons = []
         for poly in self.coordinates:
             shell = poly[0]
             holes = poly[1:]
             polygon = geometry.Polygon(shell, holes)
             polgons.append(polygon)
         return geometry.MultiPolygon(polgons)
+
+
+Geometry = Union[
+    TimeStamp,
+    TimeInterval,
+    Point,
+    LineString,
+    Polygon,
+    BoundingBox,
+    MultiPoint,
+    MultiLineString,
+    MultiPolygon,
+]
```

### Comparing `soundevent-0.3.0/src/soundevent/data/matches.py` & `soundevent-0.4.0/src/soundevent/data/matches.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/model_run.py` & `soundevent-0.4.0/src/soundevent/data/model_run.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/notes.py` & `soundevent-0.4.0/src/soundevent/data/notes.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/predicted_sound_events.py` & `soundevent-0.4.0/src/soundevent/data/predicted_sound_events.py`

 * *Files 15% similar despite different names*

```diff
@@ -65,7 +65,11 @@
     """The probability score of the predicted sound event."""
 
     tags: List[PredictedTag] = Field(default_factory=list)
     """List of predicted tags associated with the prediction."""
 
     features: List[Feature] = Field(default_factory=list)
     """List of features associated with the prediction."""
+
+    def __hash__(self) -> int:
+        """Return hash value of the predicted sound event."""
+        return hash(self.id)
```

### Comparing `soundevent-0.3.0/src/soundevent/data/predicted_tags.py` & `soundevent-0.4.0/src/soundevent/data/predicted_tags.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/processed_clip.py` & `soundevent-0.4.0/src/soundevent/data/processed_clip.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,30 +31,38 @@
 
 The predicted sound events within the `ProcessedClip` object can be further
 enriched with tags and/or features associated with each predicted sound event.
 These annotations and additional information provide more detailed insights
 into the predicted events and aid in subsequent analysis and interpretation.
 """
 from typing import List
+from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.clips import Clip
 from soundevent.data.features import Feature
 from soundevent.data.predicted_sound_events import PredictedSoundEvent
 from soundevent.data.predicted_tags import PredictedTag
 
 
 class ProcessedClip(BaseModel):
     """Processed clip."""
 
+    uuid: UUID = Field(default_factory=uuid4, repr=False)
+    """Unique identifier for the processed clip."""
+
     clip: Clip
     """The clip that was processed."""
 
     sound_events: List[PredictedSoundEvent] = Field(default_factory=list)
     """List of predicted sound events."""
 
     tags: List[PredictedTag] = Field(default_factory=list)
     """List of predicted tags at the clip level."""
 
     features: List[Feature] = Field(default_factory=list)
     """List of features associated with the clip."""
+
+    def __hash__(self):
+        """Hash function for the processed clip."""
+        return hash(self.uuid)
```

### Comparing `soundevent-0.3.0/src/soundevent/data/recordings.py` & `soundevent-0.4.0/src/soundevent/data/recordings.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 related fields.
 """
 
 import datetime
 import os
 from pathlib import Path
 from typing import List, Optional
+from uuid import UUID, uuid4
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.features import Feature
 from soundevent.data.notes import Note
 from soundevent.data.tags import Tag
 
@@ -64,14 +65,17 @@
     "Recording",
 ]
 
 
 class Recording(BaseModel):
     """Recordings."""
 
+    id: UUID = Field(default_factory=uuid4, repr=False)
+    """The unique identifier of the recording."""
+
     path: Path
     """The path to the audio file."""
 
     duration: float
     """The duration of the audio file in seconds.
 
     The duration of the audio file is adjusted by the time expansion
@@ -117,15 +121,15 @@
     """A list of features associated with the recording."""
 
     notes: List[Note] = Field(default_factory=list, repr=False)
     """A list of notes associated with the recording."""
 
     def __hash__(self):
         """Hash function."""
-        return hash(self.hash)
+        return hash(self.id)
 
     @classmethod
     def from_file(
         cls,
         path: os.PathLike,
         time_expansion: float = 1,
         **kwargs,
```

### Comparing `soundevent-0.3.0/src/soundevent/data/sequences.py` & `soundevent-0.4.0/src/soundevent/data/sequences.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/src/soundevent/data/sound_events.py` & `soundevent-0.4.0/src/soundevent/data/sound_events.py`

 * *Files 14% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 provide quantitative information about the sound events, such as
 duration, bandwidth, peak frequency, and other detailed measurements
 that can be extracted using advanced techniques like deep learning
 models. Features offer valuable insights into the acoustic properties
 of the sound events.
 """
 
+from typing import List, Optional
 from uuid import UUID, uuid4
-from typing import List
 
 from pydantic import BaseModel, Field
 
 from soundevent.data.features import Feature
 from soundevent.data.geometries import Geometry
 from soundevent.data.recordings import Recording
 from soundevent.data.tags import Tag
@@ -50,21 +50,25 @@
     "SoundEvent",
 ]
 
 
 class SoundEvent(BaseModel):
     """Sound events."""
 
-    uuid: UUID = Field(default_factory=uuid4)
+    uuid: UUID = Field(default_factory=uuid4, repr=False)
     """The UUID of the sound event."""
 
-    recording: Recording
+    recording: Recording = Field(..., repr=False)
     """The recording containing the sound event."""
 
-    geometry: Geometry
+    geometry: Optional[Geometry]
     """The geometry locating the sound event within the recording."""
 
-    tags: List[Tag] = Field(default_factory=list)
+    tags: List[Tag] = Field(default_factory=list, repr=False)
     """The tags associated with the sound event."""
 
-    features: List[Feature] = Field(default_factory=list)
+    features: List[Feature] = Field(default_factory=list, repr=False)
     """The features associated with the sound event."""
+
+    def __hash__(self):
+        """Compute the hash of the sound event."""
+        return hash(self.uuid)
```

### Comparing `soundevent-0.3.0/src/soundevent/data/tags.py` & `soundevent-0.4.0/src/soundevent/data/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,7 +61,11 @@
 
     value: str
     """The value of the tag."""
 
     def __hash__(self):
         """Hash the Tag object."""
         return hash((self.key, self.value))
+
+    def __str__(self):
+        """Return the string representation of the Tag object."""
+        return f"{self.key}: {self.value}"
```

### Comparing `soundevent-0.3.0/tests/test_audio/conftest.py` & `soundevent-0.4.0/tests/test_audio/conftest.py`

 * *Files identical despite different names*

### Comparing `soundevent-0.3.0/tests/test_audio/test_audio.py` & `soundevent-0.4.0/tests/test_audio/test_audio.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Test suite for audio loading functions."""
 from pathlib import Path
 
 import numpy as np
+from uuid import uuid4
 import pytest
 import xarray as xr
 from hypothesis import HealthCheck, given, settings
 from hypothesis import strategies as st
 from scipy.io import wavfile
 
 from soundevent import data
@@ -80,15 +81,15 @@
     # Arrange
 
     # Create a random wav for an audio of 2 seconds.
     samples = int(np.floor(samplerate * 2))
     wav = np.random.random((samples, channels)).astype(np.float32)
 
     # Save the wav to a file
-    path = tmp_path / "test.wav"
+    path = tmp_path / f"{uuid4()}.wav"
 
     # Save the wav with the adjusted samplerate
     adjusted_samplerate = int(np.floor(samplerate / time_expansion))
     wavfile.write(path, adjusted_samplerate, wav)
 
     recording = data.Recording(
         path=path,
```

### Comparing `soundevent-0.3.0/tests/test_audio/test_spectrograms.py` & `soundevent-0.4.0/tests/test_audio/test_spectrograms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """Test suite for spectrograms functions."""
 
 import numpy as np
-import pytest
 import xarray as xr
 
 from soundevent import audio, data
 
 
 def test_compute_spectrograms_from_recordings(random_wav):
     """Test computing spectrograms from a random recording."""
```

