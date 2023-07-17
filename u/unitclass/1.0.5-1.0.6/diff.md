# Comparing `tmp/unitclass-1.0.5.tar.gz` & `tmp/unitclass-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.5.tar", last modified: Fri Jul 14 02:31:42 2023, max compression
+gzip compressed data, was "unitclass-1.0.6.tar", last modified: Mon Jul 17 06:09:21 2023, max compression
```

## Comparing `unitclass-1.0.5.tar` & `unitclass-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-14 02:31:42.877619 unitclass-1.0.5/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.5/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-14 02:31:42.877475 unitclass-1.0.5/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6513 2023-03-20 22:39:31.000000 unitclass-1.0.5/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-14 02:31:00.000000 unitclass-1.0.5/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-14 02:31:42.877661 unitclass-1.0.5/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-14 02:31:42.877283 unitclass-1.0.5/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7282 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-14 02:31:42.000000 unitclass-1.0.5/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    43608 2023-07-14 02:30:50.000000 unitclass-1.0.5/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 06:09:21.574113 unitclass-1.0.6/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.6/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7287 2023-07-17 06:09:21.573977 unitclass-1.0.6/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6518 2023-07-17 04:55:49.000000 unitclass-1.0.6/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-17 06:09:05.000000 unitclass-1.0.6/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-17 06:09:21.574147 unitclass-1.0.6/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 06:09:21.573789 unitclass-1.0.6/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7287 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    47716 2023-07-17 06:08:01.000000 unitclass-1.0.6/unitclass.py
```

### Comparing `unitclass-1.0.5/LICENSE` & `unitclass-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.5/PKG-INFO` & `unitclass-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.5
+Version: 1.0.6
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -155,15 +155,15 @@
 `help(Unit.simplify)` at an interactive prompt.
 
 ```python
 >>> a = Unit('1 W')/Unit('1 A')
 >>> a
 1 W/A
 >>> a.expand()
-1 N·m/(A·s)
+1 m²·kg/(A·s³)
 >>> a.simplify()
 1 V
 
 ```
 
 ### Add Custom Unit
```

### Comparing `unitclass-1.0.5/README.md` & `unitclass-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 `help(Unit.simplify)` at an interactive prompt.
 
 ```python
 >>> a = Unit('1 W')/Unit('1 A')
 >>> a
 1 W/A
 >>> a.expand()
-1 N·m/(A·s)
+1 m²·kg/(A·s³)
 >>> a.simplify()
 1 V
 
 ```
 
 ### Add Custom Unit
```

### Comparing `unitclass-1.0.5/pyproject.toml` & `unitclass-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.5/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.6/unitclass.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.5
+Version: 1.0.6
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -155,15 +155,15 @@
 `help(Unit.simplify)` at an interactive prompt.
 
 ```python
 >>> a = Unit('1 W')/Unit('1 A')
 >>> a
 1 W/A
 >>> a.expand()
-1 N·m/(A·s)
+1 m²·kg/(A·s³)
 >>> a.simplify()
 1 V
 
 ```
 
 ### Add Custom Unit
