# Comparing `tmp/spmp-0.1.4.tar.gz` & `tmp/spmp-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spmp-0.1.4.tar", last modified: Sun Jul 16 15:01:11 2023, max compression
+gzip compressed data, was "spmp-0.2.0.tar", last modified: Mon Jul 17 19:14:29 2023, max compression
```

## Comparing `spmp-0.1.4.tar` & `spmp-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 15:01:11.701573 spmp-0.1.4/
--rw-rw-rw-   0        0        0    35803 2020-10-31 14:33:20.000000 spmp-0.1.4/LICENSE
--rw-rw-rw-   0        0        0    43078 2023-07-16 15:01:11.696574 spmp-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     1182 2023-07-16 14:53:48.000000 spmp-0.1.4/README.md
--rw-rw-rw-   0        0        0     3508 2023-07-16 14:51:16.000000 spmp-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-16 15:01:11.701573 spmp-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-16 15:01:11.185419 spmp-0.1.4/spmp/
--rw-rw-rw-   0        0        0      949 2023-07-16 14:01:31.000000 spmp-0.1.4/spmp/__init__.py
--rw-rw-rw-   0        0        0     3050 2023-07-16 13:58:33.000000 spmp-0.1.4/spmp/__main__.py
--rw-rw-rw-   0        0        0      744 2023-07-16 14:53:31.000000 spmp-0.1.4/spmp/_version.py
--rw-rw-rw-   0        0        0     6694 2023-07-16 14:01:31.000000 spmp-0.1.4/spmp/naming_convention.py
-drwxrwxrwx   0        0        0        0 2023-07-16 15:01:11.597586 spmp-0.1.4/spmp.egg-info/
--rw-rw-rw-   0        0        0    43078 2023-07-16 15:01:10.000000 spmp-0.1.4/spmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-07-16 15:01:11.000000 spmp-0.1.4/spmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 15:01:10.000000 spmp-0.1.4/spmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 15:01:10.000000 spmp-0.1.4/spmp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-07-16 15:01:10.000000 spmp-0.1.4/spmp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-16 15:01:10.000000 spmp-0.1.4/spmp.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-16 15:01:11.691573 spmp-0.1.4/tests/
--rw-rw-rw-   0        0        0     1928 2023-07-16 13:58:34.000000 spmp-0.1.4/tests/test_satelliteimage.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:14:29.919409 spmp-0.2.0/
+-rw-rw-rw-   0        0        0    35803 2020-10-31 14:33:20.000000 spmp-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0    43376 2023-07-17 19:14:29.915405 spmp-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-07-17 19:11:58.000000 spmp-0.2.0/README.md
+-rw-rw-rw-   0        0        0     3508 2023-07-16 14:51:16.000000 spmp-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:14:29.920404 spmp-0.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-17 19:14:29.457074 spmp-0.2.0/spmp/
+-rw-rw-rw-   0        0        0      949 2023-07-16 14:01:31.000000 spmp-0.2.0/spmp/__init__.py
+-rw-rw-rw-   0        0        0     2815 2023-07-17 19:00:07.000000 spmp-0.2.0/spmp/__main__.py
+-rw-rw-rw-   0        0        0      744 2023-07-17 18:46:48.000000 spmp-0.2.0/spmp/_version.py
+-rw-rw-rw-   0        0        0     6694 2023-07-16 14:01:31.000000 spmp-0.2.0/spmp/naming_convention.py
+drwxrwxrwx   0        0        0        0 2023-07-17 19:14:29.767147 spmp-0.2.0/spmp.egg-info/
+-rw-rw-rw-   0        0        0    43376 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-07-17 19:14:29.000000 spmp-0.2.0/spmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 19:14:29.881406 spmp-0.2.0/tests/
+-rw-rw-rw-   0        0        0     1928 2023-07-16 13:58:34.000000 spmp-0.2.0/tests/test_satelliteimage.py
```

### Comparing `spmp-0.1.4/LICENSE` & `spmp-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spmp-0.1.4/PKG-INFO` & `spmp-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spmp
-Version: 0.1.4
+Version: 0.2.0
 Summary: Satellite Products Metadata Parser
 Author-email: "P. MANCHON" <pierre.manchon@pm.me>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,18 +701,36 @@
 `spmp` uses only built-in packages.
 
 ``pip install spmp``
 
 ## Usage
 The package can be used both as a module and a cli which invoke the same
 function.
