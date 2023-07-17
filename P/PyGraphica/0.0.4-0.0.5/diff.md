# Comparing `tmp/PyGraphica-0.0.4.tar.gz` & `tmp/PyGraphica-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGraphica-0.0.4.tar", last modified: Mon Jun 19 09:44:28 2023, max compression
+gzip compressed data, was "PyGraphica-0.0.5.tar", last modified: Mon Jul 17 00:13:51 2023, max compression
```

## Comparing `PyGraphica-0.0.4.tar` & `PyGraphica-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/
--rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0      287 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    13331 2023-06-18 21:47:30.000000 PyGraphica-0.0.4/README.txt
--rw-rw-rw-   0        0        0      116 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      445 2023-06-19 09:42:20.000000 PyGraphica-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:44:27.974277 PyGraphica-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-19 09:44:27.994686 PyGraphica-0.0.4/src/PyGraphica/
--rw-rw-rw-   0        0        0        0 2023-06-18 02:45:11.000000 PyGraphica-0.0.4/src/PyGraphica/__init__.py
--rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.4/src/PyGraphica/colours.py
--rw-rw-rw-   0        0        0    28435 2023-06-19 09:42:08.000000 PyGraphica-0.0.4/src/PyGraphica/draw.py
--rw-rw-rw-   0        0        0      873 2023-06-19 09:19:35.000000 PyGraphica-0.0.4/src/PyGraphica/fonts.py
--rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.4/src/PyGraphica/origins.py
-drwxrwxrwx   0        0        0        0 2023-06-19 09:44:28.022899 PyGraphica-0.0.4/src/PyGraphica.egg-info/
--rw-rw-rw-   0        0        0      287 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-19 09:44:27.000000 PyGraphica-0.0.4/src/PyGraphica.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 00:13:51.656776 PyGraphica-0.0.5/
+-rw-rw-rw-   0        0        0     1078 2023-06-18 02:58:08.000000 PyGraphica-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      287 2023-07-17 00:13:51.656776 PyGraphica-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    13331 2023-07-17 00:07:25.000000 PyGraphica-0.0.5/README.md
+-rw-rw-rw-   0        0        0      115 2023-07-17 00:13:51.656776 PyGraphica-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-07-17 00:13:34.000000 PyGraphica-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:13:51.590026 PyGraphica-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-07-17 00:13:51.629768 PyGraphica-0.0.5/src/PyGraphica/
+-rw-rw-rw-   0        0        0       49 2023-07-17 00:13:32.000000 PyGraphica-0.0.5/src/PyGraphica/__init__.py
+-rw-rw-rw-   0        0        0   915212 2023-06-18 01:37:01.000000 PyGraphica-0.0.5/src/PyGraphica/arial.ttf
+-rw-rw-rw-   0        0        0    48086 2023-06-18 01:41:16.000000 PyGraphica-0.0.5/src/PyGraphica/baskerville.ttf
+-rw-rw-rw-   0        0        0    57552 2023-07-16 23:54:03.000000 PyGraphica-0.0.5/src/PyGraphica/brushscript.ttf
+-rw-rw-rw-   0        0        0   811412 2023-06-18 01:37:29.000000 PyGraphica-0.0.5/src/PyGraphica/calibri.ttf
+-rw-rw-rw-   0        0        0      708 2023-04-05 22:35:46.000000 PyGraphica-0.0.5/src/PyGraphica/colours.py
+-rw-rw-rw-   0        0        0   709600 2023-06-18 02:16:24.000000 PyGraphica-0.0.5/src/PyGraphica/courier.ttf
+-rw-rw-rw-   0        0        0    28490 2023-07-17 00:03:06.000000 PyGraphica-0.0.5/src/PyGraphica/draw.py
+-rw-rw-rw-   0        0        0     1097 2023-07-17 00:01:26.000000 PyGraphica-0.0.5/src/PyGraphica/fonts.py
+-rw-rw-rw-   0        0        0   196588 2023-06-18 01:41:35.000000 PyGraphica-0.0.5/src/PyGraphica/garamond.ttf
+-rw-rw-rw-   0        0        0   317968 2023-06-18 01:41:02.000000 PyGraphica-0.0.5/src/PyGraphica/helvetica.ttf
+-rw-rw-rw-   0        0        0   136076 2023-06-18 01:40:58.000000 PyGraphica-0.0.5/src/PyGraphica/impact.ttf
+-rw-rw-rw-   0        0        0   237868 2023-07-16 23:55:24.000000 PyGraphica-0.0.5/src/PyGraphica/opendyslexic.ttf
+-rw-rw-rw-   0        0        0       74 2023-04-05 22:24:48.000000 PyGraphica-0.0.5/src/PyGraphica/origins.py
+-rw-rw-rw-   0        0        0   347988 2023-06-18 01:38:19.000000 PyGraphica-0.0.5/src/PyGraphica/timesnewroman.ttf
+-rw-rw-rw-   0        0        0   136172 2023-06-18 02:16:15.000000 PyGraphica-0.0.5/src/PyGraphica/trebuchet.ttf
+drwxrwxrwx   0        0        0        0 2023-07-17 00:13:51.656776 PyGraphica-0.0.5/src/PyGraphica.egg-info/
+-rw-rw-rw-   0        0        0      287 2023-07-17 00:13:51.000000 PyGraphica-0.0.5/src/PyGraphica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      673 2023-07-17 00:13:51.000000 PyGraphica-0.0.5/src/PyGraphica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:13:51.000000 PyGraphica-0.0.5/src/PyGraphica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-07-17 00:13:51.000000 PyGraphica-0.0.5/src/PyGraphica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-17 00:13:51.000000 PyGraphica-0.0.5/src/PyGraphica.egg-info/top_level.txt
```

### Comparing `PyGraphica-0.0.4/LICENSE.txt` & `PyGraphica-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.4/README.txt` & `PyGraphica-0.0.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-PyGraphica 1.0.1
+PyGraphica 0.0.5
 
 By Luke Campbell
 
 PyGraphica is a simple GUI and game development module designed for Python, built of the Python bindings (pysdl2) for SDL-2.
 
 One important note before we start. For all coordinates and lengths, if represented as an integer will be interpreted as a measurement in pixels, and if represented as a string (e.g. '35') will be interpreted as a  percentage of the height or width.
