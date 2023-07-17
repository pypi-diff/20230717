# Comparing `tmp/sdss_lvmscp-0.5.1.tar.gz` & `tmp/sdss_lvmscp-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmscp-0.5.1.tar", max compression
+gzip compressed data, was "sdss_lvmscp-0.5.2.tar", max compression
```

## Comparing `sdss_lvmscp-0.5.1.tar` & `sdss_lvmscp-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1504 2023-07-13 23:26:28.638223 sdss_lvmscp-0.5.1/LICENSE.md
--rw-r--r--   0        0        0     1578 2023-07-13 23:26:28.638685 sdss_lvmscp-0.5.1/README.md
--rw-r--r--   0        0        0     2715 2023-07-13 23:26:28.702215 sdss_lvmscp-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      369 2023-07-13 23:26:28.703298 sdss_lvmscp-0.5.1/python/lvmscp/__init__.py
--rw-r--r--   0        0        0     1618 2023-07-13 23:26:28.703789 sdss_lvmscp-0.5.1/python/lvmscp/__main__.py
--rw-r--r--   0        0        0      258 2023-07-13 23:26:28.704155 sdss_lvmscp-0.5.1/python/lvmscp/actor/__init__.py
--rw-r--r--   0        0        0     8321 2023-07-13 23:26:28.704512 sdss_lvmscp-0.5.1/python/lvmscp/actor/actor.py
--rw-r--r--   0        0        0      859 2023-07-13 23:26:28.705060 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/__init__.py
--rw-r--r--   0        0        0     1515 2023-07-13 23:26:28.705354 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/expose.py
--rw-r--r--   0        0        0     3827 2023-07-13 23:26:28.705730 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/focus.py
--rw-r--r--   0        0        0     1272 2023-07-13 23:26:28.706014 sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/hardware_status.py
--rw-r--r--   0        0        0      758 2023-07-13 23:26:28.706314 sdss_lvmscp-0.5.1/python/lvmscp/controller.py
--rw-r--r--   0        0        0    13581 2023-07-13 23:26:28.706624 sdss_lvmscp-0.5.1/python/lvmscp/delegate.py
--rw-r--r--   0        0        0    40775 2023-07-13 23:26:28.707229 sdss_lvmscp-0.5.1/python/lvmscp/etc/LVM_100kHz.acf
--rw-r--r--   0        0        0     5466 2023-07-13 23:26:28.707967 sdss_lvmscp-0.5.1/python/lvmscp/etc/lvmscp.yml
--rw-r--r--   0        0        0      161 2023-07-13 23:26:28.708248 sdss_lvmscp-0.5.1/python/lvmscp/etc/schema.json
--rw-r--r--   0        0        0    18807 2023-07-13 23:26:28.708730 sdss_lvmscp-0.5.1/python/lvmscp/ln2.py
--rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2023-07-17 21:19:01.855097 sdss_lvmscp-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0     1578 2023-07-17 21:19:01.855381 sdss_lvmscp-0.5.2/README.md
+-rw-r--r--   0        0        0     2715 2023-07-17 21:19:03.919656 sdss_lvmscp-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      369 2023-07-17 21:19:03.920422 sdss_lvmscp-0.5.2/python/lvmscp/__init__.py
+-rw-r--r--   0        0        0     1618 2023-07-17 21:19:03.920800 sdss_lvmscp-0.5.2/python/lvmscp/__main__.py
+-rw-r--r--   0        0        0      258 2023-07-17 21:19:03.921295 sdss_lvmscp-0.5.2/python/lvmscp/actor/__init__.py
+-rw-r--r--   0        0        0     8321 2023-07-17 21:19:03.921704 sdss_lvmscp-0.5.2/python/lvmscp/actor/actor.py
+-rw-r--r--   0        0        0      859 2023-07-17 21:19:03.922201 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1515 2023-07-17 21:19:03.922558 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/expose.py
+-rw-r--r--   0        0        0     3827 2023-07-17 21:19:03.922963 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/focus.py
+-rw-r--r--   0        0        0     1272 2023-07-17 21:19:03.923301 sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/hardware_status.py
+-rw-r--r--   0        0        0      758 2023-07-17 21:19:03.923644 sdss_lvmscp-0.5.2/python/lvmscp/controller.py
+-rw-r--r--   0        0        0    13727 2023-07-17 21:19:03.924065 sdss_lvmscp-0.5.2/python/lvmscp/delegate.py
+-rw-r--r--   0        0        0    40775 2023-07-17 21:19:03.924729 sdss_lvmscp-0.5.2/python/lvmscp/etc/LVM_100kHz.acf
+-rw-r--r--   0        0        0     5736 2023-07-17 21:19:03.925225 sdss_lvmscp-0.5.2/python/lvmscp/etc/lvmscp.yml
+-rw-r--r--   0        0        0      161 2023-07-17 21:19:03.925605 sdss_lvmscp-0.5.2/python/lvmscp/etc/schema.json
+-rw-r--r--   0        0        0    18807 2023-07-17 21:19:03.926089 sdss_lvmscp-0.5.2/python/lvmscp/ln2.py
+-rw-r--r--   0        0        0     2812 1970-01-01 00:00:00.000000 sdss_lvmscp-0.5.2/PKG-INFO
```

### Comparing `sdss_lvmscp-0.5.1/LICENSE.md` & `sdss_lvmscp-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/README.md` & `sdss_lvmscp-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/pyproject.toml` & `sdss_lvmscp-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmscp"
-version = "0.5.1"
+version = "0.5.2"
 description = "LVM spectrograph control package."
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>"]
 maintainers = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmscp"
 repository = "https://github.com/sdss/lvmscp"
