# Comparing `tmp/captif_cpx_db-0.9.tar.gz` & `tmp/captif_cpx_db-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.9.tar", max compression
+gzip compressed data, was "captif_cpx_db-1.0.0.tar", max compression
```

## Comparing `captif_cpx_db-0.9.tar` & `captif_cpx_db-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/LICENSE
--rw-r--r--   0        0        0       16 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/README.md
--rw-r--r--   0        0        0      334 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0    27546 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/captif_cpx_db/models.py
--rw-r--r--   0        0        0      523 2023-06-22 23:21:17.142681 captif_cpx_db-0.9/pyproject.toml
--rw-r--r--   0        0        0      534 1970-01-01 00:00:00.000000 captif_cpx_db-0.9/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/LICENSE
+-rw-r--r--   0        0        0       16 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/README.md
+-rw-r--r--   0        0        0      765 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0    29312 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/captif_cpx_db/models.py
+-rw-r--r--   0        0        0       22 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/captif_cpx_db/version.py
+-rw-r--r--   0        0        0      525 2023-07-17 09:44:05.963917 captif_cpx_db-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      536 1970-01-01 00:00:00.000000 captif_cpx_db-1.0.0/PKG-INFO
```

### Comparing `captif_cpx_db-0.9/LICENSE` & `captif_cpx_db-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.9/captif_cpx_db/models.py` & `captif_cpx_db-1.0.0/captif_cpx_db/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 from datetime import date as date_
 from pydantic import condecimal, validator
-from shapely.wkt import loads
+from shapely.wkt import loads as wkt_loads
+from shapely.wkb import loads as wkb_loads
 from sqlalchemy import ForeignKeyConstraint as ForeignKeyConstraint_
-from sqlmodel import Field, SQLModel, Relationship
+from sqlmodel import Field, SQLModel
+from sqlmodel import Relationship as Relationship_
 from typing import List, Optional
 
+from .version import __version__
+
 
 def ForeignKeyConstraint(*args, **kwargs):
     return ForeignKeyConstraint_(
         *args,
         **kwargs,
         onupdate="CASCADE",
-        ondelete="RESTRICT",
+        ondelete="CASCADE",
+    )
+
+
+def Relationship(*args, **kwargs):
+    return Relationship_(
+        *args,
+        **kwargs,
+        sa_relationship_kwargs={
+            "cascade": "all, delete-orphan",
+        },
     )
 
 
 """
 Measurement-level models
 
 """
@@ -63,22 +77,41 @@
     wav_scale: condecimal(decimal_places=1) = Field(
         nullable=False,
         description=(
             "scale factor to apply to the raw wav file data (-1 to + 1 range) "
             "to convert the data back into volts."
         ),
     )
+    measurement_group_date: Optional[date_] = Field(
+        nullable=False,
+        description=(
+            "date used for grouping repeat runs performed across difference "
+            "measurement sessions. Defaults to the measurement date if not "
+            "specified."
+        ),
+    )
+    measurement_session_path: Optional[str] = Field(
+        nullable=False,
+        description=(
+            "measurement session path, relative to the 'Measurement files' "
+            "SharePoint folder"
+        ),
+    )
     notes: Optional[str] = Field(
         default=None,
         description="other notes about the measurement",
     )
 
     results_sets: List["ResultsSet"] = Relationship()
     wheel_bay_details: List["MeasurementWheelBayDetails"] = Relationship()
 
+    @validator("measurement_group_date", always=True)
+    def measurement_group_date_validator(cls, v, values):
+        return values.get("date") if v is None else v
+
 
 class MeasurementWheelBayDetails(SQLModel, table=True):
     """
     Measurement-level wheel bay details for a given results set. Each results
     set can have up to two wheel bay entries.
     """
 
@@ -279,14 +312,19 @@
         default=None,
         primary_key=True,
     )
     software_version: str = Field(
         nullable=False,
         description=("processing software version used to generate the results set"),
     )
+    database_version: str = Field(
+        default=__version__,
+        nullable=False,
+        description=("database version used to generate the results set"),
+    )
     segment_length_m: Optional[condecimal(decimal_places=1)] = Field(
         default=None,
         description=(
             "length of the road segment in metres. Set to None if results use "
             "a variable segment length."
         ),
     )
@@ -314,14 +352,21 @@
     )
     gps_acceleration_threshold_kph_sec: condecimal(decimal_places=2) = Field(
         nullable=False,
         description=(
             "threshold for determining if the GPS acceleration is valid in " "km/h/sec"
         ),
     )
