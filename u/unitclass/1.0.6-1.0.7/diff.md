# Comparing `tmp/unitclass-1.0.6.tar.gz` & `tmp/unitclass-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitclass-1.0.6.tar", last modified: Mon Jul 17 06:09:21 2023, max compression
+gzip compressed data, was "unitclass-1.0.7.tar", last modified: Mon Jul 17 21:48:19 2023, max compression
```

## Comparing `unitclass-1.0.6.tar` & `unitclass-1.0.7.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 06:09:21.574113 unitclass-1.0.6/
--rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.6/LICENSE
--rw-r--r--   0 blake      (501) staff       (20)     7287 2023-07-17 06:09:21.573977 unitclass-1.0.6/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)     6518 2023-07-17 04:55:49.000000 unitclass-1.0.6/README.md
--rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-17 06:09:05.000000 unitclass-1.0.6/pyproject.toml
--rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-17 06:09:21.574147 unitclass-1.0.6/setup.cfg
-drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 06:09:21.573789 unitclass-1.0.6/unitclass.egg-info/
--rw-r--r--   0 blake      (501) staff       (20)     7287 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/PKG-INFO
--rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/SOURCES.txt
--rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/dependency_links.txt
--rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-17 06:09:21.000000 unitclass-1.0.6/unitclass.egg-info/top_level.txt
--rw-r--r--   0 blake      (501) staff       (20)    47716 2023-07-17 06:08:01.000000 unitclass-1.0.6/unitclass.py
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 21:48:19.570690 unitclass-1.0.7/
+-rw-r--r--   0 blake      (501) staff       (20)    35149 2023-01-29 20:27:25.000000 unitclass-1.0.7/LICENSE
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-07-17 21:48:19.570548 unitclass-1.0.7/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)     6480 2023-07-17 21:47:14.000000 unitclass-1.0.7/README.md
+-rw-r--r--   0 blake      (501) staff       (20)      852 2023-07-17 21:47:37.000000 unitclass-1.0.7/pyproject.toml
+-rw-r--r--   0 blake      (501) staff       (20)       38 2023-07-17 21:48:19.570724 unitclass-1.0.7/setup.cfg
+drwxr-xr-x   0 blake      (501) staff       (20)        0 2023-07-17 21:48:19.570370 unitclass-1.0.7/unitclass.egg-info/
+-rw-r--r--   0 blake      (501) staff       (20)     7249 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/PKG-INFO
+-rw-r--r--   0 blake      (501) staff       (20)      177 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/SOURCES.txt
+-rw-r--r--   0 blake      (501) staff       (20)        1 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/dependency_links.txt
+-rw-r--r--   0 blake      (501) staff       (20)       10 2023-07-17 21:48:19.000000 unitclass-1.0.7/unitclass.egg-info/top_level.txt
+-rw-r--r--   0 blake      (501) staff       (20)    48408 2023-07-17 21:39:22.000000 unitclass-1.0.7/unitclass.py
```

### Comparing `unitclass-1.0.6/LICENSE` & `unitclass-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `unitclass-1.0.6/PKG-INFO` & `unitclass-1.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.6
+Version: 1.0.7
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -243,19 +243,16 @@
 
 ```
 
 ## Caveats
 
 ### Force/Mass
 
-One huge compromise was made in the design of the unit system. Because people
-expect to convert from pounds to kilograms (i.e. force to mass), this library
-designates force as a fundmental unit instead of mass. Mass is defined in terms
-of force and acceleration of gravity. While this differs from the official SI
-Base Units, it makes conversion between force and mass intuitive for the layman
+Because people expect to convert from pounds to kilograms (i.e. force to mass), this library
+will automatically handle conversion to/from forces and masses when explicit conversion is requested. This is accomplished by dividing or multiplying by the acceleration of gravity as needed, which makes conversion between force and mass intuitive for the layman
 and convenient for the rest.
 
 ### Temperature
 
 Because of the nature of the temperature scales, a simple multiplier does not
 work, so temperature is handled independently of the other units. This leads to
 a the limitations that you cannot have custom or compound units with
```

### Comparing `unitclass-1.0.6/README.md` & `unitclass-1.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -225,19 +225,16 @@
 
 ```
 
 ## Caveats
 
 ### Force/Mass
 
-One huge compromise was made in the design of the unit system. Because people
-expect to convert from pounds to kilograms (i.e. force to mass), this library
-designates force as a fundmental unit instead of mass. Mass is defined in terms
-of force and acceleration of gravity. While this differs from the official SI
-Base Units, it makes conversion between force and mass intuitive for the layman
+Because people expect to convert from pounds to kilograms (i.e. force to mass), this library
+will automatically handle conversion to/from forces and masses when explicit conversion is requested. This is accomplished by dividing or multiplying by the acceleration of gravity as needed, which makes conversion between force and mass intuitive for the layman
 and convenient for the rest.
 
 ### Temperature
 
 Because of the nature of the temperature scales, a simple multiplier does not
 work, so temperature is handled independently of the other units. This leads to
 a the limitations that you cannot have custom or compound units with
```

