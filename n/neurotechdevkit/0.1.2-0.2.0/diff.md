# Comparing `tmp/neurotechdevkit-0.1.2.tar.gz` & `tmp/neurotechdevkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurotechdevkit-0.1.2.tar", max compression
+gzip compressed data, was "neurotechdevkit-0.2.0.tar", max compression
```

## Comparing `neurotechdevkit-0.1.2.tar` & `neurotechdevkit-0.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0    11339 2023-07-07 14:59:39.884003 neurotechdevkit-0.1.2/LICENSE
--rw-r--r--   0        0        0     4034 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/docs/index.md
--rw-r--r--   0        0        0     2217 2023-07-07 14:59:56.776350 neurotechdevkit-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2404 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/__init__.py
--rw-r--r--   0        0        0     4747 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_animations.py
--rw-r--r--   0        0        0     2304 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_formatting.py
--rw-r--r--   0        0        0     8996 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_source.py
--rw-r--r--   0        0        0     3485 2023-07-07 14:59:40.016007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_target.py
--rw-r--r--   0        0        0    49858 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/colormaps.py
--rw-r--r--   0        0        0     2307 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=10°.png
--rw-r--r--   0        0        0    30101 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=120°.png
--rw-r--r--   0        0        0    50607 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=150°.png
--rw-r--r--   0        0        0    61496 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=180°.png
--rw-r--r--   0        0        0     4467 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=20°.png
--rw-r--r--   0        0        0      715 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=2°.png
--rw-r--r--   0        0        0     8691 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=40°.png
--rw-r--r--   0        0        0     1147 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=5°.png
--rw-r--r--   0        0        0    12673 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=60°.png
--rw-r--r--   0        0        0    20015 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=90°.png
--rw-r--r--   0        0        0     2753 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=Flat.png
--rw-r--r--   0        0        0     3377 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-dark.png
--rw-r--r--   0        0        0     3598 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-light.png
--rw-r--r--   0        0        0      722 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/font.py
--rw-r--r--   0        0        0    96364 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
--rw-r--r--   0        0        0    97116 2023-07-07 14:59:40.020007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
--rw-r--r--   0        0        0    96304 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
--rw-r--r--   0        0        0    96312 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
--rw-r--r--   0        0        0    96492 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
--rw-r--r--   0        0        0    96412 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
--rw-r--r--   0        0        0    96528 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
--rw-r--r--   0        0        0     4314 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layers.py
--rw-r--r--   0        0        0     5561 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layout.py
--rw-r--r--   0        0        0     6290 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/legends.py
--rw-r--r--   0        0        0     7499 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/napari.py
--rw-r--r--   0        0        0     8880 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/simulations.py
--rw-r--r--   0        0        0      593 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/__init__.py
--rw-r--r--   0        0        0    13016 2023-07-07 14:59:40.024007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/_metrics.py
--rw-r--r--   0        0        0    53384 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/results/_results.py
--rw-r--r--   0        0        0      619 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/__init__.py
--rw-r--r--   0        0        0    44605 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_base.py
--rw-r--r--   0        0        0     6053 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_resources.py
--rw-r--r--   0        0        0     4549 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_0.py
--rw-r--r--   0        0        0     8500 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_1.py
--rw-r--r--   0        0        0    11457 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_2.py
--rw-r--r--   0        0        0     7378 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_shots.py
--rw-r--r--   0        0        0     4559 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_time.py
--rw-r--r--   0        0        0    11913 2023-07-07 14:59:40.028007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_utils.py
--rw-r--r--   0        0        0  2195183 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
--rw-r--r--   0        0        0      936 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/materials.py
--rw-r--r--   0        0        0    55819 2023-07-07 14:59:40.040007 neurotechdevkit-0.1.2/src/neurotechdevkit/sources.py
--rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 neurotechdevkit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2023-07-17 05:54:50.547055 neurotechdevkit-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4034 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/docs/index.md
+-rw-r--r--   0        0        0     2217 2023-07-17 05:55:06.671558 neurotechdevkit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2432 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/__init__.py
+-rw-r--r--   0        0        0     4777 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/materials.py
+-rw-r--r--   0        0        0     1162 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/__init__.py
+-rw-r--r--   0        0        0     4747 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_animations.py
+-rw-r--r--   0        0        0     2304 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_formatting.py
+-rw-r--r--   0        0        0     8996 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_source.py
+-rw-r--r--   0        0        0     3485 2023-07-17 05:54:50.667059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_target.py
+-rw-r--r--   0        0        0    49858 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/colormaps.py
+-rw-r--r--   0        0        0     2307 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=10°.png
+-rw-r--r--   0        0        0    30101 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=120°.png
+-rw-r--r--   0        0        0    50607 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=150°.png
+-rw-r--r--   0        0        0    61496 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=180°.png
+-rw-r--r--   0        0        0     4467 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=20°.png
+-rw-r--r--   0        0        0      715 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=2°.png
+-rw-r--r--   0        0        0     8691 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=40°.png
+-rw-r--r--   0        0        0     1147 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=5°.png
+-rw-r--r--   0        0        0    12673 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=60°.png
+-rw-r--r--   0        0        0    20015 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=90°.png
+-rw-r--r--   0        0        0     2753 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=Flat.png
+-rw-r--r--   0        0        0     3377 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/target-dark.png
+-rw-r--r--   0        0        0     3598 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/target-light.png
+-rw-r--r--   0        0        0      722 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/font.py
+-rw-r--r--   0        0        0    96364 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf
+-rw-r--r--   0        0        0    97116 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf
+-rw-r--r--   0        0        0    96304 2023-07-17 05:54:50.671059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf
+-rw-r--r--   0        0        0    96312 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf
+-rw-r--r--   0        0        0    96492 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf
+-rw-r--r--   0        0        0    96412 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf
+-rw-r--r--   0        0        0    96528 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf
+-rw-r--r--   0        0        0     4314 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/layers.py
+-rw-r--r--   0        0        0     5561 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/layout.py
+-rw-r--r--   0        0        0     6290 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/legends.py
+-rw-r--r--   0        0        0     7490 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/napari.py
+-rw-r--r--   0        0        0     8880 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/simulations.py
+-rw-r--r--   0        0        0      593 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/results/__init__.py
+-rw-r--r--   0        0        0    13017 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/results/_metrics.py
+-rw-r--r--   0        0        0    53469 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/results/_results.py
+-rw-r--r--   0        0        0      620 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/__init__.py
+-rw-r--r--   0        0        0    43498 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_base.py
+-rw-r--r--   0        0        0     6053 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_resources.py
+-rw-r--r--   0        0        0     4800 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_0.py
+-rw-r--r--   0        0        0     8297 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_1.py
+-rw-r--r--   0        0        0    11365 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_2.py
+-rw-r--r--   0        0        0     7378 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_shots.py
+-rw-r--r--   0        0        0     4559 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_time.py
+-rw-r--r--   0        0        0    11913 2023-07-17 05:54:50.675059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_utils.py
+-rw-r--r--   0        0        0  2195183 2023-07-17 05:54:50.687059 neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat
+-rw-r--r--   0        0        0    55819 2023-07-17 05:54:50.691059 neurotechdevkit-0.2.0/src/neurotechdevkit/sources.py
+-rw-r--r--   0        0        0     5507 1970-01-01 00:00:00.000000 neurotechdevkit-0.2.0/PKG-INFO
```

### Comparing `neurotechdevkit-0.1.2/LICENSE` & `neurotechdevkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/docs/index.md` & `neurotechdevkit-0.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/pyproject.toml` & `neurotechdevkit-0.2.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neurotechdevkit"
-version = "v0.1.2"
+version = "v0.2.0"
 description = "Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology"
 authors = ["AE Studio <bci@ae.studio>"]
 maintainers = ["AE Studio <bci@ae.studio>"]
 packages = [{include = "neurotechdevkit", from = "src" }]
 
 readme = "README.md"
 license = "Apache-2.0"
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/__init__.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Main package for the neurotechdevkit."""
 from __future__ import annotations
 
 import os
 
-from . import scenarios, sources
+from . import materials, scenarios, sources
 from .results import load_result_from_disk
 
 __all__ = [
     "results",
     "scenarios",
+    "materials",
     "sources",
     "make",
     "ScenarioNotFoundError",
     "load_result_from_disk",
 ]
 
 if "DEVITO_ARCH" not in os.environ:
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/__init__.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_animations.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_animations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_formatting.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_formatting.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_source.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_source.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/_target.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/_target.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/colormaps.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/colormaps.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=10°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=10°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=120°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=120°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=150°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=150°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=180°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=180°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=20°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=20°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=2°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=2°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=40°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=40°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=5°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=5°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=60°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=60°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=90°.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=90°.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/Angle=Flat.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/Angle=Flat.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-dark.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/target-dark.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/components/target-light.png` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/components/target-light.png`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/font.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/font.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Bold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Light.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Medium.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-Regular.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/fonts/Manrope-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layers.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/layers.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/layout.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/layout.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/legends.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/legends.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/napari.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/napari.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,14 @@
 
     Args:
         scenario: the 3D scenario to be rendered.
 
     Raises:
         ImportError: If napari is not found.
     """