+    max_gps_interpolation_distance_m: condecimal(decimal_places=1) = Field(
+        nullable=False,
+        description=(
+            "the maximum distance between GPS points before road segments are "
+            "marked as using estimated GPS data"
+        ),
+    )
     rsrp_database: str = Field(
         nullable=False,
         description=("name of the Rs/Rp database used to generate the results set"),
     )
     rsrp_date: date_ = Field(
         nullable=False,
         description="date that the Rs/Rp database was accessed",
@@ -463,15 +508,15 @@
         default=None,
         primary_key=True,
     )
     wav_path: str = Field(
         nullable=False,
         description=(
             "path to the wav file associated with the segment result "
-            "(relative to the SharePoint measurement files folder)"
+            "relative to the measurement session folder)"
         ),
     )
     run_number: int = Field(
         nullable=False,
         description=(
             "run number as per the measurement files. This cannot be relied "
             "on when determining the number of runs across a given road "
@@ -491,29 +536,29 @@
             "the results set."
         ),
     )
     road_id: int = Field(
         nullable=False,
         description="RAMM road ID",
     )
-    start_m: condecimal(decimal_places=1) = Field(
+    start_m: float = Field(
         nullable=False,
         description=(
             "start position of the road segment in metres (Rs/Rp route "
             "position). 'start_m' is always lower than 'end_m'."
         ),
     )
-    end_m: condecimal(decimal_places=1) = Field(
+    end_m: float = Field(
         nullable=False,
         description=(
             "end position of the road segment in metres (Rs/Rp route "
             "position). 'end_'m' is always higher than 'start_m'."
         ),
     )
-    length_m: condecimal(decimal_places=1) = Field(
+    length_m: float = Field(
         nullable=False,
         description="length of the road segment in metres",
     )
     lane: str = Field(
         nullable=False,
         description="RAMM lane number (e.g. 'L1', 'L2', 'R1', 'R2', etc)",
     )
@@ -569,41 +614,52 @@
         default=False,
         description="passing truck (true/false)",
     )
     other_flag: Optional[bool] = Field(
         default=False,
         description="other flag (true/false)",
     )
+    gps_estimate: Optional[bool] = Field(
+        default=False,
+        description=(
+            "whether or not the GPS position is considered an estimate, based "
+            "on the distance to the nearest GPS reading and the "
+            "max_interpolation_distance_m value"
+        ),
+    )
     valid: bool = Field(
         nullable=False,
         description=(
             "indicates whether the road segment results are valid or not, "
             "based on the speed and any event flags"
         ),
     )
-    geometry: str = Field(
+    geometry: bytes = Field(
         nullable=False,
-        description="RAMM centreline geometry of the road segment",
+        description=(
+            "RAMM centreline geometry of the road segment. The field can be "
+            "specified as a WKT LINESTRING; however, it will be converted to "
+            "WKB when stored in the database."
+        ),
     )
 
     wheel_bay_details: List["SegmentWheelBayDetails"] = Relationship()
 
     @validator("start_m", "end_m", "length_m", pre=True)
     def round_1(cls, v):
         return round(v, 1) if v is not None else None
 
-    @validator("geometry")
+    @validator("geometry", pre=True)
     def validate_linestring(cls, v):
         try:
-            linestring = loads(v)
-            if not linestring.is_valid or linestring.geom_type != "LineString":
-                raise ValueError("Invalid WKT LINESTRING")
+            linestring = wkt_loads(v) if isinstance(v, str) else wkb_loads(v)
         except Exception as e:
-            raise ValueError("Invalid WKT LINESTRING") from e
-        return v
+            raise ValueError("Invalid WKT/WKB LINESTRING") from e
+
+        return linestring.wkb
 
 
 class SegmentWheelBayDetails(SQLModel, table=True):
     """
     Segment-level (results set) wheel bay details.
     """
```

### Comparing `captif_cpx_db-0.9/pyproject.toml` & `captif_cpx_db-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "captif-cpx-db"
-version = "0.9"
+version = "1.0.0"
 description = ""
 authors = ["John Bull <john.bull@nzta.govt.nz>"]
 readme = "README.md"
 packages = [{include = "captif_cpx_db"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `captif_cpx_db-0.9/PKG-INFO` & `captif_cpx_db-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-db
-Version: 0.9
+Version: 1.0.0
 Summary: 
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

