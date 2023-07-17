# Comparing `tmp/PyGraphica-0.0.8.tar.gz` & `tmp/PyGraphica-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.8.tar", last modified: Mon Jul 17 01:05:08 2023, max compression
+gzip compressed data, was "PyGraphica-0.1.0.tar", last modified: Mon Jul 17 01:52:51 2023, max compression
```

## Comparing `PyGraphica-0.0.8.tar` & `PyGraphica-0.1.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.8/LICENSE.txt
--rw-rw-rw-   0        0        0    11861 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    11436 2023-07-17 00:42:31.000000 PyGraphica-0.0.8/README.md
--rw-rw-rw-   0        0        0       85 2023-07-17 01:05:08.030586 PyGraphica-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      762 2023-07-17 01:04:49.000000 PyGraphica-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 01:05:07.947004 PyGraphica-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 01:05:07.983317 PyGraphica-0.0.8/src/PyGraphica/
--rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.0.8/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.0.8/src/PyGraphica/arial.ttf
--rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.0.8/src/PyGraphica/baskerville.ttf
--rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.0.8/src/PyGraphica/brushscript.ttf
--rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.0.8/src/PyGraphica/calibri.ttf
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.8/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.0.8/src/PyGraphica/courier.ttf
--rw-rw-rw-   0        0        0    28497 2023-07-17 01:02:19.000000 PyGraphica-0.0.8/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.0.8/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.0.8/src/PyGraphica/garamond.ttf
--rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.0.8/src/PyGraphica/helvetica.ttf
--rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.0.8/src/PyGraphica/impact.ttf
--rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.0.8/src/PyGraphica/opendyslexic.ttf
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.8/src/PyGraphica/origins.py
--rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.0.8/src/PyGraphica/timesnewroman.ttf
--rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.0.8/src/PyGraphica/trebuchet.ttf
-drwxrwxrwx   0        0        0        0 2023-07-17 01:05:08.014955 PyGraphica-0.0.8/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0    11861 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      673 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-17 01:05:07.000000 PyGraphica-0.0.8/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.1.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    11861 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11436 2023-07-17 01:52:18.000000 PyGraphica-0.1.0/README.md
+-rw-rw-rw-   0        0        0       85 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      762 2023-07-17 01:52:07.000000 PyGraphica-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.179421 PyGraphica-0.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.232448 PyGraphica-0.1.0/src/PyGraphica/
+-rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.1.0/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.1.0/src/PyGraphica/arial.ttf
+-rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.1.0/src/PyGraphica/baskerville.ttf
+-rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.1.0/src/PyGraphica/brushscript.ttf
+-rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.1.0/src/PyGraphica/calibri.ttf
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.1.0/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.1.0/src/PyGraphica/courier.ttf
+-rw-rw-rw-   0        0        0    30674 2023-07-17 01:49:47.000000 PyGraphica-0.1.0/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.1.0/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.1.0/src/PyGraphica/garamond.ttf
+-rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.1.0/src/PyGraphica/helvetica.ttf
+-rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.1.0/src/PyGraphica/impact.ttf
+-rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.1.0/src/PyGraphica/opendyslexic.ttf
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.1.0/src/PyGraphica/origins.py
+-rw-rw-rw-   0        0        0      136 2023-07-17 01:51:22.000000 PyGraphica-0.1.0/src/PyGraphica/test.py
+-rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.1.0/src/PyGraphica/timesnewroman.ttf
+-rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.1.0/src/PyGraphica/trebuchet.ttf
+drwxrwxrwx   0        0        0        0 2023-07-17 01:52:51.265612 PyGraphica-0.1.0/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0    11861 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      696 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 01:52:51.000000 PyGraphica-0.1.0/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.8/LICENSE.txt` & `PyGraphica-0.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/PKG-INFO` & `PyGraphica-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.0.8
+Version: 0.1.0
 Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## **PyGraphica** *0.0.7*
+## **PyGraphica** *0.1.0*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.0.8/README.md` & `PyGraphica-0.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-## **PyGraphica** *0.0.7*
+## **PyGraphica** *0.1.0*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.0.8/src/PyGraphica/arial.ttf` & `PyGraphica-0.1.0/src/PyGraphica/arial.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/baskerville.ttf` & `PyGraphica-0.1.0/src/PyGraphica/baskerville.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/brushscript.ttf` & `PyGraphica-0.1.0/src/PyGraphica/brushscript.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/calibri.ttf` & `PyGraphica-0.1.0/src/PyGraphica/calibri.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/colours.py` & `PyGraphica-0.1.0/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/courier.ttf` & `PyGraphica-0.1.0/src/PyGraphica/courier.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/draw.py` & `PyGraphica-0.1.0/src/PyGraphica/draw.py`

 * *Files 6% similar despite different names*

