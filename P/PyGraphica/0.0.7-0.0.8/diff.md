# Comparing `tmp/PyGraphica-0.0.7.tar.gz` & `tmp/PyGraphica-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.7.tar", last modified: Mon Jul 17 00:43:10 2023, max compression
+gzip compressed data, was "PyGraphica-0.0.8.tar", last modified: Mon Jul 17 01:05:08 2023, max compression
```

## Comparing `PyGraphica-0.0.7.tar` & `PyGraphica-0.0.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 00:43:10.160792 PyGraphica-0.0.7/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0    11757 2023-07-17 00:43:10.160792 PyGraphica-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    11436 2023-07-17 00:42:31.000000 PyGraphica-0.0.7/README.md
--rw-rw-rw-   0        0        0       85 2023-07-17 00:43:10.160792 PyGraphica-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-07-17 00:42:41.000000 PyGraphica-0.0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 00:43:10.018452 PyGraphica-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 00:43:10.143900 PyGraphica-0.0.7/src/PyGraphica/
--rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.0.7/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.0.7/src/PyGraphica/arial.ttf
--rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.0.7/src/PyGraphica/baskerville.ttf
--rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.0.7/src/PyGraphica/brushscript.ttf
--rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.0.7/src/PyGraphica/calibri.ttf
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.7/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.0.7/src/PyGraphica/courier.ttf
--rw-rw-rw-   0        0        0    28518 2023-07-17 00:42:03.000000 PyGraphica-0.0.7/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.0.7/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.0.7/src/PyGraphica/garamond.ttf
--rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.0.7/src/PyGraphica/helvetica.ttf
--rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.0.7/src/PyGraphica/impact.ttf
--rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.0.7/src/PyGraphica/opendyslexic.ttf
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.7/src/PyGraphica/origins.py
--rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.0.7/src/PyGraphica/timesnewroman.ttf
--rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.0.7/src/PyGraphica/trebuchet.ttf
-drwxrwxrwx   0        0        0        0 2023-07-17 00:43:10.160792 PyGraphica-0.0.7/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0    11757 2023-07-17 00:43:09.000000 PyGraphica-0.0.7/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-07-17 00:43:09.000000 PyGraphica-0.0.7/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 00:43:09.000000 PyGraphica-0.0.7/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-17 00:43:09.000000 PyGraphica-0.0.7/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 00:43:09.000000 PyGraphica-0.0.7/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    11861 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11436 2023-07-17 00:42:31.000000 PyGraphica-0.0.8/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-17 01:05:08.030586 PyGraphica-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-17 01:04:49.000000 PyGraphica-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 01:05:07.947004 PyGraphica-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 01:05:07.983317 PyGraphica-0.0.8/src/PyGraphica/
+-rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.0.8/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.0.8/src/PyGraphica/arial.ttf
+-rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.0.8/src/PyGraphica/baskerville.ttf
+-rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.0.8/src/PyGraphica/brushscript.ttf
+-rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.0.8/src/PyGraphica/calibri.ttf
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.8/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.0.8/src/PyGraphica/courier.ttf
+-rw-rw-rw-   0        0        0    28497 2023-07-17 01:02:19.000000 PyGraphica-0.0.8/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.0.8/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.0.8/src/PyGraphica/garamond.ttf
+-rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.0.8/src/PyGraphica/helvetica.ttf
+-rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.0.8/src/PyGraphica/impact.ttf
+-rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.0.8/src/PyGraphica/opendyslexic.ttf
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.8/src/PyGraphica/origins.py
+-rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.0.8/src/PyGraphica/timesnewroman.ttf
+-rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.0.8/src/PyGraphica/trebuchet.ttf
+drwxrwxrwx   0        0        0        0 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0    11861 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.7/LICENSE.txt` & `PyGraphica-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/PKG-INFO` & `PyGraphica-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
+Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyGraphica-0.0.7/README.md` & `PyGraphica-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/setup.py` & `PyGraphica-0.0.8/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='PyGraphica',
-    version='0.0.7',
+    version='0.0.8',
     license='MIT',
     author="Luke Campbell",
     author_email='LukeCampbell5853@gmail.com',
-    short_description="PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.",
+    description="PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     package_data={'':['*.ttf']},
     url='https://github.com/LukeCampbell5853/PyGraphica',
     keywords='gui',
```

### Comparing `PyGraphica-0.0.7/src/PyGraphica/arial.ttf` & `PyGraphica-0.0.8/src/PyGraphica/arial.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/baskerville.ttf` & `PyGraphica-0.0.8/src/PyGraphica/baskerville.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/brushscript.ttf` & `PyGraphica-0.0.8/src/PyGraphica/brushscript.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/calibri.ttf` & `PyGraphica-0.0.8/src/PyGraphica/calibri.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/colours.py` & `PyGraphica-0.0.8/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/courier.ttf` & `PyGraphica-0.0.8/src/PyGraphica/courier.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/draw.py` & `PyGraphica-0.0.8/src/PyGraphica/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
         self.width = width
         self.content = ""
         self.visible = True
         #Text that will be displayed as a prompt when the textbox is empty
         self.default_text = default_text
 
         #Text object component of textbox
-        self.__text = text(self.__window,self.x1,self.y1,self.size,(0,0,0),"Type here...","PyGraphica/fonts/calibri.ttf")
+        self.__text = text(self.__window,self.x1,self.y1,self.size,(0,0,0),"Type here...",self.font)
         #The textbox will have its own display function, so the text component must be removed from the list of objects to display
         all_shapes.remove(self.__text)
 
         #create function to calculate the width of the textbox to the start of the text
         if self.__window.origin in [1,3]:
             self.__add_width = lambda obj:obj.__text.x1-obj.width
         else:
```

### Comparing `PyGraphica-0.0.7/src/PyGraphica/fonts.py` & `PyGraphica-0.0.8/src/PyGraphica/fonts.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/garamond.ttf` & `PyGraphica-0.0.8/src/PyGraphica/garamond.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/helvetica.ttf` & `PyGraphica-0.0.8/src/PyGraphica/helvetica.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/impact.ttf` & `PyGraphica-0.0.8/src/PyGraphica/impact.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/opendyslexic.ttf` & `PyGraphica-0.0.8/src/PyGraphica/opendyslexic.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/timesnewroman.ttf` & `PyGraphica-0.0.8/src/PyGraphica/timesnewroman.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica/trebuchet.ttf` & `PyGraphica-0.0.8/src/PyGraphica/trebuchet.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.7/src/PyGraphica.egg-info/PKG-INFO` & `PyGraphica-0.0.8/src/PyGraphica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.0.7
-Summary: UNKNOWN
+Version: 0.0.8
+Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `PyGraphica-0.0.7/src/PyGraphica.egg-info/SOURCES.txt` & `PyGraphica-0.0.8/src/PyGraphica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

