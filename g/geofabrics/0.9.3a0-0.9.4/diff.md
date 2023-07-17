# Comparing `tmp/geofabrics-0.9.3a0.tar.gz` & `tmp/geofabrics-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geofabrics-0.9.3a0.tar", last modified: Thu Jun 23 14:51:03 2022, max compression
+gzip compressed data, was "geofabrics-0.9.4.tar", last modified: Thu Jun 23 19:18:47 2022, max compression
```

## Comparing `geofabrics-0.9.3a0.tar` & `geofabrics-0.9.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 14:51:03.800379 geofabrics-0.9.3a0/
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    35149 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/LICENSE
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    43028 2022-06-23 14:51:03.800723 geofabrics-0.9.3a0/PKG-INFO
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)     1671 2022-06-23 14:48:46.000000 geofabrics-0.9.3a0/README.md
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)     1316 2022-06-23 14:49:51.000000 geofabrics-0.9.3a0/pyproject.toml
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      113 2022-06-23 14:51:03.801349 geofabrics-0.9.3a0/setup.cfg
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      208 2022-06-23 14:48:46.000000 geofabrics-0.9.3a0/setup.py
-drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 14:51:03.788443 geofabrics-0.9.3a0/src/
-drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 14:51:03.796433 geofabrics-0.9.3a0/src/geofabrics/
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      560 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/src/geofabrics/__init__.py
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    67279 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/src/geofabrics/bathymetry_estimation.py
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    78938 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/src/geofabrics/dem.py
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    35205 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/src/geofabrics/geometry.py
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    82373 2022-06-23 13:56:24.000000 geofabrics-0.9.3a0/src/geofabrics/processor.py
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       96 2022-06-23 14:48:46.000000 geofabrics-0.9.3a0/src/geofabrics/version.py
-drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 14:51:03.799895 geofabrics-0.9.3a0/src/geofabrics.egg-info/
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    43028 2022-06-23 14:51:03.797173 geofabrics-0.9.3a0/src/geofabrics.egg-info/PKG-INFO
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      451 2022-06-23 14:51:03.797730 geofabrics-0.9.3a0/src/geofabrics.egg-info/SOURCES.txt
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)        1 2022-06-23 14:51:03.798296 geofabrics-0.9.3a0/src/geofabrics.egg-info/dependency_links.txt
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       41 2022-06-23 14:51:03.798848 geofabrics-0.9.3a0/src/geofabrics.egg-info/entry_points.txt
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      184 2022-06-23 14:51:03.799463 geofabrics-0.9.3a0/src/geofabrics.egg-info/requires.txt
--rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       11 2022-06-23 14:51:03.800014 geofabrics-0.9.3a0/src/geofabrics.egg-info/top_level.txt
+drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 19:18:47.242148 geofabrics-0.9.4/
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    35149 2022-06-23 13:56:24.000000 geofabrics-0.9.4/LICENSE
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    43026 2022-06-23 19:18:47.242638 geofabrics-0.9.4/PKG-INFO
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)     1671 2022-06-23 14:48:46.000000 geofabrics-0.9.4/README.md
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)     1314 2022-06-23 19:17:34.000000 geofabrics-0.9.4/pyproject.toml
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      113 2022-06-23 19:18:47.243289 geofabrics-0.9.4/setup.cfg
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      208 2022-06-23 14:48:46.000000 geofabrics-0.9.4/setup.py
+drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 19:18:47.180016 geofabrics-0.9.4/src/
+drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 19:18:47.237418 geofabrics-0.9.4/src/geofabrics/
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      560 2022-06-23 13:56:24.000000 geofabrics-0.9.4/src/geofabrics/__init__.py
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    67279 2022-06-23 13:56:24.000000 geofabrics-0.9.4/src/geofabrics/bathymetry_estimation.py
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    78944 2022-06-23 18:01:19.000000 geofabrics-0.9.4/src/geofabrics/dem.py
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    35208 2022-06-23 19:17:34.000000 geofabrics-0.9.4/src/geofabrics/geometry.py
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    83179 2022-06-23 18:01:19.000000 geofabrics-0.9.4/src/geofabrics/processor.py
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       96 2022-06-23 19:17:34.000000 geofabrics-0.9.4/src/geofabrics/version.py
+drwxrwxr-x   0 pearsonra (308304) pearsonra (308304)        0 2022-06-23 19:18:47.241810 geofabrics-0.9.4/src/geofabrics.egg-info/
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)    43026 2022-06-23 19:18:46.000000 geofabrics-0.9.4/src/geofabrics.egg-info/PKG-INFO
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      451 2022-06-23 19:18:47.239332 geofabrics-0.9.4/src/geofabrics.egg-info/SOURCES.txt
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)        1 2022-06-23 19:18:46.000000 geofabrics-0.9.4/src/geofabrics.egg-info/dependency_links.txt
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       41 2022-06-23 19:18:46.000000 geofabrics-0.9.4/src/geofabrics.egg-info/entry_points.txt
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)      184 2022-06-23 19:18:46.000000 geofabrics-0.9.4/src/geofabrics.egg-info/requires.txt
+-rw-rw-r--   0 pearsonra (308304) pearsonra (308304)       11 2022-06-23 19:18:47.241929 geofabrics-0.9.4/src/geofabrics.egg-info/top_level.txt
```

### Comparing `geofabrics-0.9.3a0/LICENSE` & `geofabrics-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `geofabrics-0.9.3a0/PKG-INFO` & `geofabrics-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofabrics
-Version: 0.9.3a0
+Version: 0.9.4
 Summary: A package for creating geofabrics for flood modelling.
 Author-email: Rose pearson <rose.pearson@niwa.co.nz>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `geofabrics-0.9.3a0/README.md` & `geofabrics-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `geofabrics-0.9.3a0/pyproject.toml` & `geofabrics-0.9.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geofabrics"
-version = "0.9.3a0"
+version = "0.9.4"
 description = "A package for creating geofabrics for flood modelling."
 readme = "README.md"
 authors = [{ name = "Rose pearson", email = "rose.pearson@niwa.co.nz" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
```

