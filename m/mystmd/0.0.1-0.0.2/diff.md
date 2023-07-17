# Comparing `tmp/mystmd-0.0.1.tar.gz` & `tmp/mystmd-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mystmd-0.0.1.tar", last modified: Wed Jun 14 14:50:42 2023, max compression
+gzip compressed data, was "mystmd-0.0.2.tar", last modified: Mon Jul 17 19:13:12 2023, max compression
```

## Comparing `mystmd-0.0.1.tar` & `mystmd-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-06-14 14:50:42.767375 mystmd-0.0.1/
--rw-r--r--   0 stevejpurves   (501) staff       (20)     1088 2023-06-14 14:45:59.000000 mystmd-0.0.1/LICENSE
--rw-r--r--   0 stevejpurves   (501) staff       (20)      663 2023-06-14 14:50:42.767437 mystmd-0.0.1/PKG-INFO
--rw-r--r--   0 stevejpurves   (501) staff       (20)       72 2023-06-14 14:49:58.000000 mystmd-0.0.1/README.md
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-06-14 14:50:42.766773 mystmd-0.0.1/mystmd/
--rw-r--r--   0 stevejpurves   (501) staff       (20)       70 2023-06-14 14:45:59.000000 mystmd-0.0.1/mystmd/__init__.py
--rw-r--r--   0 stevejpurves   (501) staff       (20)       31 2023-06-14 14:45:59.000000 mystmd-0.0.1/mystmd/version.py
-drwxr-xr-x   0 stevejpurves   (501) staff       (20)        0 2023-06-14 14:50:42.767278 mystmd-0.0.1/mystmd.egg-info/
--rw-r--r--   0 stevejpurves   (501) staff       (20)      663 2023-06-14 14:50:42.000000 mystmd-0.0.1/mystmd.egg-info/PKG-INFO
--rw-r--r--   0 stevejpurves   (501) staff       (20)      193 2023-06-14 14:50:42.000000 mystmd-0.0.1/mystmd.egg-info/SOURCES.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)        1 2023-06-14 14:50:42.000000 mystmd-0.0.1/mystmd.egg-info/dependency_links.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)        7 2023-06-14 14:50:42.000000 mystmd-0.0.1/mystmd.egg-info/top_level.txt
--rw-r--r--   0 stevejpurves   (501) staff       (20)      114 2023-06-14 14:50:42.767678 mystmd-0.0.1/setup.cfg
--rw-r--r--   0 stevejpurves   (501) staff       (20)     1021 2023-06-14 14:50:08.000000 mystmd-0.0.1/setup.py
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.779007 mystmd-0.0.2/
+-rw-r--r--   0 franklin   (501) staff       (20)     1088 2023-07-17 16:52:14.000000 mystmd-0.0.2/LICENSE
+-rw-r--r--   0 franklin   (501) staff       (20)       55 2023-07-17 17:15:36.000000 mystmd-0.0.2/MANIFEST.in
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 19:13:12.779106 mystmd-0.0.2/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)       78 2023-07-04 19:42:57.000000 mystmd-0.0.2/README.md
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.766081 mystmd-0.0.2/dist/
+-rwxr-xr-x   0 franklin   (501) staff       (20) 13079621 2023-07-15 00:22:54.000000 mystmd-0.0.2/dist/myst.cjs
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.778373 mystmd-0.0.2/mystmd.egg-info/
+-rw-r--r--   0 franklin   (501) staff       (20)      815 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/PKG-INFO
+-rw-r--r--   0 franklin   (501) staff       (20)      255 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/SOURCES.txt
+-rw-r--r--   0 franklin   (501) staff       (20)        1 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/dependency_links.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       45 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/entry_points.txt
+-rw-r--r--   0 franklin   (501) staff       (20)       10 2023-07-17 19:13:12.000000 mystmd-0.0.2/mystmd.egg-info/top_level.txt
+drwxr-xr-x   0 franklin   (501) staff       (20)        0 2023-07-17 19:13:12.778681 mystmd-0.0.2/mystmd_py/
+-rw-r--r--   0 franklin   (501) staff       (20)        0 2023-07-17 16:26:51.000000 mystmd-0.0.2/mystmd_py/__init__.py
+-rw-r--r--   0 franklin   (501) staff       (20)      829 2023-07-17 17:28:11.000000 mystmd-0.0.2/mystmd_py/main.py
+-rw-r--r--   0 franklin   (501) staff       (20)      901 2023-07-17 19:13:12.779548 mystmd-0.0.2/setup.cfg
+-rw-r--r--   0 franklin   (501) staff       (20)       37 2023-07-17 16:56:36.000000 mystmd-0.0.2/setup.py
```

### Comparing `mystmd-0.0.1/LICENSE` & `mystmd-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2020 ExecutableBookProject
+Copyright (c) 2023 ExecutableBookProject
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mystmd-0.0.1/PKG-INFO` & `mystmd-0.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.1
-Summary: MyST Markdown
-Home-page: https://myst-tools.org
-Author: Steve Purves
-Author-email: stevejpurves@gmail.com
-Classifier: Development Status :: 4 - Beta
+Version: 0.0.2
+Summary: Command line tools for MyST Markdown
+Home-page: https://github.com/executablebooks/mystmd
+Author: Franklin Koch
+License: MIT
+Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 License-File: LICENSE
-
-# mystmd
-
-Markedly Restructured Text - [myst.tools](https://myst.tools)
```

### Comparing `mystmd-0.0.1/mystmd.egg-info/PKG-INFO` & `mystmd-0.0.2/mystmd.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: mystmd
-Version: 0.0.1
-Summary: MyST Markdown
-Home-page: https://myst-tools.org
-Author: Steve Purves
-Author-email: stevejpurves@gmail.com
-Classifier: Development Status :: 4 - Beta
+Version: 0.0.2
+Summary: Command line tools for MyST Markdown
+Home-page: https://github.com/executablebooks/mystmd
+Author: Franklin Koch
+License: MIT
+Keywords: markdown,latex,writing-software,scientific-visualization,pdf-generation,science-research
+Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: JavaScript
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Text Processing :: Markup
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Information Technology
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
+Classifier: Topic :: Scientific/Engineering
+Requires-Python: >=3.6
 License-File: LICENSE
-
-# mystmd
-
-Markedly Restructured Text - [myst.tools](https://myst.tools)
```

