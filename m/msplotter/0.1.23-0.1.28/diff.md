# Comparing `tmp/msplotter-0.1.23.tar.gz` & `tmp/msplotter-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msplotter-0.1.23.tar", last modified: Sat Jul  8 02:41:38 2023, max compression
+gzip compressed data, was "msplotter-0.1.28.tar", last modified: Mon Jul 17 03:36:54 2023, max compression
```

## Comparing `msplotter-0.1.23.tar` & `msplotter-0.1.28.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.431542 msplotter-0.1.23/
--rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.23/LICENSE
--rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-08 02:41:38.430505 msplotter-0.1.23/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)     4544 2023-06-08 15:44:32.000000 msplotter-0.1.23/README.md
--rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-06 15:23:32.000000 msplotter-0.1.23/pyproject.toml
--rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-08 02:41:38.431685 msplotter-0.1.23/setup.cfg
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.400503 msplotter-0.1.23/src/
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.411350 msplotter-0.1.23/src/msp/
--rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.23/src/msp/__init__.py
--rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.23/src/msp/__main__.py
--rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.23/src/msp/arrows.py
--rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.23/src/msp/colormap_picker.py
--rw-r--r--   0 msp        (501) staff       (20)    12930 2023-07-08 00:07:06.000000 msplotter-0.1.23/src/msp/gui.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.426090 msplotter-0.1.23/src/msp/images/
--rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.23/src/msp/images/Blues.png
--rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/BuGn.png
--rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/BuPu.png
--rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/GnBu.png
--rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Greens.png
--rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Greys.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/OrRd.png
--rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Oranges.png
--rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuBu.png
--rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuBuGn.png
--rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/PuRd.png
--rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Purples.png
--rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/RdPu.png
--rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/Reds.png
--rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlGn.png
--rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlGnBu.png
--rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlOrBr.png
--rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/YlOrRd.png
--rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.23/src/msp/images/logo.png
--rw-r--r--   0 msp        (501) staff       (20)    30089 2023-07-07 15:34:46.000000 msplotter-0.1.23/src/msp/msplotter.py
--rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.23/src/msp/plot.py
--rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.23/src/msp/slider_widget.py
--rw-r--r--   0 msp        (501) staff       (20)    14412 2023-07-08 00:53:57.000000 msplotter-0.1.23/src/msp/user_input.py
-drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-08 02:41:38.429759 msplotter-0.1.23/src/msplotter.egg-info/
--rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/PKG-INFO
--rw-r--r--   0 msp        (501) staff       (20)      914 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/SOURCES.txt
--rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/dependency_links.txt
--rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/entry_points.txt
--rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/requires.txt
--rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-08 02:41:38.000000 msplotter-0.1.23/src/msplotter.egg-info/top_level.txt
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-17 03:36:54.206971 msplotter-0.1.28/
+-rw-r--r--   0 msp        (501) staff       (20)     1507 2023-01-12 04:50:28.000000 msplotter-0.1.28/LICENSE
+-rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-17 03:36:54.206422 msplotter-0.1.28/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)     4544 2023-06-08 15:44:32.000000 msplotter-0.1.28/README.md
+-rw-r--r--   0 msp        (501) staff       (20)      961 2023-07-15 20:54:21.000000 msplotter-0.1.28/pyproject.toml
+-rw-r--r--   0 msp        (501) staff       (20)       38 2023-07-17 03:36:54.207098 msplotter-0.1.28/setup.cfg
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-17 03:36:54.171259 msplotter-0.1.28/src/
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-17 03:36:54.183596 msplotter-0.1.28/src/msp/
+-rw-r--r--   0 msp        (501) staff       (20)        0 2023-06-04 02:01:52.000000 msplotter-0.1.28/src/msp/__init__.py
+-rw-r--r--   0 msp        (501) staff       (20)      431 2023-06-06 20:35:01.000000 msplotter-0.1.28/src/msp/__main__.py
+-rw-r--r--   0 msp        (501) staff       (20)     5859 2023-06-04 00:27:56.000000 msplotter-0.1.28/src/msp/arrows.py
+-rw-r--r--   0 msp        (501) staff       (20)     5096 2023-06-04 02:40:56.000000 msplotter-0.1.28/src/msp/colormap_picker.py
+-rw-r--r--   0 msp        (501) staff       (20)    14508 2023-07-16 23:44:54.000000 msplotter-0.1.28/src/msp/gui.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-17 03:36:54.201516 msplotter-0.1.28/src/msp/images/
+-rw-r--r--   0 msp        (501) staff       (20)      560 2023-03-28 02:55:33.000000 msplotter-0.1.28/src/msp/images/Blues.png
+-rw-------   0 msp        (501) staff       (20)      614 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/BuGn.png
+-rw-------   0 msp        (501) staff       (20)      593 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/BuPu.png
+-rw-------   0 msp        (501) staff       (20)      617 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/GnBu.png
+-rw-------   0 msp        (501) staff       (20)      575 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/Greens.png
+-rw-------   0 msp        (501) staff       (20)      453 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/Greys.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/OrRd.png
+-rw-------   0 msp        (501) staff       (20)      569 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/Oranges.png
+-rw-------   0 msp        (501) staff       (20)      591 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/PuBu.png
+-rw-------   0 msp        (501) staff       (20)      609 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/PuBuGn.png
+-rw-------   0 msp        (501) staff       (20)      662 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/PuRd.png
+-rw-------   0 msp        (501) staff       (20)      557 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/Purples.png
+-rw-------   0 msp        (501) staff       (20)      621 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/RdPu.png
+-rw-------   0 msp        (501) staff       (20)      587 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/Reds.png
+-rw-------   0 msp        (501) staff       (20)      618 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/YlGn.png
+-rw-------   0 msp        (501) staff       (20)      624 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/YlGnBu.png
+-rw-------   0 msp        (501) staff       (20)      592 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/YlOrBr.png
+-rw-------   0 msp        (501) staff       (20)      596 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/YlOrRd.png
+-rw-------   0 msp        (501) staff       (20)    25253 2023-03-24 21:28:57.000000 msplotter-0.1.28/src/msp/images/logo.png
+-rw-r--r--   0 msp        (501) staff       (20)    34228 2023-07-16 04:32:07.000000 msplotter-0.1.28/src/msp/msplotter.py
+-rw-r--r--   0 msp        (501) staff       (20)     3507 2023-07-08 00:04:00.000000 msplotter-0.1.28/src/msp/plot.py
+-rw-r--r--   0 msp        (501) staff       (20)     7391 2023-06-04 02:29:49.000000 msplotter-0.1.28/src/msp/slider_widget.py
+-rw-r--r--   0 msp        (501) staff       (20)     2958 2023-07-17 00:23:03.000000 msplotter-0.1.28/src/msp/spinbox.py
+-rw-r--r--   0 msp        (501) staff       (20)    14329 2023-07-15 21:18:20.000000 msplotter-0.1.28/src/msp/user_input.py
+drwxr-xr-x   0 msp        (501) staff       (20)        0 2023-07-17 03:36:54.205686 msplotter-0.1.28/src/msplotter.egg-info/
+-rw-r--r--   0 msp        (501) staff       (20)     5234 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/PKG-INFO
+-rw-r--r--   0 msp        (501) staff       (20)      933 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 msp        (501) staff       (20)        1 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 msp        (501) staff       (20)       48 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/entry_points.txt
+-rw-r--r--   0 msp        (501) staff       (20)       55 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/requires.txt
+-rw-r--r--   0 msp        (501) staff       (20)        4 2023-07-17 03:36:54.000000 msplotter-0.1.28/src/msplotter.egg-info/top_level.txt
```

### Comparing `msplotter-0.1.23/LICENSE` & `msplotter-0.1.28/LICENSE`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/PKG-INFO` & `msplotter-0.1.28/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.23
+Version: 0.1.28
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.23/README.md` & `msplotter-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/pyproject.toml` & `msplotter-0.1.28/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "msplotter"
-version = "0.1.23"
+version = "0.1.28"
 authors = [
     {name = "Ivan Muñoz-Gutierrez", email = "ivan.munoz.gutierrez@gmail.com"},
 ]
 description = "Make a graphical representation of a blastn alignment"
 readme = "README.md"
 requires-python = ">=3.11"
 keywords = [
```

