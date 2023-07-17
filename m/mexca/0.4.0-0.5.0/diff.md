# Comparing `tmp/mexca-0.4.0.tar.gz` & `tmp/mexca-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mexca-0.4.0.tar", last modified: Wed Apr 26 15:06:49 2023, max compression
+gzip compressed data, was "mexca-0.5.0.tar", last modified: Mon Jul 17 15:17:12 2023, max compression
```

## Comparing `mexca-0.4.0.tar` & `mexca-0.5.0.tar`

### file list

```diff
@@ -1,45 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.101131 mexca-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-26 15:06:04.000000 mexca-0.4.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-26 15:06:04.000000 mexca-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-26 15:06:04.000000 mexca-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-26 15:06:04.000000 mexca-0.4.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-26 15:06:49.101131 mexca-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8987 2023-04-26 15:06:04.000000 mexca-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.081131 mexca-0.4.0/mexca/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.085131 mexca-0.4.0/mexca/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23559 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    67298 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/audio/identification.py
--rw-r--r--   0 runner    (1001) docker     (123)    11966 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    28611 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     9526 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.085131 mexca-0.4.0/mexca/text/
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9655 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/text/transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28529 2023-04-26 15:06:04.000000 mexca-0.4.0/mexca/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.081131 mexca-0.4.0/mexca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9997 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:06:17.000000 mexca-0.4.0/mexca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-26 15:06:49.000000 mexca-0.4.0/mexca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-04-26 15:06:04.000000 mexca-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-26 15:06:49.101131 mexca-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-26 15:06:04.000000 mexca-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:06:49.101131 mexca-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    15766 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_audio_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_text_sentiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_text_transcription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-26 15:06:04.000000 mexca-0.4.0/tests/test_video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.596119 mexca-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-17 15:16:41.000000 mexca-0.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-07-17 15:16:41.000000 mexca-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-17 15:16:41.000000 mexca-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-17 15:16:41.000000 mexca-0.5.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-17 15:17:12.600119 mexca-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-17 15:16:41.000000 mexca-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.592119 mexca-0.5.0/mexca/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.596119 mexca-0.5.0/mexca/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24845 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/audio/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68329 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/audio/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5229 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/audio/identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11829 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31864 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9724 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.596119 mexca-0.5.0/mexca/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/text/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5710 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/text/sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/text/transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7888 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.596119 mexca-0.5.0/mexca/video/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8079 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/anfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29270 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/mefarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11183 2023-07-17 15:16:41.000000 mexca-0.5.0/mexca/video/mefl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.592119 mexca-0.5.0/mexca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:16:48.000000 mexca-0.5.0/mexca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:17:12.000000 mexca-0.5.0/mexca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-17 15:16:41.000000 mexca-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-07-17 15:17:12.600119 mexca-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 15:16:41.000000 mexca-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:17:12.596119 mexca-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_audio_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16722 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_audio_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_audio_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10002 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_text_sentiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_text_transcription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2741 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_video_anfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8306 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_video_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_video_helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_video_mefarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-07-17 15:16:41.000000 mexca-0.5.0/tests/test_video_mefl.py
```

### Comparing `mexca-0.4.0/CITATION.cff` & `mexca-0.5.0/CITATION.cff`

 * *Files 16% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     orcid: "https://orcid.org/0000-0002-1330-0585"
   - family-names: Pipal
     given-names: Christian
     orcid: "https://orcid.org/0000-0002-5395-2035"
   - family-names: Schumacher
     given-names: Gijs
     orcid: "https://orcid.org/0000-0002-6503-4514"
-date-released: 2023-04-26
+date-released: 2023-07-17
 doi: 10.5281/zenodo.6976414
-version: "0.4.0"
+version: "0.5.0"
 repository-code: "https://github.com/mexca/mexca"
 keywords:
   - emotion
   - multimodal
   - expression
 message: "If you use this software, please cite it using these metadata."
 license: Apache-2.0
```

### Comparing `mexca-0.4.0/LICENSE` & `mexca-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mexca-0.4.0/PKG-INFO` & `mexca-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 0.4.0
+Version: 0.5.0
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: <3.11,>3.7
 Description-Content-Type: text/markdown
 Provides-Extra: vid
 Provides-Extra: spe
 Provides-Extra: voi
 Provides-Extra: tra
 Provides-Extra: sen
 Provides-Extra: all