-    pass
     _create_napari_3d(scenario=result.scenario, amplitudes=result.get_steady_state())
 
 
 def _create_napari_3d(
     scenario: "scenarios.Scenario3D", amplitudes: npt.NDArray[np.float_] | None
 ) -> None:
     try:
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/rendering/simulations.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/rendering/simulations.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/results/__init__.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/results/__init__.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/results/_metrics.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/results/_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
                     f"The mechanical index (MI) within the {layer} layer. The MI is"
                     " defined as peak negative pressure divided by the square root of"
                     " the frequency of the ultrasound wave. An example FDA recommended"
                     " limit for MI is 1.9 (the exact value can vary depending on the"
                     " intended use)."
                 ),
             }
-            for layer in result.scenario.ordered_layers
+            for layer in result.scenario.material_layers
         },
     }
 
 
 def calculate_mechanical_index(
     result: results.SteadyStateResult, layer: str | None = None
 ) -> float:
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/results/_results.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/results/_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1293,14 +1293,15 @@
             center_frequency=save_data["center_frequency"],
             effective_dt=save_data["effective_dt"],
             pde=None,
             shot=None,
             wavefield=save_data.get("wavefield"),
             traces=None,
         )
+        scenario._problem = scenario._compile_problem(save_data["center_frequency"])
 
         if save_data.get("steady_state") is not None:
             fields_kwargs.update(steady_state=save_data["steady_state"])
 
         return result_type(**fields_kwargs)
     except FileNotFoundError:
         raise
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/__init__.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Scenarios module."""
-from . import materials
+from .. import materials
 from ._base import Scenario, Scenario2D, Scenario3D, Target
 from ._scenario_0 import Scenario0
 from ._scenario_1 import Scenario1_2D, Scenario1_3D
 from ._scenario_2 import Scenario2_2D, Scenario2_3D
 from ._utils import add_material_fields_to_problem, create_grid_circular_mask, make_grid
 
 __all__ = [
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_base.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 import numpy.typing as npt
 import stride
 from frozenlist import FrozenList
 from mosaic.types import Struct
 from stride.problem import StructuredData
 
 from .. import rendering, results
+from ..materials import Material, get_material, get_render_color
 from ..sources import Source
 from ._resources import budget_time_and_memory_resources
 from ._shots import create_shot
 from ._time import (
     create_time_grid,
     find_largest_delay_in_sources,
     select_simulation_time_for_pulsed,
@@ -56,26 +57,31 @@
 
 class Scenario(abc.ABC):
     """The base scenario."""
 
     _SCENARIO_ID: str
     _TARGET_OPTIONS: dict[str, Target]
 
+    # The list of material layers in the scenario.
+    material_layers: list[str]
+
+    # The customization to the material layers.
+    material_properties: dict[str, Material] = {}
+
     def __init__(
         self,
         origin: npt.NDArray[np.float_],
         complexity: str = "fast",
     ):
         """Initialize the scenario."""
         self._complexity = complexity
         if self._complexity != "fast":
             raise ValueError("the only complexity currently supported is 'fast'")
 
         self._origin = origin
-        self._problem = self._compile_problem()
         self._sources: FrozenList[Source] = FrozenList()
         self._target_id: str
 
     @property
     def scenario_id(self) -> str:
         """The ID for this scenario."""
         return self._SCENARIO_ID
@@ -210,40 +216,53 @@
         return self.target.center
 
     @property
     def target_radius(self) -> float:
         """The radius of the target region (in meters)."""
         return self.target.radius
 
-    @property
-    def materials(self) -> Mapping[str, Struct]:
-        """A map between material name and material properties.
+    def get_materials(self, center_frequency=float) -> Mapping[str, Struct]:
+        """Return a map between material name and material properties.
 
         - vp: the speed of sound (in m/s).
         - rho: the mass density (in kg/m³).
         - alpha: the absorption (in dB/cm).
         - render_color: the color used when rendering this material in the
         scenario layout plot.
         """
