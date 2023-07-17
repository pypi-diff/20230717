# Comparing `tmp/toycoronagraph-1.2.1.tar.gz` & `tmp/toycoronagraph-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toycoronagraph-1.2.1.tar", last modified: Fri Jul 14 15:46:13 2023, max compression
+gzip compressed data, was "toycoronagraph-1.2.2.tar", last modified: Sun Jul 16 23:57:30 2023, max compression
```

## Comparing `toycoronagraph-1.2.1.tar` & `toycoronagraph-1.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 15:46:13.042117 toycoronagraph-1.2.1/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1066 2023-07-11 23:55:42.000000 toycoronagraph-1.2.1/LICENSE
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      475 2023-07-14 15:46:13.042117 toycoronagraph-1.2.1/PKG-INFO
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       88 2023-07-14 00:20:27.000000 toycoronagraph-1.2.1/README.md
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       38 2023-07-14 15:46:13.042117 toycoronagraph-1.2.1/setup.cfg
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1298 2023-07-13 21:52:16.000000 toycoronagraph-1.2.1/setup.py
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 15:46:13.042117 toycoronagraph-1.2.1/toycoronagraph/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      201 2023-07-14 15:41:19.000000 toycoronagraph-1.2.1/toycoronagraph/__init__.py
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     3683 2023-07-14 15:40:52.000000 toycoronagraph-1.2.1/toycoronagraph/main.py
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     3320 2023-07-14 13:56:27.000000 toycoronagraph-1.2.1/toycoronagraph/psf.py
-drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-14 15:46:13.042117 toycoronagraph-1.2.1/toycoronagraph.egg-info/
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      475 2023-07-14 15:46:13.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/PKG-INFO
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      324 2023-07-14 15:46:13.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/SOURCES.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-14 15:46:13.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/dependency_links.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-14 15:42:16.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/not-zip-safe
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       57 2023-07-14 15:46:13.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/requires.txt
--rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       15 2023-07-14 15:46:13.000000 toycoronagraph-1.2.1/toycoronagraph.egg-info/top_level.txt
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-16 23:57:30.113281 toycoronagraph-1.2.2/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1066 2023-07-11 23:55:42.000000 toycoronagraph-1.2.2/LICENSE
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      475 2023-07-16 23:57:30.113281 toycoronagraph-1.2.2/PKG-INFO
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     2745 2023-07-16 23:40:30.000000 toycoronagraph-1.2.2/README.md
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       38 2023-07-16 23:57:30.113281 toycoronagraph-1.2.2/setup.cfg
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     1298 2023-07-13 21:52:16.000000 toycoronagraph-1.2.2/setup.py
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-16 23:57:30.109280 toycoronagraph-1.2.2/toycoronagraph/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      200 2023-07-16 04:11:50.000000 toycoronagraph-1.2.2/toycoronagraph/__init__.py
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     4246 2023-07-16 04:12:27.000000 toycoronagraph-1.2.2/toycoronagraph/main.py
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)     3320 2023-07-14 13:56:27.000000 toycoronagraph-1.2.2/toycoronagraph/psf.py
+drwxrwxr-x   0 yuchia    (1000) yuchia    (1000)        0 2023-07-16 23:57:30.113281 toycoronagraph-1.2.2/toycoronagraph.egg-info/
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      475 2023-07-16 23:57:30.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/PKG-INFO
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)      324 2023-07-16 23:57:30.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/SOURCES.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-16 23:57:30.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/dependency_links.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)        1 2023-07-14 15:42:16.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/not-zip-safe
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       57 2023-07-16 23:57:30.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/requires.txt
+-rw-rw-r--   0 yuchia    (1000) yuchia    (1000)       15 2023-07-16 23:57:30.000000 toycoronagraph-1.2.2/toycoronagraph.egg-info/top_level.txt
```

### Comparing `toycoronagraph-1.2.1/LICENSE` & `toycoronagraph-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `toycoronagraph-1.2.1/setup.py` & `toycoronagraph-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `toycoronagraph-1.2.1/toycoronagraph/main.py` & `toycoronagraph-1.2.2/toycoronagraph/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,35 @@
 import numpy as np
 import matplotlib.pyplot as plt
 import hcipy