### Comparing `msplotter-0.1.23/src/msp/arrows.py` & `msplotter-0.1.28/src/msp/arrows.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/colormap_picker.py` & `msplotter-0.1.28/src/msp/colormap_picker.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/gui.py` & `msplotter-0.1.28/src/msp/gui.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,55 +6,55 @@
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 from pathlib import Path
 
 from tkinter import filedialog
 import customtkinter
-from matplotlib.backends.backend_tkagg import FigureCanvasTkAgg
 
 import msp.msplotter as msp
 from msp.colormap_picker import ColormapPicker
 from msp.plot import Plot
-
+from msp.spinbox import FloatSpinbox
 
 class App(customtkinter.CTk):
     """msplotter GUI."""
     def __init__(self):
         super().__init__()
-        # Variables for BLASTing and plotting.
-        self.figure_plt = None                        # matplotlib object.
+        # -- Variables for BLASTing and plotting ------------------------------
+        self.figure_plt = None                 # matplotlib object.
         self.gb_files: list = None
-        self.figure_msp = None                     # msplotter object.
+        self.figure_msp = None                 # msplotter object.
         self.identity_color: str = "Greys"
         self.colormap_range: tuple = (0, 0.75)
+        self.y_limit: float = 0                # to adjust position of colormap
+        self.scale_bar: bool = False
         self.annotate_sequences: bool = False
         self.annotate_genes: bool = False
-        # Set layout parameters
-        self.geometry('600x520')
+
+        # -- Set layout parameters --------------------------------------------
+        self.geometry('600x700')
         self.title('MSPlotter')
         self.grid_rowconfigure(1, weight=1)
         self.grid_columnconfigure(1, weight=1)
         # Protocol to close app, including plot if exist.
         self.protocol('WM_DELETE_WINDOW', self.on_closing)
         # Variable to store the ColormapPicker class used in the
         # launch_colormap_picker function.
         self.colormap_app = None
 
-        # ################ #
-        # Navigation frame #
-        # ################ #
+        # -- Navigation frame -------------------------------------------------
         # Create navigation frame.
         self.navigation_frame = customtkinter.CTkFrame(self, corner_radius=0)
         self.navigation_frame.grid(row=0, column=0, columnspan=3, sticky='nsew')
         self.navigation_frame.grid_columnconfigure(0, weight=1)
         # Logo label
         self.logo_label = customtkinter.CTkLabel(
             self.navigation_frame, text='MSPloter',
-            font=customtkinter.CTkFont(size=20, weight='bold')
+            font=customtkinter.CTkFont(size=24, weight='bold')
         )
         self.logo_label.grid(row=0, column=0, padx=(10,5), pady=20)
         # Select button
         self.select_button = customtkinter.CTkButton(
             self.navigation_frame, text='Select',
             command=self.get_files_path
         )