### Comparing `unitclass-1.0.6/pyproject.toml` & `unitclass-1.0.7/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "unitclass"
-version = "1.0.6"
+version = "1.0.7"
 authors = [
   { name="Blake Garretson", email="blake@blakeg.net" },
 ]
 description = "Physical unit class suitable for calculations in the sciences."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `unitclass-1.0.6/unitclass.egg-info/PKG-INFO` & `unitclass-1.0.7/unitclass.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitclass
-Version: 1.0.6
+Version: 1.0.7
 Summary: Physical unit class suitable for calculations in the sciences.
 Author-email: Blake Garretson <blake@blakeg.net>
 Project-URL: Homepage, https://github.com/blakegarretson/unitclass
 Project-URL: Bug Tracker, https://github.com/blakegarretson/unitclass/issues
 Keywords: unit,units,SI,conversion
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -243,19 +243,16 @@
 
 ```
 
 ## Caveats
 
 ### Force/Mass
 
-One huge compromise was made in the design of the unit system. Because people
-expect to convert from pounds to kilograms (i.e. force to mass), this library
-designates force as a fundmental unit instead of mass. Mass is defined in terms
-of force and acceleration of gravity. While this differs from the official SI
-Base Units, it makes conversion between force and mass intuitive for the layman
+Because people expect to convert from pounds to kilograms (i.e. force to mass), this library
+will automatically handle conversion to/from forces and masses when explicit conversion is requested. This is accomplished by dividing or multiplying by the acceleration of gravity as needed, which makes conversion between force and mass intuitive for the layman
 and convenient for the rest.
 
 ### Temperature
 
 Because of the nature of the temperature scales, a simple multiplier does not
 work, so temperature is handled independently of the other units. This leads to
 a the limitations that you cannot have custom or compound units with
```

### Comparing `unitclass-1.0.6/unitclass.py` & `unitclass-1.0.7/unitclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,24 @@
 # key: unique signature of every quantity
 # value: quantity name
 # This is useful to parse an unknown combination of units and determine if
 # it is a known quantity, e.g. N/mm2 is a MPa
 _signatures = {}
 
 
-def _gen_signature(constr):
+def _gen_signature(constr, commonize_forcemass=False):
     """Returns stable identifier/signature for any construction"""
     num, denom = constr
+    if commonize_forcemass:
+        num = [i.replace(
+            'force', 'FORCEorMASS').replace(
+            'mass', 'FORCEorMASS') for i in num]
+        denom = [i.replace(
+            'force', 'FORCEorMASS').replace(
+            'mass', 'FORCEorMASS') for i in denom]
     num = ".".join(sorted(num))
     denom = ".".join(sorted(denom))
     sig = f'{num}|{denom}'
     return sig
 
 
 def _make_signatures():
@@ -335,15 +342,15 @@
 
 
 re_oper = re.compile("(^\(.*?\))|(^(.*?)([*|\/])(.*?)(?=(\(.*?\))|[*\/]|$))"
                      )  # parens group, or next operator
 
 
 def _parse_unit(text, numerator=None, denominator=None, divflip=False, expand=True):
-    """Parse unit str and break down to indvidual components, respecting PEMDAS order 
+    """Parse unit str and break down to indvidual components, respecting PEMDAS order
     of operations and allowing for parentheses.
     e.g.:
 
     >>> _parse_unit('N*m/(s*in)')
     (['N', 'm'], ['s', 'in'])
 
     expand: will call _expand_units()
