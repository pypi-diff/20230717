# Comparing `tmp/trackplot-0.2.6.tar.gz` & `tmp/trackplot-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trackplot-0.2.6.tar", last modified: Mon Jun 12 01:54:28 2023, max compression
+gzip compressed data, was "trackplot-0.2.7.tar", max compression
```

## Comparing `trackplot-0.2.6.tar` & `trackplot-0.2.7.tar`

### file list

```diff
@@ -1,57 +1,39 @@
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.437972 trackplot-0.2.6/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1558 2022-12-13 02:20:58.000000 trackplot-0.2.6/LICENSE
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-12 01:54:28.437698 trackplot-0.2.6/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)      381 2023-05-05 02:05:07.000000 trackplot-0.2.6/Pipfile
--rw-r--r--   0 zhangyiming   (501) staff       (20)    95598 2023-05-30 08:48:54.000000 trackplot-0.2.6/Pipfile.lock
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6508 2023-05-30 02:06:13.000000 trackplot-0.2.6/README.md
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1136 2023-06-12 01:53:15.000000 trackplot-0.2.6/pyproject.toml
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-06-12 01:54:28.438048 trackplot-0.2.6/setup.cfg
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1445 2023-06-12 01:53:15.000000 trackplot-0.2.6/setup.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.414211 trackplot-0.2.6/trackplot/
--rw-r--r--   0 zhangyiming   (501) staff       (20)       38 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/__init__.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.428011 trackplot-0.2.6/trackplot/anno/
--rw-r--r--   0 zhangyiming   (501) staff       (20)      371 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/AxLabel.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1545 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/anno/theme.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.432356 trackplot-0.2.6/trackplot/base/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7428 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/CoordinateMap.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4330 2023-02-25 15:51:21.000000 trackplot-0.2.6/trackplot/base/GenomicLoci.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3546 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8883 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Protein.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8580 2023-06-12 01:40:46.000000 trackplot-0.2.6/trackplot/base/ReadDepth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     8943 2023-02-25 03:49:51.000000 trackplot-0.2.6/trackplot/base/Readder.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1200 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Stroke.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3572 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/Transcript.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     7995 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/base/pyUniprot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    43565 2023-06-12 01:53:38.000000 trackplot-0.2.6/trackplot/cli.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.433500 trackplot-0.2.6/trackplot/conf/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     4745 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/DomainSetting.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1329 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/config.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3803 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/conf/drawing.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.437394 trackplot-0.2.6/trackplot/file/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6341 2023-02-26 15:22:54.000000 trackplot-0.2.6/trackplot/file/ATAC.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    12911 2023-02-28 04:50:41.000000 trackplot-0.2.6/trackplot/file/Bam.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1481 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/BedGraph.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1515 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Bigwig.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     2779 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Depth.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1237 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Fasta.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     3639 2023-02-25 16:01:18.000000 trackplot-0.2.6/trackplot/file/File.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6415 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/HiCMatrixTrack.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)      966 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/Junction.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1020 2023-02-25 15:59:51.000000 trackplot-0.2.6/trackplot/file/Motif.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    20328 2023-02-27 13:19:33.000000 trackplot-0.2.6/trackplot/file/ReadSegments.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    21606 2023-05-05 03:09:45.000000 trackplot-0.2.6/trackplot/file/Reference.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)        0 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/file/__init__.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    45357 2023-05-06 03:20:22.000000 trackplot-0.2.6/trackplot/plot.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)    52203 2023-02-25 15:55:34.000000 trackplot-0.2.6/trackplot/plot_func.py
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6403 2023-02-25 03:47:37.000000 trackplot-0.2.6/trackplot/plot_tests.py
-drwxr-xr-x   0 zhangyiming   (501) staff       (20)        0 2023-06-12 01:54:28.426488 trackplot-0.2.6/trackplot.egg-info/
--rw-r--r--   0 zhangyiming   (501) staff       (20)     6694 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/PKG-INFO
--rw-r--r--   0 zhangyiming   (501) staff       (20)     1201 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       49 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/entry_points.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)        1 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/not-zip-safe
--rw-r--r--   0 zhangyiming   (501) staff       (20)      151 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/requires.txt
--rw-r--r--   0 zhangyiming   (501) staff       (20)       10 2023-06-12 01:54:28.000000 trackplot-0.2.6/trackplot.egg-info/top_level.txt
+-rw-r--r--   0        0        0     1558 2022-12-13 02:20:58.685741 trackplot-0.2.7/LICENSE
+-rw-r--r--   0        0        0    12535 2023-07-17 11:41:19.355720 trackplot-0.2.7/README.md
+-rw-r--r--   0        0        0     1136 2023-07-17 09:57:45.537804 trackplot-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0       38 2023-02-25 03:47:37.462308 trackplot-0.2.7/trackplot/__init__.py
+-rw-r--r--   0        0        0      371 2023-02-25 03:47:37.462598 trackplot-0.2.7/trackplot/anno/AxLabel.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.462676 trackplot-0.2.7/trackplot/anno/__init__.py
+-rw-r--r--   0        0        0     1545 2023-02-25 03:47:37.462914 trackplot-0.2.7/trackplot/anno/theme.py
+-rw-r--r--   0        0        0     7428 2023-02-25 03:47:37.463212 trackplot-0.2.7/trackplot/base/CoordinateMap.py
+-rw-r--r--   0        0        0     4425 2023-07-12 04:37:03.080978 trackplot-0.2.7/trackplot/base/GenomicLoci.py
+-rw-r--r--   0        0        0     3546 2023-02-25 03:47:37.463862 trackplot-0.2.7/trackplot/base/Junction.py
+-rw-r--r--   0        0        0     8881 2023-06-30 06:55:19.943274 trackplot-0.2.7/trackplot/base/Protein.py
+-rw-r--r--   0        0        0     8580 2023-06-12 01:40:46.369104 trackplot-0.2.7/trackplot/base/ReadDepth.py
+-rw-r--r--   0        0        0     8933 2023-07-17 11:32:19.681424 trackplot-0.2.7/trackplot/base/Readder.py
+-rw-r--r--   0        0        0     1368 2023-07-12 04:37:03.081411 trackplot-0.2.7/trackplot/base/Stroke.py
+-rw-r--r--   0        0        0     3572 2023-02-25 03:47:37.465151 trackplot-0.2.7/trackplot/base/Transcript.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.465222 trackplot-0.2.7/trackplot/base/__init__.py
+-rw-r--r--   0        0        0     7991 2023-06-30 06:55:19.957076 trackplot-0.2.7/trackplot/base/pyUniprot.py
+-rw-r--r--   0        0        0    43297 2023-07-17 11:32:19.682002 trackplot-0.2.7/trackplot/cli.py
+-rw-r--r--   0        0        0     4745 2023-02-25 03:47:37.466182 trackplot-0.2.7/trackplot/conf/DomainSetting.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.466260 trackplot-0.2.7/trackplot/conf/__init__.py
+-rw-r--r--   0        0        0     1330 2023-07-17 11:32:19.682283 trackplot-0.2.7/trackplot/conf/config.py
+-rw-r--r--   0        0        0     3803 2023-02-25 03:47:37.466652 trackplot-0.2.7/trackplot/conf/drawing.py
+-rw-r--r--   0        0        0     6341 2023-02-26 15:22:54.255231 trackplot-0.2.7/trackplot/file/ATAC.py
+-rw-r--r--   0        0        0    21597 2023-07-17 12:26:02.906206 trackplot-0.2.7/trackplot/file/Annotation.py
+-rw-r--r--   0        0        0    12907 2023-06-30 06:55:19.953467 trackplot-0.2.7/trackplot/file/Bam.py
+-rw-r--r--   0        0        0     1481 2023-02-25 03:47:37.467519 trackplot-0.2.7/trackplot/file/BedGraph.py
+-rw-r--r--   0        0        0     1515 2023-02-25 03:47:37.467778 trackplot-0.2.7/trackplot/file/Bigwig.py
+-rw-r--r--   0        0        0     2779 2023-02-25 03:47:37.468030 trackplot-0.2.7/trackplot/file/Depth.py
+-rw-r--r--   0        0        0     1233 2023-06-30 06:55:19.939595 trackplot-0.2.7/trackplot/file/Fasta.py
+-rw-r--r--   0        0        0     3539 2023-07-14 02:17:54.487679 trackplot-0.2.7/trackplot/file/File.py
+-rw-r--r--   0        0        0     6413 2023-06-30 06:55:19.949884 trackplot-0.2.7/trackplot/file/HiCMatrixTrack.py
+-rw-r--r--   0        0        0      966 2023-02-25 03:47:37.469300 trackplot-0.2.7/trackplot/file/Junction.py
+-rw-r--r--   0        0        0     1020 2023-02-25 15:59:51.023722 trackplot-0.2.7/trackplot/file/Motif.py
+-rw-r--r--   0        0        0    20423 2023-07-17 11:32:19.682598 trackplot-0.2.7/trackplot/file/ReadSegments.py
+-rw-r--r--   0        0        0        0 2023-02-25 03:47:37.470458 trackplot-0.2.7/trackplot/file/__init__.py
+-rw-r--r--   0        0        0    47253 2023-07-17 12:28:36.876308 trackplot-0.2.7/trackplot/plot.py
+-rw-r--r--   0        0        0    52344 2023-07-17 12:28:14.643398 trackplot-0.2.7/trackplot/plot_func.py
+-rw-r--r--   0        0        0     6403 2023-02-25 03:47:37.471775 trackplot-0.2.7/trackplot/plot_tests.py
+-rw-r--r--   0        0        0    13892 1970-01-01 00:00:00.000000 trackplot-0.2.7/PKG-INFO
```

### Comparing `trackplot-0.2.6/LICENSE` & `trackplot-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/pyproject.toml` & `trackplot-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trackplot"
-version = "0.2.6"
+version = "0.2.7"
 description = "The trackplot is a tool for visualizing various next-generation sequencing (NGS) data, including DNA-seq, RNA-seq, single-cell RNA-seq and full-length sequencing datasets. https://sashimi.readthedocs.io/"
 authors = ["ygidtu <ygidtu@gmail.com>"]
 license = "BSD-3"
 readme = "README.md"
 packages = [{include = "trackplot"}]
 
 [tool.poetry.dependencies]
