# Comparing `tmp/symlib-1.3.8.tar.gz` & `tmp/symlib-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symlib-1.3.8.tar", last modified: Sun Jul 16 21:24:19 2023, max compression
+gzip compressed data, was "symlib-1.3.9.tar", last modified: Mon Jul 17 18:26:09 2023, max compression
```

## Comparing `symlib-1.3.8.tar` & `symlib-1.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.007568 symlib-1.3.8/
--rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.8/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-16 21:24:19.007409 symlib-1.3.8/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.8/README.md
--rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.8/pyproject.toml
--rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-16 21:24:19.007626 symlib-1.3.8/setup.cfg
--rw-r--r--   0 phil       (501) staff       (20)      885 2023-07-16 21:07:47.000000 symlib-1.3.8/setup.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.006618 symlib-1.3.8/symlib/
--rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.8/symlib/__init__.py
--rw-r--r--   0 phil       (501) staff       (20)     7049 2022-09-20 17:00:26.000000 symlib-1.3.8/symlib/file_management.py
--rw-r--r--   0 phil       (501) staff       (20)    53792 2023-07-15 01:24:54.000000 symlib-1.3.8/symlib/lib.py
--rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.8/symlib/match.py
--rw-r--r--   0 phil       (501) staff       (20)    36177 2023-06-27 17:16:14.000000 symlib-1.3.8/symlib/star_tagging.py
--rw-r--r--   0 phil       (501) staff       (20)     9979 2023-07-15 01:24:54.000000 symlib-1.3.8/symlib/util.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-16 21:24:19.007215 symlib-1.3.8/symlib.egg-info/
--rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)      303 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/SOURCES.txt
--rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/dependency_links.txt
--rw-r--r--   0 phil       (501) staff       (20)       41 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/requires.txt
--rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-16 21:24:18.000000 symlib-1.3.8/symlib.egg-info/top_level.txt
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-17 18:26:09.827983 symlib-1.3.9/
+-rw-r--r--   0 phil       (501) staff       (20)     1071 2022-07-08 18:08:58.000000 symlib-1.3.9/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-17 18:26:09.827855 symlib-1.3.9/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      260 2022-08-19 20:35:54.000000 symlib-1.3.9/README.md
+-rw-r--r--   0 phil       (501) staff       (20)       84 2022-07-08 18:08:58.000000 symlib-1.3.9/pyproject.toml
+-rw-r--r--   0 phil       (501) staff       (20)       38 2023-07-17 18:26:09.828017 symlib-1.3.9/setup.cfg
+-rw-r--r--   0 phil       (501) staff       (20)      885 2023-07-17 18:26:04.000000 symlib-1.3.9/setup.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-17 18:26:09.827079 symlib-1.3.9/symlib/
+-rw-r--r--   0 phil       (501) staff       (20)     1715 2023-06-16 17:53:43.000000 symlib-1.3.9/symlib/__init__.py
+-rw-r--r--   0 phil       (501) staff       (20)     7006 2023-07-17 18:12:25.000000 symlib-1.3.9/symlib/file_management.py
+-rw-r--r--   0 phil       (501) staff       (20)    53792 2023-07-15 01:24:54.000000 symlib-1.3.9/symlib/lib.py
+-rw-r--r--   0 phil       (501) staff       (20)     9008 2023-06-16 17:53:43.000000 symlib-1.3.9/symlib/match.py
+-rw-r--r--   0 phil       (501) staff       (20)    36177 2023-06-27 17:16:14.000000 symlib-1.3.9/symlib/star_tagging.py
+-rw-r--r--   0 phil       (501) staff       (20)     9979 2023-07-15 01:24:54.000000 symlib-1.3.9/symlib/util.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-07-17 18:26:09.827686 symlib-1.3.9/symlib.egg-info/
+-rw-r--r--   0 phil       (501) staff       (20)      762 2023-07-17 18:26:09.000000 symlib-1.3.9/symlib.egg-info/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)      303 2023-07-17 18:26:09.000000 symlib-1.3.9/symlib.egg-info/SOURCES.txt
+-rw-r--r--   0 phil       (501) staff       (20)        1 2023-07-17 18:26:09.000000 symlib-1.3.9/symlib.egg-info/dependency_links.txt
+-rw-r--r--   0 phil       (501) staff       (20)       41 2023-07-17 18:26:09.000000 symlib-1.3.9/symlib.egg-info/requires.txt
+-rw-r--r--   0 phil       (501) staff       (20)        7 2023-07-17 18:26:09.000000 symlib-1.3.9/symlib.egg-info/top_level.txt
```

### Comparing `symlib-1.3.8/LICENSE` & `symlib-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/PKG-INFO` & `symlib-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.8
+Version: 1.3.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `symlib-1.3.8/setup.py` & `symlib-1.3.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import setuptools
-version = "1.3.8"
+version = "1.3.9"
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="symlib",
     version=version,
```

