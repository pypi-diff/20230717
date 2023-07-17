# Comparing `tmp/omero-cli-transfer-0.5.0.tar.gz` & `tmp/omero-cli-transfer-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omero-cli-transfer-0.5.0.tar", last modified: Tue Jun 20 16:57:38 2023, max compression
+gzip compressed data, was "omero-cli-transfer-0.6.0.tar", last modified: Mon Jul 17 14:41:51 2023, max compression
```

## Comparing `omero-cli-transfer-0.5.0.tar` & `omero-cli-transfer-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)    19883 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/generate_omero_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    41018 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/generate_xml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/omero/plugins/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 16:57:38.350470 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 16:57:38.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22865 2023-06-20 16:57:36.000000 omero-cli-transfer-0.5.0/src/omero_cli_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    17987 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7349 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    20068 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/generate_omero_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41549 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/generate_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/omero/plugins/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:41:51.285550 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 14:41:51.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    23764 2023-07-17 14:41:49.000000 omero-cli-transfer-0.6.0/src/omero_cli_transfer.py
```

### Comparing `omero-cli-transfer-0.5.0/LICENSE` & `omero-cli-transfer-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `omero-cli-transfer-0.5.0/PKG-INFO` & `omero-cli-transfer-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.5.0
+Version: 0.6.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -23,28 +23,28 @@
 Transfer packets contain objects and annotations. This project creates a zip file from an object 
 (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
 in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
 
 The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
 
 # Installation
-tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
+tl;dr: if you have `python>=3.8`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
 
-`omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
+`omero-cli-transfer` requires at least Python 3.8. This is due to `ome-types` requiring that as well;
 this package relies heavily on it, and it is not feasible without it. 
 
 Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
-it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
+it is possible to run `omero-py` in Python 3.8 or newer as well. Our recommended way to do so it using `conda`.
 With conda installed, you can do
 ```
-conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
+conda create -n myenv -c conda-force python=3.8 zeroc-ice==3.6.5
 conda activate myenv
 pip install omero-cli-transfer
 ```
-It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
+It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.8,
 but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
 process that can be anything from "completely seamless and without issues" to "I need to install every 
 dependency ever imagined". Try at your own risk.
 
 If you want optional RO-Crate exports, you can do 
 ```
 pip install omero-cli-transfer[rocrate]
```

