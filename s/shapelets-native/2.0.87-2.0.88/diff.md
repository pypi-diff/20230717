# Comparing `tmp/shapelets_native-2.0.87-cp39-cp39-win_amd64.whl.zip` & `tmp/shapelets_native-2.0.88-cp38-cp38-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7517665 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat      250 b- defN 23-Jul-13 12:25 shapelets_native/__init__.py
--rw-rw-rw-  2.0 fat    95123 b- defN 23-Jul-13 12:25 shapelets_native/__init__.pyi
--rw-rw-rw-  2.0 fat 22662144 b- defN 23-Jul-13 12:25 shapelets_native/_shapelets_extension.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-13 12:25 shapelets_native/_version.py
--rw-rw-rw-  2.0 fat      253 b- defN 23-Jul-13 12:25 shapelets_native/_version.pyi
--rw-rw-rw-  2.0 fat      133 b- defN 23-Jul-13 12:25 shapelets_native/py.typed
--rw-rw-rw-  2.0 fat      930 b- defN 23-Jul-13 12:26 shapelets_native-2.0.87.dist-info/LICENSE.md
--rw-rw-rw-  2.0 fat      471 b- defN 23-Jul-13 12:26 shapelets_native-2.0.87.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-13 12:26 shapelets_native-2.0.87.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-13 12:25 shapelets_native-2.0.87.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      975 b- defN 23-Jul-13 12:26 shapelets_native-2.0.87.dist-info/RECORD
-11 files, 22760556 bytes uncompressed, 7515993 bytes compressed:  67.0%
+Zip file size: 7544509 bytes, number of entries: 11
+-rw-rw-rw-  2.0 fat      250 b- defN 23-Jul-17 08:24 shapelets_native/__init__.py
+-rw-rw-rw-  2.0 fat    95123 b- defN 23-Jul-17 08:24 shapelets_native/__init__.pyi
+-rw-rw-rw-  2.0 fat 22852608 b- defN 23-Jul-17 08:24 shapelets_native/_shapelets_extension.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-17 08:24 shapelets_native/_version.py
+-rw-rw-rw-  2.0 fat      253 b- defN 23-Jul-17 08:24 shapelets_native/_version.pyi
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Jul-17 08:24 shapelets_native/py.typed
+-rw-rw-rw-  2.0 fat      930 b- defN 23-Jul-17 08:24 shapelets_native-2.0.88.dist-info/LICENSE.md
+-rw-rw-rw-  2.0 fat      471 b- defN 23-Jul-17 08:24 shapelets_native-2.0.88.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Jul-17 08:24 shapelets_native-2.0.88.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-17 08:24 shapelets_native-2.0.88.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      975 b- defN 23-Jul-17 08:24 shapelets_native-2.0.88.dist-info/RECORD
+11 files, 22951020 bytes uncompressed, 7542837 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: shapelets_native/__init__.py
 Comment: 
 
 Filename: shapelets_native/__init__.pyi
 Comment: 
 
-Filename: shapelets_native/_shapelets_extension.cp39-win_amd64.pyd
+Filename: shapelets_native/_shapelets_extension.cp38-win_amd64.pyd
 Comment: 
 
 Filename: shapelets_native/_version.py
 Comment: 
 
 Filename: shapelets_native/_version.pyi
 Comment: 
 
 Filename: shapelets_native/py.typed
 Comment: 
 
-Filename: shapelets_native-2.0.87.dist-info/LICENSE.md
+Filename: shapelets_native-2.0.88.dist-info/LICENSE.md
 Comment: 
 
-Filename: shapelets_native-2.0.87.dist-info/METADATA
+Filename: shapelets_native-2.0.88.dist-info/METADATA
 Comment: 
 
-Filename: shapelets_native-2.0.87.dist-info/WHEEL
+Filename: shapelets_native-2.0.88.dist-info/WHEEL
 Comment: 
 
-Filename: shapelets_native-2.0.87.dist-info/top_level.txt
+Filename: shapelets_native-2.0.88.dist-info/top_level.txt
 Comment: 
 
-Filename: shapelets_native-2.0.87.dist-info/RECORD
+Filename: shapelets_native-2.0.88.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## shapelets_native/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '2.0.87'
-__version_tuple__ = version_tuple = (2, 0, 87)
+__version__ = version = '2.0.88'
+__version_tuple__ = version_tuple = (2, 0, 88)
```

## Comparing `shapelets_native-2.0.87.dist-info/LICENSE.md` & `shapelets_native-2.0.88.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `shapelets_native-2.0.87.dist-info/RECORD` & `shapelets_native-2.0.88.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 shapelets_native/__init__.py,sha256=02Fs6rxo4XxpTfdKmMPgecJwnuhEgHcdXxAZwTEgevA,250
 shapelets_native/__init__.pyi,sha256=65zESK5cTUfYZjlcu--7QYATrd1xHxasp2gkDy9-2Q0,95123
-shapelets_native/_shapelets_extension.cp39-win_amd64.pyd,sha256=XhxGFWI8lUPvrX62JMJeXBQRzPOxXX4CXl2izkY_2QY,22662144
-shapelets_native/_version.py,sha256=D3f3QU8bDHU5QEkFTttFYFsFnk_h9h40DQ8DZONqePg,166
+shapelets_native/_shapelets_extension.cp38-win_amd64.pyd,sha256=CdhK0Qe7U_MUfsxPewpZnnoxcCP4fzUtx8EKz_qTrdU,22852608
+shapelets_native/_version.py,sha256=aSG-0E4905aG23K2bCf1_PXUnZ7MTJ4TlFt_AzuU6RY,166
 shapelets_native/_version.pyi,sha256=EhZqK9ILGWqaBdBaMJa21MYgoMVbndEC4PCq_mfMTiA,253
 shapelets_native/py.typed,sha256=S4MESMY2h1FTeF2pk08yejbD-NhKnOl6RZrvZ6HCrRo,133
-shapelets_native-2.0.87.dist-info/LICENSE.md,sha256=Fq071sYNrZMCA77b2pFJu67xpN8WA6peeIRoL9McDIE,930
-shapelets_native-2.0.87.dist-info/METADATA,sha256=uyBWflT1B_1zCMl1bRi7WR8UF7fsHLyTLWQlFF225sM,471
-shapelets_native-2.0.87.dist-info/WHEEL,sha256=aFh_uQusBybh-RCXOkSlg-ycdQBtqU_JDPyXfjBBBgs,94
-shapelets_native-2.0.87.dist-info/top_level.txt,sha256=fAASXfFJeVmpzpqVN5JhnQfJbziQDO_sAsN2PODOyTY,17
-shapelets_native-2.0.87.dist-info/RECORD,,
+shapelets_native-2.0.88.dist-info/LICENSE.md,sha256=Fq071sYNrZMCA77b2pFJu67xpN8WA6peeIRoL9McDIE,930
+shapelets_native-2.0.88.dist-info/METADATA,sha256=y_I-Qk_1_Ffv9bvMYjG2UYlI87pStCW-57g1u0IzjTI,471
+shapelets_native-2.0.88.dist-info/WHEEL,sha256=rjmE6jOYKSgS2T4NpCJJtLEPSybiWFu39x_TGcEjjFE,94
+shapelets_native-2.0.88.dist-info/top_level.txt,sha256=fAASXfFJeVmpzpqVN5JhnQfJbziQDO_sAsN2PODOyTY,17
+shapelets_native-2.0.88.dist-info/RECORD,,
```