@@ -70,41 +70,34 @@
         self.plot_button = customtkinter.CTkButton(
             self.navigation_frame, text='Plot',
             command=self.plot_figure,
             state='disabled'
         )
         self.plot_button.grid(row=0, column=3, padx=(5,10), pady=20)
 
-        # ################ #
-        # Appearance frame #
-        # ################ #
+        # -- Appearance frame -------------------------------------------------
         self.appearance_frame = customtkinter.CTkFrame(
             self, corner_radius=5,
         )
         self.appearance_frame.grid(
             row=1, column=0, padx=(10, 5), pady=10, sticky='nsew'
         )
-        self.appearance_frame.grid_rowconfigure(9, weight=1)
+        self.appearance_frame.grid_rowconfigure(13, weight=1)
         # Appearance label
-        self.system_appearance_mode = customtkinter.get_appearance_mode()
-        if self.system_appearance_mode == 'Dark':
-            self.appearance_fg_color = '#333333'
-        else:
-            self.appearance_fg_color = 'Gray80'
         self.appearance_label = customtkinter.CTkLabel(
             self.appearance_frame,
             text='Appearance',
-            font=customtkinter.CTkFont(size=16),
+            font=customtkinter.CTkFont(size=18, weight='bold'),
             width=120,
             height=50,
             corner_radius=5,
-            fg_color=self.appearance_fg_color,
+            # fg_color=self.appearance_fg_color,
         )
         self.appearance_label.grid(
-            row=0, column=0, pady=(0,10), sticky='nswe'
+            row=0, column=0, pady=(10,10), sticky='nswe'
         )
         # Homology color label
         self.homology_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Homology color:',
         )
         self.homology_label.grid(row=1, column=0, pady=(10,0))
         # Colormap picker
@@ -136,41 +129,67 @@
         # Variable to store annotate_seq menu selection
         self.annotate_seq_var = customtkinter.StringVar(self, 'No')
         # Annotate sequences menu
         self.annotate_seq_menu = customtkinter.CTkOptionMenu(
             self.appearance_frame,
             values=['No', 'Yes'],
             variable=self.annotate_seq_var,
-            command=lambda _:self.update_annotate_seq_var()
+            command=lambda _:self.update_annotate_seq()
         )
         self.annotate_seq_menu.grid(row=6, column=0, pady=(0,10))
         # Annotate genes label
         self.annotate_genes_label = customtkinter.CTkLabel(
             self.appearance_frame, text='Annotate genes:'
         )
-        self.annotate_genes_label.grid(row=7, column=0, pady=(10, 0))
+        self.annotate_genes_label.grid(row=7, column=0, pady=(10,0))
         # Variable to store annotate_genes menu selection
         self.annotate_genes_var = customtkinter.StringVar(self, 'No')
         # Annotate genes menu
         self.annotate_genes_menu = customtkinter.CTkOptionMenu(
             self.appearance_frame,
             values=['No', 'Yes'],
             variable=self.annotate_genes_var,
-            command=lambda _:self.update_annotate_genes_var()
+            command=lambda _:self.update_annotate_genes()
         )
         self.annotate_genes_menu.grid(row=8, column=0, pady=(0,10))
+        # Scale bar label
+        self.scale_bar_label = customtkinter.CTkLabel(
+            self.appearance_frame, text='Scale bar:'
+        )
+        self.scale_bar_label.grid(row=9, column=0, pady=(10,0))
+        # Variable to store scale_bar menu selection
+        self.scale_bar_var = customtkinter.StringVar(self, 'No')
+        # Scale bar menu
+        self.scale_bar_menu = customtkinter.CTkOptionMenu(
+            self.appearance_frame,
+            values=['No', 'Yes'],
+            variable=self.scale_bar_var,
+            command=lambda _:self.update_scale_bar()
+        )
+        self.scale_bar_menu.grid(row=10, column=0, pady=(0,10))
+        # Color map position label
+        self.cmap_position_label = customtkinter.CTkLabel(
+            self.appearance_frame, text='Position colormap:'
+        )
+        self.cmap_position_label.grid(row=11, column=0, pady=(10, 0))
+        # Color map position spinbox
+        self.cmap_position_spinbox = FloatSpinbox(
+            self.appearance_frame,
+            width=140,
+            height=28,
+            command=self.update_y_limit
+        )
+        self.cmap_position_spinbox.grid(row=12, column=0, pady=(0, 10))
         # Reset button
         self.reset_button = customtkinter.CTkButton(
             self.appearance_frame, text='Reset', command=self.reset_appearance
         )
-        self.reset_button.grid(row=9, column=0, pady=(20, 10))
+        self.reset_button.grid(row=13, column=0, pady=(20, 10))
 
-        # ############# #
-        # Display frame #
-        # ############# #
+        # -- Display frame ---------------------------------------------------
         # Create display frame
         self.display_frame = customtkinter.CTkFrame(
             self, corner_radius=0,
             fg_color='transparent'
         )
         self.display_frame.grid(row=1, column=1, columnspan=2, sticky='nsew')
         self.display_frame.grid_rowconfigure(0, weight=1)
