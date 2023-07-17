# Comparing `tmp/kirkwoodnight-1.0.3.tar.gz` & `tmp/kirkwoodnight-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kirkwoodnight-1.0.3.tar", last modified: Fri Jul 14 17:40:57 2023, max compression
+gzip compressed data, was "kirkwoodnight-1.0.4.tar", last modified: Mon Jul 17 19:59:03 2023, max compression
```

## Comparing `kirkwoodnight-1.0.3.tar` & `kirkwoodnight-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.446102 kirkwoodnight-1.0.3/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.3/LICENSE.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5951 2023-07-14 17:40:57.445554 kirkwoodnight-1.0.3/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5488 2023-07-14 17:39:27.000000 kirkwoodnight-1.0.3/README.md
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.436800 kirkwoodnight-1.0.3/kirkwoodnight/
--rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.3/kirkwoodnight/__init__.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.3/kirkwoodnight/command_line.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.444035 kirkwoodnight-1.0.3/kirkwoodnight/data/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.3/kirkwoodnight/data/obj_list.csv
--rw-r--r--   0 armaangoyal   (501) staff       (20)     6350 2023-07-14 03:09:07.000000 kirkwoodnight-1.0.3/kirkwoodnight/plotting.py
--rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 17:40:08.000000 kirkwoodnight-1.0.3/kirkwoodnight/source.py
-drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-14 17:40:57.443296 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/
--rw-r--r--   0 armaangoyal   (501) staff       (20)     5951 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/PKG-INFO
--rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/SOURCES.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/dependency_links.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/entry_points.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/requires.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-14 17:40:57.000000 kirkwoodnight-1.0.3/kirkwoodnight.egg-info/top_level.txt
--rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-14 17:40:57.446322 kirkwoodnight-1.0.3/setup.cfg
--rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-14 17:40:02.000000 kirkwoodnight-1.0.3/setup.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-17 19:59:03.684282 kirkwoodnight-1.0.4/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1119 2023-07-12 19:15:12.000000 kirkwoodnight-1.0.4/LICENSE.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5982 2023-07-17 19:59:03.683972 kirkwoodnight-1.0.4/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5519 2023-07-17 19:54:22.000000 kirkwoodnight-1.0.4/README.md
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-17 19:59:03.679923 kirkwoodnight-1.0.4/kirkwoodnight/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        0 2023-07-12 19:58:50.000000 kirkwoodnight-1.0.4/kirkwoodnight/__init__.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     4304 2023-07-14 02:42:02.000000 kirkwoodnight-1.0.4/kirkwoodnight/command_line.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-17 19:59:03.682920 kirkwoodnight-1.0.4/kirkwoodnight/data/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     7833 2023-07-13 23:53:52.000000 kirkwoodnight-1.0.4/kirkwoodnight/data/obj_list.csv
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     6354 2023-07-17 19:52:55.000000 kirkwoodnight-1.0.4/kirkwoodnight/plotting.py
+-rw-r--r--   0 armaangoyal   (501) staff       (20)    18480 2023-07-14 17:40:08.000000 kirkwoodnight-1.0.4/kirkwoodnight/source.py
+drwxr-xr-x   0 armaangoyal   (501) staff       (20)        0 2023-07-17 19:59:03.682587 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     5982 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/PKG-INFO
+-rw-r--r--   0 armaangoyal   (501) staff       (20)      392 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/SOURCES.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)        1 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/dependency_links.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       66 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/entry_points.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       69 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/requires.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       14 2023-07-17 19:59:03.000000 kirkwoodnight-1.0.4/kirkwoodnight.egg-info/top_level.txt
+-rw-r--r--   0 armaangoyal   (501) staff       (20)       38 2023-07-17 19:59:03.684388 kirkwoodnight-1.0.4/setup.cfg
+-rw-r--r--   0 armaangoyal   (501) staff       (20)     1089 2023-07-17 19:53:02.000000 kirkwoodnight-1.0.4/setup.py
```

### Comparing `kirkwoodnight-1.0.3/LICENSE.txt` & `kirkwoodnight-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.3/PKG-INFO` & `kirkwoodnight-1.0.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.3
+Version: 1.0.4
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![PyPI version](https://badge.fury.io/py/kirkwoodnight.svg)](https://badge.fury.io/py/kirkwoodnight)
 [![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
```

### Comparing `kirkwoodnight-1.0.3/README.md` & `kirkwoodnight-1.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![PyPI version](https://badge.fury.io/py/kirkwoodnight.svg)](https://badge.fury.io/py/kirkwoodnight)
 [![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
```

### Comparing `kirkwoodnight-1.0.3/kirkwoodnight/command_line.py` & `kirkwoodnight-1.0.4/kirkwoodnight/command_line.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.3/kirkwoodnight/data/obj_list.csv` & `kirkwoodnight-1.0.4/kirkwoodnight/data/obj_list.csv`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.3/kirkwoodnight/plotting.py` & `kirkwoodnight-1.0.4/kirkwoodnight/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,9 +134,9 @@
 
         # Change the color of the outer circle to white
         for spine in ax.spines.values():
             spine.set_edgecolor('white')
             
         ax.legend(loc='upper center', bbox_to_anchor=(0.5, -0.05), ncol=5, facecolor='white', edgecolor='white', fontsize=12)
         plt.title('Time:'+time,color='k')
-        fig.savefig(files_path+time+'.png',dpi=300,bbox_inches='tight')
+        fig.savefig(files_path+"/"+time+'.png',dpi=300,bbox_inches='tight')
```

### Comparing `kirkwoodnight-1.0.3/kirkwoodnight/source.py` & `kirkwoodnight-1.0.4/kirkwoodnight/source.py`

 * *Files identical despite different names*

### Comparing `kirkwoodnight-1.0.3/kirkwoodnight.egg-info/PKG-INFO` & `kirkwoodnight-1.0.4/kirkwoodnight.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kirkwoodnight
-Version: 1.0.3
+Version: 1.0.4
 Summary: Interactive command line tool to assist with observations at Kirkwood Observatory.
 Home-page: http://packages.python.org/kirkwoodnight
 Author: Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang
 Author-email: armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # kirkwoodnight
 
 [![A rectangular badge, half black half purple containing the text made at Code Astro](https://img.shields.io/badge/Made%20at-Code/Astro-blueviolet.svg)](https://semaphorep.github.io/codeastro/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-![Static Badge](https://img.shields.io/badge/PyPI_Package-1.0.3-green)
+[![PyPI version](https://badge.fury.io/py/kirkwoodnight.svg)](https://badge.fury.io/py/kirkwoodnight)
 [![DOI](https://zenodo.org/badge/665627819.svg)](https://zenodo.org/badge/latestdoi/665627819)
 
 Interactive command line tool to assist with planning and conducting observations at Indiana University's Kirkwood Observatory. Given a desired date, time, and duration of observation, this program allows the user to toggle various observational constraints to generate an observing schedule for over 100 objects of interest, including solar system planets, bright stars, and Messier objects. The user may then select specific objects (or types of objects) they would like to observe during the night, upon which the program will generate a file for each object containing characteristic information (constellation, magnitude, type of object, etc.) as well as an observing schedule with sky positions (Alt, Az) tabulated at various time intervals. The user also has the option of generating star charts for these selected objects at each interval of the observing schedule.
 
 ### Prerequisites
 [Python 3](https://www.python.org/downloads/) or greater.
```

### Comparing `kirkwoodnight-1.0.3/setup.py` & `kirkwoodnight-1.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     reqs = []
     for line in open("requirements.txt", "r").readlines():
         reqs.append(line)
     return reqs
 
 setup(
     name="kirkwoodnight",
-    version="1.0.3",
+    version="1.0.4",
     packages=find_packages(),
 
     # Metadata
     author="Armaan Goyal, Brandon Radzom, Jessica Ranshaw, Xian-Yu Wang",
     author_email="armgoyal@iu.edu, bradzom@iu.edu, jranshaw@iu.edu, xwa5@iu.edu",
     description="Interactive command line tool to assist with observations at Kirkwood Observatory.",
     long_description=open('README.md').read(),
```