### Comparing `symlib-1.3.8/symlib/__init__.py` & `symlib-1.3.9/symlib/__init__.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/symlib/file_management.py` & `symlib-1.3.9/symlib/file_management.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from . import lib
 from os import path
 import os
 import shutil
 import requests
 import time
 
-DOWNLOAD_TARGETS = ["halos", "trees"]
+DOWNLOAD_TARGETS = ["halos", "trees", "particles", "full_snapshots"]
 BASE_URL_FORMAT = "https://%s:%s@s3df.slac.stanford.edu/data/kipac/symphony/"
 RETRY_WAIT_TIME = 5
 
 def pack_files(suite, halo_name, base_out_dir, target="halos",
                logging=True):
     if logging:
         print("Packing halo %s in suite %s to %s" % (
@@ -72,33 +72,32 @@
     if isinstance(halo_name, int):
         halo_name = util.DEFAULT_HALO_NAMES[suite][halo_name]
 
     if halo_name not in util.DEFAULT_HALO_NAMES[suite]:
         raise ValueError("Unrecognized halo, %s, for the suite %s" %
                          (str(halo_name), suite))
                 
-    out_dir = path.join(base_out_dir, "tar_files", suite, target)
-    os.makedirs(out_dir, exist_ok=True)
+    os.makedirs(base_out_dir, exist_ok=True)
 
     base_url = BASE_URL_FORMAT % (user, password)
-    url = "%s%s/%s/%s.tar.gz" % (base_url, suite, target, halo_name)
-    out_file = path.join(out_dir, "%s.tar" % halo_name)
-
+    base_name = "%s_%s_%s.tar" % (suite, halo_name, target)
+    url = base_url + base_name
+    out_file = path.join(base_out_dir, base_name)    
     # The next three lines are adapted from
     # https://stackoverflow.com/a/39217788
     # Original author is John Zwink, edited by the users vog, Martjin Peters, and
     # Daniel F.
     with requests.get(url, stream=True) as r:
         with open(out_file, 'wb') as f:
             shutil.copyfileobj(r.raw, f)
             
     if not path.exists(out_file):
         raise FileNotFoundError("Unable to download halo %s from the suite %s" %
                                 (halo_name, suite))
-    
+ 
     with open(out_file, "rb") as f:
         text = f.read(6)
         if text == b"<html>":
             f.seek(0, 0)
             text = f.read()
             os.remove(out_file)
 
@@ -135,16 +134,15 @@
         for i in range(util.n_hosts(suite)):
             unpack_files(suite, i, base_out_dir, target=target)
         return
 
     if isinstance(halo_name, int):
         halo_name = util.DEFAULT_HALO_NAMES[suite][halo_name]
 
-    tar_loc = path.join(base_out_dir, "tar_files", suite,
-                        target, "%s.tar" % halo_name)
+    tar_loc = path.join(base_out_dir, "%s_%s_%s.tar" % (suite, halo_name, target))
     if not path.exists(tar_loc):
         raise FileNotFoundError("The file associated with the requested target data for host %s in suite %s does not exist within the base directory %s. This is probably because it was already downloaded or already unpacked." % (halo_name, suite, base_out_dir))
     shutil.unpack_archive(tar_loc, base_out_dir)
     os.remove(tar_loc)
     
     
 def download_files(user, password, suite, halo_name, base_out_dir,
```

### Comparing `symlib-1.3.8/symlib/lib.py` & `symlib-1.3.9/symlib/lib.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/symlib/match.py` & `symlib-1.3.9/symlib/match.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/symlib/star_tagging.py` & `symlib-1.3.9/symlib/star_tagging.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/symlib/util.py` & `symlib-1.3.9/symlib/util.py`

 * *Files identical despite different names*

### Comparing `symlib-1.3.8/symlib.egg-info/PKG-INFO` & `symlib-1.3.9/symlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: symlib
-Version: 1.3.8
+Version: 1.3.9
 Summary: A library for working with data from the Symphony and MW-est zoom-in suites.
 Home-page: https://github.com/phil-mansfield/symlib
 Author: Philip Mansfield
 Author-email: mansfield.astro@gmail.com
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

