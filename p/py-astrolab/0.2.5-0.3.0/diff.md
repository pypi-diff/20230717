# Comparing `tmp/py_astrolab-0.2.5.tar.gz` & `tmp/py_astrolab-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_astrolab-0.2.5.tar", max compression
+gzip compressed data, was "py_astrolab-0.3.0.tar", max compression
```

## Comparing `py_astrolab-0.2.5.tar` & `py_astrolab-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.2.5/README.md
--rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.2.5/py_astrolab/__init__.py
--rwxr-xr-x   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.2.5/py_astrolab/aspects.py
--rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.2.5/py_astrolab/charts/__init__.py
--rwxr-xr-x   0        0        0    76352 2023-07-16 15:13:02.987613 py_astrolab-0.2.5/py_astrolab/charts/charts_svg.py
--rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.2.5/py_astrolab/charts/templates/basic.xml
--rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.2.5/py_astrolab/charts/templates/extended.xml
--rwxr-xr-x   0        0        0    63098 2023-07-16 14:01:21.996365 py_astrolab-0.2.5/py_astrolab/charts/templates/minimal.xml
--rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.2.5/py_astrolab/charts/wonderful_mistake.py
--rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.2.5/py_astrolab/fetch_geonames.py
--rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.2.5/py_astrolab/kr.config.json
--rwxr-xr-x   0        0        0    26831 2023-07-16 14:53:31.922402 py_astrolab-0.2.5/py_astrolab/main.py
--rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.2.5/py_astrolab/print_all_data.py
--rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.2.5/py_astrolab/relationship_score.py
--rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.2.5/py_astrolab/report.py
--rwxr-xr-x   0        0        0     5074 2023-07-12 12:49:41.885152 py_astrolab-0.2.5/py_astrolab/types.py
--rwxr-xr-x   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.2.5/py_astrolab/utilities.py
--rwxr-xr-x   0        0        0      689 2023-07-16 15:13:30.935106 py_astrolab-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.2.5/PKG-INFO
+-rwxr-xr-x   0        0        0       91 2023-06-17 10:19:25.525258 py_astrolab-0.3.0/README.md
+-rwxr-xr-x   0        0        0     5017 2023-05-29 18:14:56.433552 py_astrolab-0.3.0/py_astrolab/__init__.py
+-rwxr-xr-x   0        0        0    16866 2023-07-12 12:53:57.224268 py_astrolab-0.3.0/py_astrolab/aspects.py
+-rwxr-xr-x   0        0        0        0 2023-05-29 18:14:56.433552 py_astrolab-0.3.0/py_astrolab/charts/__init__.py
+-rwxr-xr-x   0        0        0    76352 2023-07-16 15:13:02.987613 py_astrolab-0.3.0/py_astrolab/charts/charts_svg.py
+-rwxr-xr-x   0        0        0    56568 2023-05-30 14:28:48.138660 py_astrolab-0.3.0/py_astrolab/charts/templates/basic.xml
+-rwxr-xr-x   0        0        0    56755 2023-05-30 14:28:36.593933 py_astrolab-0.3.0/py_astrolab/charts/templates/extended.xml
+-rwxr-xr-x   0        0        0    63098 2023-07-16 14:01:21.996365 py_astrolab-0.3.0/py_astrolab/charts/templates/minimal.xml
+-rwxr-xr-x   0        0        0    73370 2023-07-09 16:34:16.735355 py_astrolab-0.3.0/py_astrolab/charts/wonderful_mistake.py
+-rwxr-xr-x   0        0        0     5077 2023-05-29 18:14:56.449179 py_astrolab-0.3.0/py_astrolab/fetch_geonames.py
+-rwxr-xr-x   0        0        0    12935 2023-07-08 15:20:41.033613 py_astrolab-0.3.0/py_astrolab/kr.config.json
+-rwxr-xr-x   0        0        0    27129 2023-07-17 18:38:51.293335 py_astrolab-0.3.0/py_astrolab/main.py
+-rwxr-xr-x   0        0        0     3149 2023-06-17 10:10:20.258711 py_astrolab-0.3.0/py_astrolab/print_all_data.py
+-rwxr-xr-x   0        0        0     7785 2023-06-17 10:10:20.255187 py_astrolab-0.3.0/py_astrolab/relationship_score.py
+-rwxr-xr-x   0        0        0     2361 2023-07-12 12:55:07.631989 py_astrolab-0.3.0/py_astrolab/report.py
+-rwxr-xr-x   0        0        0     5143 2023-07-17 18:38:13.988880 py_astrolab-0.3.0/py_astrolab/types.py
+-rwxr-xr-x   0        0        0     7171 2023-07-12 13:18:34.934445 py_astrolab-0.3.0/py_astrolab/utilities.py
+-rwxr-xr-x   0        0        0      689 2023-07-17 18:44:09.425143 py_astrolab-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      835 1970-01-01 00:00:00.000000 py_astrolab-0.3.0/PKG-INFO
```

### Comparing `py_astrolab-0.2.5/py_astrolab/__init__.py` & `py_astrolab-0.3.0/py_astrolab/__init__.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/aspects.py` & `py_astrolab-0.3.0/py_astrolab/aspects.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/charts/charts_svg.py` & `py_astrolab-0.3.0/py_astrolab/charts/charts_svg.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/charts/templates/basic.xml` & `py_astrolab-0.3.0/py_astrolab/charts/templates/basic.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/charts/templates/extended.xml` & `py_astrolab-0.3.0/py_astrolab/charts/templates/extended.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/charts/templates/minimal.xml` & `py_astrolab-0.3.0/py_astrolab/charts/templates/minimal.xml`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/charts/wonderful_mistake.py` & `py_astrolab-0.3.0/py_astrolab/charts/wonderful_mistake.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/fetch_geonames.py` & `py_astrolab-0.3.0/py_astrolab/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/kr.config.json` & `py_astrolab-0.3.0/py_astrolab/kr.config.json`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/main.py` & `py_astrolab-0.3.0/py_astrolab/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -301,15 +301,15 @@
         if house_method not in house_methods:
             raise KerykeionException(f"The selected house method is not yet supported. Please, select one of these: {', '.join(house_methods.keys())}.")
         house_methods = {
             house_method: bytes(character, 'ascii') 
             for house_method, character in house_methods.items()}
         return house_methods[house_method]
 