```diff
@@ -235,22 +235,50 @@
 
         #Make area where text will go
         rect = (start[0],start[1],start[0]+textbox.w,start[1]+textbox.h)
         self.width = textbox.w
         self.height = textbox.h
 
         #Make function to get the endpoint of the text based on the position of the origin and the size of the text, important for making textboxes later on
-        if self.__window.origin == 0:
-            self.__get_end = lambda obj:(obj.x1+obj.width,obj.y1+obj.height)
-        elif self.__window.origin == 1:
-            self.__get_end = lambda obj:(obj.x1-obj.width,obj.y1+obj.height)
-        elif self.__window.origin in [2,4]:
-            self.__get_end = lambda obj:(obj.x1+obj.width,obj.y1-obj.height)
-        elif self.__window.origin == 3:
-            self.__get_end = lambda obj:(obj.x1-obj.width,obj.y1-obj.height)
+        if type(self.x1) == int and type(self.y1) == int and type(self.height) == int:
+            if self.__window.origin == 0:
+                self.__get_end = lambda obj:(obj.x1+obj.width,obj.y1+obj.height)
+            elif self.__window.origin == 1:
+                self.__get_end = lambda obj:(obj.x1-obj.width,obj.y1+obj.height)
+            elif self.__window.origin in [2,4]:
+                self.__get_end = lambda obj:(obj.x1+obj.width,obj.y1-obj.height)
+            elif self.__window.origin == 3:
+                self.__get_end = lambda obj:(obj.x1-obj.width,obj.y1-obj.height)
+        elif type(self.x1) == str and type(self.y1) == str:
+            if self.__window.origin == 0:
+                self.__get_end = lambda obj:(str(int(obj.x1)+int(rela_width(obj.__window,obj.width))),str(int(obj.y1)+int(rela_height(obj.__window,obj.height))))
+            elif self.__window.origin == 1:
+                self.__get_end = lambda obj:(str(int(obj.x1)-int(rela_width(obj.__window,obj.width))),str(int(obj.y1)+int(rela_height(obj.__window,obj.height))))
+            elif self.__window.origin in [2,4]:
+                self.__get_end = lambda obj:(str(int(obj.x1)+int(rela_width(obj.__window,obj.width))),str(int(obj.y1)-int(rela_height(obj.__window,obj.height))))
+            elif self.__window.origin == 3:
+                self.__get_end = lambda obj:(str(int(obj.x1)-int(rela_width(obj.__window,obj.width))),str(int(obj.y1)-int(rela_height(obj.__window,obj.height))))
+        else:
+            if self.__window.origin == 0:
+                def func(obj):
+                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    return((x1+make_width(obj.__window,obj.width),y1+make_height(obj.__window,obj.height)))
+            elif self.__window.origin == 1:
+                def func(obj):
+                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    return((x1-make_width(obj.__window,obj.width),y1+make_height(obj.__window,obj.height)))
+            elif self.__window.origin in [2,4]:
+                def func(obj):
+                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    return((x1+make_width(obj.__window,obj.width),y1-make_height(obj.__window,obj.height)))
+            elif self.__window.origin == 3:
+                def func(obj):
+                    x1,y1 = make_pos(obj.x1,obj.y1)
+                    return((x1-make_width(obj.__window,obj.width),y1-make_height(obj.__window,obj.height)))
+            self.__get_end = func
         
         #Use function to define endpoint of text
         end = self.__get_end(self)
         self.x2 = end[0]
         self.y2 = end[1]
     
     def display(self):
@@ -582,18 +610,26 @@
 #Turn static or relative height into static height
 def make_width(window,width):
     if type(width) == str:
         width = int(window.width * (float(width) / 100))
     return(width)
 
 #Turn static or relative width into relative width
-rela_width = lambda window,width:str(int(100*(width/window.width)))
+def rela_width(window,width):
+    if type(width) == str:
+        return(width)
+    else:
+        return(str(int(100*(width/window.width))))
 
 #Turn static of relative height into relative height
-rela_height = lambda window,height:str(int(100*(height/window.height)))
+def rela_height(window,height):
+    if type(height) == str:
+        return(height)
+    else:
+        return(str(int(100*(height/window.height))))
 
 #List of shapes to be displayed
 all_shapes = []
 
 #Loop through all key_status' and add corresponding key to a list (for easier, more python suitable access)
 def keys(caps):
     keys = []
```

### Comparing `PyGraphica-0.0.8/src/PyGraphica/fonts.py` & `PyGraphica-0.1.0/src/PyGraphica/fonts.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/garamond.ttf` & `PyGraphica-0.1.0/src/PyGraphica/garamond.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/helvetica.ttf` & `PyGraphica-0.1.0/src/PyGraphica/helvetica.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/impact.ttf` & `PyGraphica-0.1.0/src/PyGraphica/impact.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/opendyslexic.ttf` & `PyGraphica-0.1.0/src/PyGraphica/opendyslexic.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/timesnewroman.ttf` & `PyGraphica-0.1.0/src/PyGraphica/timesnewroman.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica/trebuchet.ttf` & `PyGraphica-0.1.0/src/PyGraphica/trebuchet.ttf`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.8/src/PyGraphica.egg-info/PKG-INFO` & `PyGraphica-0.1.0/src/PyGraphica.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: PyGraphica
-Version: 0.0.8
+Version: 0.1.0
 Summary: PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 Home-page: https://github.com/LukeCampbell5853/PyGraphica
 Author: Luke Campbell
 Author-email: LukeCampbell5853@gmail.com
 License: MIT
 Keywords: gui
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-## **PyGraphica** *0.0.7*
+## **PyGraphica** *0.1.0*
 *By Luke Campbell*
 
 PyGraphica is an easy-to-learn GUI module designed for Python, built on the Python bindings (pysdl2) for SDL-2.
 
 *One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.*
 
 \
```

### Comparing `PyGraphica-0.0.8/src/PyGraphica.egg-info/SOURCES.txt` & `PyGraphica-0.1.0/src/PyGraphica.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/PyGraphica/draw.py
 src/PyGraphica/fonts.py
 src/PyGraphica/garamond.ttf
 src/PyGraphica/helvetica.ttf
 src/PyGraphica/impact.ttf
 src/PyGraphica/opendyslexic.ttf
 src/PyGraphica/origins.py
+src/PyGraphica/test.py
 src/PyGraphica/timesnewroman.ttf
 src/PyGraphica/trebuchet.ttf
 src/PyGraphica.egg-info/PKG-INFO
 src/PyGraphica.egg-info/SOURCES.txt
 src/PyGraphica.egg-info/dependency_links.txt
 src/PyGraphica.egg-info/requires.txt
 src/PyGraphica.egg-info/top_level.txt
```