```

### Comparing `unitclass-1.0.5/unitclass.py` & `unitclass-1.0.6/unitclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,17 +14,20 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 """
-import math, csv, numbers, re
+import math
+import csv
+import numbers
+import re
 
-g = 9.80665  # standard value of accel of gravity
+g_const = 9.80665  # standard value of accel of gravity in m/s2
 
 
 class BadOp(Exception):
     pass
 
 
 class InconsistentUnitsError(Exception):
@@ -45,67 +48,59 @@
 
 # https://www.nist.gov/pml/owm/metric-si/si-units
 # Quantity construction is a list of two lists containing the units in the
 # numerator and the denominator. Multiple units in either list are multiplied.
 # The construction does not need to use the MOST simplified units.
 # e.g. Pa is defined as force over length squared, but then this could be
 # simplified a second time to get base units.
-#
-# The worst bit of nonsense below is making force a fundamental base unit and
-# defining mass in terms of force (m=F/a). This is convenient in order to
-# seemlessly convert between newtons, pounds, grams, etc. as "normal" people expect.
 _quantities = {
     # Fundamental quantiies
     #   Used to define any other unit that will be converted to/from
     #   or will interact with other units.
     'time': [['time'], []],
     'length': [['length'], []],
     'current': [['current'], []],
     'amount': [['amount'], []],
     'luminous_intensity': [['luminous_intensity'], []],
-    'force': [['force'], []],
+    'mass': [['mass'], []],
     'angle': [['angle'], []],
     'unitless': [['unitless'], []],
     # Other special purpose
     'concentration': [['unitless'], []],
     'data': [['data'], []],
     'currency': [['currency'], []],
     # SI
-    'mass': [['force', 'time', 'time'], ['length']],  # force/acceleration
-    'energy': [['force', 'length'], []],
+    'force': [['mass', 'length'], ['time', 'time']],
+    'energy': [['mass', 'length', 'length'], ['time', 'time']],
     'charge': [['current', 'time'], []],
     'catalytic_activity': [['amount'], ['time']],
     'illuminance': [['luminous_intensity', 'angle', 'angle'], ['length'] * 2],
-    'power': [['force', 'length'], ['time']],
-    'pressure': [['force'], ['length'] * 2],
-    'voltage': [['force', 'length'], ['current', 'time']],
-    'magnetic_flux': [['force', 'length', 'time'], ['current', 'time']],
-    'mag_flux_density': [['force', 'length', 'time'],
-                         ['current', 'time', 'length', 'length']],
+    'power': [['mass', 'length', 'length'], ['time']*3],
+    'pressure': [['mass', 'length'], ['length'] * 2+['time']*2],
+    'voltage': [['mass', 'length', 'length'], ['current']+['time']*3],
+    'magnetic_flux': [['mass', 'length', 'length', 'time'], ['current', 'time', 'time', 'time']],
+    'mag_flux_density': [['mass', 'length', 'length', 'time'],
+                         ['current', 'time', 'time', 'time', 'length', 'length']],
     'luminous_flux': [['luminous_intensity', 'angle', 'angle'], []],
     'frequency': [[], ['time']],
     'radionuclide_activity': [[], ['time']],
-    'absorbed_dose': [['force', 'length', 'length'], ['force', 'time',
-                                                      'time']],
-    'resistance': [['force', 'length'], ['current', 'current', 'time']],
-    'inductance': [['force', 'length', 'time'], ['current', 'current',
-                                                 'time']],
-    'capacitance': [['current', 'time', 'current', 'time'],
-                    ['force', 'length']],
+    'absorbed_dose': [['length', 'length'], ['time', 'time']],
+    'resistance': [['mass', 'length', 'length'], ['current', 'current', 'time', 'time', 'time']],
+    'inductance': [['mass', 'length', 'length', 'time'], ['current', 'current', 'time', 'time', 'time']],
+    'capacitance': [['current']*2+['time']*4, ['mass', 'length', 'length']],
     'solid_angle': [['angle'] * 2, []],
-    'dose_equivalent': [['force', 'length', 'length'],
-                        ['force', 'time', 'time']],
-    'conductance': [['current', 'current', 'time'], ['force', 'length']],
+    'dose_equivalent': [['length', 'length'], ['time', 'time']],
+    'conductance': [['current', 'current', 'time', 'time', 'time'], ['mass', 'length', 'length']],
     # other compound units
     'area': [['length'] * 2, []],
     'volume': [['length'] * 3, []],
-    'density': [['force'], ['length'] * 3],
-    'dyn_viscosity': [['force', 'time'], ['length'] * 2],
-    'kin_viscosity': [['energy', 'time'], ['force']],
-    'torque': [['force', 'length'], []],
+    'density': [['mass'], ['length'] * 3],
+    'dyn_viscosity': [['mass', 'length'], ['length'] * 2+['time']],
+    'kin_viscosity': [['energy', 'time', 'time', 'time'], ['mass', 'length']],
+    'torque': [['mass', 'length', 'length'], ['time', 'time']],
     'speed': [['length'], ['time']],
     'angular speed': [['angle'], ['time']],
     'acceleration': [['length'], ['time', 'time']],
     'fluid_flow': [['length'] * 3, ['time']],
 }
 
 # The first unit added in any quantity becomes the default for that unit
@@ -135,28 +130,26 @@
 _make_signatures()
 
 # Format: (quantity, unit, aliases, factor, factor unit)
 #   factor: conversion factor if a factor unit is given
 #     i.e. 1 of the given unit is equal to <factor> <factor units>
 #   factor unit: if not given, the factor is ignored. For clarity, the
 #     factor is set to 1 below to make it obvious that no scaling is done
-# IMPORTANT: Due to pragmatic decisions, all units should be defined in terms
-#            of force, not mass. There should not be a mass quantity in
-#            the list below!
+
 _unit_list = [
     # SI base units
     ('time', 's', 'second seconds sec secs', 1, ''),
     ('length', 'm', 'meter meters metre metres', 1, ''),
     ('current', 'A', 'ampere amperes amp amps', 1, ''),
     ('temperature', '°K', 'K kelvin Kelvin degK', 1, ''),
     ('amount', 'mol', 'mols mole moles', 1, ''),
     ('luminous_intensity', 'cd', 'candela candelas', 1, ''),
     ('energy', 'J', 'joule joules ', 1, ''),
+    ('mass', 'kg', 'kilogram kilograms', 1, ''),
     ('force', 'N', 'newton newtons', 1, ''),
-    ('force', 'g', 'gram grams', g / 1000, 'N'),  # mass kludge
     ('charge', 'C', 'coulomb coulombs', 1, ''),
     ('catalytic_activity', 'kat', 'katal katals', 1, ''),
     ('illuminance', 'lx', 'lux Lux', 1, ''),
     ('power', 'W', 'watt watts', 1, ''),
     ('pressure', 'Pa', 'pascal pascals', 1, ''),
     ('voltage', 'V', 'volt volts', 1, ''),
     ('magnetic_flux', 'Wb', 'weber webers', 1, ''),
@@ -176,14 +169,16 @@
     ('unitless', '', 'unitless _', 1, ''),
     ('time', 'min', 'minute minutes', 60, 's'),
     ('time', 'hr', 'hrs hour hours', 60, 'min'),
     ('time', 'day', 'days', 24, 'hr'),
     ('time', 'week', 'weeks', 7, 'day'),
     ('time', 'fortnight', 'fortnights', 14, 'day'),
     ('time', 'year', 'yr yrs years', 365, 'day'),
+    ('time', 'planck_time', 'Planck_time', 5.39124760e-44, 's'),
+    ('length', 'planck_length', 'Planck_length', 1.61625518e-35, 'm'),
     ('length', 'in', 'inch inches "', 25.4, 'mm'),
     ('length', 'ft', "feet ' foot", 12, 'in'),
     ('length', 'yd', 'yard yards', 36, 'in'),
     ('length', 'mi', 'mile miles statutemile statutemiles smi', 5280, 'ft'),
     ('length', 'nmi', 'nauticalmile nauticalmiles', 1852, 'm'),
     ('length', 'league_land', 'leagues_land', 3, 'mi'),
     ('length', 'league_sea', 'leagues_sea nauticalleague nauticalleagues', 3, 'nmi'),
@@ -202,24 +197,44 @@
     ('length', 'link', 'links', 100, 'chain'),
     ('length', 'us_cable', 'us_cables', 720, 'ft'),
     ('length', 'fathom', 'fathoms', 6, 'ft'),
     ('length', 'hand', 'hands', 4, 'in'),
     ('length', 'bohrrad', 'bohrradius', 5.29177210903e-11, 'm'),
     ('length', 'smoot', 'smoots', 67, 'in'),
     ('length', 'au', 'astrounit', 149597870.691, 'km'),
-    ('acceleration', 'G', 'gravity', g, 'm/s2'),
+    ('force', 'dyn', 'dyne dynes', 1e-5, 'N'),
+    ('force', 'kgf', 'kilogram_force kilopond, kp', 9.80665, 'N'),
+    ('force', 'lb', 'lbf lb_f lbs pound pounds pound_force', 4.4482216, 'N'),  # pound force
+    ('force', 'poundal', 'pdl', 1, 'lb*ft/s2'),
+    ('force', 'kip', 'kips kipf klbf', 1000, 'lb'),
+    ('force', 'oz', 'ounce ounces ozf ounceforce', 1 / 16, 'lb'),
+    ('mass', 'ton', 'tons us_tons shortton', 907.18474, 'kg'),
+    ('mass', 'imp_ton', 'imp_tons longton', 1016.0469088, 'kg'),
+    ('mass', 'mton', 'tonne metricton metric_ton', 1000, 'kg'),
+    ('mass', 'stone', 'stones', 6.35029, 'kg'),
+    ('mass', 'g', 'gram grams', 0.001, 'kg'),
+    ('mass', 'troz', 'troyounce troyounces', 31.1034768, 'g'),
+    ('mass', 'trlb', 'troypound troypounds', 12, 'troz'),
+    ('mass', 'grain', 'grains', 1 / 480, 'troz'),
+    ('mass', 'ct', 'carat carats', 200, 'mg'),
+    ('mass', 'dwt', 'pennyweight', 24, 'grains'),
+    ('mass', 'dalton', 'Da', 1.66e-27, 'kg'),
+    ('mass', 'slug', 'slugs', 14.59390, 'kg'),
+    ('mass', 'lbm', 'lb_m poundmass pound_mass avoirdupois_pound', 0.45359237, 'kg'),
+    ('mass', 'oza', 'avoirdupois_oz avoirdupois_ounces', 1/16, 'lbm'),
+    ('mass', 'planck_mass', 'Planck_mass', 2.17643424e-8, 'kg'),
+    ('mass', 'solar_mass', 'M☉', 1.98847e30, 'kg'),
+    ('acceleration', 'm/s2', '', 1, 'm/s2'),
+    ('acceleration', 'G', 'gravity Gforce', g_const, 'm/s2'),
     ('volume', 'L', 'l liter liters litre litres', 1, 'dm3'),
     # alternate spelling of mL is manually added here for convenience
-    ('volume', 'ml', 'milliliter milliliters millilitre millilitres', 1, 'cm3'
-     ),
+    ('volume', 'ml', 'milliliter milliliters millilitre millilitres', 1, 'cm3'),
     ('volume', 'cc', 'cubic_cm', 1, 'cm3'),
-    ('volume', 'drygal', 'drygallon drygallons us_drygallon drygals', 268.8025,
-     'in3'),  # US
-    ('volume', 'bsh', 'usbsh bushel us_bushel bushels us_bushels', 2150.42,
-     'in3'),  # US
+    ('volume', 'drygal', 'drygallon drygallons us_drygallon drygals', 268.8025, 'in3'),  # US
+    ('volume', 'bsh', 'usbsh bushel us_bushel bushels us_bushels', 2150.42, 'in3'),  # US
     ('volume', 'gal', 'gallon gallons us_gallon gals', 231, 'in3'),  # US
     ('volume', 'peck', 'pecks uspecks', 0.25, 'bsh'),
     ('volume', 'floz', 'flounce fluidounce us_floz', 1 / 128, 'gal'),  # US
     ('volume', 'quart', 'quarts qt qts us_qt', 32, 'floz'),  # US
     # pint: not using pt or pts because of conflict with typography unit
     ('volume', 'pint', 'pints', 16, 'floz'),  # US,
     ('volume', 'cup', 'cups', 8, 'floz'),  # US
@@ -233,46 +248,33 @@
     ('volume', 'imp_pt', 'imp_pint', 20, 'imp_floz'),
     ('volume', 'imp_cup', '', 10, 'imp_floz'),
     ('volume', 'imp_gill', '', 5, 'imp_floz'),
     ('volume', 'imp_fldram', '', 1 / 8, 'imp_floz'),
     ('area', 'acre', 'acres', 43560, 'ft2'),
     ('area', 'sqft', 'squarefeet squarefoot', 1, 'ft2'),
     ('area', 'sqin', 'squareinches', 1, 'in2'),
-    ('force', 'dyn', 'dyne dynes', 1e-5, 'N'),
-    ('force', 'lb', 'lbf lb_f lbs pound pounds', 4.4482216,
-     'N'),  # pound force
-    ('force', 'kip', 'kips kipf klbf', 1000, 'lb'),
-    ('force', 'oz', 'ounce ounces ozf ounceforce', 1 / 16, 'lb'),
-    ('force', 'troz', 'troyounce troyounces', 31.1034768, 'g'),
-    ('force', 'trlb', 'troypound troypounds', 12, 'troz'),
-    ('force', 'grain', 'grains', 1 / 480, 'troz'),
-    ('force', 'ton', 'tons us_tons shortton', 2000, 'lb'),
-    ('force', 'imp_ton', 'imp_tons longton', 2240, 'lb'),
-    ('force', 'mton', 'metricton metric_ton', 1000, 'kg'),
-    ('force', 'ct', 'carat carats', 200, 'mg'),
-    ('force', 'stone', 'stones', 14, 'lb'),
-    ('force', 'slug', 'slugs', 32.174, 'lb'),
-    ('force', 'dwt', 'pennyweight', 24, 'grains'),
     ('pressure', 'psi', '', 1, 'lb/in2'),
     ('pressure', 'psf', '', 1 / 144, 'lb/in2'),
     ('pressure', 'ksi', '', 1000, 'lb/in2'),
     ('pressure', 'inHg', 'inhg', 3386.388640341, 'Pa'),
     ('pressure', 'inH2O', 'inh2o', 249.082, 'Pa'),
     ('pressure', 'bar', 'bars', 100000, 'Pa'),
     ('pressure', 'mBar', 'mbar mbars millibar', 100, 'Pa'),
     ('pressure', 'atm', 'atmosphere', 101325, 'Pa'),
-    ('density', 'pcf', 'PCF', 1, 'lb/ft3'),
+    ('density', 'pcf', 'PCF', 16.01846337, 'kg/m3'),
+    # ('density', 'pcf', 'PCF', 1, 'lb/ft3'),
     ('power', 'hp', 'horsepower', 550, 'ft*lb/s'),
     ('dyn_viscosity', 'cP', 'centipoise', 1, 'mPa*s'),
     ('dyn_viscosity', 'P', 'poise', 100, 'cP'),
     ('kin_viscosity', 'St', 'stokes stoke', 0.0001, 'm2/s'),
     ('kin_viscosity', 'cSt', 'centistokes centistoke', 1e-6, 'm2/s'),
     ('energy', 'BTU', 'thermochemicalBTU', 4.184 * 453.59237 * 5 / 9, 'J'),
     ('energy', 'cal', 'calorie', 4.184, 'J'),
     ('energy', 'kcal', 'kilocalorie', 1000, 'cal'),
+    ('energy', 'electronvolt', 'eV', 1.602176634e-19, 'J'),
     ('temperature', '°C', 'CC celsius centigrade degC', 1, ''),
     ('temperature', '°F', 'FF fahrenheit degF', 1, ''),
     ('angle', '°', 'deg degree degrees', math.pi / 180, 'rad'),
     ('angle', 'rev', 'revolution revolutions', 360, 'deg'),
     ('angle', 'grad', 'grads gradian gradians grade gon', math.pi / 200,
      'rad'),
     ('angle', 'turn', 'turns', 1, 'rev'),
@@ -301,49 +303,55 @@
     ('concentration', 'ppm', 'partspermillion', 1e-4, 'pct'),
     ('concentration', 'ppb', 'partsperbillion', 1e-7, 'pct'),
     ('fluid_flow', 'gpm', 'galpermin', 1, 'gal/min'),
     ('fluid_flow', 'gph', 'galperhr', 1, 'gal/hr'),
     ('fluid_flow', 'cfm', 'cubicftperminute', 1, 'ft3/min'),
     ('fluid_flow', 'cfs', 'cubicftpersec', 1, 'ft3/sec'),
     ('fluid_flow', 'lpm', 'literspermin', 1, 'L/min'),
-    ('torque', 'in*lb', 'inchpound inlb', 1, 'in*lb'),
-    ('torque', 'ft*lb', 'footpound ftlb', 1, 'ft*lb'),
+    ('torque', 'inlb', 'inchpound', 1, 'in*lb'),
+    ('torque', 'ftlb', 'footpound', 1, 'ft*lb'),
 ]
 
 # SI prefix info
 _prefix_units = 'm g s A L J N Pa W Ω V C F H Hz'.split()
+_prefix_units_names = 'meter gram second amp liter joule newton pascal weber ohm volt coulomb farad henry hertz'.split()
 _prefix_mult = (1e18, 1e15, 1e12, 1e9, 1e6, 1e3, 1e-1, 1e-2, 1e-3, 1e-6, 1e-9,
                 1e-12, 1e-15)
 _prefixes = list("EPTGMkdcmμnpf")
+_prefix_aliases = ['exa', 'peta', 'tera', 'giga', 'mega', 'kilo',
+                   'deci', 'centi', 'milli', 'micro', 'nano', 'pico', 'femto']
 
 
 def _expand_units(unitlist):
     """Take a list of units and return a list with exponents
     expanded to individual units.  e.g. ["N","m2"] -> ["N", "m", "m"]
     """
     newlist = []
     for u in unitlist:
         if u and u[-1].isdigit():
             newlist.extend([u[:-1]] * int(u[-1]))
         else:
             newlist.append(u)
     return newlist
 
+
 re_oper = re.compile("(^\(.*?\))|(^(.*?)([*|\/])(.*?)(?=(\(.*?\))|[*\/]|$))"
                      )  # parens group, or next operator
+
+
 def _parse_unit(text, numerator=None, denominator=None, divflip=False, expand=True):
     """Parse unit str and break down to indvidual components, respecting PEMDAS order 
     of operations and allowing for parentheses.
     e.g.:
 
     >>> _parse_unit('N*m/(s*in)')
     (['N', 'm'], ['s', 'in'])
 
     expand: will call _expand_units()