@@ -227,15 +246,14 @@
     def clear_input(self):
         """Clean input data store in self.gb_files."""
         self.gb_files = None
         self.display_window.configure(state='normal')
         self.display_window.delete('1.0', 'end')
         self.display_window.configure(state='disabled')
         self.plot_button.configure(state='disabled')
-        self.save_button.configure(state='disabled')
         self.clear_button.configure(state='disabled')
 
     def launch_colormap_picker(self):
         """Pick colormap and range for homology regions."""
         if self.colormap_app is None or not self.colormap_app.winfo_exists():
             self.colormap_app = ColormapPicker(self.get_colormap_data)
         else:
@@ -253,40 +271,55 @@
             'end',
             f'The homology regions are going to be shown in `{cmap_name}` ' +
             f'with a range of colors between `{round(cmap_range[0])}-'
             f'{round(cmap_range[1])}`.'
         )
         self.display_window.configure(state='disabled')
 
-    def update_annotate_seq_var(self):
+    def update_annotate_seq(self):
         if self.annotate_seq_var.get() == 'No':
             self.annotate_sequences = False
         else:
             self.annotate_sequences = True
 
-    def update_annotate_genes_var(self):
+    def update_annotate_genes(self):
         if self.annotate_genes_var.get() == 'No':
             self.annotate_genes = False
         else:
             self.annotate_genes = True
 
+    def update_scale_bar(self):
+        if self.scale_bar_var.get() == 'No':
+            self.scale_bar = False
+        else:
+            self.scale_bar = True
+
+    def update_y_limit(self):
+        self.y_limit = self.cmap_position_spinbox.get()
+
     def reset_appearance(self):
         """Reset appearance parameters."""
         # Reset color map
         self.identity_color = "Greys"
         self.colormap_range = (0, 0.75)
         # Reset align plot
         self.align_plot_var.set('Left')
         self.align_plot.configure(variable=self.align_plot_var)
         # Reset annotate sequences
         self.annotate_seq_var.set('No')
         self.annotate_seq_menu.configure(variable=self.annotate_seq_var)
-        # Reset Annotate genes
+        # Reset annotate genes
         self.annotate_genes_var.set('No')
         self.annotate_genes_menu.configure(variable=self.annotate_genes_var)
+        # Reset scale bar
+        self.scale_bar_var.set('No')
+        self.scale_bar_menu.configure(variable=self.scale_bar_var)
+        # Reset y_limit
+        self.y_limit = 0
+        self.cmap_position_spinbox.set(0.0)
 
     def plot_figure(self):
         """Plot alignments using msplotter."""
         # Create fasta files for BLASTing.
         faa_files = msp.make_fasta_file(self.gb_files)
         # Run blastn locally.
         xml_results = msp.run_blastn(faa_files)
@@ -303,14 +336,16 @@
             alignments,
             gb_records,
             alignments_position=self.align_plot_var.get().lower(),
             identity_color=self.identity_color,
             color_map_range=self.colormap_range,
             annotate_sequences=self.annotate_sequences,
             annotate_genes=self.annotate_genes,
+            scale_bar=self.scale_bar,
+            y_limit=self.y_limit,
             use_gui=True
         )
         # Plot figure using the Plot class
         self.figure_plt = self.figure_msp.make_figure()
         # Plot figure
         Plot(self.figure_plt, self.figure_msp)