```

### Comparing `PyGraphica-0.0.4/src/PyGraphica/colours.py` & `PyGraphica-0.0.5/src/PyGraphica/colours.py`

 * *Files identical despite different names*

### Comparing `PyGraphica-0.0.4/src/PyGraphica/draw.py` & `PyGraphica-0.0.5/src/PyGraphica/draw.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 
 import sdl2
 import sdl2.ext
 import time
 import ctypes
 import os
+import fonts
+import origins
 from PIL import Image
 
 class window:
     #Restart the window, used when the window is started or resized (as resize requires restart)
     def start(self):
         sdl2.ext.init()
         if self.resizable:
@@ -38,15 +40,15 @@
                 self.__window.window,
                 sdl2.ext.image.load_img(self.icon)
             )
         self.surface = self.__window.get_surface()
         self.__window.show()
     
     #Initialise window class
-    def __init__(self, name="PyGraphica", size=(800,600), resizable=False, icon=False, position=(0,20), origin=0, colour=(0,0,0)):
+    def __init__(self, name="PyGraphica", size=(800,600), resizable=False, icon=False, position=(0,20), origin=origins.TOP_LEFT, colour=(0,0,0)):
         self.name = name
         self.width = size[0]
         self.height = size[1]
         self.resizable = resizable
         self.icon = icon
         self.position = position
         self.origin = origin
@@ -204,15 +206,15 @@
         if not self.__window.mouse_held and self.__window.mouse_down:
             if self.hover and not self.clicked:
                 self.clicked = True
             else:
                 self.clicked = False
 
 class text:
-    def __init__(self, window, x1, y1, size, colour, content, font = "my_fonts/calibri.ttf"):
+    def __init__(self, window, x1, y1, size, colour, content, font = fonts.Calibri):
         self.__window = window
         self.x1 = x1
         self.y1 = y1
         self.size = size
         self.colour = colour
         self.content = content
         self.visible = True
@@ -285,15 +287,15 @@
         rect = (start[0],start[1],start[0]+textbox.w,start[1]+textbox.h)
         self.width = textbox.w
         self.height = textbox.h
         sdl2.SDL_BlitSurface(textbox,None,self.__window.surface,sdl2.SDL_Rect(rect[0],rect[1],rect[2],rect[3]))
 
 #Text input field, where users can type things and programmers can easily extract them
 class textbox:
-    def __init__(self,window,x1,y1,size,width=1,default_text="Type here..."):
+    def __init__(self,window,x1,y1,size,width=1,font=fonts.Calibri,default_text="Type here..."):
         self.__window = window
         self.x1 = x1
         self.y1 = y1
         self.size = size
         self.width = width
         self.content = ""
         self.visible = True
```

