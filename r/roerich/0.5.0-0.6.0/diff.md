# Comparing `tmp/roerich-0.5.0.tar.gz` & `tmp/roerich-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roerich-0.5.0.tar", last modified: Fri Jun 16 08:34:12 2023, max compression
+gzip compressed data, was "roerich-0.6.0.tar", last modified: Mon Jul 17 10:48:12 2023, max compression
```

## Comparing `roerich-0.5.0.tar` & `roerich-0.6.0.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.301514 roerich-0.5.0/
--rw-r--r--   0 mihailh    (501) staff       (20)     1354 2023-06-14 05:42:56.000000 roerich-0.5.0/LICENSE
--rw-r--r--   0 mihailh    (501) staff       (20)     5657 2023-06-16 08:34:12.301667 roerich-0.5.0/PKG-INFO
--rw-r--r--   0 mihailh    (501) staff       (20)     4690 2023-06-14 10:13:13.000000 roerich-0.5.0/README.md
--rw-r--r--   0 mihailh    (501) staff       (20)       81 2023-06-14 05:42:56.000000 roerich-0.5.0/pyproject.toml
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.295861 roerich-0.5.0/roerich/
--rw-r--r--   0 mihailh    (501) staff       (20)      113 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/__init__.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299040 roerich-0.5.0/roerich/algorithms/
--rw-r--r--   0 mihailh    (501) staff       (20)      794 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/algorithms/__init__.py
--rw-r--r--   0 mihailh    (501) staff       (20)    11022 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/algorithms/algorithms.py
--rw-r--r--   0 mihailh    (501) staff       (20)    13471 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/algorithms/cpdc.py
--rw-r--r--   0 mihailh    (501) staff       (20)     4188 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/cpdc_cv.py
--rw-r--r--   0 mihailh    (501) staff       (20)     1317 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/enrg_dist.py
--rw-r--r--   0 mihailh    (501) staff       (20)     4283 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/algorithms/matrix.py
--rw-r--r--   0 mihailh    (501) staff       (20)    12869 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/models.py
--rw-r--r--   0 mihailh    (501) staff       (20)      832 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/net.py
--rw-r--r--   0 mihailh    (501) staff       (20)     2416 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/algorithms/scaler.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299256 roerich-0.5.0/roerich/change_point/
--rw-r--r--   0 mihailh    (501) staff       (20)      499 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/change_point/__init__.py
--rw-r--r--   0 mihailh    (501) staff       (20)      497 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/dataset.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299449 roerich-0.5.0/roerich/density_ratio/
--rw-r--r--   0 mihailh    (501) staff       (20)      175 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/density_ratio/__init__.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.299651 roerich-0.5.0/roerich/explanation/
--rw-r--r--   0 mihailh    (501) staff       (20)       91 2023-06-16 07:52:18.000000 roerich-0.5.0/roerich/explanation/__init__.py
--rw-r--r--   0 mihailh    (501) staff       (20)     2797 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/helper.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.300267 roerich-0.5.0/roerich/metrics/
--rw-r--r--   0 mihailh    (501) staff       (20)      437 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/metrics/__init__.py
--rw-r--r--   0 mihailh    (501) staff       (20)     2896 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/metrics/metrics.py
--rw-r--r--   0 mihailh    (501) staff       (20)     7398 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/metrics/pr.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.300450 roerich-0.5.0/roerich/networks/
--rw-r--r--   0 mihailh    (501) staff       (20)      258 2023-06-14 13:22:43.000000 roerich-0.5.0/roerich/networks/__init__.py
--rw-r--r--   0 mihailh    (501) staff       (20)     1150 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/utils.py
--rw-r--r--   0 mihailh    (501) staff       (20)     1963 2023-06-14 05:42:56.000000 roerich-0.5.0/roerich/viz.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.296790 roerich-0.5.0/roerich.egg-info/
--rw-r--r--   0 mihailh    (501) staff       (20)     5657 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/PKG-INFO
--rw-r--r--   0 mihailh    (501) staff       (20)      891 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/SOURCES.txt
--rw-r--r--   0 mihailh    (501) staff       (20)        1 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/dependency_links.txt
--rw-r--r--   0 mihailh    (501) staff       (20)      146 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/requires.txt
--rw-r--r--   0 mihailh    (501) staff       (20)        8 2023-06-16 08:34:12.000000 roerich-0.5.0/roerich.egg-info/top_level.txt
--rw-r--r--   0 mihailh    (501) staff       (20)     1240 2023-06-16 08:34:12.302125 roerich-0.5.0/setup.cfg
--rw-r--r--   0 mihailh    (501) staff       (20)       93 2023-06-14 05:42:56.000000 roerich-0.5.0/setup.py
-drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-06-16 08:34:12.301362 roerich-0.5.0/tests/
--rw-r--r--   0 mihailh    (501) staff       (20)      502 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_change_point.py
--rw-r--r--   0 mihailh    (501) staff       (20)      641 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_density_ratio.py
--rw-r--r--   0 mihailh    (501) staff       (20)      686 2023-06-16 07:52:18.000000 roerich-0.5.0/tests/test_explanation.py
--rw-r--r--   0 mihailh    (501) staff       (20)      883 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_metrics.py
--rw-r--r--   0 mihailh    (501) staff       (20)      452 2023-06-14 13:22:43.000000 roerich-0.5.0/tests/test_networks.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.268629 roerich-0.6.0/
+-rw-r--r--   0 mihailh    (501) staff       (20)     1354 2023-06-14 05:42:56.000000 roerich-0.6.0/LICENSE
+-rw-r--r--   0 mihailh    (501) staff       (20)     4358 2023-07-17 10:48:12.268741 roerich-0.6.0/PKG-INFO
+-rw-r--r--   0 mihailh    (501) staff       (20)     3488 2023-07-16 17:51:21.000000 roerich-0.6.0/README.md
+-rw-r--r--   0 mihailh    (501) staff       (20)       81 2023-06-14 05:42:56.000000 roerich-0.6.0/pyproject.toml
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.263432 roerich-0.6.0/roerich/
+-rw-r--r--   0 mihailh    (501) staff       (20)      113 2023-07-12 10:13:11.000000 roerich-0.6.0/roerich/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.265529 roerich-0.6.0/roerich/algorithms/
+-rw-r--r--   0 mihailh    (501) staff       (20)      831 2023-07-13 17:22:39.000000 roerich-0.6.0/roerich/algorithms/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    19938 2023-07-16 17:51:21.000000 roerich-0.6.0/roerich/algorithms/cpdc.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     6531 2023-07-12 06:44:15.000000 roerich-0.6.0/roerich/algorithms/cpdc_cv.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1317 2023-06-14 05:42:56.000000 roerich-0.6.0/roerich/algorithms/enrg_dist.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     4283 2023-06-16 07:52:18.000000 roerich-0.6.0/roerich/algorithms/matrix.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    12869 2023-06-14 05:42:56.000000 roerich-0.6.0/roerich/algorithms/models.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      832 2023-06-14 05:42:56.000000 roerich-0.6.0/roerich/algorithms/net.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.266166 roerich-0.6.0/roerich/change_point/
+-rw-r--r--   0 mihailh    (501) staff       (20)      556 2023-07-16 17:51:21.000000 roerich-0.6.0/roerich/change_point/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    11179 2023-07-13 17:22:39.000000 roerich-0.6.0/roerich/change_point/onnc.py
+-rw-r--r--   0 mihailh    (501) staff       (20)    10135 2023-07-13 17:22:39.000000 roerich-0.6.0/roerich/change_point/onnr.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     3479 2023-07-16 17:51:21.000000 roerich-0.6.0/roerich/change_point/windows.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      497 2023-07-12 10:13:11.000000 roerich-0.6.0/roerich/dataset.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.266322 roerich-0.6.0/roerich/density_ratio/
+-rw-r--r--   0 mihailh    (501) staff       (20)      175 2023-06-14 13:22:43.000000 roerich-0.6.0/roerich/density_ratio/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.266473 roerich-0.6.0/roerich/explanation/
+-rw-r--r--   0 mihailh    (501) staff       (20)       91 2023-06-16 07:52:18.000000 roerich-0.6.0/roerich/explanation/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.266766 roerich-0.6.0/roerich/metrics/
+-rw-r--r--   0 mihailh    (501) staff       (20)      437 2023-06-14 13:22:43.000000 roerich-0.6.0/roerich/metrics/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     7398 2023-06-14 05:42:56.000000 roerich-0.6.0/roerich/metrics/pr.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.266940 roerich-0.6.0/roerich/networks/
+-rw-r--r--   0 mihailh    (501) staff       (20)      258 2023-06-14 13:22:43.000000 roerich-0.6.0/roerich/networks/__init__.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.267554 roerich-0.6.0/roerich/scores/
+-rw-r--r--   0 mihailh    (501) staff       (20)      207 2023-07-16 17:51:21.000000 roerich-0.6.0/roerich/scores/__init__.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      391 2023-07-16 17:51:21.000000 roerich-0.6.0/roerich/scores/energy.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1030 2023-06-28 16:49:28.000000 roerich-0.6.0/roerich/scores/fd.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1032 2023-06-28 16:49:28.000000 roerich-0.6.0/roerich/scores/mmd.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1963 2023-06-14 05:42:56.000000 roerich-0.6.0/roerich/viz.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.264382 roerich-0.6.0/roerich.egg-info/
+-rw-r--r--   0 mihailh    (501) staff       (20)     4358 2023-07-17 10:48:12.000000 roerich-0.6.0/roerich.egg-info/PKG-INFO
+-rw-r--r--   0 mihailh    (501) staff       (20)      973 2023-07-17 10:48:12.000000 roerich-0.6.0/roerich.egg-info/SOURCES.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)        1 2023-07-17 10:48:12.000000 roerich-0.6.0/roerich.egg-info/dependency_links.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)      146 2023-07-17 10:48:12.000000 roerich-0.6.0/roerich.egg-info/requires.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)        8 2023-07-17 10:48:12.000000 roerich-0.6.0/roerich.egg-info/top_level.txt
+-rw-r--r--   0 mihailh    (501) staff       (20)     1143 2023-07-17 10:48:12.269147 roerich-0.6.0/setup.cfg
+-rw-r--r--   0 mihailh    (501) staff       (20)       93 2023-06-14 05:42:56.000000 roerich-0.6.0/setup.py
+drwxr-xr-x   0 mihailh    (501) staff       (20)        0 2023-07-17 10:48:12.268506 roerich-0.6.0/tests/
+-rw-r--r--   0 mihailh    (501) staff       (20)     1645 2023-07-12 06:44:15.000000 roerich-0.6.0/tests/test_change_point.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      641 2023-06-14 13:22:43.000000 roerich-0.6.0/tests/test_density_ratio.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      686 2023-06-16 07:52:18.000000 roerich-0.6.0/tests/test_explanation.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      883 2023-06-14 13:22:43.000000 roerich-0.6.0/tests/test_metrics.py
+-rw-r--r--   0 mihailh    (501) staff       (20)      452 2023-06-14 13:22:43.000000 roerich-0.6.0/tests/test_networks.py
+-rw-r--r--   0 mihailh    (501) staff       (20)     1115 2023-06-28 16:49:28.000000 roerich-0.6.0/tests/test_scores.py
```

### Comparing `roerich-0.5.0/LICENSE` & `roerich-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/PKG-INFO` & `roerich-0.6.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: roerich
-Version: 0.5.0
-Summary: Roerich is a python library for online and offline change point detection in time series data based on machine learning.
+Version: 0.6.0
+Summary: Change point detection.
 Home-page: https://github.com/HSE-LAMBDA/roerich
 Author: Mikhail Hushchyn, Kenenbek Arzymatov
 Author-email: hushchyn.mikhail@gmail.com, kenenbek@gmail.com
 License: BSD-2-Clause
 Project-URL: Documentation, https://hse-lambda.github.io/roerich/
 Project-URL: Source, https://github.com/HSE-LAMBDA/roerich/
 Keywords: python,machine learning,neural networks,signal processing,segmentation,time series analysis,anomaly detection,change point detection,density ratio