-        return {name: material for name, material in self._material_layers}
+        materials = {}
+        for layer in self.material_layers:
+            if layer not in self.material_properties:
+                material_properties = get_material(layer, center_frequency)
+            else:
+                material_properties = self.material_properties[layer]
+            materials[layer] = material_properties.to_struct()
+        return materials
 
     @property
-    def layer_ids(self) -> Mapping[str, int]:
-        """A map between material names and their layer id."""
-        return {name: n for n, (name, _) in enumerate(self._material_layers)}
+    def material_colors(self) -> dict[str, str]:
+        """
+        A map between material name and material render color.
 
-    @property
-    def ordered_layers(self) -> list[str]:
-        """A list of material names in order of their layer id."""
-        return [name for name, _ in self._material_layers]
+        Returns:
+            dict[str, str]: keys are material names and values are the hex color
+        """
+        material_colors = {}
+        for material in self.material_layers:
+            if material in self.material_properties:
+                color = self.material_properties[material].render_color
+            else:
+                color = get_render_color(material_name=material)
+            material_colors[material] = color
+        return material_colors
 
     @property
-    @abc.abstractmethod
-    def _material_layers(self) -> list[tuple[str, Struct]]:
-        pass
+    def layer_ids(self) -> Mapping[str, int]:
+        """A map between material names and their layer id."""
+        return {name: n for n, name in enumerate(self.material_layers)}
 
     @property
     @abc.abstractmethod
     def _material_outline_upsample_factor(self) -> int:
         """Upsample_factor to use for this scenario when drawing material outlines.
 
         This parameter is internal to ndk, is not intended to be used directly.
@@ -316,15 +335,15 @@
 
         Returns:
             An array containing the field data.
         """
         return self.problem.medium.fields[field].data
 
     @abc.abstractmethod
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         pass
 
     def reset(self) -> None:
         """Reset the scenario to initial state."""
         raise NotImplementedError()
 
     def add_source(self, source: Source) -> None:
@@ -368,27 +387,22 @@
         """Execute a steady-state simulation.
 
         In this simulation, the sources will emit pressure waves with a continuous
         waveform until steady-state has been reached. The steady-state wave amplitude is
         found by taking the Fourier transform of the last `n_cycles_steady_state` cycles
         of data and taking the amplitude of the component at the `center_frequency`.
 
-        !!! note
-            The only supported frequency currently supported is 500kHz. Any other
-            value will raise a NotImplementedError.
-
         !!! warning
             A poor choice of arguments to this function can lead to a failed
             simulation. Make sure you understand the impact of supplying parameter
             values other than the default if you chose to do so.
 
         Args:
             center_frequency: the center frequency (in hertz) to use for the
-                continuous-wave source output. No other value besides 500kHz (the
-                default) is currently supported.
+                continuous-wave source output.
             points_per_period: the number of points in time to simulate for each cycle
                 of the wave.
             n_cycles_steady_state: the number of complete cycles to use when calculating
                 the steady-state wave amplitudes.
             time_to_steady_state: the amount of time (in seconds) the simulation should
                 run before measuring the steady-state amplitude. If the value is None,
                 this time will automatically be set to the amount of time it would take
@@ -396,31 +410,22 @@
                 the slowest speed of sound in the scenario.
             recording_time_undersampling: the undersampling factor to apply to the time
                 axis when recording simulation results. One out of every this many
                 consecutive time points will be recorded and all others will be dropped.
             n_jobs: the number of threads to be used for the computation. Use None to
                 leverage Devito automatic tuning.
 
-        Raises:
-            NotImplementedError: if a `center_frequency` other than 500kHz is provided.
-
         Returns:
             An object containing the result of the steady-state simulation.
         """
