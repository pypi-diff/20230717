# Comparing `tmp/pygame_ui_controls-1.0.2-py3-none-any.whl.zip` & `tmp/pygame_ui_controls-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17940 bytes, number of entries: 7
+Zip file size: 17995 bytes, number of entries: 7
 -rw-rw-r--  2.0 unx        0 b- defN 23-Jun-14 20:26 __init__.py
--rw-rw-r--  2.0 unx    23461 b- defN 23-Jul-14 15:29 pygame_ui_controls.py
--rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-14 15:34 pygame_ui_controls-1.0.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx      681 b- defN 23-Jul-14 15:34 pygame_ui_controls-1.0.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-14 15:34 pygame_ui_controls-1.0.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        1 b- defN 23-Jul-14 15:34 pygame_ui_controls-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-14 15:34 pygame_ui_controls-1.0.2.dist-info/RECORD
-7 files, 59968 bytes uncompressed, 16894 bytes compressed:  71.8%
+-rw-rw-r--  2.0 unx    24038 b- defN 23-Jul-17 18:58 pygame_ui_controls.py
+-rw-rw-r--  2.0 unx    35149 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      681 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      584 b- defN 23-Jul-17 19:03 pygame_ui_controls-1.0.3.dist-info/RECORD
+7 files, 60545 bytes uncompressed, 16949 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: __init__.py
 Comment: 
 
 Filename: pygame_ui_controls.py
 Comment: 
 
-Filename: pygame_ui_controls-1.0.2.dist-info/LICENSE
+Filename: pygame_ui_controls-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: pygame_ui_controls-1.0.2.dist-info/METADATA
+Filename: pygame_ui_controls-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: pygame_ui_controls-1.0.2.dist-info/WHEEL
+Filename: pygame_ui_controls-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: pygame_ui_controls-1.0.2.dist-info/top_level.txt
+Filename: pygame_ui_controls-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: pygame_ui_controls-1.0.2.dist-info/RECORD
+Filename: pygame_ui_controls-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pygame_ui_controls.py

