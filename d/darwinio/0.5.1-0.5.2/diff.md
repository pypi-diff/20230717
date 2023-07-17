# Comparing `tmp/darwinio-0.5.1.tar.gz` & `tmp/darwinio-0.5.2.tar.gz`

## Comparing `darwinio-0.5.1.tar` & `darwinio-0.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.5.1/CONTRIBUTING.md
--rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.5.1/keke
--rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.5.1/keke2
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.5.1/requirements.txt
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.5.1/todo.org
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/characteristics.ods
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/doc.md
--rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/doc.pdf
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.5.1/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     4018 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    15229 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    21588 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1787 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/stats.py
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/test.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.5.1/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.5.1/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.5.1/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.5.1/README.md
--rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 darwinio-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 darwinio-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.5.2/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.5.2/keke
+-rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.5.2/keke2
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.5.2/requirements.txt
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.5.2/todo.org
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.5.2/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     4023 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    15229 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    21606 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     3645 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1787 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/stats.py
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/test.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.5.2/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.5.2/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.5.2/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.5.2/README.md
+-rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 darwinio-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 darwinio-0.5.2/PKG-INFO
```

### Comparing `darwinio-0.5.1/CONTRIBUTING.md` & `darwinio-0.5.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/keke` & `darwinio-0.5.2/keke`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/keke2` & `darwinio-0.5.2/keke2`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/todo.org` & `darwinio-0.5.2/todo.org`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/characteristics.ods` & `darwinio-0.5.2/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/doc.md` & `darwinio-0.5.2/documentation/doc.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/doc.pdf` & `darwinio-0.5.2/documentation/doc.pdf`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/earlystages.md` & `darwinio-0.5.2/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/implementation.md` & `darwinio-0.5.2/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/graphical_interface/empty_window.png` & `darwinio-0.5.2/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/graphical_interface/main_game.png` & `darwinio-0.5.2/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/graphical_interface/starting_window.png` & `darwinio-0.5.2/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/screenshot/main_game_play.png` & `darwinio-0.5.2/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/documentation/screenshot/titlescreen.png` & `darwinio-0.5.2/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/__main__.py` & `darwinio-0.5.2/src/darwinio/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         screen, "DISCLAIMER", constants.DISCLAIMER, 2
     )
     license_notice = gsim.TextScreen(screen, constants.LICENSE_NOTICE, 3)
     world_build = gsim.Organism_selection(screen, world, 5)
     init_help_screen = gsim.TextScreen(screen, constants.HELP, 4)
     help_screen = gsim.TextScreen(screen, constants.HELP, 6)
     with gsim.get_asset_path("art", "archaebacteria_halophile.png") as path:
-        main_game = gsim.Simulation(screen, world, stats, path)
+        main_game = gsim.Simulation(screen, world, stats, str(path))
 
     # Create the state machine
     statemachine = gsim.StateMachine(
         [
             title,
             disclaimer,
             license_notice,
```

### Comparing `darwinio-0.5.1/src/darwinio/brain.py` & `darwinio-0.5.2/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/constants.py` & `darwinio-0.5.2/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/distribution.py` & `darwinio-0.5.2/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/genome.py` & `darwinio-0.5.2/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/graphical_sim.py` & `darwinio-0.5.2/src/darwinio/graphical_sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from __future__ import annotations
 from typing import Union
 import pygame as pg
 import pygame_gui as pgui
 import darwinio.distribution as dist
 import darwinio.genome as gn
-from importlib.resources import files
+from importlib.resources import files, as_file
 import threading
 import copy
 import darwinio.stats as statistics
 
 
 class World(dist.World):
     def render(self, surface: pg.Surface, image: pg.Surface):
@@ -677,8 +677,8 @@
 
 def get_asset_path(*paths: str):
     """Gets the path for an asset"""
     file_path = files("darwinio")
     file_path = file_path.joinpath("assets")
     for path in paths:
         file_path = file_path.joinpath(path)
-    return file_path
+    return as_file(file_path)
```

### Comparing `darwinio-0.5.1/src/darwinio/organism.py` & `darwinio-0.5.2/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/stats.py` & `darwinio-0.5.2/src/darwinio/stats.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/text_sim.py` & `darwinio-0.5.2/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.5.2/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.5.2/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.5.2/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.5.2/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.5.2/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.5.2/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.5.2/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.5.2/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.5.2/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.5.2/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.5.2/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.5.2/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.5.2/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.5.2/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.5.2/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.5.2/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.5.2/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/art/theme.json` & `darwinio-0.5.2/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.5.2/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/LICENSE.md` & `darwinio-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/README.md` & `darwinio-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.1/pyproject.toml` & `darwinio-0.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.5.1"
+version = "0.5.2"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.5.1/PKG-INFO` & `darwinio-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.5.1
+Version: 0.5.2
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