-        if center_frequency != 5.0e5:
-            raise NotImplementedError(
-                "500kHz is the only currently supported center frequency. Support for"
-                " other frequencies will be implemented once material properties as a"
-                " function of frequency has been implemented."
-            )
-
+        self._problem = self._compile_problem(center_frequency)
         problem = self.problem
         sim_time = select_simulation_time_for_steady_state(
             grid=problem.grid,
-            materials=self.materials,
+            materials=self.get_materials(center_frequency),
             freq_hz=center_frequency,
             time_to_steady_state=time_to_steady_state,
             n_cycles_steady_state=n_cycles_steady_state,
             delay=find_largest_delay_in_sources(self.sources),
         )
         problem.grid.time = create_time_grid(
             freq_hz=center_frequency, ppp=points_per_period, sim_time=sim_time
@@ -470,42 +475,34 @@
         n_jobs: int | None = None,
     ) -> results.PulsedResult:
         """Execute a pulsed simulation in 2D.
 
         In this simulation, the sources will emit a pulse containing a few cycles of
         oscillation and then let the pulse propagate out to all edges of the scenario.
 
-        !!! note
-            The only supported frequency currently supported is 500kHz. Any other
-            value will raise a NotImplementedError.
-
         !!! warning
             A poor choice of arguments to this function can lead to a failed
             simulation. Make sure you understand the impact of supplying parameter
             values other than the default if you chose to do so.
 
         Args:
             center_frequency: the center frequency (in hertz) to use for the
-                continuous-wave source output. No other value besides
-                500kHz (the default) is currently supported.
+                continuous-wave source output.
             points_per_period: the number of points in time to simulate for each cycle
                 of the wave.
             simulation_time: the amount of time (in seconds) the simulation should run.
                 If the value is None, this time will automatically be set to the amount
                 of time it would take to propagate from one corner to the opposite in
                 the medium with the slowest speed of sound in the scenario.
             recording_time_undersampling: the undersampling factor to apply to the time
                 axis when recording simulation results. One out of every this many
                 consecutive time points will be recorded and all others will be dropped.
             n_jobs: the number of threads to be used for the computation. Use None to
                 leverage Devito automatic tuning.
 
-        Raises:
-            NotImplementedError: if a `center_frequency` other than 500kHz is provided.
-
         Returns:
             An object containing the result of the 2D pulsed simulation.
         """
         return self._simulate_pulse(
             center_frequency=center_frequency,
             points_per_period=points_per_period,
             simulation_time=simulation_time,
@@ -526,26 +523,21 @@
         slice_position: float | None = None,
     ) -> results.PulsedResult:
         """Execute a pulsed simulation.
 
         In this simulation, the sources will emit a pulse containing a few cycles of
         oscillation and then let the pulse propagate out to all edges of the scenario.
 
-        !!! note
-            The only supported frequency currently supported is 500kHz. Any other
-            value will raise a NotImplementedError.
-
         Warning: A poor choice of arguments to this function can lead to a failed
         simulation. Make sure you understand the impact of supplying parameter values
         other than the default if you chose to do so.
 
         Args:
             center_frequency: the center frequency (in hertz) to use for the
-                continuous-wave source output. No other value besides
-                500kHz (the default) is currently supported.
+                continuous-wave source output.
             points_per_period: the number of points in time to simulate for each cycle
                 of the wave.
             simulation_time: the amount of time (in seconds) the simulation should run.
                 If the value is None, this time will automatically be set to the amount
                 of time it would take to propagate from one corner to the opposite in
                 the medium with the slowest speed of sound in the scenario.
             recording_time_undersampling: the undersampling factor to apply to the time
@@ -556,32 +548,23 @@
             slice_axis: the axis along which to slice the 3D field to be recorded. If
                 None, then the complete field will be recorded. Use 0 for X axis, 1 for
                 Y axis and 2 for Z axis. Only valid if `slice_position` is not None.
             slice_position: the position (in meters) along the slice axis at
                 which the slice of the 3D field should be made. Only valid if
                 `slice_axis` is not None.
 
-        Raises:
-            NotImplementedError: if a `center_frequency` other than 500kHz is provided.
-
         Returns:
             An object containing the result of the pulsed simulation.
         """
-        if center_frequency != 5.0e5:
-            raise NotImplementedError(
-                "500kHz is the only currently supported center frequency. Support for"
-                " other frequencies will be implemented once material properties as a"
-                " function of frequency has been implemented."
-            )
-
+        self._problem = self._compile_problem(center_frequency)
         problem = self.problem
         if simulation_time is None:
             simulation_time = select_simulation_time_for_pulsed(
                 grid=problem.grid,
-                materials=self.materials,
+                materials=self.get_materials(center_frequency),
                 delay=find_largest_delay_in_sources(self.sources),
             )
         problem.grid.time = create_time_grid(
             freq_hz=center_frequency, ppp=points_per_period, sim_time=simulation_time
         )
 
         if slice_axis is not None and slice_position is not None:
@@ -900,17 +883,15 @@
 
         Args:
             show_sources: whether or not to show the source transducer layer.
             show_target: whether or not to show the target layer.
             show_material_outlines: whether or not to display a thin white outline of
                 the transition between different materials.
         """
-        color_sequence = [
-            self.materials[name].render_color for name in self.ordered_layers
-        ]
+        color_sequence = list(self.material_colors.values())
         field = self.get_field_data("layer").astype(int)
         fig, ax = rendering.create_layout_fig(
             self.extent, self.origin, color_sequence, field
         )
 
         # add layers
         if show_material_outlines:
@@ -935,15 +916,15 @@
                 )
                 rendering.draw_source(ax, drawing_params)
 
         rendering.configure_layout_plot(
             fig=fig,
             ax=ax,
             color_sequence=color_sequence,
-            layer_labels=self.ordered_layers,
+            layer_labels=self.material_layers,
             show_sources=show_sources,
             show_target=show_target,
             extent=self.extent,
             origin=self.origin,
         )
 
 
@@ -1004,27 +985,22 @@
         slice_position: float | None = None,
     ) -> results.PulsedResult:
         """Execute a pulsed simulation in 3D.
 
         In this simulation, the sources will emit a pulse containing a few cycles of
         oscillation and then let the pulse propagate out to all edges of the scenario.
 
