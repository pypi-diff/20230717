# Comparing `tmp/SplatStats-2.1.1.tar.gz` & `tmp/SplatStats-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SplatStats-2.1.1.tar", last modified: Fri Jun  2 04:01:57 2023, max compression
+gzip compressed data, was "SplatStats-2.1.5.tar", last modified: Mon Jul 17 16:25:53 2023, max compression
```

## Comparing `SplatStats-2.1.1.tar` & `SplatStats-2.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.820232 SplatStats-2.1.1/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.1.1/LICENSE
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-02 04:01:57.820075 SplatStats-2.1.1/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.1.1/README.md
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.818949 SplatStats-2.1.1/SplatStats/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Battle.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Player.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/StatInk.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/Team.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/__init__.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats/_version.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/auxiliary.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    13972 2023-05-18 20:39:55.000000 SplatStats-2.1.1/SplatStats/colors.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5499 2023-05-16 16:38:00.000000 SplatStats-2.1.1/SplatStats/constants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/files.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/parsers.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plotsAux.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/plotsTeam.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10727 2023-06-02 03:50:03.000000 SplatStats-2.1.1/SplatStats/statInkConstants.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10588 2023-05-18 23:06:43.000000 SplatStats-2.1.1/SplatStats/statInkPlots.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.1.1/SplatStats/statInkStats.py
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.1.1/SplatStats/stats.py
-drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-06-02 04:01:57.819868 SplatStats-2.1.1/SplatStats.egg-info/
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/PKG-INFO
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/SOURCES.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/dependency_links.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/requires.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-06-02 04:01:57.000000 SplatStats-2.1.1/SplatStats.egg-info/top_level.txt
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-06-02 04:01:57.820278 SplatStats-2.1.1/setup.cfg
--rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.1.1/setup.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 16:25:53.827024 SplatStats-2.1.5/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    35149 2023-05-11 17:29:12.000000 SplatStats-2.1.5/LICENSE
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-17 16:25:53.826761 SplatStats-2.1.5/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6367 2023-05-29 20:06:53.000000 SplatStats-2.1.5/README.md
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 16:25:53.825701 SplatStats-2.1.5/SplatStats/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10828 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/Battle.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10398 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/Player.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     3058 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/StatInk.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     2477 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/Team.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      896 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/__init__.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       21 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats/_version.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6148 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/auxiliary.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14036 2023-07-17 16:23:54.000000 SplatStats-2.1.5/SplatStats/colors.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     5905 2023-06-06 02:59:04.000000 SplatStats-2.1.5/SplatStats/constants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     4137 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/files.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8663 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/parsers.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    56269 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/plots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1428 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/plotsAux.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1709 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/plotsTeam.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10747 2023-06-05 15:46:16.000000 SplatStats-2.1.5/SplatStats/statInkConstants.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    10625 2023-06-05 15:55:49.000000 SplatStats-2.1.5/SplatStats/statInkPlots.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     8511 2023-05-11 17:29:12.000000 SplatStats-2.1.5/SplatStats/statInkStats.py
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)    14368 2023-05-29 19:37:30.000000 SplatStats-2.1.5/SplatStats/stats.py
+drwxr-xr-x   0 sanchez.hmsc   (503) staff       (20)        0 2023-07-17 16:25:53.826575 SplatStats-2.1.5/SplatStats.egg-info/
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     6747 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats.egg-info/PKG-INFO
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      607 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats.egg-info/SOURCES.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)        1 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats.egg-info/dependency_links.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)      159 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats.egg-info/requires.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       11 2023-07-17 16:25:53.000000 SplatStats-2.1.5/SplatStats.egg-info/top_level.txt
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)       38 2023-07-17 16:25:53.827079 SplatStats-2.1.5/setup.cfg
+-rw-r--r--   0 sanchez.hmsc   (503) staff       (20)     1251 2023-05-11 17:29:12.000000 SplatStats-2.1.5/setup.py
```

### Comparing `SplatStats-2.1.1/LICENSE` & `SplatStats-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/PKG-INFO` & `SplatStats-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.1.1
+Version: 2.1.5
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.1.1/README.md` & `SplatStats-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/Battle.py` & `SplatStats-2.1.5/SplatStats/Battle.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/Player.py` & `SplatStats-2.1.5/SplatStats/Player.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/StatInk.py` & `SplatStats-2.1.5/SplatStats/StatInk.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/Team.py` & `SplatStats-2.1.5/SplatStats/Team.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/__init__.py` & `SplatStats-2.1.5/SplatStats/__init__.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/auxiliary.py` & `SplatStats-2.1.5/SplatStats/auxiliary.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/colors.py` & `SplatStats-2.1.5/SplatStats/colors.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 ROCK_PAPER_SCISSORS_S3      = ('#413BBA', '#BEB013', '#C03E3E', '#35BA49')
 GEAR_GRUB_FUN_S3            = ('#8A19F7', '#BE7118', '#28C05E', '#3F2CD2')
 GRASS_FIRE_WATER_S3         = ('#1BA974', '#DA4514', '#002AFF', '#FFFF00')
 SPICY_SWEET_SOUR_S3         = ('#AD5438', '#9A6FCC', '#A5B533', '#00A2E8')
 DARK_MILK_WHITE_S3          = ('#3D1F7A', '#995935', '#D6BF8F', '#FFFF00')
 NESSIE_ALIENS_BIGFOOT_S3    = ('#118F32', '#793199', '#A1482B', '#0935A6')
 POWER_WISDOM_COURAGE_S3     = ('#AB2A5C', '#488DB5', '#03A65F')