-    def __axis(self) -> list:
+    def __axes(self) -> list:
         hsys = self.__get_hsys(self.house_method)
         swe_houses = swe.houses(julday=self.julian_day, lat=self.lat,
                                            lon=self.lng, hsys=hsys)
         ac = swe_houses[1][0]
         mc = swe_houses[1][1]
         dc = (ac + 180) % 360
         ic = (mc + 180) % 360
@@ -352,30 +352,36 @@
         jupiter_deg = swe.calc(self.julian_day, 5, self.__iflag)[0][0]
         saturn_deg = swe.calc(self.julian_day, 6, self.__iflag)[0][0]
         uranus_deg = swe.calc(self.julian_day, 7, self.__iflag)[0][0]
         neptune_deg = swe.calc(self.julian_day, 8, self.__iflag)[0][0]
         pluto_deg = swe.calc(self.julian_day, 9, self.__iflag)[0][0]
         mean_node_deg = swe.calc(self.julian_day, 10, self.__iflag)[0][0]
         true_node_deg = swe.calc(self.julian_day, 11, self.__iflag)[0][0]
-
-        # print(swe.calc(self.julian_day, 7, self.__iflag)[3])
+        mean_apog_deg = swe.calc(self.julian_day, 12, self.__iflag)[0][0]
+        # oscu_apog = swe.calc(self.julian_day, 13, self.__iflag)[0][0]
+        # earth = swe.calc(self.julian_day, 14, self.__iflag)[0][0]
+        # chiron_deg = swe.calc(self.julian_day, 15, self.__iflag)[0][0]
 
         self.planets_degrees = [
             sun_deg,
             moon_deg,
             mercury_deg,
             venus_deg,
             mars_deg,
             jupiter_deg,
             saturn_deg,
             uranus_deg,
             neptune_deg,
             pluto_deg,
             mean_node_deg,
-            true_node_deg
+            true_node_deg,
+            mean_apog_deg
+            # None,
+            # None,
+            # chiron_deg
         ]
 
         return self.planets_degrees
 
     def __planets(self) -> None:
         """ Defines body positon in signs and information and
          stores them in dictionaries """
@@ -414,36 +420,27 @@
         )
         self.mean_node = calculate_position(
             self.planets_degrees[10], "Mean_Node", point_type=point_type
         )
         self.true_node = calculate_position(
             self.planets_degrees[11], "True_Node", point_type=point_type
         )
