# Comparing `tmp/darwinio-0.5.3.tar.gz` & `tmp/darwinio-0.6.0.tar.gz`

## Comparing `darwinio-0.5.3.tar` & `darwinio-0.6.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.5.3/CONTRIBUTING.md
--rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.5.3/keke
--rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.5.3/keke2
--rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.5.3/requirements.txt
--rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.5.3/todo.org
--rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/characteristics.ods
--rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/doc.md
--rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/doc.pdf
--rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/earlystages.md
--rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/implementation.md
--rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/graphical_interface/empty_window.png
--rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/graphical_interface/main_game.png
--rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/graphical_interface/starting_window.png
--rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/screenshot/main_game_play.png
--rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.5.3/documentation/screenshot/titlescreen.png
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/__init__.py
--rwxr-xr-x   0        0        0     4023 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/__main__.py
--rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/brain.py
--rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/constants.py
--rwxr-xr-x   0        0        0    15225 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/distribution.py
--rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/genome.py
--rwxr-xr-x   0        0        0    21606 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/graphical_sim.py
--rwxr-xr-x   0        0        0     3667 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/organism.py
--rwxr-xr-x   0        0        0     1787 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/stats.py
--rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/test.py
--rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/text_sim.py
--rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_halophile.png
--rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_methanogen.png
--rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
--rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/eubacteria_BGA.png
--rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/eubacteria_mycoplasma.png
--rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
--rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/fungi-ascomycetes.png
--rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/fungi-basidiomycetes.png
--rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/fungi-deuteromycetes.png
--rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/fungi-phycomycetes.png
--rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/metaphyta-algae.png
--rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/metaphyta-angiospermae.png
--rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/metaphyta-bryophyta.png
--rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/metaphyta-gymnospermae.png
--rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/metaphyta-pterdiophyta.png
--rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/protista_dinoflagellate.png
--rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/protista_euglena.png
--rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/protista_protozoan.png
--rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/protista_slimemould.png
--rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/art/theme.json
--rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.5.3/src/darwinio/assets/audio/Darwinio.mp3
--rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.5.3/.gitignore
--rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.5.3/LICENSE.md
--rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.5.3/README.md
--rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 darwinio-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 darwinio-0.5.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1873 2020-02-02 00:00:00.000000 darwinio-0.6.0/CONTRIBUTING.md
+-rwxr-xr-x   0        0        0   441990 2020-02-02 00:00:00.000000 darwinio-0.6.0/keke
+-rwxr-xr-x   0        0        0   439135 2020-02-02 00:00:00.000000 darwinio-0.6.0/keke2
+-rwxr-xr-x   0        0        0       65 2020-02-02 00:00:00.000000 darwinio-0.6.0/requirements.txt
+-rwxr-xr-x   0        0        0      562 2020-02-02 00:00:00.000000 darwinio-0.6.0/todo.org
+-rwxr-xr-x   0        0        0     5915 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/characteristics.ods
+-rwxr-xr-x   0        0        0     3002 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/doc.md
+-rwxr-xr-x   0        0        0    86371 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/doc.pdf
+-rwxr-xr-x   0        0        0      814 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/earlystages.md
+-rwxr-xr-x   0        0        0     2057 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/implementation.md
+-rwxr-xr-x   0        0        0     3062 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/graphical_interface/empty_window.png
+-rwxr-xr-x   0        0        0    11317 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/graphical_interface/main_game.png
+-rwxr-xr-x   0        0        0     7816 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/graphical_interface/starting_window.png
+-rwxr-xr-x   0        0        0    71751 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/screenshot/main_game_play.png
+-rwxr-xr-x   0        0        0    23470 2020-02-02 00:00:00.000000 darwinio-0.6.0/documentation/screenshot/titlescreen.png
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/__init__.py
+-rwxr-xr-x   0        0        0     4023 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/__main__.py
+-rwxr-xr-x   0        0        0     5460 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/brain.py
+-rwxr-xr-x   0        0        0     2438 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/constants.py
+-rwxr-xr-x   0        0        0    15225 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/distribution.py
+-rwxr-xr-x   0        0        0     2728 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/genome.py
+-rwxr-xr-x   0        0        0    21684 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/graphical_sim.py
+-rwxr-xr-x   0        0        0     3667 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/organism.py
+-rwxr-xr-x   0        0        0     1800 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/stats.py
+-rwxr-xr-x   0        0        0      252 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/test.py
+-rwxr-xr-x   0        0        0     1483 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/text_sim.py
+-rwxr-xr-x   0        0        0     3767 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_halophile.png
+-rwxr-xr-x   0        0        0     3805 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_methanogen.png
+-rwxr-xr-x   0        0        0     3712 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png
+-rwxr-xr-x   0        0        0     5075 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/eubacteria_BGA.png
+-rwxr-xr-x   0        0        0     4533 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/eubacteria_mycoplasma.png
+-rwxr-xr-x   0        0        0     5241 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png
+-rwxr-xr-x   0        0        0     4269 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/fungi-ascomycetes.png
+-rwxr-xr-x   0        0        0     4427 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/fungi-basidiomycetes.png
+-rwxr-xr-x   0        0        0     3117 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/fungi-deuteromycetes.png
+-rwxr-xr-x   0        0        0    11139 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/fungi-phycomycetes.png
+-rwxr-xr-x   0        0        0     4609 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/metaphyta-algae.png
+-rwxr-xr-x   0        0        0     6760 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/metaphyta-angiospermae.png
+-rwxr-xr-x   0        0        0     4285 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/metaphyta-bryophyta.png
+-rwxr-xr-x   0        0        0     6598 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/metaphyta-gymnospermae.png
+-rwxr-xr-x   0        0        0     3474 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png
+-rwxr-xr-x   0        0        0     4270 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/protista_dinoflagellate.png
+-rwxr-xr-x   0        0        0     2858 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/protista_euglena.png
+-rwxr-xr-x   0        0        0     3734 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/protista_protozoan.png
+-rwxr-xr-x   0        0        0     6104 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/protista_slimemould.png
+-rwxr-xr-x   0        0        0      859 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/art/theme.json
+-rwxr-xr-x   0        0        0  4128852 2020-02-02 00:00:00.000000 darwinio-0.6.0/src/darwinio/assets/audio/Darwinio.mp3
+-rwxr-xr-x   0        0        0       26 2020-02-02 00:00:00.000000 darwinio-0.6.0/.gitignore
+-rwxr-xr-x   0        0        0    34915 2020-02-02 00:00:00.000000 darwinio-0.6.0/LICENSE.md
+-rwxr-xr-x   0        0        0     2497 2020-02-02 00:00:00.000000 darwinio-0.6.0/README.md
+-rwxr-xr-x   0        0        0      877 2020-02-02 00:00:00.000000 darwinio-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3257 2020-02-02 00:00:00.000000 darwinio-0.6.0/PKG-INFO
```

### Comparing `darwinio-0.5.3/CONTRIBUTING.md` & `darwinio-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/keke` & `darwinio-0.6.0/keke`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/keke2` & `darwinio-0.6.0/keke2`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/todo.org` & `darwinio-0.6.0/todo.org`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/characteristics.ods` & `darwinio-0.6.0/documentation/characteristics.ods`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/doc.md` & `darwinio-0.6.0/documentation/doc.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/doc.pdf` & `darwinio-0.6.0/documentation/doc.pdf`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/earlystages.md` & `darwinio-0.6.0/documentation/earlystages.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/implementation.md` & `darwinio-0.6.0/documentation/implementation.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/graphical_interface/empty_window.png` & `darwinio-0.6.0/documentation/graphical_interface/empty_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/graphical_interface/main_game.png` & `darwinio-0.6.0/documentation/graphical_interface/main_game.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/graphical_interface/starting_window.png` & `darwinio-0.6.0/documentation/graphical_interface/starting_window.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/screenshot/main_game_play.png` & `darwinio-0.6.0/documentation/screenshot/main_game_play.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/documentation/screenshot/titlescreen.png` & `darwinio-0.6.0/documentation/screenshot/titlescreen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/__main__.py` & `darwinio-0.6.0/src/darwinio/__main__.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/brain.py` & `darwinio-0.6.0/src/darwinio/brain.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/constants.py` & `darwinio-0.6.0/src/darwinio/constants.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/distribution.py` & `darwinio-0.6.0/src/darwinio/distribution.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/genome.py` & `darwinio-0.6.0/src/darwinio/genome.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/graphical_sim.py` & `darwinio-0.6.0/src/darwinio/graphical_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -398,15 +398,18 @@
                     )
                     self.world.food_distribution = (
                         self.world.generate_distribution(
                             int(new_avg_food_content), 100
                         )
                     )
                     self.food_slider.update()
-            if event.type == pgui.UI_BUTTON_PRESSED:
+            if (
+                event.type == pgui.UI_BUTTON_PRESSED
+                and not self.stats.data.empty
+            ):
                 if event.ui_element == self.graph_viz_button:
                     self.stats.plot(["Population", "Food", "Temperature"])
             self.manager.process_events(event)
 
         keys_pressed = pg.key.get_pressed()
         # moving
         step_size: int = 500
```