-from .psf import psf_calculation, cir_psf
+#from .psf import psf_calculation, cir_psf
+from toycoronagraph.psf import psf_calculation, cir_psf
 from astropy.io import fits
 from toycoronagraph import DATADIR
 import os
+
+def is_positive_even_integer(number):
+  """
+  Checks if the input number is a positive even integer.
+
+  Args:
+    number: The number to check.
+
+  Returns:
+    True if the number is a positive even integer, False otherwise.
+  """
+
+  if not isinstance(number, int) or number <= 0:
+    return False
+
+  if number % 2 == 0:
+    return True
+
+  return False
+
 class Target(object):
     """
     A circular symmetric target, which could be a dust ring, a debris disk, or ice remains
 
     Args:
         file_name: The name of the FITS file containing the target image.
 
@@ -16,18 +37,14 @@
         px: The number of pixels in the x-direction.
         py: The number of pixels in the y-direction.
         psf_scale: The scale of the PSF in arcseconds per pixel.
         xpix: The x-coordinates of the pixels in arcseconds.
         ypix: The y-coordinates of the pixels in arcseconds.
         data_jy: The target image in units of Jy.
         pre_img: The target image in units of float64.
-
-    Methods:
-        plot_origin(): Plots the original target image.
-        plot_final(): Plots the target image after processing with the vortex coronagraph.
     """
     def __init__(self, file_name=None, px=512, py=512):
         """
         Constructor for the Target class.
         """
         if file_name == None:
             self.file_name = DATADIR+"example"
@@ -58,37 +75,45 @@
         ax.set_ylabel('y [arcsec]')
         ax.set_xlabel('x [arcsec]')
         cb=plt.colorbar(im,orientation='vertical')
         cb.set_label("$Jy$")
         fig.savefig("origin.png", format='png', bbox_inches='tight')
         plt.show()
         
-    def plot_final(self, charge, img_pixel = 512, psf_range = 16, rot_number = 360, plot_dpi=300):
+    def plot_final(self, charge, coronagraph_type='vortex', img_pixel=512, psf_range=16, rot_number=360, plot_dpi=300):
         """
         Plots the target image after processing with the vortex coronagraph.
 
         Args:
             charge: The vortex charge.
             img_pixel: The number of pixels in the image.
             psf_range: The range of the PSF in pixels.
             rot_number: The number of rotations.
             plot_dpi: The DPI of the plot.
 
         Returns:
             The final image.
         """
+        #check charge number
+        if coronagraph_type=='vortex':
+            if not is_positive_even_integer(charge):
+                print("charge number is not compatible with coronagraph type, auto set to 2")
+                charge = 2
+                
+        #find psf files
         psf_filename = DATADIR+"psfs_c"+str(charge)+".npy"
         if not os.path.exists(psf_filename):
             psf_calculation(charge, img_pixel, psf_range)
             psf_filename = "psfs_c"+str(charge)+".npy"
+        
         final_img_charge = cir_psf(self.pre_img, img_pixel, psf_range, img_pixel, psf_filename)
         fig=plt.figure(dpi=plot_dpi)
         ax2=plt.subplot(111)
         im2=ax2.imshow(final_img_charge,
                    cmap='gnuplot',extent=[np.min(self.ypix),np.max(self.ypix),np.min(self.xpix),np.max(self.xpix)])
         ax2.invert_yaxis()
         ax2.set_ylabel('y [arcsec]')
         ax2.set_xlabel('x [arcsec]')
         cb=plt.colorbar(im2,orientation='vertical')
         cb.set_label("$Jy$")
         fig.savefig("charge"+str(charge)+"_final.png", format='png', bbox_inches='tight')
-        plt.show()
+        plt.show()
```

### Comparing `toycoronagraph-1.2.1/toycoronagraph/psf.py` & `toycoronagraph-1.2.2/toycoronagraph/psf.py`

 * *Files identical despite different names*