-        !!! note
-            The only supported frequency currently supported is 500kHz. Any
-            other value will raise a NotImplementedError.
-
         !!! warning
             A poor choice of arguments to this function can lead to a failed
             simulation. Make sure you understand the impact of supplying parameter
             values other than the default if you chose to do so.
 
         Args:
             center_frequency: the center frequency (in hertz) to use for the
-                continuous-wave source output. No other value besides
-                500kHz (the default) is currently supported.
+                continuous-wave source output.
             points_per_period: the number of points in time to simulate for each cycle
                 of the wave.
             simulation_time: the amount of time (in seconds) the simulation should run.
                 If the value is None, this time will automatically be set to the amount
                 of time it would take to propagate from one corner to the opposite in
                 the medium with the slowest speed of sound in the scenario.
             recording_time_undersampling: the undersampling factor to apply to the time
@@ -1035,17 +1011,14 @@
             slice_axis: the axis along which to slice the 3D field to be recorded. If
                 None, then the complete field will be recorded. Use 0 for X axis, 1 for
                 Y axis and 2 for Z axis. Only valid if `slice_position` is not None.
             slice_position: the position (in meters) along the slice axis at
                 which the slice of the 3D field should be made. Only valid if
                 `slice_axis` is not None.
 
-        Raises:
-            NotImplementedError: if a `center_frequency` other than 500kHz is provided.
-
         Returns:
             An object containing the result of the 3D pulsed simulation.
         """
         return self._simulate_pulse(
             center_frequency=center_frequency,
             points_per_period=points_per_period,
             simulation_time=simulation_time,
@@ -1083,17 +1056,15 @@
                 the transition between different materials.
         """
         if slice_axis is None:
             slice_axis = self.get_default_slice_axis()
         if slice_position is None:
             slice_position = self.get_default_slice_position(slice_axis)
 
-        color_sequence = [
-            self.materials[name].render_color for name in self.ordered_layers
-        ]
+        color_sequence = list(self.material_colors.values())
         field = self.get_field_data("layer").astype(int)
         field = slice_field(field, self, slice_axis, slice_position)
         extent = drop_element(self.extent, slice_axis)
         origin = drop_element(self.origin, slice_axis)
         fig, ax = rendering.create_layout_fig(extent, origin, color_sequence, field)
 
         # add layers
@@ -1123,15 +1094,15 @@
         axis_names = np.array(["X", "Y", "Z"])
         vert_name, horz_name = drop_element(axis_names, slice_axis)
         slice_name = axis_names[slice_axis]
         rendering.configure_layout_plot(
             fig=fig,
             ax=ax,
             color_sequence=color_sequence,
-            layer_labels=self.ordered_layers,
+            layer_labels=self.material_layers,
             show_sources=show_sources,
             show_target=show_target,
             extent=extent,
             origin=origin,
             vertical_label=vert_name,
             horizontal_label=horz_name,
             title=f"Scenario Layout\nSlice: {slice_name} = {slice_position} m",
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_resources.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_resources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_0.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_0.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import numpy as np
 import stride
-from mosaic.types import Struct
 
+from ..materials import Material
 from ..sources import FocusedSource2D
-from . import materials
 from ._base import Scenario2D, Target
 from ._utils import (
     add_material_fields_to_problem,
     create_grid_circular_mask,
     create_grid_elliptical_mask,
     make_grid,
 )
@@ -21,65 +20,69 @@
         "target_1": Target(
             target_id="target_1",
             center=np.array([0.0285, 0.0024]),
             radius=0.0017,
             description="Represents a simulated tumor.",
         ),
     }
+    material_layers = [
+        "water",
+        "cortical_bone",
+        "brain",
+        "tumor",
+    ]
+    material_properties = {
+        "water": Material(vp=1500.0, rho=1000.0, alpha=0.0, render_color="#2E86AB"),
+        "cortical_bone": Material(
+            vp=2800.0, rho=1850.0, alpha=4.0, render_color="#FAF0CA"
+        ),
+        "brain": Material(vp=1560.0, rho=1040.0, alpha=0.3, render_color="#DB504A"),
+        "tumor": Material(vp=1650.0, rho=1150.0, alpha=0.8, render_color="#94332F"),
+    }
 
     def __init__(self, complexity="fast"):
         """Create a new instance of scenario 0."""
         self._target_id = "target_1"
 
         super().__init__(
             origin=np.array([0.0, -0.02]),
             complexity=complexity,
         )
 
     @property
-    def _material_layers(self) -> list[tuple[str, Struct]]:
-        return [
-            ("water", materials.water),
-            ("skull", materials.cortical_bone),
-            ("brain", materials.brain),
-            ("tumor", materials.tumor),
-        ]
-
-    @property
     def _material_outline_upsample_factor(self) -> int:
         return 16
 
     def _get_material_masks(self, problem):
         return {
             name: _create_scenario_0_mask(name, problem.grid, self._origin)
-            for name in self.materials.keys()
+            for name in self.material_layers
         }
 
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency=float) -> stride.Problem:
         extent = np.array([0.05, 0.04])  # m
         origin = self.origin  # m
 
         # scenario constants
         speed_water = 1500  # m/s
-        c_freq = 500e3  # hz
 
         # desired resolution for complexity=fast
         ppw = 6
 
         # compute resolution