+VANILLA_STRAWBERRY_MINT_S3  = ('#cca770', '#bc6d75', '#2ac29e')
 # Return of the Mammalians ----------------------------------------------------
 ORANGE_V_BLUE_S3            = ('#EE8711', '#0943F0', '#81DE17')
 YELLOW_V_INDIGO_S3          = ('#DEC109', '#531BBA', '#C920B7')
 GREEN_V_BLUE_S3             = ('#51C71B', '#2120CC', '#C920B7')
 SODA_V_MAGENTA_S3           = ('#AEF4F0', '#DD0DD3', '#C6D314')
 LBLUE_V_BLUE_S3             = ('#14BBE7', '#285EEA', '#C920B7')
 BLUE_V_MAGENTA_S3           = ('#1B18D7', '#DD0DD3', '#C6D314')
```

### Comparing `SplatStats-2.1.1/SplatStats/constants.py` & `SplatStats-2.1.5/SplatStats/constants.py`

 * *Files 5% similar despite different names*

```diff
@@ -105,15 +105,19 @@
     clr.DBLUE_V_YELLOW_S1[0],
     clr.YELLOW_V_DTEAL_LK_S3[0], clr.YELLOW_V_DTEAL_LK_S3[1], clr.YELLOW_V_DTEAL_LK_S3[2],
     clr.WINNERW_V_WOUTERW_S2[0], clr.WINNERW_V_WOUTERW_S2[1], clr.WINNERW_V_WOUTERW_S2[2],
     clr.LPINK_V_BLUE_S2[0], clr.LPINK_V_BLUE_S2[1],
     clr.NPINK_V_NGREEN_S2[1], 
     clr.RASPBERRY_V_NYELLOW_S2[1],
     clr.YELLOW_V_LBLU_V_DBLU_LK_S3[1], clr.BLUE_FRYE_S3[2],
