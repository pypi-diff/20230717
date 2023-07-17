# Comparing `tmp/nanoprep-ffm-0.0.8.tar.gz` & `tmp/nanoprep-ffm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoprep-ffm-0.0.8.tar", last modified: Thu Apr 27 13:17:46 2023, max compression
+gzip compressed data, was "nanoprep-ffm-0.0.9.tar", last modified: Thu May 11 12:41:47 2023, max compression
```

## Comparing `nanoprep-ffm-0.0.8.tar` & `nanoprep-ffm-0.0.9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1068 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/LICENSE
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/__init__.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     5425 2023-04-25 04:19:21.000000 nanoprep-ffm-0.0.8/NanoPreP/__main__.py
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/aligntools/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/aligntools/__init__.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     2824 2023-04-08 08:29:17.000000 nanoprep-ffm-0.0.8/NanoPreP/aligntools/edlibAligner.py
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/optimize/
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-18 09:25:14.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/__init__.py
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     6211 2023-04-20 12:53:07.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/__main__.py
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     2066 2023-04-19 12:45:10.000000 nanoprep-ffm-0.0.8/NanoPreP/optimize/argParser.py
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/paramtools/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/__init__.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     3802 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/argParser.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1592 2023-04-07 06:07:14.000000 nanoprep-ffm-0.0.8/NanoPreP/paramtools/paramsets.py
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/preptools/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     9302 2023-04-14 07:32:11.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/Annotator.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1287 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/Processor.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/__init__.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1332 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/preptools/polyFinder.py
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.551259 nanoprep-ffm-0.0.8/NanoPreP/seqtools/
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      545 2023-04-07 05:16:25.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/FastqIO.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     6094 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/SeqFastq.py
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/NanoPreP/seqtools/__init__.py
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/PKG-INFO
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)    10255 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.8/README.md
-drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/PKG-INFO
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      760 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/SOURCES.txt
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        1 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/dependency_links.txt
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      104 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/entry_points.txt
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       26 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/requires.txt
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        9 2023-04-27 13:17:46.000000 nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/top_level.txt
--rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       38 2023-04-27 13:17:46.555259 nanoprep-ffm-0.0.8/setup.cfg
--rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      776 2023-04-27 13:17:22.000000 nanoprep-ffm-0.0.8/setup.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1068 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/LICENSE
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     5425 2023-04-25 04:19:21.000000 nanoprep-ffm-0.0.9/NanoPreP/__main__.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/aligntools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/aligntools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     2824 2023-04-08 08:29:17.000000 nanoprep-ffm-0.0.9/NanoPreP/aligntools/edlibAligner.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/optimize/
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-18 09:25:14.000000 nanoprep-ffm-0.0.9/NanoPreP/optimize/__init__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     6209 2023-05-02 08:43:23.000000 nanoprep-ffm-0.0.9/NanoPreP/optimize/__main__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)     2066 2023-04-19 12:45:10.000000 nanoprep-ffm-0.0.9/NanoPreP/optimize/argParser.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/paramtools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/paramtools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     3802 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/paramtools/argParser.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1592 2023-04-07 06:07:14.000000 nanoprep-ffm-0.0.9/NanoPreP/paramtools/paramsets.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/preptools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     9309 2023-05-11 12:35:22.000000 nanoprep-ffm-0.0.9/NanoPreP/preptools/Annotator.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1287 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/preptools/Processor.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/preptools/__init__.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     1332 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/preptools/polyFinder.py
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/NanoPreP/seqtools/
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      545 2023-04-07 05:16:25.000000 nanoprep-ffm-0.0.9/NanoPreP/seqtools/FastqIO.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)     6094 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/seqtools/SeqFastq.py
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/NanoPreP/seqtools/__init__.py
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/PKG-INFO
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)    10255 2023-04-06 14:17:53.000000 nanoprep-ffm-0.0.9/README.md
+drwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)        0 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)    10585 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/PKG-INFO
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      760 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/SOURCES.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        1 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/dependency_links.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)      104 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/entry_points.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       26 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/requires.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)        9 2023-05-11 12:41:47.000000 nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/top_level.txt
+-rw-rw-r--   0 b05b01002  (1002) b05b01002  (1002)       38 2023-05-11 12:41:47.668823 nanoprep-ffm-0.0.9/setup.cfg
+-rwxrwxr-x   0 b05b01002  (1002) b05b01002  (1002)      776 2023-05-11 12:41:13.000000 nanoprep-ffm-0.0.9/setup.py
```

### Comparing `nanoprep-ffm-0.0.8/LICENSE` & `nanoprep-ffm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/__main__.py` & `nanoprep-ffm-0.0.9/NanoPreP/__main__.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/aligntools/edlibAligner.py` & `nanoprep-ffm-0.0.9/NanoPreP/aligntools/edlibAligner.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/optimize/__main__.py` & `nanoprep-ffm-0.0.9/NanoPreP/optimize/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,19 +214,19 @@
         }
         #code {
             font-family: Monospace;
             font-size: 14px;
         }
     </style>
     <body>