-        dx = speed_water / c_freq / ppw  # m
+        dx = speed_water / center_frequency / ppw  # m
 
         grid = make_grid(extent=extent, dx=dx)
         self._origin = origin
         problem = stride.Problem(
             name=f"{self.scenario_id}-{self.complexity}", grid=grid
         )
         problem = add_material_fields_to_problem(
             problem=problem,
-            materials=self.materials,
+            materials=self.get_materials(center_frequency),
             layer_ids=self.layer_ids,
             masks=self._get_material_masks(problem),
         )
         return problem
 
     def get_default_source(self):
         """Return the default source for the scenario."""
@@ -94,15 +97,15 @@
 
 def _create_scenario_0_mask(material, grid, origin):
     if material == "water":
         outer_skull_mask = _create_skull_interface_mask(grid, origin)
         water_mask = ~outer_skull_mask
         return water_mask
 
-    elif material == "skull":
+    elif material == "cortical_bone":
         outer_skull_mask = _create_skull_interface_mask(grid, origin)
         outer_brain_mask = _create_brain_interface_mask(grid, origin)
         skull_mask = outer_skull_mask & ~outer_brain_mask
         return skull_mask
 
     elif material == "brain":
         outer_brain_mask = _create_brain_interface_mask(grid, origin)
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_1.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_1.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,109 +1,91 @@
 from __future__ import annotations
 
-from typing import Mapping, Protocol
+from typing import Mapping
 
 import numpy as np
 import numpy.typing as npt
 import stride
-from mosaic.types import Struct
 
 from .. import rendering, sources
-from . import materials
-from ._base import Scenario2D, Scenario3D, Target
+from ..materials import Material
+from ._base import Scenario, Scenario2D, Scenario3D, Target
 from ._utils import add_material_fields_to_problem, make_grid
 
 
-class _Scenario1MixinProtocol(Protocol):
-    """Provide type-hinting for Scenario 1 members used by mixins."""
-
-    @property
-    def scenario_id(self) -> str:
-        ...
-
-    @property
-    def complexity(self) -> str:
-        ...
-
-    @property
-    def materials(self) -> Mapping[str, Struct]:
-        ...
-
-    @property
-    def layer_ids(self) -> Mapping[str, int]:
-        ...
-
-    def _get_material_masks(
-        self, problem: stride.Problem
-    ) -> Mapping[str, npt.NDArray[np.bool_]]:
-        ...
-
-
-class _Scenario1Mixin:
-    """A mixin providing specific implementation detail for scenario 1.
+class Scenario1(Scenario):
+    """Specific implementation detail for scenario 1.
 
     Scenario 1 is based on benchmark 4 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
         The Journal of the Acoustical Society of America 152, 1003 (2022);
         doi: 10.1121/10.0013426
         https://asa.scitation.org/doi/pdf/10.1121/10.0013426
     """
 
-    @property
-    def _material_layers(self: _Scenario1MixinProtocol) -> list[tuple[str, Struct]]:
-        return [
-            ("water", materials.water),
-            ("skin", materials.skin),
-            ("cortical bone", materials.cortical_bone),
-            ("trabecular bone", materials.trabecular_bone),
-            ("brain", materials.brain),
-        ]
+    material_layers = [
+        "water",
+        "skin",
+        "cortical_bone",
+        "trabecular_bone",
+        "brain",
+    ]
+    material_properties = {
+        "water": Material(vp=1500.0, rho=1000.0, alpha=0.0, render_color="#2E86AB"),
+        "skin": Material(vp=1610.0, rho=1090.0, alpha=0.2, render_color="#FA8B53"),
+        "cortical_bone": Material(
+            vp=2800.0, rho=1850.0, alpha=4.0, render_color="#FAF0CA"
+        ),
+        "trabecular_bone": Material(
+            vp=2300.0, rho=1700.0, alpha=8.0, render_color="#EBD378"
+        ),
+        "brain": Material(vp=1560.0, rho=1040.0, alpha=0.3, render_color="#DB504A"),
+    }
 
     @property
     def _material_outline_upsample_factor(self) -> int:
         return 8
 
     def _get_material_masks(
-        self: _Scenario1MixinProtocol, problem: stride.Problem
+        self, problem: stride.Problem
     ) -> Mapping[str, npt.NDArray[np.bool_]]:
         return {
             name: _create_scenario_1_mask(name, problem.grid)
-            for name in self.materials.keys()
+            for name in self.material_layers
         }
 
     def _compile_scenario_1_problem(
-        self: _Scenario1MixinProtocol, extent: npt.NDArray[np.float_]
+        self, extent: npt.NDArray[np.float_], center_frequency: float
     ) -> stride.Problem:
         # scenario constants
         speed_water = 1500  # m/s
-        c_freq = 500e3  # hz
 
         # desired resolution for complexity=fast
         ppw = 6
 
         # compute resolution
-        dx = speed_water / c_freq / ppw  # m
+        dx = speed_water / center_frequency / ppw  # m
 
         grid = make_grid(extent=extent, dx=dx)
         problem = stride.Problem(
             name=f"{self.scenario_id}-{self.complexity}", grid=grid
         )
         problem = add_material_fields_to_problem(
             problem=problem,
-            materials=self.materials,
+            materials=self.get_materials(center_frequency),
             layer_ids=self.layer_ids,
             masks=self._get_material_masks(problem),
         )
         return problem
 
 
-class Scenario1_2D(_Scenario1Mixin, Scenario2D):
+class Scenario1_2D(Scenario1, Scenario2D):
     """A 2D implementation of scenario 1.
 
     Scenario 1 is based on benchmark 4 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