```

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/__main__.py` & `sdss_lvmscp-0.5.2/python/lvmscp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/actor/actor.py` & `sdss_lvmscp-0.5.2/python/lvmscp/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/__init__.py` & `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/expose.py` & `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/focus.py` & `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/actor/commands/hardware_status.py` & `sdss_lvmscp-0.5.2/python/lvmscp/actor/commands/hardware_status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/controller.py` & `sdss_lvmscp-0.5.2/python/lvmscp/controller.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/delegate.py` & `sdss_lvmscp-0.5.2/python/lvmscp/delegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -338,45 +338,47 @@
                     f"lvm.{telescope}.km",
                     "status",
                     internal=True,
                 )
                 if km_cmd.status.did_fail:
                     self.command.warning(f"Failed getting {telescope} k-mirror status.")
                 else:
-                    km_position = km_cmd.replies.get("Position")
+                    km_position = numpy.round(km_cmd.replies.get("Position"), 2)
 
             foc_cmd = await self.command.send_command(
                 f"lvm.{telescope}.foc",
                 "status",
                 internal=True,
             )
             if foc_cmd.status.did_fail:
                 self.command.warning(f"Failed getting {telescope} focus status.")
             else:
-                foc_position = foc_cmd.replies.get("Position")
+                foc_position = numpy.round(foc_cmd.replies.get("Position"), 2)
 
             for key in keys:
                 if key == "km" and telescope == "spec":
                     continue
 
                 if key == "km":
                     data[f"{telescope}km"] = (km_position, "K-mirror position [deg]")
                 elif key == "foc":
                     data[f"{telescope}foc"] = (foc_position, "Focuser position [deg]")
                 elif key == "ra":
                     ra_h: float = pwi_status.get("ra_j2000_hours", -999.0)
                     if ra_h > 0:
                         ra_h *= 15.0
+                        ra_h = numpy.round(ra_h, 6)
                     data[f"{telescope}ra"] = (ra_h, "Telescope pointing RA [deg]")
                 elif key == "dec":
                     dec = pwi_status.get("dec_j2000_degs", -999.0)
+                    dec = numpy.round(dec, 6)
                     data[f"{telescope}dec"] = (dec, "Telescope pointing Dec [deg]")
                 elif key == "airm":
                     alt = pwi_status.get("altitude_degs", None)
                     comment = "Telescope airmass"
                     if alt is None:
                         data[f"{telescope}airm"] = (-999.0, comment)
                     else:
-                        airm = 1 / numpy.cos(numpy.radians(90 - alt))
+                        airm = numpy.round(1 / numpy.cos(numpy.radians(90 - alt)), 3)
                         data[f"{telescope}airm"] = (airm, comment)
 
         return data
```

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/etc/LVM_100kHz.acf` & `sdss_lvmscp-0.5.2/python/lvmscp/etc/LVM_100kHz.acf`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/etc/lvmscp.yml` & `sdss_lvmscp-0.5.2/python/lvmscp/etc/lvmscp.yml`

 * *Files 9% similar despite different names*

```diff
@@ -112,18 +112,22 @@
       z1: ['mod12/tempb', 'LN2 temperature (HEATERX 12)', 2]
       r2: ['mod2/tempb', 'Temperature of the sensor (HEATERX 2)', 2]
       b2: ['mod2/tempc', 'Temperature of the sensor (HEATERX 12)', 2]
       z2: ['mod12/tempb', 'Temperature of the sensor (HEATERX 12)', 2]
       r3: ['mod2/tempb', 'Temperature of the sensor (HEATERX 2)', 2]
       b3: ['mod2/tempc', 'Temperature of the sensor (HEATERX 12)', 2]
       z3: ['mod12/tempb', 'Temperature of the sensor (HEATERX 12)', 2]
-  DATASEC: ['[1:4120,1:4080]', 'Section of the detector containing data']
-  CCDSEC: ['[1:4120,1:4080]', 'Section of the detector read out']
-  BIASSEC: ['[2041:2080,1:4080]', 'Section of calibration/bias data']
-  TRIMSEC: ['[1:2040,1:4080],[2081:4120,1:4080]', 'Section with useful data']
+  TRIMSEC1: ['[1:2043, 2041:4080]', 'Data section for quadrant 1']
+  TRIMSEC2: ['[2078:4120, 2041:4080]', 'Data section for quadrant 2']
+  TRIMSEC3: ['[1:2043, 1:2040]', 'Data section for quadrant 3']
+  TRIMSEC4: ['[2078:4120, 1:2040]', 'Data section for quadrant 4']
+  BIASSEC1: ['[2044:2060, 2041:4080]', 'Overscan section for quadrant 1']
+  BIASSEC2: ['[2061:2077, 2041:4080]', 'Overscan section for quadrant 2']
+  BIASSEC3: ['[2044:2060, 1:2040]', 'Overscan section for quadrant 3']
+  BIASSEC4: ['[2061:2077, 1:2040]', 'Overscan section for quadrant 4']
 
 # This is the ACF configuration file to be loaded to the Archon including the
 # timing script. {archon_etc} gets completed with the path of the etc directory once
 # installed. If the path is not absolute, the root of the package is used as working
 # directory.
 archon:
   acf_file: LVM_100kHz.acf
```

### Comparing `sdss_lvmscp-0.5.1/python/lvmscp/ln2.py` & `sdss_lvmscp-0.5.2/python/lvmscp/ln2.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmscp-0.5.1/PKG-INFO` & `sdss_lvmscp-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmscp
-Version: 0.5.1
+Version: 0.5.2
 Summary: LVM spectrograph control package.
 Home-page: https://github.com/sdss/lvmscp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Maintainer: José Sánchez-Gallego
```