-
-    def __axes(self) -> None:
-        point_type = "Axis"
-        self.ascendant = calculate_position(
-            self.planets_degrees[0], "Sun", point_type=point_type
-        )
-        self.midheaven = calculate_position(
-            self.planets_degrees[0], "Sun", point_type=point_type
-        )
-        self.descendant = calculate_position(
-            self.planets_degrees[0], "Sun", point_type=point_type
-        )
-        self.imum_coeli = calculate_position(
-            self.planets_degrees[0], "Sun", point_type=point_type
+        self.mean_apog = calculate_position(
+            self.planets_degrees[12], "Mean_Apog", point_type=point_type
         )
+        # self.chiron = calculate_position(
+        #     self.planets_degrees[15], "Chiron", point_type=point_type
+        # )
 
     def __planets_in_houses(self):
         """Calculates the house of the planet and updates
         the planets dictionary."""
         self.__planets()
         self.__houses()
-        self.__axis()
+        self.__axes()
 
         def for_every_planet(planet, planet_deg):
             """Function to do the calculation.
             Args: planet dictionary, planet degree"""
 
             def point_between(p1, p2, p3):
                 """Finds if a point is between two other in a circle
@@ -528,14 +525,20 @@
         )
         self.mean_node = for_every_planet(
             self.mean_node, self.planets_degrees[10]
         )
         self.true_node = for_every_planet(
             self.true_node, self.planets_degrees[11]
         )
+        self.mean_apog = for_every_planet(
+            self.mean_apog, self.planets_degrees[12]
+        )
+        # self.chiron = for_every_planet(
+        #     self.chiron, self.planets_degrees[15]
+        # )
         self.ascendant = for_every_planet(
             self.ascendant, self.ascendant['abs_pos']
         )
         self.midheaven = for_every_planet(
             self.midheaven, self.midheaven['abs_pos']
         )
         self.descendant = for_every_planet(
@@ -554,14 +557,16 @@
             self.jupiter,
             self.saturn,
             self.uranus,
             self.neptune,
             self.pluto,
             self.mean_node,
             self.true_node
+            # self.mean_apog
+            # self.chiron
         ]
 
         # Check in retrograde or not:
         planets_ret = []
         for p in planets_list:
             planet_number = get_number_from_name(p["name"])
             if swe.calc(self.julian_day, planet_number, self.__iflag)[0][3] < 0:
```

### Comparing `py_astrolab-0.2.5/py_astrolab/print_all_data.py` & `py_astrolab-0.3.0/py_astrolab/print_all_data.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/relationship_score.py` & `py_astrolab-0.3.0/py_astrolab/relationship_score.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/report.py` & `py_astrolab-0.3.0/py_astrolab/report.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/py_astrolab/types.py` & `py_astrolab-0.3.0/py_astrolab/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,15 +64,16 @@
     "Mars",
     "Jupiter",
     "Saturn",
     "Uranus",
     "Neptune",
     "Pluto",
     "Mean_Node",
-    "True_Node"
+    "True_Node",
+    "Mean_Apog"
 ]
 
 Axis = Literal[
     "Ascendant",
     "Midheaven",
     "Descendant",
     "Imum Coeli"
@@ -219,14 +220,17 @@
     descendant: KerykeionPoint
     imum_coeli: KerykeionPoint
 
     # Nodes
     mean_node: KerykeionPoint
     true_node: KerykeionPoint
 
+    # Black Moon
+    mean_apog: KerykeionPoint
+
     # Lunar Phase
     lunar_phase: LunarPhaseObject
 
 if __name__ == "__main__":
     sun = KerykeionPoint(
         name='Sun',
         element='Air',
```

### Comparing `py_astrolab-0.2.5/py_astrolab/utilities.py` & `py_astrolab-0.3.0/py_astrolab/utilities.py`

 * *Files identical despite different names*

### Comparing `py_astrolab-0.2.5/pyproject.toml` & `py_astrolab-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "py-astrolab"
-version = "0.2.5"
+version = "0.3.0"
 description = "A Python interface on Swiss Ephemeris to perform astrological calculations"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>", "Arcangelo Massari <arcangelomas@gmail.com>"]
 license = "GNU General Public License (GPL)"
 readme = "README.md"
 packages = [{include = "py_astrolab"}]
 
 [tool.poetry.dependencies]
```

### Comparing `py_astrolab-0.2.5/PKG-INFO` & `py_astrolab-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-astrolab
-Version: 0.2.5
+Version: 0.3.0
 Summary: A Python interface on Swiss Ephemeris to perform astrological calculations
 License: GNU General Public License (GPL)
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<3.10
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

