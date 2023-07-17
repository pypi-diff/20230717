# Comparing `tmp/PyGraphica-0.1.0.tar.gz` & `tmp/PyGraphica-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.1.0.tar", last modified: Mon Jul 17 01:52:51 2023, max compression
+gzip compressed data, was "PyGraphica-0.1.1.tar", last modified: Mon Jul 17 02:47:28 2023, max compression
```

## Comparing `PyGraphica-0.1.0.tar` & `PyGraphica-0.1.1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0    11861 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    11436 2023-07-17 01:52:18.000000 PyGraphica-0.1.0/README.md
--rw-rw-rw-   0        0        0       85 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-17 01:52:07.000000 PyGraphica-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.179421 PyGraphica-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.232448 PyGraphica-0.1.0/src/PyGraphica/
--rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.1.0/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.1.0/src/PyGraphica/arial.ttf
--rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.1.0/src/PyGraphica/baskerville.ttf
--rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.1.0/src/PyGraphica/brushscript.ttf
--rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.1.0/src/PyGraphica/calibri.ttf
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.1.0/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.1.0/src/PyGraphica/courier.ttf
--rw-rw-rw-   0        0        0    30674 2023-07-17 01:49:47.000000 PyGraphica-0.1.0/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.1.0/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.1.0/src/PyGraphica/garamond.ttf
--rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.1.0/src/PyGraphica/helvetica.ttf
--rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.1.0/src/PyGraphica/impact.ttf
--rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.1.0/src/PyGraphica/opendyslexic.ttf
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.1.0/src/PyGraphica/origins.py
--rw-rw-rw-   0        0        0      136 2023-07-17 01:51:22.000000 PyGraphica-0.1.0/src/PyGraphica/test.py
--rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.1.0/src/PyGraphica/timesnewroman.ttf
--rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.1.0/src/PyGraphica/trebuchet.ttf
-drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0    11861 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      696 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 02:47:28.099392 PyGraphica-0.1.1/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    11861 2023-07-17 02:47:28.099392 PyGraphica-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    11436 2023-07-17 02:45:41.000000 PyGraphica-0.1.1/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-17 02:47:28.099392 PyGraphica-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-17 02:45:39.000000 PyGraphica-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 02:47:28.025038 PyGraphica-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 02:47:28.066511 PyGraphica-0.1.1/src/PyGraphica/
+-rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.1.1/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.1.1/src/PyGraphica/arial.ttf
+-rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.1.1/src/PyGraphica/baskerville.ttf
+-rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.1.1/src/PyGraphica/brushscript.ttf
+-rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.1.1/src/PyGraphica/calibri.ttf
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.1.1/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.1.1/src/PyGraphica/courier.ttf
+-rw-rw-rw-   0        0        0    31204 2023-07-17 02:42:13.000000 PyGraphica-0.1.1/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.1.1/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.1.1/src/PyGraphica/garamond.ttf
+-rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.1.1/src/PyGraphica/helvetica.ttf
+-rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.1.1/src/PyGraphica/impact.ttf
+-rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.1.1/src/PyGraphica/opendyslexic.ttf
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.1.1/src/PyGraphica/origins.py
+-rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.1.1/src/PyGraphica/timesnewroman.ttf
+-rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.1.1/src/PyGraphica/trebuchet.ttf
+drwxrwxrwx   0        0        0        0 2023-07-17 02:47:28.099392 PyGraphica-0.1.1/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0    11861 2023-07-17 02:47:27.000000 PyGraphica-0.1.1/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-07-17 02:47:27.000000 PyGraphica-0.1.1/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 02:47:27.000000 PyGraphica-0.1.1/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-17 02:47:27.000000 PyGraphica-0.1.1/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 02:47:27.000000 PyGraphica-0.1.1/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.1.0/LICENSE.txt` & `PyGraphica-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/PKG-INFO` & `PyGraphica-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## **PyGraphica** *0.1.0*
+## **PyGraphica** *0.1.1*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.1.0/README.md` & `PyGraphica-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## **PyGraphica** *0.1.0*
+## **PyGraphica** *0.1.1*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.1.0/setup.py` & `PyGraphica-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 setup(
     name='PyGraphica',
-    version='0.1.0',
+    version='0.1.1',
     license='MIT',
     author="Luke Campbell",
     author_email='LukeCampbell5853@gmail.com',
     description="PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type='text/markdown',
     packages=find_packages('src'),
```

### Comparing `PyGraphica-0.1.0/src/PyGraphica/arial.ttf` & `PyGraphica-0.1.1/src/PyGraphica/arial.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/baskerville.ttf` & `PyGraphica-0.1.1/src/PyGraphica/baskerville.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/brushscript.ttf` & `PyGraphica-0.1.1/src/PyGraphica/brushscript.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/calibri.ttf` & `PyGraphica-0.1.1/src/PyGraphica/calibri.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/colours.py` & `PyGraphica-0.1.1/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/courier.ttf` & `PyGraphica-0.1.1/src/PyGraphica/courier.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/draw.py` & `PyGraphica-0.1.1/src/PyGraphica/draw.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,27 +256,27 @@
             elif self.__window.origin in [2,4]:
                 self.__get_end = lambda obj:(str(int(obj.x1)+int(rela_width(obj.__window,obj.width))),str(int(obj.y1)-int(rela_height(obj.__window,obj.height))))
             elif self.__window.origin == 3:
                 self.__get_end = lambda obj:(str(int(obj.x1)-int(rela_width(obj.__window,obj.width))),str(int(obj.y1)-int(rela_height(obj.__window,obj.height))))
         else:
             if self.__window.origin == 0:
                 def func(obj):