-    """    
+    """
     if not numerator:
         numerator = []
     if not denominator:
         denominator = []
     text = text.strip()
     if divflip:
         numerator, denominator = denominator, numerator
@@ -351,48 +359,53 @@
     while match := re_oper.search(text):
         parens = match.group(1)
         term1 = match.group(3)
         op = match.group(4)
         term2 = match.group(5)
         term2_parens = match.group(6)
 
-        if op in ('*','×','·','•','⋅'):
+        if op in ('*', '×', '·', '•', '⋅'):
             end = match.end()
-            if term1: numerator.append(term1)
-            if term2: numerator.append(term2)
+            if term1:
+                numerator.append(term1)
+            if term2:
+                numerator.append(term2)
             elif term2_parens:
                 numerator, denominator = _parse_unit(
                     term2_parens[1:-1], numerator, denominator, expand=False)
                 end += len(term2_parens)
             text = text[end:]
-        elif op in ('/','÷'):
+        elif op in ('/', '÷'):
             end = match.end()
-            if term1: numerator.append(term1)
-            if term2: denominator.append(term2)
+            if term1:
+                numerator.append(term1)
+            if term2:
+                denominator.append(term2)
             elif term2_parens:  # flip num/denom since it's being divided
                 numerator, denominator = _parse_unit(term2_parens[1:-1],
-                                                          numerator,
-                                                          denominator,
-                                                          divflip=True, expand=False)
+                                                     numerator,
+                                                     denominator,
+                                                     divflip=True, expand=False)
                 end += len(term2_parens)
             text = text[end:]
         elif parens:
             text = text[match.end():]
             numerator, denominator = _parse_unit(parens[1:][:-1],
-                                                      numerator, denominator, expand=False)
+                                                 numerator, denominator, expand=False)
     if text:  # just a single term left
         numerator.append(text)
         text = ''
     if divflip:
         numerator, denominator = denominator, numerator
     if expand:
         numerator = _expand_units(numerator)
         denominator = _expand_units(denominator)
     return numerator, denominator
 