-        <div id="title">NanoPreP-optimizer</div>
+        <div id="title">NanoPreP-optimize</div>
         <div class="gap-20"></div>
         <div>%(plot)</div>
         <div id="text">Command line:</div>
-        <div id="code">nanoprep-optimizer %(args)</div>
+        <div id="code">nanoprep-optimize %(args)</div>
         <div class="gap-10"></div>
         <div id="text">Parameters:</div>
         <div id="code">%(params)</div>
     </body>
 </html>"""
         out = out.replace("%(args)", " ".join(sys.argv[1:]))
         out = out.replace("%(plot)", fig.to_html())
```

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/optimize/argParser.py` & `nanoprep-ffm-0.0.9/NanoPreP/optimize/argParser.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/paramtools/argParser.py` & `nanoprep-ffm-0.0.9/NanoPreP/paramtools/argParser.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/paramtools/paramsets.py` & `nanoprep-ffm-0.0.9/NanoPreP/paramtools/paramsets.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/preptools/Annotator.py` & `nanoprep-ffm-0.0.9/NanoPreP/preptools/Annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from NanoPreP.seqtools.SeqFastq import SeqFastq, SeqAnnot
 from NanoPreP.aligntools.edlibAligner import edlibAligner as aligner
 from NanoPreP.preptools.polyFinder import polyFinder
 from collections import namedtuple
-from typing import Tuple
+from typing import Tuple, Dict
 import re
 
 class Annotator(object):
     def __init__(
         self,
         p5_sense: str,
         p3_sense: str,
@@ -150,15 +150,15 @@
         self.p3_sense = p3_sense
         self.p5_anti = p5_anti if p5_anti else SeqFastq.reverse_complement_static(p3_sense)
         self.p3_anti = p3_anti if p3_anti else SeqFastq.reverse_complement_static(p5_sense)
         self.isl5 = isl5
         self.isl3 = isl3
         return 
     
-    def alignPNbests(self, read: SeqFastq, plen: int, nbests: int) -> dict[str,namedtuple]:
+    def alignPNbests(self, read: SeqFastq, plen: int, nbests: int) -> Dict[str, namedtuple]:
         """_summary_
 
         Args:
             read (SeqFastq): _description_
             plen (int): _description_
             nbests (int): _description_
```

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/preptools/Processor.py` & `nanoprep-ffm-0.0.9/NanoPreP/preptools/Processor.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/preptools/polyFinder.py` & `nanoprep-ffm-0.0.9/NanoPreP/preptools/polyFinder.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/seqtools/FastqIO.py` & `nanoprep-ffm-0.0.9/NanoPreP/seqtools/FastqIO.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/NanoPreP/seqtools/SeqFastq.py` & `nanoprep-ffm-0.0.9/NanoPreP/seqtools/SeqFastq.py`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/PKG-INFO` & `nanoprep-ffm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoprep-ffm
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data
 Home-page: https://github.com/Woodformation1136/NanoPreP
 Author: Chia-Chen Chu
 Author-email: jerry955071@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nanoprep-ffm-0.0.8/README.md` & `nanoprep-ffm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/PKG-INFO` & `nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoprep-ffm
-Version: 0.0.8
+Version: 0.0.9
 Summary: A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data
 Home-page: https://github.com/Woodformation1136/NanoPreP
 Author: Chia-Chen Chu
 Author-email: jerry955071@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `nanoprep-ffm-0.0.8/nanoprep_ffm.egg-info/SOURCES.txt` & `nanoprep-ffm-0.0.9/nanoprep_ffm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanoprep-ffm-0.0.8/setup.py` & `nanoprep-ffm-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 
 # read README.md
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoprep-ffm",
-    version="0.0.8",
+    version="0.0.9",
     author="Chia-Chen Chu",
     author_email="jerry955071@gmail.com",
     description="A fully-equipped, fast, and memory-efficient pre-processor for ONT transcriptomic data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Woodformation1136/NanoPreP",
     packages=find_packages(),
-    install_requires=["edlib>=1.3.8", "numpy", "plotly"],
+    install_requires=["edlib==1.3.8", "numpy", "plotly"],
     entry_points={
         "console_scripts": [
             "nanoprep = NanoPreP.__main__:main",
             "nanoprep-optimize = NanoPreP.optimize.__main__:main"
         ]
     }
 )
```