@@ -40,27 +40,28 @@
 [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=mexca_mexca&metric=coverage)](https://sonarcloud.io/dashboard?id=mexca_mexca)
 [![build](https://github.com/mexca/mexca/actions/workflows/build.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/build.yml)
 [![cffconvert](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml)
 [![markdown-link-check](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml)
 [![DOI](https://zenodo.org/badge/500818250.svg)](https://zenodo.org/badge/latestdoi/500818250)
 [![docker hub badge](https://img.shields.io/static/v1?label=Docker%20Hub&message=mexca&color=blue&style=flat&logo=docker)](https://hub.docker.com/u/mexca)
 [![docker build badge](https://img.shields.io/github/actions/workflow/status/mexca/mexca/docker.yml?label=Docker%20build&logo=docker)](https://github.com/mexca/mexca/actions/workflows/docker.yml)
+[![black code style badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 <div align="center">
 <img src="mexca_logo.png">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
 ## How To Use Mexca
 
-mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos. 
-It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text). 
-The blocks can also be integrated into a single pipeline to extract the features from all modalities at once. 
-Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations. 
+mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
+It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
+The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
+Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
 
 Please cite mexca if you use it for scientific or commercial purposes.
 
 <div align="center">
 <img src="docs/mexca_flowchart.svg" width="600">
 </div>
@@ -73,16 +74,16 @@
 The package contains five components that must be explicitly installed [^1]. By default, only the base package is installed
 (which requires only a few dependencies). The components can still be used through Docker containers which must be downloaded
 from Docker Hub. We recommend this setup for users with little experience with installing Python packages or who simply want to
 quickly try out the package. Using the containers also adds stability to your program.
 
 ### Requirements
 
-mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing), 
-which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails, 
+mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing),
+which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails,
 it must be installed manually.
 
 To download and run the components as Docker containers, Docker must be installed on your system. Instructions on how to install
 Docker Desktop can be found [here](https://www.docker.com/get-started/).
 
 All components but the VoiceExtractor depend on PyTorch (version 1.12). Usually, it should be automatically installed when specifying any
 of these components. In case the installation fails, see the installation instructions on the PyTorch [web page](https://pytorch.org/get-started/locally/).
@@ -131,17 +132,21 @@
 If you would like to learn how to use mexca, take a look at our [example](https://github.com/mexca/mexca/tree/main/examples) notebook.
 
 *Note*: mexca builds on pretrained models from the pyannote.audio package. Since release 2.1.1, downloading the pretrained models requires the user to accept two user agreements on Hugging Face hub and generate an authentication token. Therefore, to run the mexca pipeline, please accept the user agreements on [here](https://huggingface.co/pyannote/speaker-diarization) and [here](https://huggingface.co/pyannote/segmentation). Then, generate an authentication token [here](https://huggingface.co/settings/tokens). Use this token to login to Hugging Face hub by running `notebook_login()` (from a jupyter notebook) or `huggingface-cli login` (from the command line). You only need to login when running mexca for the first time. See this [link](https://huggingface.co/docs/hub/models-adding-libraries) for details. When running container components, you need to supply the token excplicitly as value for the `use_auth_token` argument. We recommend storing the token on your system and accessing it from Python.
 
 To create and apply the MEXCA pipeline with container components to a video file run the following code in a Jupyter notebook or a Python script (requires the base package and Docker):
 
 ```python
-from mexca.container import (AudioTranscriberContainer, FaceExtractorContainer,
-                             SentimentExtractorContainer, SpeakerIdentifierContainer, 
-                             VoiceExtractorContainer)
+from mexca.container import (
+    AudioTranscriberContainer,
+    FaceExtractorContainer,
+    SentimentExtractorContainer,
+    SpeakerIdentifierContainer,
+    VoiceExtractorContainer,
+)
 from mexca.pipeline import Pipeline
 
 # Set path to video file
 filepath = 'path/to/video'
 
 # Create standard pipeline with two faces and speakers
 pipeline = Pipeline(
```

### Comparing `mexca-0.4.0/README.md` & `mexca-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=mexca_mexca&metric=coverage)](https://sonarcloud.io/dashboard?id=mexca_mexca)
 [![build](https://github.com/mexca/mexca/actions/workflows/build.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/build.yml)
 [![cffconvert](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml)
 [![markdown-link-check](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml)
 [![DOI](https://zenodo.org/badge/500818250.svg)](https://zenodo.org/badge/latestdoi/500818250)
 [![docker hub badge](https://img.shields.io/static/v1?label=Docker%20Hub&message=mexca&color=blue&style=flat&logo=docker)](https://hub.docker.com/u/mexca)
 [![docker build badge](https://img.shields.io/github/actions/workflow/status/mexca/mexca/docker.yml?label=Docker%20build&logo=docker)](https://github.com/mexca/mexca/actions/workflows/docker.yml)
+[![black code style badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 <div align="center">
 <img src="mexca_logo.png">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
 ## How To Use Mexca
 
-mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos. 
-It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text). 
-The blocks can also be integrated into a single pipeline to extract the features from all modalities at once. 
-Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations. 
+mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
+It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
+The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
+Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
 
 Please cite mexca if you use it for scientific or commercial purposes.
 
 <div align="center">
 <img src="docs/mexca_flowchart.svg" width="600">
 </div>
@@ -42,16 +43,16 @@
 The package contains five components that must be explicitly installed [^1]. By default, only the base package is installed
 (which requires only a few dependencies). The components can still be used through Docker containers which must be downloaded
 from Docker Hub. We recommend this setup for users with little experience with installing Python packages or who simply want to
 quickly try out the package. Using the containers also adds stability to your program.
 
 ### Requirements
 
-mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing), 
-which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails, 
+mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing),
+which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails,
 it must be installed manually.
 
 To download and run the components as Docker containers, Docker must be installed on your system. Instructions on how to install
 Docker Desktop can be found [here](https://www.docker.com/get-started/).
 
 All components but the VoiceExtractor depend on PyTorch (version 1.12). Usually, it should be automatically installed when specifying any
 of these components. In case the installation fails, see the installation instructions on the PyTorch [web page](https://pytorch.org/get-started/locally/).
@@ -100,17 +101,21 @@
 If you would like to learn how to use mexca, take a look at our [example](https://github.com/mexca/mexca/tree/main/examples) notebook.
 
 *Note*: mexca builds on pretrained models from the pyannote.audio package. Since release 2.1.1, downloading the pretrained models requires the user to accept two user agreements on Hugging Face hub and generate an authentication token. Therefore, to run the mexca pipeline, please accept the user agreements on [here](https://huggingface.co/pyannote/speaker-diarization) and [here](https://huggingface.co/pyannote/segmentation). Then, generate an authentication token [here](https://huggingface.co/settings/tokens). Use this token to login to Hugging Face hub by running `notebook_login()` (from a jupyter notebook) or `huggingface-cli login` (from the command line). You only need to login when running mexca for the first time. See this [link](https://huggingface.co/docs/hub/models-adding-libraries) for details. When running container components, you need to supply the token excplicitly as value for the `use_auth_token` argument. We recommend storing the token on your system and accessing it from Python.
 
 To create and apply the MEXCA pipeline with container components to a video file run the following code in a Jupyter notebook or a Python script (requires the base package and Docker):
 
 ```python
-from mexca.container import (AudioTranscriberContainer, FaceExtractorContainer,
-                             SentimentExtractorContainer, SpeakerIdentifierContainer, 
-                             VoiceExtractorContainer)
+from mexca.container import (
+    AudioTranscriberContainer,
+    FaceExtractorContainer,
+    SentimentExtractorContainer,
+    SpeakerIdentifierContainer,
+    VoiceExtractorContainer,
+)
 from mexca.pipeline import Pipeline
 
 # Set path to video file
 filepath = 'path/to/video'
 
 # Create standard pipeline with two faces and speakers
 pipeline = Pipeline(
@@ -156,8 +161,8 @@
 
 ## Credits
 
 Mexca is being developed by the [Netherlands eScience Center](https://www.esciencecenter.nl/) in collaboration with the [Hot Politics Lab](http://www.hotpolitics.eu/) at the University of Amsterdam.
 
 This package was created with [Cookiecutter](https://github.com/audreyr/cookiecutter) and the [NLeSC/python-template](https://github.com/NLeSC/python-template).
 
-[^1]: We explain the rationale for this setup in the [Docker](https://mexca.readthedocs.io/en/latest/docker.html) section.
+[^1]: We explain the rationale for this setup in the [Docker](https://mexca.readthedocs.io/en/latest/docker.html) section.
```

### Comparing `mexca-0.4.0/mexca/audio/extraction.py` & `mexca-0.5.0/mexca/audio/extraction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 """Extract voice features from an audio file.
 
 Construct a dictionary with keys as feature names and values as feature objects. The dictionary can
 be used to extract the specified features with the :class:`VoiceExtractor`. Feature objects require
-lower-level voice signal properties, which are defined in the :func:`requires` method of feach 
-feature class. The :class:`VoiceExtractor` class computes the properties and supplies them to 
+lower-level voice signal properties, which are defined in the :func:`requires` method of feach
+feature class. The :class:`VoiceExtractor` class computes the properties and supplies them to
 the feature objects.
 
 """
 
 import argparse
 import logging
 import os
 from typing import Dict, Optional, Union
+
 import numpy as np
 from scipy.interpolate import interp1d
-from mexca.audio.features import (AlphaRatioFrames, AudioSignal, BaseFrames, FormantAmplitudeFrames, FormantAudioSignal,
-                                  FormantFrames, HammarIndexFrames, HnrFrames, JitterFrames, MelSpecFrames, MfccFrames,
-                                  PitchFrames, PitchHarmonicsFrames, PitchPulseFrames, RmsEnergyFrames, ShimmerFrames,
-                                  SpecFrames, SpectralFluxFrames, SpectralSlopeFrames)
+
+from mexca.audio.features import (
+    AlphaRatioFrames,
+    AudioSignal,
+    BaseFrames,
+    FormantAmplitudeFrames,
+    FormantAudioSignal,
+    FormantFrames,
+    HammarIndexFrames,
+    HnrFrames,
+    JitterFrames,
+    MelSpecFrames,
+    MfccFrames,
+    PitchFrames,
+    PitchHarmonicsFrames,
+    PitchPulseFrames,
+    RmsEnergyFrames,
+    ShimmerFrames,
+    SpecFrames,
+    SpectralFluxFrames,
+    SpectralSlopeFrames,
+)
 from mexca.data import VoiceFeatures, VoiceFeaturesConfig
 from mexca.utils import ClassInitMessage, optional_str
 
 
 class BaseFeature:
     """Base class for features.
 
@@ -40,15 +59,17 @@
         -------
         dict
             Dictionary where keys are the names and values the types of required objects.
 
         """
         return None
 
-    def _get_interp_fun(self, ts: np.ndarray, feature: np.ndarray) -> np.ndarray:
+    def _get_interp_fun(
+        self, ts: np.ndarray, feature: np.ndarray
+    ) -> np.ndarray:
         return interp1d(ts, feature, kind="linear", bounds_error=False)
 
     def apply(self, time: np.ndarray) -> np.ndarray:
         """Extract features at time points by linear interpolation.
 
         Parameters
         ----------
@@ -77,17 +98,17 @@
         dict
             Dictionary with key `pitch_frames`.
 
         """
         return {"pitch_frames": PitchFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        return self._get_interp_fun(self.pitch_frames.ts, self.pitch_frames.frames)(
-            time
-        )
+        return self._get_interp_fun(
+            self.pitch_frames.ts, self.pitch_frames.frames
+        )(time)
 
 
 class FeatureJitter(BaseFeature):
     """Extract local jitter relative to the fundamental frequency."""
 
     jitter_frames: Optional[JitterFrames] = None
 
@@ -99,17 +120,17 @@
         dict
             Dictionary with key `jitter_frames`.
 
         """
         return {"jitter_frames": JitterFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        return self._get_interp_fun(self.jitter_frames.ts, self.jitter_frames.frames)(
-            time
-        )
+        return self._get_interp_fun(
+            self.jitter_frames.ts, self.jitter_frames.frames
+        )(time)
 
 
 class FeatureShimmer(BaseFeature):
     """Extract local shimmer relative to the fundamental frequency."""
 
     shimmer_frames: Optional[ShimmerFrames] = None
 
@@ -121,17 +142,17 @@
         dict
             Dictionary with key `shimmer_frames`.
 
         """
         return {"shimmer_frames": ShimmerFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        return self._get_interp_fun(self.shimmer_frames.ts, self.shimmer_frames.frames)(
-            time
-        )
+        return self._get_interp_fun(
+            self.shimmer_frames.ts, self.shimmer_frames.frames
+        )(time)
 
 
 class FeatureHnr(BaseFeature):
     """Extract the harmonicity-to-noise ratio in dB."""
 
     hnr_frames: Optional[HnrFrames] = None
 
@@ -143,15 +164,17 @@
         dict
             Dictionary with key `hnr_frames`.
 
         """
         return {"hnr_frames": HnrFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        return self._get_interp_fun(self.hnr_frames.ts, self.hnr_frames.frames)(time)
+        return self._get_interp_fun(self.hnr_frames.ts, self.hnr_frames.frames)(
+            time
+        )
 
 
 class FeatureFormantFreq(BaseFeature):
     """Extract formant central frequency in Hz.
 
     Parameters
     ----------
@@ -173,30 +196,36 @@
         dict
             Dictionary with key `formant_frames`.
 
         """
         return {"formant_frames": FormantFrames}
 
     def apply(self, time: np.ndarray) -> Optional[np.ndarray]:
-        formants_freqs = self.formant_frames.select_formant_attr(self.n_formant, 0)
-        return self._get_interp_fun(self.formant_frames.ts, formants_freqs)(time)
+        formants_freqs = self.formant_frames.select_formant_attr(
+            self.n_formant, 0
+        )
+        return self._get_interp_fun(self.formant_frames.ts, formants_freqs)(
+            time
+        )
 
 
 class FeatureFormantBandwidth(FeatureFormantFreq):
     """Extract formant frequency bandwidth in Hz.
 
     Parameters
     ----------
     n_formant: int
         Index of the formant (starting at 0).
 
     """
 
     def apply(self, time: np.ndarray) -> Optional[np.ndarray]:
-        formants_bws = self.formant_frames.select_formant_attr(self.n_formant, 1)
+        formants_bws = self.formant_frames.select_formant_attr(
+            self.n_formant, 1
+        )
         return self._get_interp_fun(self.formant_frames.ts, formants_bws)(time)
 
 
 class FeatureFormantAmplitude(BaseFeature):
     """Extract formant amplitude relative to F0 harmonic amplitude.
 
     Parameters
@@ -227,14 +256,15 @@
         return self._get_interp_fun(
             self.formant_amp_frames.ts, formants_amps[:, self.n_formant]
         )(time)
 
 
 class FeatureAlphaRatio(BaseFeature):
     """Extract the alpha ratio in dB."""
+
     alpha_ratio_frames: Optional[AlphaRatioFrames] = None
 
     def requires(self) -> Optional[Dict[str, AlphaRatioFrames]]:
         """Specify objects required for feature extraction.
 
         Returns
         -------
@@ -248,14 +278,15 @@
         return self._get_interp_fun(
             self.alpha_ratio_frames.ts, self.alpha_ratio_frames.frames
         )(time)
 
 
 class FeatureHammarIndex(BaseFeature):
     """Extract the Hammarberg index in dB."""
+
     hammar_index_frames: Optional[HammarIndexFrames] = None
 
     def requires(self) -> Optional[Dict[str, HammarIndexFrames]]:
         """Specify objects required for feature extraction.
 
         Returns
         -------
@@ -269,22 +300,23 @@
         return self._get_interp_fun(
             self.hammar_index_frames.ts, self.hammar_index_frames.frames
         )(time)
 
 
 class FeatureSpectralSlope(BaseFeature):
     """Extract spectral slopes for frequency bands.
-    
+
     Parameters
     ----------
     lower, upper: float
         Lower and upper boundary of the frequency band for which to extract the spectral slope.
         A band with these boundaries must exist in the required `spectral_slope_frames` object.
 
     """
+
     spectral_slope_frames: Optional[SpectralSlopeFrames] = None
 
     def __init__(self, lower: float, upper: float) -> None:
         self.lower = lower
         self.upper = upper
 
     def requires(self) -> Optional[Dict[str, type]]:
@@ -295,15 +327,17 @@
         dict
             Dictionary with key `spectral_slope_frames`.
 
         """
         return {"spectral_slope_frames": SpectralSlopeFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        slope_idx = self.spectral_slope_frames.bands.index((self.lower, self.upper))
+        slope_idx = self.spectral_slope_frames.bands.index(
+            (self.lower, self.upper)
+        )
         return self._get_interp_fun(
             self.spectral_slope_frames.ts,
             self.spectral_slope_frames.frames[:, slope_idx],
         )(time)
 
 
 class FeatureHarmonicDifference(BaseFeature):
@@ -315,31 +349,38 @@
         Index of the first/second amplitude.
     x_type, y_type: str, default='h'
         Type of the first/second amplitude. Must be either `'h'` for pitch harmonic or `'f'` for formant.
 
     Raises
     ------
     ValueError
-        If `x_type` or `y_type` is not `'h'` or `'f'`.    
-    
+        If `x_type` or `y_type` is not `'h'` or `'f'`.
+
     """
+
     formant_amp_frames: Optional[FormantAmplitudeFrames] = None
     pitch_harmonics_frames: Optional[PitchHarmonicsFrames] = None
 
     def __init__(
-        self, x_idx: int = 0, x_type: str = "h", y_idx: int = 1, y_type: str = "h"
+        self,
+        x_idx: int = 0,
+        x_type: str = "h",
+        y_idx: int = 1,
+        y_type: str = "h",
     ):
         self.x_idx = x_idx
         self.x_type = x_type
         self.y_idx = y_idx
         self.y_type = y_type
 
     def requires(
         self,
-    ) -> Optional[Dict[str, Union[FormantAmplitudeFrames, PitchHarmonicsFrames]]]:
+    ) -> Optional[
+        Dict[str, Union[FormantAmplitudeFrames, PitchHarmonicsFrames]]
+    ]:
         """Specify objects required for feature extraction.
 
         Returns
         -------
         dict
             Dictionary with keys `formant_amp_frames` and `pitch_harmonics_frames`.
 
@@ -348,22 +389,28 @@
             "formant_amp_frames": FormantAmplitudeFrames,
             "pitch_harmonics_frames": PitchHarmonicsFrames,
         }
 
     def _get_harmonic_or_formant(self, which: str = "x") -> np.ndarray:
         if getattr(self, which + "_type") == "h":
             var = 20 * np.log10(
-                self.pitch_harmonics_frames.frames[:, getattr(self, which + "_idx")]
+                self.pitch_harmonics_frames.frames[
+                    :, getattr(self, which + "_idx")
+                ]
             )
         elif getattr(self, which + "_type") == "f":
             # Formant amplitude is already on dB scale
-            var = self.formant_amp_frames.frames[:, getattr(self, which + "_idx")]
+            var = self.formant_amp_frames.frames[
+                :, getattr(self, which + "_idx")
+            ]
             # Multiply by F0 on dB scale
             if self.formant_amp_frames.rel_f0:
-                var = var + 20 * np.log10(self.pitch_harmonics_frames.frames[:, 0])
+                var = var + 20 * np.log10(
+                    self.pitch_harmonics_frames.frames[:, 0]
+                )
         else:
             raise ValueError(
                 f"'{which}_type' must be either 'h' (pitch harmonic) or 'f' (formant)"
             )
 
         return var
 
@@ -381,14 +428,15 @@
 
     Parameters
     ----------
     n_mfcc: int, default=0
         Index of the MFCC to be extracted.
 
     """
+
     mfcc_frames: Optional[MfccFrames] = None
 
     def __init__(self, n_mfcc: int = 0) -> None:
         self.n_mfcc = n_mfcc
 
     def requires(self) -> Optional[Dict[str, MfccFrames]]:
         """Specify objects required for feature extraction.
@@ -404,16 +452,16 @@
     def apply(self, time: np.ndarray) -> np.ndarray:
         return self._get_interp_fun(
             self.mfcc_frames.ts, self.mfcc_frames.frames[:, self.n_mfcc]
         )(time)
 
 
 class FeatureSpectralFlux(BaseFeature):
-    """Extract spectral flux.
-    """
+    """Extract spectral flux."""
+
     spec_flux_frames: Optional[SpectralFluxFrames] = None
 
     def requires(self) -> Optional[Dict[str, SpectralFluxFrames]]:
         """Specify objects required for feature extraction.
 
         Returns
         -------
@@ -426,31 +474,33 @@
     def apply(self, time: np.ndarray) -> np.ndarray:
         return self._get_interp_fun(
             self.spec_flux_frames.ts, self.spec_flux_frames.frames
         )(time)
 
 
 class FeatureRmsEnergy(BaseFeature):
-    """Extract the root mean squared energy in dB.
-    """
+    """Extract the root mean squared energy in dB."""
+
     rms_frames: Optional[RmsEnergyFrames] = None
 
     def requires(self) -> Optional[Dict[str, type]]:
         """Specify objects required for feature extraction.
 
         Returns
         -------
         dict
             Dictionary with key `rms_frames`.
 
         """
         return {"rms_frames": RmsEnergyFrames}
 
     def apply(self, time: np.ndarray) -> np.ndarray:
-        return self._get_interp_fun(self.rms_frames.ts, self.rms_frames.frames)(time)
+        return self._get_interp_fun(self.rms_frames.ts, self.rms_frames.frames)(
+            time
+        )
 
 
 class VoiceExtractor:
     """Extract voice features from an audio file.
 
     For default features, see the :ref:`Output <voice_features_output>` section.
 
@@ -460,15 +510,19 @@
         Dictionary with keys as feature names and values as feature extraction objects. If `None`,
         default features are extracted.
     config: VoiceFeaturesConfig, optional, default=None
         Voice feature extraction configuration object. If `None`, uses :class:`VoiceFeaturesConfig`'s default configuration.
 
     """
 
-    def __init__(self, features: Optional[Dict[str, BaseFeature]] = None, config: Optional[VoiceFeaturesConfig] = None):
+    def __init__(
+        self,
+        features: Optional[Dict[str, BaseFeature]] = None,
+        config: Optional[VoiceFeaturesConfig] = None,
+    ):
         self.logger = logging.getLogger("mexca.audio.extraction.VoiceExtractor")
 
         if features is None:
             features = self._set_default_features()
 
         if config is None:
             config = VoiceFeaturesConfig()
@@ -480,17 +534,19 @@
 
         self.logger.debug(ClassInitMessage())
 
     @staticmethod
     def _check_features(features: dict):
         for key, item in features.items():
             if not isinstance(key, str):
-                raise TypeError(f'Feature name {key} is not a string')
+                raise TypeError(f"Feature name {key} is not a string")
             if not isinstance(item, BaseFeature):
-                raise TypeError(f'Feature object {item} with name {key} is not a subclass of "mexca.audio.features.BaseFeature"')
+                raise TypeError(
+                    f'Feature object {item} with name {key} is not a subclass of "mexca.audio.features.BaseFeature"'
+                )
 
     @staticmethod
     def _set_default_features() -> Dict[str, BaseFeature]:
         return {
             "pitch_f0_hz": FeaturePitchF0(),
             "jitter_local_rel_f0": FeatureJitter(),
             "shimmer_local_rel_f0": FeatureShimmer(),
@@ -503,15 +559,17 @@
             "f2_amplitude_rel_f0": FeatureFormantAmplitude(n_formant=1),
             "f3_freq_hz": FeatureFormantFreq(n_formant=2),
             "f3_bandwidth_hz": FeatureFormantBandwidth(n_formant=2),
             "f3_amplitude_rel_f0": FeatureFormantAmplitude(n_formant=2),
             "alpha_ratio_db": FeatureAlphaRatio(),
             "hammar_index_db": FeatureHammarIndex(),
             "spectral_slope_0_500": FeatureSpectralSlope(lower=0, upper=500),
-            "spectral_slope_500_1500": FeatureSpectralSlope(lower=500, upper=1500),
+            "spectral_slope_500_1500": FeatureSpectralSlope(
+                lower=500, upper=1500
+            ),
             "h1_h2_diff_db": FeatureHarmonicDifference(),
             "h1_f3_diff_db": FeatureHarmonicDifference(y_idx=2, y_type="f"),
             "mfcc_1": FeatureMfcc(),
             "mfcc_2": FeatureMfcc(n_mfcc=1),
             "mfcc_3": FeatureMfcc(n_mfcc=2),
             "mfcc_4": FeatureMfcc(n_mfcc=3),
             "spectral_flux": FeatureSpectralFlux(),
@@ -540,57 +598,127 @@
         """
         self.logger.debug("Loading audio file")
         audio_signal = AudioSignal.from_file(filename=filepath)
 
         self.logger.debug("Extracting features with time step: %s", time_step)
 
         time = np.arange(
-            audio_signal.ts.min(), audio_signal.ts.max(), time_step, dtype=np.float32
+            audio_signal.ts.min(),
+            audio_signal.ts.max(),
+            time_step,
+            dtype=np.float32,
         )
         frame = np.array((time / time_step) * skip_frames, dtype=np.int32)
 
         sig_frames = BaseFrames.from_signal(
-            audio_signal, frame_len=self.config.frame_len, hop_len=self.config.hop_len, center=self.config.center, pad_mode=self.config.pad_mode
+            audio_signal,
+            frame_len=self.config.frame_len,
+            hop_len=self.config.hop_len,
+            center=self.config.center,
+            pad_mode=self.config.pad_mode,
         )
 
         spec_frames = SpecFrames.from_signal(
-            audio_signal, frame_len=self.config.frame_len, hop_len=self.config.hop_len, center=self.config.center, pad_mode=self.config.pad_mode, window=self.config.spec_window
+            audio_signal,
+            frame_len=self.config.frame_len,
+            hop_len=self.config.hop_len,
+            center=self.config.center,
+            pad_mode=self.config.pad_mode,
+            window=self.config.spec_window,
         )
         pitch_frames = PitchFrames.from_signal(
-            audio_signal, frame_len=self.config.frame_len, hop_len=self.config.hop_len, center=self.config.center, pad_mode=self.config.pad_mode, lower=self.config.pitch_lower_freq, upper=self.config.pitch_upper_freq, method=self.config.pitch_method
+            audio_signal,
+            frame_len=self.config.frame_len,
+            hop_len=self.config.hop_len,
+            center=self.config.center,
+            pad_mode=self.config.pad_mode,
+            lower=self.config.pitch_lower_freq,
+            upper=self.config.pitch_upper_freq,
+            method=self.config.pitch_method,
         )
         pulses_frames = PitchPulseFrames.from_signal_and_pitch_frames(
             audio_signal, pitch_frames
         )
-        jitter_frames = JitterFrames.from_pitch_pulse_frames(pulses_frames, rel=self.config.jitter_rel, lower=self.config.pitch_pulse_lower_period, upper=self.config.pitch_pulse_upper_period, max_period_ratio=self.config.pitch_pulse_max_period_ratio)
-        shimmer_frames = ShimmerFrames.from_pitch_pulse_frames(pulses_frames, rel=self.config.shimmer_rel, lower=self.config.pitch_pulse_lower_period, upper=self.config.pitch_pulse_upper_period, max_period_ratio=self.config.pitch_pulse_max_period_ratio, max_amp_factor=self.config.pitch_pulse_max_amp_factor)
-        hnr_frames = HnrFrames.from_frames(sig_frames, lower=self.config.hnr_lower_freq, rel_silence_threshold=self.config.hnr_rel_silence_threshold)
+        jitter_frames = JitterFrames.from_pitch_pulse_frames(
+            pulses_frames,
+            rel=self.config.jitter_rel,
+            lower=self.config.pitch_pulse_lower_period,
+            upper=self.config.pitch_pulse_upper_period,
+            max_period_ratio=self.config.pitch_pulse_max_period_ratio,
+        )
+        shimmer_frames = ShimmerFrames.from_pitch_pulse_frames(
+            pulses_frames,
+            rel=self.config.shimmer_rel,
+            lower=self.config.pitch_pulse_lower_period,
+            upper=self.config.pitch_pulse_upper_period,
+            max_period_ratio=self.config.pitch_pulse_max_period_ratio,
+            max_amp_factor=self.config.pitch_pulse_max_amp_factor,
+        )
+        hnr_frames = HnrFrames.from_frames(
+            sig_frames,
+            lower=self.config.hnr_lower_freq,
+            rel_silence_threshold=self.config.hnr_rel_silence_threshold,
+        )
 
         formant_signal = FormantAudioSignal.from_audio_signal(
-            audio_signal, preemphasis_from=self.config.formants_signal_preemphasis_from
+            audio_signal,
+            preemphasis_from=self.config.formants_signal_preemphasis_from,
         )
         formant_sig_frames = BaseFrames.from_signal(
-            formant_signal, frame_len=self.config.frame_len, hop_len=self.config.hop_len, center=self.config.center, pad_mode=self.config.pad_mode
+            formant_signal,
+            frame_len=self.config.frame_len,
+            hop_len=self.config.hop_len,
+            center=self.config.center,
+            pad_mode=self.config.pad_mode,
         )
         formant_frames = FormantFrames.from_frames(
-            formant_sig_frames, max_formants=self.config.formants_max, lower=self.config.formants_lower_freq, upper=self.config.formants_upper_freq, preemphasis_from=None, window=self.config.formants_window
+            formant_sig_frames,
+            max_formants=self.config.formants_max,
+            lower=self.config.formants_lower_freq,
+            upper=self.config.formants_upper_freq,
+            preemphasis_from=None,
+            window=self.config.formants_window,
         )
         pitch_harmonics = PitchHarmonicsFrames.from_spec_and_pitch_frames(
             spec_frames, pitch_frames, n_harmonics=self.config.pitch_n_harmonics
         )
         formant_amp_frames = (
             FormantAmplitudeFrames.from_formant_harmonics_and_pitch_frames(
-                formant_frames, pitch_harmonics, pitch_frames, lower=self.config.formants_amp_lower, upper=self.config.formants_amp_upper, rel_f0=self.config.formants_amp_rel_f0
+                formant_frames,
+                pitch_harmonics,
+                pitch_frames,
+                lower=self.config.formants_amp_lower,
+                upper=self.config.formants_amp_upper,
+                rel_f0=self.config.formants_amp_rel_f0,
             )
         )
-        alpha_ratio_frames = AlphaRatioFrames.from_spec_frames(spec_frames, lower_band=self.config.alpha_ratio_lower_band, upper_band=self.config.alpha_ratio_upper_band)
-        hammar_index_frames = HammarIndexFrames.from_spec_frames(spec_frames, pivot_point=self.config.hammar_index_pivot_point_freq, upper=self.config.hammar_index_upper_freq)
-        spectral_slope_frames = SpectralSlopeFrames.from_spec_frames(spec_frames, bands=self.config.spectral_slopes_bands)
-        mel_spec_frames = MelSpecFrames.from_spec_frames(spec_frames, n_mels=self.config.mel_spec_n_mels, lower=self.config.mel_spec_lower_freq, upper=self.config.mel_spec_upper_freq)
-        mfcc_frames = MfccFrames.from_mel_spec_frames(mel_spec_frames, n_mfcc=self.config.mfcc_n, lifter=self.config.mfcc_lifter)
+        alpha_ratio_frames = AlphaRatioFrames.from_spec_frames(
+            spec_frames,
+            lower_band=self.config.alpha_ratio_lower_band,
+            upper_band=self.config.alpha_ratio_upper_band,
+        )
+        hammar_index_frames = HammarIndexFrames.from_spec_frames(
+            spec_frames,
+            pivot_point=self.config.hammar_index_pivot_point_freq,
+            upper=self.config.hammar_index_upper_freq,
+        )
+        spectral_slope_frames = SpectralSlopeFrames.from_spec_frames(
+            spec_frames, bands=self.config.spectral_slopes_bands
+        )
+        mel_spec_frames = MelSpecFrames.from_spec_frames(
+            spec_frames,
+            n_mels=self.config.mel_spec_n_mels,
+            lower=self.config.mel_spec_lower_freq,
+            upper=self.config.mel_spec_upper_freq,
+        )
+        mfcc_frames = MfccFrames.from_mel_spec_frames(
+            mel_spec_frames,
+            n_mfcc=self.config.mfcc_n,
+            lifter=self.config.mfcc_lifter,
+        )
         spec_flux_frames = SpectralFluxFrames.from_spec_frames(spec_frames)
         rms_frames = RmsEnergyFrames.from_spec_frames(spec_frames)
 
         requirements = [
             audio_signal,
             pitch_frames,
             pulses_frames,
@@ -605,15 +733,17 @@
             spectral_slope_frames,
             mfcc_frames,
             spec_flux_frames,
             rms_frames,
         ]
         requirements_types = [type(r) for r in requirements]
 
-        extracted_features = VoiceFeatures(frame=frame.tolist(), time=time.tolist())
+        extracted_features = VoiceFeatures(
+            frame=frame.tolist(), time=time.tolist()
+        )
         extracted_features.add_attributes(self.features.keys())
 
         for key, feat in self.features.items():
             for attr, req in feat.requires().items():
                 idx = requirements_types.index(req)
                 setattr(feat, attr, requirements[idx])
 
@@ -630,28 +760,34 @@
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter
     )
 
     parser.add_argument("-f", "--filepath", type=str, required=True)
     parser.add_argument("-o", "--outdir", type=str, required=True)
     parser.add_argument("-t", "--time-step", type=float, dest="time_step")
-    parser.add_argument("--skip-frames", type=int, default=1, dest="skip_frames")
-    parser.add_argument("--config-filepath", type=optional_str, default=None, dest="config")
+    parser.add_argument(
+        "--skip-frames", type=int, default=1, dest="skip_frames"
+    )
+    parser.add_argument(
+        "--config-filepath", type=optional_str, default=None, dest="config"
+    )
 
     args = parser.parse_args().__dict__
 
     if "config" in args:
         config = VoiceFeaturesConfig.from_yaml(args["config"])
     else:
         config = VoiceFeaturesConfig()
 
     extractor = VoiceExtractor(config=config)
 
     output = extractor.apply(
-        args["filepath"], time_step=args["time_step"], skip_frames=args["skip_frames"]
+        args["filepath"],
+        time_step=args["time_step"],
+        skip_frames=args["skip_frames"],
     )
 
     output.write_json(
         os.path.join(
             args["outdir"],
             os.path.splitext(os.path.basename(args["filepath"]))[0]
             + "_voice_features.json",
```

### Comparing `mexca-0.4.0/mexca/audio/features.py` & `mexca-0.5.0/mexca/audio/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,22 @@
 
 """
 
 import logging
 import math
 from copy import copy
 from typing import List, Optional, Tuple, Union
+
 import librosa
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.signal import find_peaks
 from scipy.signal.windows import get_window
 from sklearn.linear_model import LinearRegression
+
 from mexca.utils import ClassInitMessage
 
 
 class BaseSignal:
     """Store a signal.
 
     Parameters
@@ -83,15 +85,17 @@
         self.logger = logging.getLogger("mexca.audio.extraction.AudioSignal")
         self.filename = filename
         self.mono = mono
         super().__init__(sig, sr)
         self.logger.debug(ClassInitMessage())
 
     @classmethod
-    def from_file(cls, filename: str, sr: Optional[float] = None, mono: bool = True):
+    def from_file(
+        cls, filename: str, sr: Optional[float] = None, mono: bool = True
+    ):
         """Load a signal from an audio file.
 
         Parameters
         ----------
         filename: str
             Name of the audio file.
             File types must be supported by ``soundfile`` or ``audiofile``.
@@ -119,20 +123,24 @@
 
     @staticmethod
     def _calc_preemphasis_coef(preemphasis_from: float, sr: float) -> float:
         return math.exp(-2 * math.pi * preemphasis_from * (1 / sr))
 
     @classmethod
     def from_audio_signal(
-        cls, audio_sig_obj: AudioSignal, preemphasis_from: Optional[float] = 50.0
+        cls,
+        audio_sig_obj: AudioSignal,
+        preemphasis_from: Optional[float] = 50.0,
     ):
         sig = audio_sig_obj.sig
 
         if preemphasis_from is not None:
-            pre_coef = cls._calc_preemphasis_coef(preemphasis_from, audio_sig_obj.sr)
+            pre_coef = cls._calc_preemphasis_coef(
+                preemphasis_from, audio_sig_obj.sr
+            )
             sig = librosa.effects.preemphasis(sig, coef=pre_coef)
 
         return cls(
             sig,
             audio_sig_obj.sr,
             audio_sig_obj.mono,
             audio_sig_obj.filename,
@@ -351,15 +359,17 @@
                 sr=sig_obj.sr,
                 frame_length=frame_len,
                 hop_length=hop_len,
                 center=center,
                 pad_mode=pad_mode,
             )
         else:
-            raise NotImplementedError('Only the "pyin" method is currently available')
+            raise NotImplementedError(
+                'Only the "pyin" method is currently available'
+            )
 
         return cls(
             frames=pitch_f0,
             flag=flag,
             prob=prob,
             sr=sig_obj.sr,
             lower=lower,
@@ -408,15 +418,17 @@
         self._freqs = None
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @property
     def freqs(self):
         if self._freqs is None:
-            self._freqs = librosa.fft_frequencies(sr=self.sr, n_fft=self.frame_len)
+            self._freqs = librosa.fft_frequencies(
+                sr=self.sr, n_fft=self.frame_len
+            )
         return self._freqs
 
     @classmethod
     def from_signal(
         cls,
         sig_obj: BaseSignal,
         frame_len: int,
@@ -535,15 +547,16 @@
     def _praat_gauss_window(frame_len: int):
         # This is the Gaussian window that is used in Praat for formant estimation
         # See: https://github.com/YannickJadoul/Parselmouth/blob/master/praat/fon/Sound_to_Formant.cpp
         sample_idx = np.arange(frame_len) + 1
         idx_mid = 0.5 * (frame_len + 1)
         edge = np.exp(-12.0)
         return (
-            np.exp(-48.0 * (sample_idx - idx_mid) ** 2 / (frame_len) ** 2) - edge
+            np.exp(-48.0 * (sample_idx - idx_mid) ** 2 / (frame_len) ** 2)
+            - edge
         ) / (1.0 - edge)
 
     @classmethod
     def from_frames(
         cls,
         sig_frames_obj: BaseFrames,
         max_formants: int = 5,
@@ -572,27 +585,32 @@
         """
         frames = sig_frames_obj.frames
 
         if preemphasis_from is not None:
             pre_coef = math.exp(
                 -2 * math.pi * preemphasis_from * (1 / sig_frames_obj.sr)
             )
-            frames = librosa.effects.preemphasis(sig_frames_obj.frames, coef=pre_coef)
+            frames = librosa.effects.preemphasis(
+                sig_frames_obj.frames, coef=pre_coef
+            )
         if window is not None:
             if window == "praat_gaussian":
                 win = cls._praat_gauss_window(sig_frames_obj.frame_len)
             else:
-                win = get_window(window, sig_frames_obj.frame_len, fftbins=False)
+                win = get_window(
+                    window, sig_frames_obj.frame_len, fftbins=False
+                )
             frames = frames * win
 
         # Calc linear predictive coefficients
         coefs = librosa.lpc(frames, order=max_formants * 2)
         # Transform LPCs to formants
         formants = [
-            cls._calc_formants(coef, sig_frames_obj.sr, lower, upper) for coef in coefs
+            cls._calc_formants(coef, sig_frames_obj.sr, lower, upper)
+            for coef in coefs
         ]
 
         return cls(
             formants,
             sig_frames_obj.sr,
             sig_frames_obj.frame_len,
             sig_frames_obj.hop_len,
@@ -620,23 +638,27 @@
         mask = np.imag(roots) > 0
         roots = roots[mask]
         # Calc angular frequency
         ang_freq = np.abs(np.arctan2(np.imag(roots), np.real(roots)))
         # Calc formant centre freq
         formant_freqs = ang_freq * nf_pi
         # Calc formant bandwidth
-        formant_bws = -np.log(np.apply_along_axis(complex_norm, 0, roots)) * nf_pi
+        formant_bws = (
+            -np.log(np.apply_along_axis(complex_norm, 0, roots)) * nf_pi
+        )
         # Select formants within boundaries
         in_bounds = np.logical_and(formant_freqs > lower, formant_freqs < upper)
         formants_sorted = sorted(
             list(zip(formant_freqs[in_bounds], formant_bws[in_bounds]))
         )
         return formants_sorted
 
-    def select_formant_attr(self, formant_idx: int, attr_idx: int) -> np.ndarray:
+    def select_formant_attr(
+        self, formant_idx: int, attr_idx: int
+    ) -> np.ndarray:
         return np.array(
             [
                 f[formant_idx][attr_idx] if len(f) > formant_idx else np.nan
                 for f in self.frames
             ]
         )
 
@@ -666,15 +688,17 @@
         sr: int,
         frame_len: int,
         hop_len: int,
         center: bool = True,
         pad_mode: str = "constant",
         n_harmonics: int = 100,
     ):
-        self.logger = logging.getLogger("mexca.audio.extraction.PitchHarmonicsFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.PitchHarmonicsFrames"
+        )
         self.n_harmonics = n_harmonics
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_and_pitch_frames(
         cls,
@@ -742,15 +766,17 @@
                 fill_value=0,
             )
             return interp(f0_harmonic_freqs)
 
         xfunc = np.vectorize(mag_interp_fun, signature="(f),(h)->(h)")
         harmonics_frames = xfunc(
             np.abs(spec_frames),
-            np.multiply.outer(f0_frames, np.arange(n_harmonics) + 1),  # Shift one up
+            np.multiply.outer(
+                f0_frames, np.arange(n_harmonics) + 1
+            ),  # Shift one up
         )
 
         return harmonics_frames
 
 
 class FormantAmplitudeFrames(BaseFrames):
     """Estimate and store formant amplitudes.
@@ -848,15 +874,17 @@
             harmonic_peaks[harmonics_amp_all_na] = np.nan
             harmonic_peaks[~harmonics_amp_all_na] = np.nanmax(
                 harmonics_amp[~harmonics_amp_all_na], axis=1
             )
             harmonic_peaks_db = librosa.amplitude_to_db(harmonic_peaks)
 
             if rel_f0:
-                harmonic_peaks_db = harmonic_peaks_db - librosa.amplitude_to_db(f0_amp)
+                harmonic_peaks_db = harmonic_peaks_db - librosa.amplitude_to_db(
+                    f0_amp
+                )
 
             amp_frames.append(harmonic_peaks_db)
 
         return cls(
             np.array(amp_frames).T,
             formant_frames_obj.sr,
             formant_frames_obj.frame_len,
@@ -905,15 +933,17 @@
         frames: List[Tuple],
         sr: int,
         frame_len: int,
         hop_len: int,
         center: bool = True,
         pad_mode: str = "constant",
     ) -> None:
-        self.logger = logging.getLogger("mexca.audio.extraction.PitchPulseFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.PitchPulseFrames"
+        )
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @property
     def idx(self) -> np.ndarray:
         if self._idx is None:
             self._idx = np.arange(len(self.frames))
@@ -931,16 +961,21 @@
             Signal object.
         pitch_frames_obj: PitchFrames
             Voice pitch frames object.
 
         """
         # Access to padded signal required so we transform it here again! Could go into separate private method perhaps
         padding = [(0, 0) for _ in sig_obj.sig.shape]
-        padding[-1] = (pitch_frames_obj.frame_len // 2, pitch_frames_obj.frame_len // 2)
-        sig_padded = np.pad(sig_obj.sig, padding, mode=pitch_frames_obj.pad_mode)
+        padding[-1] = (
+            pitch_frames_obj.frame_len // 2,
+            pitch_frames_obj.frame_len // 2,
+        )
+        sig_padded = np.pad(
+            sig_obj.sig, padding, mode=pitch_frames_obj.pad_mode
+        )
         # Create ts for padded signal
         sig_padded_ts = librosa.samples_to_time(
             np.arange(sig_padded.shape[0]), sr=sig_obj.sr
         )
 
         # Frame padded signal
         sig_frames_obj = BaseFrames.from_signal(
@@ -1038,15 +1073,17 @@
             start = new_ts_mid - 1.25 * new_t0_interp_mid
             stop = new_ts_mid - 0.8 * new_t0_interp_mid
         else:  # Move interval to right
             stop = new_ts_mid + 1.25 * new_t0_interp_mid
             start = new_ts_mid + 0.8 * new_t0_interp_mid
 
         # Find next pulse in new interval
-        return cls._get_next_pulse(sig, ts, t0_interp, start, stop, left, pulses)
+        return cls._get_next_pulse(
+            sig, ts, t0_interp, start, stop, left, pulses
+        )
 
     @classmethod
     def _detect_pulses_in_frame(
         cls,
         frame_idx: int,
         sig_frames_obj: BaseFrames,
         sig_ts_frames_obj: BaseFrames,
@@ -1071,18 +1108,22 @@
             return pulses
 
         # Set start interval
         start = ts_mid - t0_mid / 2
         stop = ts_mid + t0_mid / 2
 
         # Get pulses to the left
-        cls._get_next_pulse(sig_frame, ts_sig_frame, t0, start, stop, True, pulses)
+        cls._get_next_pulse(
+            sig_frame, ts_sig_frame, t0, start, stop, True, pulses
+        )
 
         # Get pulses to the right
-        cls._get_next_pulse(sig_frame, ts_sig_frame, t0, start, stop, False, pulses)
+        cls._get_next_pulse(
+            sig_frame, ts_sig_frame, t0, start, stop, False, pulses
+        )
 
         return list(sorted(set(pulses)))
 
 
 class PitchPeriodFrames(BaseFrames):
     def __init__(
         self,
@@ -1091,15 +1132,17 @@
         frame_len: int,
         hop_len: int,
         center: bool,
         pad_mode: str,
         lower: float,
         upper: float,
     ):
-        self.logger = logging.getLogger("mexca.audio.extraction.PitchPeriodFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.PitchPeriodFrames"
+        )
         self.lower = lower
         self.upper = upper
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @staticmethod
     def _calc_period_length(
@@ -1160,15 +1203,17 @@
         lower: float,
         upper: float,
         max_period_ratio: float,
     ):
         self.logger = logging.getLogger("mexca.audio.extraction.JitterFrames")
         self.rel = rel
         self.max_period_ratio = max_period_ratio
-        super().__init__(frames, sr, frame_len, hop_len, center, pad_mode, lower, upper)
+        super().__init__(
+            frames, sr, frame_len, hop_len, center, pad_mode, lower, upper
+        )
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_pitch_pulse_frames(
         cls,
         pitch_pulse_frames_obj: PitchPulseFrames,
         rel: bool = True,
@@ -1189,15 +1234,17 @@
         upper: float, optional, default=0.02
             Upper limit for periods between glottal pulses.
         max_period_ratio: float, optional, default=1.3
             Maximum ratio between consecutive periods for jitter extraction.
         """
         jitter_frames = np.array(
             [
-                cls._calc_jitter_frame(pulses, rel, lower, upper, max_period_ratio)
+                cls._calc_jitter_frame(
+                    pulses, rel, lower, upper, max_period_ratio
+                )
                 for pulses in pitch_pulse_frames_obj.frames
             ]
         )
 
         return cls(
             jitter_frames,
             pitch_pulse_frames_obj.sr,
@@ -1233,24 +1280,28 @@
         # only consider period pairs where ratio is < max_period_ratio
         period_diff = [
             np.abs(np.diff(period)[cls._check_ratio(period, max_period_ratio)])
             for period in periods
             if len(period) > 1
         ]
 
-        if len(period_diff) == 0 or all(len(period) == 0 for period in period_diff):
+        if len(period_diff) == 0 or all(
+            len(period) == 0 for period in period_diff
+        ):
             return np.nan
 
         avg_period_diff = np.nanmean(
             np.array([np.mean(period) for period in period_diff])
         )
 
         if rel:  # Relative to mean period length
             avg_period_len = np.nanmean(
-                np.array([np.mean(period) for period in periods if len(period) > 1])
+                np.array(
+                    [np.mean(period) for period in periods if len(period) > 1]
+                )
             )
             return avg_period_diff / avg_period_len
 
         return avg_period_diff
 
 
 class ShimmerFrames(PitchPeriodFrames):
@@ -1294,15 +1345,17 @@
         max_period_ratio: float,
         max_amp_factor: float,
     ):
         self.logger = logging.getLogger("mexca.audio.extraction.ShimmerFrames")
         self.rel = rel
         self.max_period_ratio = max_period_ratio
         self.max_amp_factor = max_amp_factor
-        super().__init__(frames, sr, frame_len, hop_len, center, pad_mode, lower, upper)
+        super().__init__(
+            frames, sr, frame_len, hop_len, center, pad_mode, lower, upper
+        )
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_pitch_pulse_frames(
         cls,
         pitch_pulse_frames_obj: PitchPulseFrames,
         rel: bool = True,
@@ -1475,15 +1528,19 @@
             Lower fundamental frequency limit for choosing pitch candidates.
         rel_silence_threshold: float, default = 0.1
             Relative threshold for treating signal frames as silent.
 
         """
         auto_cor = librosa.autocorrelate(sig_frames_obj.frames)
         harmonic_strength = np.apply_along_axis(
-            cls._find_max_peak, 1, auto_cor[:, 1:], sr=sig_frames_obj.sr, lower=lower
+            cls._find_max_peak,
+            1,
+            auto_cor[:, 1:],
+            sr=sig_frames_obj.sr,
+            lower=lower,
         )
         harmonic_comp = harmonic_strength / auto_cor[:, 0]
         hnr = harmonic_comp / (1 - harmonic_comp)
         silence_mask = np.max(
             np.abs(sig_frames_obj.frames), axis=1
         ) > rel_silence_threshold * np.max(np.abs(sig_frames_obj.frames))
         hnr[np.logical_or(~silence_mask, hnr <= 0)] = np.nan
@@ -1547,15 +1604,17 @@
         frame_len: int,
         hop_len: int,
         center: bool,
         pad_mode: str,
         lower_band: Tuple[float],
         upper_band: Tuple[float],
     ):
-        self.logger = logging.getLogger("mexca.audio.extraction.AlphaRatioFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.AlphaRatioFrames"
+        )
         self.lower_band = lower_band
         self.upper_band = upper_band
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_frames(
@@ -1642,15 +1701,17 @@
         frame_len: int,
         hop_len: int,
         center: bool,
         pad_mode: str,
         pivot_point: float,
         upper: float,
     ):
-        self.logger = logging.getLogger("mexca.audio.extraction.HammarIndexFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.HammarIndexFrames"
+        )
         self.pivot_point = pivot_point
         self.upper = upper
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_frames(
@@ -1678,15 +1739,16 @@
             spec_frames_obj.freqs > pivot_point, spec_frames_obj.freqs <= upper
         )
         upper_band = np.abs(spec_frames_obj.frames[:, upper_band_freqs])
 
         hammar_index_frames = np.zeros(lower_band.shape[0])
 
         upper_band_is_valid = np.logical_and(
-            np.any(np.isfinite(upper_band), axis=1), np.all(upper_band > 0, axis=1)
+            np.any(np.isfinite(upper_band), axis=1),
+            np.all(upper_band > 0, axis=1),
         )
 
         hammar_index_frames[~upper_band_is_valid] = np.nan
         hammar_index_frames[upper_band_is_valid] = np.nanmax(
             lower_band[upper_band_is_valid, :], axis=1
         ) / np.nanmax(upper_band[upper_band_is_valid, :], axis=1)
 
@@ -1727,15 +1789,17 @@
         sr: int,
         frame_len: int,
         hop_len: int,
         center: bool,
         pad_mode: str,
         bands: Tuple[Tuple[float]],
     ):
-        self.logger = logging.getLogger("mexca.audio.extraction.HammarIndexFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.HammarIndexFrames"
+        )
         self.bands = bands
         super().__init__(frames, sr, frame_len, hop_len, center, pad_mode)
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_frames(
         cls,
@@ -1748,19 +1812,22 @@
         ----------
         spec_frames_obj: SpecFrames
             Spectrogram frames object.
         bands: tuple, default=((0.0, 500.0), (500.0, 1500.0))
             Frequency bands in Hz for which slopes are estimated.
 
         """
-        spectral_slopes = np.zeros(shape=(spec_frames_obj.idx.shape[0], len(bands)))
+        spectral_slopes = np.zeros(
+            shape=(spec_frames_obj.idx.shape[0], len(bands))
+        )
 
         for i, band in enumerate(bands):
             band_freqs_mask = np.logical_and(
-                spec_frames_obj.freqs > band[0], spec_frames_obj.freqs <= band[1]
+                spec_frames_obj.freqs > band[0],
+                spec_frames_obj.freqs <= band[1],
             )
             band_power = np.abs(spec_frames_obj.frames[:, band_freqs_mask])
             band_freqs = spec_frames_obj.freqs[band_freqs_mask]
             spectral_slopes[:, i] = np.apply_along_axis(
                 cls._calc_spectral_slope, 1, band_power, band_freqs=band_freqs
             ).squeeze()
 
@@ -1774,21 +1841,25 @@
             bands,
         )
 
     @staticmethod
     def _calc_spectral_slope(
         band_power: np.ndarray, band_freqs: np.ndarray
     ) -> np.ndarray:
-        band_power_is_valid = np.logical_and(np.isfinite(band_power), band_power > 0)
+        band_power_is_valid = np.logical_and(
+            np.isfinite(band_power), band_power > 0
+        )
 
         if np.all(~band_power_is_valid):
             return np.nan
 
         band_freqs_finite = band_freqs[band_power_is_valid]
-        band_power_finite_db = librosa.amplitude_to_db(band_power[band_power_is_valid])
+        band_power_finite_db = librosa.amplitude_to_db(
+            band_power[band_power_is_valid]
+        )
 
         linear_model = LinearRegression()
         linear_model.fit(band_freqs_finite.reshape(-1, 1), band_power_finite_db)
         return linear_model.coef_
 
 
 class MelSpecFrames(SpecFrames):
@@ -1824,15 +1895,17 @@
         lower: float,
         upper: float,
     ):
         self.logger = logging.getLogger("mexca.audio.extraction.MelSpecFrames")
         self.n_mels = n_mels
         self.lower = lower
         self.upper = upper
-        super().__init__(frames, sr, window, frame_len, hop_len, center, pad_mode)
+        super().__init__(
+            frames, sr, window, frame_len, hop_len, center, pad_mode
+        )
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_frames(
         cls,
         spec_frames_obj: SpecFrames,
         n_mels: int = 26,
@@ -1923,15 +1996,18 @@
             lower,
             upper,
         )
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_mel_spec_frames(
-        cls, mel_spec_frames_obj: MelSpecFrames, n_mfcc: int = 4, lifter: float = 22.0
+        cls,
+        mel_spec_frames_obj: MelSpecFrames,
+        n_mfcc: int = 4,
+        lifter: float = 22.0,
     ):
         """Estimate MFCCs from Mel spectogram frames.
 
         Parameters
         ----------
         mel_spec_frames_obj: MelSpecFrames
             Mel spectrogram frames object.
@@ -1942,15 +2018,17 @@
 
         See Also
         --------
         librosa.feature.mfcc
 
         """
         mfcc_frames = librosa.feature.mfcc(
-            S=librosa.power_to_db(mel_spec_frames_obj.frames.T),  # dB on power spectrum
+            S=librosa.power_to_db(
+                mel_spec_frames_obj.frames.T
+            ),  # dB on power spectrum
             sr=mel_spec_frames_obj.sr,
             n_mfcc=n_mfcc,
             lifter=lifter,
         )
 
         return cls(
             mfcc_frames.T,
@@ -2003,23 +2081,30 @@
         frame_len: int,
         hop_len: int,
         center: bool,
         pad_mode: str,
         lower: float,
         upper: float,
     ) -> None:
-        self.logger = logging.getLogger("mexca.audio.extraction.SpectralFluxFrames")
+        self.logger = logging.getLogger(
+            "mexca.audio.extraction.SpectralFluxFrames"
+        )
         self.lower = lower
         self.upper = upper
-        super().__init__(frames, sr, window, frame_len, hop_len, center, pad_mode)
+        super().__init__(
+            frames, sr, window, frame_len, hop_len, center, pad_mode
+        )
         self.logger.debug(ClassInitMessage())
 
     @classmethod
     def from_spec_frames(
-        cls, spec_frames_obj: SpecFrames, lower: float = 0.0, upper: float = 5000.0
+        cls,
+        spec_frames_obj: SpecFrames,
+        lower: float = 0.0,
+        upper: float = 5000.0,
     ):
         """Calculate the spectral flux from spectrogram frames.
 
         Parameters
         ----------
         spec_frames_obj: SpecFrames
             Spectrogram frames object.
@@ -2030,15 +2115,17 @@
 
         """
         spec_freq_mask = np.logical_and(
             spec_frames_obj.freqs >= lower, spec_frames_obj.freqs < upper
         )
         spec_mag = np.abs(spec_frames_obj.frames)
         spec_norm = np.sum(spec_mag, axis=1)
-        spec_diff = np.diff(spec_mag[:, spec_freq_mask] / spec_norm[:, None], axis=0)
+        spec_diff = np.diff(
+            spec_mag[:, spec_freq_mask] / spec_norm[:, None], axis=0
+        )
         spec_flux_frames = np.sum(spec_diff**2, axis=1)
 
         return cls(
             spec_flux_frames,
             spec_frames_obj.sr,
             spec_frames_obj.window,
             spec_frames_obj.frame_len,
```

### Comparing `mexca-0.4.0/mexca/audio/identification.py` & `mexca-0.5.0/mexca/audio/identification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Speech segment and speaker identification.
 """
 
 import argparse
 import logging
 import os
 from typing import Optional, Union
+
 from pyannote.audio import Pipeline
+
 from mexca.data import SpeakerAnnotation
 from mexca.utils import ClassInitMessage, bool_or_str, optional_int
 
 
 class AuthenticationError(Exception):
     """Failed authentication to HuggingFace Hub.
 
@@ -48,15 +50,17 @@
     """
 
     def __init__(
         self,
         num_speakers: Optional[int] = None,
         use_auth_token: Union[bool, str] = True,
     ):
-        self.logger = logging.getLogger("mexca.audio.identification.SpeakerIdentifier")
+        self.logger = logging.getLogger(
+            "mexca.audio.identification.SpeakerIdentifier"
+        )
         self.num_speakers = num_speakers
         self.use_auth_token = use_auth_token
         # Lazy initialization
         self._pipeline = None
         self.logger.debug(ClassInitMessage())
 
     # Initialize pretrained models only when needed
@@ -64,15 +68,16 @@
     def pipeline(self) -> Pipeline:
         """The pretrained speaker diarization pipeline.
         See `pyannote.audio.SpeakerDiarization <https://github.com/pyannote/pyannote-audio/blob/develop/pyannote/audio/pipelines/speaker_diarization.py#L56>`_ for details.
         """
         if not self._pipeline:
             try:
                 self._pipeline = Pipeline.from_pretrained(
-                    "pyannote/speaker-diarization", use_auth_token=self.use_auth_token
+                    "pyannote/speaker-diarization",
+                    use_auth_token=self.use_auth_token,
                 )
 
             except EnvironmentError as exc:
                 self.logger.exception("EnvironmentError: %s", exc)
                 raise exc
 
             try:
@@ -133,15 +138,18 @@
 
     parser.add_argument("-f", "--filepath", type=str, required=True)
     parser.add_argument("-o", "--outdir", type=str, required=True)
     parser.add_argument(
         "--num-speakers", type=optional_int, default=None, dest="num_speakers"
     )
     parser.add_argument(
-        "--use-auth-token", type=bool_or_str, default=True, dest="use_auth_token"
+        "--use-auth-token",
+        type=bool_or_str,
+        default=True,
+        dest="use_auth_token",
     )
 
     args = parser.parse_args().__dict__
 
     identifier = SpeakerIdentifier(
         num_speakers=args["num_speakers"], use_auth_token=args["use_auth_token"]
     )
```

### Comparing `mexca-0.4.0/mexca/container.py` & `mexca-0.5.0/mexca/container.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,40 @@
 """Containers of pipeline components.
 """
 
 import os
 from typing import List, Optional, Tuple, Union
+
 import docker
 from docker.errors import DockerException
 from docker.types import Mount
+
 from mexca import __version__ as VERSION
-from mexca.data import (AudioTranscription, SentimentAnnotation, SpeakerAnnotation, VideoAnnotation, VoiceFeatures,
-                        VoiceFeaturesConfig)
+from mexca.data import (
+    AudioTranscription,
+    SentimentAnnotation,
+    SpeakerAnnotation,
+    VideoAnnotation,
+    VoiceFeatures,
+    VoiceFeaturesConfig,
+)
 
 
 class BaseContainer:
     """Base class for container components. Only for internal use.
 
     Parameters
     ----------
     get_latest_tag : bool, default=False
         Whether to pull the latest version of the container instead of the version matching the package version.
         This is mainly useful for debugging.
 
     """
-    mounts: Optional[None] = None
 
+    mounts: Optional[None] = None
 
     def __init__(self, image_name: str, get_latest_tag: bool = False):
         if get_latest_tag:
             self.image_name = image_name + ":latest"
         else:
             self.image_name = image_name + ":v" + str(VERSION)
         try:
@@ -47,15 +55,17 @@
         outdir = os.path.abspath(os.path.dirname(filepath))
         self.mounts = [Mount(target=self.mount_dir, source=outdir, type="bind")]
 
         return outdir
 
     @staticmethod
     def _create_out_path_stem(filepath: str, outdir: str):
-        return os.path.join(outdir, os.path.splitext(os.path.basename(filepath))[0])
+        return os.path.join(
+            outdir, os.path.splitext(os.path.basename(filepath))[0]
+        )
 
     @staticmethod
     def _create_base_cmd(filepath: str) -> List[str]:
         mount_dir = "../mnt/vol/"
         return ["-f", mount_dir + os.path.basename(filepath), "-o", mount_dir]
 
     def _run_container(self, args: List[str], show_progress: bool = True):
@@ -81,45 +91,41 @@
 
     See Also
     --------
     FaceExtractor
 
     """
 
-    def __init__( #pylint: disable=too-many-arguments,too-many-locals
+    def __init__(  # pylint: disable=too-many-arguments
         self,
         num_faces: Optional[int],
         min_face_size: int = 20,
         thresholds: Tuple[float] = (0.6, 0.7, 0.7),
         factor: float = 0.709,
         post_process: bool = True,
         select_largest: bool = True,
         selection_method: Optional[str] = None,
         keep_all: bool = True,
         device: Optional["torch.device"] = "cpu",
         max_cluster_frames: Optional[int] = None,
         embeddings_model: str = "vggface2",
-        au_model: str = "xgb",
-        landmark_model: str = "mobilefacenet",
         image_name: str = "mexca/face-extractor",
         get_latest_tag: bool = False,
     ):
         self.num_faces = num_faces
         self.min_face_size = min_face_size
         self.thresholds = thresholds
         self.factor = factor
         self.post_process = post_process
         self.select_largest = select_largest
         self.selection_method = selection_method
         self.keep_all = keep_all
         self.device = device
         self.max_cluster_frames = max_cluster_frames
         self.embeddings_model = embeddings_model
-        self.au_model = au_model
-        self.landmark_model = landmark_model
 
         super().__init__(image_name=image_name, get_latest_tag=get_latest_tag)
 
     def apply(
         self,
         filepath: str,
         batch_size: int = 1,
@@ -157,18 +163,14 @@
             self.keep_all,
             "--device",
             self.device,
             "--max-cluster-frames",
             self.max_cluster_frames,
             "--embeddings-model",
             self.embeddings_model,
-            "--au-model",
-            self.au_model,
-            "--landmark-model",
-            self.landmark_model,
         ]
 
         # Convert cli args to string (otherwise docker entrypoint can't read them)
         cmd_args_str = [str(arg) for arg in cmd_args]
 
         cmd = self._create_base_cmd(filepath=filepath)
 
@@ -242,31 +244,42 @@
     See Also
     --------
     VoiceExtractor
 
     """
 
     def __init__(
-        self, config: Optional[VoiceFeaturesConfig] = None, image_name: str = "mexca/voice-extractor", get_latest_tag: bool = False
+        self,
+        config: Optional[VoiceFeaturesConfig] = None,
+        image_name: str = "mexca/voice-extractor",
+        get_latest_tag: bool = False,
     ):
         self.config = config
         super().__init__(image_name=image_name, get_latest_tag=get_latest_tag)
 
     def apply(
         self, filepath: str, time_step: float, skip_frames: int = 1
     ) -> VoiceFeatures:
         outdir = self._create_mounts(filepath=filepath)
 
-        cmd_args = ["--time-step", str(time_step), "--skip-frames", str(skip_frames)]
+        cmd_args = [
+            "--time-step",
+            str(time_step),
+            "--skip-frames",
+            str(skip_frames),
+        ]
 
         if self.config is not None:
-            config_path = self._create_out_path_stem(filepath=filepath, outdir=outdir) + "voice_features_config.yml"
+            config_path = (
+                self._create_out_path_stem(filepath=filepath, outdir=outdir)
+                + "voice_features_config.yml"
+            )
             self.config.write_yaml(config_path)
             cmd_args.extend(["--config-filepath", config_path])
-        
+
         cmd = self._create_base_cmd(filepath=filepath)
 
         self._run_container(cmd + cmd_args)
 
         if self.config is not None:
             os.remove(config_path)
```

### Comparing `mexca-0.4.0/mexca/data.py` & `mexca-0.5.0/mexca/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import json
 import sys
 from dataclasses import asdict, dataclass, field, fields, make_dataclass
 from datetime import timedelta
 from functools import reduce
 from typing import Any, Dict, List, Optional, TextIO, Tuple, Union
+
 import numpy as np
 import pandas as pd
 import srt
 import yaml
 from intervaltree import Interval, IntervalTree
 
 
@@ -33,60 +34,62 @@
     face_aus : list, optional
         Facial action unit activations of a detected face. Is `numpy.nan` if no face was detected.
     face_label : list, optional
         Label of a detected face. Is `numpy.nan` if no face was detected.
     face_confidence : list, optional
         Confidence of the `face_label` assignment. Is `numpy.nan` if no face was detected or
         only one face label was assigned.
-
+    face_average_embeddings : list, optional
+        Average embedding vector for each face in the input video.
     """
+
     frame: Optional[List[int]] = field(default_factory=list)
     time: Optional[List[float]] = field(default_factory=list)
     face_box: Optional[List[List[float]]] = field(default_factory=list)
     face_prob: Optional[List[float]] = field(default_factory=list)
-    face_landmarks: Optional[List[List[List[float]]]] = field(default_factory=list)
+    face_landmarks: Optional[List[List[List[float]]]] = field(
+        default_factory=list
+    )
     face_aus: Optional[List[List[float]]] = field(default_factory=list)
     face_label: Optional[List[Union[str, int]]] = field(default_factory=list)
     face_confidence: Optional[List[float]] = field(default_factory=list)
-
+    face_average_embeddings: Optional[dict] = field(default_factory=dict)
 
     @classmethod
     def _from_dict(cls, data: Dict):
         field_names = [f.name for f in fields(cls)]
         filtered_data = {k: v for k, v in data.items() if k in field_names}
         return cls(**filtered_data)
 
-
     @classmethod
     def from_json(cls, filename: str):
         """Load a video annotation from a JSON file.
 
         Parameters
         ----------
         filename: str
             Name of the JSON file from which the object should be loaded.
             Must have a .json ending.
 
         """
-        with open(filename, 'r', encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             data = json.load(file)
 
         return cls._from_dict(data=data)
 
-
     def write_json(self, filename: str):
         """Write the video annotation to a JSON file.
 
         Arguments
         ---------
         filename: str
             Name of the destination file. Must have a .json ending.
 
         """
-        with open(filename, 'w', encoding='utf-8') as file:
+        with open(filename, "w", encoding="utf-8") as file:
             json.dump(asdict(self), file, allow_nan=True)
 
 
 @dataclass(frozen=True)
 class VoiceFeaturesConfig:
     """Configure the calculation of signal properties used for voice feature extraction.
 
@@ -165,14 +168,15 @@
         Upper frequency boundary for Mel spectogram transformation in Hz.
     mfcc_n: int, default=4
         Number of Mel frequency cepstral coefficients (MFCCs) that are estimated per frame.
     mfcc_lifter: float, default=22.0
         Cepstral liftering coefficient for MFCC estimation. Must be >= 0. If zero, no liftering is applied.
 
     """
+
     frame_len: int = 1024
     hop_len: int = 256
     center: bool = True
     pad_mode: str = "constant"
     spec_window: Optional[Union[str, float, Tuple]] = "hann"
     pitch_lower_freq: float = 75.0
     pitch_upper_freq: float = 600.0
@@ -211,16 +215,20 @@
         if isinstance(obj, list):
             return tuple(cls._transform_sequence(e) for e in obj)
         return obj
 
     @classmethod
     def _from_dict(cls, data: Dict):
         field_names = [f.name for f in fields(cls)]
-        filtered_data = {k: cls._transform_sequence(v) for k, v in data.items() if k in field_names}
-        
+        filtered_data = {
+            k: cls._transform_sequence(v)
+            for k, v in data.items()
+            if k in field_names
+        }
+
         return cls(**filtered_data)
 
     @classmethod
     def from_yaml(cls, filename: str):
         """Load a voice configuration object from a YAML file.
 
         Uses safe YAML loading (only supports native YAML but no Python tags).
@@ -228,32 +236,31 @@
 
         Parameters
         ----------
         filename: str
             Path to the YAML file. Must have a .yml or .yaml ending.
 
         """
-        with open(filename, 'r', encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             config_dict = yaml.safe_load(file)
 
         return cls._from_dict(config_dict)
-       
 
     def write_yaml(self, filename: str):
         """Write a voice configuration object to a YAML file.
 
         Uses safe YAML dumping (only supports native YAML but no Python tags).
 
         Parameters
         ----------
         filename: str
             Path to the YAML file. Must have a .yml or .yaml ending.
 
         """
-        with open(filename, 'w', encoding='utf-8') as file:
+        with open(filename, "w", encoding="utf-8") as file:
             yaml.safe_dump(asdict(self), file)
 
 
 @dataclass
 class VoiceFeatures:
     """Class for storing voice features.
 
@@ -264,82 +271,92 @@
     ----------
     frame: list
         The frame index for which features were extracted.
     time: list
         The time stamp at which features were extracted.
 
     """
+
     frame: List[int]
     time: List[float]
 
-
     def add_attributes(self, attr_names: List[str]):
-        self.__class__ = make_dataclass('VoiceFeatures', fields=attr_names, bases=(self.__class__,))
-
+        self.__class__ = make_dataclass(
+            "VoiceFeatures", fields=attr_names, bases=(self.__class__,)
+        )
 
     def add_feature(self, name: str, feature: List):
         if not isinstance(feature, list):
             try:
                 feature = feature.tolist()
             except Exception as exc:
-                raise Exception(f'Feature must be a list, not {type(feature)}') from exc
-        
+                raise Exception(
+                    f"Feature must be a list, not {type(feature)}"
+                ) from exc
+
         feature_len = len(feature)
         if feature_len != len(self.frame) and feature_len != 1:
-            raise Exception(f'Feature must have same length as frame attribute or length 1 but has length {feature_len}')
-        
-        setattr(self, name, feature)
+            raise Exception(
+                f"Feature must have same length as frame attribute or length 1 but has length {feature_len}"
+            )
 
+        setattr(self, name, feature)
 
     @classmethod
     def _from_dict(cls, data: Dict):
         field_names = [f.name for f in fields(cls)]
         filtered_data = {k: v for k, v in data.items() if k in field_names}
         remaining_data = {k: v for k, v in data.items() if k not in field_names}
         obj = cls(**filtered_data)
         obj.add_attributes(remaining_data.keys())
         for key in remaining_data:
             obj.add_feature(key, remaining_data[key])
         return obj
 
-
     @classmethod
     def from_json(cls, filename: str):
         """Load voice features from a JSON file.
 
         Parameters
         ----------
         filename: str
             Name of the JSON file from which the object should be loaded.
             Must have a .json ending.
 
         """
-        with open(filename, 'r', encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             data = json.load(file)
 
         return cls._from_dict(data=data)
 
-
     def write_json(self, filename: str):
         """Store voice features in a JSON file.
 
         Arguments
         ---------
         filename: str
             Name of the destination file. Must have a .json ending.
 
         """
-        with open(filename, 'w', encoding='utf-8') as file:
+        with open(filename, "w", encoding="utf-8") as file:
             json.dump(asdict(self), file, allow_nan=True)
 
 
 def _get_rttm_header() -> List[str]:
-    return ["type", "file", "chnl", "tbeg",
-            "tdur", "ortho", "stype", "name",
-            "conf"]
+    return [
+        "type",
+        "file",
+        "chnl",
+        "tbeg",
+        "tdur",
+        "ortho",
+        "stype",
+        "name",
+        "conf",
+    ]
 
 
 @dataclass
 class SegmentData:
     """Class for storing speech segment data.
 
     Parameters
@@ -350,120 +367,130 @@
         Channel index.
     name : str, optional, default=None
         Speaker label.
     conf : float, optional, default=None
         Confidence of speaker label.
 
     """
+
     filename: str
     channel: int
     name: Optional[int] = None
     conf: Optional[float] = None
 
 
 class SpeakerAnnotation(IntervalTree):
     """Class for storing speaker and speech segment annotations.
 
     Stores speech segments as ``intervaltree.Interval`` in an ``intervaltree.IntervalTree``.
     Speaker labels are stored in `SegmentData` objects in the `data` attribute of each interval.
 
     """
+
     def __init__(self, intervals: List[Interval] = None):
         super().__init__(intervals)
 
-
-    def __str__(self, end: str = "\t", file: TextIO = sys.stdout, header: bool = True):
+    def __str__(
+        self, end: str = "\t", file: TextIO = sys.stdout, header: bool = True
+    ):
         if header:
             for h in _get_rttm_header():
                 print(h, end=end, file=file)
 
             print("", file=file)
 
         for seg in self.items():
             for col in (
-                "SPEAKER", seg.data.filename, seg.data.channel, seg.begin, seg.end-seg.begin,
-                None, None, seg.data.name, seg.data.conf
+                "SPEAKER",
+                seg.data.filename,
+                seg.data.channel,
+                seg.begin,
+                seg.end - seg.begin,
+                None,
+                None,
+                seg.data.name,
+                seg.data.conf,
             ):
                 if col is not None:
                     if isinstance(col, float):
                         col = round(col, 2)
                     print(col, end=end, file=file)
                 else:
-                    print('<NA>', end=end, file=file)
+                    print("<NA>", end=end, file=file)
 
             print("", file=file)
 
         return ""
 
-
     @classmethod
     def from_pyannote(cls, annotation: Any):
         """Create a `SpeakerAnnotation` object from a ``pyannote.core.Annotation`` object.
 
         Parameters
         ----------
         annotation : pyannote.core.Annotation
             Annotation object containing speech segments and speaker labels.
 
         """
         segments = []
 
         for seg, _, spk in annotation.itertracks(yield_label=True):
-            segments.append(Interval(
-                begin=seg.start,
-                end=seg.end,
-                data=SegmentData(
-                    filename=annotation.uri,
-                    channel=1,
-                    name=str(spk)
+            segments.append(
+                Interval(
+                    begin=seg.start,
+                    end=seg.end,
+                    data=SegmentData(
+                        filename=annotation.uri, channel=1, name=str(spk)
+                    ),
                 )
-            ))
+            )
 
         return cls(intervals=segments)
 
-
     @classmethod
     def from_rttm(cls, filename: str):
         """Load a speaker annotation from an RTTM file.
 
         Parameters
         ----------
         filename : str
             Path to the file. Must have an RTTM ending.
 
         """
-        with open(filename, "r", encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             segments = []
             for row in file:
-                row_split = [None if cell == "<NA>" else cell for cell in row.split(" ")]
+                row_split = [
+                    None if cell == "<NA>" else cell for cell in row.split(" ")
+                ]
                 segment = Interval(
                     begin=float(row_split[3]),
                     end=float(row_split[3]) + float(row_split[4]),
                     data=SegmentData(
                         filename=row_split[1],
                         channel=int(row_split[2]),
                         name=row_split[7],
-                    )
+                    ),
                 )
                 segments.append(segment)
 
             return cls(segments)
 
-
+    # pylint: disable=unnecessary-dunder-call
     def write_rttm(self, filename: str):
         """Write a speaker annotation to an RTTM file.
 
         Parameters
         ----------
         filename : str
             Path to the file. Must have an RTTM ending.
 
         """
-        with open(filename, "w", encoding='utf-8') as file:
-            self.__str__(end=" ", file=file, header=False) #pylint: disable=unnecessary-dunder-call
+        with open(filename, "w", encoding="utf-8") as file:
+            self.__str__(end=" ", file=file, header=False)
 
 
 @dataclass
 class TranscriptionData:
     """Class for storing transcription data.
 
     Parameters
@@ -472,94 +499,95 @@
         Index of the transcribed sentence.
     text: str
         Transcribed text.
     speaker: str, optional
         Speaker of the transcribed text.
 
     """
+
     index: int
     text: str
     speaker: Optional[str] = None
+    confidence: Optional[float] = None  # probability of transcription accuracy
 
 
 class AudioTranscription:
     """Class for storing audio transcriptions.
 
     Parameters
     ----------
     filename: str
         Name of the transcribed audio file.
     subtitles: intervaltree.IntervalTree, optional, default=None
         Interval tree containing the transcribed speech segments split into sentences as intervals.
         The transcribed sentences are stored in the `data` attribute of each interval.
 
     """
-    def __init__(self,
-        filename: str,
-        subtitles: Optional[IntervalTree] = None
-    ):
+
+    def __init__(self, filename: str, subtitles: Optional[IntervalTree] = None):
         self.filename = filename
         self.subtitles = subtitles
 
-
     def __len__(self) -> int:
         return len(self.subtitles)
 
-
     @classmethod
     def from_srt(cls, filename: str):
         """Load an audio transcription from an SRT file.
 
         Parameters
         ----------
         filename: str
             Name of the file to be loaded. Must have an .srt ending.
 
         """
-        with open(filename, 'r', encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             subtitles = srt.parse(file)
 
             intervals = []
 
             for sub in subtitles:
-                content = sub.content.split('>')
-                intervals.append(Interval(
-                    begin=sub.start.total_seconds(),
-                    end=sub.end.total_seconds(),
-                    data=TranscriptionData(
-                        index=sub.index,
-                        text=content[1],
-                        speaker=content[0][1:]
+                content = sub.content.split(">")
+                intervals.append(
+                    Interval(
+                        begin=sub.start.total_seconds(),
+                        end=sub.end.total_seconds(),
+                        data=TranscriptionData(
+                            index=sub.index,
+                            text=content[1],
+                            speaker=content[0][1:],
+                        ),
                     )
-                ))
+                )
 
             return cls(filename=filename, subtitles=IntervalTree(intervals))
 
-
     def write_srt(self, filename: str):
         """Write an audio transcription to an SRT file
 
         Parameters
         ----------
         filename: str
             Name of the file to write to. Must have an .srt ending.
 
         """
         subtitles = []
 
         for iv in self.subtitles.all_intervals:
             content = f"<{iv.data.speaker}> {iv.data.text}"
-            subtitles.append(srt.Subtitle(
-                index=iv.data.index,
-                start=timedelta(seconds=iv.begin),
-                end=timedelta(seconds=iv.end),
-                content=content
-            ))
+            subtitles.append(
+                srt.Subtitle(
+                    index=iv.data.index,
+                    start=timedelta(seconds=iv.begin),
+                    end=timedelta(seconds=iv.end),
+                    content=content,
+                )
+            )
 
-        with open(filename, 'w', encoding='utf-8') as file:
+        with open(filename, "w", encoding="utf-8") as file:
             file.write(srt.compose(subtitles))
 
 
 @dataclass
 class SentimentData:
     """Class for storing sentiment data.
 
@@ -571,78 +599,80 @@
         Positive sentiment score.
     neg: float
         Negative sentiment score.
     neu: float
         Neutral sentiment score.
 
     """
+
     text: str
     pos: float
     neg: float
     neu: float
 
 
 @dataclass
 class SentimentAnnotation(IntervalTree):
     """Class for storing sentiment scores of transcribed sentences.
 
     Stores sentiment scores as intervals in an interval tree. The scores are stored in the `data` attribute of each interval.
 
     """
+
     def __init__(self, intervals: List[Interval] = None):
         super().__init__(intervals)
 
-
     @classmethod
     def from_json(cls, filename: str):
         """Load a sentiment annotation from a JSON file.
 
         Parameters
         ----------
         filename: str
             Name of the JSON file from which the object should be loaded.
             Must have a .json ending.
 
         """
-        with open(filename, 'r', encoding='utf-8') as file:
+        with open(filename, "r", encoding="utf-8") as file:
             sentiment = json.load(file)
 
             intervals = []
 
             for sen in sentiment:
-                intervals.append(Interval(
-                    begin=sen['begin'],
-                    end=sen['end'],
-                    data=SentimentData(
-                        text=sen['text'],
-                        pos=sen['pos'],
-                        neg=sen['neg'],
-                        neu=sen['neu']
+                intervals.append(
+                    Interval(
+                        begin=sen["begin"],
+                        end=sen["end"],
+                        data=SentimentData(
+                            text=sen["text"],
+                            pos=sen["pos"],
+                            neg=sen["neg"],
+                            neu=sen["neu"],
+                        ),
                     )
-                ))
+                )
 
             return cls(intervals=intervals)
 
-
     def write_json(self, filename: str):
         """Write a sentiment annotation to a JSON file.
 
         Parameters
         ----------
         filename: str
             Name of the destination file. Must have a .json ending.
 
         """
-        with open(filename, 'w', encoding='utf-8') as file:
+        with open(filename, "w", encoding="utf-8") as file:
             sentiment = []
 
             for iv in self.all_intervals:
                 data_dict = asdict(iv.data)
-                data_dict['begin'] = iv.begin
-                data_dict['end'] = iv.end
+                data_dict["begin"] = iv.begin
+                data_dict["end"] = iv.end
                 sentiment.append(data_dict)
 
             json.dump(sentiment, file, allow_nan=True)
 
 
 class Multimodal:
     """Class for storing multimodal features.
@@ -670,136 +700,177 @@
         Object containing transcribed speech segments split into sentences.
     sentiment : SentimentAnnotation
         Object containing sentiment scores for transcribed sentences.
     features : pandas.DataFrame
         Merged features.
 
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         filename: str,
         duration: Optional[float] = None,
         fps: Optional[int] = None,
         fps_adjusted: Optional[int] = None,
         video_annotation: Optional[VideoAnnotation] = None,
         audio_annotation: Optional[SpeakerAnnotation] = None,
         voice_features: Optional[VoiceFeatures] = None,
         transcription: Optional[AudioTranscription] = None,
         sentiment: Optional[SentimentAnnotation] = None,
-        features: Optional[pd.DataFrame] = None
+        features: Optional[pd.DataFrame] = None,
     ):
         self.filename = filename
         self.duration = duration
         self.fps = fps
         self.fps_adjusted = fps if fps_adjusted is None else fps_adjusted
         self.video_annotation = video_annotation
         self.audio_annotation = audio_annotation
         self.voice_features = voice_features
         self.transcription = transcription
         self.sentiment = sentiment
         self.features = features
 
-
     def _merge_video_annotation(self, data_frames: List):
+        # create a new VideoAnnotation instance and copy all fields to the new instance
+        # (except for average face embeddings) because the face embeddings have a different
+        # dimension to the other fields in the instance. if we include the face embeddings
+        # then the conversion of the data to a dataframe would fail.
         if self.video_annotation:
-            data_frames.append(pd.DataFrame(asdict(self.video_annotation)))
-
+            video_annotation_dict = asdict(self.video_annotation)
+            del video_annotation_dict["face_average_embeddings"]
+            data_frames.append(pd.DataFrame(video_annotation_dict))
+
+            # video_annotation_minus_avg_face_embeddings = VideoAnnotation()
+            # video_annotation_minus_avg_face_embeddings.frame = self.video_annotation.frame
+            # video_annotation_minus_avg_face_embeddings.time = self.video_annotation.time
+            # video_annotation_minus_avg_face_embeddings.face_box = self.video_annotation.face_box
+            # video_annotation_minus_avg_face_embeddings.face_prob = self.video_annotation.face_prob
+            # video_annotation_minus_avg_face_embeddings.face_landmarks = self.video_annotation.face_landmarks
+            # video_annotation_minus_avg_face_embeddings.face_aus = self.video_annotation.face_aus
+            # video_annotation_minus_avg_face_embeddings.face_label = self.video_annotation.face_label
+            # video_annotation_minus_avg_face_embeddings.face_confidence = self.video_annotation.face_confidence
+            # # ensure that the average face embeddings field is excluded from the instance
+            # video_annotation_minus_avg_face_embeddings.face_average_embeddings = None
+            # dict_version = asdict(video_annotation_minus_avg_face_embeddings)
+            # del dict_version['face_average_embeddings']
+            # data_frames.append(pd.DataFrame(dict_version))
 
     def _merge_audio_text_features(self, data_frames: List):
         if self.audio_annotation:
             audio_annotation_dict = {
                 "frame": [],
                 "segment_start": [],
                 "segment_end": [],
-                "segment_speaker_label": []
+                "segment_speaker_label": [],
             }
 
-            time = np.arange(0.0, self.duration, 1/self.fps_adjusted, dtype=np.float32)
-            frame = np.arange(0, self.duration*self.fps, self.fps/self.fps_adjusted, dtype=np.int32)
+            time = np.arange(
+                0.0, self.duration, 1 / self.fps_adjusted, dtype=np.float32
+            )
+            frame = np.arange(
+                0,
+                self.duration * self.fps,
+                self.fps / self.fps_adjusted,
+                dtype=np.int32,
+            )
 
             if self.transcription:
                 text_features_dict = {
                     "frame": [],
                     "span_start": [],
                     "span_end": [],
                     "span_text": [],
-                    "segment_speaker_label": []
+                    "segment_speaker_label": [],
+                    "confidence": [],  # store confidence of transcription accuracy
                 }
 
                 if self.sentiment:
                     sentiment_dict = {
                         "frame": [],
                         "span_text": [],
                         "span_sent_pos": [],
                         "span_sent_neg": [],
-                        "span_sent_neu": []
+                        "span_sent_neu": [],
                     }
 
             for i, t in zip(frame, time):
                 overlap_segments = self.audio_annotation[t]
 
                 if len(overlap_segments) > 0:
                     for seg in overlap_segments:
-                        audio_annotation_dict['frame'].append(i)
-                        audio_annotation_dict['segment_start'].append(seg.begin)
-                        audio_annotation_dict['segment_end'].append(seg.end)
-                        audio_annotation_dict['segment_speaker_label'].append(str(seg.data.name))
+                        audio_annotation_dict["frame"].append(i)
+                        audio_annotation_dict["segment_start"].append(seg.begin)
+                        audio_annotation_dict["segment_end"].append(seg.end)
+                        audio_annotation_dict["segment_speaker_label"].append(
+                            str(seg.data.name)
+                        )
                 else:
-                    audio_annotation_dict['frame'].append(i)
-                    audio_annotation_dict['segment_start'].append(np.NaN)
-                    audio_annotation_dict['segment_end'].append(np.NaN)
-                    audio_annotation_dict['segment_speaker_label'].append(np.NaN)
+                    audio_annotation_dict["frame"].append(i)
+                    audio_annotation_dict["segment_start"].append(np.NaN)
+                    audio_annotation_dict["segment_end"].append(np.NaN)
+                    audio_annotation_dict["segment_speaker_label"].append(
+                        np.NaN
+                    )
 
                 if self.transcription:
-                    for span in self.transcription.subtitles[t]:      
-                        text_features_dict['frame'].append(i)
-                        text_features_dict['span_start'].append(span.begin)
-                        text_features_dict['span_end'].append(span.end)
-                        text_features_dict['span_text'].append(span.data.text)
-                        text_features_dict['segment_speaker_label'].append(span.data.speaker)
+                    for span in self.transcription.subtitles[t]:
+                        text_features_dict["frame"].append(i)
+                        text_features_dict["span_start"].append(span.begin)
+                        text_features_dict["span_end"].append(span.end)
+                        text_features_dict["span_text"].append(span.data.text)
+                        text_features_dict["segment_speaker_label"].append(
+                            span.data.speaker
+                        )
+                        text_features_dict["confidence"].append(
+                            span.data.confidence
+                        )  # store confidence of transcription accuracy
 
                     if self.sentiment:
                         for sent in self.sentiment[t]:
-                            sentiment_dict['frame'].append(i)
-                            sentiment_dict['span_text'].append(sent.data.text)
-                            sentiment_dict['span_sent_pos'].append(sent.data.pos)
-                            sentiment_dict['span_sent_neg'].append(sent.data.neg)
-                            sentiment_dict['span_sent_neu'].append(sent.data.neu)
+                            sentiment_dict["frame"].append(i)
+                            sentiment_dict["span_text"].append(sent.data.text)
+                            sentiment_dict["span_sent_pos"].append(
+                                sent.data.pos
+                            )
+                            sentiment_dict["span_sent_neg"].append(
+                                sent.data.neg
+                            )
+                            sentiment_dict["span_sent_neu"].append(
+                                sent.data.neu
+                            )
 
             audio_text_features_df = pd.DataFrame(audio_annotation_dict)
 
             if self.transcription:
-                text_features_df =  pd.DataFrame(text_features_dict)
+                text_features_df = pd.DataFrame(text_features_dict)
                 if self.sentiment:
                     text_features_df = text_features_df.merge(
                         pd.DataFrame(sentiment_dict),
-                        on=['frame', 'span_text'],
-                        how='left'
+                        on=["frame", "span_text"],
+                        how="left",
                     )
 
                 audio_text_features_df = audio_text_features_df.merge(
                     text_features_df,
-                    on=['frame', 'segment_speaker_label'],
-                    how='left'
+                    on=["frame", "segment_speaker_label"],
+                    how="left",
                 )
 
             data_frames.append(audio_text_features_df)
 
-
     def _merge_voice_features(self, data_frames: List):
         if self.voice_features:
             data_frames.append(pd.DataFrame(asdict(self.voice_features)))
 
-
     @staticmethod
     def _delete_time_col(df: pd.DataFrame) -> pd.DataFrame:
-        if 'time' in df.columns:
-            del df['time']
+        if "time" in df.columns:
+            del df["time"]
         return df
 
-
     def merge_features(self) -> pd.DataFrame:
         """Merge multimodal features from pipeline components into a common data frame.
 
         Transforms and merges the available output stored in the `Multimodal` object
         based on the `'frame'` variable. Stores the merged features as a `pandas.DataFrame`
         in the `features` attribute.
 
@@ -816,19 +887,19 @@
 
         self._merge_audio_text_features(data_frames=dfs)
 
         self._merge_voice_features(data_frames=dfs)
 
         if len(dfs) > 0:
             dfs = map(self._delete_time_col, dfs)
-            self.features = reduce(lambda left, right:
-                pd.merge(left , right,
-                    on = ["frame"],
-                    how = "left"),
-                dfs
+            self.features = reduce(
+                lambda left, right: pd.merge(
+                    left, right, on=["frame"], how="left"
+                ),
+                dfs,
             )
 
-            time = self.features.frame * (1/self.fps)
+            time = self.features.frame * (1 / self.fps)
 
-            self.features.insert(1, 'time', time)
+            self.features.insert(1, "time", time)
 
         return self.features
```

### Comparing `mexca-0.4.0/mexca/pipeline.py` & `mexca-0.5.0/mexca/pipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Build a pipeline to extract emotion expression features from a video file.
 """
 
 import logging
 import logging.config
 import os
 from typing import Optional, Tuple, Union
+
 from moviepy.editor import VideoFileClip
+
 from mexca.data import Multimodal
 from mexca.utils import ClassInitMessage
 
 
 class Pipeline:
     """Build a pipeline to extract emotion expression features from a video file.
 
@@ -80,39 +82,52 @@
     ...     ),
     ...     voice_extractor=VoiceExtractor(), # standard
     ...     audio_transcriber=AudioTranscriberContainer(),
     ...     sentiment_extractor=SentimentExtractorContainer()
     ... )
 
     """
-    def __init__(self,
-        face_extractor: Optional[Union['FaceExtractor', 'FaceExtractorContainer']] = None,
-        speaker_identifier: Optional[Union['SpeakerIdentifier', 'SpeakerIdentifierContainer']] = None,
-        voice_extractor: Optional[Union['VoiceExtractor', 'VoiceExtractorContainer']] = None,
-        audio_transcriber: Optional[Union['AudioTranscriber', 'AudioTranscriberContainer']] = None,
-        sentiment_extractor: Optional[Union['SentimentExtractor', 'SentimentExtractorContainer']] = None
+
+    def __init__(
+        self,
+        face_extractor: Optional[
+            Union["FaceExtractor", "FaceExtractorContainer"]
+        ] = None,
+        speaker_identifier: Optional[
+            Union["SpeakerIdentifier", "SpeakerIdentifierContainer"]
+        ] = None,
+        voice_extractor: Optional[
+            Union["VoiceExtractor", "VoiceExtractorContainer"]
+        ] = None,
+        audio_transcriber: Optional[
+            Union["AudioTranscriber", "AudioTranscriberContainer"]
+        ] = None,
+        sentiment_extractor: Optional[
+            Union["SentimentExtractor", "SentimentExtractorContainer"]
+        ] = None,
     ):
-        self.logger = logging.getLogger('mexca.pipeline.Pipeline')
+        self.logger = logging.getLogger("mexca.pipeline.Pipeline")
         self.face_extractor = face_extractor
         self.speaker_identifier = speaker_identifier
         self.voice_extractor = voice_extractor
         self.audio_transcriber = audio_transcriber
         self.sentiment_extractor = sentiment_extractor
         self.logger.debug(ClassInitMessage())
 
-
-    def apply(self, # pylint: disable=too-many-locals
+    # pylint: disable=too-many-locals
+    def apply(
+        self,
         filepath: str,
         frame_batch_size: int = 1,
         skip_frames: int = 1,
         process_subclip: Tuple[Optional[float]] = (0, None),
         language: Optional[str] = None,
         keep_audiofile: bool = False,
-        show_progress: bool = True
-    ) -> 'Multimodal':
+        show_progress: bool = True,
+    ) -> "Multimodal":
         """
         Extract emotion expression features from a video file.
 
         This is the main function to apply the complete mexca pipeline to a video file.
 
         Parameters
         ----------
@@ -151,84 +166,86 @@
         >>> output = pipeline.apply(filepath)
         >>> assert isinstance(output.features, pd.DataFrame)
         True
 
         """
         if show_progress:
             logging.getLogger(__name__).setLevel(logging.INFO)
-            
 
-        self.logger.info('Starting MEXCA pipeline')
+        self.logger.info("Starting MEXCA pipeline")
         output = Multimodal(filename=filepath)
 
         with VideoFileClip(filepath) as clip:
-            audio_path = os.path.splitext(filepath)[0] + '.wav'
-            subclip = clip.subclip(
-                process_subclip[0],
-                process_subclip[1]
+            audio_path = os.path.splitext(filepath)[0] + ".wav"
+            subclip = clip.subclip(process_subclip[0], process_subclip[1])
+            self.logger.debug(
+                "Reading video file from %s to %s", subclip.start, subclip.end
             )
-            self.logger.debug('Reading video file from %s to %s', subclip.start, subclip.end)
             output.duration = subclip.duration
             output.fps = subclip.fps
             output.fps_adjusted = subclip.fps / skip_frames
             time_step = 1 / (subclip.fps / skip_frames)
 
             if self.speaker_identifier or self.voice_extractor:
-                self.logger.debug('Writing audio file')
-                subclip.audio.write_audiofile(audio_path, logger=None, fps=16000, ffmpeg_params=["-ac", "1"])
-                self.logger.info('Wrote audio file to %s', audio_path)
+                self.logger.debug("Writing audio file")
+                subclip.audio.write_audiofile(
+                    audio_path,
+                    logger=None,
+                    fps=16000,
+                    ffmpeg_params=["-ac", "1"],
+                )
+                self.logger.info("Wrote audio file to %s", audio_path)
 
         if self.face_extractor:
-            self.logger.info('Processing video frames')
+            self.logger.info("Processing video frames")
             video_annotation = self.face_extractor.apply(
                 filepath,
                 batch_size=frame_batch_size,
                 skip_frames=skip_frames,
                 process_subclip=process_subclip,
-                show_progress=show_progress
+                show_progress=show_progress,
             )
             output.video_annotation = video_annotation
 
         if self.speaker_identifier:
-            self.logger.info('Identifying speakers')
+            self.logger.info("Identifying speakers")
             audio_annotation = self.speaker_identifier.apply(audio_path)
 
             output.audio_annotation = audio_annotation
 
             if self.audio_transcriber:
-                self.logger.info('Transcribing speech segments to text')
+                self.logger.info("Transcribing speech segments to text")
                 transcription = self.audio_transcriber.apply(
                     audio_path,
                     audio_annotation,
                     language=language,
-                    show_progress=show_progress
+                    show_progress=show_progress,
                 )
 
                 output.transcription = transcription
 
                 if self.sentiment_extractor:
-                    self.logger.info('Extracting sentiment from transcribed text')
+                    self.logger.info(
+                        "Extracting sentiment from transcribed text"
+                    )
                     sentiment = self.sentiment_extractor.apply(
-                        transcription=transcription,
-                        show_progress=show_progress
+                        transcription=transcription, show_progress=show_progress
                     )
 
                     output.sentiment = sentiment
 
         if self.voice_extractor:
-            self.logger.info('Extracting voice features')
+            self.logger.info("Extracting voice features")
             voice_features = self.voice_extractor.apply(
-                audio_path,
-                time_step=time_step,
-                skip_frames=skip_frames
+                audio_path, time_step=time_step, skip_frames=skip_frames
             )
 
             output.voice_features = voice_features
 
         output.merge_features()
 
         if not keep_audiofile and os.path.exists(audio_path):
-            self.logger.info('Removing audio file at %s', audio_path)
+            self.logger.info("Removing audio file at %s", audio_path)
             os.remove(audio_path)
 
-        self.logger.info('MEXCA pipeline finished')
+        self.logger.info("MEXCA pipeline finished")
         return output
```

### Comparing `mexca-0.4.0/mexca/text/sentiment.py` & `mexca-0.5.0/mexca/text/sentiment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,25 @@
 """Extract sentiment from text.
 """
 
 import argparse
 import logging
 import os
 from typing import Optional
+
 import torch
 from intervaltree import Interval
 from scipy.special import softmax
 from tqdm import tqdm
-from transformers import AutoModelForSequenceClassification, AutoTokenizer, XLMRobertaForSequenceClassification
+from transformers import (
+    AutoModelForSequenceClassification,
+    AutoTokenizer,
+    XLMRobertaForSequenceClassification,
+)
+
 from mexca.data import AudioTranscription, SentimentAnnotation, SentimentData
 from mexca.utils import ClassInitMessage, str2bool
 
 
 class SentimentExtractor:
     """Extract sentiment from text.
 
@@ -28,56 +34,67 @@
     Attributes
     ----------
     tokenizer: transformers.PreTrainedTokenizer
         The pretrained tokenizer for sequence classification.
         Loaded automatically from `model_name`.
 
     """
-    def __init__(self, model_name: Optional[str] = None, device: Optional[torch.device] = None):
-        self.logger = logging.getLogger('mexca.text.extraction.SentimentExtractor')
+
+    def __init__(
+        self,
+        model_name: Optional[str] = None,
+        device: Optional[torch.device] = None,
+    ):
+        self.logger = logging.getLogger(
+            "mexca.text.extraction.SentimentExtractor"
+        )
         if not model_name:
             model_name = "cardiffnlp/twitter-xlm-roberta-base-sentiment"
-            self.logger.debug('Using default pretrained model %s because "model_name=None"', model_name)
+            self.logger.debug(
+                'Using default pretrained model %s because "model_name=None"',
+                model_name,
+            )
 
         if device is None:
             device = "cpu"
 
         self.device = device
         self.model_name = model_name
         self.tokenizer = AutoTokenizer.from_pretrained(model_name)
         # Lazy initialization
         self._classifier = None
         self.logger.debug(ClassInitMessage())
 
-
     # Initialize pretrained models only when needed
     @property
     def classifier(self) -> XLMRobertaForSequenceClassification:
         """The pretrained sequence classification model for sentiment prediction.
         Loaded automatically from `model_name`.
         """
         if not self._classifier:
-            self._classifier = AutoModelForSequenceClassification.from_pretrained(
-                self.model_name,
-                device_map="auto",
-                load_in_8bit=self.device == "cuda"
+            self._classifier = (
+                AutoModelForSequenceClassification.from_pretrained(
+                    self.model_name,
+                    device_map="auto",
+                    load_in_8bit=self.device == "cuda",
+                )
             )
-            self.logger.debug('Initialized sentiment extraction model')
+            self.logger.debug("Initialized sentiment extraction model")
 
         return self._classifier
 
-
     # Delete pretrained models when not needed anymore
     @classifier.deleter
     def classifier(self):
         self._classifier = None
-        self.logger.debug('Removed sentiment extraction model')
-
+        self.logger.debug("Removed sentiment extraction model")
 
-    def apply(self, transcription: AudioTranscription, show_progress: bool = True) -> SentimentAnnotation:
+    def apply(
+        self, transcription: AudioTranscription, show_progress: bool = True
+    ) -> SentimentAnnotation:
         """Extract the sentiment from text.
 
         Iterates over the sentences in the audio transcription and predicts the sentiment
         (negative, neutral, positive).
 
         Parameters
         ----------
@@ -93,53 +110,78 @@
             An data class object with the positive, negative, and neutral sentiment scores
             for each sentence.
 
         """
 
         sentiment_annotation = SentimentAnnotation()
 
-        for i, sent in tqdm(enumerate(transcription.subtitles), total=len(transcription), disable=not show_progress):
-            self.logger.debug('Extracting sentiment for sentence %s', i)
-            tokens = self.tokenizer(sent.data.text, return_tensors='pt').to(self.device)
+        for i, sent in tqdm(
+            enumerate(transcription.subtitles),
+            total=len(transcription),
+            disable=not show_progress,
+        ):
+            self.logger.debug("Extracting sentiment for sentence %s", i)
+            tokens = self.tokenizer(sent.data.text, return_tensors="pt").to(
+                self.device
+            )
             output = self.classifier(**tokens)
             logits = output.logits.detach().cpu().numpy()
             scores = softmax(logits)[0]
-            sentiment_annotation.add(Interval(
-                begin=sent.begin,
-                end=sent.end,
-                data=SentimentData(
-                    text=sent.data.text,
-                    pos=float(scores[2]),
-                    neg=float(scores[0]),
-                    neu=float(scores[1])
-            )))
+            sentiment_annotation.add(
+                Interval(
+                    begin=sent.begin,
+                    end=sent.end,
+                    data=SentimentData(
+                        text=sent.data.text,
+                        pos=float(scores[2]),
+                        neg=float(scores[0]),
+                        neu=float(scores[1]),
+                    ),
+                )
+            )
 
         del self.classifier
 
         return sentiment_annotation
 
 
 def cli():
     """Command line interface for sentiment extraction.
     See `extract-sentiment -h` for details.
     """
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-
-    parser.add_argument('-t', '--transcription-path', type=str, required=True, dest='transcription_path')
-    parser.add_argument('-o', '--outdir', type=str, required=True)
-    parser.add_argument('--show-progress', type=str2bool, default=True, dest='show_progress')
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
+
+    parser.add_argument(
+        "-t",
+        "--transcription-path",
+        type=str,
+        required=True,
+        dest="transcription_path",
+    )
+    parser.add_argument("-o", "--outdir", type=str, required=True)
+    parser.add_argument(
+        "--show-progress", type=str2bool, default=True, dest="show_progress"
+    )
 
     args = parser.parse_args().__dict__
 
     extractor = SentimentExtractor()
 
-    transcription = AudioTranscription.from_srt(args['transcription_path'])
+    transcription = AudioTranscription.from_srt(args["transcription_path"])
 
-    output = extractor.apply(transcription, show_progress=args['show_progress'])
+    output = extractor.apply(transcription, show_progress=args["show_progress"])
 
-    base_name = "_".join(os.path.splitext(os.path.basename(args['transcription_path']))[0].split('_')[:-1])
+    base_name = "_".join(
+        os.path.splitext(os.path.basename(args["transcription_path"]))[0].split(
+            "_"
+        )[:-1]
+    )
 
-    output.write_json(os.path.join(args['outdir'], base_name + '_sentiment.json'))
+    output.write_json(
+        os.path.join(args["outdir"], base_name + "_sentiment.json")
+    )
 
 
-if __name__ == '__main__':
-    cli()
+if __name__ == "__main__":
+    cli()
```

### Comparing `mexca-0.4.0/mexca/text/transcription.py` & `mexca-0.5.0/mexca/text/transcription.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,26 +4,27 @@
 import argparse
 import logging
 import os
 import re
 import warnings
 from dataclasses import asdict
 from typing import Optional, Union
-import stable_whisper
+
 import torch
 import whisper
 from intervaltree import Interval, IntervalTree
 from tqdm import tqdm
 from whisper.audio import SAMPLE_RATE
+
 from mexca.data import AudioTranscription, SpeakerAnnotation, TranscriptionData
 from mexca.utils import ClassInitMessage, optional_str, str2bool
 
-
 # To filter out shift warnings which do not apply here
-warnings.simplefilter('ignore', category=UserWarning)
+warnings.simplefilter("ignore", category=UserWarning)
+
 
 class AudioTranscriber:
     """Transcribe speech from audio to text.
 
     Parameters
     ----------
     whisper_model: str, optional, default='small'
@@ -34,62 +35,74 @@
         available, this can be `'cuda'`, otherwise use `'cpu'` (the default).
     sentence_rule: str, optional
         A regular expression used to split segment transcripts into sentences. If `None` (default), it splits
         the text at all '.', '?', '!', and ':' characters that are followed by whitespace characters. It
         omits single or multiple words abbreviated with dots (e.g., 'Nr. ' and 'e.g. ').
 
     """
-    def __init__(self,
-        whisper_model: Optional[str] = 'small',
-        device: Optional[Union[str, torch.device]] = 'cpu',
-        sentence_rule: Optional[str] = None
+
+    def __init__(
+        self,
+        whisper_model: Optional[str] = "small",
+        device: Optional[Union[str, torch.device]] = "cpu",
+        sentence_rule: Optional[str] = None,
     ):
-        self.logger = logging.getLogger('mexca.text.transcription.AudioTranscriber')
+        self.logger = logging.getLogger(
+            "mexca.text.transcription.AudioTranscriber"
+        )
         self.whisper_model = whisper_model
         self.device = device
         # Lazy initialization
         self._transcriber = None
 
         if not sentence_rule:
-            self.sentence_rule = r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|!|:)\s"
-            self.logger.debug('Using default sentence rule %s because "sentence_rule=None"', self.sentence_rule)
+            self.sentence_rule = (
+                r"(?<!\w\.\w.)(?<![A-Z][a-z]\.)(?<=\.|\?|!|:)\s"
+            )
+            self.logger.debug(
+                'Using default sentence rule %s because "sentence_rule=None"',
+                self.sentence_rule,
+            )
         else:
             self.sentence_rule = sentence_rule
 
         self.logger.debug(ClassInitMessage())
 
-
     # Initialize pretrained models only when needed
     @property
     def transcriber(self) -> whisper.Whisper:
-        """The loaded whisper model for audio transcription.
-        """
+        """The loaded whisper model for audio transcription."""
         if not self._transcriber:
-            self._transcriber = stable_whisper.load_model(
+            self._transcriber = whisper.load_model(
+                self.whisper_model, self.device
+            )
+            self.logger.debug(
+                "Initialized %s whisper model for audio transcription",
                 self.whisper_model,
-                self.device
             )
-            self.logger.debug('Initialized %s whisper model for audio transcription', self.whisper_model)
 
         return self._transcriber
 
-
     # Delete pretrained models when not needed anymore
     @transcriber.deleter
     def transcriber(self):
         self._transcriber = None
-        self.logger.debug('Removed %s whisper model for audio transcription', self.whisper_model)
-
+        self.logger.debug(
+            "Removed %s whisper model for audio transcription",
+            self.whisper_model,
+        )
 
-    def apply(self, # pylint: disable=too-many-locals
+    # pylint: disable=too-many-locals
+    def apply(
+        self,
         filepath: str,
         audio_annotation: SpeakerAnnotation,
         language: Optional[str] = None,
         options: Optional[whisper.DecodingOptions] = None,
-        show_progress: bool = True
+        show_progress: bool = True,
     ) -> AudioTranscription:
         """Transcribe speech in an audio file to text.
 
         Transcribe each annotated speech segment in the audio file
         and split the transcription into sentences according to `sentence_rule`.
 
         Parameters
@@ -111,144 +124,232 @@
         Returns
         -------
         AudioTranscription
             A data class object containing transcribed speech segments split into sentences.
 
         """
         if not options:
-            self.logger.debug('Using default options for whisper: No native timestamps and FP16 only if CUDA is available')
+            self.logger.debug(
+                "Using default options for whisper: No native timestamps and FP16 only if CUDA is available"
+            )
             options = self.get_default_options(language=language)
 
         audio = torch.Tensor(whisper.load_audio(filepath))
 
         transcription = AudioTranscription(
-            filename=filepath,
-            subtitles=IntervalTree()
+            filename=filepath, subtitles=IntervalTree()
         )
 
         for i, seg in tqdm(
             enumerate(audio_annotation),
             total=len(audio_annotation),
-            disable=not show_progress
+            disable=not show_progress,
         ):
+            # Get segment length
+            segment_length = seg.end - seg.begin
+
             # Get start and end frame
             start = int(seg.begin * SAMPLE_RATE)
             end = int(seg.end * SAMPLE_RATE)
 
             # Subset audio signal
             audio_sub = audio[start:end]
 
-            self.logger.debug('Transcribing segment %s from %s to %s', i, seg.begin, seg.end)
+            self.logger.debug(
+                "Transcribing segment %s from %s to %s", i, seg.begin, seg.end
+            )
             try:
-                output = self.transcriber.transcribe(audio_sub, verbose=None, **asdict(options))
+                output = self.transcriber.transcribe(
+                    audio_sub,
+                    word_timestamps=True,
+                    verbose=None,
+                    **asdict(options),
+                )
             except RuntimeError as exc:
-                self.logger.error('Audio waveform too short to be transcribed: %s', exc)
+                if segment_length < 0.02:
+                    self.logger.error(
+                        "Audio waveform too short to be transcribed: %s", exc
+                    )
+                else:
+                    self.logger.error(
+                        "The operator aten::_index_put_impl_ is not current implemented for the MPS device"
+                    )
                 continue
 
-            self.logger.debug('Detected language: %s', whisper.tokenizer.LANGUAGES[output['language']].title())
-            segment_text = output['text'].strip()
+            self.logger.debug(
+                "Detected language: %s",
+                whisper.tokenizer.LANGUAGES[output["language"]].title(),
+            )
+            text = output["text"].strip()
 
             # Split text into sentences
-            sents = re.split(self.sentence_rule, segment_text)
-            self.logger.debug('Segment text split into %s sentences', len(sents))
+            sents = re.split(self.sentence_rule, text)
+            self.logger.debug(
+                "Segment text split into %s sentences", len(sents)
+            )
 
             # Concatenate word timestamps from every segment
             whole_word_timestamps = []
 
-            for segment in output['segments']:
-                whole_word_timestamps.extend(segment['whole_word_timestamps'])
+            for segment in output["segments"]:
+                whole_word_timestamps.extend(segment["words"])
 
             if len(whole_word_timestamps) > 0:
                 idx = 0
 
                 for j, sent in enumerate(sents):
                     sent_len = len(sent.split(" ")) - 1
 
-                    sent_start = whole_word_timestamps[idx]['timestamp']
-                    sent_end = whole_word_timestamps[idx + sent_len]['timestamp']
+                    # Get timestamp of first word in sentence (BEFORE the first word is spoken - 'start')
+                    sent_start = self._get_timestamp(
+                        whole_word_timestamps, idx, timestamp_type="start"
+                    )
+                    # Get timestamp of last word in sentence (AFTER the last word is spoken - 'end')
+                    sent_end = self._get_timestamp(
+                        whole_word_timestamps,
+                        (idx + sent_len),
+                        timestamp_type="end",
+                    )
+                    # Calculate average probability of transcription accuracy for sentence
+                    conf = self._get_avg_confidence(
+                        whole_word_timestamps, idx, sent_len
+                    )
+
                     self.logger.debug(
-                        'Processing sentence %s from %s to %s with text: %s', j, seg.begin+sent_start, seg.begin+sent_end, sent
+                        "Processing sentence %s from %s to %s with text: %s",
+                        j,
+                        seg.begin + sent_start,
+                        seg.begin + sent_end,
+                        sent,
                     )
 
                     if (sent_end - sent_start) > 0:
-                        transcription.subtitles.add(Interval(
-                            begin=seg.begin + sent_start,
-                            end=seg.begin + sent_end,
-                            data=TranscriptionData(
-                                index=i,
-                                text=sent,
-                                speaker=seg.data.name
+                        transcription.subtitles.add(
+                            Interval(
+                                begin=seg.begin + sent_start,
+                                end=seg.begin + sent_end,
+                                data=TranscriptionData(
+                                    index=i,
+                                    text=sent,
+                                    speaker=seg.data.name,
+                                    confidence=conf,
+                                ),
                             )
-                        ))
+                        )
                     else:
-                        self.logger.warning('Sentence has duration <= 0 and was not added to transcription')
+                        self.logger.warning(
+                            "Sentence has duration <= 0 and was not added to transcription"
+                        )
 
                     idx += sent_len + 1
 
         del self._transcriber
 
         return transcription
 
-
     @staticmethod
-    def get_default_options(language: Optional[str] = None) -> whisper.DecodingOptions:
+    def get_default_options(
+        language: Optional[str] = None,
+    ) -> whisper.DecodingOptions:
         """Set default options for transcription.
 
         Sets language as well as `without_timestamps=False` and `fp16=torch.cuda.is_available()`.
 
         Returns
         -------
         whisper.DecodingOptions
 
         """
         return whisper.DecodingOptions(
             language=language,
             without_timestamps=False,
-            fp16=torch.cuda.is_available()
+            fp16=torch.cuda.is_available(),
         )
 
+    @staticmethod
+    def _get_timestamp(
+        word_timestamps: list, idx: int, timestamp_type: str = "start"
+    ) -> float:
+        # get word-level timestamp for the word located at index idx in sequence list of words
+        return word_timestamps[idx][timestamp_type]
+
+    @staticmethod
+    def _get_avg_confidence(
+        word_timestamps: list, idx: int, sentence_len: int
+    ) -> float:
+        # Computes the average probability / accuracy of
+        # transcription for a given sentence. Sums the
+        # probabilities for individual words in the sentence
+        # and divide by the sentence length
+        total = 0.0
+        for j, word in enumerate(word_timestamps):
+            if idx <= j < sentence_len:
+                total += word["probability"]
+
+        return total / sentence_len
+
 
 # Adapted from whisper.trascribe.cli
 # See: https://github.com/openai/whisper/blob/main/whisper/transcribe.py
 def cli():
     """Command line interface for audio transcription.
     See `transcribe -h` for details.
     """
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
 
-    parser.add_argument('-f', '--filepath', type=str, required=True)
-    parser.add_argument('-a', '--annotation-path', type=str, required=True, dest='annotation_path')
-    parser.add_argument('-o', '--outdir', type=str, required=True)
-    parser.add_argument("--model", default="small", choices=whisper.available_models())
+    parser.add_argument("-f", "--filepath", type=str, required=True)
+    parser.add_argument(
+        "-a",
+        "--annotation-path",
+        type=str,
+        required=True,
+        dest="annotation_path",
+    )
+    parser.add_argument("-o", "--outdir", type=str, required=True)
+    parser.add_argument(
+        "--model", default="small", choices=whisper.available_models()
+    )
     parser.add_argument("--device", default="cpu")
     parser.add_argument("--language", type=optional_str, default=None)
-    parser.add_argument('--sentence-rule', type=optional_str, default=None, dest='sentence_rule')
-    parser.add_argument('--show-progress', type=str2bool, default=True, dest='show_progress')
+    parser.add_argument(
+        "--sentence-rule", type=optional_str, default=None, dest="sentence_rule"
+    )
+    parser.add_argument(
+        "--show-progress", type=str2bool, default=True, dest="show_progress"
+    )
 
     args = parser.parse_args().__dict__
 
     transcriber = AudioTranscriber(
-        whisper_model=args['model'],
-        device=args['device'],
-        sentence_rule=args['sentence_rule']
+        whisper_model=args["model"],
+        device=args["device"],
+        sentence_rule=args["sentence_rule"],
     )
 
     options = whisper.DecodingOptions(
-        language=args['language'],
+        language=args["language"],
         without_timestamps=False,
-        fp16=torch.cuda.is_available()
+        fp16=torch.cuda.is_available(),
     )
 
-    audio_annotation = SpeakerAnnotation.from_rttm(args['annotation_path'])
+    audio_annotation = SpeakerAnnotation.from_rttm(args["annotation_path"])
 
     output = transcriber.apply(
-        args['filepath'],
+        args["filepath"],
         audio_annotation=audio_annotation,
         options=options,
-        show_progress=args['show_progress']
+        show_progress=args["show_progress"],
     )
 
-    output.write_srt(os.path.join(args['outdir'], os.path.splitext(os.path.basename(args['filepath']))[0] + '_transcription.srt'))
+    output.write_srt(
+        os.path.join(
+            args["outdir"],
+            os.path.splitext(os.path.basename(args["filepath"]))[0]
+            + "_transcription.srt",
+        )
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `mexca-0.4.0/mexca/utils.py` & `mexca-0.5.0/mexca/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 """Utility functions.
 """
 
 import numpy as np
 import pandas as pd
-from mexca.data import (AudioTranscription, Multimodal, SentimentAnnotation, SpeakerAnnotation, VideoAnnotation,
-                        VoiceFeatures)
 
+from mexca.data import (
+    AudioTranscription,
+    Multimodal,
+    SentimentAnnotation,
+    SpeakerAnnotation,
+    VideoAnnotation,
+    VoiceFeatures,
+)
 
 # Adapted from whisper.utils
 # See: https://github.com/openai/whisper/blob/28769fcfe50755a817ab922a7bc83483159600a9/whisper/utils.py
 
 
 def str2bool(string: str):
     str2val = {"True": True, "False": False}
@@ -51,16 +57,18 @@
     assert multimodal.features.face_prob.dtype == "float64"
     assert multimodal.features.face_landmarks.dtype == "object"
     assert multimodal.features.face_aus.dtype == "object"
     assert multimodal.features.face_label.dtype == "float64"
     assert multimodal.features.face_confidence.dtype == "float64"
 
     assert all(len(bbox) == 4 for bbox in multimodal.features.face_box.dropna())
-    assert all(len(lmks) == 68 for lmks in multimodal.features.face_landmarks.dropna())
-    assert all(len(aus) == 20 for aus in multimodal.features.face_aus.dropna())
+    assert all(
+        len(lmks) == 5 for lmks in multimodal.features.face_landmarks.dropna()
+    )
+    assert all(len(aus) == 41 for aus in multimodal.features.face_aus.dropna())
 
     assert (
         multimodal.features.face_box.isna()
         .eq(multimodal.features.face_prob.isna())
         .all()
     )
     assert (
@@ -111,15 +119,18 @@
         assert seg.end in multimodal.features.segment_end.to_numpy()
         assert str(
             seg.data.name
         ) in multimodal.features.segment_speaker_label.to_numpy().astype(str)
 
 
 def _validate_voice_feature(
-    feat: pd.Series, ref_feat: np.ndarray, d_type: str = "float64", is_pos: bool = False
+    feat: pd.Series,
+    ref_feat: np.ndarray,
+    d_type: str = "float64",
+    is_pos: bool = False,
 ):
     assert feat.dtype == d_type
     assert len(feat.dropna()) > 0
     if is_pos:
         assert feat[np.isfinite(feat)] > 0
 
     for f in feat[:-1]:
@@ -225,9 +236,15 @@
         _validate_transcription(output)
     if check_sentiment:
         assert isinstance(output.sentiment, SentimentAnnotation)
         _validate_sentiment(output)
 
     assert isinstance(output.features, pd.DataFrame)
 
-    assert output.features.frame.le(125).all() and output.features.frame.ge(0).all()
-    assert output.features.time.le(5.0).all() and output.features.time.ge(0.0).all()
+    assert (
+        output.features.frame.le(125).all()
+        and output.features.frame.ge(0).all()
+    )
+    assert (
+        output.features.time.le(5.0).all()
+        and output.features.time.ge(0.0).all()
+    )
```

### Comparing `mexca-0.4.0/mexca/video.py` & `mexca-0.5.0/mexca/video/extraction.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,82 +2,84 @@
 """
 
 import argparse
 import logging
 import os
 import warnings
 from typing import Dict, List, Optional, Tuple, Union
-import feat
+
 import numpy as np
 import torch
 from facenet_pytorch import MTCNN, InceptionResnetV1
 from feat.utils.image_operations import convert_image_to_tensor
 from sklearn.metrics.pairwise import cosine_distances
 from spectralcluster import SpectralClusterer
-from torch import transpose
 from torch.utils.data import DataLoader, Dataset
+from torchvision import transforms
 from torchvision.io import read_video, read_video_timestamps
 from tqdm import tqdm
+
 from mexca.data import VideoAnnotation
 from mexca.utils import ClassInitMessage, optional_float, optional_int, str2bool
-
+from mexca.video.mefarg import MEFARG
 
 EMPTY_VALUE = np.nan
 """Value that is returned if no faces are detected in a video frame.
 """
 # Package versions are pinned so we can ignore future and deprecation warnings
 # Ignore warning from facenet_pytorch
 #
 # VisibleDeprecationWarning: Creating an ndarray from ragged nested sequences
 # (which is a list-or-tuple of lists-or-tuples-or ndarrays with different lengths or shapes)
 # is deprecated. If you meant to do this, you must specify 'dtype=object' when creating the ndarray.
 #    probs = np.array(probs)
-warnings.simplefilter('ignore', category=np.VisibleDeprecationWarning)
+warnings.simplefilter("ignore", category=np.VisibleDeprecationWarning)
 
 # Ignore warning from spectralclusterer
 #
-# FutureWarning: The default value of `n_init` will change from 10 to 'auto' in 1.4. 
+# FutureWarning: The default value of `n_init` will change from 10 to 'auto' in 1.4.
 # Set the value of `n_init` explicitly to suppress the warning
-warnings.simplefilter('ignore', category=FutureWarning)
+warnings.simplefilter("ignore", category=FutureWarning)
 
 
 class NotEnoughFacesError(Exception):
     """Less detected faces than `num_faces`.
-    
+
     Cannot perform clustering if samples are less than the number of clusters.
 
     Parameters
     ----------
     msg : str
         Error message.
-    
+
     """
+
     def __init__(self, msg: str):
         super().__init__(msg)
 
 
 # Adapted from pyfeat.data.VideoDataset
 # See: https://github.com/cosanlab/py-feat/blob/03337f44e98a915a8488388bce94154d2d5ba73c/feat/data.py#L2154
 class VideoDataset(Dataset):
     """Custom torch dataset for a video file.
 
     Only reads the frame timestamps of the video but not the frames themselves when initialized.
     Decodes the video frame-by-frame.
-    
+
     Arguments
     ---------
     video_file : str
         Path to the video file.
     skip_frames : int, default=1
         Only load every nth frame.
     start : float, default=0
         Start of the subclip of the video to be loaded (in seconds).
     end : float, optional, default=None
         End of the subclip of the video to be loaded (in seconds).
-    
+
     Attributes
     ----------
     file_name : str
         Name of the video file.
     video_pts : torch.Tensor
         Timestamps of video frames.
     video_frames_idx : torch.Tensor
@@ -85,98 +87,99 @@
     video_fps: int
         Frames per second.
     video_frames : numpy.ndarray
         Indices of loaded frames.
 
     """
 
-    def __init__(self, video_file: str, skip_frames: int = 1, start: float = 0, end: Optional[float] = None):
-        self.logger = logging.getLogger('mexca.video.VideoDataset')
-        self.logger.debug('Reading video timestamps')
+    def __init__(
+        self,
+        video_file: str,
+        skip_frames: int = 1,
+        start: float = 0,
+        end: Optional[float] = None,
+    ):
+        self.logger = logging.getLogger("mexca.video.VideoDataset")
+        self.logger.debug("Reading video timestamps")
         video_pts, video_fps = read_video_timestamps(video_file)
 
         self.file_name = os.path.basename(video_file)
-        self._filepath = video_file # Store path to video for reading frames in __getitem__()
+        self._filepath = video_file  # Store path to video for reading frames in __getitem__()
 
         self.video_fps = video_fps
 
         # Frame indices of start and end
         start_idx = int(start * video_fps)
         if end is None:
             end_idx = len(video_pts)
         else:
             end_idx = int(end * video_fps)
-        
+
         self.video_frames_idx = np.arange(start_idx, end_idx, skip_frames)
 
         # Store timestamps of frames to be loaded
         self.video_pts = torch.Tensor(video_pts)[self.video_frames_idx]
 
         self.logger.debug(ClassInitMessage())
 
-
     @property
     def duration(self) -> float:
-        """Duration of the video (read-only).
-        """
-        return len(self)/self.video_fps
-
+        """Duration of the video (read-only)."""
+        return len(self) / self.video_fps
 
     def __len__(self) -> int:
-        """Number of video frames.
-        """
+        """Number of video frames."""
         return self.video_pts.shape[0]
 
-
     def __getitem__(self, idx: int) -> Dict[str, torch.Tensor]:
         """Get an item from the data set.
 
         Loads the video frame into memory.
 
         Parameters
         ----------
         idx : int
             Index of the item in the dataset.
-        
+
         Returns
         -------
         dict
             Dictionary with 'Image' containing the video frame (T, H, W, C)
             and 'Frame' containing the frame index.
 
         """
-        self.logger.debug('Getting item %s', idx)
+        self.logger.debug("Getting item %s", idx)
         frame_pts = self.video_pts[idx]
 
         # Read video frame at timestamp of idx
         with warnings.catch_warnings():
             # We can safely ignore this warning because we don't need accurate AV sync:
             # https://github.com/pytorch/vision/issues/1931
             #
             # UserWarning: The pts_unit 'pts' gives wrong results. Please use
             # pts_unit 'sec'
             warnings.simplefilter("ignore", UserWarning)
 
             image, _, _ = read_video(
                 self._filepath,
                 start_pts=int(frame_pts.min()),
-                end_pts=int(frame_pts.max())
+                end_pts=int(frame_pts.max()),
             )
 
         # Adjust slice if idx is slice
         if isinstance(idx, slice):
             zero_idx = slice(0, idx.stop - idx.start, idx.step)
             return {
                 "Image": image[zero_idx, :, :, :],
-                "Frame": self.video_frames_idx[idx]
+                "Frame": self.video_frames_idx[idx],
             }
 
         return {
-            "Image": image.squeeze(), # Remove first dim
-            "Frame": self.video_frames_idx[idx]
+            "Image": image.squeeze(),  # Remove first dim
+            "Frame": self.video_frames_idx[idx],
         }
 
 
 class FaceExtractor:
     """Combine steps to extract features from faces in a video file.
 
     Parameters
@@ -194,173 +197,155 @@
     select_largest : bool, default=True
         Whether to return the largest face or the one with the highest probability
         if multiple faces are detected.
     selection_method : {None, 'probability', 'largest', 'largest_over_threshold', 'center_weighted_size'}, optional, default=None
         The heuristic used for selecting detected faces. If not `None`, overrides `select_largest`.
     keep_all: bool, default=True
         Whether all faces should be returned in the order of `select_largest`.
-    device: torch.device, optional, default=None
+    device: torch.device, optional, default=torch.device("cpu")
         The device on which face detection and embedding computations are performed.
     max_cluster_frames : int, optional, default=None
         Maximum number of frames that are used for spectral clustering. If the number of frames exceeds the maximum,
         hierarchical clustering is applied first to reduce the frames to this number. This can reduce the computational
         costs for long videos.
     embeddings_model : {'vggface2', 'casia-webface'}, default='vggface2'
         Pretrained Inception Resnet V1 model for computing face embeddings.
-    au_model : {'xgb', 'svm'}, default='xgb'
-        Pretrained model for predicting facial action unit activations.
-    landmark_model : {'mobilefacenet', 'mobilenet', 'pfld'}, default='mobilefacenet'
-        Pretrained model for detecting facial landmarks.
-
-    Notes
-    -----
-    For details on the available pretrained models for facial action unit and landmark detection,
-    see the documentation of `py-feat <https://py-feat.org/pages/models.html>`__.
-    The pretrained action unit models return different outputs: `'xgb'` returns continous values (0-1),
-    whereas `'svm'` returns binary (0, 1) values.
 
     """
-    def __init__(self,
+
+    def __init__(
+        self,
         num_faces: Optional[int],
         min_face_size: int = 20,
         thresholds: Tuple[float] = (0.6, 0.7, 0.7),
         factor: float = 0.709,
         post_process: bool = True,
         select_largest: bool = True,
         selection_method: Optional[str] = None,
         keep_all: bool = True,
-        device: Optional[torch.device] = None,
+        device: torch.device = torch.device(type="cpu"),
         max_cluster_frames: Optional[int] = None,
-        embeddings_model: str = 'vggface2',
-        au_model: str = 'xgb',
-        landmark_model: str = 'mobilefacenet'
+        embeddings_model: str = "vggface2",
     ):
-        self.logger = logging.getLogger('mexca.video.FaceExtractor')
+        self.logger = logging.getLogger("mexca.video.FaceExtractor")
         self.min_face_size = min_face_size
         self.thresholds = thresholds
         self.factor = factor
         self.post_process = post_process
         self.select_largest = select_largest
         self.selection_method = selection_method
         self.keep_all = keep_all
+        self.logger.debug("Initializing FaceExtractor on device %s", device)
         self.device = device
         self.embeddings_model = embeddings_model
         self.num_faces = num_faces
-        self.au_model = au_model
-        self.landmark_model = landmark_model
         self.max_cluster_frames = max_cluster_frames
-        
+
         # Lazy initialization: See getter functions
         self._detector = None
         self._encoder = None
         self._clusterer = None
         self._extractor = None
-        
-        self.logger.debug(ClassInitMessage())
 
+        self.logger.debug(ClassInitMessage())
 
     # Initialize pretrained models only when needed
     @property
     def detector(self) -> MTCNN:
         """The MTCNN model for face detection and extraction.
         See `facenet-pytorch <https://github.com/timesler/facenet-pytorch/blob/555aa4bec20ca3e7c2ead14e7e39d5bbce203e4b/models/mtcnn.py#L157>`_ for details.
         """
         if not self._detector:
             self._detector = MTCNN(
+                image_size=224,
                 min_face_size=self.min_face_size,
                 thresholds=self.thresholds,
                 factor=self.factor,
                 post_process=self.post_process,
                 select_largest=self.select_largest,
                 selection_method=self.selection_method,
                 keep_all=self.keep_all,
-                device=self.device
+                device=self.device,
             )
-            self.logger.debug('Initialized MTCNN face detector')
+            self.logger.debug("Initialized MTCNN face detector")
         return self._detector
 
-
     # Delete pretrained models when not needed anymore
     @detector.deleter
     def detector(self):
         self._detector = None
-        self.logger.debug('Removed MTCNN face detector')
-
+        self.logger.debug("Removed MTCNN face detector")
 
     @property
     def encoder(self) -> InceptionResnetV1:
         """The ResnetV1 model for computing face embeddings.
         See `facenet-pytorch <https://github.com/timesler/facenet-pytorch/blob/555aa4bec20ca3e7c2ead14e7e39d5bbce203e4b/models/inception_resnet_v1.py#L184>`__ for details.
         """
         if not self._encoder:
             self._encoder = InceptionResnetV1(
-                pretrained=self.embeddings_model,
-                device=self.device
+                pretrained=self.embeddings_model, device=self.device
             ).eval()
-            self.logger.debug('Initialized InceptionResnetV1 face encoder')
+            self.logger.debug("Initialized InceptionResnetV1 face encoder")
         return self._encoder
 
-
     @encoder.deleter
     def encoder(self):
         self._encoder = None
-        self.logger.debug('Removed InceptionResnetV1 face encoder')
-
+        self.logger.debug("Removed InceptionResnetV1 face encoder")
 
     @property
     def clusterer(self) -> SpectralClusterer:
         """The spectral clustering model for identifying faces based on embeddings.
         See `spectralcluster <https://wq2012.github.io/SpectralCluster/>`_ for details.
         """
         if not self._clusterer:
             self._clusterer = SpectralClusterer(
                 min_clusters=self.num_faces,
                 max_clusters=self.num_faces,
-                max_spectral_size=self.max_cluster_frames
+                max_spectral_size=self.max_cluster_frames,
             )
-            self.logger.debug('Initialized spectral clusterer')
+            self.logger.debug("Initialized spectral clusterer")
         return self._clusterer
 
-
     @clusterer.deleter
     def clusterer(self):
         self._clusterer = None
-        self.logger.debug('Removed spectral clusterer')
-
+        self.logger.debug("Removed spectral clusterer")
 
     @property
-    def extractor(self) -> feat.detector.Detector:
-        """The model for extracting facial landmarks and action units.
-        See `py-feat <https://py-feat.org/pages/api.html>`_ for details.
+    def extractor(self) -> MEFARG:
+        """The MEFARG model for extracting action unit activations.
+        See ME-GraphAU `model <https://github.com/CVI-SZU/ME-GraphAU>`_ and
+        `paper <https://arxiv.org/abs/2205.01782>`_ for details.
         """
         if not self._extractor:
-            self._extractor = feat.detector.Detector(
-                au_model=self.au_model,
-                landmark_model=self.landmark_model,
-                device='cpu' if self.device is None else self.device
+            self._extractor = MEFARG.from_pretrained(device=self.device)
+            self._extractor.eval()
+            self.logger.debug(
+                "Initialized MEFARG action unit feature extractor"
             )
-            self.logger.debug('Initialized pyfeat facial feature extractor')
         return self._extractor
 
-
     @extractor.deleter
     def extractor(self):
         self._extractor = None
-        self.logger.debug('Removed pyfeat facial feature extractor')
-
+        self.logger.debug("Removed MEFARG action unit feature extractor")
 
     def __call__(self, **callargs) -> VideoAnnotation:
-        """Alias for `apply`.
-        """
+        """Alias for `apply`."""
         return self.apply(**callargs)
 
-
-    def detect(self,
-        frame: Union[np.ndarray, torch.Tensor]
-    ) -> Tuple[List[torch.Tensor], Union[List[np.ndarray], np.ndarray], Union[List[np.ndarray], np.ndarray]]:
+    def detect(
+        self, frame: Union[np.ndarray, torch.Tensor]
+    ) -> Tuple[
+        List[torch.Tensor],
+        Union[List[np.ndarray], np.ndarray],
+        Union[List[np.ndarray], np.ndarray],
+        Union[List[np.ndarray], np.ndarray],
+    ]:
         """Detect faces in a video frame.
 
         Parameters
         ----------
         frame: numpy.ndarray or torch.Tensor
             Batch of B frames containing RGB values with dimensions (B, W, H, 3).
 
@@ -373,27 +358,29 @@
             Batch of B bounding boxes of the N detected faces as (x1, y1, x2, y2) coordinates with
             dimensions (B, N, 4). Returns a list if different numbers of faces are detected across batched frames.
             Is `None` if a frame contains no faces.
         probs: numpy.ndarray or list
             Probabilities of the detected faces (B, N).
             Returns a list if different numbers of faces are detected across batched frames.
             Is `None` if a frame contains no faces.
+        landmarks: numpy.ndarray or list
+            Batch of B facial landmarks for N detected faces as (x, y) coordinates with dimensions (5, 2).
+            Is `None` if a frame contains no faces.
 
         """
-        
+
         frame = convert_image_to_tensor(frame)
 
-        self.logger.debug('Detecting faces')
-        boxes, probs = self.detector.detect(frame, landmarks=False) # pylint: disable=unbalanced-tuple-unpacking
+        self.logger.debug("Detecting faces and facial landmarks")
+        boxes, probs, landmarks = self.detector.detect(frame, landmarks=True)
 
-        self.logger.debug('Extracting facial action units and landmarks')
+        self.logger.debug("Extracting facial action unit activations")
         faces = self.detector.extract(frame, boxes, save_path=None)
 
-        return faces, boxes, probs
-
+        return faces, boxes, probs, landmarks
 
     def encode(self, faces: torch.Tensor) -> np.ndarray:
         """Compute embeddings for face images.
 
         Parameters
         ----------
         faces: torch.Tensor
@@ -403,20 +390,19 @@
         Returns
         -------
         numpy.ndarray
             Embeddings of the N face images with dimensions (N, 512).
 
         """
 
-        self.logger.debug('Encoding faces')
+        self.logger.debug("Encoding faces")
         embeddings = self.encoder(faces.to(self.device)).detach().cpu().numpy()
 
         return embeddings
 
-
     def identify(self, embeddings: np.ndarray) -> np.ndarray:
         """Cluster faces based on their embeddings.
 
         Parameters
         ----------
         embeddings: numpy.ndarray
             Embeddings of the N face images with dimensions (N, E) where E is the length
@@ -426,101 +412,80 @@
         -------
         numpy.ndarray
             Cluster indices for the N face embeddings.
 
         """
         labels = np.full((embeddings.shape[0]), np.nan)
         labels_finite = np.all(np.isfinite(embeddings), 1)
-        embeddings_finite =  embeddings[labels_finite, :]
+        embeddings_finite = embeddings[labels_finite, :]
 
-        self.logger.info('Clustering face embeddings')
+        self.logger.info("Clustering face embeddings")
 
         try:
             if embeddings_finite.shape[0] < self.num_faces:
                 raise NotEnoughFacesError(
                     "Not enough faces detected to perform clustering; consider reducing 'num_faces', 'min_face_size', or 'thresholds'"
                 )
-                
+
         except NotEnoughFacesError as exc:
-            self.logger.exception('NotEnoughFacesError: %s', exc)
+            self.logger.exception("NotEnoughFacesError: %s", exc)
             raise exc
 
-        labels[labels_finite] = self.clusterer.predict(
-            embeddings_finite)
+        labels[labels_finite] = self.clusterer.predict(embeddings_finite)
 
         return labels
 
-
-    def extract(self,
+    def extract(
+        self,
         frame: Union[np.ndarray, torch.Tensor],
-        boxes: Union[List[np.ndarray], np.ndarray]
-    ) -> Tuple[List[List[np.ndarray]], List[np.ndarray]]:
-        """Detect facial action units and landmarks.
+    ) -> Union[List[np.ndarray], np.ndarray]:
+        """Detect facial action units activations.
 
         Parameters
         ----------
         frame: numpy.ndarray or torch.Tensor
             Batch of B frames containing RGB values with dimensions (B, H, W, 3).
-        boxes: numpy.ndarray or list
-            Batch of B bounding boxes of the N detected faces as (x1, y1, x2, y2) coordinates with
-            dimensions (B, N, 4) or list of B elements with (N, 4).
 
         Returns
         -------
-        landmarks: list
-            Batch of B facial landmarks for N detected faces as (x, y) coordinates with dimensions (68, 2).
-            Is `None` if a frame contains no faces.
-        aus: list
-            Batch of B action unit activations for N detected faces with dimensions (N, 20).
+        aus: numpy.ndarray or list
+            Batch of B action unit activations for N detected faces with dimensions (N, 41).
             Is `None` if a frame contains no faces.
 
         """
-        # pyfeat requires a different format (T, C, H, W)
-        frame = transpose(transpose(frame, 1, 3), -1, -2)
-
-        boxes_list = []
-
-        # Append a 5th value to each bounding box to mimic the
-        # result by pyfeat.Detector.detect_faces() which returns the
-        # bounding box with the probability;
-        # this is required by pyfeat.Detector.detect_landmarks()
-        for batch in boxes:
-            if batch is not None:
-                batch_list = []
-
-                for face in batch:
-                    batch_list.append(face.tolist() + [0])
-                
-                boxes_list.append(batch_list)
-
-        # Only if any faces were detected
-        if len(boxes_list) > 0:
-            landmarks = self.extractor.detect_landmarks(frame, boxes_list)
-            aus = self.extractor.detect_aus(frame, landmarks)
 
-        landmarks_list = []
         aus_list = []
-        i = 0
 
-        for box in boxes:
-            if box is None:
-                landmarks_list.append(None)
+        for frm in frame:
+            if frm is None:
                 aus_list.append(None)
-            else:
-                landmarks_list.append(landmarks[i])
-                aus_list.append(aus[i])
-                i += 1
+                continue
+
+            normalize = transforms.Normalize(
+                mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225]
+            )
+            transform = transforms.Compose(
+                [
+                    transforms.ConvertImageDtype(torch.float),
+                    normalize,
+                ]
+            )
+
+            frm = transform(frm)
+
+            with torch.no_grad():
+                aus = self.extractor(frm)
 
-        return landmarks_list, aus_list
+            aus_list.append(aus.numpy())
 
+        return np.array(aus_list)
 
     @staticmethod
     def _compute_centroids(
-        embs: np.ndarray,
-        labels: np.ndarray
+        embs: np.ndarray, labels: np.ndarray
     ) -> Tuple[List[np.ndarray], Dict[Union[str, int, float], int]]:
         # compute unique cluster labels
         unique_labels = np.unique(labels)
         # get rid of nan label
         unique_labels = unique_labels[np.logical_not(np.isnan(unique_labels))]
         # compute centroids:
         centroids = []
@@ -534,18 +499,55 @@
             centroid = np.nanmean(label_embeddings, axis=0)
             # appends centroid list
             centroids.append(centroid)
             cluster_label_mapping[label] = i
 
         return centroids, cluster_label_mapping
 
+    def compute_avg_embeddings(
+        self, embeddings: np.ndarray, labels: np.ndarray
+    ) -> dict:
+        """Computes average embedding vector for each face detected in the video.
 
-    def compute_confidence(self,
-        embeddings: np.ndarray,
-        labels: np.ndarray
+        Parameters
+        ----------
+        embeddings: numpy.ndarray
+            Face embeddings.
+        labels: numpy.ndarray
+            Face labels.
+
+        Returns
+        -------
+        average embedding dictionary: dict
+            Dictionary with keys representing face labels and values representing
+            the average embedding vector for each face label.
+        """
+        self.logger.info("Computing average embeddings")
+
+        # collect face embeddings and map them to face labels
+        face_embedding_dict = {}
+        for embedding, label in zip(embeddings, labels):
+            # do not take into account nan values for average embedding calculation
+            if str(label) != "nan":
+                if label in face_embedding_dict:
+                    face_embedding_dict[label].append(embedding)
+                else:
+                    face_embedding_dict[label] = [embedding]
+
+        # calculate average embeddings for each face label
+        face_avg_embedding_dict = {}
+        for label, embeddings_lst in face_embedding_dict.items():
+            face_avg_embedding_dict[label] = np.mean(
+                np.array(embeddings_lst), axis=0
+            ).tolist()
+
+        return face_avg_embedding_dict
+
+    def compute_confidence(
+        self, embeddings: np.ndarray, labels: np.ndarray
     ) -> np.ndarray:
         """Compute face label classification confidence.
 
         Parameters
         ----------
         embeddings: numpy.ndarray
             Face embeddings.
@@ -554,16 +556,18 @@
 
         Returns
         -------
         confidence: numpy.ndarray
             Confidence scores between 0 and 1. Returns `numpy.nan` if no label was assigned to a face.
 
         """
-        self.logger.info('Computing face clustering confidence')
-        centroids, cluster_label_mapping = self._compute_centroids(embeddings, labels)
+        self.logger.info("Computing face clustering confidence")
+        centroids, cluster_label_mapping = self._compute_centroids(
+            embeddings, labels
+        )
 
         # create empty array with same lenght as labels
         confidence = np.empty_like(labels)
 
         for i, (frame_embedding, label) in enumerate(zip(embeddings, labels)):
             # if frame is unclassified, assigns zero confidence
             if np.isnan(label):
@@ -581,35 +585,39 @@
                     # recover index of centroid of cluster
                     cluster_centroid_idx = cluster_label_mapping[label]
 
                     # distance to the centroid of the cluster to which the frame belongs
                     d1 = distances[cluster_centroid_idx]
                     # mimimum of all other distance
 
-                    d2 = np.min(distances[np.arange(len(distances)) != cluster_centroid_idx])
+                    d2 = np.min(
+                        distances[
+                            np.arange(len(distances)) != cluster_centroid_idx
+                        ]
+                    )
 
                     # confidence score: 0 if d1 = d2, 1 if d1 = 0
                     c = (d2 - d1) / d2
 
                     # handle edge cases: d1<d2 by definition, but if the clustering that produced
                     # the labels used a different distance definition, this could not be the case.
                     # These edge cases are low in confidence, i.e., c = 0.
                     c = max(c, 0)
 
                 confidence[i] = c
 
         return confidence
 
-
-    def apply(self, #pylint: disable=too-many-locals
+    def apply(  # pylint: disable=too-many-locals
+        self,
         filepath: str,
         batch_size: int = 1,
         skip_frames: int = 1,
         process_subclip: Tuple[Optional[float]] = (0, None),
-        show_progress: bool = True
+        show_progress: bool = True,
     ) -> VideoAnnotation:
         """Apply multiple steps to extract features from faces in a video file.
 
         This method subsequently calls other methods for each frame of a video file to detect
         and cluster faces. It also extracts facial landmarks and action units.
 
         Parameters
@@ -631,124 +639,184 @@
             A data class object with extracted facial features.
 
         """
         video_dataset = VideoDataset(
             filepath,
             skip_frames=skip_frames,
             start=process_subclip[0],
-            end=process_subclip[1]
+            end=process_subclip[1],
         )
 
-        batch_data_loader = DataLoader(
-            video_dataset,
-            batch_size=batch_size
-        )
+        batch_data_loader = DataLoader(video_dataset, batch_size=batch_size)
 
         # Store features
         annotation = VideoAnnotation()
 
-        embeddings = []  # Embeddings are separate because they won't be returned
+        embeddings = (
+            []
+        )  # Embeddings are separate because they won't be returned
 
-        self.logger.info('Detecting and encoding faces, extracting facial features')
+        self.logger.info(
+            "Detecting and encoding faces, extracting facial features"
+        )
         for b, batch in tqdm(
             enumerate(batch_data_loader),
             total=len(batch_data_loader),
-            disable=not show_progress
+            disable=not show_progress,
         ):
-            self.logger.debug('Processing batch %s', b)
-            faces, boxes, probs = self.detect(batch['Image'])
-            landmarks, aus = self.extract(batch['Image'], boxes)
+            self.logger.debug("Processing batch %s", b)
+            faces, boxes, probs, landmarks = self.detect(batch["Image"])
+            aus = self.extract(faces)
 
             # If no faces were detected in batch
-            for i, frame in enumerate(batch['Frame']):
-                self.logger.debug('Processing frame %s', int(frame))
+            for i, frame in enumerate(batch["Frame"]):
+                self.logger.debug("Processing frame %s", int(frame))
                 if faces[i] is None:
-                    self.logger.debug('No faces detected in frame %s', int(frame))
-                    embeddings.append(np.full((self.encoder.last_bn.num_features), np.nan))
+                    self.logger.debug(
+                        "No faces detected in frame %s", int(frame)
+                    )
+                    embeddings.append(
+                        np.full((self.encoder.last_bn.num_features), np.nan)
+                    )
                     annotation.frame.append(int(frame))
                     annotation.face_box.append(EMPTY_VALUE)
                     annotation.face_landmarks.append(EMPTY_VALUE)
                     annotation.face_prob.append(EMPTY_VALUE)
                     annotation.face_aus.append(EMPTY_VALUE)
 
                 else:
-                    self.logger.debug('%s faces detected in frame %s', len(faces[i]), int(frame))
+                    self.logger.debug(
+                        "%s faces detected in frame %s",
+                        len(faces[i]),
+                        int(frame),
+                    )
                     embs = self.encode(faces[i])
-                    for k, (box, prob, landmark, au, emb) in enumerate(zip(boxes[i], probs[i], landmarks[i], aus[i], embs)):
-                        self.logger.debug('Processing face %s', k)
+                    for k, (box, prob, landmark, au, emb) in enumerate(
+                        zip(boxes[i], probs[i], landmarks[i], aus[i], embs)
+                    ):
+                        self.logger.debug("Processing face %s", k)
                         # Convert everything to lists to make saving and loading easier
                         annotation.frame.append(int(frame))
                         annotation.face_box.append(box.tolist())
                         annotation.face_landmarks.append(landmark.tolist())
-                        annotation.face_prob.append(float(prob)) # convert to build-in float to avoid trouble when saving to json
+                        annotation.face_prob.append(
+                            float(prob)
+                        )  # convert to build-in float to avoid trouble when saving to json
                         annotation.face_aus.append(au.tolist())
 
                         embeddings.append(emb)
 
         # Delete pretrained models to save memory
         del self.detector
         del self.encoder
         del self.extractor
 
-        annotation.face_label = self.identify(np.asarray(embeddings).squeeze()).tolist()
-        annotation.face_confidence = self.compute_confidence(np.asarray(embeddings), np.asarray(annotation.face_label)).tolist()
-        annotation.time = (np.array(annotation.frame) / video_dataset.video_fps).tolist()
+        annotation.face_label = self.identify(
+            np.asarray(embeddings).squeeze()
+        ).tolist()
+        annotation.face_average_embeddings = self.compute_avg_embeddings(
+            np.asarray(embeddings), np.asarray(annotation.face_label)
+        )
+        annotation.face_confidence = self.compute_confidence(
+            np.asarray(embeddings), np.asarray(annotation.face_label)
+        ).tolist()
+        annotation.time = (
+            np.array(annotation.frame) / video_dataset.video_fps
+        ).tolist()
 
         del self.clusterer
 
         return annotation
 
 
 def cli():
     """Command line interface for extracting facial features.
     See `extract-faces -h` for details.
     """
-    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser = argparse.ArgumentParser(
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter
+    )
 
-    parser.add_argument('-f', '--filepath', type=str, required=True)
-    parser.add_argument('-o', '--outdir', type=str, required=True)
-    parser.add_argument('--num-faces', type=optional_int, default=None, dest='num_faces')
-
-    parser.add_argument('--batch-size', type=int, default=1, dest='batch_size')
-    parser.add_argument('--skip-frames', type=int, default=1, dest='skip_frames')
-    parser.add_argument('--process-subclip', type=optional_float, nargs=2, default=[0, None], dest='process_subclip')
-    parser.add_argument('--show-progress', type=str2bool, default=True, dest='show_progress')
-
-    parser.add_argument('--min-face-size', type=int, default=20, dest='min_face_size')
-    parser.add_argument('--thresholds', type=float, nargs=3, default=[0.6, 0.7, 0.7])
-    parser.add_argument('--factor', type=float, default=0.709)
-    parser.add_argument('--post-process', type=str2bool, default=True, dest='post_process')
-    parser.add_argument('--select-largest', type=str2bool, default=True, dest='select_largest')
-    parser.add_argument('--selection-method', type=str, default=None, dest='selection_method')
-    parser.add_argument('--keep-all', type=str2bool, default=True, dest='keep_all')
-    parser.add_argument('--device', type=str, default='cpu')
-    parser.add_argument('--max-cluster-frames', type=optional_int, default=None, dest='max_cluster_frames')
-    parser.add_argument('--embeddings-model', type=str, default='vggface2', dest='embeddings_model')
-    parser.add_argument('--au-model', type=str, default='xgb', dest='au_model')
-    parser.add_argument('--landmark-model', type=str, default='mobilefacenet', dest='landmark_model')
+    parser.add_argument("-f", "--filepath", type=str, required=True)
+    parser.add_argument("-o", "--outdir", type=str, required=True)
+    parser.add_argument(
+        "--num-faces", type=optional_int, default=None, dest="num_faces"
+    )
+
+    parser.add_argument("--batch-size", type=int, default=1, dest="batch_size")
+    parser.add_argument(
+        "--skip-frames", type=int, default=1, dest="skip_frames"
+    )
+    parser.add_argument(
+        "--process-subclip",
+        type=optional_float,
+        nargs=2,
+        default=[0, None],
+        dest="process_subclip",
+    )
+    parser.add_argument(
+        "--show-progress", type=str2bool, default=True, dest="show_progress"
+    )
+
+    parser.add_argument(
+        "--min-face-size", type=int, default=20, dest="min_face_size"
+    )
+    parser.add_argument(
+        "--thresholds", type=float, nargs=3, default=[0.6, 0.7, 0.7]
+    )
+    parser.add_argument("--factor", type=float, default=0.709)
+    parser.add_argument(
+        "--post-process", type=str2bool, default=True, dest="post_process"
+    )
+    parser.add_argument(
+        "--select-largest", type=str2bool, default=True, dest="select_largest"
+    )
+    parser.add_argument(
+        "--selection-method", type=str, default=None, dest="selection_method"
+    )
+    parser.add_argument(
+        "--keep-all", type=str2bool, default=True, dest="keep_all"
+    )
+    parser.add_argument("--device", type=str, default="cpu")
+    parser.add_argument(
+        "--max-cluster-frames",
+        type=optional_int,
+        default=None,
+        dest="max_cluster_frames",
+    )
+    parser.add_argument(
+        "--embeddings-model",
+        type=str,
+        default="vggface2",
+        dest="embeddings_model",
+    )
 
     args = parser.parse_args().__dict__
 
-    filepath: str = args.pop('filepath')
-    outdir: str = args.pop('outdir')
-    batch_size: int = args.pop('batch_size')
-    skip_frames: int = args.pop('skip_frames')
-    process_subclip: list = args.pop('process_subclip')
-    show_progress: bool = args.pop('show_progress')
+    filepath: str = args.pop("filepath")
+    outdir: str = args.pop("outdir")
+    batch_size: int = args.pop("batch_size")
+    skip_frames: int = args.pop("skip_frames")
+    process_subclip: list = args.pop("process_subclip")
+    show_progress: bool = args.pop("show_progress")
 
-    extractor = FaceExtractor(
-        **args
-    )
+    extractor = FaceExtractor(**args)
 
     output = extractor.apply(
         filepath=filepath,
         batch_size=batch_size,
         skip_frames=skip_frames,
         process_subclip=process_subclip,
-        show_progress=show_progress
+        show_progress=show_progress,
     )
 
-    output.write_json(os.path.join(outdir, os.path.splitext(os.path.basename(filepath))[0] + '_video_annotation.json'))
+    output.write_json(
+        os.path.join(
+            outdir,
+            os.path.splitext(os.path.basename(filepath))[0]
+            + "_video_annotation.json",
+        )
+    )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `mexca-0.4.0/mexca.egg-info/PKG-INFO` & `mexca-0.5.0/mexca.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: mexca
-Version: 0.4.0
+Version: 0.5.0
 Summary: Emotion expression capture from multiple modalities.
 Home-page: https://github.com/mexca/mexca
 Author: Malte Luken
 Author-email: m.luken@esciencecenter.nl
 Project-URL: Bug Tracker, https://github.com/mexca/mexca/issues
 Keywords: emotion,multimodal,expression
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.10,>=3.7
+Requires-Python: <3.11,>3.7
 Description-Content-Type: text/markdown
 Provides-Extra: vid
 Provides-Extra: spe
 Provides-Extra: voi
 Provides-Extra: tra
 Provides-Extra: sen
 Provides-Extra: all
@@ -40,27 +40,28 @@
 [![workflow scc badge](https://sonarcloud.io/api/project_badges/measure?project=mexca_mexca&metric=coverage)](https://sonarcloud.io/dashboard?id=mexca_mexca)
 [![build](https://github.com/mexca/mexca/actions/workflows/build.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/build.yml)
 [![cffconvert](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/cffconvert.yml)
 [![markdown-link-check](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml/badge.svg)](https://github.com/mexca/mexca/actions/workflows/markdown-link-check.yml)
 [![DOI](https://zenodo.org/badge/500818250.svg)](https://zenodo.org/badge/latestdoi/500818250)
 [![docker hub badge](https://img.shields.io/static/v1?label=Docker%20Hub&message=mexca&color=blue&style=flat&logo=docker)](https://hub.docker.com/u/mexca)
 [![docker build badge](https://img.shields.io/github/actions/workflow/status/mexca/mexca/docker.yml?label=Docker%20build&logo=docker)](https://github.com/mexca/mexca/actions/workflows/docker.yml)
+[![black code style badge](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 <div align="center">
 <img src="mexca_logo.png">
 </div>
 
 mexca is an open-source Python package which aims to capture human emotion expressions from videos in a single pipeline.
 
 ## How To Use Mexca
 
-mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos. 
-It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text). 
-The blocks can also be integrated into a single pipeline to extract the features from all modalities at once. 
-Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations. 
+mexca implements the customizable yet easy-to-use Multimodal Emotion eXpression Capture Amsterdam (MEXCA) pipeline for extracting emotion expression features from videos.
+It contains building blocks that can be used to extract features for individual modalities (i.e., facial expressions, voice, and dialogue/spoken text).
+The blocks can also be integrated into a single pipeline to extract the features from all modalities at once.
+Next to extracting features, mexca can also identify the speakers shown in the video by clustering speaker and face representations.
 This allows users to compare emotion expressions across speakers, time, and contexts.
 
 Please cite mexca if you use it for scientific or commercial purposes.
 
 <div align="center">
 <img src="docs/mexca_flowchart.svg" width="600">
 </div>
@@ -73,16 +74,16 @@
 The package contains five components that must be explicitly installed [^1]. By default, only the base package is installed
 (which requires only a few dependencies). The components can still be used through Docker containers which must be downloaded
 from Docker Hub. We recommend this setup for users with little experience with installing Python packages or who simply want to
 quickly try out the package. Using the containers also adds stability to your program.
 
 ### Requirements
 
-mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing), 
-which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails, 
+mexca requires Python version >= 3.7 and <= 3.9. It further depends on [FFmpeg](https://ffmpeg.org/) (for video and audio processing),
+which is usually automatically installed through the MoviePy package (i.e., its imageio dependency). In case the automatic install fails,
 it must be installed manually.
 
 To download and run the components as Docker containers, Docker must be installed on your system. Instructions on how to install
 Docker Desktop can be found [here](https://www.docker.com/get-started/).
 
 All components but the VoiceExtractor depend on PyTorch (version 1.12). Usually, it should be automatically installed when specifying any
 of these components. In case the installation fails, see the installation instructions on the PyTorch [web page](https://pytorch.org/get-started/locally/).
@@ -131,17 +132,21 @@
 If you would like to learn how to use mexca, take a look at our [example](https://github.com/mexca/mexca/tree/main/examples) notebook.
 
 *Note*: mexca builds on pretrained models from the pyannote.audio package. Since release 2.1.1, downloading the pretrained models requires the user to accept two user agreements on Hugging Face hub and generate an authentication token. Therefore, to run the mexca pipeline, please accept the user agreements on [here](https://huggingface.co/pyannote/speaker-diarization) and [here](https://huggingface.co/pyannote/segmentation). Then, generate an authentication token [here](https://huggingface.co/settings/tokens). Use this token to login to Hugging Face hub by running `notebook_login()` (from a jupyter notebook) or `huggingface-cli login` (from the command line). You only need to login when running mexca for the first time. See this [link](https://huggingface.co/docs/hub/models-adding-libraries) for details. When running container components, you need to supply the token excplicitly as value for the `use_auth_token` argument. We recommend storing the token on your system and accessing it from Python.
 
 To create and apply the MEXCA pipeline with container components to a video file run the following code in a Jupyter notebook or a Python script (requires the base package and Docker):
 
 ```python
-from mexca.container import (AudioTranscriberContainer, FaceExtractorContainer,
-                             SentimentExtractorContainer, SpeakerIdentifierContainer, 
-                             VoiceExtractorContainer)
+from mexca.container import (
+    AudioTranscriberContainer,
+    FaceExtractorContainer,
+    SentimentExtractorContainer,
+    SpeakerIdentifierContainer,
+    VoiceExtractorContainer,
+)
 from mexca.pipeline import Pipeline
 
 # Set path to video file
 filepath = 'path/to/video'
 
 # Create standard pipeline with two faces and speakers
 pipeline = Pipeline(
```

### Comparing `mexca-0.4.0/mexca.egg-info/SOURCES.txt` & `mexca-0.5.0/mexca.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,32 +7,41 @@
 setup.cfg
 setup.py
 mexca/__init__.py
 mexca/container.py
 mexca/data.py
 mexca/pipeline.py
 mexca/utils.py
-mexca/video.py
 mexca.egg-info/PKG-INFO
 mexca.egg-info/SOURCES.txt
 mexca.egg-info/dependency_links.txt
 mexca.egg-info/entry_points.txt
 mexca.egg-info/not-zip-safe
 mexca.egg-info/requires.txt
 mexca.egg-info/top_level.txt
 mexca/audio/__init__.py
 mexca/audio/extraction.py
 mexca/audio/features.py
 mexca/audio/identification.py
 mexca/text/__init__.py
 mexca/text/sentiment.py
 mexca/text/transcription.py
+mexca/video/__init__.py
+mexca/video/anfl.py
+mexca/video/extraction.py
+mexca/video/helper_classes.py
+mexca/video/mefarg.py
+mexca/video/mefl.py
 tests/test_audio_extraction.py
 tests/test_audio_features.py
 tests/test_audio_identification.py
 tests/test_container.py
 tests/test_data.py
 tests/test_pipeline.py
 tests/test_text_sentiment.py
 tests/test_text_transcription.py
 tests/test_utils.py
-tests/test_video.py
+tests/test_video_anfl.py
+tests/test_video_extraction.py
+tests/test_video_helper_classes.py
+tests/test_video_mefarg.py
+tests/test_video_mefl.py
```

### Comparing `mexca-0.4.0/mexca.egg-info/requires.txt` & `mexca-0.5.0/mexca.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-docker==6.0.1
-intervaltree==3.1.0
+docker>=6.0.1
+intervaltree>=3.1.0
 moviepy>=1.0.3
-numpy>=1.21.6
-pandas==1.3
-pyyaml==6.0
-scipy==1.7.3
-srt==3.5.2
+numpy<1.24,>=1.21
+pandas==1.4
+pyyaml>=6.0
+scipy>=1.7.3
+srt>=3.5.2
 tqdm>=4.64.0
 
 [all]
 mexca[sen,spe,tra,vid,voi]
 
 [demo]
 ipywidgets
 
 [dev]
+black
 bump2version
 prospector[with_pyroma]==1.7.7
+pre-commit
 pylint==2.15.6
 isort
 pytest
 pytest-cov
 sphinx
 sphinx_rtd_theme
 sphinx-autoapi
@@ -38,24 +40,25 @@
 sentencepiece
 torch==1.12.0
 transformers==4.25.1
 
 [spe]
 pyannote.audio==2.1.1
 pyannote.core<5.0,>=4.4
+ruamel.yaml==0.17.28
 torch==1.12.0
 
 [tra]
 openai-whisper
-stable-ts==1.1.5
 torch==1.12.0
 transformers==4.25.1
 
 [vid]
 facenet-pytorch==2.5.2
+gdown==4.7.1
 py-feat==0.5.0
 spectralcluster==0.2.16
 torch==1.12.0
 torchvision==0.13.0
 
 [voi]
 librosa<0.10.0
```

### Comparing `mexca-0.4.0/setup.cfg` & `mexca-0.5.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -17,73 +17,76 @@
 	expression
 long_description = file: README.md
 long_description_content_type = text/markdown
 name = mexca
 project_urls = 
 	Bug Tracker = https://github.com/mexca/mexca/issues
 url = https://github.com/mexca/mexca
-version = 0.4.0
+version = 0.5.0
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
-python_requires = >=3.7,<3.10
+python_requires = >3.7,<3.11
 install_requires = 
-	docker==6.0.1
-	intervaltree==3.1.0
+	docker>=6.0.1
+	intervaltree>=3.1.0
 	moviepy>=1.0.3
-	numpy>=1.21.6
-	pandas==1.3
-	pyyaml==6.0
-	scipy==1.7.3
-	srt==3.5.2
+	numpy>=1.21,<1.24
+	pandas==1.4
+	pyyaml>=6.0
+	scipy>=1.7.3
+	srt>=3.5.2
 	tqdm>=4.64.0
 
 [options.entry_points]
 console_scripts = 
-	extract-faces = mexca.video:cli
+	extract-faces = mexca.video.extraction:cli
 	identify-speakers = mexca.audio.identification:cli
 	extract-voice = mexca.audio.extraction:cli
 	transcribe = mexca.text.transcription:cli
 	extract-sentiment = mexca.text.sentiment:cli
 
 [options.data_files]
 
 [options.extras_require]
 vid = 
 	facenet-pytorch==2.5.2
+	gdown==4.7.1
 	py-feat==0.5.0
 	spectralcluster==0.2.16
 	torch==1.12.0
 	torchvision==0.13.0
 spe = 
 	pyannote.audio==2.1.1
 	pyannote.core>=4.4,<5.0
+	ruamel.yaml==0.17.28 # necessary due to dependency issue with pyannote.audio
 	torch==1.12.0
 voi = 
 	librosa<0.10.0
 tra = 
 	openai-whisper
-	stable-ts==1.1.5
 	torch==1.12.0
 	transformers==4.25.1
 sen = 
 	accelerate==0.18.0
 	bitsandbytes==0.38.1
 	protobuf==3.20
 	sentencepiece
 	torch==1.12.0
 	transformers==4.25.1
 all = mexca[vid,spe,voi,tra,sen]
 demo = 
 	ipywidgets
 dev = 
+	black
 	bump2version
 	prospector[with_pyroma]==1.7.7
+	pre-commit
 	pylint==2.15.6
 	isort
 	pytest
 	pytest-cov
 	sphinx
 	sphinx_rtd_theme
 	sphinx-autoapi
@@ -93,18 +96,17 @@
 	twine
 	wheel
 
 [options.packages.find]
 include = mexca, mexca.*
 
 [isort]
-lines_after_imports = 2
-force_single_line = 0
-no_lines_before = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
+profile = black
 known_first_party = mexca
 src_paths = mexca,tests
-line_length = 120
+line_length = 80
+multi_line_output = 3
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `mexca-0.4.0/tests/test_audio_extraction.py` & `mexca-0.5.0/tests/test_audio_extraction.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,84 @@
 """ Test voice feature extraction classes and methods """
 
 import os
 import subprocess
-import pytest
+
 import numpy as np
-from mexca.audio.extraction import FeaturePitchF0, VoiceExtractor, VoiceFeaturesConfig
+import pytest
+
+from mexca.audio.extraction import (
+    FeaturePitchF0,
+    VoiceExtractor,
+    VoiceFeaturesConfig,
+)
 from mexca.data import VoiceFeatures
 
 
 @pytest.fixture
 def config():
     return VoiceFeaturesConfig()
 
 
 class TestVoiceFeaturesConfig:
     filename = "test.yaml"
-    
 
     def test_write_read(self, config):
         config.write_yaml(self.filename)
-        
+
         assert os.path.exists(self.filename)
 
         new_config = config.from_yaml(self.filename)
 
         assert isinstance(new_config, VoiceFeaturesConfig)
 
         os.remove(self.filename)
 
 
 class TestVoiceExtractor:
     time_step = 0.04
-    filepath = os.path.join('tests', 'test_files', 'test_video_audio_5_seconds.wav')
+    filepath = os.path.join(
+        "tests", "test_files", "test_video_audio_5_seconds.wav"
+    )
 
     @pytest.fixture
     def voice_extractor(self):
         return VoiceExtractor()
 
-
     def test_feature_dict(self):
         with pytest.raises(TypeError):
             _ = VoiceExtractor(features={1: FeaturePitchF0()})
             _ = VoiceExtractor(features={"pitch_fo_hz": [0.0]})
 
-
     def test_apply(self, voice_extractor):
         features = voice_extractor.apply(self.filepath, self.time_step)
         assert isinstance(features, VoiceFeatures)
         assert np.issubdtype(np.array(features.frame).dtype, np.int_)
-        assert np.all(np.array(features.frame) >= 0) and np.all(np.array(features.frame) <= 125)
+        assert np.all(np.array(features.frame) >= 0) and np.all(
+            np.array(features.frame) <= 125
+        )
         assert len(features.frame) == len(features.pitch_f0_hz)
 
-
     def test_cli(self, config):
         config_filepath = "test_config.yaml"
-        out_filename = os.path.splitext(os.path.basename(self.filepath))[0] + '_voice_features.json'
+        out_filename = (
+            os.path.splitext(os.path.basename(self.filepath))[0]
+            + "_voice_features.json"
+        )
         config.write_yaml(config_filepath)
-        subprocess.run(['extract-voice', '-f', self.filepath,
-                        '-o', '.', '-t', '0.04', "--config-filepath", config_filepath], check=True)
+        subprocess.run(
+            [
+                "extract-voice",
+                "-f",
+                self.filepath,
+                "-o",
+                ".",
+                "-t",
+                "0.04",
+                "--config-filepath",
+                config_filepath,
+            ],
+            check=True,
+        )
         assert os.path.exists(out_filename)
         os.remove(out_filename)
-        os.remove(config_filepath)
+        os.remove(config_filepath)
```

### Comparing `mexca-0.4.0/tests/test_audio_features.py` & `mexca-0.5.0/tests/test_audio_features.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,47 +1,50 @@
 """Test audio feature calculation classes and methods.
 """
 
 import librosa
-import pytest
 import numpy as np
+import pytest
+
 from mexca.audio.features import (
     AlphaRatioFrames,
     AudioSignal,
     BaseFrames,
     BaseSignal,
-    FormantFrames,
     FormantAmplitudeFrames,
+    FormantFrames,
     HammarIndexFrames,
+    HnrFrames,
+    JitterFrames,
     MelSpecFrames,
     MfccFrames,
     PitchFrames,
     PitchHarmonicsFrames,
     PitchPulseFrames,
-    SpectralFluxFrames,
+    RmsEnergyFrames,
+    ShimmerFrames,
     SpecFrames,
+    SpectralFluxFrames,
     SpectralSlopeFrames,
-    JitterFrames,
-    ShimmerFrames,
-    HnrFrames,
-    RmsEnergyFrames
 )
 
 
 @pytest.fixture
 def audio_file():
     return librosa.ex("trumpet")
 
 
 class TestBaseSignal:
     n_samples = 10
 
     @pytest.fixture
     def sig_obj(self):
-        return BaseSignal(np.random.uniform(-1, 1, self.n_samples), self.n_samples)
+        return BaseSignal(
+            np.random.uniform(-1, 1, self.n_samples), self.n_samples
+        )
 
     def test_idx(self, sig_obj):
         idx = sig_obj.idx
         assert np.all(idx == np.arange(self.n_samples))
 
     def test_ts(self, sig_obj):
         ts = sig_obj.ts
@@ -70,22 +73,26 @@
 
     @pytest.fixture
     def frames_scope(self, sig_frames_obj):
         return sig_frames_obj
 
     def test_idx(self, sig_obj, frames_scope):
         idx = frames_scope.idx
-        assert np.all(idx == np.arange((sig_obj.sig.shape[0] + 1) // self.hop_len + 1))
+        assert np.all(
+            idx == np.arange((sig_obj.sig.shape[0] + 1) // self.hop_len + 1)
+        )
 
     def test_ts(self, frames_scope):
         ts = frames_scope.ts
         assert np.all(
             ts
             == librosa.frames_to_time(
-                frames_scope.idx, sr=frames_scope.sr, hop_length=frames_scope.hop_len
+                frames_scope.idx,
+                sr=frames_scope.sr,
+                hop_length=frames_scope.hop_len,
             )
         )
 
 
 class TestPitchFrames(TestBaseFrames):
     @pytest.fixture
     def pitch_frames_obj(self, sig_obj):
@@ -95,15 +102,19 @@
 
     @pytest.fixture
     def frames_scope(self, pitch_frames_obj):
         return pitch_frames_obj
 
     def test_pitch_pyin(self, pitch_frames_obj):
         pitch_f0 = pitch_frames_obj.frames
-        assert pitch_f0.shape == pitch_frames_obj.ts.shape == pitch_frames_obj.idx.shape
+        assert (
+            pitch_f0.shape
+            == pitch_frames_obj.ts.shape
+            == pitch_frames_obj.idx.shape
+        )
         assert np.all(np.logical_or(pitch_f0 > 0, np.isnan(pitch_f0)))
 
 
 class TestSpecFrames(TestBaseFrames):
     @pytest.fixture
     def spec_frames_obj(self, sig_obj):
         return SpecFrames.from_signal(
@@ -112,15 +123,19 @@
 
     @pytest.fixture
     def frames_scope(self, spec_frames_obj):
         return spec_frames_obj
 
     def test_spec(self, spec_frames_obj):
         spec = spec_frames_obj.frames
-        assert spec.shape[:1] == spec_frames_obj.ts.shape == spec_frames_obj.idx.shape
+        assert (
+            spec.shape[:1]
+            == spec_frames_obj.ts.shape
+            == spec_frames_obj.idx.shape
+        )
         assert np.all(
             np.iscomplex(spec[:, 1:-1])
         )  # First and last columns are not complex
 
 
 class TestFormantFrames(TestBaseFrames):
     @pytest.fixture
@@ -185,29 +200,33 @@
             formant_frames_obj, harmonics_frames_obj, pitch_frames_obj
         )
 
     @pytest.fixture
     def frames_scope(self, formant_amp_frames_obj):
         return formant_amp_frames_obj
 
-    def test_formant_amplitude(self, formant_amp_frames_obj, formant_frames_obj):
+    def test_formant_amplitude(
+        self, formant_amp_frames_obj, formant_frames_obj
+    ):
         amp = formant_amp_frames_obj.frames
         assert isinstance(amp, np.ndarray)
         assert (
             amp.shape[0]
             == formant_amp_frames_obj.ts.shape[0]
             == formant_amp_frames_obj.idx.shape[0]
         )
         assert amp.shape[1] == formant_frames_obj.max_formants
 
 
 class TestPitchPulseFrames(TestPitchFrames):
     @pytest.fixture
     def pulses_frames_obj(self, sig_obj, pitch_frames_obj):
-        return PitchPulseFrames.from_signal_and_pitch_frames(sig_obj, pitch_frames_obj)
+        return PitchPulseFrames.from_signal_and_pitch_frames(
+            sig_obj, pitch_frames_obj
+        )
 
     @pytest.fixture
     def frames_scope(self, pulses_frames_obj):
         return pulses_frames_obj
 
     def test_pulses(self, pulses_frames_obj):
         pulses = pulses_frames_obj.frames
@@ -231,34 +250,47 @@
     def test_get_next_pulse(self, pulses_frames_obj):
         frame = np.random.uniform(-1, 1, self.frame_len)
         ts = np.linspace(0, 1, num=self.frame_len)
         t0 = 0.005 + np.random.uniform(0, 0.0005, self.frame_len)
         start = 0.5 - 0.0025
         stop = 0.5 + 0.0025
         pulses = []
-        pulses_frames_obj._get_next_pulse(frame, ts, t0, start, stop, True, pulses)
-        pulses_frames_obj._get_next_pulse(frame, ts, t0, start, stop, False, pulses)
+        pulses_frames_obj._get_next_pulse(
+            frame, ts, t0, start, stop, True, pulses
+        )
+        pulses_frames_obj._get_next_pulse(
+            frame, ts, t0, start, stop, False, pulses
+        )
         assert len(pulses) > 0
         assert np.all(
-            np.array([isinstance(puls, tuple) and puls[0] >= 0 and puls[1] >= 0 for puls in pulses])
+            np.array(
+                [
+                    isinstance(puls, tuple) and puls[0] >= 0 and puls[1] >= 0
+                    for puls in pulses
+                ]
+            )
         )
 
 
 class TestJitterFrames(TestPitchPulseFrames):
     @pytest.fixture
     def jitter_frames_obj(self, pulses_frames_obj):
         return JitterFrames.from_pitch_pulse_frames(pulses_frames_obj)
 
     @pytest.fixture
     def frames_scope(self, jitter_frames_obj):
         return jitter_frames_obj
 
     def test_jitter(self, jitter_frames_obj):
         jitter = jitter_frames_obj.frames
-        assert jitter.shape == jitter_frames_obj.ts.shape == jitter_frames_obj.idx.shape
+        assert (
+            jitter.shape
+            == jitter_frames_obj.ts.shape
+            == jitter_frames_obj.idx.shape
+        )
         assert np.all(np.logical_or(jitter > 0, np.isnan(jitter)))
 
     def test_calc_jitter_frame(self, pulses_frames_obj, jitter_frames_obj):
         jitter_frame = jitter_frames_obj._calc_jitter_frame(
             pulses_frames_obj.frames[1],
             rel=True,
             lower=0.0001,
@@ -277,15 +309,17 @@
     @pytest.fixture
     def frames_scope(self, shimmer_frames_obj):
         return shimmer_frames_obj
 
     def test_shimmer(self, shimmer_frames_obj):
         shimmer = shimmer_frames_obj.frames
         assert (
-            shimmer.shape == shimmer_frames_obj.ts.shape == shimmer_frames_obj.idx.shape
+            shimmer.shape
+            == shimmer_frames_obj.ts.shape
+            == shimmer_frames_obj.idx.shape
         )
         assert np.all(np.logical_or(shimmer > 0, np.isnan(shimmer)))
 
     def test_calc_shimmer_frame(self, pulses_frames_obj, shimmer_frames_obj):
         shimmer_frame = shimmer_frames_obj._calc_shimmer_frame(
             pulses_frames_obj.frames[1],
             rel=True,
@@ -297,174 +331,215 @@
         assert isinstance(shimmer_frame, float)
         assert shimmer_frame > 0 or np.isnan(shimmer_frame)
 
     def test_get_amplitude(self, pulses_frames_obj, shimmer_frames_obj):
         _, mask = shimmer_frames_obj._calc_period_length(
             pulses_frames_obj.frames[1], 0.0001, 0.02
         )
-        amps = shimmer_frames_obj._get_amplitude(pulses_frames_obj.frames[1], mask)
+        amps = shimmer_frames_obj._get_amplitude(
+            pulses_frames_obj.frames[1], mask
+        )
         assert isinstance(amps, list)
 
 
 class TestHnrFrames(TestBaseFrames):
     @pytest.fixture
     def hnr_frames_obj(self, sig_frames_obj):
         return HnrFrames.from_frames(sig_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, hnr_frames_obj):
         return hnr_frames_obj
-    
 
     def test_hnr(self, hnr_frames_obj):
         hnr = hnr_frames_obj.frames
         assert hnr.shape == hnr_frames_obj.ts.shape == hnr_frames_obj.idx.shape
         assert np.all(np.logical_or(10 ** (hnr / 10) > 0, np.isnan(hnr)))
 
-
     def test_find_max_peak(self, hnr_frames_obj):
-        sig = (1 + 0.3 * np.sin(2 * np.pi * 140 * np.linspace(0, 1, self.frame_len)))
+        sig = 1 + 0.3 * np.sin(
+            2 * np.pi * 140 * np.linspace(0, 1, self.frame_len)
+        )
         autocor = librosa.autocorrelate(sig)
-        max_peak = hnr_frames_obj._find_max_peak(autocor, hnr_frames_obj.sr, hnr_frames_obj.lower)
-        assert max_peak == autocor[(1 / np.arange(autocor.shape[0]) * hnr_frames_obj.sr) < hnr_frames_obj.sr / 2].max()
-
+        max_peak = hnr_frames_obj._find_max_peak(
+            autocor, hnr_frames_obj.sr, hnr_frames_obj.lower
+        )
+        assert (
+            max_peak
+            == autocor[
+                (1 / np.arange(autocor.shape[0]) * hnr_frames_obj.sr)
+                < hnr_frames_obj.sr / 2
+            ].max()
+        )
 
     def test_find_max_peak_all_below_threshold(self, hnr_frames_obj):
-        sig = (1 + 0.3 * np.sin(2 * np.pi * 0 * np.linspace(0, 1, self.frame_len)))
+        sig = 1 + 0.3 * np.sin(
+            2 * np.pi * 0 * np.linspace(0, 1, self.frame_len)
+        )
         autocor = librosa.autocorrelate(sig)
-        max_peak = hnr_frames_obj._find_max_peak(autocor, hnr_frames_obj.sr, hnr_frames_obj.lower)
+        max_peak = hnr_frames_obj._find_max_peak(
+            autocor, hnr_frames_obj.sr, hnr_frames_obj.lower
+        )
         assert np.isnan(max_peak)
 
 
 class TestAlphaRatioFrames(TestSpecFrames):
     @pytest.fixture
     def alpha_ratio_frames_obj(self, spec_frames_obj):
         return AlphaRatioFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, alpha_ratio_frames_obj):
         return alpha_ratio_frames_obj
-    
 
     def test_alpha_ratio(self, alpha_ratio_frames_obj):
         alpha_ratio = alpha_ratio_frames_obj.frames
-        assert alpha_ratio.shape == alpha_ratio_frames_obj.ts.shape == alpha_ratio_frames_obj.idx.shape
-        assert np.all(np.logical_or(10 ** (alpha_ratio / 10) > 0, np.isnan(alpha_ratio)))
+        assert (
+            alpha_ratio.shape
+            == alpha_ratio_frames_obj.ts.shape
+            == alpha_ratio_frames_obj.idx.shape
+        )
+        assert np.all(
+            np.logical_or(10 ** (alpha_ratio / 10) > 0, np.isnan(alpha_ratio))
+        )
 
 
 class TestHammarIndexFrames(TestSpecFrames):
     @pytest.fixture
     def hammar_index_frames_obj(self, spec_frames_obj):
         return HammarIndexFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, hammar_index_frames_obj):
         return hammar_index_frames_obj
-    
 
     def test_hammar_index(self, hammar_index_frames_obj):
         hammar_index = hammar_index_frames_obj.frames
-        assert hammar_index.shape == hammar_index_frames_obj.ts.shape == hammar_index_frames_obj.idx.shape
-        assert np.all(np.logical_or(10 ** (hammar_index / 10) > 0, np.isnan(hammar_index)))
+        assert (
+            hammar_index.shape
+            == hammar_index_frames_obj.ts.shape
+            == hammar_index_frames_obj.idx.shape
+        )
+        assert np.all(
+            np.logical_or(10 ** (hammar_index / 10) > 0, np.isnan(hammar_index))
+        )
 
 
 class TestSpectralSlopeFrames(TestSpecFrames):
     @pytest.fixture
     def spectral_slope_frames_obj(self, spec_frames_obj):
         return SpectralSlopeFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, spectral_slope_frames_obj):
         return spectral_slope_frames_obj
-    
 
     def test_spectral_slope(self, spectral_slope_frames_obj):
         spectral_slope = spectral_slope_frames_obj.frames
-        assert spectral_slope.shape[:1] == spectral_slope_frames_obj.ts.shape == spectral_slope_frames_obj.idx.shape
-    
+        assert (
+            spectral_slope.shape[:1]
+            == spectral_slope_frames_obj.ts.shape
+            == spectral_slope_frames_obj.idx.shape
+        )
 
     def test_calc_spectral_slope(self, spectral_slope_frames_obj):
         n = 512
         band_power = np.random.uniform(0, 1, n)
         band_freqs = np.random.uniform(0, 8000, n)
-        coefs = spectral_slope_frames_obj._calc_spectral_slope(band_power, band_freqs)
+        coefs = spectral_slope_frames_obj._calc_spectral_slope(
+            band_power, band_freqs
+        )
         assert coefs.shape == (1,)
 
-
     def test_calc_spectral_slope_nan(self, spectral_slope_frames_obj):
         n = 512
         band_power = np.random.uniform(0, 1, n)
         band_freqs = np.random.uniform(0, 8000, n)
         band_power[1:3] = np.nan
-        coefs = spectral_slope_frames_obj._calc_spectral_slope(band_power, band_freqs)
+        coefs = spectral_slope_frames_obj._calc_spectral_slope(
+            band_power, band_freqs
+        )
         assert coefs.shape == (1,)
 
 
 class TestMelSpecFrames(TestSpecFrames):
     @pytest.fixture
     def mel_spec_frames_obj(self, spec_frames_obj):
         return MelSpecFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, mel_spec_frames_obj):
         return mel_spec_frames_obj
-    
 
     def test_spectral_slope(self, mel_spec_frames_obj):
         mel_spec = mel_spec_frames_obj.frames
-        assert mel_spec.shape[:1] == mel_spec_frames_obj.ts.shape == mel_spec_frames_obj.idx.shape
+        assert (
+            mel_spec.shape[:1]
+            == mel_spec_frames_obj.ts.shape
+            == mel_spec_frames_obj.idx.shape
+        )
         assert mel_spec.shape[1] == mel_spec_frames_obj.n_mels
 
 
 class TestMfccFrames(TestMelSpecFrames):
     @pytest.fixture
     def mfcc_frames_obj(self, mel_spec_frames_obj):
         return MfccFrames.from_mel_spec_frames(mel_spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, mfcc_frames_obj):
         return mfcc_frames_obj
-    
 
     def test_mfcc(self, mfcc_frames_obj):
         mfcc = mfcc_frames_obj.frames
-        assert mfcc.shape[:1] == mfcc_frames_obj.ts.shape == mfcc_frames_obj.idx.shape
+        assert (
+            mfcc.shape[:1]
+            == mfcc_frames_obj.ts.shape
+            == mfcc_frames_obj.idx.shape
+        )
         assert mfcc.shape[1] == mfcc_frames_obj.n_mfcc
 
 
 class TestSpectralFluxFrames(TestSpecFrames):
     @pytest.fixture
     def spectral_flux_frames_obj(self, spec_frames_obj):
         return SpectralFluxFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, spectral_flux_frames_obj):
         return spectral_flux_frames_obj
-    
 
     def test_idx(self, sig_obj, frames_scope):
         idx = frames_scope.idx
-        assert np.all(idx == np.arange((sig_obj.sig.shape[0] + 1) // self.hop_len))
-
+        assert np.all(
+            idx == np.arange((sig_obj.sig.shape[0] + 1) // self.hop_len)
+        )
 
     def test_spectral_flux(self, spectral_flux_frames_obj):
         spectral_flux = spectral_flux_frames_obj.frames
 
-        assert spectral_flux.shape == spectral_flux_frames_obj.ts.shape == spectral_flux_frames_obj.idx.shape
+        assert (
+            spectral_flux.shape
+            == spectral_flux_frames_obj.ts.shape
+            == spectral_flux_frames_obj.idx.shape
+        )
         assert np.all(spectral_flux > 0)
 
 
 class TestRmsEnergyFrames(TestSpecFrames):
     @pytest.fixture
     def rms_energy_frames_obj(self, spec_frames_obj):
         return RmsEnergyFrames.from_spec_frames(spec_frames_obj)
-    
+
     @pytest.fixture
     def frames_scope(self, rms_energy_frames_obj):
         return rms_energy_frames_obj
-        
 
     def test_rms_energy(self, rms_energy_frames_obj):
         rms_energy = rms_energy_frames_obj.frames
-        
-        assert rms_energy.shape == rms_energy_frames_obj.ts.shape == rms_energy_frames_obj.idx.shape
+
+        assert (
+            rms_energy.shape
+            == rms_energy_frames_obj.ts.shape
+            == rms_energy_frames_obj.idx.shape
+        )
         assert np.all(10 ** (rms_energy / 10.0) > 0)
```

### Comparing `mexca-0.4.0/tests/test_audio_identification.py` & `mexca-0.5.0/tests/test_audio_identification.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,91 +1,102 @@
 """ Test speaker identification classes and methods """
 
 import os
 import subprocess
+
 import pytest
 from huggingface_hub import HfFolder
 from pyannote.audio import Pipeline
+
 from mexca.audio import SpeakerIdentifier
 from mexca.audio.identification import AuthenticationError
 from mexca.data import SegmentData, SpeakerAnnotation
 
 
 class TestSpeakerIdentifier:
-    use_auth_token = os.environ['HF_TOKEN'] if 'HF_TOKEN' in os.environ else True
+    use_auth_token = (
+        os.environ["HF_TOKEN"] if "HF_TOKEN" in os.environ else True
+    )
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.wav'
+        "tests", "test_files", "test_video_audio_5_seconds.wav"
     )
 
-
     @staticmethod
     def check_rttm_annotation(annotation):
         assert isinstance(annotation, SpeakerAnnotation)
-                
+
         for seg in annotation.items():
             assert isinstance(seg.data, SegmentData)
             assert isinstance(seg.begin, float)
             assert 5.0 >= seg.begin >= 0.0
             assert isinstance(seg.end, float)
             assert 5.0 >= seg.end >= 0.0
             assert isinstance(seg.data.name, str)
 
-
     @pytest.fixture
     def speaker_identifier(self):
         return SpeakerIdentifier(use_auth_token=self.use_auth_token)
 
-
     def test_lazy_init(self, speaker_identifier):
         assert not speaker_identifier._pipeline
         assert isinstance(speaker_identifier.pipeline, Pipeline)
         del speaker_identifier.pipeline
         assert not speaker_identifier._pipeline
 
-
     hf_folder = HfFolder()
 
-
     @pytest.mark.skipif(
         hf_folder.get_token() is not None,
-        reason='Running test locally and a token might be cached'
+        reason="Running test locally and a token might be cached",
     )
     def test_environment_error(self):
         with pytest.raises(EnvironmentError):
             speaker_identifier = SpeakerIdentifier(use_auth_token=True)
             speaker_identifier.pipeline
 
-
     def test_authentication_error(self):
         with pytest.raises(AuthenticationError):
-            speaker_identifier = SpeakerIdentifier(use_auth_token='')
+            speaker_identifier = SpeakerIdentifier(use_auth_token="")
             speaker_identifier.pipeline
 
         with pytest.raises(AuthenticationError):
-            speaker_identifier = SpeakerIdentifier(use_auth_token='hf_riskdkdifseflskefssfjsfsjfsfjsfsfj') # dummy token
+            speaker_identifier = SpeakerIdentifier(
+                use_auth_token="hf_riskdkdifseflskefssfjsfsjfsfjsfsfj"
+            )  # dummy token
             speaker_identifier.pipeline
 
-
     def test_apply(self, speaker_identifier):
         annotation = speaker_identifier.apply(self.filepath)
 
         self.check_rttm_annotation(annotation)
 
-
     def test_apply_num_speakers(self):
         num_speakers = 2
         speaker_identifier = SpeakerIdentifier(
             num_speakers=num_speakers,
             use_auth_token=self.use_auth_token,
         )
         annotation = speaker_identifier.apply(self.filepath)
 
         self.check_rttm_annotation(annotation)
 
-
     def test_cli(self):
-        out_filename = os.path.splitext(os.path.basename(self.filepath))[0] + '_audio_annotation.rttm'
-        subprocess.run(['identify-speakers', '-f', self.filepath,
-                        '-o', '.', '--num-speakers', '2',
-                        '--use-auth-token', self.use_auth_token], check=True)
+        out_filename = (
+            os.path.splitext(os.path.basename(self.filepath))[0]
+            + "_audio_annotation.rttm"
+        )
+        subprocess.run(
+            [
+                "identify-speakers",
+                "-f",
+                self.filepath,
+                "-o",
+                ".",
+                "--num-speakers",
+                "2",
+                "--use-auth-token",
+                self.use_auth_token,
+            ],
+            check=True,
+        )
         assert os.path.exists(out_filename)
         os.remove(out_filename)
```

### Comparing `mexca-0.4.0/tests/test_container.py` & `mexca-0.5.0/tests/test_container.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,155 +1,164 @@
 import os
+
 import pytest
 from docker.errors import NotFound
-from mexca.container import AudioTranscriberContainer, BaseContainer, FaceExtractorContainer, SentimentExtractorContainer, SpeakerIdentifierContainer, VoiceExtractorContainer
+
+from mexca.container import (
+    AudioTranscriberContainer,
+    BaseContainer,
+    FaceExtractorContainer,
+    SentimentExtractorContainer,
+    SpeakerIdentifierContainer,
+    VoiceExtractorContainer,
+)
 from mexca.pipeline import Pipeline
 from mexca.utils import _validate_multimodal
 
 
-@pytest.mark.skip_env('runner')
+@pytest.mark.skip_env("runner")
 class TestBaseContainer:
     def test_invalid_image_name(self):
         with pytest.raises(NotFound):
-            BaseContainer(image_name='sdfsdf')
-
+            BaseContainer(image_name="sdfsdf")
 
     def test_get_latest_tag(self):
         container = VoiceExtractorContainer(get_latest_tag=True)
         assert isinstance(container, VoiceExtractorContainer)
-        assert container.image_name == 'mexca/voice-extractor:latest'
+        assert container.image_name == "mexca/voice-extractor:latest"
 
 
-@pytest.mark.skip_env('runner')
+@pytest.mark.skip_env("runner")
 class TestPipelineContainer:
-    use_auth_token = os.environ['HF_TOKEN'] if 'HF_TOKEN' in os.environ else True
+    use_auth_token = (
+        os.environ["HF_TOKEN"] if "HF_TOKEN" in os.environ else True
+    )
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.mp4'
+        "tests", "test_files", "test_video_audio_5_seconds.mp4"
     )
-    components = ["face-extractor", "speaker-identifier", "voice-extractor", "audio-transcriber", "sentiment-extractor"]
-
+    components = [
+        "face-extractor",
+        "speaker-identifier",
+        "voice-extractor",
+        "audio-transcriber",
+        "sentiment-extractor",
+    ]
 
     @pytest.fixture
     def face_extractor_pipeline(self, num_faces=2):
         pipeline = Pipeline(
             face_extractor=FaceExtractorContainer(num_faces=num_faces)
         )
 
         return pipeline
 
-
     @pytest.fixture
     def speaker_identifier_pipeline(self, num_speakers=2):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifierContainer(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             )
         )
 
         return pipeline
 
-
     @pytest.fixture
     def voice_extractor_pipeline(self):
-        pipeline = Pipeline(
-            voice_extractor=VoiceExtractorContainer()
-        )
+        pipeline = Pipeline(voice_extractor=VoiceExtractorContainer())
 
         return pipeline
 
-
     @pytest.fixture
     def speaker_identifier_transcription_pipeline(self, num_speakers=2):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifierContainer(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             ),
-            audio_transcriber=AudioTranscriberContainer(whisper_model='tiny')
+            audio_transcriber=AudioTranscriberContainer(whisper_model="tiny"),
         )
 
         return pipeline
 
-
     @pytest.fixture
-    def speaker_identifier_transcription_sentiment_pipeline(self, num_speakers=2):
+    def speaker_identifier_transcription_sentiment_pipeline(
+        self, num_speakers=2
+    ):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifierContainer(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             ),
-            audio_transcriber=AudioTranscriberContainer(whisper_model='tiny'),
-            sentiment_extractor=SentimentExtractorContainer()
+            audio_transcriber=AudioTranscriberContainer(whisper_model="tiny"),
+            sentiment_extractor=SentimentExtractorContainer(),
         )
 
         return pipeline
 
-
     def test_face_extractor_pipeline(self, face_extractor_pipeline):
         result = face_extractor_pipeline.apply(
             self.filepath,
             frame_batch_size=5,
             skip_frames=5,
-            keep_audiofile=True
+            keep_audiofile=True,
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_audio_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
     def test_speaker_identifier_pipeline(self, speaker_identifier_pipeline):
         result = speaker_identifier_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
     def test_voice_extractor_pipeline(self, voice_extractor_pipeline):
         result = voice_extractor_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_audio_annotation=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_speaker_identifier_transcription_pipeline(self, speaker_identifier_transcription_pipeline):
+    def test_speaker_identifier_transcription_pipeline(
+        self, speaker_identifier_transcription_pipeline
+    ):
         result = speaker_identifier_transcription_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_voice_features=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_speaker_identifier_transcription_sentiment_pipeline(self, speaker_identifier_transcription_sentiment_pipeline):
+    def test_speaker_identifier_transcription_sentiment_pipeline(
+        self, speaker_identifier_transcription_sentiment_pipeline
+    ):
         result = speaker_identifier_transcription_sentiment_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
-            check_video_annotation=False,
-            check_voice_features=False
+        _validate_multimodal(
+            result, check_video_annotation=False, check_voice_features=False
         )
-
```

### Comparing `mexca-0.4.0/tests/test_data.py` & `mexca-0.5.0/tests/test_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,48 @@
 """Test data classes and methods.
 """
 
 import datetime
 import os
+
 import pytest
 import srt
 from intervaltree import Interval, IntervalTree
 from pyannote.core import Annotation, Segment
-from mexca.data import AudioTranscription, Multimodal, SegmentData, SentimentData, SentimentAnnotation, SpeakerAnnotation, TranscriptionData, VideoAnnotation, VoiceFeatures, _get_rttm_header
+
+from mexca.data import (
+    AudioTranscription,
+    Multimodal,
+    SegmentData,
+    SentimentAnnotation,
+    SentimentData,
+    SpeakerAnnotation,
+    TranscriptionData,
+    VideoAnnotation,
+    VoiceFeatures,
+    _get_rttm_header,
+)
 from mexca.utils import _validate_multimodal
 
 
 class TestVideoAnnotation:
     def test_write_from_json(self):
-        filename = 'test.json'
+        filename = "test.json"
         annotation = VideoAnnotation(frame=[0, 1, 2])
         annotation.write_json(filename)
         assert os.path.exists(filename)
         annotation = VideoAnnotation.from_json(filename=filename)
         assert isinstance(annotation, VideoAnnotation)
         assert annotation.frame == [0, 1, 2]
         os.remove(filename)
 
 
 class TestVoiceFeatures:
     def test_write_from_json(self):
-        filename = 'test.json'
+        filename = "test.json"
         annotation = VoiceFeatures(frame=[0, 1, 2], time=[0, 1, 2])
         annotation.write_json(filename)
         assert os.path.exists(filename)
         annotation = VoiceFeatures.from_json(filename=filename)
         assert isinstance(annotation, VoiceFeatures)
         assert annotation.frame == [0, 1, 2]
         assert annotation.time == [0, 1, 2]
@@ -47,234 +60,285 @@
     def check_object(obj):
         assert isinstance(obj, SpeakerAnnotation)
         assert len(obj) == 1
         assert isinstance(list(obj.items())[0].data, SegmentData)
 
     def test_from_pyannote(self):
         annotation = Annotation()
-        annotation[Segment(0, 1), 'A'] = 'spk_1'
+        annotation[Segment(0, 1), "A"] = "spk_1"
 
-        speaker_annotation = SpeakerAnnotation.from_pyannote(annotation=annotation)
-        
-        self.check_object(speaker_annotation)
+        speaker_annotation = SpeakerAnnotation.from_pyannote(
+            annotation=annotation
+        )
 
+        self.check_object(speaker_annotation)
 
     def test_write_from_rttm(self):
-        filename = 'test.rttm'
+        filename = "test.rttm"
         speaker_annotation = SpeakerAnnotation(
-            [Interval(0.0, 1.0, data=SegmentData(filename=filename, channel=1, name='spk_1'))]
+            [
+                Interval(
+                    0.0,
+                    1.0,
+                    data=SegmentData(
+                        filename=filename, channel=1, name="spk_1"
+                    ),
+                )
+            ]
         )
 
         speaker_annotation.write_rttm(filename=filename)
         assert os.path.exists(filename)
 
         speaker_annotation = SpeakerAnnotation.from_rttm(filename)
         self.check_object(speaker_annotation)
         os.remove(filename)
 
 
 class TestAudioTranscription:
     def test_write_from_srt(self):
-        filename = 'test.srt'
+        filename = "test.srt"
         transcription = AudioTranscription(
             filename=filename,
-            subtitles=IntervalTree([
-                Interval(
-                    begin=0,
-                    end=1,
-                    data=TranscriptionData(
-                        index=0,
-                        text="Test",
-                        speaker='1'
+            subtitles=IntervalTree(
+                [
+                    Interval(
+                        begin=0,
+                        end=1,
+                        data=TranscriptionData(
+                            index=0, text="Test", speaker="1"
+                        ),
                     )
-                )
-            ])
+                ]
+            ),
         )
 
         transcription.write_srt(filename=filename)
         assert os.path.exists(filename)
 
         transcription = AudioTranscription.from_srt(filename=filename)
         assert isinstance(transcription, AudioTranscription)
         for seg in transcription.subtitles.items():
             assert isinstance(seg.data, TranscriptionData)
-        
+
         os.remove(filename)
 
 
 class TestSentimentAnnotation:
     def test_write_from_json(self):
-        filename = 'test.json'
-        sentiment = SentimentAnnotation([Interval(
-            begin=0,
-            end=1,
-            data=SentimentData(
-                text='test',
-                pos=0.4,
-                neg=0.4,
-                neu=0.2
-            )
-        )])
+        filename = "test.json"
+        sentiment = SentimentAnnotation(
+            [
+                Interval(
+                    begin=0,
+                    end=1,
+                    data=SentimentData(text="test", pos=0.4, neg=0.4, neu=0.2),
+                )
+            ]
+        )
         sentiment.write_json(filename)
         assert os.path.exists(filename)
         sentiment = SentimentAnnotation.from_json(filename=filename)
         assert isinstance(sentiment, SentimentAnnotation)
         for sent in sentiment.items():
             assert isinstance(sent.data, SentimentData)
         os.remove(filename)
 
 
 class TestMultimodal:
-    ref_dir = os.path.join('tests', 'reference_files')
-    filepath = 'test_video_audio_5_seconds.mp4'
-
+    ref_dir = os.path.join("tests", "reference_files")
+    filepath = "test_video_audio_5_seconds.mp4"
 
     @pytest.fixture
     def video_annotation(self) -> VideoAnnotation:
         return VideoAnnotation.from_json(
-            os.path.join(self.ref_dir, 'test_video_audio_5_seconds_video_annotation.json')
+            os.path.join(
+                self.ref_dir, "test_video_audio_5_seconds_video_annotation.json"
+            )
         )
 
-
     @pytest.fixture
     def audio_annotation(self) -> SpeakerAnnotation:
-        return SpeakerAnnotation([
-            Interval(begin=1.92, end=2.92, data=SegmentData(filename=self.filepath, channel=0, name=0)),
-            Interval(begin=3.86, end=4.87, data=SegmentData(filename=self.filepath, channel=0, name=0))
-        ])
-
+        return SpeakerAnnotation(
+            [
+                Interval(
+                    begin=1.92,
+                    end=2.92,
+                    data=SegmentData(filename=self.filepath, channel=0, name=0),
+                ),
+                Interval(
+                    begin=3.86,
+                    end=4.87,
+                    data=SegmentData(filename=self.filepath, channel=0, name=0),
+                ),
+            ]
+        )
 
     @pytest.fixture
     def voice_features(self) -> VoiceFeatures:
         return VoiceFeatures.from_json(
-            os.path.join(self.ref_dir, 'test_video_audio_5_seconds_voice_features.json')
+            os.path.join(
+                self.ref_dir, "test_video_audio_5_seconds_voice_features.json"
+            )
         )
 
-
     @pytest.fixture
     def transcription(self) -> AudioTranscription:
         return AudioTranscription(
             filename=self.filepath,
-            subtitles=IntervalTree([
-                Interval(begin=2.00, end=2.41, data=TranscriptionData(index=0, text='Thank you, honey.', speaker='0')),
-                Interval(begin=4.47, end=4.67, data=TranscriptionData(index=1, text='I, uh...', speaker='0'))
-            ])
+            subtitles=IntervalTree(
+                [
+                    Interval(
+                        begin=2.00,
+                        end=2.41,
+                        data=TranscriptionData(
+                            index=0, text="Thank you, honey.", speaker="0"
+                        ),
+                    ),
+                    Interval(
+                        begin=4.47,
+                        end=4.67,
+                        data=TranscriptionData(
+                            index=1, text="I, uh...", speaker="0"
+                        ),
+                    ),
+                ]
+            ),
         )
 
-
     @pytest.fixture
     def sentiment(self) -> SentimentAnnotation:
-        return SentimentAnnotation([
-            Interval(begin=2.00, end=2.41, data=SentimentData(text='Thank you, honey.', pos=0.88, neg=0.02, neu=0.1)),
-            Interval(begin=4.47, end=4.67, data=SentimentData(text='I, uh...', pos=0.1, neg=0.37, neu=0.53))
-        ])
-
+        return SentimentAnnotation(
+            [
+                Interval(
+                    begin=2.00,
+                    end=2.41,
+                    data=SentimentData(
+                        text="Thank you, honey.", pos=0.88, neg=0.02, neu=0.1
+                    ),
+                ),
+                Interval(
+                    begin=4.47,
+                    end=4.67,
+                    data=SentimentData(
+                        text="I, uh...", pos=0.1, neg=0.37, neu=0.53
+                    ),
+                ),
+            ]
+        )
 
     @pytest.fixture
-    def multimodal(self, video_annotation, audio_annotation, voice_features, transcription, sentiment) -> Multimodal:
+    def multimodal(
+        self,
+        video_annotation,
+        audio_annotation,
+        voice_features,
+        transcription,
+        sentiment,
+    ) -> Multimodal:
         return Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
             video_annotation=video_annotation,
             audio_annotation=audio_annotation,
             voice_features=voice_features,
             transcription=transcription,
-            sentiment=sentiment
+            sentiment=sentiment,
         )
 
-
     def test_merge_features(self, multimodal):
         multimodal.merge_features()
         _validate_multimodal(multimodal)
 
-
     def test_merge_features_video_annotation(self, video_annotation):
         output = Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
-            video_annotation=video_annotation
+            video_annotation=video_annotation,
         )
 
         output.merge_features()
-        _validate_multimodal(output,
+        _validate_multimodal(
+            output,
             check_audio_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
     def test_merge_features_audio_annotation(self, audio_annotation):
         output = Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
-            audio_annotation=audio_annotation
+            audio_annotation=audio_annotation,
         )
 
         output.merge_features()
-        _validate_multimodal(output,
+        _validate_multimodal(
+            output,
             check_video_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-    
     def test_merge_features_voice_features(self, voice_features):
         output = Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
-            voice_features=voice_features
+            voice_features=voice_features,
         )
 
         output.merge_features()
-        _validate_multimodal(output,
+        _validate_multimodal(
+            output,
             check_video_annotation=False,
             check_audio_annotation=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_merge_features_transcription(self, audio_annotation, transcription):
+    def test_merge_features_transcription(
+        self, audio_annotation, transcription
+    ):
         output = Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
             audio_annotation=audio_annotation,
-            transcription=transcription
+            transcription=transcription,
         )
 
         output.merge_features()
-        _validate_multimodal(output,
+        _validate_multimodal(
+            output,
             check_video_annotation=False,
             check_voice_features=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_merge_features_sentiment(self, audio_annotation, transcription, sentiment):
+    def test_merge_features_sentiment(
+        self, audio_annotation, transcription, sentiment
+    ):
         output = Multimodal(
             filename=self.filepath,
             duration=5.0,
             fps=25,
             fps_adjusted=5,
             audio_annotation=audio_annotation,
             transcription=transcription,
-            sentiment=sentiment
+            sentiment=sentiment,
         )
 
         output.merge_features()
-        _validate_multimodal(output,
-            check_video_annotation=False,
-            check_voice_features=False
+        _validate_multimodal(
+            output, check_video_annotation=False, check_voice_features=False
         )
-
```

### Comparing `mexca-0.4.0/tests/test_pipeline.py` & `mexca-0.5.0/tests/test_pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,168 +1,166 @@
 import os
 import platform
+
 import pytest
+
 from mexca.audio import SpeakerIdentifier, VoiceExtractor
 from mexca.pipeline import Pipeline
 from mexca.text import AudioTranscriber, SentimentExtractor
 from mexca.utils import _validate_multimodal
 from mexca.video import FaceExtractor
 
 
 class TestPipeline:
-    use_auth_token = os.environ['HF_TOKEN'] if 'HF_TOKEN' in os.environ else True
+    use_auth_token = (
+        os.environ["HF_TOKEN"] if "HF_TOKEN" in os.environ else True
+    )
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.mp4'
+        "tests", "test_files", "test_video_audio_5_seconds.mp4"
     )
 
     @pytest.fixture
     def full_pipeline(self, num_faces=2, num_speakers=2):
         pipeline = Pipeline(
             face_extractor=FaceExtractor(num_faces=num_faces),
             speaker_identifier=SpeakerIdentifier(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             ),
             voice_extractor=VoiceExtractor(),
-            audio_transcriber=AudioTranscriber(whisper_model='tiny'),
-            sentiment_extractor=SentimentExtractor()
+            audio_transcriber=AudioTranscriber(whisper_model="tiny"),
+            sentiment_extractor=SentimentExtractor(),
         )
 
         return pipeline
 
-
     @pytest.fixture
     def face_extractor_pipeline(self, num_faces=2):
-        pipeline = Pipeline(
-            face_extractor=FaceExtractor(num_faces=num_faces)
-        )
+        pipeline = Pipeline(face_extractor=FaceExtractor(num_faces=num_faces))
 
         return pipeline
 
-
     @pytest.fixture
     def speaker_identifier_pipeline(self, num_speakers=2):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifier(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             )
         )
 
         return pipeline
 
-
     @pytest.fixture
     def voice_extractor_pipeline(self):
-        pipeline = Pipeline(
-            voice_extractor=VoiceExtractor()
-        )
+        pipeline = Pipeline(voice_extractor=VoiceExtractor())
 
         return pipeline
 
-
     @pytest.fixture
     def speaker_identifier_transcription_pipeline(self, num_speakers=2):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifier(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             ),
-            audio_transcriber=AudioTranscriber(whisper_model='tiny')
+            audio_transcriber=AudioTranscriber(whisper_model="tiny"),
         )
 
         return pipeline
 
-
     @pytest.fixture
-    def speaker_identifier_transcription_sentiment_pipeline(self, num_speakers=2):
+    def speaker_identifier_transcription_sentiment_pipeline(
+        self, num_speakers=2
+    ):
         pipeline = Pipeline(
             speaker_identifier=SpeakerIdentifier(
-                num_speakers=num_speakers,
-                use_auth_token=self.use_auth_token
+                num_speakers=num_speakers, use_auth_token=self.use_auth_token
             ),
-            audio_transcriber=AudioTranscriber(whisper_model='tiny'),
-            sentiment_extractor=SentimentExtractor()
+            audio_transcriber=AudioTranscriber(whisper_model="tiny"),
+            sentiment_extractor=SentimentExtractor(),
         )
 
         return pipeline
 
-
     def test_full_pipeline(self, full_pipeline):
         result = full_pipeline.apply(
             self.filepath,
             frame_batch_size=5,
             skip_frames=5,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        check_darwin = platform.system() != 'Darwin'
-        _validate_multimodal(result, check_transcription=check_darwin, check_sentiment=check_darwin) # Currently fails only on macOS for unknown reason
-
+        check_darwin = platform.system() != "Darwin"
+        _validate_multimodal(
+            result,
+            check_transcription=check_darwin,
+            check_sentiment=check_darwin,
+        )  # Currently fails only on macOS for unknown reason
 
     def test_face_extractor_pipeline(self, face_extractor_pipeline):
         result = face_extractor_pipeline.apply(
             self.filepath,
             frame_batch_size=5,
             skip_frames=5,
-            keep_audiofile=True
+            keep_audiofile=True,
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_audio_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
     def test_speaker_identifier_pipeline(self, speaker_identifier_pipeline):
         result = speaker_identifier_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_voice_features=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
     def test_voice_extractor_pipeline(self, voice_extractor_pipeline):
         result = voice_extractor_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_audio_annotation=False,
             check_transcription=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_speaker_identifier_transcription_pipeline(self, speaker_identifier_transcription_pipeline):
+    def test_speaker_identifier_transcription_pipeline(
+        self, speaker_identifier_transcription_pipeline
+    ):
         result = speaker_identifier_transcription_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
+        _validate_multimodal(
+            result,
             check_video_annotation=False,
             check_voice_features=False,
-            check_sentiment=False
+            check_sentiment=False,
         )
 
-
-    def test_speaker_identifier_transcription_sentiment_pipeline(self, speaker_identifier_transcription_sentiment_pipeline):
+    def test_speaker_identifier_transcription_sentiment_pipeline(
+        self, speaker_identifier_transcription_sentiment_pipeline
+    ):
         result = speaker_identifier_transcription_sentiment_pipeline.apply(
             self.filepath,
-            keep_audiofile=True # Otherwise test audio file is removed
+            keep_audiofile=True,  # Otherwise test audio file is removed
         )
 
-        _validate_multimodal(result,
-            check_video_annotation=False,
-            check_voice_features=False
+        _validate_multimodal(
+            result, check_video_annotation=False, check_voice_features=False
         )
```

### Comparing `mexca-0.4.0/tests/test_text_sentiment.py` & `mexca-0.5.0/tests/test_text_sentiment.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,75 +1,80 @@
 """ Test audio sentiment extraction classes and methods """
 
 import os
 import subprocess
+
 import pytest
 from intervaltree import Interval, IntervalTree
 from transformers import XLMRobertaForSequenceClassification
-from mexca.data import AudioTranscription, SentimentData, SentimentAnnotation, TranscriptionData
+
+from mexca.data import (
+    AudioTranscription,
+    SentimentAnnotation,
+    SentimentData,
+    TranscriptionData,
+)
 from mexca.text import SentimentExtractor
 
 
 # Skip tests on GitHub actions runner for Windows and Linux but
 # allow local runs
-@pytest.mark.skip_env('runner')
-@pytest.mark.skip_os(['Windows', 'Linux'])
+@pytest.mark.skip_env("runner")
+@pytest.mark.skip_os(["Windows", "Linux"])
 class TestSentimentExtractor:
     transcription_path = os.path.join(
-        'tests', 'reference_files', 'test_video_audio_5_seconds_transcription.srt'
+        "tests",
+        "reference_files",
+        "test_video_audio_5_seconds_transcription.srt",
     )
-    reference = {
-        'pos': 0.9203513,
-        'neg': 0.01545323,
-        'neu': 0.06419527
-    }
-
+    reference = {"pos": 0.9203513, "neg": 0.01545323, "neu": 0.06419527}
 
     @pytest.fixture
     def extractor(self):
         return SentimentExtractor()
 
-
     @pytest.fixture
     def transcription(self):
         transcription = AudioTranscription(
             filename=self.transcription_path,
-            subtitles=IntervalTree([
-                Interval(
-                    begin=0,
-                    end=1,
-                    data=TranscriptionData(
-                        index=0,
-                        text='Today was a good day!',
-                        speaker='0'
+            subtitles=IntervalTree(
+                [
+                    Interval(
+                        begin=0,
+                        end=1,
+                        data=TranscriptionData(
+                            index=0, text="Today was a good day!", speaker="0"
+                        ),
                     )
-                )
-            ])
+                ]
+            ),
         )
 
         return transcription
 
-
     def test_lazy_init(self, extractor):
         assert not extractor._classifier
-        assert isinstance(extractor.classifier, XLMRobertaForSequenceClassification)
+        assert isinstance(
+            extractor.classifier, XLMRobertaForSequenceClassification
+        )
         del extractor.classifier
         assert not extractor._classifier
 
-
     def test_apply(self, extractor, transcription):
         sentiment = extractor.apply(transcription)
         # Get first sentence object from first segment
         assert isinstance(sentiment, SentimentAnnotation)
-        
+
         for sent in sentiment.items():
             assert isinstance(sent.data, SentimentData)
-            assert pytest.approx(sent.data.pos) == self.reference['pos']
-            assert pytest.approx(sent.data.neg) == self.reference['neg']
-            assert pytest.approx(sent.data.neu) == self.reference['neu']
-
+            assert pytest.approx(sent.data.pos) == self.reference["pos"]
+            assert pytest.approx(sent.data.neg) == self.reference["neg"]
+            assert pytest.approx(sent.data.neu) == self.reference["neu"]
 
     def test_cli(self):
-        out_filename = 'test_video_audio_5_seconds_sentiment.json'
-        subprocess.run(['extract-sentiment', '-t', self.transcription_path, '-o', '.'], check=True)
+        out_filename = "test_video_audio_5_seconds_sentiment.json"
+        subprocess.run(
+            ["extract-sentiment", "-t", self.transcription_path, "-o", "."],
+            check=True,
+        )
         assert os.path.exists(out_filename)
         os.remove(out_filename)
```

### Comparing `mexca-0.4.0/tests/test_text_transcription.py` & `mexca-0.5.0/tests/test_text_transcription.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,94 +1,90 @@
 """ Test Audio to text transcription classes and methods """
 
 import os
 import subprocess
 from datetime import timedelta
+
 import pytest
 import srt
-import stable_whisper
 import whisper
+
 from mexca.data import AudioTranscription, SpeakerAnnotation, TranscriptionData
 from mexca.text import AudioTranscriber
 
 
 class TestAudioTranscription:
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.wav'
+        "tests", "test_files", "test_video_audio_5_seconds.wav"
     )
     annotation_path = os.path.join(
-        'tests', 'reference_files', 'test_video_audio_5_seconds_audio_annotation.rttm'
+        "tests",
+        "reference_files",
+        "test_video_audio_5_seconds_audio_annotation.rttm",
     )
-    
+
     annotation = SpeakerAnnotation.from_rttm(annotation_path)
 
-    
     @pytest.fixture
     def audio_transcriber(self):
-        return AudioTranscriber(whisper_model='tiny')
-
+        return AudioTranscriber(whisper_model="tiny")
 
     def test_lazy_init(self, audio_transcriber):
         assert not audio_transcriber._transcriber
         assert isinstance(audio_transcriber.transcriber, whisper.Whisper)
         del audio_transcriber.transcriber
         assert not audio_transcriber._transcriber
 
-
     def test_apply(self, audio_transcriber):
         transcription = audio_transcriber.apply(self.filepath, self.annotation)
 
         assert isinstance(transcription, AudioTranscription)
         # Only one segment
         for seg in transcription.subtitles.items():
             assert isinstance(seg.data, TranscriptionData)
             assert isinstance(seg.begin, float)
             assert 5.0 >= seg.begin >= 0.0
             assert isinstance(seg.end, float)
             assert 5.0 >= seg.end >= 0.0
             assert isinstance(seg.data.text, str)
 
-
     def test_cli(self):
-        out_filename = os.path.splitext(os.path.basename(self.filepath))[0] + '_transcription.srt'
-        subprocess.run(['transcribe', '-f', self.filepath,
-                        '-a', self.annotation_path, '-o', '.'], check=True)
+        out_filename = (
+            os.path.splitext(os.path.basename(self.filepath))[0]
+            + "_transcription.srt"
+        )
+        subprocess.run(
+            [
+                "transcribe",
+                "-f",
+                self.filepath,
+                "-a",
+                self.annotation_path,
+                "-o",
+                ".",
+            ],
+            check=True,
+        )
         assert os.path.exists(out_filename)
         os.remove(out_filename)
 
 
 class TestWhisper:
-    model_size = 'tiny'
+    model_size = "tiny"
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.wav'
+        "tests", "test_files", "test_video_audio_5_seconds.wav"
     )
 
-
     @pytest.fixture
     def model(self):
         return whisper.load_model(self.model_size)
 
-
     @pytest.fixture
     def stable_model(self):
-        return stable_whisper.load_model(self.model_size)
-
+        return whisper.load_model(self.model_size)
 
     def test_transcribe(self, model):
         output = model.transcribe(self.filepath, fp16=False)
 
         # Test entire text of audio and language detection
-        assert isinstance(output['text'].strip(), str)
-        assert isinstance(output['language'], str)
-
-
-    def test_word_ts(self, stable_model):
-        output = stable_model.transcribe(self.filepath, fp16=False)
-        # Test word level timestamps of first segment
-        first_segment = output['segments'][0]
-
-        assert 'whole_word_timestamps' in first_segment
-
-        first_segment_ts = output['segments'][0]['whole_word_timestamps']
-        # Test first token of first segment
-        assert isinstance(first_segment_ts[0]['word'], str)
-        assert isinstance(first_segment_ts[0]['timestamp'], float)
+        assert isinstance(output["text"].strip(), str)
+        assert isinstance(output["language"], str)
```

### Comparing `mexca-0.4.0/tests/test_video.py` & `mexca-0.5.0/tests/test_video_extraction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,255 +1,256 @@
 """Test facial feature extraction class and methods.
 """
 
 import json
 import os
 import subprocess
+
 import numpy as np
 import pytest
 import torch
 from facenet_pytorch import MTCNN, InceptionResnetV1
-from feat.detector import Detector
 from spectralcluster import SpectralClusterer
 from torch.utils.data import DataLoader
-from mexca.video import FaceExtractor, NotEnoughFacesError, VideoAnnotation, VideoDataset
+
+from mexca.data import VideoAnnotation
+from mexca.video.extraction import (
+    FaceExtractor,
+    NotEnoughFacesError,
+    VideoDataset,
+)
+from mexca.video.mefarg import MEFARG
 
 
 class TestVideoDataset:
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.mp4'
+        "tests", "test_files", "test_video_audio_5_seconds.mp4"
     )
 
-
     @pytest.fixture
     def video_dataset(self):
         return VideoDataset(self.filepath)
 
-        
     def test_duration(self, video_dataset):
         assert isinstance(video_dataset.duration, float)
 
-
     def test_len(self, video_dataset):
         assert isinstance(len(video_dataset), int)
 
-
     def test_getitem(self, video_dataset):
         item = video_dataset[0]
         assert isinstance(item, dict)
-        assert isinstance(item['Image'], torch.Tensor)
-        assert item['Frame'] == 0
-        assert len(item['Image'].shape) == 3
-
+        assert isinstance(item["Image"], torch.Tensor)
+        assert item["Frame"] == 0
+        assert len(item["Image"].shape) == 3
 
     def test_getitem_slice(self, video_dataset):
         item = video_dataset[0:1]
         assert isinstance(item, dict)
-        assert isinstance(item['Image'], torch.Tensor)
-        assert item['Frame'].shape[0] == 1
-        assert len(item['Image'].shape) == 4
+        assert isinstance(item["Image"], torch.Tensor)
+        assert item["Frame"].shape[0] == 1
+        assert len(item["Image"].shape) == 4
 
 
 class TestFaceExtractor:
     filepath = os.path.join(
-        'tests', 'test_files', 'test_video_audio_5_seconds.mp4'
+        "tests", "test_files", "test_video_audio_5_seconds.mp4"
     )
-    with open(os.path.join(
-            'tests', 'reference_files', 'face_features_video_audio_5_seconds.json'
-        ), 'r', encoding="utf-8") as file:
+    with open(
+        os.path.join(
+            "tests",
+            "reference_files",
+            "test_video_audio_5_seconds_video_annotation.json",
+        ),
+        "r",
+        encoding="utf-8",
+    ) as file:
         features = json.loads(file.read())
     dataset = VideoDataset(filepath, skip_frames=5)
     data_loader = DataLoader(dataset, batch_size=5)
 
-
     @pytest.fixture
     def extractor(self):
         return FaceExtractor(num_faces=4)
 
-
     @staticmethod
     def check_private_attrs(extractor):
         assert not extractor._detector
         assert not extractor._encoder
         assert not extractor._clusterer
         assert not extractor._extractor
 
-
     def test_lazy_init(self, extractor):
         self.check_private_attrs(extractor)
 
         assert isinstance(extractor.detector, MTCNN)
         assert isinstance(extractor.encoder, InceptionResnetV1)
         assert isinstance(extractor.clusterer, SpectralClusterer)
-        assert isinstance(extractor.extractor, Detector)
+        assert isinstance(extractor.extractor, MEFARG)
 
         del extractor.detector
         del extractor.encoder
         del extractor.clusterer
         del extractor.extractor
 
         # Check again after deletion
         self.check_private_attrs(extractor)
 
-
     def test_detect_face(self, extractor):
-        _, boxes, probs = extractor.detect(self.dataset[5]['Image'])
-        assert boxes.shape[1] == probs.shape[0]
-        assert boxes.shape[2] == 4
-        assert probs.shape[1] == 1
-
+        _, boxes, probs, lmks = extractor.detect(self.dataset[5]["Image"])
+        assert boxes.shape == (1, 1, 4)
+        assert probs.shape == (1, 1)
+        assert lmks.shape == (1, 1, 5, 2)
 
     def test_detect_no_face(self, extractor):
-        _, boxes, probs = extractor.detect(self.dataset[0]['Image'])
+        _, boxes, probs, lmks = extractor.detect(self.dataset[0]["Image"])
         assert boxes == np.array([None])
         assert probs == np.array([None])
-
+        assert lmks == np.array([None])
 
     def test_encode(self, extractor):
-        faces, _, _ = extractor.detect(self.dataset[5]['Image'])
+        faces, _, _, _ = extractor.detect(self.dataset[5]["Image"])
         embeddings = extractor.encode(faces[0])
         assert embeddings.shape == (1, 512)
 
-
     def test_identify(self, extractor):
         n_samples = 10
         embeddings = np.random.uniform(0, 1, size=(n_samples, 512))
         labels = extractor.identify(embeddings)
         assert labels.shape == (n_samples,)
 
-
     def test_identify_with_nan(self, extractor):
         n_samples = 10
         embeddings = np.random.uniform(0, 1, size=(n_samples, 512))
         embeddings[8, :] = np.nan
         labels = extractor.identify(embeddings)
         assert labels.shape == (n_samples,)
 
-
     def test_identify_not_enough_faces(self, extractor):
         n_samples = 10
         embeddings = np.random.uniform(0, 1, size=(n_samples, 512))
-        
+
         with pytest.raises(NotEnoughFacesError):
             extractor.identify(embeddings[0:3])
 
         # When embeddings are not valid
         embeddings[:7, :] = np.nan
 
         with pytest.raises(NotEnoughFacesError):
             extractor.identify(embeddings)
 
-
-    def test_extract_xgb_mobilefacenet(self, extractor):
-        image = self.dataset[5:6]['Image']
-        _, boxes, _ = extractor.detect(image)
-        landmarks, aus = extractor.extract(image, boxes)
-        assert isinstance(landmarks, list)
-        assert isinstance(aus, list)
-        assert np.array(landmarks).shape[2:4] == (68, 2)
-        assert np.array(aus).shape[2] == 20
-
-
-    def test_extract_svm_mobilenet(self):
-        extractor = FaceExtractor(num_faces=4, au_model='svm', landmark_model='mobilenet')
-        image = self.dataset[5:6]['Image']
-        _, boxes, _ = extractor.detect(image)
-        landmarks, aus = extractor.extract(image, boxes)
-        assert isinstance(landmarks, list)
-        assert isinstance(aus, list)
-        assert np.array(landmarks).shape[2:4] == (68, 2)
-        assert np.array(aus).shape[2] == 20
-
-
-    def test_extract_xgb_pfld(self):
-        extractor = FaceExtractor(num_faces=4, au_model='xgb', landmark_model='pfld')
-        image = self.dataset[5:6]['Image']
-        _, boxes, _ = extractor.detect(image)
-        landmarks, aus = extractor.extract(image, boxes)
-        assert isinstance(landmarks, list)
-        assert isinstance(aus, list)
-        assert np.array(landmarks).shape[2:4] == (68, 2)
-        assert np.array(aus).shape[2] == 20
-
+    def test_extract(self, extractor):
+        image = self.dataset[5:6]["Image"]
+        faces, _, _, _ = extractor.detect(image)
+        aus = extractor.extract(faces)
+        assert isinstance(aus, np.ndarray)
+        assert np.array(aus).shape == (1, 1, 41)
 
     def test_extract_no_face(self, extractor):
-        image = self.dataset[0:1]['Image']
-        _, boxes, _ = extractor.detect(image)
-        landmarks, aus = extractor.extract(image, boxes)
-        assert isinstance(landmarks, list)
-        assert isinstance(aus, list)
-        assert np.array(landmarks) == np.array([None])
+        image = self.dataset[0:1]["Image"]
+        faces, _, _, _ = extractor.detect(image)
+        aus = extractor.extract(faces)
+        assert isinstance(aus, np.ndarray)
         assert np.array(aus) == np.array([None])
 
-
     def test_compute_centroids(self, extractor):
         # create two array embeddings
         v1 = np.random.uniform(size=10)
         v2 = np.random.uniform(size=10)
 
         embeddings = np.vstack([v1, v1, v2, -v2])
 
         labels = np.asarray([0, 0, 1, 1])
-        centroids, cluster_label_mapping = extractor._compute_centroids(embeddings, labels)
+        centroids, cluster_label_mapping = extractor._compute_centroids(
+            embeddings, labels
+        )
         # test whether we got two unique labels
         assert len(centroids) == 2
         # the centroid of two arrays that are equal (i.e., v1) is equal to both of them
         assert all(centroids[0] == v1)
         # the centroid of two arrays that are opposite, is equal as all elements equal to 0
         assert all(centroids[1] == 0)
         # centroids must be a list
         assert isinstance(centroids, list)
         # cluster_label_mapping must be a dict
         assert isinstance(cluster_label_mapping, dict)
 
-
     def test_compute_confidence(self, extractor):
         # create two array embeddings
         v1 = np.random.uniform(low=-1, high=1, size=10)
         v2 = np.random.uniform(low=-1, high=1, size=10)
-        v3 = (v2 + 1. * v1) / 2.
+        v3 = (v2 + 1.0 * v1) / 2.0
 
         embeddings = np.vstack([v1, v1, v2, v3])
 
-        labels = [0., 0., 1., 1.]
+        labels = [0.0, 0.0, 1.0, 1.0]
         confidence = extractor.compute_confidence(embeddings, labels)
 
         # assert isistance confidence np.array
         assert len(confidence) == len(labels)
 
         # I expect first two instances to be equal to 1 as they are both V1
         assert np.isclose(confidence[0], 1)
         assert np.isclose(confidence[1], 1)
 
         # I expect both V2 and V3 to be less than 1, no particular value
-        assert confidence[2] < 1.
-        assert confidence[3] < 1.
+        assert confidence[2] < 1.0
+        assert confidence[3] < 1.0
 
         # I expect confidence of V3 to be less than V2, as this is more close to V1 than V2
         assert confidence[3] < confidence[2]
 
-
     def test_apply(self, extractor):
-        features = extractor.apply(self.filepath, batch_size=5, skip_frames=5, show_progress=False)
+        features = extractor.apply(
+            self.filepath, batch_size=5, skip_frames=5, show_progress=False
+        )
         assert isinstance(features, VideoAnnotation)
 
-        assert features.frame == self.features['frame']
-        assert features.time == self.features['time']
+        assert features.frame == self.features["frame"]
+        assert features.time == self.features["time"]
 
-        for attr in ['frame', 'time', 'face_box', 'face_prob', 'face_label', 'face_landmarks', 'face_aus']:
+        for attr in [
+            "frame",
+            "time",
+            "face_box",
+            "face_prob",
+            "face_label",
+            "face_landmarks",
+            "face_aus",
+        ]:
             assert len(getattr(features, attr)) == len(self.features[attr])
             assert len(getattr(features, attr)) == len(features.frame)
 
-
     def test_apply_no_face_batch(self, extractor):
-        features = extractor.apply(self.filepath, batch_size=1, skip_frames=5, process_subclip=(0, 2), show_progress=False)
+        features = extractor.apply(
+            self.filepath,
+            batch_size=1,
+            skip_frames=5,
+            process_subclip=(0, 2),
+            show_progress=False,
+        )
         assert isinstance(features, VideoAnnotation)
         assert np.isnan(features.face_prob[0])
 
-
     def test_cli(self):
-        out_filename = os.path.splitext(os.path.basename(self.filepath))[0] + '_video_annotation.json'
-        subprocess.run(['extract-faces', '-f', self.filepath,
-                        '-o', '.', '--num-faces', '4', '--batch-size', '5',
-                        '--skip-frames', '5'], check=True)
+        out_filename = (
+            os.path.splitext(os.path.basename(self.filepath))[0]
+            + "_video_annotation.json"
+        )
+        subprocess.run(
+            [
+                "extract-faces",
+                "-f",
+                self.filepath,
+                "-o",
+                ".",
+                "--num-faces",
+                "4",
+                "--batch-size",
+                "5",
+                "--skip-frames",
+                "5",
+            ],
+            check=True,
+        )
         assert os.path.exists(out_filename)
-        os.remove(out_filename)
+        os.remove(out_filename)
```