+
 def _get_unit(unit):
     """Returns unit dict, handling aliases too"""
     if unit in _units:
         return _units[unit]
     elif unit in _aliases:
         return _units[_aliases[unit]]
     else:
@@ -425,36 +438,39 @@
 
 def add_unit(qty, unit, alias_list, factor, factor_unit):
     """Create unit definition.
     Takes arguments in this format:
     add_unit(<quantity>, <name>, <aliases>, <factor>, <factor unit>)
     e.g. add_unit('length', "in", 'inch inches', 25.4, 'mm')
 
-    >>> add_unit("length", "blake", "blakes bunits", 6, 'ft')
-
     factor: this is a conversion factor to specify the equivalent
             quantity in a different unit. In the above example
             1 inch is equivalent to 25.4 mm.
+
+    >>> add_unit("length", "blake", "blakes bunits", 6, 'ft')
+
     """
     if factor_unit:
         factor *= _get_factors(factor_unit)
     _units[unit] = {
         'factor': factor,
         'qty': qty,
         'aliases': alias_list.split()
     }
     if qty not in _defaults:
         _defaults[qty] = unit
     # add SI prefixes for certain units
     if unit in _prefix_units:
-        for mult, prefix in zip(_prefix_mult, _prefixes):
+        for mult, prefix, alias_prefix, prefix_unit_name in zip(_prefix_mult, _prefixes, _prefix_aliases, _prefix_units_names):
+            if prefix+unit == 'kg':  # skip fundamental mass unit
+                continue
             _units[prefix + unit] = {
                 'factor': mult * factor,
                 'qty': qty,
-                'aliases': []
+                'aliases': [alias_prefix+prefix_unit_name, alias_prefix+prefix_unit_name+'s']
             }
             if unit == 'Ω':
                 _aliases[prefix + 'ohm'] = prefix + unit
                 _units[prefix + unit]['aliases'].append(prefix + 'ohm')
             if prefix == 'μ':
                 _aliases['u' + unit] = prefix + unit
                 _units[prefix + unit]['aliases'].append('u' + unit)