@@ -122,30 +104,30 @@
         self._target_id = "target_1"
 
         super().__init__(
             origin=np.array([0.0, -0.035]),
             complexity=complexity,
         )
 
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         extent = np.array([0.12, 0.07])  # m
-        return self._compile_scenario_1_problem(extent)
+        return self._compile_scenario_1_problem(extent, center_frequency)
 
     def get_default_source(self) -> sources.Source:
         """Return the default source for the scenario."""
         return sources.FocusedSource2D(
             position=np.array([0.0, 0.0]),
             direction=np.array([1.0, 0.0]),
             aperture=0.064,
             focal_length=0.064,
             num_points=1000,
         )
 
 
-class Scenario1_3D(_Scenario1Mixin, Scenario3D):
+class Scenario1_3D(Scenario1, Scenario3D):
     """A 3D implementation of scenario 1.
 
     Scenario 1 is based on benchmark 4 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
@@ -186,39 +168,39 @@
         """Return the default viewer configuration for the scenario."""
         return rendering.ViewerConfig3D(
             init_angles=(-15, 45, 160),
             init_zoom=3.0,
             colormaps={
                 "water": "blue",
                 "skin": "viridis",
-                "cortical bone": "magma",
-                "trabecular bone": "inferno",
+                "cortical_bone": "magma",
+                "trabecular_bone": "inferno",
                 "brain": "bop orange",
             },
             opacities={
                 "water": 0.8,
                 "skin": 0.2,
-                "cortical bone": 0.2,
-                "trabecular bone": 0.2,
+                "cortical_bone": 0.2,
+                "trabecular_bone": 0.2,
                 "brain": 0.4,
             },
         )
 
     def get_default_slice_axis(self) -> int:
         """Return the default slice axis for the scenario."""
         return 1
 
     def get_default_slice_position(self, axis: int) -> float:
         """Return the default slice position for the scenario."""
         default_positions = np.array([0.064, 0.0, 0.0])
         return default_positions[axis]
 
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         extent = np.array([0.12, 0.07, 0.07])  # m
-        return self._compile_scenario_1_problem(extent)
+        return self._compile_scenario_1_problem(extent, center_frequency)
 
     def get_default_source(self) -> sources.Source:
         """Return the default source for the scenario."""
         return sources.FocusedSource3D(
             position=np.array([0.0, 0.0, 0.0]),
             direction=np.array([1.0, 0.0, 0.0]),
             aperture=0.064,
@@ -248,19 +230,19 @@
 
     if material == "water":
         _fill_mask(mask, start=0, end=interfaces[0], dx=dx)
 
     elif material == "skin":
         _fill_mask(mask, start=interfaces[0], end=interfaces[1], dx=dx)
 
-    elif material == "cortical bone":
+    elif material == "cortical_bone":
         _fill_mask(mask, start=interfaces[1], end=interfaces[2], dx=dx)
         _fill_mask(mask, start=interfaces[3], end=interfaces[4], dx=dx)
 
-    elif material == "trabecular bone":
+    elif material == "trabecular_bone":
         _fill_mask(mask, start=interfaces[2], end=interfaces[3], dx=dx)
 
     elif material == "brain":
         _fill_mask(mask, start=interfaces[4], end=None, dx=dx)
 
     else:
         raise ValueError(material)
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_scenario_2.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_scenario_2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,99 +1,83 @@
 from __future__ import annotations
 
 import pathlib
-from typing import Mapping, Protocol
+from typing import Mapping
 
 import hdf5storage
 import numpy as np
 import numpy.typing as npt
 import stride
-from mosaic.types import Struct
 
 from .. import rendering, sources
-from . import materials
-from ._base import Scenario2D, Scenario3D, Target
+from ..materials import Material
+from ._base import Scenario, Scenario2D, Scenario3D, Target
 from ._utils import add_material_fields_to_problem, make_grid
 
 
-class _Scenario2MixinProtocol(Protocol):
-    """Provide type-hinting for Scenario 2 members used by mixins."""
-
-    @property
-    def scenario_id(self) -> str:
-        ...
-
-    @property
-    def complexity(self) -> str:
-        ...
-
-    @property
-    def materials(self) -> Mapping[str, Struct]:
-        ...
-
-    @property
-    def layer_ids(self) -> Mapping[str, int]:
-        ...
-
-    def _get_material_masks(self) -> Mapping[str, npt.NDArray[np.bool_]]:
-        ...
-
-
-class _Scenario2Mixin:
-    """A mixin providing specific implementation detail for scenario 2.
+class Scenario2(Scenario):
+    """Specific implementation detail for scenario 2.
 
     Scenario 2 is based on benchmark 8 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
         The Journal of the Acoustical Society of America 152, 1003 (2022);
         doi: 10.1121/10.0013426
         https://asa.scitation.org/doi/pdf/10.1121/10.0013426
     """
 
-    @property
-    def _material_layers(self: _Scenario2MixinProtocol) -> list[tuple[str, Struct]]:
-        return [
-            ("water", materials.water),
-            ("skull", materials.cortical_bone),
-            ("brain", materials.brain),
-        ]
+    material_layers = [
+        "water",
+        "cortical_bone",
+        "brain",
+    ]
+    material_properties = {
+        "water": Material(vp=1500.0, rho=1000.0, alpha=0.0, render_color="#2E86AB"),
+        "cortical_bone": Material(
+            vp=2800.0, rho=1850.0, alpha=4.0, render_color="#FAF0CA"
+        ),
+        "brain": Material(vp=1560.0, rho=1040.0, alpha=0.3, render_color="#DB504A"),
+    }
 
     @property
     def _material_outline_upsample_factor(self) -> int:
         return 4
 