-                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    x1,y1 = make_pos(obj.__window,(obj.x1,obj.y1))
                     return((x1+make_width(obj.__window,obj.width),y1+make_height(obj.__window,obj.height)))
             elif self.__window.origin == 1:
                 def func(obj):
-                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    x1,y1 = make_pos(obj.__window,(obj.x1,obj.y1))
                     return((x1-make_width(obj.__window,obj.width),y1+make_height(obj.__window,obj.height)))
             elif self.__window.origin in [2,4]:
                 def func(obj):
-                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    x1,y1 = make_pos(obj.__window,(obj.x1,obj.y1))
                     return((x1+make_width(obj.__window,obj.width),y1-make_height(obj.__window,obj.height)))
             elif self.__window.origin == 3:
                 def func(obj):
-                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    x1,y1 = make_pos(obj.__window,(obj.x1,obj.y1))
                     return((x1-make_width(obj.__window,obj.width),y1-make_height(obj.__window,obj.height)))
             self.__get_end = func
         
         #Use function to define endpoint of text
         end = self.__get_end(self)
         self.x2 = end[0]
         self.y2 = end[1]
@@ -332,18 +332,24 @@
 
         #Text object component of textbox
         self.__text = text(self.__window,self.x1,self.y1,self.size,(0,0,0),"Type here...",self.font)
         #The textbox will have its own display function, so the text component must be removed from the list of objects to display
         all_shapes.remove(self.__text)
 
         #create function to calculate the width of the textbox to the start of the text
-        if self.__window.origin in [1,3]:
-            self.__add_width = lambda obj:obj.__text.x1-obj.width
+        if type(self.__text.x1) == str:
+            if self.__window.origin in [1,3]:
+                self.__add_width = lambda obj:(str(int(obj.__text.x1)-int(rela_width(obj.__window,obj.width))))
+            else:
+                self.__add_width = lambda obj:(str(int(obj.__text.x1)+int(rela_width(obj.__window,obj.width))))
         else:
-            self.__add_width = lambda obj:obj.__text.x1+obj.width
+            if self.__window.origin in [1,3]:
+                self.__add_width = lambda obj:(obj.__text.x1-make_width(obj.__window,obj.width))
+            else:
+                self.__add_width = lambda obj:(obj.__text.x1+make_width(obj.__window,obj.width))
 
         self.x2 = self.__text.x2
         self.y2 = self.__text.y2
 
         #Create box component of the textbox
         self.__box = rect(self.__window,self.x1,self.y1,self.x2,self.y2,(255,255,255),((0,0,0),1))
         all_shapes.remove(self.__box)
@@ -354,15 +360,15 @@
         #Redefine position of textbox
         self.__text.x1 = self.x1
         self.__text.y1 = self.y1
         self.__box.x1 = self.x1
         self.__box.y1 = self.y1
 
         #If the text typed in to the textbox is larger than the defaul width of the textbox, stretch to fit it, otherwise use default width
-        if self.width > self.__text.width:
+        if make_width(self.__window,self.width) > make_width(self.__window,self.__text.width):
             self.__box.x2 = self.__add_width(self)
             self.__box.y2 = self.__text.y2
         else:
             self.__box.x2 = self.__text.x2
             self.__box.y2 = self.__text.y2
 
         #Extra animations for if box is clicked
```

### Comparing `PyGraphica-0.1.0/src/PyGraphica/fonts.py` & `PyGraphica-0.1.1/src/PyGraphica/fonts.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/garamond.ttf` & `PyGraphica-0.1.1/src/PyGraphica/garamond.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/helvetica.ttf` & `PyGraphica-0.1.1/src/PyGraphica/helvetica.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/impact.ttf` & `PyGraphica-0.1.1/src/PyGraphica/impact.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/opendyslexic.ttf` & `PyGraphica-0.1.1/src/PyGraphica/opendyslexic.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/timesnewroman.ttf` & `PyGraphica-0.1.1/src/PyGraphica/timesnewroman.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica/trebuchet.ttf` & `PyGraphica-0.1.1/src/PyGraphica/trebuchet.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.1.0/src/PyGraphica.egg-info/PKG-INFO` & `PyGraphica-0.1.1/src/PyGraphica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.1.0
+Version: 0.1.1
 Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## **PyGraphica** *0.1.0*
+## **PyGraphica** *0.1.1*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.1.0/src/PyGraphica.egg-info/SOURCES.txt` & `PyGraphica-0.1.1/src/PyGraphica.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 src/PyGraphica/draw.py
 src/PyGraphica/fonts.py
 src/PyGraphica/garamond.ttf
 src/PyGraphica/helvetica.ttf
 src/PyGraphica/impact.ttf
 src/PyGraphica/opendyslexic.ttf
 src/PyGraphica/origins.py
-src/PyGraphica/test.py
 src/PyGraphica/timesnewroman.ttf
 src/PyGraphica/trebuchet.ttf
 src/PyGraphica.egg-info/PKG-INFO
 src/PyGraphica.egg-info/SOURCES.txt
 src/PyGraphica.egg-info/dependency_links.txt
 src/PyGraphica.egg-info/requires.txt
 src/PyGraphica.egg-info/top_level.txt
```