@@ -514,71 +530,103 @@
     denom_str = "*".join(new_denom)
     if num_str == '' and denom_str == '':
         new_unit = ""
     elif denom_str == '':
         new_unit = num_str
     else:
         if len(new_denom) > 1:
-            new_unit = f"{num_str}/({denom_str})" # parens
+            new_unit = f"{num_str}/({denom_str})"  # parens
         else:
             new_unit = f"{num_str}/{denom_str}"
     return new_unit
 
 
-def _get_construction(fractional_unit, combine=False, listform=False):
-    """Reduce the units down to the fundamental quantities (length, force, time, etc.)
+def _get_construction(fractional_unit, combine=False, listform=False, retain_force=False):
+    """Reduce the units down to the fundamental quantities (length, mass, time, etc.)
     This should be used with the _parse_unit() function to split
     the unit into fractional parts and pass the pair into this function.
     """
     num, denom = fractional_unit
     num_constr = [_get_unit(i)['qty'] for i in num]
     denom_constr = [_get_unit(i)['qty'] for i in denom]
+    new_num_constr = []
+    new_denom_constr = []
     for u in num_constr:
-        if u in _quantities:
+        if retain_force and (u == 'force'):
+            new_num_constr.append(u)
+        elif u in _quantities:
             n, d = _quantities[u]
-            num_constr.remove(u)
-            num_constr.extend(n)
-            denom_constr.extend(d)
+            new_num_constr.extend(n)
+            new_denom_constr.extend(d)
+        else:
+            new_num_constr.append(u)
     for u in denom_constr:
-        if u in _quantities:
+        if retain_force and (u == 'force'):
+            new_denom_constr.append(u)
+        elif u in _quantities:
             n, d = _quantities[u]
-            denom_constr.remove(u)
-            num_constr.extend(d)
-            denom_constr.extend(n)
+            new_num_constr.extend(d)
+            new_denom_constr.extend(n)
+        else:
+            new_denom_constr.append(u)
+    num_constr = new_num_constr
+    denom_constr = new_denom_constr
     num_constr, denom_constr = _simplify_unit(num_constr, denom_constr)
     num_constr.sort()
     denom_constr.sort()
     if num_constr in ([], [''], ['unitless'], ['1']):
         num_constr = ['']
     if listform:
         return [num_constr, denom_constr]
     else:
         construction = _make_name(num_constr, denom_constr, combine=combine)
         return construction
 
 
-def _check_consistent_units(from_unit, to_unit, silent=False):
+def _check_consistent_units(from_unit, to_unit, silent=False, handle_mass_conversion=False):
     """Return True if units are fundamentally the same OR if one is unitless