```

### Comparing `trackplot-0.2.6/trackplot/anno/theme.py` & `trackplot-0.2.7/trackplot/anno/theme.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/base/CoordinateMap.py` & `trackplot-0.2.7/trackplot/base/CoordinateMap.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/base/GenomicLoci.py` & `trackplot-0.2.7/trackplot/base/GenomicLoci.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,16 @@
         self.strand = strand
 
     def __str__(self):
         u"""
         convert this to string
         :return:
         """
+        if self.strand == "*":
+            return f"{self.chromosome}:{self.start}-{self.end}"
         return f"{self.chromosome}:{self.start}-{self.end}:{self.strand}"
 
     def __iter__(self):
         for i in range(self.start, self.end+1):
             yield i
 
     def __gt__(self, other):
```

### Comparing `trackplot-0.2.6/trackplot/base/Junction.py` & `trackplot-0.2.7/trackplot/base/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/base/Protein.py` & `trackplot-0.2.7/trackplot/base/Protein.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
                     boundary_for_iter.append(line.end)
 
                 if line.transcript_id in transcript_id and \
                         line.feature == "CDS":
                     cds_dict[line.transcript_id].append(line)
 
             except KeyError as err:
-                logger.warning(err)
+                logger.debug(err)
 
         cds_contain = {}
         start_site = float('Inf')
         end_site = float('-Inf')
 
         if len(cds_dict) != 0:
```

### Comparing `trackplot-0.2.6/trackplot/base/ReadDepth.py` & `trackplot-0.2.7/trackplot/base/ReadDepth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/base/Readder.py` & `trackplot-0.2.7/trackplot/base/Readder.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             logger.info(f"try to create index for {path}")
             pysam.index(path)
 
         with pysam.AlignmentFile(path, 'rb') as bam_file:
             try:
                 relevant_reads = bam_file.fetch(reference=chrom, start=region.start, end=region.end)
             except ValueError as err:
-                logger.warning(err)
+                # logger.debug(err)
                 relevant_reads = cls.__modify_chrom__(region, bam_file)
 
             for read in relevant_reads:
                 if read.is_qcfail or read.is_unmapped or read.is_duplicate:
                     continue
 
                 yield read, __get_strand__(read, library=library)
@@ -130,15 +130,15 @@
                     region.start,
                     region.end,
                     parser=pysam.asGTF() if not bed else pysam.asBed())
             except ValueError:
                 try:
                     iter_ = cls.__modify_chrom__(region, r, parser=pysam.asGTF() if not bed else pysam.asBed())
                 except ValueError as err:
-                    logger.warning("please check the input region and gtf files")
+                    logger.debug("please check the input region and gtf files")
                     logger.error(err)
                     raise err
 
             for record in iter_:
                 yield record
 
     @classmethod
@@ -149,15 +149,15 @@
             logger.error(f"Please install pyBigWig properly to enable bigWig support: {err}")
             sys.exit(1)
 
         with pyBigWig.open(path) as r:
             try:
                 return r.values(region.chromosome, region.start, region.end + 1)
             except RuntimeError as e:
-                logger.warning(e)
+                logger.debug(e)
 
                 logger.info("may be caused by the mismatch of chromosome")
                 if region.chromosome.startswith("chr"):
                     return r.values(region.chromosome.replace("chr", ""), region.start, region.end + 1)
                 else:
                     return r.values("chr" + region.chromosome, region.start, region.end + 1)
 
@@ -167,21 +167,21 @@
             import pyBigWig
         except ImportError as err:
             logger.error(f"Please install pyBigWig properly to enable bigWig support: {err}")
             sys.exit(1)
 
         with pyBigWig.open(path) as r:
             if not r.isBigBed():
-                logger.warning(f"{path} don't look like bigbed file.")
+                logger.debug(f"{path} don't look like bigbed file.")
                 yield from []
             else:
                 try:
                     iter_ = r.entries(region.chromosome, region.start, region.end + 1)
                 except RuntimeError as e:
-                    logger.warning(e)
+                    logger.debug(e)
 
                     logger.info("may be caused by the mismatch of chromosome")
                     if region.chromosome.startswith("chr"):
                         iter_ = r.entries(
                             region.chromosome.replace("chr", "") if region.chromosome != "chrM" else "MT",
                             region.start,
                             region.end + 1
@@ -212,15 +212,15 @@
             else:
                 try:
                     iter_ = r.fetch(region.chromosome, region.start, region.end, parser=pysam.asTuple())
                 except ValueError:
                     try:
                         iter_ = cls.__modify_chrom__(region, r, parser=pysam.asTuple())
                     except ValueError as err:
-                        logger.warning("please check the input region and gtf files")
+                        logger.debug("please check the input region and gtf files")
                         logger.error(err)
                         raise err
 
             for record in iter_:
                 yield record
 
     @classmethod
```

### Comparing `trackplot-0.2.6/trackplot/base/Stroke.py` & `trackplot-0.2.7/trackplot/base/Stroke.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,25 @@
 u"""
 
 """
 from trackplot.base.GenomicLoci import GenomicLoci
 
 
 class Stroke(object):
+    __slots__ = ["start", "end", "color", "label", "origin"]
 
-    __slots__ = ["start", "end", "color", "label"]
-    def __init__(self, start: int, end: int, color: str = "red", label: str = ""):
+    def __init__(self, start: int, end: int, color: str = "red", label: str = "", origin: str = ""):
         self.start = start
         self.end = end
         self.color = color
         self.label = label
+        self.origin = origin if origin else f"{start}-{end}@{color}-{label}"
+
+    def __str__(self):
+        return self.origin
 
     @property
     def center(self) -> float:
         return (self.end + self.start) / 2
 
     @classmethod
     def create(cls, stroke: str, region: GenomicLoci, default_color: str = "red"):
@@ -35,14 +39,13 @@
             label = ""
             if len(i) > 1:
                 i = i[-1].split("-")
                 color = i[0]
 
                 if len(i) > 1:
                     label = i[-1]
-
-            res.append(Stroke(sites[0], sites[-1], color, label))
+            res.append(Stroke(sites[0], sites[-1], color, label, "@".join(i)))
         return res
 
 
 if __name__ == "__main__":
     pass
```

### Comparing `trackplot-0.2.6/trackplot/base/Transcript.py` & `trackplot-0.2.7/trackplot/base/Transcript.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/base/pyUniprot.py` & `trackplot-0.2.7/trackplot/base/pyUniprot.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,18 +159,18 @@
                         raise f"Timeout for {request_url}."
             else:
                 if isinstance(xml_dic['accession'], list):
                     return xml_dic['accession'][0]
                 return xml_dic['accession']
 
         except ExpatError:
-            logger.warning(f"Timeout or no domain information found, id: {self.ui}.")
+            logger.debug(f"Timeout or no domain information found, id: {self.ui}.")
             return None
         except KeyError:
-            # logger.warning(f"Timeout or no domain information found, id: {self.ui}.")
+            # logger.debug(f"Timeout or no domain information found, id: {self.ui}.")
             return None
 
         # this set may be empty
         if not current_uniprot_id:
             return None
 
         # if there were multiple protein id, return first.
```

### Comparing `trackplot-0.2.6/trackplot/cli.py` & `trackplot-0.2.7/trackplot/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,23 @@
 import gzip
 import os
 import sys
 from multiprocessing import cpu_count
 from typing import Optional, Dict, Set, Tuple
 
 import click
-import matplotlib as mpl
 from click_option_group import optgroup
 from loguru import logger
 
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.conf.config import CLUSTERING_METHOD, COLORS, COLORMAP, DISTANCE_METRIC, IMAGE_TYPE, NORMALIZATION
 from trackplot.file.ATAC import ATAC
 from trackplot.plot import Plot
 
-__version__ = "0.2.6"
+__version__ = "0.2.7"
 __author__ = "ygidtu & Ran Zhou"
 __email__ = "ygidtu@gmail.com"
 
 
 def decode_region(region: str):
     regions = region.split(":")
 
@@ -46,15 +45,14 @@
                  label: Optional[str] = None,
                  group: Optional[str] = None,
                  exon_focus: Optional[str] = None,
                  library: str = "fru",
                  trans: Optional[str] = None,
                  depth: Optional[int] = None,
                  tad: Optional[str] = None):
-
         self.path = os.path.abspath(os.path.expanduser(path))
 
         if not os.path.exists(self.path):
             raise FileNotFoundError(f"{self.path} not found.")
 
         self.label = label if label else os.path.basename(path)
         self.group = group
@@ -250,15 +248,16 @@
     except FileNotFoundError as err:
         logger.error(f"{infile} -> {err}")
         exit(1)
 
 
 @click.command(context_settings=dict(help_option_names=['-h', '--help']), no_args_is_help=True)
 @click.version_option(__version__, message="Current version %(version)s")
-@click.option("--debug", is_flag=True, help="enable debug level log")
+@click.option("--verbose", is_flag=True, default=False, help="enable debug level log")
+@click.option("--logfile", type=click.Path(), help="save log info into file")
 @click.option("-e", "--event", type=click.STRING, required=True,
               help="Event range eg: chr1:100-200:+")
 @optgroup.group("Common input files configuration")
 @optgroup.option("--color-factor", default=1, type=click.IntRange(min=1),
                  help="Index of column with color levels (1-based); "
                       "NOTE: LUAD|red -> LUAD while be labeled in plots and red while be the fill color",
                  show_default=True)