### Comparing `omero-cli-transfer-0.5.0/README.md` & `omero-cli-transfer-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 Transfer packets contain objects and annotations. This project creates a zip file from an object 
 (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
 in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
 
 The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
 
 # Installation
-tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
+tl;dr: if you have `python>=3.8`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
 
-`omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
+`omero-cli-transfer` requires at least Python 3.8. This is due to `ome-types` requiring that as well;
 this package relies heavily on it, and it is not feasible without it. 
 
 Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
-it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
+it is possible to run `omero-py` in Python 3.8 or newer as well. Our recommended way to do so it using `conda`.
 With conda installed, you can do
 ```
-conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
+conda create -n myenv -c conda-force python=3.8 zeroc-ice==3.6.5
 conda activate myenv
 pip install omero-cli-transfer
 ```
-It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
+It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.8,
 but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
 process that can be anything from "completely seamless and without issues" to "I need to install every 
 dependency ever imagined". Try at your own risk.
 
 If you want optional RO-Crate exports, you can do 
 ```
 pip install omero-cli-transfer[rocrate]
```

### Comparing `omero-cli-transfer-0.5.0/setup.py` & `omero-cli-transfer-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     packages=['', 'omero.plugins'],
     package_dir={"": "src"},
     name="omero-cli-transfer",
-    version='0.5.0',
+    version='0.6.0',
     maintainer="Erick Ratamero",
     maintainer_email="erick.ratamero@jax.org",
     description=("A set of utilities for exporting a transfer"
                  " packet from an OMERO server and importing "
                  "it in a different server. Developed by the "
                  "Research IT team at The Jackson Laboratory."),
     long_description=long_description,
```

### Comparing `omero-cli-transfer-0.5.0/src/generate_omero_objects.py` & `omero-cli-transfer-0.6.0/src/generate_omero_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,23 +146,27 @@
 def create_plate_map(ome: OME, img_map: dict, conn: BlitzGateway
                      ) -> Tuple[dict, OME]:
     newome = copy.deepcopy(ome)
     plate_map = {}
     map_ref_ids = []
     for plate in ome.plates:
         ann_ids = [i.id for i in plate.annotation_ref]
+        file_path = ""
         for ann in ome.structured_annotations:
             if (ann.id in ann_ids and
                     type(ann) == CommentAnnotation and
                     int(ann.id.split(":")[-1]) < 0):
                 newome.structured_annotations.remove(ann)
                 map_ref_ids.append(ann.id)
                 file_path = ann.value
         q = conn.getQueryService()
         params = Parameters()
+        if not file_path:
+            raise ValueError(f"Plate ID {plate.id} does not have a \
+                             CommentAnnotation with a file path!")
         path_query = str(file_path).strip('/')
         if path_query.endswith('mock_folder'):
             path_query = path_query.rstrip("mock_folder")
         params.map = {"cpath": rstring('%%%s%%' % path_query)}
         results = q.projection(
             "SELECT p.id FROM Plate p"
             " JOIN p.plateAcquisitions a"
```

### Comparing `omero-cli-transfer-0.5.0/src/generate_xml.py` & `omero-cli-transfer-0.6.0/src/generate_xml.py`

 * *Files 3% similar despite different names*

```diff
@@ -459,42 +459,51 @@
             mmap.append(M(k=_key, value=''))
     kv, ref = create_kv_and_ref(id=id,
                                 namespace=ns,
                                 value=Map(m=mmap))
     return kv, ref
 
 
-def create_objects(folder):
+def create_objects(folder, filelist):
     img_files = []
-    for path, subdirs, files in os.walk(folder):
-        for f in files:
-            img_files.append(os.path.abspath(os.path.join(path, f)))
-    targets = copy.deepcopy(img_files)
     cli = CLI()
     cli.loadplugins()
-    for img in img_files:
-        if img not in (targets):
-            continue
-        cmd = ["omero", 'import', '-f', img, "\n"]
-        res = cli.popen(cmd, stdout=PIPE, stderr=DEVNULL)
-        std = res.communicate()
-        files = parse_files_import(std[0].decode('UTF-8'))
-        if len(files) > 1:
+    if not filelist:
+        for path, subdirs, files in os.walk(folder):
             for f in files:
-                targets.remove(f)
-            targets.append(img)
-        if len(files) == 0:
-            targets.remove(img)
+                img_files.append(os.path.abspath(os.path.join(path, f)))
+        targets = copy.deepcopy(img_files)
+        for img in img_files:
+            if img not in (targets):
+                continue
+            cmd = ["omero", 'import', '-f', img, "\n"]
+            res = cli.popen(cmd, stdout=PIPE, stderr=DEVNULL)
+            std = res.communicate()
+            files = parse_files_import(std[0].decode('UTF-8'))
+            if len(files) > 1:
+                for f in files:
+                    targets.remove(f)
+                targets.append(img)
+            if len(files) == 0:
+                targets.remove(img)
+    else:
+        with open(folder, "r") as f:
+            targets_str = f.read().splitlines()
+        targets = []
+        par_folder = Path(folder).parent
+        for target in targets_str:
+            targets.append(str((par_folder / target).resolve()))
     images = []
     plates = []
     annotations = []
     counter_imgs = 1
     counter_pls = 1
     for target in targets:
-        print(f"Processing file {target}\n")
+        target = str(Path(target).absolute())
+        print(f"Processing file {target}")
         res = run_showinf(target, cli)
         imgs, pls, anns = parse_showinf(res,
                                         counter_imgs, counter_pls, target)
         images.extend(imgs)
         counter_imgs = counter_imgs + len(imgs)
         plates.extend(pls)
         counter_pls = counter_pls + len(pls)
@@ -850,28 +859,31 @@
         with open(filepath, 'w') as fp:
             print(to_xml(ome), file=fp)
             fp.close()
     path_id_dict = list_file_ids(ome)
     return ome, path_id_dict
 
 
-def populate_xml_folder(folder: str, conn: BlitzGateway, session: str
-                        ) -> Tuple[OME, dict]:
+def populate_xml_folder(folder: str, filelist: bool, conn: BlitzGateway,
+                        session: str) -> Tuple[OME, dict]:
     ome = OME()
-    images, plates, annotations = create_objects(folder)
+    images, plates, annotations = create_objects(folder, filelist)
     ome.images = images
     ome.plates = plates
     ome.structured_annotations = annotations
-    filepath = str(Path(folder) / "transfer.xml")
-    if Path(folder).exists():
-        with open(filepath, 'w') as fp:
-            print(to_xml(ome), file=fp)
-            fp.close()
+    if filelist:
+        filepath = str(Path(folder).parent.resolve() / "transfer.xml")
     else:
-        raise ValueError("Folder cannot be found!")
+        if Path(folder).exists():
+            filepath = str(Path(folder) / "transfer.xml")
+        else:
+            raise ValueError("Folder cannot be found!")
+    with open(filepath, 'w') as fp:
+        print(to_xml(ome), file=fp)
+        fp.close()
     path_id_dict = list_file_ids(ome)
     return ome, path_id_dict
 
 
 def populate_tsv(datatype: str, ome: OME, filepath: str,
                  path_id_dict: dict, folder: str):
     if datatype == "Plate" or datatype == "Screen":
```

### Comparing `omero-cli-transfer-0.5.0/src/omero/plugins/transfer.py` & `omero-cli-transfer-0.6.0/src/omero/plugins/transfer.py`

 * *Files identical despite different names*

### Comparing `omero-cli-transfer-0.5.0/src/omero_cli_transfer.egg-info/PKG-INFO` & `omero-cli-transfer-0.6.0/src/omero_cli_transfer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omero-cli-transfer
-Version: 0.5.0
+Version: 0.6.0
 Summary: A set of utilities for exporting a transfer packet from an OMERO server and importing it in a different server. Developed by the Research IT team at The Jackson Laboratory.
 Home-page: https://github.com/TheJacksonLaboratory/omero-cli-transfer
 Maintainer: Erick Ratamero
 Maintainer-email: erick.ratamero@jax.org
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
@@ -23,28 +23,28 @@
 Transfer packets contain objects and annotations. This project creates a zip file from an object 
 (Project, Dataset, Image, Screen, Plate) containing all original files necessary to create the images 
 in that object, plus an XML file detailing the links between entities, annotations and ROIs thereof.
 
 The CLI plugin add the subcommand `transfer`, which in its turn has two further subcommands `omero transfer pack` and `omero transfer unpack`. Both subcommands (pack and unpack) will use an existing OMERO session created via CLI or prompt the user for parameters to create one.
 
 # Installation
-tl;dr: if you have `python>=3.7`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
+tl;dr: if you have `python>=3.8`, a simple `pip install omero-cli-transfer` _might_ do. We recommend conda, though.
 
-`omero-cli-transfer` requires at least Python 3.7. This is due to `ome-types` requiring that as well;
+`omero-cli-transfer` requires at least Python 3.8. This is due to `ome-types` requiring that as well;
 this package relies heavily on it, and it is not feasible without it. 
 
 Of course, this CAN be an issue, especially given `omero-py` _officially_ only supports Python 3.6. However,
-it is possible to run `omero-py` in Python 3.7 or newer as well. Our recommended way to do so it using `conda`.
+it is possible to run `omero-py` in Python 3.8 or newer as well. Our recommended way to do so it using `conda`.
 With conda installed, you can do
 ```
-conda create -n myenv -c conda-force python=3.7 zeroc-ice==3.6.5
+conda create -n myenv -c conda-force python=3.8 zeroc-ice==3.6.5
 conda activate myenv
 pip install omero-cli-transfer
 ```
-It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.7,
+It is possible to do the same thing without `conda` as long as your python/pip version is at least 3.8,
 but that will require locally building a wheel for `zeroc-ice` (which pip does automatically) - it is a
 process that can be anything from "completely seamless and without issues" to "I need to install every 
 dependency ever imagined". Try at your own risk.
 
 If you want optional RO-Crate exports, you can do 
 ```
 pip install omero-cli-transfer[rocrate]
```

### Comparing `omero-cli-transfer-0.5.0/src/omero_cli_transfer.py` & `omero-cli-transfer-0.6.0/src/omero_cli_transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,16 +115,29 @@
 PREPARE_HELP = ("""Creates an XML from a folder with images.
 
 Creates an XML file appropriate for usage with `omero transfer unpack` from
 a folder that contains image files, rather than a source OMERO server. This
 is intended as a first step on a bulk-import workflow, followed by using
 `omero transfer unpack` to complete an import.
 
+Note: images imported from an XML generated with this tool will have whichever
+names `showinf` reports them to have; that is, the names on their internal
+metadata, which might be different from filenames. For multi-image files,
+image names follow the pattern "filename [imagename]", where 'imagename' is
+the one reported by `showinf`.
+
+--filelist allows you to specify a text file containing a list of file paths
+(one per line). Relative paths should be relative to the location of the file
+list. The XML file will only take those files into consideration.
+The resulting `transfer.xml` file will be created on the same directory of
+your file list.
+
 Examples:
 omero transfer prepare /home/user/folder_with_files
+omero transfer prepare --filelist /home/user/file_with_paths.txt
 """)
 
 
 def gateway_required(func: Callable) -> Callable:
     """
     Decorator which initializes a client (self.client),
     a BlitzGateway (self.gateway), and makes sure that
@@ -202,14 +215,17 @@
             choices=['all', 'none', 'img_id', 'plate_id', 'timestamp',
                      'software', 'version', 'md5', 'hostname', 'db_id',
                      'orig_user', 'orig_group'], nargs='+',
             help="Metadata field to be added to MapAnnotation"
         )
         folder_help = ("Path to folder with image files")
         prepare.add_argument("folder", type=str, help=folder_help)
+        prepare.add_argument(
+            "--filelist", help="Pass path to a filelist rather than a folder",
+            action="store_true")
 
     @gateway_required
     def pack(self, args):
         """ Implements the 'pack' command """
         self.__pack(args)
 
     @gateway_required
@@ -542,15 +558,16 @@
                 if len(src_v) == len(dest_v):
                     for count in range(len(src_v)):
                         map_key = f"Image:{src_v[count]}"
                         imgmap[map_key] = dest_v[count]
         return imgmap
 
     def __prepare(self, args):
-        populate_xml_folder(args.folder, self.gateway, self.session)
+        populate_xml_folder(args.folder, args.filelist, self.gateway,
+                            self.session)
         return
 
 
 try:
     register("transfer", TransferControl, HELP)
 except NameError:
     if __name__ == "__main__":
```