-    
+
     arguments are strings, not Unit class"""
     if not all([from_unit, to_unit]):
-        return True # one of the units is unitless, so it's essentially a scalar
-    to_constr = _get_construction(_parse_unit(to_unit))
-    from_constr = _get_construction(_parse_unit(from_unit))
+        return True  # one of the units is unitless, so it's essentially a scalar
+    to_unit_parsed = _parse_unit(to_unit)
+    from_unit_parsed = _parse_unit(from_unit)
+    to_constr = _get_construction(to_unit_parsed)
+    from_constr = _get_construction(from_unit_parsed)
     if to_constr != from_constr:
-        errstr = f"Error: Units are not consistent.\n" +\
-            f"       {from_unit} is {from_constr}\n" +\
-            f"       {to_unit} is {to_constr}"
-        if not silent:
-            raise InconsistentUnitsError(errstr)
+        throw_error = False
+        if handle_mass_conversion:
+            # count mass and force and make sure they are balanced
+            # to_constr_list = _get_construction(to_unit_parsed,listform=True)
+            # from_constr_list = _get_construction(from_unit_parsed,listform=True)
+            
+            # get qty for each unit
+            # to_qty = [[_units[i]['qty'] for i in lst] for lst in to_unit_parsed]
+            # from_qty = [[_units[i]['qty'] for i in lst] for lst in from_unit_parsed]
+            to_qty = _get_construction(to_unit_parsed, listform=True, retain_force=True)
+            from_qty = _get_construction(from_unit_parsed, listform=True, retain_force=True)
+            to_count = [(lst.count('mass'), lst.count('force')) for lst in to_qty]
+            from_count = [(lst.count('force'), lst.count('mass')) for lst in from_qty]
+            # check if difference is just mass and force
+            if to_count != from_count:
+                throw_error = True
+            else:
+                return from_count
         else:
-            return False
+            throw_error = True
+        if throw_error:
+            errstr = f"Inconsistent units: {from_unit} is {from_constr}, {to_unit} is {to_constr}"
+            if not silent:
+                raise InconsistentUnitsError(errstr)
+            else:
+                return False
     else:
         return True
 
+
 def _convert_C2F(value):
     return value * 9.0 / 5.0 + 32
 
 
 def _convert_F2C(value):
     return (value - 32) * 5.0 / 9.0
 
@@ -593,18 +641,18 @@
 
 def convert(value, from_unit, to_unit):
     """Convert value from original unit to new unit
     Example: convert(40, 'pcf', 'kg/m3') returns 640.7
     Special cases include temperature
     """
     # TODO: this doesn't handle compound units with temperature, like J/degC
-    
-    if (not to_unit) and (from_unit != '%'): # unitless, treat as same unit
+
+    if (not to_unit) and (from_unit != '%'):  # unitless, treat as same unit
         return value
-    elif (not from_unit) and (to_unit != '%'): # unitless, treat as same unit
+    elif (not from_unit) and (to_unit != '%'):  # unitless, treat as same unit
         return value
 
     both = _get_unit_name(from_unit, ignore_error=True) + \
         _get_unit_name(to_unit, ignore_error=True)
     if both == '°C°F':
         newvalue = _convert_C2F(value)
     elif both == '°F°C':
@@ -614,16 +662,28 @@
     elif both == '°C°K':
         newvalue = _convert_C2K(value)
     elif both == '°F°K':
         newvalue = _convert_C2K(_convert_F2C(value))
     elif both == '°K°F':
         newvalue = _convert_C2F(_convert_K2C(value))
     else:
-        _check_consistent_units(from_unit, to_unit)
-        newvalue = value * _get_factors(from_unit) / _get_factors(to_unit)
+        forcemass_counts = _check_consistent_units(from_unit, to_unit, handle_mass_conversion=True)
+        mass_factor = 1
+        if isinstance(forcemass_counts, list):
+            num_force, num_mass = forcemass_counts[0]
+            den_force, den_mass = forcemass_counts[1]
+            if num_force:
+                mass_factor = mass_factor/(num_force*g_factor)
+            if num_mass:
+                mass_factor = mass_factor*(num_mass*g_factor)
+            if den_force:
+                mass_factor = mass_factor*(den_force*g_factor)
+            if den_mass:
+                mass_factor = mass_factor/(den_mass*g_factor)
+        newvalue = mass_factor * value * _get_factors(from_unit) / _get_factors(to_unit)
     return newvalue
 
 
 def list_quantities():
     """List available quantities"""
     [print(x) for x in sorted(list(_quantities.keys()))]
 
@@ -639,15 +699,15 @@
             the search term.
     """
     if not qty:
         qty = _quantities.keys()
     for name, unit in _units.items():
         if unit['qty'] in qty:
             if ((not search) or (search in name) or any(
-                (search in x) for x in unit['aliases'])):
+                    (search in x) for x in unit['aliases'])):
                 print(
                     f"{name:6}->unit of {unit['qty']:10} aliases: {unit['aliases'] if unit['aliases'] else []}"
                 )
 
 
 # The below lists are the approved functions that are allowed in
 # math equations during unit imports.
@@ -751,36 +811,36 @@
         value = None
         unit = ''
         to_unit = ''
 
         if not argv:
             raise Exception("No arguments given for Unit.")
         elif len(argv) == 1:  # 1, '1', '1 mm', '1 mm in'
-            arg =  argv[0]
-            if isinstance(arg, Unit): # pass through, if you try to instance a Unit
+            arg = argv[0]
+            if isinstance(arg, Unit):  # pass through, if you try to instance a Unit
                 unit = arg.unit
                 value = arg.value