@@ -288,38 +287,38 @@
                       "(speed up rendering and produce smaller files), only affects pdf, svg and PS")
 @optgroup.option("--height", default=1, type=float,
                  help="The height of single subplot, default adjust image height by content", show_default=True)
 @optgroup.option("--width", default=10, type=click.IntRange(min=0, clamp=True),
                  help="The width of output file, default adjust image width by content", show_default=True)
 @optgroup.option("--backend", type=click.STRING, default="Agg", help="Recommended backend", show_default=True)
 @optgroup.group("Reference settings")
-@optgroup.option("-r", "--reference", type=click.Path(exists=True),
+@optgroup.option("-r", "--annotation", type=click.Path(exists=True),
                  help="Path to gtf file, both transcript and exon tags are necessary")
 @optgroup.option("--interval", type=click.Path(exists=True),
                  help="Path to list of interval files in bed format, "
                       "1st column is path to file, 2nd column is the label [optional]")
 @optgroup.option("--show-id", is_flag=True, show_default=True, help="Whether show gene id or gene name")
 @optgroup.option("--show-exon-id", is_flag=True, show_default=True, help="Whether show gene id or gene name")
 @optgroup.option("--no-gene", is_flag=True, type=click.BOOL, show_default=True,
                  help="Do not show gene id next to transcript id")
 @optgroup.option("--domain", default=False, is_flag=True, type=click.BOOL, show_default=True,
-                 help="Add domain information into reference track")
+                 help="Add domain information into annotation track")
 @optgroup.option("--proxy", default=None, type=click.STRING,
                  help="The http or https proxy for EBI/Uniprot requests,"
                       "if `--domain` is True, eg: http://127.0.0.1:1080")
 @optgroup.option("--timeout", default=10, type=click.IntRange(min=1, clamp=True),
                  show_default=True,
                  help="The requests timeout when `--domain` is True.")
 @optgroup.option("--local-domain", default="", is_flag=False, type=click.STRING, show_default=True,
-                 help="Load local domain folder and load into reference track, download from "
+                 help="Load local domain folder and load into annotation track, download from "
                       "https://hgdownload.soe.ucsc.edu/gbdb/hg38/uniprot/")
 @optgroup.option("--domain-include", default=None, type=click.STRING, show_default=True,
-                 help="Which domain will be included in reference plot")
+                 help="Which domain will be included in annotation plot")
 @optgroup.option("--domain-exclude", default=None, type=click.STRING, show_default=True,
-                 help="Which domain will be excluded in reference plot")
+                 help="Which domain will be excluded in annotation plot")
 @optgroup.option("--remove-empty", is_flag=True, type=click.BOOL, show_default=True,
                  help="Whether to plot empty transcript")
 @optgroup.option("--transcripts-to-show", default="", show_default=True,
                  help="Which transcript to show, transcript name or id in gtf file, eg: transcript1,transcript2")
 @optgroup.option("--choose-primary", is_flag=True, type=click.BOOL, show_default=True,
                  help="Whether choose primary transcript to plot.")
 @optgroup.option("--ref-color", default="black", type=click.STRING,
@@ -468,25 +467,25 @@
 @optgroup.option("--motif-region", type=click.STRING, default="",
                  help="The region of motif to plot in start-end format", show_default=True)
 @optgroup.option("--motif-width", type=click.FLOAT, default=0.8,
                  help="The width of ATCG characters", show_default=True)
 @optgroup.group("Layout settings")
 @optgroup.option("--n-y-ticks", default=4, type=click.IntRange(min=0, clamp=True),
                  help="The number of ticks of y-axis")
-@optgroup.option("--distance-ratio", type=click.FLOAT, default=0.1,
+@optgroup.option("--distance-ratio", type=click.FLOAT, default=0,
                  help="The distance between transcript label and transcript line", show_default=True)
-@optgroup.option("--reference-scale", type=click.FLOAT, default=.25,
-                 help="The size of reference plot in final plot", show_default=True)
+@optgroup.option("--annotation-scale", type=click.FLOAT, default=.25,
+                 help="The size of annotation plot in final plot", show_default=True)
 @optgroup.option("--stroke-scale", type=click.FLOAT, default=.25,
                  help="The size of stroke plot in final image", show_default=True)
 @optgroup.group("Overall settings")
 @optgroup.option("--font-size", default=8, type=click.IntRange(min=1, clamp=True),
                  help="The font size of x, y-axis and so on")
 @optgroup.option("--reverse-minus", default=False, is_flag=True, type=click.BOOL,
-                 help="Whether to reverse strand of bam/reference file")
+                 help="Whether to reverse strand of bam/annotation file")
 @optgroup.option("--hide-y-label", default=False, is_flag=True, type=click.BOOL,
                  help="Whether hide y-axis label")
 @optgroup.option("--same-y", default=False, is_flag=True, type=click.BOOL,
                  help="Whether different density/line plots shared same y-axis boundaries")
 @optgroup.option("--same-y-sc", default=False, is_flag=True, type=click.BOOL,
                  help="Similar with --same-y, but only shared same y-axis boundaries between same single cell files")
 @optgroup.option('--log', type=click.Choice(["0", "2", "10", "zscore"]), default="0",
@@ -495,79 +494,66 @@
 @optgroup.option("--font", type=click.STRING, default=None, help="Fonts", show_default=True)
 def main(**kwargs):
     u"""
     Welcome to use trackplot
     \f
     """
     logger.remove()
-    logger.add(sys.stderr, level="INFO" if not kwargs["debug"] else "DEBUG")
+    logger.add(sys.stderr, level="DEBUG" if kwargs["verbose"] else "INFO")
+    logger.debug("DEBUG" if kwargs["verbose"] else "INFO")
 
     # print warning info about backend
     if (kwargs["domain"] or kwargs["local_domain"]) and kwargs["backend"].lower() != "cairo":
-        logger.warning(f"{kwargs['backend']} backend may have problems with small domain, "
-                       f"if there is any please try cairo backend instead.")
+        logger.debug(f"{kwargs['backend']} backend may have problems with small domain, "
+                     f"if there is any please try cairo backend instead.")
 
     if kwargs["raster"] and kwargs["heatmap"] and kwargs["backend"].lower() == "cairo":
-        logger.warning(f"{kwargs['backend']} backend may have problems with rasterized heatmap, "
-                       f"if there is any, please try another backend instead.")
-
-    try:
-        mpl.use(kwargs["backend"])
-    except ImportError as err:
-        if kwargs["backend"].lower() == "cairo":
-            logger.warning("Cairo backend required cairocffi installed")
-            logger.warning("Switch back to Agg backend")
-        else:
-            logger.warning(f"backend error, switch back to Agg: {err}")
-        mpl.use("Agg")
-
-    mpl.rcParams['pdf.fonttype'] = 42
-
-    if kwargs["font"]:
-        mpl.rcParams['font.family'] = kwargs["font"]
+        logger.debug(f"{kwargs['backend']} backend may have problems with rasterized heatmap, "
+                     f"if there is any, please try another backend instead.")
 
     for k, v in kwargs.items():
         logger.debug(f"{k} => {v}")
 
     if kwargs["included_junctions"] is not None:
         included_junctions = set([sj.strip() for sj in kwargs["included_junctions"].split(',')])
     else:
         included_junctions = {}
 
-    p = Plot()
+    p = Plot(logfile=kwargs["logfile"], font_family=kwargs["font"], backend=kwargs["backend"])
 
     region = decode_region(kwargs["event"])
     p.set_region(region=region)
     p.add_customized_junctions(kwargs["customized_junction"])
 
     barcodes, sc_colors = {}, {}
     if kwargs.get("barcode") and os.path.exists(kwargs.get("barcode")):
         barcodes, sc_colors = load_barcodes(kwargs.get("barcode"))
 
     size_factors = {}
 
-    # add reference
+    # add annotation
+    # print(kwargs.keys())
     for key in kwargs.keys():
         if key in IMAGE_TYPE and kwargs[key] and os.path.exists(kwargs[key]):
-            logger.debug(f"add {key} {kwargs[key]}")
-            if key == "reference":
-                p.set_reference(kwargs["reference"],
-                                show_gene=not kwargs["no_gene"],
-                                color=kwargs["ref_color"],
-                                remove_empty_transcripts=kwargs["remove_empty"],
-                                choose_primary=kwargs["choose_primary"],
-                                font_size=kwargs["font_size"],
-                                show_id=kwargs["show_id"],
-                                show_exon_id=kwargs["show_exon_id"],
-                                transcripts=kwargs["transcripts_to_show"],
-                                add_domain=kwargs["domain"],
-                                local_domain=kwargs["local_domain"],
-                                domain_include=kwargs["domain_include"],
-                                domain_exclude=kwargs["domain_exclude"]
-                                )
+            if key == "annotation":
+                print("set_annotation")
+                p.set_annotation(kwargs["annotation"],
+                                 show_gene=not kwargs["no_gene"],
+                                 color=kwargs["ref_color"],
+                                 remove_empty_transcripts=kwargs["remove_empty"],
+                                 choose_primary=kwargs["choose_primary"],
+                                 font_size=kwargs["font_size"],
+                                 show_id=kwargs["show_id"],
+                                 show_exon_id=kwargs["show_exon_id"],
+                                 transcripts=kwargs["transcripts_to_show"],
+                                 add_domain=kwargs["domain"],
+                                 local_domain=kwargs["local_domain"],
+                                 domain_include=kwargs["domain_include"],
+                                 domain_exclude=kwargs["domain_exclude"]
+                                 )
             elif key == "interval":
                 for f in process_file_list(kwargs[key], key):
                     p.add_interval(f.path, f.label)
             elif key == "density":
                 for f in process_file_list(kwargs[key], key):
                     bcs = barcodes.get(f.path, barcodes.get(f.name, barcodes.get(f.label, {})))
                     if bcs and f.category in ["bam", "atac"]:
@@ -734,15 +720,14 @@
                               show_y_label=not kwargs["hide_y_label"],
                               deletion_ignore=True if kwargs["del_ratio_ignore"] == 1.0 else False,
                               del_ratio_ignore=kwargs["del_ratio_ignore"],
                               exon_focus=f.exon_focus
                               )
             elif key == "hic":
                 for f in process_file_list(kwargs[key], "hic"):
-
                     p.add_hic(
                         f.path,
                         category=f.category,
                         label=f.label,
                         log_trans=f.trans,
                         tad=f.tad,
                         depth=f.depth,
@@ -779,15 +764,15 @@
         kwargs["output"],
         width=kwargs["width"],
         height=kwargs["height"],
         dpi=kwargs["dpi"],
         raster=kwargs["raster"],
         intron_scale=kwargs["intron_scale"],
         exon_scale=kwargs["exon_scale"],
-        reference_scale=kwargs["reference_scale"],
+        annotation_scale=kwargs["annotation_scale"],
         stroke_scale=kwargs["stroke_scale"],
         same_y=kwargs["same_y"],
         same_y_sc=kwargs.get("same_y_sc", False),
         remove_duplicate_umi=kwargs["remove_duplicate_umi"],
         threshold=kwargs["threshold"],
         sc_height_ratio={
             "heatmap": kwargs["sc_heatmap_height_ratio"],
@@ -796,12 +781,11 @@
         distance_between_label_axis=kwargs["distance_ratio"],
         included_junctions=included_junctions,
         n_jobs=kwargs.get("process", 1),
         normalize_format=kwargs.get("normalize_format"),
         fill_step=kwargs.get("fill_step", "post"),
         smooth_bin=kwargs["smooth_bin"]
     )
-    logger.info("DONE")
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `trackplot-0.2.6/trackplot/conf/DomainSetting.py` & `trackplot-0.2.7/trackplot/conf/DomainSetting.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/conf/config.py` & `trackplot-0.2.7/trackplot/conf/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 
-IMAGE_TYPE = ["reference", "interval", "density", "heatmap", "line", "igv", "hic", "motif"]
+IMAGE_TYPE = ["annotation", "interval", "density", "heatmap", "line", "igv", "hic", "motif"]
 
 COLORS = ["#A0C807", "#0084D1", '#db5f57', '#dbc257', '#91db57', '#57db80', '#57d3db', '#5770db', '#a157db', '#db57b2']
 COLORMAP = [
     'Blues', 'Greens', 'Oranges', 'Reds', 'Greys', 'Purples',
     'YlOrBr', 'YlOrRd', 'OrRd', 'PuRd', 'RdPu', 'BuPu',
     'GnBu', 'PuBu', 'YlGnBu', 'PuBuGn', 'BuGn', 'YlGn',
     'binary', 'gist_yarg', 'gist_gray', 'gray', 'bone',
```

### Comparing `trackplot-0.2.6/trackplot/conf/drawing.py` & `trackplot-0.2.7/trackplot/conf/drawing.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/ATAC.py` & `trackplot-0.2.7/trackplot/file/ATAC.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/Bam.py` & `trackplot-0.2.7/trackplot/file/Bam.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                             umis[barcode] = {}
 
                         # filter reads with duplicate umi by barcode
                         if read.has_tag(self.umi_tag):
                             umi = read.get_tag(self.umi_tag)
                         else:
                             if scatac_alert:
-                                logger.warning(f"Is {self.path} an scATAC-seq bam? There is no {self.umi_tag}")
+                                logger.debug(f"Is {self.path} an scATAC-seq bam? There is no {self.umi_tag}")
                                 scatac_alert = False
                             umi = read.query_name
 
                         if umi in umis[barcode].keys() and umis[barcode][umi] != hash(read.query_name):
                             continue
 
                         if len(umis[barcode]) == 0:
@@ -262,15 +262,15 @@
                             junction_name = Junction(region.chromosome, cur_start, cur_end, strand)
 
                             if junction_name not in spanned_junctions:
                                 spanned_junctions[junction_name] = 0
 
                             spanned_junctions[junction_name] = spanned_junctions[junction_name] + 1
                         except ValueError as err:
-                            logger.warning(err)
+                            logger.debug(err)
                             continue
                 start = read.reference_start + 1 if read.reference_start + 1 > region.start else region.start
                 end = read.reference_end + 1 if read.reference_end + 1 < region.end else region.end
                 if strand == "+" and 0 <= start - region.start < len(plus):
                     site_plus[end - region.start] += 1
                 elif strand == "-" and 0 <= end - region.start < len(minus):
                     site_minus[start - region.start] += 1
```

### Comparing `trackplot-0.2.6/trackplot/file/BedGraph.py` & `trackplot-0.2.7/trackplot/file/BedGraph.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/Bigwig.py` & `trackplot-0.2.7/trackplot/file/Bigwig.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/Depth.py` & `trackplot-0.2.7/trackplot/file/Depth.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/Fasta.py` & `trackplot-0.2.7/trackplot/file/Fasta.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,29 +17,29 @@
     def __init__(self, path: str):
         super().__init__(path)
         assert os.path.exists(path), f"{path} not exists"
 
     @classmethod
     def create(cls, path: str):
         if not os.path.exists(path + ".fai"):
-            logger.warning(f"{path}.fai not exists, try to create it")
+            logger.debug(f"{path}.fai not exists, try to create it")
 
             pysam.faidx(path)
 
         return cls(path)
 
     def load(self, region: GenomicLoci, **kwargs):
         u"""
         load sequence from a fasta file
         :param region:
         :return:
         """
 
         if not os.path.exists(self.path + ".fai"):
-            logger.warning(f"{self.path}.fai not exists, try to create it")
+            logger.debug(f"{self.path}.fai not exists, try to create it")
             pysam.faidx(self.path)
 
         self.data = {}
         with pysam.FastaFile(self.path) as r:
             for i, j in zip(
                     range(self.region.start, self.region.end + 1),
                     r.fetch(region.chromosome, region.start, region.end + 1)
```

### Comparing `trackplot-0.2.6/trackplot/file/File.py` & `trackplot-0.2.7/trackplot/file/File.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 u"""
 The parent object of input files
 """
 from copy import deepcopy
-from loguru import logger
 from typing import Optional, Set, List, Dict
 
 
 class File(object):
 
     __slots__ = "path", "data", "label", "region", "log_trans", "title", "is_single_cell"
 
@@ -52,17 +51,16 @@
         return self.path == other.path and self.label == other.label and self.title == other.title
 
     def transform(self):
         if self.data is not None:
             if isinstance(self.data, list):
                 try:
                     [x.transform(self.log_trans) for x in self.data]
-                except AttributeError as err:
-                    # should be Reads
-                    logger.debug(f"one of current data should be Reads: {err}: {[type(x) for x in self.data]}")
+                except AttributeError as _:
+                    # should be Reads, Reads will cause this error, ignore it
                     pass
             elif not isinstance(self.data, dict):
                 self.data.transform(self.log_trans)
 
 
 def __set_barcodes__(barcodes: Optional[List[str]]) -> Dict:
     u"""
```

### Comparing `trackplot-0.2.6/trackplot/file/HiCMatrixTrack.py` & `trackplot-0.2.7/trackplot/file/HiCMatrixTrack.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         matrix = hic.matrix[idx, :][:, idx]
         region_len = region_end - region_start
 
         current_depth = min(self.depth, int(region_len * 1.25))
         depth_in_bins = max(1, int(1.5 * region_len / hic.getBinSize()))
 
         if current_depth < self.depth:
-            logger.warning(f"The depth was set to {self.depth} which is more than 125% "
+            logger.debug(f"The depth was set to {self.depth} which is more than 125% "
                            f"of the region plotted. The depth will be set "
                            f"to {current_depth}.\n")
             # remove from matrix all data points that are not visible.
             matrix = matrix - sparse.triu(matrix, k=depth_in_bins, format='csr')
 
         matrix = np.asarray(matrix.todense().astype(float))
```

### Comparing `trackplot-0.2.6/trackplot/file/Junction.py` & `trackplot-0.2.7/trackplot/file/Junction.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/Motif.py` & `trackplot-0.2.7/trackplot/file/Motif.py`

 * *Files identical despite different names*

### Comparing `trackplot-0.2.6/trackplot/file/ReadSegments.py` & `trackplot-0.2.7/trackplot/file/ReadSegments.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,16 @@
         )
 
     def get_index(self):
         u"""
         get a nested list which presents the order of plot
         :return:
         """
+        import warnings
+        warnings.simplefilter(action='ignore', category=FutureWarning)
         assert self.meta is not None, f"Not found meta information, please `load` first."
         for ind in self.meta.groupby(['y_loci'])['list_index'].apply(list).tolist()[::-1]:
             yield ind
 
     def set_region(self,
                    chromosome,
                    start,
```

### Comparing `trackplot-0.2.6/trackplot/file/Reference.py` & `trackplot-0.2.7/trackplot/file/Annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.base.Protein import CdsProtein
 from trackplot.base.Readder import Reader
 from trackplot.base.Transcript import Transcript
 from trackplot.file.File import File
 
 
-class Reference(File):
+class Annotation(File):
     u"""
     The reference file, support gtf and gff format
     """
 
     __slots__ = "category", "add_domain", "domain", \
         "interval_file", "add_local_domain", "local_domain", "proxy", "timeout", \
                 "domain_include", "domain_exclude"
@@ -331,15 +331,15 @@
                 pysam.tabix_index(
                     output_gtf,
                     preset="gff",
                     force=True,
                     keep_original=True
                 )
             except OSError as err:
-                logger.warning(f"Guess gtf needs to be sorted: {err}")
+                logger.debug(f"Guess gtf needs to be sorted: {err}")
 
                 sorted_gtf = re.sub(r"\.gtf(.gz)?$", "", input_gtf) + ".sorted.gtf.gz"
                 if os.path.exists(sorted_gtf) and os.path.exists(sorted_gtf + ".tbi"):
                     return sorted_gtf
 
                 cls.sort_gtf(input_gtf, sorted_gtf)
                 pysam.tabix_index(sorted_gtf, preset="gff", force=True, keep_original=True)
@@ -434,17 +434,17 @@
                     start=read.reference_start + 1 if read.reference_start + 1 > region.start else region.start,
                     end=read.reference_end + 1 if read.reference_end + 1 < region.end else region.end,
                     strand=strand,
                     exons=exons_in_read
                 )
                 transcripts[t] = transcripts.get(t, 0) + 1
         except IOError as err:
-            logger.warning(f"There is no .bam file at {self.path}: {err}")
+            logger.debug(f"There is no .bam file at {self.path}: {err}")
         except ValueError as err:
-            logger.warning(f"{self.path}: {err}")
+            logger.debug(f"{self.path}: {err}")
 
         return sorted([x for x, y in transcripts.items() if y > threshold_of_reads])
 
     def __load_bed__(self, region: GenomicLoci) -> List[Transcript]:
         transcripts = []
         try:
             for rec in Reader.read_gtf(self.path, region=region, bed=True):
@@ -492,17 +492,17 @@
                 )
                 if read.start < self.region.start or read.end > self.region.end:
                     continue
 
                 transcripts.append(read)
 
         except IOError as err:
-            logger.warning(f"There is no .bed file at {self.path}: {err}")
+            logger.debug(f"There is no .bed file at {self.path}: {err}")
         except ValueError as err:
-            logger.warning(f"{self.path}: {err}")
+            logger.debug(f"{self.path}: {err}")
         return transcripts
 
     def load(self, region: GenomicLoci, threshold_of_reads: int = 0, **kwargs):
         u"""
         Load transcripts inside of region
         :param region: target region
         :param threshold_of_reads: used for bam file, only kept reads with minimum frequency
```

### Comparing `trackplot-0.2.6/trackplot/plot.py` & `trackplot-0.2.7/trackplot/plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Set
 
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 from matplotlib.backends.backend_pdf import FigureCanvasPdf
 
+from trackplot.file.ATAC import ATAC
 from trackplot.file.Bam import Bam
 from trackplot.file.BedGraph import Bedgraph
 from trackplot.file.Bigwig import Bigwig
 from trackplot.file.Depth import Depth
 from trackplot.file.Fasta import Fasta
 from trackplot.file.Junction import load_custom_junction
 from trackplot.file.Motif import Motif
@@ -147,36 +148,58 @@
     u"""
     this class is the main framework of sashimi
     """
 
     __slots__ = [
         "__n_objs__", "region", "sites",
         "focus", "stroke", "events",
-        "sequence", "reference", "graph_coords",
+        "sequence", "annotation", "graph_coords",
         "plots", "params", "junctions", "link"
     ]
 
-    def __init__(self):
+    def __init__(self,
+                 logfile: Optional[str] = None,
+                 backend: Optional[str] = None,
+                 font_family: Optional[str] = None):
         u"""
         init this class
         """
         self.__n_objs__ = 0
         self.region = None
         self.sites = {}
         self.focus = {}
         self.stroke = []
         self.events = None
         self.sequence = None
-        self.reference = None
+        self.annotation = None
         self.graph_coords = None
         self.plots = []
         self.params = {}
         self.junctions = {}
         self.link = []
 
+        if logfile:
+            logger.add(logfile, level="TRACE")
+
+        # print warning info about backend
+        if backend:
+            try:
+                plt.switch_backend(backend)
+            except ImportError as err:
+                if backend.lower() == "cairo":
+                    logger.debug("Cairo backend required cairocffi installed")
+                    logger.debug("Switch back to Agg backend")
+                else:
+                    logger.debug(f"backend error, switch back to Agg: {err}")
+                plt.switch_backend("Agg")
+
+        plt.rcParams['pdf.fonttype'] = 42
+        if font_family:
+            plt.rcParams['font.family'] = font_family
+
     @property
     def chrom(self) -> Optional[str]:
         if self.region:
             return self.region.chrom
 
     @property
     def start(self) -> Optional[int]:
@@ -191,16 +214,16 @@
     @property
     def strand(self) -> Optional[str]:
         if self.region:
             return self.region.strand
 
     @property
     def exons(self) -> Optional[List[List[int]]]:
-        if self.reference:
-            return self.reference.exons
+        if self.annotation:
+            return self.annotation.exons
 
     def set_region(self, chromosome: str = "",
                    start: int = 0, end: int = 0,
                    strand: str = "+",
                    region: Optional[GenomicLoci] = None):
         u"""
         change the plot region
@@ -216,14 +239,15 @@
     def add_sites(self, sites):
         u"""
         highlight specific sites
         :param sites: string in 100,200 format or int
         :return:
         """
         assert self.region is not None, f"please set plot region first."
+        logger.info(f"add sites: {sites}")
         if sites is not None:
             if isinstance(sites, str):
                 sites = [int(x) for x in sites.split(",")]
 
                 for s in sites:
                     s = s - self.start
                     if s not in self.sites.keys():
@@ -234,35 +258,37 @@
                 sites = sites - self.start
                 if sites not in self.sites.keys():
                     self.sites[sites] = "blue"
                 else:
                     self.sites[sites] = "red"
         return self
 
-    def add_focus(self, focus: Optional[str], start: int = 0, end: int = 0):
+    def add_focus(self, focus: Optional[str] = None, start: int = 0, end: int = 0):
         u"""
         set focus region
         :param focus: string in 100-200:300-400
         :param start: start site
         :param end: end site
         :return:
         """
         assert self.region is not None, f"please set plot region first."
         if focus:
+            logger.info(f"add focus: {focus}")
             for site in focus.split(":"):
                 site = sorted([int(x) - self.start for x in site.split("-")])
                 if site[0] < 0:
                     site[0] = 0
 
                 if site[-1] > len(self):
                     site[-1] = len(self)
 
                 self.focus[site[0]] = max(site[1], self.focus.get(site[0], -1))
 
         if 0 < start < end:
+            logger.info(f"add focus: {start}-{end}")
             self.focus[start] = max(end, self.focus.get(start, -1))
         return self
 
     def add_stroke(
             self,
             stroke: Optional[str] = None,
             start: int = 0,
@@ -277,17 +303,19 @@
         :param end: end site of stroke
         :param label: label of stroke
         :param color: color of stroke
         :return:
         """
         assert self.region is not None, f"please set plot region first."
         if stroke:
+            logger.info(f"add stroke: {stroke}")
             self.stroke += Stroke.create(stroke, self.region)
 
         if 0 < start < end:
+            logger.info(f"add stroke: {start}-{end}")
             self.stroke.append(Stroke(start - self.start, end - self.end, color, label))
         return self
 
     def add_links(
             self,
             link: Optional[str] = None,
             start: int = 0,
@@ -301,85 +329,89 @@
         :param start: start site of stroke
         :param end: end site of stroke
         :param label: label of stroke
         :param color: color of stroke
         :return:
         """
         assert self.region is not None, f"please set plot region first."
+
         if link:
+            logger.info(f"add link: {link}")
             self.link.append(Stroke.create(link, self.region, default_color=color))
 
         if 0 < start < end:
+            logger.info(f"add link: {start}-{end}")
             self.link.append([Stroke(start - self.start, end - self.end, color, label)])
         return self
 
     def set_sequence(self, fasta: str):
         u"""
         set sequence info for
         :param fasta: path to indexed fasta file
         :return:
         """
         logger.info(f"fetch sequence from {fasta}")
         self.sequence = Fasta.create(fasta)
         return self
 
-    def set_reference(self, gtf: str,
-                      add_domain: bool = False,
-                      local_domain: Optional[str] = False,
-                      domain_include: Optional[str] = False,
-                      domain_exclude: Optional[str] = False,
-                      interval: Optional[str] = None,
-                      interval_label: Optional[str] = None,
-                      transcripts: Optional[List[str]] = None,
-                      remove_empty_transcripts: bool = False,
-                      choose_primary: bool = False,
-                      color: Optional[str] = "black",
-
-                      # transcripts related parameters
-                      font_size: int = 5,
-                      show_gene: bool = False,
-                      show_id: bool = False,
-                      exon_width: float = .3,
-                      show_exon_id: bool = False,
-                      theme: str = "blank"
-                      ):
+    def set_annotation(self, gtf: str,
+                       add_domain: bool = False,
+                       local_domain: Optional[str] = False,
+                       domain_include: Optional[str] = False,
+                       domain_exclude: Optional[str] = False,
+                       interval: Optional[str] = None,
+                       interval_label: Optional[str] = None,
+                       transcripts: Optional[List[str]] = None,
+                       remove_empty_transcripts: bool = False,
+                       choose_primary: bool = False,
+                       color: Optional[str] = "black",
+
+                       # transcripts related parameters
+                       font_size: int = 5,
+                       show_gene: bool = True,
+                       show_id: bool = False,
+                       exon_width: float = .3,
+                       show_exon_id: bool = False,
+                       theme: str = "blank",
+                       **kwargs
+                       ):
         u"""
         add transcripts to this region
         :param gtf: the path of gtf file
-        :param add_domain: whether add domain information into reference plot
-        :param local_domain: add a local domain file into reference plot
-        :param domain_exclude: the domain will be included in reference plot
-        :param domain_include: the domain will be excluded in reference plot
+        :param add_domain: whether add domain information into annotation plot
+        :param local_domain: add a local domain file into annotation plot
+        :param domain_exclude: the domain will be included in annotation plot
+        :param domain_include: the domain will be excluded in annotation plot
         :param interval: the path of interval annotation file, such as polyAsites
         :param interval_label: the label of current interval annotation file
         :param font_size: the size of transcript id, name
         :param transcripts: the list of name or ids of transcripts to draw
         :param remove_empty_transcripts: whether to remove transcripts without any exons
         :param choose_primary: whether to choose primary transcript for each gene
         :param color: the color of exons
         :param show_gene: whether to show gene name/id
         :param show_id: show gene id or gene name
         :param theme: the theme of transcript
         :param exon_width: the height of exons
         :param show_exon_id: whether to show exon id
         :return:
         """
-        logger.info(f"set reference file to {gtf}")
-        self.reference = Reference.create(
+        logger.info(f"set annotation file to {gtf}")
+        self.annotation = Annotation.create(
             gtf,
             add_domain=add_domain,
             add_local_domain=local_domain,
             domain_exclude=domain_exclude,
             domain_include=domain_include
         )
 
         if interval and interval_label:
-            self.reference.add_interval(interval, interval_label)
+            self.add_interval(interval, interval_label)
 
-        self.params["reference"] = {
+        self.params["annotation"] = {
             "transcripts": transcripts,
             "remove_empty_transcripts": remove_empty_transcripts,
             "choose_primary": choose_primary,
             "color": color,
             "font_size": font_size,
             "show_gene": show_gene,
             "show_id": show_id,
@@ -387,16 +419,17 @@
             "show_exon_id": show_exon_id,
             "theme": theme
         }
 
         return self
 
     def add_interval(self, interval: str, interval_label: str):
-        assert self.reference is not None, "please set_reference first."
-        self.reference.add_interval(interval, interval_label)
+        assert self.annotation is not None, "please set_annotation first."
+        logger.info(f"add interval: {interval} - {interval_label}")
+        self.annotation.add_interval(interval, interval_label)
         return self
 
     def __init_input_file__(self, path: str,
                             category: str = "bam",
                             label: Union[str, List[str]] = "",
                             title: str = "",
                             barcode: str = "",
@@ -417,14 +450,15 @@
                             # for ATAC
                             size_factor=None,
 
                             log_trans: Optional[str] = None,
                             ):
         self.__n_objs__ += 1
         path = os.path.expanduser(path)
+        logger.info(f"add {category} {label} {path}")
         if category == "bam":
             obj = Bam.create(
                 path,
                 label=label,
                 title=title,
                 barcodes=barcode_groups.get(barcode) if barcode_groups else None,
                 barcode_tag=barcode_tag,
@@ -552,15 +586,15 @@
             log_trans=log_trans
         )
 
         type_ = "density"
         if show_site_plot and category == "bam":
             type_ = "site-plot"
         elif show_site_plot:
-            logger.warning("show_site_plot only works with bam files")
+            logger.debug("show_site_plot only works with bam files")
 
         info = PlotInfo(obj=obj, type_=type_, category=category)
 
         new_obj = True
         for p in self.plots:
             if p.category == info.category:
                 for obj_ in p.obj:
@@ -973,29 +1007,29 @@
         return self.end - self.start + 1
 
     def copy(self):
         return deepcopy(self)
 
     def plot(self,
              output: Optional[str] = None,
-             reference_scale: Union[int, float] = .25,
+             annotation_scale: Union[int, float] = .25,
              stroke_scale: Union[int, float] = .25,
              dpi: int = 300,
              width: Union[int, float] = 0,
              height: Union[int, float] = 0,
              raster: bool = False,
              return_image: Optional[str] = None,
              sc_height_ratio: Optional[Dict[str, float]] = None,
              distance_between_label_axis: float = .3,
              n_jobs: int = 1, fill_step: str = "post",
              *args, **kwargs):
         u"""
         draw image
         :param output: if output is empty then show this image by plt.showfig
-        :param reference_scale: to adjust the size of reference plot
+        :param annotation_scale: to adjust the size of annotation plot
         :param stroke_scale: to adjust the size of stroke plot
         :param dpi: the dpi of saved plot
         :param width: the width of figure, if width == 0, the let matplotlib decide the size of image
         :param height: the height of figure, if height == 0, the let matplotlib decide the size of image
         :param raster: plot rasterizer site plot
         :param sc_height_ratio: adjust the relative height of single cell plots
         :param distance_between_label_axis: distance between y-axis label and y-axis ticks
@@ -1003,22 +1037,21 @@
         :param fill_step: post, pre or mid
         :param return_image: used for interactive ui
         """
         if sc_height_ratio is None:
             sc_height_ratio = {"density": .2, "heatmap": .2}
         assert self.region is not None, f"please set the plotting region first."
 
-        plots_n_rows = 1
-        plots_n_cols = 1
+        plots_n_rows, plots_n_cols = 1, 1
 
         height_ratio = []
-        if self.reference is not None:
-            logger.info("load reference")
-            self.reference.load(self.region, *args, **kwargs)
-            plots_n_rows += self.reference.len(scale=reference_scale)
+        if self.annotation is not None:
+            logger.info("load annotation")
+            self.annotation.load(self.region, *args, **kwargs)
+            plots_n_rows += self.annotation.len(scale=annotation_scale)
 
         if self.stroke:
             plots_n_rows += int(max(len(self.stroke) * stroke_scale, 1))
 
         if self.link:
             plots_n_rows += len(self.link)
 
@@ -1045,47 +1078,38 @@
                 self.plots = p.map(__load__, cmds)
 
         # count the plots size
         for p in self.plots:
             if n_jobs <= 1:
                 p.load(self.region, junctions=self.junctions.get(p.obj[0].label, {}), *args, **kwargs)
 
-            # for obj in p.obj:
-            #     if isinstance(obj, ReadSegment):
-            #         continue
-            #     if isinstance(obj, HiCTrack):
-            #         continue
-            #     obj.transform()
-
-            plots_n_rows += p.len(reference_scale)
+            plots_n_rows += p.len(annotation_scale)
             if p.type in ["heatmap", "hic"]:
                 plots_n_cols = 2
 
             if p.is_single_cell:
                 height_ratio.append(sc_height_ratio.get(p.type, 1))
             elif p.type == "igv":
-                height_ratio.append(p.len(reference_scale))
+                height_ratio.append(p.len(annotation_scale))
+            elif p.type == "site-plot":
+                height_ratio += [1, 1]
             else:
                 height_ratio.append(1)
 
+        height_ratio += [1 for _ in range(plots_n_rows - len(height_ratio))]
+
         logger.debug(f"plots n_rows={plots_n_rows}; n_cols = {plots_n_cols}")
         logger.info("init graph_coords")
         exon_scale = kwargs.get("exon_scale", 1)
         intron_scale = kwargs.get("intron_scale", .5)
         if plots_n_cols > 1 and intron_scale != 1:
-            logger.warning(f"heatmap require intron_scale = 1")
+            logger.debug(f"heatmap require intron_scale = 1")
             intron_scale = 1
 
-        self.graph_coords = init_graph_coords(
-            self.region, self.exons,
-            exon_scale=exon_scale,
-            intron_scale=intron_scale
-        )
-
-        height_ratio += [1 for _ in range(plots_n_rows - len(height_ratio))]
+        self.graph_coords = init_graph_coords(self.region, self.exons, exon_scale=exon_scale, intron_scale=intron_scale)
 
         if width and height:
             fig = plt.figure(figsize=[width, height * sum(height_ratio)], dpi=dpi)
         else:
             fig = plt.figure(dpi=dpi)
 
         if plots_n_cols > 1:
@@ -1106,24 +1130,28 @@
                             min_used_y_val[obj.path] = min(min(obj.data.wiggle), min_used_y_val.get(obj.path, 0))
                         else:
                             min_used_y_val[obj.path] = min(min(obj.data.minus), min_used_y_val.get(obj.path, 0))
 
         curr_idx = 0
         for p in self.plots:
             if p.type == "igv":
-                ax_var = plt.subplot(gs[curr_idx: curr_idx + p.len(reference_scale), 0])
+                ax_var = plt.subplot(gs[curr_idx: curr_idx + p.len(annotation_scale), 0])
             else:
                 ax_var = plt.subplot(gs[curr_idx, 0])
 
+            if curr_idx == 0:
+                ax_var.set_title(str(self.region), loc="left")
+
             max_y_val_, min_y_val_ = None, None
             if kwargs.get("same_y_sc") and p.obj[0].is_single_cell:
                 max_y_val_, min_y_val_ = max_used_y_val[p.obj[0].path], min_used_y_val[p.obj[0].path]
             elif kwargs.get("same_y"):
                 max_y_val_, min_y_val_ = max(max_used_y_val.values()), min(min_used_y_val.values())
 
+            logger.info(f"plotting {p.type} at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
             if p.type == "density":
                 plot_density(
                     ax=ax_var,
                     obj=p.obj[0],
                     graph_coords=self.graph_coords,
                     max_used_y_val=max_y_val_,
                     min_used_y_val=min_y_val_,
@@ -1149,24 +1177,22 @@
                     max_used_y_val=max_y_val_,
                     min_used_y_val=min_y_val_,
                     distance_between_label_axis=distance_between_label_axis,
                     raster=raster,
                     **self.params[p]
                 )
 
-                site_ax = plt.subplot(gs[curr_idx + 1, 0])
-
+                curr_idx += 1
                 plot_site_plot(
-                    site_ax, p.obj[0],
+                    plt.subplot(gs[curr_idx, 0]), p.obj[0],
                     graph_coords=self.graph_coords,
                     raster=raster,
                     distance_between_label_axis=distance_between_label_axis,
                     **self.params[p]
                 )
-                curr_idx += 1
             elif p.type == "heatmap":
                 plot_heatmap(
                     ax=ax_var,
                     cbar_ax=plt.subplot(gs[curr_idx, 1]),
                     data=p.data,
                     y_label=p.group,
                     graph_coords=self.graph_coords,
@@ -1202,59 +1228,66 @@
             # adjust indicator lines and focus background
             set_indicator_lines(ax=ax_var, sites=self.sites, graph_coords=self.graph_coords)
             set_focus(ax=ax_var, focus=self.focus, graph_coords=self.graph_coords)
 
             if p.type != "igv":
                 curr_idx += 1
             else:
-                curr_idx += p.len(reference_scale)
+                curr_idx += p.len(annotation_scale)
 
         if self.link:
+            logger.info(f"plotting links at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
             for link in self.link:
                 plot_links(ax=plt.subplot(gs[curr_idx:(curr_idx + 1), 0]),
                            data=link, graph_coords=self.graph_coords)
                 curr_idx += 1
 
         # draw x label
+        logger.info(f"plotting x-axis ticks at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
         set_x_ticks(
             ax=plt.subplot(gs[curr_idx, 0]), region=self.region,
             graph_coords=self.graph_coords,
             sequence=self.sequence.data if self.sequence else None,
             *args, **kwargs
         )
         curr_idx += 1
 
-        if self.reference is not None:
-            ax_var = plt.subplot(gs[curr_idx:curr_idx + self.reference.len(scale=reference_scale), 0])
-            plot_reference(ax=ax_var, obj=self.reference,
+        if self.annotation is not None:
+            logger.info(f"plotting annotation at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
+            ax_var = plt.subplot(gs[curr_idx:curr_idx + self.annotation.len(scale=annotation_scale), 0])
+            plot_annotation(ax=ax_var, obj=self.annotation,
                            graph_coords=self.graph_coords,
-                           plot_domain=self.reference.add_domain,
+                           plot_domain=self.annotation.add_domain,
                            distance_between_label_axis=distance_between_label_axis,
-                           **self.params["reference"])
+                           **self.params["annotation"])
 
             # adjust indicator lines and focus background
             set_indicator_lines(ax=ax_var, sites=self.sites, graph_coords=self.graph_coords)
             set_focus(ax=ax_var, focus=self.focus, graph_coords=self.graph_coords)
-            curr_idx += self.reference.len(scale=reference_scale)
+            curr_idx += self.annotation.len(scale=annotation_scale)
 
         if self.stroke:
+            logger.info(f"plotting stroke at idx: {curr_idx} with height_ratio: {height_ratio[curr_idx]}")
             ax_var = plt.subplot(gs[curr_idx:plots_n_rows, 0])
             plot_stroke(ax=ax_var, data=self.stroke, graph_coords=self.graph_coords, *args, **kwargs)
 
         if output:
+            logger.info(f"saving fig into {output}")
             fig.savefig(output, transparent=True, bbox_inches='tight')
         elif return_image:
             output = io.BytesIO()
             if return_image == "png":
                 FigureCanvasAgg(fig).print_png(output)
             elif return_image == "pdf":
                 FigureCanvasPdf(fig).print_pdf(output)
             return output
         else:
             plt.show()
 
         plt.close()
+
+        logger.info("Plot done")
         return self
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `trackplot-0.2.6/trackplot/plot_func.py` & `trackplot-0.2.7/trackplot/plot_func.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,18 @@
 from scipy.stats import gaussian_kde, zscore
 
 from trackplot.anno.theme import Theme
 from trackplot.base.GenomicLoci import GenomicLoci
 from trackplot.base.ReadDepth import ReadDepth
 from trackplot.base.Stroke import Stroke
 from trackplot.conf.config import CLUSTERING_METHOD, DISTANCE_METRIC
+from trackplot.file.Annotation import Annotation
 from trackplot.file.File import File
 from trackplot.file.HiCMatrixTrack import HiCTrack
 from trackplot.file.ReadSegments import ReadSegment
-from trackplot.file.Reference import Reference
-from trackplot.file.ATAC import ATAC
 
 
 def get_limited_index(num, length):
     u"""
     Created by Zhang yiming at 2018.12.19
     Due to the original author didn't draw any element out of provided range
     So the scripts will through a lot of IndexError
@@ -147,15 +146,15 @@
         log_trans: Optional[str] = None,
         nx_ticks: int = 4, font_size: int = 6, **kwargs):
     Theme.set_theme(ax, "blank")
     if graph_coords is None:
         graph_coords = init_graph_coords(region)
 
     # @2018.12.19 unnecessary text in figure
-    x_label = 'Genomic coordinate (%s), "%s" strand' % (region.chromosome, region.strand)
+    x_label = str(region)
 
     if log_trans:
         if log_trans in ["2", "10"]:
             log_trans = f"log{log_trans}"
         x_label = f"{x_label}, y axis is {log_trans} transformed"
 
     ax.hlines(y=0, xmin=0, xmax=max(graph_coords), color="black", lw=1)
@@ -191,45 +190,44 @@
             line_space[relative_i] = temp_txs
 
     for x, s in line_space.items():
         ax.vlines(x=x, ymin=-.5, ymax=0, color="black", lw=1)
         ax.text(x=x, y=-1, s=s, fontsize=font_size, ha="center", va="top")
 
     ax.set_ylim(-3.5, 1)
-    ax.set_xlim(0, max(graph_coords))
+    ax.set_xlim(min(graph_coords), max(graph_coords))
 
 
 def set_y_ticks(
         ax: mpl.axes.Axes,
         label: str,
         graph_coords: Union[Dict, np.array],
         max_used_y_val: Union[int, float],
         min_used_y_val: Optional[Union[int, float]] = None,
-        distance_between_label_axis: float = .1,
+        distance_between_label_axis: float = 0,
         n_y_ticks: int = 4,
         theme: str = "ticks",
         font_size: int = 5,
         show_y_label: bool = True,
         set_label_only: bool = False,
         y_axis_skip_zero: bool = True,
         **kwargs
 ):
     u"""
     The y ticks are formatted here
     @2019.03.31 add little check here to make sure the y-axis shows the real value
     """
     # set y ticks, y label and label
     Theme.set_theme(ax, theme)
-
+    ax.set_xlim(min(graph_coords), max(graph_coords))
     if min_used_y_val is None:
         min_used_y_val, _ = ax.get_ylim()
 
+    curr_y_tick_labels = []
     if not set_label_only:
-        ax.set_xlim(0, max(graph_coords))
-
         max_ = max_used_y_val
         plus = 0.2
         while max_ > 10:
             max_ /= 10
             plus /= 10
 
         plus = (max_used_y_val - min_used_y_val) * plus
@@ -242,15 +240,15 @@
         universal_y_ticks = pylab.linspace(min_used_y_val, 0, assign_ticks_y[0] + 1)
         for i in pylab.linspace(0, max_used_y_val, assign_ticks_y[1] + 1):
             universal_y_ticks = np.append(universal_y_ticks, i)
 
         # add zero into strand-aware plot
         universal_y_ticks = np.unique(np.append(universal_y_ticks, 0))
         universal_y_ticks = sorted(universal_y_ticks)
-        curr_y_tick_labels = []
+
         for lab in universal_y_ticks:
             if y_axis_skip_zero and lab == 0:
                 # Exclude label for 0
                 curr_y_tick_labels.append("")
             elif max_used_y_val < 1e-2:
                 curr_y_tick_labels.append(f"{Decimal(lab):.2E}")
             else:
@@ -264,17 +262,27 @@
         ax.yaxis.set_ticks_position('left')
 
     """
     Plot y labels
     @2018.12.20 using BAM label as y label
     @2019.01.04 change the standards of distance between y label and y-axis
     """
+
     if show_y_label:
+        def __dynamic_distance__(distance_between_label_axis: float, label: str, scale: int = 100) -> float:
+            if distance_between_label_axis != 0:
+                return -distance_between_label_axis
+
+            return max(0.01, math.ceil(len(label) / 10) * 10 / scale) * -1
+
+        curr_y_tick_labels = sorted(curr_y_tick_labels, key=lambda x: len(x), reverse=True)
         ax.text(
-            x=-1 * distance_between_label_axis * max(graph_coords),
+            x=__dynamic_distance__(
+                distance_between_label_axis, curr_y_tick_labels[0] if curr_y_tick_labels else ""
+            ) * max(graph_coords),
             y=(max_used_y_val + min_used_y_val) / 2,
             s=label, fontsize=font_size, ha="right"
         )
 
     if max_used_y_val is not None and min_used_y_val is not None:
         ax.set_ylim(ymin=min_used_y_val, ymax=max_used_y_val)
 
@@ -289,15 +297,15 @@
             left, right = graph_coords[left], graph_coords[right]
             fill_x = [left, right, right, left]
 
             y1, y2 = ax.get_ylim()
             fill_y = [y1, y1, y2, y2]
             ax.fill(fill_x, fill_y, alpha=0.1, color='grey')
         except IndexError as err:
-            logger.warning("focus region is out of bound: " + str(err))
+            logger.debug("focus region is out of bound: " + str(err))
 
 
 def set_indicator_lines(
         ax: mpl.axes.Axes,
         graph_coords: Union[Dict, np.array],
         sites: Dict[int, str],
         min_y_used: Union[int, float] = 0,
@@ -316,79 +324,67 @@
                 ymin=min_y_used,
                 ymax=max_y_used,
                 color=color,
                 linestyles="dashed",
                 lw=0.5
             )
         except IndexError as err:
-            logger.warning("Indicator line is out of bound: " + str(err))
+            logger.debug("Indicator line is out of bound: " + str(err))
 
 
 def plot_stroke(
         ax: mpl.axes.Axes,
         data: List[Stroke],
         graph_coords: Optional[Union[Dict, np.ndarray]] = None,
         font_size: int = 5,
-        distance_between_label_axis: Union[int, float] = .1,
         theme: str = "blank",
         **kwargs
 ):
     u"""
     plot stoke
     """
 
     strokes = sorted(data, key=lambda x: [x.start, x.end])
 
     for i, stroke in enumerate(strokes):
         try:
-            ax.hlines(
-                y=i,
-                xmin=graph_coords[stroke.start],
-                xmax=graph_coords[stroke.end],
-                color=stroke.color, lw=2)
-            ax.text(
-                -1 * distance_between_label_axis * max(graph_coords),
-                i + .2,
-                stroke.label,
-                fontsize=font_size,
-                color=stroke.color
-            )
-        except IndexError as err:
-            logger.warning(f"stroke is out of bound: {err}")
+            ax.hlines(y=i, xmin=graph_coords[stroke.start], xmax=graph_coords[stroke.end],  color=stroke.color, lw=2)
+            ax.text(-.1 * max(graph_coords),  i + .2, stroke.label, fontsize=font_size, color=stroke.color)
+        except IndexError as _:
+            logger.info(f"stroke {stroke} is out of bound, this stroke won't show up in final plot")
 
     Theme.set_theme(ax, theme)
-    ax.set_xlim(left=0, right=max(graph_coords))
+    ax.set_xlim(min(graph_coords), max(graph_coords))
     ax.set_ylim(bottom=-1, top=len(strokes))
 
 
-def plot_reference(
+def plot_annotation(
         ax: mpl.axes.Axes,
-        obj: Reference,
+        obj: Annotation,
         graph_coords: Optional[Union[Dict, np.ndarray]] = None,
         font_size: int = 5,
         show_gene: bool = False,
         show_id: bool = False,
         transcripts: Optional[List[str]] = None,
         remove_empty_transcripts: bool = False,
         choose_primary: bool = False,
         color: Optional[str] = None,
         theme: str = "blank",
         y_loc: int = 0,
         exon_width: float = .3,
         plot_domain: bool = False,
         show_exon_id: bool = False,
         raster: bool = True,
-        distance_between_label_axis: float = 0.3,
         **kwargs
 ):
     u"""
-    Plot the structure of reference
+    Plot the structure of annotation
     """
     Theme.set_theme(ax, theme)
-    ax.set_xlim(0, max(graph_coords))
+    ax.set_xlim(min(graph_coords), max(graph_coords))
 
     region = obj.region
 
     data = sorted(obj.data)
     if not data:
         return
 
@@ -407,15 +403,15 @@
             genes[transcript.gene_id].append(transcript)
 
         for _, transcripts_list in genes.items():
             primary_transcripts = sorted(
                 transcripts_list, key=lambda i_: len(i_), reverse=True)[0]
             transcripts.append(primary_transcripts.transcript_id)
     elif choose_primary and (len(transcripts) != 0 or transcripts is not None):
-        logger.warning(
+        logger.debug(
             "--transcripts-to-show is prior to --choose-primary, and primary transcript won't be presented.")
     else:
         pass
 
     """
     @2018.12.26
     Maybe I'm too stupid for this, using 30% of total length of x axis as the gap between text with axis
@@ -431,25 +427,23 @@
             continue
 
         strand = transcript.strand
         # @2018.12.20 add transcript id, based on fixed coordinates
         if transcript.transcript:
             if show_gene and transcript.gene and transcript.gene_id != transcript.transcript_id:
                 if show_id:
-                    ax.text(x=-1 * distance_between_label_axis * max(graph_coords), y=y_loc + 0.25,
+                    ax.text(x=-.01 * max(graph_coords), y=y_loc + 0.25,
                             s=transcript.gene_id, fontsize=font_size, ha="right")
-                    ax.text(x=-1 * distance_between_label_axis * max(graph_coords), y=y_loc - 0.25,
+                    ax.text(x=-.01 * max(graph_coords), y=y_loc - 0.25,
                             s=transcript.transcript_id, fontsize=font_size, ha="right")
                 else:
-                    ax.text(x=-1 * distance_between_label_axis * max(graph_coords), y=y_loc,
-                            s=transcript.gene + " | " + transcript.transcript,
-                            fontsize=font_size, ha="right")
+                    ax.text(x=-.01 * max(graph_coords), y=y_loc,
+                            s=transcript.gene + " | " + transcript.transcript, fontsize=font_size, ha="right")
             else:
-                ax.text(x=-1 * distance_between_label_axis * max(graph_coords), y=y_loc - 0.1, s=transcript.transcript,
-                        fontsize=font_size, ha="right")
+                ax.text(x=-1, y=y_loc - 0.1, s=transcript.transcript, fontsize=font_size, ha="right")
 
         # @2018.12.19
         # s and e is the start and end site of single exon
         # @2022.05.13
         # add index to avoid label overlapping of neighbor exon
         for ind, exon in enumerate(transcript.exons):
             s, e, strand = region.relative(
@@ -610,14 +604,15 @@
 
                 ax.text(x=-1, y=y_loc - 0.125, s=f"{sub_current_domain.gene}|{base_name}",
                         fontsize=font_size / 2, ha="right")
 
             y_loc += 1
 
     # @2022.05.13 Set y lim using y_loc value.
+    ax.set_xlim(min(graph_coords), max(graph_coords))
     ax.set_ylim(-.5, y_loc + .5)
 
 
 def plot_density(
         ax: mpl.axes.Axes,
         obj: Optional[File] = None,
         data: Optional[ReadDepth] = None,
@@ -699,16 +694,16 @@
     #     for idx, y in enumerate([y1, y2]):
     #         if np.sum(y) > 0:
     #             array_hist = np.repeat(graph_coords, np.abs(y1).astype(np.int32))
     #             try:
     #                 kde = gaussian_kde(array_hist)
     #                 fit_value = kde.pdf(graph_coords)
     #             except (ValueError, np.linalg.LinAlgError):
-    #                 # logger.warning(err)
-    #                 # logger.warning(traceback.format_exc())
+    #                 # logger.debug(err)
+    #                 # logger.debug(traceback.format_exc())
     #                 continue
     #
     #             fit_value = fit_value / fit_value.max()
     #             ax.plot(graph_coords, fit_value * np.max(y), c=color, lw=1)
 
     if data.strand_aware:
         max_used_y_val = max(abs(min_used_y_val), max_used_y_val)
@@ -814,15 +809,15 @@
                 t.set_bbox(dict(alpha=0))
                 jxn_numbers.append(t)
 
         try:
             adjust_text(jxn_numbers, force_text=0.2, arrowprops=dict(arrowstyle="-", color='black', lw=1),
                         autoalign="y")
         except IndexError as err:
-            logger.warning(err)
+            logger.debug(err)
 
     if obj and obj.title:
         ax.text(max(graph_coords) - len(obj.title), max_used_y_val, obj.title, color=color, fontsize=font_size)
 
     # update the y-axis actually used
     if not fixed_max_used_y:
         _, max_used_y_val = ax.get_ylim()
@@ -902,16 +897,16 @@
             continue
 
         array_hist = np.repeat(graph_coords, np.abs(array_plot).astype(np.int32))
         try:
             kde = gaussian_kde(array_hist)
             fit_value = kde.pdf(graph_coords)
         except (ValueError, np.linalg.LinAlgError):
-            # logger.warning(err)
-            # logger.warning(traceback.format_exc())
+            # logger.debug(err)
+            # logger.debug(traceback.format_exc())
             continue
 
         fit_value = fit_value / fit_value.max()
         ax.bar(graph_coords, array_plot, color=color, rasterized=raster)
         ax.plot(graph_coords,
                 fit_value * array_plot.max() if label == 'plus' else fit_value * array_plot.min(),
                 c=color, lw=1)
@@ -1157,15 +1152,15 @@
         ax.legend(loc=legend_position,
                   ncol=int(len(data) / 1.5) if legend_ncol <= 0 else legend_ncol,
                   fancybox=False, shadow=False)
     else:
         try:
             adjust_text(legend, arrowprops=dict(arrowstyle="-", lw=1))
         except IndexError as err:
-            logger.warning(err)
+            logger.debug(err)
 
     set_y_ticks(
         ax, label=y_label, theme=theme,
         graph_coords=graph_coords,
         max_used_y_val=max_y_val if max_used_y_val is None else max_used_y_val,
         distance_between_label_axis=distance_between_label_axis,
         font_size=font_size,
@@ -1277,24 +1272,26 @@
                     ]
                     width_ratio = 0.75 if not is_site else 1.5
 
                     y = [
                         y_loc - exon_width * width_ratio, y_loc - exon_width * width_ratio,
                         y_loc + exon_width * width_ratio, y_loc + exon_width * width_ratio
                     ]
-                    ax.fill(
-                        x, y, 'r' if not feature_color else feature_color, lw=.2, zorder=20)
+
                     if is_site:
+                        ax.fill(x, y, 'b' if not feature_color else feature_color, lw=.2, zorder=20)
                         ax.scatter(graph_coords[s],
                                    y_loc + exon_width * width_ratio,
                                    c='b' if not feature_color else feature_color,
                                    s=.5,
                                    linewidths=(0,),
                                    rasterized=raster
                                    )
+                    else:
+                        ax.fill(x, y, 'r' if not feature_color else feature_color, lw=.2, zorder=20)
             if add_plot:
                 y_loc += 1
 
     set_y_ticks(
         ax, label=y_label, theme=theme,
         graph_coords=graph_coords,
         max_used_y_val=y_loc,
@@ -1319,15 +1316,15 @@
             (leftss + step, max_y),
             (rightss - step, max_y),
             (rightss, 0)
         ]
         a = Path(pts, [Path.MOVETO, Path.CURVE4, Path.CURVE4, Path.CURVE4])
         ax.add_patch(PathPatch(a, fc="none", ec=stroke.color, lw=1))
 
-    ax.set_xlim(0, max(graph_coords))
+    ax.set_xlim(min(graph_coords), max(graph_coords))
     ax.set_ylim(max_y, 0)
     ax.axis("off")
 
 
 def make_text_elements(text, x=0.0, y=0.0, width=1.0, height=1.0,
                        color='blue', edgecolor="black",
                        font=FontProperties(family='monospace')):
```

### Comparing `trackplot-0.2.6/trackplot/plot_tests.py` & `trackplot-0.2.7/trackplot/plot_tests.py`

 * *Files identical despite different names*