### Comparing `geofabrics-0.9.3a0/src/geofabrics/__init__.py` & `geofabrics-0.9.4/src/geofabrics/__init__.py`

 * *Files identical despite different names*

### Comparing `geofabrics-0.9.3a0/src/geofabrics/bathymetry_estimation.py` & `geofabrics-0.9.4/src/geofabrics/bathymetry_estimation.py`

 * *Files identical despite different names*

### Comparing `geofabrics-0.9.3a0/src/geofabrics/dem.py` & `geofabrics-0.9.4/src/geofabrics/dem.py`

 * *Files 0% similar despite different names*

```diff
@@ -719,15 +719,15 @@
         # intersection errors
         if type(dense_extents) is shapely.geometry.Polygon:
             dense_extents = shapely.geometry.Polygon(dense_extents.exterior)
         elif type(dense_extents) is shapely.geometry.MultiPolygon:
             dense_extents = shapely.geometry.MultiPolygon(
                 [
                     shapely.geometry.Polygon(polygon.exterior)
-                    for polygon in dense_extents
+                    for polygon in dense_extents.geoms
                 ]
             )
         # Convert into a Geopandas dataframe
         dense_extents = geopandas.GeoDataFrame(
             {"geometry": [dense_extents]}, crs=self.catchment_geometry.crs["horizontal"]
         )
```

### Comparing `geofabrics-0.9.3a0/src/geofabrics/geometry.py` & `geofabrics-0.9.4/src/geofabrics/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -354,40 +354,40 @@
                     row.interpolate(i * resolution)
                     for i in range(int(numpy.ceil(row.length / resolution)))
                 ]
             )
         )
 
         points = numpy.empty(
-            [points_df.apply(lambda row: len(row)).sum()],
+            [points_df.apply(lambda row: len(row.geoms)).sum()],
             dtype=[("X", numpy.float64), ("Y", numpy.float64), ("Z", numpy.float64)],
         )
 
         # Extract the x, y and z values from the Shapely MultiPoints and possibly a
         # depth column
         points["X"] = numpy.concatenate(
-            points_df.apply(lambda row: [row[i].x for i in range(len(row))]).to_list()
+            points_df.apply(lambda row: [row_i.x for row_i in row.geoms]).to_list()
         )
         points["Y"] = numpy.concatenate(
-            points_df.apply(lambda row: [row[i].y for i in range(len(row))]).to_list()
+            points_df.apply(lambda row: [row_i.y for row_i in row.geoms]).to_list()
         )
         if self.z_label is None:
             points["Z"] = (
                 numpy.concatenate(
                     points_df.apply(
-                        lambda row: [row[i].z for i in range(len(row))]
+                        lambda row: [row_i.z for row_i in row.geoms]
                     ).to_list()
                 )
                 * -1
             )
         else:
             points["Z"] = (
                 numpy.concatenate(
                     [
-                        numpy.ones(len(points_df.loc[i]))
+                        numpy.ones(len(points_df.loc[i].geoms))
                         * self._contour[self.z_label].loc[i]
                         for i in range(len(points_df))
                     ]
                 )
                 * -1
             )
         return points
```

### Comparing `geofabrics-0.9.3a0/src/geofabrics/processor.py` & `geofabrics-0.9.4/src/geofabrics/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,14 +129,20 @@
         ]
 
         if key in self.instructions["data_paths"]:
             return True
         else:
             return key in defaults
 