-            elif isinstance(arg, (float,int)): # -> 1
+            elif isinstance(arg, (float, int)):  # -> 1
                 value = arg
-            elif isinstance(arg, str): # -> '1' or 'mm' or '1 mm' or '1 mm in'
+            elif isinstance(arg, str):  # -> '1' or 'mm' or '1 mm' or '1 mm in'
                 if arg.startswith('$'):
                     items = arg[1:].split()
                     items = [items[0], 'USD']+items[1:]
                 else:
                     items = arg.split()
                 if len(items) == 1:
                     item = items[0]
-                    if all([(i in '0123456789-+.') for i in item]): # is number
+                    if all([(i in '0123456789-+.') for i in item]):  # is number
                         value = item
-                    else: # is a unit with no value given
+                    else:  # is a unit with no value given
                         value = 1
                         unit = item
-                elif len(items) == 2: # -> 1,'mm'
+                elif len(items) == 2:  # -> 1,'mm'
                     value, unit = items
-                elif len(items) == 3: # -> 1, 'mm', 'in' (convert on the fly)
+                elif len(items) == 3:  # -> 1, 'mm', 'in' (convert on the fly)
                     value, unit, to_unit = items
                 else:
                     raise Exception(f"Too many arguments given: {items}")
         elif len(argv) == 2:
             value, unit = argv
         else:
             value, unit, to_unit, *_ = argv
@@ -802,22 +862,22 @@
         Operations:
         - Verifies unit is in database
         - Checks for aliases (throws exception if it isn't available)
         - Replace superscripts and special characters in case they were passed in
         - if one of the Unit objects was unitless, it removes the empty string from the name
         - Returns primary name (after replacements)
         """
-        return _get_unit_name(unit_str.translate(self.from_specials).replace('^','').replace('**',''))
+        return _get_unit_name(unit_str.translate(self.from_specials).replace('^', '').replace('**', ''))
 
     def _tocopy(self, newunit):
         """Converts and returns a new Unit() copy"""
         newunit = self._validate_unit(newunit)
         value = convert(self.value, self.unit, newunit)
         return Unit(value, newunit)
-    
+
     def to(self, newunit):
         """Converts in-place, and returns self for viewing the result in Jupyter immediately"""
         newunit = self._validate_unit(newunit)
         self.value = convert(self.value, self.unit, newunit)
         self.unit = newunit
         return self
 
@@ -853,15 +913,15 @@
                 raise BadOp(
                     "Bad op passed. Must be: addsub, pow, mul, div, rdiv")
 
         return _make_name(num, denom)
 
     def expand(self,
                length=_defaults['length'],
-               force=_defaults['force'],
+               mass=_defaults['mass'],
                time=_defaults['time'],
                temperature=_defaults['temperature'],
                current=_defaults['current'],
                angle=_defaults['angle'],
                unitless=_defaults['unitless'],
                amount=_defaults['amount'],
                luminous_intensity=_defaults['luminous_intensity']):
@@ -877,35 +937,39 @@
 
         Examples:
 
         >>> a = Unit('1 W')/Unit('1 A')
         >>> a
         1 W/A
         >>> a.expand()
-        1 N·m/(A·s)
-        >>> a.expand(time='ms', force='lb')
-        0.000224809 lb·m/(A·ms)
-                        
+        1 m²·kg/(A·s³)
+        >>> a.expand(time='ms', mass='g', length='mm')
+        1 mm²·g/(A·ms³)
+
         """
+        # self.simplify()
         constr = _get_construction(_parse_unit(self.unit), combine=True)
 
         constr = constr.replace("length", length).replace(  # type: ignore
-            "force", force).replace("time", time).replace(
-                "temperature",
-                temperature).replace("current", current).replace(
-                    "angle", angle).replace("unitless", unitless).replace(
-                        "luminous_intensity",
-                        luminous_intensity).replace("amount", amount)
+            "mass", mass).replace(
+            # 'force',force).replace(
+            "time", time).replace(
+            "temperature", temperature).replace(
+            "current", current).replace(
+            "angle", angle).replace(
+            "unitless", unitless).replace(
+            "luminous_intensity", luminous_intensity).replace(
+            "amount", amount)
         self.to(constr)
         return self
 
     def simplify(self):
         """Attempts to find a unit that fits the fundamental quantities of this Unit.
         This does nothing if it can't find a better compound unit to use instead.
-        
+
         >>> a = Unit('1 W')/Unit('1 A')
         >>> a
         1 W/A
         >>> a.simplify()
         1 V
 
         """
@@ -921,15 +985,15 @@
         return self
 
     def __format__(self, format_spec):
         unit_str = self.unit.translate(self.to_specials)
         prefix = ''
         if 'USD' in unit_str:
             prefix = '$'
-            unit_str = unit_str.replace('USD','')
+            unit_str = unit_str.replace('USD', '')
             format_spec = '.2f'
         number = "{r:{f}}".format(r=self.value, f=format_spec)
         return "{}{} {}".format(prefix, number, unit_str).strip()
 
     def _true_repr(self):
         """
         This is the true __repr__ method that returns a representation that can 
@@ -961,23 +1025,23 @@
 
         """
         if isinstance(self.value, numbers.Number):
             unit_str = self.unit.translate(self.to_specials)
             prefix = ''
             if 'USD' in unit_str:
                 prefix = '$'