```diff
@@ -218,14 +218,17 @@
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
     def set_text(name, text):
         UI.dict[Button.__name__][name].text = text
     
+    def set_hoverable(name, hoverable):
+        UI.dict[Button.__name__][name].hoverable = hoverable
+    
     def text_color(self):
         if self.locked:
             return Button.TEXT_COLOR_LOCKED
         return Button.TEXT_COLOR_CLASSIC
 
     def text_pos(self, text):
         x, y = self.pos
@@ -253,18 +256,20 @@
     thickness = 3
     extern_thickness = 2
     intern_thickness = 2
 
     def __init__(self, name, path, pos, size=(50, 50), hoverable=True, locked=False, on_click=None):
         UI.__init__(self, name, pos, size, hoverable, locked, on_click=on_click)
 
-        self.set_image_data(path)
+        self.path = path
         self.appearence = self.appearences()
 
     def appearences(self):
+        self.set_image_data()
+
         outer_rect = (0, 0, self.size[0], self.size[1])
         inner_rect = (ImageButton.thickness, ImageButton.thickness, self.size[0] - 2 * ImageButton.thickness, self.size[1] - 2 * ImageButton.thickness)
 
         locked = pygame.Surface(self.size, pygame.SRCALPHA)
         down = pygame.Surface(self.size, pygame.SRCALPHA)
         hovered = pygame.Surface(self.size, pygame.SRCALPHA)
         classic = pygame.Surface(self.size, pygame.SRCALPHA)
@@ -297,39 +302,44 @@
         locked = locked.convert_alpha()
         down = down.convert_alpha()
         hovered = hovered.convert_alpha()
         classic = classic.convert_alpha()
 
         return {'locked': locked, 'down': down, 'hovered': hovered, 'classic': classic}
 
-    def set_image_data(self, path):
+    def set_image_data(self):
         thickness, intern_thickness, extern_thickness = ImageButton.thickness, ImageButton.intern_thickness, ImageButton.extern_thickness
 
         max_width = self.size[0] - 2 * thickness - 2 * intern_thickness - 2 * extern_thickness
         max_height = self.size[1] - 2 * thickness - 2 * intern_thickness - 2 * extern_thickness
 
-        default_width, default_height = get_image_size(path)
+        default_width, default_height = get_image_size(self.path)
         width, height = 0, 0
 
         if default_width / max_width > default_height / max_height:
             width = max_width
             height = default_height * width / default_width
         else:
             height = max_height
             width = default_width * height / default_height
         
-        self.image = get_image((width, height), path)
+        self.image = get_image((width, height), self.path)
         self.im_pos = (self.size[0] // 2 - width // 2, self.size[1] // 2 - height // 2)
 
         self.mask_size = (self.size[0] - 2 * thickness - 2 * extern_thickness, self.size[1] - 2 * thickness - 2 * extern_thickness)   
         self.mask_rect = (0, 0, *self.mask_size)     
         self.mask_pos = (thickness + extern_thickness, thickness + extern_thickness)
         
     def set_image(name, path):
-        UI.dict[ImageButton.__name__][name].set_image_data(path)
+        self = UI.dict[ImageButton.__name__][name]
+        self.path = path
+        self.appearence = self.appearences()
+    
+    def set_hoverable(name, hoverable):
+        UI.dict[ImageButton.__name__][name].hoverable = hoverable
 
     def on_update(self, surface):
         UI.new_rects.append((*self.pos, *self.size))
 
         if self.locked:
             surface.blit(self.appearence['locked'], self.pos)
         elif self.down:
@@ -485,14 +495,16 @@
 
 
 class CheckBox(UI):
 
     thickness = 3
     border_radius = 4
 
+    COLOR_BUTTON_SIDE = (10, 14, 18)
+
     def __init__(self, name, pos, size=30, checked=False, hoverable=True, locked=False, linked=None, on_check=None, on_uncheck=None, on_action=None):
         UI.__init__(self, name, pos, (size, size), hoverable, locked)
         self.checked = checked
         if on_check:
             self.on_check = on_check
         if on_uncheck:
             self.on_uncheck = on_uncheck
@@ -620,16 +632,24 @@
         self.size = rendered[0].get_size()
         return rendered[0]
 
     def set_text(name, text):
         self = UI.dict[Text.__name__][name]
         self.text = text
         self.appearence = self.appearences()
+    
+    def set_text_color(name, color):
+        self = UI.dict[Text.__name__][name]
+        self.color = color
+        self.appearence = self.appearences()
 
     def on_update(self, surface):
+        rect = (*self.pos, *self.size)
+        UI.new_rects.append(rect)
+        
         x, y = self.pos
 
         if self.centered[0]:
             x -= self.size[0] / 2
         if self.centered[1]:
             y -= self.size[1] / 2
```

## Comparing `pygame_ui_controls-1.0.2.dist-info/LICENSE` & `pygame_ui_controls-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pygame_ui_controls-1.0.2.dist-info/METADATA` & `pygame_ui_controls-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame-ui-controls
-Version: 1.0.2
+Version: 1.0.3
 Summary: Pygame UI controls
 Home-page: https://github.com/ArthurLeFloch/PygameUI
 Author: Arthur Le Floch
 Author-email: alf.github@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `pygame_ui_controls-1.0.2.dist-info/RECORD` & `pygame_ui_controls-1.0.3.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 __init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pygame_ui_controls.py,sha256=9h9n81erDwXbpbZN3hljzpPLD9hZvH7b8ZWzDTBtO7Q,23461
-pygame_ui_controls-1.0.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-pygame_ui_controls-1.0.2.dist-info/METADATA,sha256=_773pDWdntOCwhN2BuEXWnxnbThKRWyjP53bVKphdWY,681
-pygame_ui_controls-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pygame_ui_controls-1.0.2.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pygame_ui_controls-1.0.2.dist-info/RECORD,,
+pygame_ui_controls.py,sha256=81utCbo73P5hwla7C7o2b21ZUhZIwfYZSVV4PnPdPtk,24038
+pygame_ui_controls-1.0.3.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+pygame_ui_controls-1.0.3.dist-info/METADATA,sha256=wRaE3nCkuPfmoknbOXR0Cgw9vjP0ynWOyDhqKfu01Q8,681
+pygame_ui_controls-1.0.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pygame_ui_controls-1.0.3.dist-info/top_level.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pygame_ui_controls-1.0.3.dist-info/RECORD,,
```