### Comparing `darwinio-0.5.3/src/darwinio/organism.py` & `darwinio-0.6.0/src/darwinio/organism.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/stats.py` & `darwinio-0.6.0/src/darwinio/stats.py`

 * *Files 11% similar despite different names*

```diff
@@ -56,9 +56,9 @@
         """
         Plot the specified columns of the data.
 
         Args:
         -----
         columns: A list of column names to be plotted.
         """
-        self.data[columns].plot()
+        self.data[columns].plot(subplots=True)
         plt.show()
```

### Comparing `darwinio-0.5.3/src/darwinio/text_sim.py` & `darwinio-0.6.0/src/darwinio/text_sim.py`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_halophile.png` & `darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_halophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_methanogen.png` & `darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_methanogen.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/archaebacteria_thermoacidophile.png` & `darwinio-0.6.0/src/darwinio/assets/art/archaebacteria_thermoacidophile.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/eubacteria_BGA.png` & `darwinio-0.6.0/src/darwinio/assets/art/eubacteria_BGA.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/eubacteria_mycoplasma.png` & `darwinio-0.6.0/src/darwinio/assets/art/eubacteria_mycoplasma.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/eubacteroa_chemosynthetic.png` & `darwinio-0.6.0/src/darwinio/assets/art/eubacteroa_chemosynthetic.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/fungi-ascomycetes.png` & `darwinio-0.6.0/src/darwinio/assets/art/fungi-ascomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/fungi-basidiomycetes.png` & `darwinio-0.6.0/src/darwinio/assets/art/fungi-basidiomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/fungi-deuteromycetes.png` & `darwinio-0.6.0/src/darwinio/assets/art/fungi-deuteromycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/fungi-phycomycetes.png` & `darwinio-0.6.0/src/darwinio/assets/art/fungi-phycomycetes.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/metaphyta-algae.png` & `darwinio-0.6.0/src/darwinio/assets/art/metaphyta-algae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/metaphyta-angiospermae.png` & `darwinio-0.6.0/src/darwinio/assets/art/metaphyta-angiospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/metaphyta-bryophyta.png` & `darwinio-0.6.0/src/darwinio/assets/art/metaphyta-bryophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/metaphyta-gymnospermae.png` & `darwinio-0.6.0/src/darwinio/assets/art/metaphyta-gymnospermae.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/metaphyta-pterdiophyta.png` & `darwinio-0.6.0/src/darwinio/assets/art/metaphyta-pterdiophyta.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/protista_dinoflagellate.png` & `darwinio-0.6.0/src/darwinio/assets/art/protista_dinoflagellate.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/protista_euglena.png` & `darwinio-0.6.0/src/darwinio/assets/art/protista_euglena.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/protista_protozoan.png` & `darwinio-0.6.0/src/darwinio/assets/art/protista_protozoan.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/protista_slimemould.png` & `darwinio-0.6.0/src/darwinio/assets/art/protista_slimemould.png`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/art/theme.json` & `darwinio-0.6.0/src/darwinio/assets/art/theme.json`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/src/darwinio/assets/audio/Darwinio.mp3` & `darwinio-0.6.0/src/darwinio/assets/audio/Darwinio.mp3`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/LICENSE.md` & `darwinio-0.6.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/README.md` & `darwinio-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `darwinio-0.5.3/pyproject.toml` & `darwinio-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [tool.hatch.build]
 exclude = [
   "*.wav",
 ]
 
 [project]
 name = "darwinio"
-version = "0.5.3"
+version = "0.6.0"
 authors = [
   { name="Tushar Maharana", email="tusharhero@sdf.org" },
   { name="Mihir Nallagonda", email="adhikshithamihir@gmail.com" },
 ]
 description = "An evolution simulator"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `darwinio-0.5.3/PKG-INFO` & `darwinio-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: darwinio
-Version: 0.5.3
+Version: 0.6.0
 Summary: An evolution simulator
 Project-URL: Homepage, https://github.com/tusharhero/darwinio
 Project-URL: Bug Tracker, https://github.com/tusharhero/darwinio/issues
 Author-email: Tushar Maharana <tusharhero@sdf.org>, Mihir Nallagonda <adhikshithamihir@gmail.com>
 License-File: LICENSE.md
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