+    def _get_material_masks(self) -> Mapping[str, npt.NDArray[np.bool_]]:
+        """Will be implemented by the subclass."""
+        raise NotImplementedError()
+
     def _compile_scenario_2_problem(
-        self: _Scenario2MixinProtocol, extent: npt.NDArray[np.float_]
+        self, extent: npt.NDArray[np.float_], center_frequency: float
     ) -> stride.Problem:
         # scenario constants
         speed_water = 1500  # m/s
-        c_freq = 500e3  # hz
 
         # desired resolution for complexity=fast
         ppw = 6
 
         # compute resolution
-        dx = speed_water / c_freq / ppw  # m
+        dx = speed_water / center_frequency / ppw  # m
 
         grid = make_grid(extent=extent, dx=dx)
         problem = stride.Problem(
             name=f"{self.scenario_id}-{self.complexity}", grid=grid
         )
         problem = add_material_fields_to_problem(
             problem=problem,
-            materials=self.materials,
+            materials=self.get_materials(center_frequency),
             layer_ids=self.layer_ids,
             masks=self._get_material_masks(),
         )
         return problem
 
 
-class Scenario2_2D(_Scenario2Mixin, Scenario2D):
+class Scenario2_2D(Scenario2, Scenario2D):
     """A 2D implementation of scenario 2.
 
     Scenario 2 is based on benchmark 8 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
@@ -144,36 +128,36 @@
         self._target_id = "primary-visual-cortex"
 
         super().__init__(
             origin=np.array([0.0, -0.085]),
             complexity=complexity,
         )
 
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         extent = np.array([0.225, 0.170])  # m
-        return self._compile_scenario_2_problem(extent)
+        return self._compile_scenario_2_problem(extent, center_frequency)
 
     def _get_material_masks(self) -> Mapping[str, npt.NDArray[np.bool_]]:
         return {
             name: _create_scenario_2_mask(name, convert_2d=True)
-            for name in self.materials.keys()
+            for name in self.material_layers
         }
 
     def get_default_source(self) -> sources.Source:
         """Get the default source for the scenario."""
         return sources.FocusedSource2D(
             position=np.array([0.0, 0.0]),
             direction=np.array([1.0, 0.0]),
             aperture=0.064,
             focal_length=0.064,
             num_points=1000,
         )
 
 
-class Scenario2_3D(_Scenario2Mixin, Scenario3D):
+class Scenario2_3D(Scenario2, Scenario3D):
     """A 3D implementation of scenario 2.
 
     Scenario 2 is based on benchmark 8 of the following paper:
 
         Jean-Francois Aubry, Oscar Bates, Christian Boehm, et al., "Benchmark problems
         for transcranial ultrasound simulation: Intercomparison of compressional wave
         models",
@@ -256,41 +240,41 @@
     def viewer_config_3d(self) -> rendering.ViewerConfig3D:
         """Get the default viewer configuration for the scenario."""
         return rendering.ViewerConfig3D(
             init_angles=(90, 10, -60),
             init_zoom=2.0,
             colormaps={
                 "water": "blue",
-                "skull": "magma",
+                "cortical_bone": "magma",
                 "brain": "bop orange",
             },
             opacities={
                 "water": 0.8,
-                "skull": 0.2,
+                "cortical_bone": 0.2,
                 "brain": 0.2,
             },
         )
 
     def get_default_slice_axis(self) -> int:
         """Get the default slice axis for the scenario."""
         return 2
 
     def get_default_slice_position(self, axis: int) -> float:
         """Get the default slice position for the scenario."""
         default_positions = np.array([0.1, 0.0, 0.0])
         return default_positions[axis]
 
-    def _compile_problem(self) -> stride.Problem:
+    def _compile_problem(self, center_frequency: float) -> stride.Problem:
         extent = np.array([0.225, 0.170, 0.190])  # m
-        return self._compile_scenario_2_problem(extent)
+        return self._compile_scenario_2_problem(extent, center_frequency)
 
     def _get_material_masks(self):
         return {
             name: _create_scenario_2_mask(name, convert_2d=False)
-            for name in self.materials.keys()
+            for name in self.material_layers
         }
 
     def get_default_source(self):
         """Get the default source for the scenario."""
         return sources.FocusedSource3D(
             position=np.array([0.0, 0.0, 0.0]),
             direction=np.array([1.0, 0.0, 0.0]),
@@ -305,15 +289,15 @@
     cur_dir = pathlib.Path(__file__).parent
     data_file = cur_dir / "data" / "skull_mask_bm8_dx_0.5mm.mat"
     mat_data = hdf5storage.loadmat(str(data_file))
 
     skull_mask = mat_data["skull_mask"].astype(np.bool_)
     brain_mask = mat_data["brain_mask"].astype(np.bool_)
 
-    if material == "skull":
+    if material == "cortical_bone":
         mask = skull_mask
 
     elif material == "brain":
         mask = brain_mask
 
     elif material == "water":
         mask = ~(skull_mask | brain_mask)
```

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_shots.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_shots.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_time.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_time.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/_utils.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/_utils.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat` & `neurotechdevkit-0.2.0/src/neurotechdevkit/scenarios/data/skull_mask_bm8_dx_0.5mm.mat`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/src/neurotechdevkit/sources.py` & `neurotechdevkit-0.2.0/src/neurotechdevkit/sources.py`

 * *Files identical despite different names*

### Comparing `neurotechdevkit-0.1.2/PKG-INFO` & `neurotechdevkit-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neurotechdevkit
-Version: 0.1.2
+Version: 0.2.0
 Summary: Neurotech Development Kit: an open-source software library designed to enhance accessibility to cutting-edge neurotechnology
 License: Apache-2.0
 Author: AE Studio
 Author-email: bci@ae.studio
 Maintainer: AE Studio
 Maintainer-email: bci@ae.studio
 Requires-Python: >=3.9,<3.12
```