+    def create_results_folder(self):
+        """Ensure the results folder has been created."""
+
+        results_folder = self.get_instruction_path("subfolder")
+        results_folder.mkdir(parents=True, exist_ok=True)
+
     def get_resolution(self) -> float:
         """Return the resolution from the instruction file. Raise an error if
         not in the instructions."""
 
         assert "output" in self.instructions, (
             "'output' is not a key-word in the instructions. It should exist"
             " and is where the resolution and optionally the CRS of the output"
@@ -528,14 +534,19 @@
     def run(self):
         """This method executes the geofabrics generation pipeline to produce geofabric
         derivatives.
 
         Note it currently only considers one LiDAR dataset that can have many tiles.
         See 'get_lidar_file_list' for where to change this."""
 
+        logging.info("Create a raw DEM layer from LiDAR.")
+
+        # Ensure the results folder has been created
+        self.create_results_folder()
+
         # Only include data in addition to LiDAR if the area_threshold is not covered
         area_threshold = 10.0 / 100  # Used to decide if bathymetry should be included
 
         # create the catchment geometry object
         self.catchment_geometry = self.create_catchment()
 
         # Get LiDAR data file-list - this may involve downloading lidar files
@@ -708,14 +719,17 @@
                 estimated_bathymetry=self.estimated_bathymetry_points
             )
 
     def run(self):
         """This method executes the geofabrics generation pipeline to produce geofabric
         derivatives."""
 
+        # Ensure the results folder has been created
+        self.create_results_folder()
+
         # Only include data in addition to LiDAR if the area_threshold is not covered
         area_threshold = 10.0 / 100  # Used to decide if bathymetry should be included
 
         # create the catchment geometry object
         self.catchment_geometry = self.create_catchment()
 
         # setup the hydrologically conditioned DEM generator
@@ -759,14 +773,19 @@
 
         self.roughness_dem = None
 
     def run(self):
         """This method executes the geofabrics generation pipeline to produce geofabric
         derivatives."""
 
+        logging.info("Adding a roughness layer to the geofabric.")
+
+        # Ensure the results folder has been created
+        self.create_results_folder()
+
         # create the catchment geometry object
         self.catchment_geometry = self.create_catchment()
 
         # Get LiDAR data file-list - this may involve downloading lidar files
         lidar_dataset_info = self.get_lidar_file_list("open_topography")
 
         # setup the roughness DEM generator
@@ -1579,15 +1598,18 @@
         fan_bathymetry.to_file(self.get_result_file_path(key="fan_bathymetry"))
 
     def run(self):
         """This method extracts a main channel then executes the DemGeneration
         pipeline to produce a DEM before sampling this to extimate width, slope
         and eventually depth."""
 
-        logging.info("Adding river and fan bathymetry if it doesn't already" "exist.")
+        logging.info("Adding river and fan bathymetry if it doesn't already exist.")
+
+        # Ensure the results folder has been created
+        self.create_results_folder()
 
         # Characterise river channel if not already done - may generate DEMs
         if not self.channel_characteristics_exist():
             buffer = 50
             self.characterise_channel(buffer=buffer)
         # Estimate channel and fan depths if not already done
         if not self.channel_bathymetry_exist():
@@ -1823,15 +1845,15 @@
         for drain_index, row in enumerate(points):
             row_bathymetries = [
                 max(
                     open_drains.iloc[drain_index]["start_elevation"],
                     open_drains.iloc[drain_index]["end_elevation"],
                 )
             ]
-            for point in row.geoms[1:]:
+            for point in list(row.geoms)[1:]:
                 elevation = float(dem.z.sel(x=point.x, y=point.y, method="nearest"))
                 row_bathymetries.append(
                     elevation
                     if elevation < row_bathymetries[-1]
                     else row_bathymetries[-1]
                 )
             bathymetries.extend(row_bathymetries)
@@ -1950,14 +1972,17 @@
 
         # Don't reprocess if already estimated
         if self.drain_bathymetry_exists():
             logging.info("Drain and tunnel bed elevations already estimated.")
             return
         logging.info("Estimating drain and tunnel bed elevation from OpenStreetMap.")
 
+        # Ensure the results folder has been created
+        self.create_results_folder()
+
         # Load in catchment
         self.catchment_geometry = self.create_catchment()
 
         # Download drains and tunnels from OSM
         drains = self.download_osm_values()
 
         # Create a DEM where the drains and tunnels are
```

### Comparing `geofabrics-0.9.3a0/src/geofabrics.egg-info/PKG-INFO` & `geofabrics-0.9.4/src/geofabrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geofabrics
-Version: 0.9.3a0
+Version: 0.9.4
 Summary: A package for creating geofabrics for flood modelling.
 Author-email: Rose pearson <rose.pearson@niwa.co.nz>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