```

### Comparing `msplotter-0.1.23/src/msp/images/Blues.png` & `msplotter-0.1.28/src/msp/images/Blues.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/BuGn.png` & `msplotter-0.1.28/src/msp/images/BuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/BuPu.png` & `msplotter-0.1.28/src/msp/images/BuPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/GnBu.png` & `msplotter-0.1.28/src/msp/images/GnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/Greens.png` & `msplotter-0.1.28/src/msp/images/Greens.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/OrRd.png` & `msplotter-0.1.28/src/msp/images/OrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/Oranges.png` & `msplotter-0.1.28/src/msp/images/Oranges.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/PuBu.png` & `msplotter-0.1.28/src/msp/images/PuBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/PuBuGn.png` & `msplotter-0.1.28/src/msp/images/PuBuGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/PuRd.png` & `msplotter-0.1.28/src/msp/images/PuRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/Purples.png` & `msplotter-0.1.28/src/msp/images/Purples.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/RdPu.png` & `msplotter-0.1.28/src/msp/images/RdPu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/Reds.png` & `msplotter-0.1.28/src/msp/images/Reds.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/YlGn.png` & `msplotter-0.1.28/src/msp/images/YlGn.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/YlGnBu.png` & `msplotter-0.1.28/src/msp/images/YlGnBu.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/YlOrBr.png` & `msplotter-0.1.28/src/msp/images/YlOrBr.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/YlOrRd.png` & `msplotter-0.1.28/src/msp/images/YlOrRd.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/images/logo.png` & `msplotter-0.1.28/src/msp/images/logo.png`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/msplotter.py` & `msplotter-0.1.28/src/msp/msplotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,21 @@
 BSD 3-Clause License
 Copyright (c) 2023, Ivan Munoz Gutierrez
 """
 import os
 import sys
 
 import matplotlib as mpl
+from matplotlib.axes import Axes
 import matplotlib.colors as colors
+from matplotlib.colors import Colormap
 import matplotlib.patches as mpatches
 import matplotlib.pyplot as plt
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+import matplotlib.ticker as ticker
 import numpy as np
 from Bio import SeqIO
 from Bio.Blast import NCBIXML
 from Bio.Blast.Applications import NcbiblastnCommandline
 from Bio.SeqRecord import SeqRecord
 from pathlib import Path
 
@@ -295,25 +298,30 @@
     annotate_sequences : bool
         Annotate sequences in plot (defalult: False). If True, the `top` and
         `bottom` sequences are annotated.
     sequence_name : str
         String to access either `name` or `accession` from GenBankRecord class
         (default: `accession`). Either `name` or `accession` is used to
         annotate the sequence if `add_annotations_sequences` attribute is True.
-    y_separation : int
+    y_separation : float
         Distance between sequences in the y-axis (default: 10).
+    y_limit : float
+        Lower limit to show in the plot (default: 5). Use this value to adjust
+        the position of the color map and the scale bar.
     sequence_color : str
         Color used for lines representing sequences (default: `black`). You can
         use any color name allowed by `Matplotlib`.
     sequence_width : int
         Width of lines representing sequences (default: 3).
     identity_color : str
         Color used to represent regions of homology (default: `Greys`). This
         color represent a `Matplotlib` colormap. Therefore, you should provide
         a valid colormap name.
+    scale_bar : bool
+        Show scale bar (default: True).
     color_map_range : tupple
         Tyupple with a min and max value between 0 and 1. The min and max
         values are used in color_map to determine the range of the color_map
         to use (default: (0, 0.75)).
     color_map : matplotlib colormaps object
         Color map to represent homology regions.
     homology_padding : float
@@ -331,31 +339,33 @@
     user_gui : bool
         Run app in a graphical user interface (default: False).
     """
     def __init__(
         self, alignments, gb_records, alignments_position="left",
         annotate_genes=False, annotate_genes_on_sequence=("top", "bottom"),
         annotate_sequences=False, sequence_name="accession", y_separation=10,
-        sequence_color="black", sequence_width=3, identity_color="Greys",
-        color_map_range=(0, 0.75), homology_padding=0.1,
-        figure_name=(Path.cwd() / 'figure.png'),
+        y_limit=5, sequence_color="black", sequence_width=3,
+        identity_color="Greys", scale_bar=True, color_map_range=(0, 0.75),
+        homology_padding=0.1, figure_name=(Path.cwd() / 'figure.png'),
         figure_format='png', dpi=300.0, use_gui=False
     ):
         self.alignments = alignments
         self.num_alignments = len(alignments)
         self.gb_records = gb_records
         self.alignments_position = alignments_position
         self.annotate_genes = annotate_genes
         self.annotate_genes_on_sequence = annotate_genes_on_sequence
         self.annotate_sequences = annotate_sequences
         self.sequence_name = sequence_name
         self.y_separation = y_separation
+        self.y_limit = y_limit
         self.sequence_color = sequence_color
         self.sequence_width = sequence_width
         self.identity_color = identity_color
+        self.scale_bar = scale_bar
         self.color_map_range = color_map_range
         self.color_map = self.make_colormap(
             identity_color=identity_color,
             min_val=self.color_map_range[0],
             max_val=self.color_map_range[1],
             n=100
         )
@@ -431,21 +441,16 @@
             shift_h = (self.size_longest_sequence - alignment.hit_len) / 2
             for region in alignment.regions:
                 region.query_from = region.query_from + shift_q
                 region.query_to = region.query_to + shift_q
                 region.hit_from = region.hit_from + shift_h
                 region.hit_to = region.hit_to + shift_h
 
-    def plot_dna_sequences(self, ax) -> None:
-        """Plot lines that represent DNA sequences.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def plot_dna_sequences(self, ax: Axes) -> None:
+        """Plot lines that represent DNA sequences."""
         y_distance = len(self.gb_records) * self.y_separation
         # Readjust position sequences to the right or center if requested.
         if self.alignments_position == "right":
             self.adjust_positions_sequences_right()
         elif self.alignments_position == 'center':
             self.adjust_positions_sequences_center()
         # Plot lines representing sequences.
@@ -460,15 +465,54 @@
                 linestyle='solid',
                 color='black',
                 linewidth=2,
                 zorder=1
             )
             y_distance -= self.y_separation
 
-    def make_colormap(self, identity_color, min_val=0.0, max_val=1.0, n=100):
+    def draw_scale_bar(self, ax: Axes, bar_position: int = 0) -> None:
+        """Draw a horizontal scale bar for DNA length."""
+        # Get x_ticks to calculate sequence length.
+        x_ticks = ax.get_xticks()
+        len_ticks = x_ticks[1] - x_ticks[0]
+        # Draw scale_bar.
+        ax.plot(
+            (0, len_ticks),
+            (bar_position, bar_position),
+            linestyle='solid',
+            color='black',
+            linewidth=2,
+            zorder=1
+        )
+        # Annotate scale_bar.
+        location_annotation = len_ticks / 2
+        ax.annotate(
+            f'{self.get_units_size_dna(len_ticks)}',
+            fontsize=8,
+            xy=(location_annotation, bar_position),
+            xytext=(0, -9),
+            textcoords='offset points',
+            ha='center',
+        )
+
+    def get_units_size_dna(self, len_dna: float) -> str:
+        """Get the units of the dna length."""
+        if len_dna < 1_000_000 and len_dna >= 1_000:
+            num = len_dna / 1_000
+            return str(round(num, 1)) + ' kbp'
+        elif len_dna < 1_000_000_000 and len_dna >= 1_000_000:
+            num = len_dna / 1_000_000
+            return str(round(num, 1)) + ' Mbp'
+        else:
+            return str(round(len_dna)) + ' bp'
+
+    def make_colormap(
+            self, identity_color: str, min_val: float = 0.0, max_val:
+            float = 1.0, n: int = 100
+        ) -> Colormap:
         """Make color map for homology regions."""
         try:
             cmap = plt.colormaps[identity_color]
         except KeyError:
             sys.exit(
                 f"Error: the identity color '{identity_color}' provided is "
                 "not valid.\nUse the help option to find valid colors or "
@@ -483,21 +527,16 @@
             truncated_cmap = cmap(np.linspace(min_val, max_val, n))
             new_cmap = colors.LinearSegmentedColormap.from_list(
                 name,
                 truncated_cmap
             )
             return new_cmap
 
-    def plot_homology_regions(self, ax):
-        """Plot homology regions of aligned sequences.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def plot_homology_regions(self, ax: Axes) -> None:
+        """Plot homology regions of aligned sequences."""
         y_distance = ((len(self.alignments) + 1) * self.y_separation)
         # Readjust position of alignment to right or center if requested.
         if self.alignments_position == "right":
             self.adjust_positions_alignments_right()
         elif self.alignments_position == "center":
             self.adjust_positions_alignments_center()
         # Plot regions with homology.
@@ -519,68 +558,104 @@
                     xpoints,
                     ypoints,
                     facecolor=self.color_map(region.homology),
                     linewidth=0
                 )
             y_distance -= self.y_separation
 
-    def plot_colorbar(self, ax):
-        """Plot color bar for homology regions.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def draw_colorbar(self, fig, ax: Axes) -> None:
+        """Draw color bar for homology regions."""
         norm = mpl.colors.Normalize(vmin=0, vmax=100)
         print(
             "lowest and highest plot colorbar:",
             self.lowest_homology, self.highest_homology
         )
+        # if self.lowest_homology != self.highest_homology:
+        #     boundaries = np.linspace(
+        #         self.lowest_homology, self.highest_homology, 100
+        #     )
+        #     pos = ax.get_position()
+        #     print(pos)
+        #     ax.set_position([0, 0, 0.9, 1])
+        #     axins = inset_axes(
+        #         ax,
+        #         width="2%",  # width: 5% of parent_bbox width
+        #         height="20%",  # height: 50%
+        #         loc="lower left",
+        #         bbox_to_anchor=(1.0, 0.01, 1, 1),
+        #         bbox_transform=ax.transAxes,
+        #         borderpad=0,
+        #     )
+        #     colormap = fig.colorbar(
+        #             plt.cm.ScalarMappable(norm=norm, cmap=self.color_map),
+        #             cax=axins,                 # Axes to draw colormap.
+        #             # shrink=0.18,
+        #             # aspect=10,
+        #             orientation='vertical',
+        #             boundaries=boundaries,
+        #             ticks=[self.lowest_homology, self.highest_homology],
+        #     )
+        #     colormap.ax.tick_params(labelsize=8)
+        #     colormap.set_label(
+        #         label="Identity (%)",
+        #         size=7,
+        #         labelpad=-7,
+        #     )
+        #     colormap.outline.set_visible(False) # Remove colormap frame.
+        #     axins.set_aspect(8)                 # Set aspect of colormap.
         if self.lowest_homology != self.highest_homology:
-            # Place colorbar inside figure.
-            # axins = inset_axes(
-            #     ax,
-            #     width='20%',
-            #     height='50%',
-            #     loc='center'
-            # )
             boundaries = np.linspace(
                 self.lowest_homology, self.highest_homology, 100
             )
-            colormap = plt.colorbar(
+            # ax.set_position([0, 0, 0.9, 1])
+            axins = inset_axes(
+                ax,
+                width="15%",  # width: 5% of parent_bbox width
+                height="2.5%",  # height: 50%
+                loc="lower right",
+                bbox_to_anchor=(0., 0.04, 0.95, 0.95),
+                bbox_transform=ax.transAxes,
+                borderpad=0,
+            )
+            colormap = fig.colorbar(
                     plt.cm.ScalarMappable(norm=norm, cmap=self.color_map),
-                    ax=ax,                 # Axes to draw colormap
-                    shrink=0.25,
-                    aspect=10,
-                    label='Identity (%)',
+                    cax=axins,                 # Axes to draw colormap.
                     orientation='horizontal',
                     boundaries=boundaries,
-                    ticks=[self.lowest_homology, self.highest_homology]
+                    ticks=[self.lowest_homology, self.highest_homology],
+            )
+            colormap.ax.tick_params(labelsize=8)
+            # Format ticks 
+            colormap.ax.xaxis.set_major_formatter(
+                ticker.FuncFormatter(lambda x, pos: f'{x}%')
             )
-            colormap.outline.set_visible(False) # Remove colormap frame
-            print("Making colormap...")
+            colormap.set_label(
+                label="Identity",
+                size=7,
+                labelpad=-7,
+            )
+            colormap.outline.set_visible(False) # Remove colormap frame.
+            axins.set_aspect(0.1)               # Set aspect of colormap.
         else:
             homology_path = mpatches.Patch(
                 color=self.color_map(self.highest_homology/100),
-                label=f'{self.highest_homology}',
+                label=f'{self.highest_homology}%',
             )
-            ax.legend(
-                loc="center",
+            legend = ax.legend(
+                loc="center left",
+                bbox_to_anchor=(0.8, 0.04),
                 handles=[homology_path],
                 frameon=False,
-                title="Identity (%)"
+                title="Identity",
+                fontsize=8
             )
+            legend.get_title().set_fontsize(8)
 
-    def plot_genes(self, ax):
-        """Plot genes.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def plot_genes(self, ax: Axes) -> None:
+        """Plot genes."""
         # Separation of genes of each sequence in the y axis.
         y_distance = len(self.gb_records) * self.y_separation
         arrowstyle = mpatches.ArrowStyle(
             "simple", head_width=0.5, head_length=0.2
         )
         # Iterate over GenBankRecords and plot genes.
         for gb_record in self.gb_records:
@@ -592,21 +667,16 @@
                     color=gene.color,
                     mutation_scale=30,
                     zorder=2
                 )
                 ax.add_patch(arrow)
             y_distance -= self.y_separation
 
-    def plot_arrows(self, ax):
-        """Plot arrows to reprent genes.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def plot_arrows(self, ax: Axes) -> None:
+        """Plot arrows to reprent genes."""
         # Separation of genes of each sequence in the y axis.
         y_distance = len(self.gb_records) * self.y_separation
         # Ratio head_height vs lenght of longest sequence.
         ratio = 0.02
         head_height = self.size_longest_sequence * ratio
         # Iterate over GenBankRecords and plot genes.
         for gb_record in self.gb_records:
@@ -617,50 +687,42 @@
                     y=y_distance,
                     head_height=head_height
                 )
                 x_values, y_values = arrow.get_coordinates()
                 ax.fill(x_values, y_values, gene.color)
             y_distance -= self.y_separation
 
-    def annotate_dna_sequences(self, ax):
-        """Annotate DNA sequences.
-
-        Parameters
-        ----------
-        ax : axes, matplotlib object
-        """
+    def annotate_dna_sequences(self, ax: Axes) -> None:
+        """Annotate DNA sequences."""
         # Separation of annotations of each sequence in the y axis.
         y_distance = len(self.gb_records) * self.y_separation
         # Annotate sequences.
         for gb_record in self.gb_records:
             # Check if sequence name is valis.
             if self.sequence_name == 'accession':
                 sequence_name = gb_record.accession
             elif self.sequence_name == 'name':
                 sequence_name = gb_record.name
             elif self.sequence_name == 'fname':
                 sequence_name = gb_record.file_name
             else:
                 sys.exit(
-                    f'Error: invalid sequence name `{sequence_name}` for ' +
+                    f'Error: invalid sequence name `{sequence_name}` for '
                     'annotating sequences.')
             ax.annotate(
                 sequence_name,
                 xy=(gb_record.sequence_end, y_distance),
-                xytext=(10, 0),
+                xytext=(10, -4),
                 textcoords="offset points"
             )
             y_distance -= self.y_separation
 
-    def annotate_gene_sequences(self, ax):
+    def annotate_gene_sequences(self, ax: Axes) -> None:
         """Annotate genes of DNA sequence.
-        
-        Parameters
-        ----------
-        ax : axes, matplotlib object
+
         Note
         ----
         This function annotates genes only of top and bottom sequences.
         """
         # Define dictionaries with parameters to annotate top and bottom
         # sequences. `y_text` indicates how far the annotation is going to be
         # from the position of the gene. `h_alignment` and `v_alignment`
@@ -696,64 +758,65 @@
                     textcoords="offset points",
                     rotation=90,
                     ha="center",
                     horizontalalignment=parameters["h_alignment"],
                     verticalalignment=parameters["v_alignment"]
                 )
 
-    def determine_figure_size(self, num_alignments) -> tuple:
+    def determine_figure_size(
+            self, num_alignments: int) -> tuple[float, float]:
         """Determine figure size."""
         # The Matplotlib default figure size is 6.4 x 4.8.
         width = 6.4
         height = 4.8
-        # Increase height after four alignments.
+        # Adjust height based on four alignments.
         if num_alignments > 4:
             height = height * (num_alignments / 4)
         return (width, height)
 
     def make_figure(self):
         """Make figure with matplotlib."""
-        # Remove toolbar from plot.
+        # -- Remove toolbar from plot -----------------------------------------
         mpl.rcParams['toolbar'] = 'None'
-        # Determine figure size by number of alignments.
+        # -- Determine figure size by number of alignments --------------------
         width, height = self.determine_figure_size(self.num_alignments)
-        # Change figure size. Matplotlib default size is 6.4 x 4.8.
-        if self.lowest_homology == self.highest_homology:
-            fig, (ax_1, ax_2) = plt.subplots(
-                2, 1,
-                figsize=(width, height),
-                layout="constrained",
-                gridspec_kw={'height_ratios': [15, 1]}
-            )
-            # Remove axis
-            ax_1.set_axis_off()
-            ax_2.set_axis_off()
-        else:
-            fig, ax_1 = plt.subplots(
-                figsize=(width, height),
-                layout="constrained"
-            )
-            ax_1.set_axis_off()
-        # Plot DNA sequences.
-        self.plot_dna_sequences(ax_1)
-        # Annotate DNA sequences.
+        # -- Change figure size -----------------------------------------------
+        # Matplotlib default size is 6.4 x 4.8.
+        fig, ax = plt.subplots(
+            figsize=(width, height),
+            layout="constrained"
+        )
+        # -- Remove figure axis -----------------------------------------------
+        ax.set_axis_off()
+        # -- Plot DNA sequences -----------------------------------------------
+        self.plot_dna_sequences(ax)
+        # -- Plot genes using the Arrow class ---------------------------------
+        self.plot_arrows(ax)
+        # -- Plot homology regions --------------------------------------------
+        self.plot_homology_regions(ax)
+        # -- Draw colorbar ----------------------------------------------------
+        self.draw_colorbar(fig, ax)
+        # -- Annotate DNA sequences -------------------------------------------
         if self.annotate_sequences:
-            self.annotate_dna_sequences(ax_1)
-        # Plot homology regions.
-        self.plot_homology_regions(ax_1)
-        # Plot colorbar.
-        if self.lowest_homology == self.highest_homology:
-            self.plot_colorbar(ax_2)
-        else:
-            self.plot_colorbar(ax_1)
-        # Plot genes using the Arrow class.
-        self.plot_arrows(ax_1)
-        # Annotate genes.
+            self.annotate_dna_sequences(ax)
+        # -- Annotate genes ---------------------------------------------------
         if self.annotate_genes:
-            self.annotate_gene_sequences(ax_1)
+            self.annotate_gene_sequences(ax)
+        # -- Plot scale bar ---------------------------------------------------
+        if self.scale_bar and not self.annotate_genes:
+            self.draw_scale_bar(ax, bar_position=self.y_limit)
+        # If annotate genes is activated with scale bar, provide more space for
+        # annotations.
+        elif self.scale_bar and self.annotate_genes:
+            self.draw_scale_bar(ax, bar_position=self.y_limit - 5)
+        # If neither scale bar nor annotate ges are activated, set the y limit
+        # to zero. This will give space for the colorbar.
+        else:
+            ax.set_ylim(bottom=self.y_limit)
+
         return fig
 
     def check_save_figure(self) -> bool:
         """Check if save figure is True."""
         if (self.figure_format is None) and (self.figure_name is None):
             return False
         else:
@@ -763,16 +826,22 @@
         """Save plot."""
         plt.savefig(
             fname=self.figure_name, format=self.figure_format, dpi=self.dpi
         )
 
     def display_figure(self) -> None:
         """Display and save figure."""
-        # # Adjust the padding between and around subplots.
-        # plt.tight_layout()
+        # Adjust the padding between and around subplots.
+        plt.tight_layout()
+        plt.subplots_adjust(
+            left=0, bottom=0, right=1, top=1, wspace=0, hspace=0
+        )
+        plt.margins(0,0)
+        plt.gca().xaxis.set_major_locator(plt.NullLocator())
+        plt.gca().yaxis.set_major_locator(plt.NullLocator())
         # Save figure.
         if self.save_figure and not self.use_gui:
             self.save_plot()
         # Show plot.
         plt.show()
 
     def close_figure(self) -> None:
```

