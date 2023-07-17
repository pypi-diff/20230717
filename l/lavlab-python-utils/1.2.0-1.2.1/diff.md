# Comparing `tmp/lavlab-python-utils-1.2.0.tar.gz` & `tmp/lavlab-python-utils-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.2.0.tar", last modified: Sat Jul 15 18:30:10 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.2.1.tar", last modified: Mon Jul 17 11:08:51 2023, max compression
```

## Comparing `lavlab-python-utils-1.2.0.tar` & `lavlab-python-utils-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    30893 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-15 18:30:10.000000 lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 18:30:10.783745 lavlab-python-utils-1.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/test/test_omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-15 18:29:59.000000 lavlab-python-utils-1.2.0/test/test_python_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.858035 lavlab-python-utils-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.858035 lavlab-python-utils-1.2.1/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10726 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30918 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10553 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 11:08:51.000000 lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 11:08:51.862035 lavlab-python-utils-1.2.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/test/test_omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-07-17 11:08:37.000000 lavlab-python-utils-1.2.1/test/test_python_utils.py
```

### Comparing `lavlab-python-utils-1.2.0/PKG-INFO` & `lavlab-python-utils-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.2.0/pyproject.toml` & `lavlab-python-utils-1.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lavlab-python-utils"
 description = "LaViolette Lab utility package"
-version = "1.2.0"
+version = "1.2.1"
 
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 
 readme = "README.rst"
 classifiers = [
```

### Comparing `lavlab-python-utils-1.2.0/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.2.1/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.0/src/lavlab/omero_util.py` & `lavlab-python-utils-1.2.1/src/lavlab/omero_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,16 @@
         # create and init rps for this group
         rps = await session.createRawPixelsStore()
         await rps.setPixelsId(id,rps_bypass)
 
         # set res and get default res level if necessary
         if resLvl is None:
             resLvl = await rps.getResolutionLevels()
-        await rps.setResolutionLevel(resLvl-1)
+            resLvl -= 1
+        await rps.setResolutionLevel(resLvl)
 
         # request and return tiles
         i=1
         tile_len=len(tiles)
         for z,c,t,tile in tiles:
             rv = np.frombuffer(await rps.getTile(z,c,t,*tile), dtype=np.uint8)
             rv.shape=tile[3],tile[2]
@@ -294,15 +295,15 @@
             image = Image.fromarray(arr)
             if image.size != xy:
                 del arr # just to be safe
                 image = image.resize(xy)
             images.append(image)
         return images
     
-    event_loop = asyncio.get_running_loop()
+    event_loop = asyncio._get_running_loop()
     if event_loop is None:
         return asyncio.run(work(img, xy_dim, channels))
     else:
         return work(img,xy_dim,channels)
 
 def getImageAtResolution(img: ImageWrapper, xy_dim: tuple[int,int]) -> Image.Image:
     """
@@ -334,15 +335,15 @@
         image = Image.fromarray(arr)
         if image.size != xy:
             del arr # just to be safe
             image = image.resize(xy)
 
         return image
 
-    event_loop = asyncio.get_running_loop()
+    event_loop = asyncio._get_running_loop()
     if event_loop is None:
         return asyncio.run(work(img, xy_dim))
     else:
         return work(img, xy_dim)
 
 def getLargeRecon(img:ImageWrapper, downsample_factor:int = 10, workdir='./', skip_upload=False):
     """
@@ -428,15 +429,15 @@
                 coord[1]:coord[1]+coord[3],
                 coord[0]:coord[0]+coord[2],
                 c ] = tile
         return Image.fromarray(arr)
     
     mask = maskTissueLoose(img_obj)
 
-    event_loop = asyncio.get_running_loop()
+    event_loop = asyncio._get_running_loop()
     if event_loop is None:
         return asyncio.run(work(img_obj, mask))
     else:
         return work(img_obj, mask)
 
 
 #
```

### Comparing `lavlab-python-utils-1.2.0/src/lavlab/python_util.py` & `lavlab-python-utils-1.2.1/src/lavlab/python_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.0/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.2.1/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.2.0
+Version: 1.2.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.2.0/test/test_omero_util.py` & `lavlab-python-utils-1.2.1/test/test_omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.2.0/test/test_python_utils.py` & `lavlab-python-utils-1.2.1/test/test_python_utils.py`

 * *Files identical despite different names*