+
 #### module
 ```python
 >>> from spmp import parse
 >>> product = parse('path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz')
->>> product.tile = '187021'
+>>> product['title']
+'187021'
 ```
 #### command-line
 ```shell
-$ python spmp -p LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz
-ProductName(program='L', sensor='C', mission='08', processing_level='L1TP', tile='187021', sensing_date='20140328', processing_year='20170424', collection_number='01', collection_category='T1')
+$ python spmp -p path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz
+{'program': 'L',
+ 'sensor': 'C',
+ 'mission': '08',
+ 'processing_level': 'L1TP',
+ 'tile': '187021',
+ 'sensing_date': '20140328',
+ 'processing_year': '20170424',
+ 'collection_number': '01',
+ 'collection_category': 'T1'
+ }
+```
+
+It is quite fast so don't worry about it impacting your performance:
+
+```shell
+ $ python -m timeit -s "from spmp import parse" "parse('path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz')"
+100000 loops, best of 5: 2.01 usec per loop
 ```
```

### Comparing `spmp-0.1.4/pyproject.toml` & `spmp-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spmp-0.1.4/spmp/__init__.py` & `spmp-0.2.0/spmp/__init__.py`

 * *Files identical despite different names*

### Comparing `spmp-0.1.4/spmp/__main__.py` & `spmp-0.2.0/spmp/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import re
 import sys
 from argparse import ArgumentParser
-from collections import namedtuple
 
 try:
     from _version import __version__
     from naming_convention import naming_convention
 except ImportError:
     from spmp._version import __version__
     from spmp.naming_convention import naming_convention
 
 
-def parse(product: str) -> namedtuple:
-    match = None
+def parse(product: str) -> dict:
     result = None
     for k in naming_convention.keys():
         if match := re.search(k, product):
-            result = namedtuple(typename='ProductName',
-                                field_names=' '.join(naming_convention[k].keys()),
-                                rename=True,
-                                defaults=None)
+            result = dict(zip(naming_convention[k].keys(), match.groups()))
             break
     if result is None:
         msg = f'Could not find matching regex for product "{product}"'
         print(msg)
-    return result(*match.groups())
+    return result
 
 
 def run():
     parser = ArgumentParser(prog=f"$ python spmp",
                             description="Satellite Product Metadata Parser",
                             add_help=False,
                             epilog="\n")
```

### Comparing `spmp-0.1.4/spmp/_version.py` & `spmp-0.2.0/spmp/_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-__version__ = '0.1.4'
+__version__ = '0.2.0'
```

### Comparing `spmp-0.1.4/spmp/naming_convention.py` & `spmp-0.2.0/spmp/naming_convention.py`

 * *Files identical despite different names*

### Comparing `spmp-0.1.4/spmp.egg-info/PKG-INFO` & `spmp-0.2.0/spmp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spmp
-Version: 0.1.4
+Version: 0.2.0
 Summary: Satellite Products Metadata Parser
 Author-email: "P. MANCHON" <pierre.manchon@pm.me>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -701,18 +701,36 @@
 `spmp` uses only built-in packages.
 
 ``pip install spmp``
 
 ## Usage
 The package can be used both as a module and a cli which invoke the same
 function.
+
 #### module
 ```python
 >>> from spmp import parse
 >>> product = parse('path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz')
->>> product.tile = '187021'
+>>> product['title']
+'187021'
 ```
 #### command-line
 ```shell
-$ python spmp -p LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz
-ProductName(program='L', sensor='C', mission='08', processing_level='L1TP', tile='187021', sensing_date='20140328', processing_year='20170424', collection_number='01', collection_category='T1')
+$ python spmp -p path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz
+{'program': 'L',
+ 'sensor': 'C',
+ 'mission': '08',
+ 'processing_level': 'L1TP',
+ 'tile': '187021',
+ 'sensing_date': '20140328',
+ 'processing_year': '20170424',
+ 'collection_number': '01',
+ 'collection_category': 'T1'
+ }
+```
+
+It is quite fast so don't worry about it impacting your performance:
+
+```shell
+ $ python -m timeit -s "from spmp import parse" "parse('path/to/LC08_L1TP_187021_20140328_20170424_01_T1.tar.gz')"
+100000 loops, best of 5: 2.01 usec per loop
 ```
```

### Comparing `spmp-0.1.4/tests/test_satelliteimage.py` & `spmp-0.2.0/tests/test_satelliteimage.py`

 * *Files identical despite different names*