### Comparing `msplotter-0.1.23/src/msp/plot.py` & `msplotter-0.1.28/src/msp/plot.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/slider_widget.py` & `msplotter-0.1.28/src/msp/slider_widget.py`

 * *Files identical despite different names*

### Comparing `msplotter-0.1.23/src/msp/user_input.py` & `msplotter-0.1.28/src/msp/user_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from argparse import Namespace
 import sys
 from pathlib import Path
 import pkg_resources
 from typing import Union
 
 # TODO: test it with app_cli() function.
-# TODO: I need to check the activation of gui
 
 class UserInput:
     """Store information provided by user via the command line."""
     def __init__(
             self,
             input_files: Union[list[Path], None] = None,
             output_folder: Union[None, Path] = None,
@@ -349,15 +348,14 @@
             'is not valid.\n'
             'Valid parameters are: `left`, `center`, or `right`.'
         )
 
 
 def check_annotate_sequences(annotate_sequences: str) -> Union[None, str]:
     """Check correct input for annotate sequences."""
-    #TODO it looks like fname is off
     if (
         annotate_sequences == 'accession'
         or annotate_sequences == 'name'
         or annotate_sequences == 'fname'
     ):
         return annotate_sequences
     else:
```

### Comparing `msplotter-0.1.23/src/msplotter.egg-info/PKG-INFO` & `msplotter-0.1.28/src/msplotter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msplotter
-Version: 0.1.23
+Version: 0.1.28
 Summary: Make a graphical representation of a blastn alignment
 Author-email: Ivan Muñoz-Gutierrez <ivan.munoz.gutierrez@gmail.com>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/ivanmugu/MSPlotter
 Keywords: blast,alignment,graphical representation,DNA sequence,easyfig
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `msplotter-0.1.23/src/msplotter.egg-info/SOURCES.txt` & `msplotter-0.1.28/src/msplotter.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 src/msp/__main__.py
 src/msp/arrows.py
 src/msp/colormap_picker.py
 src/msp/gui.py
 src/msp/msplotter.py
 src/msp/plot.py
 src/msp/slider_widget.py
+src/msp/spinbox.py
 src/msp/user_input.py
 src/msp/images/Blues.png
 src/msp/images/BuGn.png
 src/msp/images/BuPu.png
 src/msp/images/GnBu.png
 src/msp/images/Greens.png
 src/msp/images/Greys.png
```