-                unit_str = unit_str.replace('USD','')
-            return "{}{:g} {}".format(prefix,self.value, unit_str).strip()
+                unit_str = unit_str.replace('USD', '')
+            return "{}{:g} {}".format(prefix, self.value, unit_str).strip()
         else:
             return ""
 
     def __mul__(self, other):
         other = Unit(other)
         if all([_check_consistent_units(self.unit, other.unit, silent=True),
-                    (self.unit != other.unit), all( [self.unit,other.unit]) ]):
+                (self.unit != other.unit), all([self.unit, other.unit])]):
             # this ensures we don't have 2in * 3m = 6 in*m
             # If we have the same fundamental quantity (e.g. length), make them the same
             # before the operation
             other = other._tocopy(self.unit)
         newunit = self._new_unit(other, op="mul")
         newvalue = self.value * other.value  # type: ignore
         if (not newunit) and (not isinstance(other, Unit)):
@@ -986,21 +1050,21 @@
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def __truediv__(self, other, op='div'):
         other = Unit(other)
         if all([_check_consistent_units(self.unit, other.unit, silent=True),
-                    (self.unit != other.unit), all( [self.unit,other.unit]) ]):
+                (self.unit != other.unit), all([self.unit, other.unit])]):
             # this ensures we don't have 2in * 3m = 6 in*m
             # If we have the same fundamental quantity (e.g. length), make them the same
             # before the operation
             other = other._tocopy(self.unit)
         newunit = self._new_unit(other, op=op)
-        newvalue = (self.value / other.value) if op=='div' else (other.value/self.value)
+        newvalue = (self.value / other.value) if op == 'div' else (other.value/self.value)
         new_constr = _get_construction(_parse_unit(newunit))
         self_constr = self._get_construction()
         other_constr = other._get_construction()
         u = Unit(newvalue, newunit)
         if new_constr == self_constr:
             u.to(self.unit)
         elif new_constr == other_constr:
@@ -1050,21 +1114,21 @@
         return float(self.value)  # type: ignore
 
     def __int__(self):
         return int(self.value)  # type: ignore
 
     def __abs__(self):
         return Unit(abs(self.value), self.unit)  # type: ignore
-    
+
     def __pos__(self):
         return self
-    
+
     def __neg__(self):
         return Unit(-self.value, self.unit)  # type: ignore
-    
+
     def __lt__(self, other):
         if isinstance(other, Unit):
             _check_consistent_units(other.unit, self.unit)
             other = convert(other.value, other.unit, self.unit)
         return self.value < other
 
     def __le__(self, other):
@@ -1094,40 +1158,72 @@
     def __ge__(self, other):
         if isinstance(other, Unit):
             _check_consistent_units(other.unit, self.unit)
             other = convert(other.value, other.unit, self.unit)
         return self.value >= other
 
 
+g = Unit(g_const, 'm/s2')
+c = Unit(299792458, 'm/s')
+g_factor = g_const*_get_factors('m/s2')
+
 __all__ = [
     'Unit', 'convert', 'add_unit', 'list_units', 'import_units',
-    'list_quantities'
+    'list_quantities', 'g', 'c'
 ]
 
 if __name__ == '__main__':
+    pass
     import doctest
     doctest.testmod()
     doctest.testfile('doctests.txt')
     doctest.testfile('README.md', optionflags=doctest.ELLIPSIS+doctest.NORMALIZE_WHITESPACE)
 
     # print(Unit(4, 'in2')/Unit(50.8,'mm'))
     # print(Unit(50.8,'mm2')/Unit(4, 'in'))
     # print(4/Unit('2 m'))
     # print(Unit('4 m')/Unit('2 m'))
-    print(Unit('1 USD'))
-    print(Unit('$1.00'))
-    print("{:.10g}".format(Unit('1.00 USD/sqft')))
+    # print(Unit('1 USD'))
+    # print(Unit('$1.00'))
+    # print("{:.10g}".format(Unit('1.00 USD/sqft')))
     # print(Unit('1 USD')/Unit('sqft'))
     # print(Unit('1 USD').to('pennies'))
     # print(Unit('4 m2')/Unit('2 m'))
     # print(Unit(50.8,'mm')*Unit(4, 'in'))
     # print(Unit('1 m')/Unit('1 m'))
     # print(Unit('1 m')/Unit('1 m') + Unit('1 m'))
     # print(Unit('1 m') + Unit('1 m')/Unit('1 m'))
-    # a = Unit(1, 'in')
+    # print(Unit('1 (N*in)/s').to('gram*mm/s'))
+    # print(Unit('1 lb').to('kg'))
+    # print(Unit('1 kg').to('N'))
+    # print(Unit('1 N').to('kg'))
+    # print(Unit('1 N').to('lb'))
+    # print(Unit('1 lb').to('kg'))
+    # print(Unit('1 kg').to('N'))
+    # print(Unit('1 kg').to('lb'))
+    # print(Unit('1 m/kg2').to('m/lb2'))
+    # print((Unit('1 N')/Unit('1 kg')).simplify().to('m/s2'))
+    # print((Unit('1 N')/Unit('1 kg')).simplify())
+    # print(Unit('1 stone').to('lb'))
+    # print(Unit('1 ton').to('kg'))
+    # print(Unit('1 ton').to('lb'))
+    # print(Unit('1 N*m').to('in*lb'))
+    # print(Unit('1 pcf').to('kg/m3'))
+    # print(Unit('40 pcf').to('kg/m3'))
+    # print(Unit('40 pcf').to('lb/ft3'))
+    # print(Unit('640 kg/m3').to('lb/ft3'))
     # b = Unit(1, 'm')/Unit(1, 'm')
     # print(a)
     # print(a.value,'>', a.unit)
     # print(b)
     # print(b.value,'>', b.unit)
     # print(a+b)
     # print(b+a)
+
+    # print(_units['N'])
+
+    # a = Unit('1 W/A')
+    # # a = Unit('1 W')/Unit('1 A')
+    # a.expand()
+    # print(a)
+    # a.simplify()
+    # print(a)
```