-    clr.GRAPE_V_TURQUOISE_S2[0], clr.GRAPE_V_TURQUOISE_S2[1]
+    clr.GRAPE_V_TURQUOISE_S2[0], clr.GRAPE_V_TURQUOISE_S2[1],
+    clr.PBODY_V_PBRAIN_S1[0], clr.PBODY_V_PBRAIN_S1[1],
+    clr.SGREEN_V_GRAPE_S2[0], clr.SGREEN_V_GRAPE_S2[1], clr.SGREEN_V_GRAPE_S2[2],
+    clr.TEAL_PURPLE_ORANGE_S3[0], clr.TEAL_PURPLE_ORANGE_S3[1], clr.TEAL_PURPLE_ORANGE_S3[2], clr.TEAL_PURPLE_ORANGE_S3[3],
+    clr.YELLOW_V_LBLU_V_DBLU_LK_S3[0], clr.YELLOW_V_LBLU_V_DBLU_LK_S3[1], clr.YELLOW_V_LBLU_V_DBLU_LK_S3[2], clr.YELLOW_V_LBLU_V_DBLU_LK_S3[3]
 ]
 CLR_BAR = clr.SMUSHROOM_V_SSTAR_S2[-1]
 ###############################################################################
 # Weapons Classes
 ###############################################################################
 WPN_CLASS = {
     'Blaster': {
```

### Comparing `SplatStats-2.1.1/SplatStats/files.py` & `SplatStats-2.1.5/SplatStats/files.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/parsers.py` & `SplatStats-2.1.5/SplatStats/parsers.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/plots.py` & `SplatStats-2.1.5/SplatStats/plots.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/plotsAux.py` & `SplatStats-2.1.5/SplatStats/plotsAux.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/plotsTeam.py` & `SplatStats-2.1.5/SplatStats/plotsTeam.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/statInkConstants.py` & `SplatStats-2.1.5/SplatStats/statInkConstants.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 LOBBY_MODE = {
   'regular': 'Regular',
   'bankara_challenge': 'Anarchy (Series)',
   'bankara_open': 'Anarchy (Open)',
   'xmatch': 'X Battle',
   'splatfest_challenge': 'Splatfest (Pro)',
-  'splatfest_open': 'Splatfest (Open)'
+  'splatfest_open': 'Splatfest (Open)',
+  'event': 'Event'
 }
 
 WPNS_DICT = {
   '52gal': '.52 Gal',
   '96gal': '.96 Gal',
   '96gal_deco': '.96 Gal Deco',
   'bold': 'Sploosh-o-matic',
```

### Comparing `SplatStats-2.1.1/SplatStats/statInkPlots.py` & `SplatStats-2.1.5/SplatStats/statInkPlots.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,17 @@
 
 def barChartLobby(
         lbyFreq,
         figAx=None,
         scaler=('k', 1e3),
         fontSizes=(8.5, 20),
         colors=[
-            '#2E0CB5', '#B400FF', '#6BFF00', '#525CF5', '#FDFF00', '#D01D79'
+            '#2E0CB5', '#B400FF', '#6BFF00', 
+            '#525CF5', '#FDFF00', '#D01D79', 
+            '#E2E2E2'
         ]
     ):
     (series, data) = (
         list(lbyFreq.keys()), [[int(i)] for i in list(lbyFreq.values())]
     )
     data = [[i[0]/scaler[1]] for i in data]
     if figAx:
```

### Comparing `SplatStats-2.1.1/SplatStats/statInkStats.py` & `SplatStats-2.1.5/SplatStats/statInkStats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats/stats.py` & `SplatStats-2.1.5/SplatStats/stats.py`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/SplatStats.egg-info/PKG-INFO` & `SplatStats-2.1.5/SplatStats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SplatStats
-Version: 2.1.1
+Version: 2.1.5
 Home-page: https://github.com/Chipdelmal/SplatStats
 Author: chipdelmal
 Author-email: chipdelmal@gmail.com
 License: GPLv3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `SplatStats-2.1.1/SplatStats.egg-info/SOURCES.txt` & `SplatStats-2.1.5/SplatStats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SplatStats-2.1.1/setup.py` & `SplatStats-2.1.5/setup.py`

 * *Files identical despite different names*