@@ -588,30 +595,36 @@
     arguments are strings, not Unit class"""
     if not all([from_unit, to_unit]):
         return True  # one of the units is unitless, so it's essentially a scalar
     to_unit_parsed = _parse_unit(to_unit)
     from_unit_parsed = _parse_unit(from_unit)
     to_constr = _get_construction(to_unit_parsed)
     from_constr = _get_construction(from_unit_parsed)
+    # print(from_constr,to_constr)
     if to_constr != from_constr:
         throw_error = False
         if handle_mass_conversion:
             # count mass and force and make sure they are balanced
             # to_constr_list = _get_construction(to_unit_parsed,listform=True)
             # from_constr_list = _get_construction(from_unit_parsed,listform=True)
-            
+
             # get qty for each unit
             # to_qty = [[_units[i]['qty'] for i in lst] for lst in to_unit_parsed]
             # from_qty = [[_units[i]['qty'] for i in lst] for lst in from_unit_parsed]
             to_qty = _get_construction(to_unit_parsed, listform=True, retain_force=True)
             from_qty = _get_construction(from_unit_parsed, listform=True, retain_force=True)
+            # print(from_qty,to_qty)
             to_count = [(lst.count('mass'), lst.count('force')) for lst in to_qty]
             from_count = [(lst.count('force'), lst.count('mass')) for lst in from_qty]
+            to_constr_common = _gen_signature(to_qty, commonize_forcemass=True)
+            from_constr_common = _gen_signature(from_qty, commonize_forcemass=True)
+            # print(to_count,from_count)
+            # print(to_constr_common,from_constr_common)
             # check if difference is just mass and force
-            if to_count != from_count:
+            if (to_count != from_count) or (to_constr_common != from_constr_common):
                 throw_error = True
             else:
                 return from_count
         else:
             throw_error = True
         if throw_error:
             errstr = f"Inconsistent units: {from_unit} is {from_constr}, {to_unit} is {to_constr}"
@@ -712,18 +725,18 @@
 # The below lists are the approved functions that are allowed in
 # math equations during unit imports.
 
 
 def _build_import_funcs():
     """
     Create a dictionary of functions that are allowed to be used in equations
-    in imported CSV files. Most math fuctions from the math module and some 
+    in imported CSV files. Most math fuctions from the math module and some
     from __builtins__ are allowed, and everything else is forbidden.
 
-    Used in conjunction with _import_units() function which actually reads the 
+    Used in conjunction with _import_units() function which actually reads the
     CSV and does the eval().
     """
     available_funcs = {}
     mathops = [
         'acos', 'acosh', 'asin', 'asinh', 'atan', 'atan2', 'atanh', 'cbrt',
         'ceil', 'comb', 'copysign', 'cos', 'cosh', 'degrees', 'dist', 'e',
         'erf', 'erfc', 'exp', 'exp2', 'expm1', 'fabs', 'factorial', 'floor',
@@ -787,24 +800,24 @@
 #######################################################################
 class Unit:
     """
     Unit class
 
     Usage:
     Create Unit w/
-        String: 
+        String:
             Unit("1 N*m")
             Unit("3.4 mi/hr")
-        Int/Float & Str: 
+        Int/Float & Str:
             Unit(1, "N*m")
             Unit(3.4, "mi/hr")
         Create unit and convert:
             Unit(3.4, "mi/hr", "km/hr")
             Unit("3.4 mi/hr km/hr")
-        Create & convert w/ method: 
+        Create & convert w/ method:
             Unit(3.4, "mi/hr").to("km/hr")
     """
 
     def __init__(self, *argv):
         self.to_specials = str.maketrans("0123456789*", "⁰¹²³⁴⁵⁶⁷⁸⁹·")
         self.from_specials = str.maketrans("⁰¹²³⁴⁵⁶⁷⁸⁹⋅·×", "0123456789***")
 
@@ -992,23 +1005,23 @@
             unit_str = unit_str.replace('USD', '')
             format_spec = '.2f'
         number = "{r:{f}}".format(r=self.value, f=format_spec)
         return "{}{} {}".format(prefix, number, unit_str).strip()
 
     def _true_repr(self):
         """
-        This is the true __repr__ method that returns a representation that can 
+        This is the true __repr__ method that returns a representation that can
         reconstruct the object. e.g.:
 
         >>> Unit('2 mm')._true_repr()
         "Unit(2, 'mm')"
 
-        The __repr__ method should really be the __str__ method, but this is library is 
-        intended to be used as an interactive calculator from the REPL, so the str() 
-        output is desired without using print() from the REPL. If you really want the 
+        The __repr__ method should really be the __str__ method, but this is library is
+        intended to be used as an interactive calculator from the REPL, so the str()
+        output is desired without using print() from the REPL. If you really want the
         conventional __repr__ output, this method will do it.
 
         """
         if isinstance(self.value, numbers.Number):
             return f"Unit({self.value:g}, '{self.unit}')"
         else:
             return ""
@@ -1206,14 +1219,15 @@
     # print(Unit('1 stone').to('lb'))
     # print(Unit('1 ton').to('kg'))
     # print(Unit('1 ton').to('lb'))
     # print(Unit('1 N*m').to('in*lb'))
     # print(Unit('1 pcf').to('kg/m3'))
     # print(Unit('40 pcf').to('kg/m3'))
     # print(Unit('40 pcf').to('lb/ft3'))
+    # print(Unit('1 m2').to('ft'))
     # print(Unit('640 kg/m3').to('lb/ft3'))
     # b = Unit(1, 'm')/Unit(1, 'm')
     # print(a)
     # print(a.value,'>', a.unit)
     # print(b)
     # print(b.value,'>', b.unit)
     # print(a+b)
```