@@ -51,21 +51,23 @@
 
 (See more examples in the [documentation](https://hse-lambda.github.io/roerich).)
 
 The following code snippet generates a noisy synthetic data, performs change point detection, and displays the results. If you use own dataset, make
 sure that it has a shape `(seq_len, n_dims)`.
 ```python
 import roerich
-from roerich.algorithms import ChangePointDetectionClassifier
+from roerich.change_point import ChangePointDetectionClassifier
 
 # generate time series
 X, cps_true = roerich.generate_dataset(period=200, N_tot=2000)
 
 # detection
-cpd = ChangePointDetectionClassifier()
+# base_classifier = 'logreg', 'qda', 'dt', 'rf', 'mlp', 'knn', 'nb'
+# metric = 'klsym', 'pesym', 'jsd', 'mmd', 'fd'
+cpd = ChangePointDetectionClassifier(base_classifier='mlp', metric='klsym', window_size=100)
 score, cps_pred = cpd.predict(X)
 
 # visualization
 roerich.display(X, cps_true, score, cps_pred)
 ```
 
 ![](https://raw.githubusercontent.com/HSE-LAMBDA/roerich/main/images/demo.png)
@@ -85,36 +87,7 @@
 
 ## Thanks to all our contributors
 
 <a href="https://github.com/HSE-LAMBDA/roerich/graphs/contributors">
   <img src="https://contributors-img.web.app/image?repo=HSE-LAMBDA/roerich" />
 </a>
 
-## License
-
-```
-BSD 2-Clause License
-
-Copyright (c) 2020 Laboratory of methods for Big Data Analysis at HSE
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-* Redistributions of source code must retain the above copyright notice, this
-  list of conditions and the following disclaimer.
-
-* Redistributions in binary form must reproduce the above copyright notice,
-  this list of conditions and the following disclaimer in the documentation
-  and/or other materials provided with the distribution.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-```
```

### Comparing `roerich-0.5.0/README.md` & `roerich-0.6.0/roerich.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,294 +1,273 @@
-00000000: 2320 5765 6c63 6f6d 6520 746f 2052 6f65  # Welcome to Roe
-00000010: 7269 6368 0a0a 5b21 5b50 7950 4920 7665  rich..[![PyPI ve
-00000020: 7273 696f 6e5d 2868 7474 7073 3a2f 2f62  rsion](https://b
-00000030: 6164 6765 2e66 7572 792e 696f 2f70 792f  adge.fury.io/py/
-00000040: 726f 6572 6963 682e 7376 6729 5d28 6874  roerich.svg)](ht
-00000050: 7470 733a 2f2f 6261 6467 652e 6675 7279  tps://badge.fury
-00000060: 2e69 6f2f 7079 2f72 6f65 7269 6368 290a  .io/py/roerich).
-00000070: 5b21 5b44 6f63 756d 656e 7461 7469 6f6e  [![Documentation
-00000080: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000090: 6965 6c64 732e 696f 2f62 6164 6765 2f64  ields.io/badge/d
-000000a0: 6f63 756d 656e 7461 7469 6f6e 2d79 6573  ocumentation-yes
-000000b0: 2d67 7265 656e 2e73 7667 295d 2868 7474  -green.svg)](htt
-000000c0: 7073 3a2f 2f68 7365 2d6c 616d 6264 612e  ps://hse-lambda.
-000000d0: 6769 7468 7562 2e69 6f2f 726f 6572 6963  github.io/roeric
-000000e0: 6829 0a5b 215b 446f 776e 6c6f 6164 735d  h).[![Downloads]
-000000f0: 2868 7474 7073 3a2f 2f70 6570 792e 7465  (https://pepy.te
-00000100: 6368 2f62 6164 6765 2f72 6f65 7269 6368  ch/badge/roerich
-00000110: 295d 2868 7474 7073 3a2f 2f70 6570 792e  )](https://pepy.
-00000120: 7465 6368 2f70 726f 6a65 6374 2f72 6f65  tech/project/roe
-00000130: 7269 6368 290a 5b21 5b4c 6963 656e 7365  rich).[![License
-00000140: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
-00000150: 6965 6c64 732e 696f 2f62 6164 6765 2f4c  ields.io/badge/L
-00000160: 6963 656e 7365 2d42 5344 5f32 2d2d 436c  icense-BSD_2--Cl
-00000170: 6175 7365 2d6f 7261 6e67 652e 7376 6729  ause-orange.svg)
-00000180: 5d28 6874 7470 733a 2f2f 6f70 656e 736f  ](https://openso
-00000190: 7572 6365 2e6f 7267 2f6c 6963 656e 7365  urce.org/license
-000001a0: 732f 4253 442d 322d 436c 6175 7365 290a  s/BSD-2-Clause).
-000001b0: 0a60 526f 6572 6963 6860 2069 7320 6120  .`Roerich` is a 
-000001c0: 7079 7468 6f6e 206c 6962 7261 7279 2066  python library f
-000001d0: 6f72 206f 6e6c 696e 6520 616e 6420 6f66  or online and of
-000001e0: 666c 696e 6520 6368 616e 6765 2070 6f69  fline change poi
-000001f0: 6e74 2064 6574 6563 7469 6f6e 2066 6f72  nt detection for
-00000200: 2074 696d 6520 7365 7269 6573 2061 6e61   time series ana
-00000210: 6c79 7369 732c 2073 6967 6e61 6c20 7072  lysis, signal pr
-00000220: 6f63 6573 7369 6e67 2c20 616e 6420 7365  ocessing, and se
-00000230: 676d 656e 7461 7469 6f6e 2e20 4974 2077  gmentation. It w
-00000240: 6173 206e 616d 6564 2061 6674 6572 2074  as named after t
-00000250: 6865 2070 6169 6e74 6572 204e 6963 686f  he painter Nicho
-00000260: 6c61 7320 526f 6572 6963 682c 206b 6e6f  las Roerich, kno
-00000270: 776e 2061 7320 7468 6520 4d61 7374 6572  wn as the Master
-00000280: 206f 6620 7468 6520 4d6f 756e 7461 696e   of the Mountain
-00000290: 732e 2052 6561 6420 6d6f 7265 2061 743a  s. Read more at:
-000002a0: 2068 7474 7073 3a2f 2f77 7777 2e72 6f65   https://www.roe
-000002b0: 7269 6368 2e6f 7267 2e0a 0a21 5b5d 2868  rich.org...![](h
-000002c0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000002d0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000002e0: 2f48 5345 2d4c 414d 4244 412f 726f 6572  /HSE-LAMBDA/roer
-000002f0: 6963 682f 6d61 696e 2f69 6d61 6765 732f  ich/main/images/
-00000300: 3730 3031 3235 7631 2e6a 7065 6729 0a5f  700125v1.jpeg)._
-00000310: 4672 6167 6d65 6e74 206f 6620 2248 696d  Fragment of "Him
-00000320: 616c 6179 6173 222c 2031 3933 335f 0a0a  alayas", 1933_..
-00000330: 4375 7272 656e 746c 792c 2074 6865 206c  Currently, the l
-00000340: 6962 7261 7279 2063 6f6e 7461 696e 7320  ibrary contains 
-00000350: 6f66 6669 6369 616c 2069 6d70 6c65 6d65  official impleme
-00000360: 6e74 6174 696f 6e73 206f 6620 6368 616e  ntations of chan
-00000370: 6765 2070 6f69 6e74 2064 6574 6563 7469  ge point detecti
-00000380: 6f6e 2061 6c67 6f72 6974 686d 7320 6261  on algorithms ba
-00000390: 7365 6420 6f6e 2064 6972 6563 7420 6465  sed on direct de
-000003a0: 6e73 6974 7920 7261 7469 6f20 6573 7469  nsity ratio esti
-000003b0: 6d61 7469 6f6e 2066 726f 6d20 7468 6520  mation from the 
-000003c0: 666f 6c6c 6f77 696e 6720 6172 7469 636c  following articl
-000003d0: 6573 3a0a 0a2d 204d 696b 6861 696c 2048  es:..- Mikhail H
-000003e0: 7573 6863 6879 6e20 616e 6420 416e 6472  ushchyn and Andr
-000003f0: 6579 2055 7374 7975 7a68 616e 696e 2e20  ey Ustyuzhanin. 
-00000400: e280 9c47 656e 6572 616c 697a 6174 696f  ...Generalizatio
-00000410: 6e20 6f66 2043 6861 6e67 652d 506f 696e  n of Change-Poin
-00000420: 7420 4465 7465 6374 696f 6e20 696e 2054  t Detection in T
-00000430: 696d 6520 5365 7269 6573 2044 6174 6120  ime Series Data 
-00000440: 4261 7365 6420 6f6e 2044 6972 6563 7420  Based on Direct 
-00000450: 4465 6e73 6974 7920 5261 7469 6f20 4573  Density Ratio Es
-00000460: 7469 6d61 7469 6f6e 2ee2 809d 204a 2e20  timation.... J. 
-00000470: 436f 6d70 7574 2e20 5363 692e 2035 3320  Comput. Sci. 53 
-00000480: 2832 3032 3129 3a20 3130 3133 3835 2e20  (2021): 101385. 
-00000490: 5b5b 6a6f 7572 6e61 6c5d 5d28 6874 7470  [[journal]](http
-000004a0: 733a 2f2f 646f 692e 6f72 672f 3130 2e31  s://doi.org/10.1
-000004b0: 3031 362f 6a2e 6a6f 6373 2e32 3032 312e  016/j.jocs.2021.
-000004c0: 3130 3133 3835 2920 5b5b 6172 7869 765d  101385) [[arxiv]
-000004d0: 5d28 6874 7470 733a 2f2f 646f 692e 6f72  ](https://doi.or
-000004e0: 672f 3130 2e34 3835 3530 2f61 7258 6976  g/10.48550/arXiv
-000004f0: 2e32 3030 312e 3036 3338 3629 0a2d 204d  .2001.06386).- M
-00000500: 696b 6861 696c 2048 7573 6863 6879 6e2c  ikhail Hushchyn,
-00000510: 204b 656e 656e 6265 6b20 4172 7a79 6d61   Kenenbek Arzyma
-00000520: 746f 7620 616e 6420 4465 6e69 7320 4465  tov and Denis De
-00000530: 726b 6163 682e 20e2 809c 4f6e 6c69 6e65  rkach. ...Online
-00000540: 204e 6575 7261 6c20 4e65 7477 6f72 6b73   Neural Networks
-00000550: 2066 6f72 2043 6861 6e67 652d 506f 696e   for Change-Poin
-00000560: 7420 4465 7465 6374 696f 6e2e e280 9d20  t Detection.... 
-00000570: 4172 5869 7620 6162 732f 3230 3130 2e30  ArXiv abs/2010.0
-00000580: 3133 3838 2028 3230 3230 292e 205b 5b61  1388 (2020). [[a
-00000590: 7278 6976 5d5d 2868 7474 7073 3a2f 2f64  rxiv]](https://d
-000005a0: 6f69 2e6f 7267 2f31 302e 3438 3535 302f  oi.org/10.48550/
-000005b0: 6172 5869 762e 3230 3130 2e30 3133 3838  arXiv.2010.01388
-000005c0: 290a 0a23 2320 4465 7065 6e64 656e 6369  )..## Dependenci
-000005d0: 6573 2061 6e64 2069 6e73 7461 6c6c 0a0a  es and install..
-000005e0: 6060 600a 7069 7020 696e 7374 616c 6c20  ```.pip install 
-000005f0: 726f 6572 6963 680a 6060 600a 6f72 0a60  roerich.```.or.`
-00000600: 6060 7079 7468 6f6e 0a67 6974 2063 6c6f  ``python.git clo
-00000610: 6e65 2068 7474 7073 3a2f 2f67 6974 6875  ne https://githu
-00000620: 622e 636f 6d2f 4853 452d 4c41 4d42 4441  b.com/HSE-LAMBDA
-00000630: 2f72 6f65 7269 6368 2e67 6974 0a63 6420  /roerich.git.cd 
-00000640: 726f 6572 6963 680a 7069 7020 696e 7374  roerich.pip inst
-00000650: 616c 6c20 2d65 202e 0a60 6060 0a0a 2323  all -e ..```..##
-00000660: 2042 6173 6963 2075 7361 6765 0a0a 2853   Basic usage..(S
-00000670: 6565 206d 6f72 6520 6578 616d 706c 6573  ee more examples
-00000680: 2069 6e20 7468 6520 5b64 6f63 756d 656e   in the [documen
-00000690: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
-000006a0: 6873 652d 6c61 6d62 6461 2e67 6974 6875  hse-lambda.githu
-000006b0: 622e 696f 2f72 6f65 7269 6368 292e 290a  b.io/roerich).).
-000006c0: 0a54 6865 2066 6f6c 6c6f 7769 6e67 2063  .The following c
-000006d0: 6f64 6520 736e 6970 7065 7420 6765 6e65  ode snippet gene
-000006e0: 7261 7465 7320 6120 6e6f 6973 7920 7379  rates a noisy sy
-000006f0: 6e74 6865 7469 6320 6461 7461 2c20 7065  nthetic data, pe
-00000700: 7266 6f72 6d73 2063 6861 6e67 6520 706f  rforms change po
-00000710: 696e 7420 6465 7465 6374 696f 6e2c 2061  int detection, a
-00000720: 6e64 2064 6973 706c 6179 7320 7468 6520  nd displays the 
-00000730: 7265 7375 6c74 732e 2049 6620 796f 7520  results. If you 
-00000740: 7573 6520 6f77 6e20 6461 7461 7365 742c  use own dataset,
-00000750: 206d 616b 650a 7375 7265 2074 6861 7420   make.sure that 
-00000760: 6974 2068 6173 2061 2073 6861 7065 2060  it has a shape `
-00000770: 2873 6571 5f6c 656e 2c20 6e5f 6469 6d73  (seq_len, n_dims
-00000780: 2960 2e0a 6060 6070 7974 686f 6e0a 696d  )`..```python.im
-00000790: 706f 7274 2072 6f65 7269 6368 0a66 726f  port roerich.fro
-000007a0: 6d20 726f 6572 6963 682e 616c 676f 7269  m roerich.algori
-000007b0: 7468 6d73 2069 6d70 6f72 7420 4368 616e  thms import Chan
-000007c0: 6765 506f 696e 7444 6574 6563 7469 6f6e  gePointDetection
-000007d0: 436c 6173 7369 6669 6572 0a0a 2320 6765  Classifier..# ge
-000007e0: 6e65 7261 7465 2074 696d 6520 7365 7269  nerate time seri
-000007f0: 6573 0a58 2c20 6370 735f 7472 7565 203d  es.X, cps_true =
-00000800: 2072 6f65 7269 6368 2e67 656e 6572 6174   roerich.generat
-00000810: 655f 6461 7461 7365 7428 7065 7269 6f64  e_dataset(period
-00000820: 3d32 3030 2c20 4e5f 746f 743d 3230 3030  =200, N_tot=2000
-00000830: 290a 0a23 2064 6574 6563 7469 6f6e 0a63  )..# detection.c
-00000840: 7064 203d 2043 6861 6e67 6550 6f69 6e74  pd = ChangePoint
-00000850: 4465 7465 6374 696f 6e43 6c61 7373 6966  DetectionClassif
-00000860: 6965 7228 290a 7363 6f72 652c 2063 7073  ier().score, cps
-00000870: 5f70 7265 6420 3d20 6370 642e 7072 6564  _pred = cpd.pred
-00000880: 6963 7428 5829 0a0a 2320 7669 7375 616c  ict(X)..# visual
-00000890: 697a 6174 696f 6e0a 726f 6572 6963 682e  ization.roerich.
-000008a0: 6469 7370 6c61 7928 582c 2063 7073 5f74  display(X, cps_t
-000008b0: 7275 652c 2073 636f 7265 2c20 6370 735f  rue, score, cps_
-000008c0: 7072 6564 290a 6060 600a 0a21 5b5d 2868  pred).```..![](h
-000008d0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
-000008e0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
-000008f0: 2f48 5345 2d4c 414d 4244 412f 726f 6572  /HSE-LAMBDA/roer
-00000900: 6963 682f 6d61 696e 2f69 6d61 6765 732f  ich/main/images/
-00000910: 6465 6d6f 2e70 6e67 290a 0a23 2320 5375  demo.png)..## Su
-00000920: 7070 6f72 740a 0a2d 2048 6f6d 653a 205b  pport..- Home: [
-00000930: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000940: 6f6d 2f48 5345 2d4c 414d 4244 412f 726f  om/HSE-LAMBDA/ro
-00000950: 6572 6963 685d 2868 7474 7073 3a2f 2f67  erich](https://g
-00000960: 6974 6875 622e 636f 6d2f 4853 452d 4c41  ithub.com/HSE-LA
-00000970: 4d42 4441 2f72 6f65 7269 6368 290a 2d20  MBDA/roerich).- 
-00000980: 446f 6375 6d65 6e74 6174 696f 6e3a 205b  Documentation: [
-00000990: 6874 7470 733a 2f2f 6873 652d 6c61 6d62  https://hse-lamb
-000009a0: 6461 2e67 6974 6875 622e 696f 2f72 6f65  da.github.io/roe
-000009b0: 7269 6368 5d28 6874 7470 733a 2f2f 6873  rich](https://hs
-000009c0: 652d 6c61 6d62 6461 2e67 6974 6875 622e  e-lambda.github.
-000009d0: 696f 2f72 6f65 7269 6368 290a 2d20 466f  io/roerich).- Fo
-000009e0: 7220 616e 7920 7573 6167 6520 7175 6573  r any usage ques
-000009f0: 7469 6f6e 732c 2073 7567 6765 7374 696f  tions, suggestio
-00000a00: 6e73 2061 6e64 2062 7567 7320 7573 6520  ns and bugs use 
-00000a10: 7468 6520 5b69 7373 7565 2070 6167 655d  the [issue page]
-00000a20: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000a30: 636f 6d2f 4853 452d 4c41 4d42 4441 2f72  com/HSE-LAMBDA/r
-00000a40: 6f65 7269 6368 2f69 7373 7565 7329 2c20  oerich/issues), 
-00000a50: 706c 6561 7365 2e0a 0a23 2320 5265 6c61  please...## Rela
-00000a60: 7465 6420 6c69 6272 6172 6965 730a 0a5b  ted libraries..[
-00000a70: 215b 4765 6e65 7269 6320 6261 6467 655d  ![Generic badge]
-00000a80: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000a90: 656c 6473 2e69 6f2f 6261 6467 652f 5e2e  elds.io/badge/^.
-00000aa0: 5e2d 7275 7074 7572 6573 2d62 6c75 652e  ^-ruptures-blue.
-00000ab0: 7376 6729 5d28 6874 7470 733a 2f2f 6769  svg)](https://gi
-00000ac0: 7468 7562 2e63 6f6d 2f64 6565 7063 6861  thub.com/deepcha
-00000ad0: 726c 6573 2f72 7570 7475 7265 7329 0a5b  rles/ruptures).[
-00000ae0: 215b 4765 6e65 7269 6320 6261 6467 655d  ![Generic badge]
-00000af0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-00000b00: 656c 6473 2e69 6f2f 6261 6467 652f 5e2e  elds.io/badge/^.
-00000b10: 5e2d 6b6c 6370 642d 626c 7565 2e73 7667  ^-klcpd-blue.svg
-00000b20: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
-00000b30: 622e 636f 6d2f 486f 6c79 4261 7965 732f  b.com/HolyBayes/
-00000b40: 6b6c 6370 6429 0a5b 215b 4765 6e65 7269  klcpd).[![Generi
-00000b50: 6320 6261 6467 655d 2868 7474 7073 3a2f  c badge](https:/
-00000b60: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
-00000b70: 6261 6467 652f 5e2e 5e2d 7469 7265 2d62  badge/^.^-tire-b
-00000b80: 6c75 652e 7376 6729 5d28 6874 7470 733a  lue.svg)](https:
-00000b90: 2f2f 6769 7468 7562 2e63 6f6d 2f48 6f6c  //github.com/Hol
-00000ba0: 7942 6179 6573 2f54 4952 455f 7079 746f  yBayes/TIRE_pyto
-00000bb0: 7263 6829 0a5b 215b 4765 6e65 7269 6320  rch).[![Generic 
-00000bc0: 6261 6467 655d 2868 7474 7073 3a2f 2f69  badge](https://i
-00000bd0: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
-00000be0: 6467 652f 5e2e 5e2d 626f 6370 642d 626c  dge/^.^-bocpd-bl
-00000bf0: 7565 2e73 7667 295d 2868 7474 7073 3a2f  ue.svg)](https:/
-00000c00: 2f67 6974 6875 622e 636f 6d2f 6869 6c64  /github.com/hild
-00000c10: 656e 7369 612f 6261 7965 7369 616e 5f63  ensia/bayesian_c
-00000c20: 6861 6e67 6570 6f69 6e74 5f64 6574 6563  hangepoint_detec
-00000c30: 7469 6f6e 290a 0a23 2320 5468 616e 6b73  tion)..## Thanks
-00000c40: 2074 6f20 616c 6c20 6f75 7220 636f 6e74   to all our cont
-00000c50: 7269 6275 746f 7273 0a0a 3c61 2068 7265  ributors..<a hre
-00000c60: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000c70: 622e 636f 6d2f 4853 452d 4c41 4d42 4441  b.com/HSE-LAMBDA
-00000c80: 2f72 6f65 7269 6368 2f67 7261 7068 732f  /roerich/graphs/
-00000c90: 636f 6e74 7269 6275 746f 7273 223e 0a20  contributors">. 
-00000ca0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000cb0: 3a2f 2f63 6f6e 7472 6962 7574 6f72 732d  ://contributors-
-00000cc0: 696d 672e 7765 622e 6170 702f 696d 6167  img.web.app/imag
-00000cd0: 653f 7265 706f 3d48 5345 2d4c 414d 4244  e?repo=HSE-LAMBD
-00000ce0: 412f 726f 6572 6963 6822 202f 3e0a 3c2f  A/roerich" />.</
-00000cf0: 613e 0a0a 2323 204c 6963 656e 7365 0a0a  a>..## License..
-00000d00: 6060 600a 4253 4420 322d 436c 6175 7365  ```.BSD 2-Clause
-00000d10: 204c 6963 656e 7365 0a0a 436f 7079 7269   License..Copyri
-00000d20: 6768 7420 2863 2920 3230 3230 204c 6162  ght (c) 2020 Lab
-00000d30: 6f72 6174 6f72 7920 6f66 206d 6574 686f  oratory of metho
-00000d40: 6473 2066 6f72 2042 6967 2044 6174 6120  ds for Big Data 
-00000d50: 416e 616c 7973 6973 2061 7420 4853 450a  Analysis at HSE.
-00000d60: 416c 6c20 7269 6768 7473 2072 6573 6572  All rights reser
-00000d70: 7665 642e 0a0a 5265 6469 7374 7269 6275  ved...Redistribu
-00000d80: 7469 6f6e 2061 6e64 2075 7365 2069 6e20  tion and use in 
-00000d90: 736f 7572 6365 2061 6e64 2062 696e 6172  source and binar
-00000da0: 7920 666f 726d 732c 2077 6974 6820 6f72  y forms, with or
-00000db0: 2077 6974 686f 7574 0a6d 6f64 6966 6963   without.modific
-00000dc0: 6174 696f 6e2c 2061 7265 2070 6572 6d69  ation, are permi
-00000dd0: 7474 6564 2070 726f 7669 6465 6420 7468  tted provided th
-00000de0: 6174 2074 6865 2066 6f6c 6c6f 7769 6e67  at the following
-00000df0: 2063 6f6e 6469 7469 6f6e 7320 6172 6520   conditions are 
-00000e00: 6d65 743a 0a0a 2a20 5265 6469 7374 7269  met:..* Redistri
-00000e10: 6275 7469 6f6e 7320 6f66 2073 6f75 7263  butions of sourc
-00000e20: 6520 636f 6465 206d 7573 7420 7265 7461  e code must reta
-00000e30: 696e 2074 6865 2061 626f 7665 2063 6f70  in the above cop
-00000e40: 7972 6967 6874 206e 6f74 6963 652c 2074  yright notice, t
-00000e50: 6869 730a 2020 6c69 7374 206f 6620 636f  his.  list of co
-00000e60: 6e64 6974 696f 6e73 2061 6e64 2074 6865  nditions and the
-00000e70: 2066 6f6c 6c6f 7769 6e67 2064 6973 636c   following discl
-00000e80: 6169 6d65 722e 0a0a 2a20 5265 6469 7374  aimer...* Redist
-00000e90: 7269 6275 7469 6f6e 7320 696e 2062 696e  ributions in bin
-00000ea0: 6172 7920 666f 726d 206d 7573 7420 7265  ary form must re
-00000eb0: 7072 6f64 7563 6520 7468 6520 6162 6f76  produce the abov
-00000ec0: 6520 636f 7079 7269 6768 7420 6e6f 7469  e copyright noti
-00000ed0: 6365 2c0a 2020 7468 6973 206c 6973 7420  ce,.  this list 
-00000ee0: 6f66 2063 6f6e 6469 7469 6f6e 7320 616e  of conditions an
-00000ef0: 6420 7468 6520 666f 6c6c 6f77 696e 6720  d the following 
-00000f00: 6469 7363 6c61 696d 6572 2069 6e20 7468  disclaimer in th
-00000f10: 6520 646f 6375 6d65 6e74 6174 696f 6e0a  e documentation.
-00000f20: 2020 616e 642f 6f72 206f 7468 6572 206d    and/or other m
-00000f30: 6174 6572 6961 6c73 2070 726f 7669 6465  aterials provide
-00000f40: 6420 7769 7468 2074 6865 2064 6973 7472  d with the distr
-00000f50: 6962 7574 696f 6e2e 0a0a 5448 4953 2053  ibution...THIS S
-00000f60: 4f46 5457 4152 4520 4953 2050 524f 5649  OFTWARE IS PROVI
-00000f70: 4445 4420 4259 2054 4845 2043 4f50 5952  DED BY THE COPYR
-00000f80: 4947 4854 2048 4f4c 4445 5253 2041 4e44  IGHT HOLDERS AND
-00000f90: 2043 4f4e 5452 4942 5554 4f52 5320 2241   CONTRIBUTORS "A
-00000fa0: 5320 4953 220a 414e 4420 414e 5920 4558  S IS".AND ANY EX
-00000fb0: 5052 4553 5320 4f52 2049 4d50 4c49 4544  PRESS OR IMPLIED
-00000fc0: 2057 4152 5241 4e54 4945 532c 2049 4e43   WARRANTIES, INC
-00000fd0: 4c55 4449 4e47 2c20 4255 5420 4e4f 5420  LUDING, BUT NOT 
-00000fe0: 4c49 4d49 5445 4420 544f 2c20 5448 450a  LIMITED TO, THE.
-00000ff0: 494d 504c 4945 4420 5741 5252 414e 5449  IMPLIED WARRANTI
-00001000: 4553 204f 4620 4d45 5243 4841 4e54 4142  ES OF MERCHANTAB
-00001010: 494c 4954 5920 414e 4420 4649 544e 4553  ILITY AND FITNES
-00001020: 5320 464f 5220 4120 5041 5254 4943 554c  S FOR A PARTICUL
-00001030: 4152 2050 5552 504f 5345 2041 5245 0a44  AR PURPOSE ARE.D
-00001040: 4953 434c 4149 4d45 442e 2049 4e20 4e4f  ISCLAIMED. IN NO
-00001050: 2045 5645 4e54 2053 4841 4c4c 2054 4845   EVENT SHALL THE
-00001060: 2043 4f50 5952 4947 4854 2048 4f4c 4445   COPYRIGHT HOLDE
-00001070: 5220 4f52 2043 4f4e 5452 4942 5554 4f52  R OR CONTRIBUTOR
-00001080: 5320 4245 204c 4941 424c 450a 464f 5220  S BE LIABLE.FOR 
-00001090: 414e 5920 4449 5245 4354 2c20 494e 4449  ANY DIRECT, INDI
-000010a0: 5245 4354 2c20 494e 4349 4445 4e54 414c  RECT, INCIDENTAL
-000010b0: 2c20 5350 4543 4941 4c2c 2045 5845 4d50  , SPECIAL, EXEMP
-000010c0: 4c41 5259 2c20 4f52 2043 4f4e 5345 5155  LARY, OR CONSEQU
-000010d0: 454e 5449 414c 0a44 414d 4147 4553 2028  ENTIAL.DAMAGES (
-000010e0: 494e 434c 5544 494e 472c 2042 5554 204e  INCLUDING, BUT N
-000010f0: 4f54 204c 494d 4954 4544 2054 4f2c 2050  OT LIMITED TO, P
-00001100: 524f 4355 5245 4d45 4e54 204f 4620 5355  ROCUREMENT OF SU
-00001110: 4253 5449 5455 5445 2047 4f4f 4453 204f  BSTITUTE GOODS O
-00001120: 520a 5345 5256 4943 4553 3b20 4c4f 5353  R.SERVICES; LOSS
-00001130: 204f 4620 5553 452c 2044 4154 412c 204f   OF USE, DATA, O
-00001140: 5220 5052 4f46 4954 533b 204f 5220 4255  R PROFITS; OR BU
-00001150: 5349 4e45 5353 2049 4e54 4552 5255 5054  SINESS INTERRUPT
-00001160: 494f 4e29 2048 4f57 4556 4552 0a43 4155  ION) HOWEVER.CAU
-00001170: 5345 4420 414e 4420 4f4e 2041 4e59 2054  SED AND ON ANY T
-00001180: 4845 4f52 5920 4f46 204c 4941 4249 4c49  HEORY OF LIABILI
-00001190: 5459 2c20 5748 4554 4845 5220 494e 2043  TY, WHETHER IN C
-000011a0: 4f4e 5452 4143 542c 2053 5452 4943 5420  ONTRACT, STRICT 
-000011b0: 4c49 4142 494c 4954 592c 0a4f 5220 544f  LIABILITY,.OR TO
-000011c0: 5254 2028 494e 434c 5544 494e 4720 4e45  RT (INCLUDING NE
-000011d0: 474c 4947 454e 4345 204f 5220 4f54 4845  GLIGENCE OR OTHE
-000011e0: 5257 4953 4529 2041 5249 5349 4e47 2049  RWISE) ARISING I
-000011f0: 4e20 414e 5920 5741 5920 4f55 5420 4f46  N ANY WAY OUT OF
-00001200: 2054 4845 2055 5345 0a4f 4620 5448 4953   THE USE.OF THIS
-00001210: 2053 4f46 5457 4152 452c 2045 5645 4e20   SOFTWARE, EVEN 
-00001220: 4946 2041 4456 4953 4544 204f 4620 5448  IF ADVISED OF TH
-00001230: 4520 504f 5353 4942 494c 4954 5920 4f46  E POSSIBILITY OF
-00001240: 2053 5543 4820 4441 4d41 4745 2e0a 6060   SUCH DAMAGE..``
-00001250: 600a                                     `.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 726f 6572  : 2.1.Name: roer
+00000020: 6963 680a 5665 7273 696f 6e3a 2030 2e36  ich.Version: 0.6
+00000030: 2e30 0a53 756d 6d61 7279 3a20 4368 616e  .0.Summary: Chan
+00000040: 6765 2070 6f69 6e74 2064 6574 6563 7469  ge point detecti
+00000050: 6f6e 2e0a 486f 6d65 2d70 6167 653a 2068  on..Home-page: h
+00000060: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000070: 6d2f 4853 452d 4c41 4d42 4441 2f72 6f65  m/HSE-LAMBDA/roe
+00000080: 7269 6368 0a41 7574 686f 723a 204d 696b  rich.Author: Mik
+00000090: 6861 696c 2048 7573 6863 6879 6e2c 204b  hail Hushchyn, K
+000000a0: 656e 656e 6265 6b20 4172 7a79 6d61 746f  enenbek Arzymato
+000000b0: 760a 4175 7468 6f72 2d65 6d61 696c 3a20  v.Author-email: 
+000000c0: 6875 7368 6368 796e 2e6d 696b 6861 696c  hushchyn.mikhail
+000000d0: 4067 6d61 696c 2e63 6f6d 2c20 6b65 6e65  @gmail.com, kene
+000000e0: 6e62 656b 4067 6d61 696c 2e63 6f6d 0a4c  nbek@gmail.com.L
+000000f0: 6963 656e 7365 3a20 4253 442d 322d 436c  icense: BSD-2-Cl
+00000100: 6175 7365 0a50 726f 6a65 6374 2d55 524c  ause.Project-URL
+00000110: 3a20 446f 6375 6d65 6e74 6174 696f 6e2c  : Documentation,
+00000120: 2068 7474 7073 3a2f 2f68 7365 2d6c 616d   https://hse-lam
+00000130: 6264 612e 6769 7468 7562 2e69 6f2f 726f  bda.github.io/ro
+00000140: 6572 6963 682f 0a50 726f 6a65 6374 2d55  erich/.Project-U
+00000150: 524c 3a20 536f 7572 6365 2c20 6874 7470  RL: Source, http
+00000160: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f48  s://github.com/H
+00000170: 5345 2d4c 414d 4244 412f 726f 6572 6963  SE-LAMBDA/roeric
+00000180: 682f 0a4b 6579 776f 7264 733a 2070 7974  h/.Keywords: pyt
+00000190: 686f 6e2c 6d61 6368 696e 6520 6c65 6172  hon,machine lear
+000001a0: 6e69 6e67 2c6e 6575 7261 6c20 6e65 7477  ning,neural netw
+000001b0: 6f72 6b73 2c73 6967 6e61 6c20 7072 6f63  orks,signal proc
+000001c0: 6573 7369 6e67 2c73 6567 6d65 6e74 6174  essing,segmentat
+000001d0: 696f 6e2c 7469 6d65 2073 6572 6965 7320  ion,time series 
+000001e0: 616e 616c 7973 6973 2c61 6e6f 6d61 6c79  analysis,anomaly
+000001f0: 2064 6574 6563 7469 6f6e 2c63 6861 6e67   detection,chang
+00000200: 6520 706f 696e 7420 6465 7465 6374 696f  e point detectio
+00000210: 6e2c 6465 6e73 6974 7920 7261 7469 6f0a  n,density ratio.
+00000220: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000230: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000240: 2053 6369 656e 6365 2f52 6573 6561 7263   Science/Researc
+00000250: 680a 436c 6173 7369 6669 6572 3a20 546f  h.Classifier: To
+00000260: 7069 6320 3a3a 2053 6369 656e 7469 6669  pic :: Scientifi
+00000270: 632f 456e 6769 6e65 6572 696e 670a 436c  c/Engineering.Cl
+00000280: 6173 7369 6669 6572 3a20 5072 6f67 7261  assifier: Progra
+00000290: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+000002a0: 3a20 5079 7468 6f6e 203a 3a20 330a 436c  : Python :: 3.Cl
+000002b0: 6173 7369 6669 6572 3a20 4c69 6365 6e73  assifier: Licens
+000002c0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000002d0: 6420 3a3a 2042 5344 204c 6963 656e 7365  d :: BSD License
+000002e0: 0a43 6c61 7373 6966 6965 723a 204f 7065  .Classifier: Ope
+000002f0: 7261 7469 6e67 2053 7973 7465 6d20 3a3a  rating System ::
+00000300: 204f 5320 496e 6465 7065 6e64 656e 740a   OS Independent.
+00000310: 5265 7175 6972 6573 2d50 7974 686f 6e3a  Requires-Python:
+00000320: 203e 3d33 2e36 0a44 6573 6372 6970 7469   >=3.6.Descripti
+00000330: 6f6e 2d43 6f6e 7465 6e74 2d54 7970 653a  on-Content-Type:
+00000340: 2074 6578 742f 6d61 726b 646f 776e 0a4c   text/markdown.L
+00000350: 6963 656e 7365 2d46 696c 653a 204c 4943  icense-File: LIC
+00000360: 454e 5345 0a0a 2320 5765 6c63 6f6d 6520  ENSE..# Welcome 
+00000370: 746f 2052 6f65 7269 6368 0a0a 5b21 5b50  to Roerich..[![P
+00000380: 7950 4920 7665 7273 696f 6e5d 2868 7474  yPI version](htt
+00000390: 7073 3a2f 2f62 6164 6765 2e66 7572 792e  ps://badge.fury.
+000003a0: 696f 2f70 792f 726f 6572 6963 682e 7376  io/py/roerich.sv
+000003b0: 6729 5d28 6874 7470 733a 2f2f 6261 6467  g)](https://badg
+000003c0: 652e 6675 7279 2e69 6f2f 7079 2f72 6f65  e.fury.io/py/roe
+000003d0: 7269 6368 290a 5b21 5b44 6f63 756d 656e  rich).[![Documen
+000003e0: 7461 7469 6f6e 5d28 6874 7470 733a 2f2f  tation](https://
+000003f0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+00000400: 6164 6765 2f64 6f63 756d 656e 7461 7469  adge/documentati
+00000410: 6f6e 2d79 6573 2d67 7265 656e 2e73 7667  on-yes-green.svg
+00000420: 295d 2868 7474 7073 3a2f 2f68 7365 2d6c  )](https://hse-l
+00000430: 616d 6264 612e 6769 7468 7562 2e69 6f2f  ambda.github.io/
+00000440: 726f 6572 6963 6829 0a5b 215b 446f 776e  roerich).[![Down
+00000450: 6c6f 6164 735d 2868 7474 7073 3a2f 2f70  loads](https://p
+00000460: 6570 792e 7465 6368 2f62 6164 6765 2f72  epy.tech/badge/r
+00000470: 6f65 7269 6368 295d 2868 7474 7073 3a2f  oerich)](https:/
+00000480: 2f70 6570 792e 7465 6368 2f70 726f 6a65  /pepy.tech/proje
+00000490: 6374 2f72 6f65 7269 6368 290a 5b21 5b4c  ct/roerich).[![L
+000004a0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+000004b0: 696d 672e 7368 6965 6c64 732e 696f 2f62  img.shields.io/b
+000004c0: 6164 6765 2f4c 6963 656e 7365 2d42 5344  adge/License-BSD
+000004d0: 5f32 2d2d 436c 6175 7365 2d6f 7261 6e67  _2--Clause-orang
+000004e0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+000004f0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+00000500: 6963 656e 7365 732f 4253 442d 322d 436c  icenses/BSD-2-Cl
+00000510: 6175 7365 290a 0a60 526f 6572 6963 6860  ause)..`Roerich`
+00000520: 2069 7320 6120 7079 7468 6f6e 206c 6962   is a python lib
+00000530: 7261 7279 2066 6f72 206f 6e6c 696e 6520  rary for online 
+00000540: 616e 6420 6f66 666c 696e 6520 6368 616e  and offline chan
+00000550: 6765 2070 6f69 6e74 2064 6574 6563 7469  ge point detecti
+00000560: 6f6e 2066 6f72 2074 696d 6520 7365 7269  on for time seri
+00000570: 6573 2061 6e61 6c79 7369 732c 2073 6967  es analysis, sig
+00000580: 6e61 6c20 7072 6f63 6573 7369 6e67 2c20  nal processing, 
+00000590: 616e 6420 7365 676d 656e 7461 7469 6f6e  and segmentation
+000005a0: 2e20 4974 2077 6173 206e 616d 6564 2061  . It was named a
+000005b0: 6674 6572 2074 6865 2070 6169 6e74 6572  fter the painter
+000005c0: 204e 6963 686f 6c61 7320 526f 6572 6963   Nicholas Roeric
+000005d0: 682c 206b 6e6f 776e 2061 7320 7468 6520  h, known as the 
+000005e0: 4d61 7374 6572 206f 6620 7468 6520 4d6f  Master of the Mo
+000005f0: 756e 7461 696e 732e 2052 6561 6420 6d6f  untains. Read mo
+00000600: 7265 2061 743a 2068 7474 7073 3a2f 2f77  re at: https://w
+00000610: 7777 2e72 6f65 7269 6368 2e6f 7267 2e0a  ww.roerich.org..
+00000620: 0a21 5b5d 2868 7474 7073 3a2f 2f72 6177  .![](https://raw
+00000630: 2e67 6974 6875 6275 7365 7263 6f6e 7465  .githubuserconte
+00000640: 6e74 2e63 6f6d 2f48 5345 2d4c 414d 4244  nt.com/HSE-LAMBD
+00000650: 412f 726f 6572 6963 682f 6d61 696e 2f69  A/roerich/main/i
+00000660: 6d61 6765 732f 3730 3031 3235 7631 2e6a  mages/700125v1.j
+00000670: 7065 6729 0a5f 4672 6167 6d65 6e74 206f  peg)._Fragment o
+00000680: 6620 2248 696d 616c 6179 6173 222c 2031  f "Himalayas", 1
+00000690: 3933 335f 0a0a 4375 7272 656e 746c 792c  933_..Currently,
+000006a0: 2074 6865 206c 6962 7261 7279 2063 6f6e   the library con
+000006b0: 7461 696e 7320 6f66 6669 6369 616c 2069  tains official i
+000006c0: 6d70 6c65 6d65 6e74 6174 696f 6e73 206f  mplementations o
+000006d0: 6620 6368 616e 6765 2070 6f69 6e74 2064  f change point d
+000006e0: 6574 6563 7469 6f6e 2061 6c67 6f72 6974  etection algorit
+000006f0: 686d 7320 6261 7365 6420 6f6e 2064 6972  hms based on dir
+00000700: 6563 7420 6465 6e73 6974 7920 7261 7469  ect density rati
+00000710: 6f20 6573 7469 6d61 7469 6f6e 2066 726f  o estimation fro
+00000720: 6d20 7468 6520 666f 6c6c 6f77 696e 6720  m the following 
+00000730: 6172 7469 636c 6573 3a0a 0a2d 204d 696b  articles:..- Mik
+00000740: 6861 696c 2048 7573 6863 6879 6e20 616e  hail Hushchyn an
+00000750: 6420 416e 6472 6579 2055 7374 7975 7a68  d Andrey Ustyuzh
+00000760: 616e 696e 2e20 e280 9c47 656e 6572 616c  anin. ...General
+00000770: 697a 6174 696f 6e20 6f66 2043 6861 6e67  ization of Chang
+00000780: 652d 506f 696e 7420 4465 7465 6374 696f  e-Point Detectio
+00000790: 6e20 696e 2054 696d 6520 5365 7269 6573  n in Time Series
+000007a0: 2044 6174 6120 4261 7365 6420 6f6e 2044   Data Based on D
+000007b0: 6972 6563 7420 4465 6e73 6974 7920 5261  irect Density Ra
+000007c0: 7469 6f20 4573 7469 6d61 7469 6f6e 2ee2  tio Estimation..
+000007d0: 809d 204a 2e20 436f 6d70 7574 2e20 5363  .. J. Comput. Sc
+000007e0: 692e 2035 3320 2832 3032 3129 3a20 3130  i. 53 (2021): 10
+000007f0: 3133 3835 2e20 5b5b 6a6f 7572 6e61 6c5d  1385. [[journal]
+00000800: 5d28 6874 7470 733a 2f2f 646f 692e 6f72  ](https://doi.or
+00000810: 672f 3130 2e31 3031 362f 6a2e 6a6f 6373  g/10.1016/j.jocs
+00000820: 2e32 3032 312e 3130 3133 3835 2920 5b5b  .2021.101385) [[
+00000830: 6172 7869 765d 5d28 6874 7470 733a 2f2f  arxiv]](https://
+00000840: 646f 692e 6f72 672f 3130 2e34 3835 3530  doi.org/10.48550
+00000850: 2f61 7258 6976 2e32 3030 312e 3036 3338  /arXiv.2001.0638
+00000860: 3629 0a2d 204d 696b 6861 696c 2048 7573  6).- Mikhail Hus
+00000870: 6863 6879 6e2c 204b 656e 656e 6265 6b20  hchyn, Kenenbek 
+00000880: 4172 7a79 6d61 746f 7620 616e 6420 4465  Arzymatov and De
+00000890: 6e69 7320 4465 726b 6163 682e 20e2 809c  nis Derkach. ...
+000008a0: 4f6e 6c69 6e65 204e 6575 7261 6c20 4e65  Online Neural Ne
+000008b0: 7477 6f72 6b73 2066 6f72 2043 6861 6e67  tworks for Chang
+000008c0: 652d 506f 696e 7420 4465 7465 6374 696f  e-Point Detectio
+000008d0: 6e2e e280 9d20 4172 5869 7620 6162 732f  n.... ArXiv abs/
+000008e0: 3230 3130 2e30 3133 3838 2028 3230 3230  2010.01388 (2020
+000008f0: 292e 205b 5b61 7278 6976 5d5d 2868 7474  ). [[arxiv]](htt
+00000900: 7073 3a2f 2f64 6f69 2e6f 7267 2f31 302e  ps://doi.org/10.
+00000910: 3438 3535 302f 6172 5869 762e 3230 3130  48550/arXiv.2010
+00000920: 2e30 3133 3838 290a 0a23 2320 4465 7065  .01388)..## Depe
+00000930: 6e64 656e 6369 6573 2061 6e64 2069 6e73  ndencies and ins
+00000940: 7461 6c6c 0a0a 6060 600a 7069 7020 696e  tall..```.pip in
+00000950: 7374 616c 6c20 726f 6572 6963 680a 6060  stall roerich.``
+00000960: 600a 6f72 0a60 6060 7079 7468 6f6e 0a67  `.or.```python.g
+00000970: 6974 2063 6c6f 6e65 2068 7474 7073 3a2f  it clone https:/
+00000980: 2f67 6974 6875 622e 636f 6d2f 4853 452d  /github.com/HSE-
+00000990: 4c41 4d42 4441 2f72 6f65 7269 6368 2e67  LAMBDA/roerich.g
+000009a0: 6974 0a63 6420 726f 6572 6963 680a 7069  it.cd roerich.pi
+000009b0: 7020 696e 7374 616c 6c20 2d65 202e 0a60  p install -e ..`
+000009c0: 6060 0a0a 2323 2042 6173 6963 2075 7361  ``..## Basic usa
+000009d0: 6765 0a0a 2853 6565 206d 6f72 6520 6578  ge..(See more ex
+000009e0: 616d 706c 6573 2069 6e20 7468 6520 5b64  amples in the [d
+000009f0: 6f63 756d 656e 7461 7469 6f6e 5d28 6874  ocumentation](ht
+00000a00: 7470 733a 2f2f 6873 652d 6c61 6d62 6461  tps://hse-lambda
+00000a10: 2e67 6974 6875 622e 696f 2f72 6f65 7269  .github.io/roeri
+00000a20: 6368 292e 290a 0a54 6865 2066 6f6c 6c6f  ch).)..The follo
+00000a30: 7769 6e67 2063 6f64 6520 736e 6970 7065  wing code snippe
+00000a40: 7420 6765 6e65 7261 7465 7320 6120 6e6f  t generates a no
+00000a50: 6973 7920 7379 6e74 6865 7469 6320 6461  isy synthetic da
+00000a60: 7461 2c20 7065 7266 6f72 6d73 2063 6861  ta, performs cha
+00000a70: 6e67 6520 706f 696e 7420 6465 7465 6374  nge point detect
+00000a80: 696f 6e2c 2061 6e64 2064 6973 706c 6179  ion, and display
+00000a90: 7320 7468 6520 7265 7375 6c74 732e 2049  s the results. I
+00000aa0: 6620 796f 7520 7573 6520 6f77 6e20 6461  f you use own da
+00000ab0: 7461 7365 742c 206d 616b 650a 7375 7265  taset, make.sure
+00000ac0: 2074 6861 7420 6974 2068 6173 2061 2073   that it has a s
+00000ad0: 6861 7065 2060 2873 6571 5f6c 656e 2c20  hape `(seq_len, 
+00000ae0: 6e5f 6469 6d73 2960 2e0a 6060 6070 7974  n_dims)`..```pyt
+00000af0: 686f 6e0a 696d 706f 7274 2072 6f65 7269  hon.import roeri
+00000b00: 6368 0a66 726f 6d20 726f 6572 6963 682e  ch.from roerich.
+00000b10: 6368 616e 6765 5f70 6f69 6e74 2069 6d70  change_point imp
+00000b20: 6f72 7420 4368 616e 6765 506f 696e 7444  ort ChangePointD
+00000b30: 6574 6563 7469 6f6e 436c 6173 7369 6669  etectionClassifi
+00000b40: 6572 0a0a 2320 6765 6e65 7261 7465 2074  er..# generate t
+00000b50: 696d 6520 7365 7269 6573 0a58 2c20 6370  ime series.X, cp
+00000b60: 735f 7472 7565 203d 2072 6f65 7269 6368  s_true = roerich
+00000b70: 2e67 656e 6572 6174 655f 6461 7461 7365  .generate_datase
+00000b80: 7428 7065 7269 6f64 3d32 3030 2c20 4e5f  t(period=200, N_
+00000b90: 746f 743d 3230 3030 290a 0a23 2064 6574  tot=2000)..# det
+00000ba0: 6563 7469 6f6e 0a23 2062 6173 655f 636c  ection.# base_cl
+00000bb0: 6173 7369 6669 6572 203d 2027 6c6f 6772  assifier = 'logr
+00000bc0: 6567 272c 2027 7164 6127 2c20 2764 7427  eg', 'qda', 'dt'
+00000bd0: 2c20 2772 6627 2c20 276d 6c70 272c 2027  , 'rf', 'mlp', '
+00000be0: 6b6e 6e27 2c20 276e 6227 0a23 206d 6574  knn', 'nb'.# met
+00000bf0: 7269 6320 3d20 276b 6c73 796d 272c 2027  ric = 'klsym', '
+00000c00: 7065 7379 6d27 2c20 276a 7364 272c 2027  pesym', 'jsd', '
+00000c10: 6d6d 6427 2c20 2766 6427 0a63 7064 203d  mmd', 'fd'.cpd =
+00000c20: 2043 6861 6e67 6550 6f69 6e74 4465 7465   ChangePointDete
+00000c30: 6374 696f 6e43 6c61 7373 6966 6965 7228  ctionClassifier(
+00000c40: 6261 7365 5f63 6c61 7373 6966 6965 723d  base_classifier=
+00000c50: 276d 6c70 272c 206d 6574 7269 633d 276b  'mlp', metric='k
+00000c60: 6c73 796d 272c 2077 696e 646f 775f 7369  lsym', window_si
+00000c70: 7a65 3d31 3030 290a 7363 6f72 652c 2063  ze=100).score, c
+00000c80: 7073 5f70 7265 6420 3d20 6370 642e 7072  ps_pred = cpd.pr
+00000c90: 6564 6963 7428 5829 0a0a 2320 7669 7375  edict(X)..# visu
+00000ca0: 616c 697a 6174 696f 6e0a 726f 6572 6963  alization.roeric
+00000cb0: 682e 6469 7370 6c61 7928 582c 2063 7073  h.display(X, cps
+00000cc0: 5f74 7275 652c 2073 636f 7265 2c20 6370  _true, score, cp
+00000cd0: 735f 7072 6564 290a 6060 600a 0a21 5b5d  s_pred).```..![]
+00000ce0: 2868 7474 7073 3a2f 2f72 6177 2e67 6974  (https://raw.git
+00000cf0: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
+00000d00: 6f6d 2f48 5345 2d4c 414d 4244 412f 726f  om/HSE-LAMBDA/ro
+00000d10: 6572 6963 682f 6d61 696e 2f69 6d61 6765  erich/main/image
+00000d20: 732f 6465 6d6f 2e70 6e67 290a 0a23 2320  s/demo.png)..## 
+00000d30: 5375 7070 6f72 740a 0a2d 2048 6f6d 653a  Support..- Home:
+00000d40: 205b 6874 7470 733a 2f2f 6769 7468 7562   [https://github
+00000d50: 2e63 6f6d 2f48 5345 2d4c 414d 4244 412f  .com/HSE-LAMBDA/
+00000d60: 726f 6572 6963 685d 2868 7474 7073 3a2f  roerich](https:/
+00000d70: 2f67 6974 6875 622e 636f 6d2f 4853 452d  /github.com/HSE-
+00000d80: 4c41 4d42 4441 2f72 6f65 7269 6368 290a  LAMBDA/roerich).
+00000d90: 2d20 446f 6375 6d65 6e74 6174 696f 6e3a  - Documentation:
+00000da0: 205b 6874 7470 733a 2f2f 6873 652d 6c61   [https://hse-la
+00000db0: 6d62 6461 2e67 6974 6875 622e 696f 2f72  mbda.github.io/r
+00000dc0: 6f65 7269 6368 5d28 6874 7470 733a 2f2f  oerich](https://
+00000dd0: 6873 652d 6c61 6d62 6461 2e67 6974 6875  hse-lambda.githu
+00000de0: 622e 696f 2f72 6f65 7269 6368 290a 2d20  b.io/roerich).- 
+00000df0: 466f 7220 616e 7920 7573 6167 6520 7175  For any usage qu
+00000e00: 6573 7469 6f6e 732c 2073 7567 6765 7374  estions, suggest
+00000e10: 696f 6e73 2061 6e64 2062 7567 7320 7573  ions and bugs us
+00000e20: 6520 7468 6520 5b69 7373 7565 2070 6167  e the [issue pag
+00000e30: 655d 2868 7474 7073 3a2f 2f67 6974 6875  e](https://githu
+00000e40: 622e 636f 6d2f 4853 452d 4c41 4d42 4441  b.com/HSE-LAMBDA
+00000e50: 2f72 6f65 7269 6368 2f69 7373 7565 7329  /roerich/issues)
+00000e60: 2c20 706c 6561 7365 2e0a 0a23 2320 5265  , please...## Re
+00000e70: 6c61 7465 6420 6c69 6272 6172 6965 730a  lated libraries.
+00000e80: 0a5b 215b 4765 6e65 7269 6320 6261 6467  .[![Generic badg
+00000e90: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000ea0: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000eb0: 5e2e 5e2d 7275 7074 7572 6573 2d62 6c75  ^.^-ruptures-blu
+00000ec0: 652e 7376 6729 5d28 6874 7470 733a 2f2f  e.svg)](https://
+00000ed0: 6769 7468 7562 2e63 6f6d 2f64 6565 7063  github.com/deepc
+00000ee0: 6861 726c 6573 2f72 7570 7475 7265 7329  harles/ruptures)
+00000ef0: 0a5b 215b 4765 6e65 7269 6320 6261 6467  .[![Generic badg
+00000f00: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000f10: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000f20: 5e2e 5e2d 6b6c 6370 642d 626c 7565 2e73  ^.^-klcpd-blue.s
+00000f30: 7667 295d 2868 7474 7073 3a2f 2f67 6974  vg)](https://git
+00000f40: 6875 622e 636f 6d2f 486f 6c79 4261 7965  hub.com/HolyBaye
+00000f50: 732f 6b6c 6370 6429 0a5b 215b 4765 6e65  s/klcpd).[![Gene
+00000f60: 7269 6320 6261 6467 655d 2868 7474 7073  ric badge](https
+00000f70: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000f80: 6f2f 6261 6467 652f 5e2e 5e2d 7469 7265  o/badge/^.^-tire
+00000f90: 2d62 6c75 652e 7376 6729 5d28 6874 7470  -blue.svg)](http
+00000fa0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f48  s://github.com/H
+00000fb0: 6f6c 7942 6179 6573 2f54 4952 455f 7079  olyBayes/TIRE_py
+00000fc0: 746f 7263 6829 0a5b 215b 4765 6e65 7269  torch).[![Generi
+00000fd0: 6320 6261 6467 655d 2868 7474 7073 3a2f  c badge](https:/
+00000fe0: 2f69 6d67 2e73 6869 656c 6473 2e69 6f2f  /img.shields.io/
+00000ff0: 6261 6467 652f 5e2e 5e2d 626f 6370 642d  badge/^.^-bocpd-
+00001000: 626c 7565 2e73 7667 295d 2868 7474 7073  blue.svg)](https
+00001010: 3a2f 2f67 6974 6875 622e 636f 6d2f 6869  ://github.com/hi
+00001020: 6c64 656e 7369 612f 6261 7965 7369 616e  ldensia/bayesian
+00001030: 5f63 6861 6e67 6570 6f69 6e74 5f64 6574  _changepoint_det
+00001040: 6563 7469 6f6e 290a 0a23 2320 5468 616e  ection)..## Than
+00001050: 6b73 2074 6f20 616c 6c20 6f75 7220 636f  ks to all our co
+00001060: 6e74 7269 6275 746f 7273 0a0a 3c61 2068  ntributors..<a h
+00001070: 7265 663d 2268 7474 7073 3a2f 2f67 6974  ref="https://git
+00001080: 6875 622e 636f 6d2f 4853 452d 4c41 4d42  hub.com/HSE-LAMB
+00001090: 4441 2f72 6f65 7269 6368 2f67 7261 7068  DA/roerich/graph
+000010a0: 732f 636f 6e74 7269 6275 746f 7273 223e  s/contributors">
+000010b0: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
+000010c0: 7073 3a2f 2f63 6f6e 7472 6962 7574 6f72  ps://contributor
+000010d0: 732d 696d 672e 7765 622e 6170 702f 696d  s-img.web.app/im
+000010e0: 6167 653f 7265 706f 3d48 5345 2d4c 414d  age?repo=HSE-LAM
+000010f0: 4244 412f 726f 6572 6963 6822 202f 3e0a  BDA/roerich" />.
+00001100: 3c2f 613e 0a0a                           </a>..
```

### Comparing `roerich-0.5.0/roerich/algorithms/__init__.py` & `roerich-0.6.0/roerich/algorithms/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-from .algorithms import OnlineNNClassifier, OnlineNNRuLSIF
+from ..change_point.onnr import OnlineNNRuLSIF
+from ..change_point.onnc import OnlineNNClassifier
 from .cpdc import ChangePointDetectionClassifier, ChangePointDetectionRuLSIF
 from .matrix import MatrixImportance
 from .enrg_dist import EnergyDistanceCalculator
 from .cpdc_cv import ChangePointDetectionClassifierCV
 from .models import GBDTRuLSIFRegressor
 from .models import RegressionNetwork, NNRuLSIFRegressor
 from .models import ClassificationNetwork, NNClassifier
 
 
 __all__ = [
-    'OnlineNNClassifier', 
-    'OnlineNNRuLSIF', 
+    'OnlineNNClassifier',
+    'OnlineNNRuLSIF',
     'ChangePointDetectionClassifier', 
     'ChangePointDetectionRuLSIF',
     'MatrixImportance',
     'EnergyDistanceCalculator',
     'ChangePointDetectionClassifierCV',
     'ClassificationNetwork', 
     'NNClassifier',
```

### Comparing `roerich-0.5.0/roerich/algorithms/enrg_dist.py` & `roerich-0.6.0/roerich/algorithms/enrg_dist.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich/algorithms/matrix.py` & `roerich-0.6.0/roerich/algorithms/matrix.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich/algorithms/models.py` & `roerich-0.6.0/roerich/algorithms/models.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich/algorithms/net.py` & `roerich-0.6.0/roerich/algorithms/net.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich/metrics/pr.py` & `roerich-0.6.0/roerich/metrics/pr.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich/viz.py` & `roerich-0.6.0/roerich/viz.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/roerich.egg-info/SOURCES.txt` & `roerich-0.6.0/roerich.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,39 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 roerich/__init__.py
 roerich/dataset.py
-roerich/helper.py
-roerich/utils.py
 roerich/viz.py
 roerich.egg-info/PKG-INFO
 roerich.egg-info/SOURCES.txt
 roerich.egg-info/dependency_links.txt
 roerich.egg-info/requires.txt
 roerich.egg-info/top_level.txt
 roerich/algorithms/__init__.py
-roerich/algorithms/algorithms.py
 roerich/algorithms/cpdc.py
 roerich/algorithms/cpdc_cv.py
 roerich/algorithms/enrg_dist.py
 roerich/algorithms/matrix.py
 roerich/algorithms/models.py
 roerich/algorithms/net.py
-roerich/algorithms/scaler.py
 roerich/change_point/__init__.py
+roerich/change_point/onnc.py
+roerich/change_point/onnr.py
+roerich/change_point/windows.py
 roerich/density_ratio/__init__.py
 roerich/explanation/__init__.py
 roerich/metrics/__init__.py
-roerich/metrics/metrics.py
 roerich/metrics/pr.py
 roerich/networks/__init__.py
+roerich/scores/__init__.py
+roerich/scores/energy.py
+roerich/scores/fd.py
+roerich/scores/mmd.py
 tests/test_change_point.py
 tests/test_density_ratio.py
 tests/test_explanation.py
 tests/test_metrics.py
-tests/test_networks.py
+tests/test_networks.py
+tests/test_scores.py
```

### Comparing `roerich-0.5.0/setup.cfg` & `roerich-0.6.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = roerich
-version = 0.5.0
+version = 0.6.0
 author = Mikhail Hushchyn, Kenenbek Arzymatov
 author_email = hushchyn.mikhail@gmail.com, kenenbek@gmail.com
-description = Roerich is a python library for online and offline change point detection in time series data based on machine learning.
+description = Change point detection.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/HSE-LAMBDA/roerich
 project_urls = 
 	Documentation = https://hse-lambda.github.io/roerich/
 	Source = https://github.com/HSE-LAMBDA/roerich/
 license = BSD-2-Clause
```

### Comparing `roerich-0.5.0/tests/test_density_ratio.py` & `roerich-0.6.0/tests/test_density_ratio.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/tests/test_explanation.py` & `roerich-0.6.0/tests/test_explanation.py`

 * *Files identical despite different names*

### Comparing `roerich-0.5.0/tests/test_metrics.py` & `roerich-0.6.0/tests/test_metrics.py`

 * *Files identical despite different names*

