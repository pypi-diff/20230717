# Comparing `tmp/cmind-1.5.0.tar.gz` & `tmp/cmind-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmind-1.5.0.tar", last modified: Wed Jul  5 19:29:19 2023, max compression
+gzip compressed data, was "cmind-1.5.1.tar", last modified: Mon Jul 17 20:13:26 2023, max compression
```

## Comparing `cmind-1.5.0.tar` & `cmind-1.5.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6415 2023-07-05 19:29:19.373726 cmind-1.5.0/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5428 2023-07-05 19:28:57.000000 cmind-1.5.0/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/__main__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2023-06-19 07:06:03.000000 cmind-1.5.0/cmind/artifact.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    46812 2023-06-19 07:06:30.000000 cmind-1.5.0/cmind/automation.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     5324 2023-06-09 07:26:00.000000 cmind-1.5.0/cmind/cli.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/config.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-06-06 10:14:36.000000 cmind-1.5.0/cmind/core.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9500 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/index.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/net.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/README.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/automation/
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind/repo/automation/automation/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/automation/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module_dummy.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/module_misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/automation/template_list_of_automations.md
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/ck/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/ck/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/ck/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/ck/module.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/core/
--rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/core/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/_cm.json
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/
--rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/core/module_misc.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.373726 cmind-1.5.0/cmind/repo/automation/repo/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-05-30 19:25:20.000000 cmind-1.5.0/cmind/repo/automation/repo/README.md
--rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/automation/repo/_cm.json
--rw-r--r--   0 fursin    (1000) fursin    (1000)    31292 2023-07-05 19:28:57.000000 cmind-1.5.0/cmind/repo/automation/repo/module.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo/cmr.yaml
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repo.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/repos.py
--rw-r--r--   0 fursin    (1000) fursin    (1000)    41400 2023-05-25 12:13:31.000000 cmind-1.5.0/cmind/utils.py
-drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-05 19:29:19.363726 cmind-1.5.0/cmind.egg-info/
--rw-r--r--   0 fursin    (1000) fursin    (1000)     6415 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/PKG-INFO
--rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/SOURCES.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/dependency_links.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)      118 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/entry_points.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-06-06 10:27:33.000000 cmind-1.5.0/cmind.egg-info/not-zip-safe
--rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/requires.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-07-05 19:29:19.000000 cmind-1.5.0/cmind.egg-info/top_level.txt
--rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-07-05 19:29:19.373726 cmind-1.5.0/setup.cfg
--rw-r--r--   0 fursin    (1000) fursin    (1000)     2808 2023-06-09 07:26:00.000000 cmind-1.5.0/setup.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6591 2023-07-17 20:13:26.314896 cmind-1.5.1/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5588 2023-07-17 20:08:31.000000 cmind-1.5.1/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      136 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       35 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/__main__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     4888 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/artifact.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    46812 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/automation.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     5324 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/cli.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3285 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/config.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    24589 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/core.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9500 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/index.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2046 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/net.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      491 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/README.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/automation/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2647 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      289 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     3799 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1518 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/module_dummy.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     8772 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/module_misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      310 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/automation/template_list_of_automations.md
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/ck/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      984 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/ck/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      325 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/ck/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1015 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/ck/module.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/core/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      996 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      302 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/_cm.json
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/core/cm_60cb625a46b38610/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/cm_60cb625a46b38610/__init__.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/cm_60cb625a46b38610/misc.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1008 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      220 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/core/module_misc.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind/repo/automation/repo/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     9508 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/repo/README.md
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      377 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/repo/_cm.json
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    31292 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/automation/repo/module.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       71 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo/cmr.yaml
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1978 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repo.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    18709 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/repos.py
+-rw-r--r--   0 fursin    (1000) fursin    (1000)    41515 2023-07-17 20:08:31.000000 cmind-1.5.1/cmind/utils.py
+drwxr-xr-x   0 fursin    (1000) fursin    (1000)        0 2023-07-17 20:13:26.314896 cmind-1.5.1/cmind.egg-info/
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     6591 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/PKG-INFO
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     1222 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/SOURCES.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/dependency_links.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)      118 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/entry_points.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        1 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/not-zip-safe
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       16 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/requires.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)        6 2023-07-17 20:13:26.000000 cmind-1.5.1/cmind.egg-info/top_level.txt
+-rw-r--r--   0 fursin    (1000) fursin    (1000)       38 2023-07-17 20:13:26.314896 cmind-1.5.1/setup.cfg
+-rw-r--r--   0 fursin    (1000) fursin    (1000)     2808 2023-07-17 20:08:31.000000 cmind-1.5.1/setup.py
```

### Comparing `cmind-1.5.0/PKG-INFO` & `cmind-1.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.5.0
+Version: 1.5.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -12,18 +12,20 @@
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
         [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
         
         ### About
         
-        *Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
-        and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+        ***We deeply believe in the power of open science and open source to solve the world's most challenging problems.
+           That's why we are developing a common automation and reproducibility language to help connect academia and industry,
+           facilitate reproducible research and bridge the growing gap between research and production - 
+           [see our ACM REP'23 keynote for more details](https://doi.org/10.5281/zenodo.8105339)!***
         
-        [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
+        [Collective Mind automation and reproducibility language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
         is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
         It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
         when reproducing experiments from more than 150 research papers and validating them in the real world - 
         there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
         on any platform with any software, hardware, and data.
         
         CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-1.5.0/README.md` & `cmind-1.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,18 +4,20 @@
 [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
 
 [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
 [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
 
 ### About
 
-*Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
-and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+***We deeply believe in the power of open science and open source to solve the world's most challenging problems.
+   That's why we are developing a common automation and reproducibility language to help connect academia and industry,
+   facilitate reproducible research and bridge the growing gap between research and production - 
+   [see our ACM REP'23 keynote for more details](https://doi.org/10.5281/zenodo.8105339)!***
 
-[Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
+[Collective Mind automation and reproducibility language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
 is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
 It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
 when reproducing experiments from more than 150 research papers and validating them in the real world - 
 there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
 on any platform with any software, hardware, and data.
 
 CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-1.5.0/cmind/artifact.py` & `cmind-1.5.1/cmind/artifact.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/automation.py` & `cmind-1.5.1/cmind/automation.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/cli.py` & `cmind-1.5.1/cmind/cli.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/config.py` & `cmind-1.5.1/cmind/config.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/core.py` & `cmind-1.5.1/cmind/core.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/index.py` & `cmind-1.5.1/cmind/index.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/net.py` & `cmind-1.5.1/cmind/net.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/automation/README.md` & `cmind-1.5.1/cmind/repo/automation/automation/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/automation/module.py` & `cmind-1.5.1/cmind/repo/automation/automation/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/automation/module_dummy.py` & `cmind-1.5.1/cmind/repo/automation/automation/module_dummy.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/automation/module_misc.py` & `cmind-1.5.1/cmind/repo/automation/automation/module_misc.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/ck/README.md` & `cmind-1.5.1/cmind/repo/automation/ck/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/ck/module.py` & `cmind-1.5.1/cmind/repo/automation/ck/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/core/README.md` & `cmind-1.5.1/cmind/repo/automation/core/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/core/module.py` & `cmind-1.5.1/cmind/repo/automation/core/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/repo/README.md` & `cmind-1.5.1/cmind/repo/automation/repo/README.md`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo/automation/repo/module.py` & `cmind-1.5.1/cmind/repo/automation/repo/module.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repo.py` & `cmind-1.5.1/cmind/repo.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/repos.py` & `cmind-1.5.1/cmind/repos.py`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/cmind/utils.py` & `cmind-1.5.1/cmind/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -807,41 +807,42 @@
        * dict1 (dict): dict1 passed through the function
 
     """
 
     a = i['dict1']
     b = i['dict2']
 
-    append_lists = i.get('append_lists', False)
-    append_unique = i.get('append_unique', False)
-
-    ignore_keys = i.get('ignore_keys',[])
-
-    for k in b:
-        if k in ignore_keys:
-            continue
-        v = b[k]
-        if type(v) is dict:
-            if k not in a:
-                a.update({k: b[k]})
-            elif type(a[k]) == dict:
-                merge_dicts({'dict1': a[k], 'dict2': b[k], 'append_lists':append_lists})
+    if a != b:
+        append_lists = i.get('append_lists', False)
+        append_unique = i.get('append_unique', False)
+
+        ignore_keys = i.get('ignore_keys',[])
+
+        for k in b:
+            if k in ignore_keys:
+                continue
+            v = b[k]
+            if type(v) is dict:
+                if k not in a:
+                    a.update({k: b[k]})
+                elif type(a[k]) == dict:
+                    merge_dicts({'dict1': a[k], 'dict2': b[k], 'append_lists':append_lists})
+                else:
+                    a[k] = b[k]
+            elif type(v) is list:
+                if not append_lists or k not in a:
+                   a[k] = []
+                for y in v:
+                    if append_unique:
+                        if y not in a[k]:
+                            a[k].append(y)
+                    else:
+                        a[k].append(y)
             else:
                 a[k] = b[k]
-        elif type(v) is list:
-            if not append_lists or k not in a:
-               a[k] = []
-            for y in v:
-                if append_unique:
-                    if y not in a[k]:
-                        a[k].append(y)
-                else:
-                    a[k].append(y)
-        else:
-            a[k] = b[k]
 
     return {'return': 0, 'dict1': a}
 
 ###########################################################################
 def process_meta_for_inheritance(i):
     """
     Check CM meta description for inheritance and update it if needed ("_base":"automation::artifact").
```

### Comparing `cmind-1.5.0/cmind.egg-info/PKG-INFO` & `cmind-1.5.1/cmind.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmind
-Version: 1.5.0
+Version: 1.5.1
 Summary: cmind
 Home-page: https://github.com/mlcommons/ck/tree/master/cm
 Author: Grigori Fursin
 Author-email: Grigori.Fursin@cTuning.org
 License: Apache 2.0
 Description: [![PyPI version](https://badge.fury.io/py/cmind.svg)](https://pepy.tech/project/cmind)
         [![Python Version](https://img.shields.io/badge/python-3+-blue.svg)](https://github.com/mlcommons/ck/tree/master/cm/cmind)
@@ -12,18 +12,20 @@
         [![License](https://img.shields.io/badge/License-Apache%202.0-green)](LICENSE.md)
         
         [![CM test](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm.yml)
         [![CM script automation features test](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml/badge.svg)](https://github.com/mlcommons/ck/actions/workflows/test-cm-script-features.yml)
         
         ### About
         
-        *Our mission is to connect academia and industry to solve the real-world problems by facilitating reproducible research 
-        and bridging the growing gap between research and production - [see our ACM REP'23 keynote to learn more about our vision](https://doi.org/10.5281/zenodo.8105339)!*
+        ***We deeply believe in the power of open science and open source to solve the world's most challenging problems.
+           That's why we are developing a common automation and reproducibility language to help connect academia and industry,
+           facilitate reproducible research and bridge the growing gap between research and production - 
+           [see our ACM REP'23 keynote for more details](https://doi.org/10.5281/zenodo.8105339)!***
         
-        [Collective Mind scripting language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
+        [Collective Mind automation and reproducibility language (MLCommons CM)](https://github.com/mlcommons/ck/tree/master/cm/cmind) 
         is a part of the [MLCommons Collective Knowledge project](https://github.com/mlcommons/ck).
         It is motivated by the [feedback from researchers and practitioners](https://learning.acm.org/techtalks/reproducibility)
         when reproducing experiments from more than 150 research papers and validating them in the real world - 
         there is a need for a common, human-readable and technology-agnostic interface to manage and run any software project 
         on any platform with any software, hardware, and data.
         
         CM is being developed by the [public MLCommons task force on automation and reproducibility](https://github.com/mlcommons/ck/blob/master/docs/taskforce.md)
```

### Comparing `cmind-1.5.0/cmind.egg-info/SOURCES.txt` & `cmind-1.5.1/cmind.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cmind-1.5.0/setup.py` & `cmind-1.5.1/setup.py`

 * *Files identical despite different names*

