# Comparing `tmp/fp23dpy-0.3.8.tar.gz` & `tmp/fp23dpy-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp23dpy-0.3.8.tar", last modified: Tue Mar  3 17:04:10 2020, max compression
+gzip compressed data, was "dist/fp23dpy-0.3.9.tar", last modified: Fri Apr 24 07:36:28 2020, max compression
```

## Comparing `fp23dpy-0.3.8.tar` & `fp23dpy-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5253 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      524 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       49 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/fp23dpy/
--rw-rw-rw-   0 root         (0) root         (0)      506 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7386 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/calibration.py
--rw-rw-rw-   0 root         (0) root         (0)     6269 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/wavelets.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/version.py
--rw-rw-rw-   0 root         (0) root         (0)     4382 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/fp23dpy.py
--rw-rw-rw-   0 root         (0) root         (0)     2699 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/simulation.py
--rw-rw-rw-   0 root         (0) root         (0)     5666 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2848 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/__calibrate_main__.py
--rw-rw-rw-   0 root         (0) root         (0)     5786 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/frequencyPeakFinder.py
--rwxrwxrwx   0 root         (0) root         (0)    10108 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)     9786 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/export.py
--rw-rw-rw-   0 root         (0) root         (0)     3600 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/demodulation.py
--rw-rw-rw-   0 root         (0) root         (0)     3417 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/fp23dpy/roi.py
--rw-rw-rw-   0 root         (0) root         (0)     4147 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/README.md
--rw-r--r--   0 root         (0) root         (0)     5253 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)       78 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      468 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/tests/test_fp23d.py
--rw-r--r--   0 root         (0) root         (0)       38 2020-03-03 17:04:10.000000 fp23dpy-0.3.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1287 2020-03-03 17:03:28.000000 fp23dpy-0.3.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5253 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      524 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/fp23dpy/
+-rw-rw-rw-   0 root         (0) root         (0)      506 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8629 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/calibration.py
+-rw-rw-rw-   0 root         (0) root         (0)     6269 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/wavelets.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     4560 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/fp23dpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2699 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/simulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     5666 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2664 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/__calibrate_main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5786 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/frequencyPeakFinder.py
+-rwxrwxrwx   0 root         (0) root         (0)    10108 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9786 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/demodulation.py
+-rw-rw-rw-   0 root         (0) root         (0)     3417 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/fp23dpy/roi.py
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/README.md
+-rw-r--r--   0 root         (0) root         (0)     5253 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       78 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      468 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/tests/test_fp23d.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-04-24 07:36:28.000000 fp23dpy-0.3.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1287 2020-04-24 07:35:53.000000 fp23dpy-0.3.9/setup.py
```

### Comparing `fp23dpy-0.3.8/fp23dpy.egg-info/PKG-INFO` & `fp23dpy-0.3.9/fp23dpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fp23dpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for 3D reconstruction of Fringe Patterns captured using the Fringe Projection - Laser Induced Fluorescence technique.
 Home-page: https://gitlab.com/roth.adrian/fp23dpy
 Author: Adrian Roth
 Author-email: adrian.roth@forbrf.lth.se
 License: UNKNOWN
 Description: # Fringe Pattern to 3D python
         This is a python package for applying phase demodulation and 3D reconstruction as post processing of Fringe Pattern (FP) images recorded using the Fringe Projection - Laser Induced Fluorescence (FP-LIF) technique.
```

### Comparing `fp23dpy-0.3.8/fp23dpy.egg-info/SOURCES.txt` & `fp23dpy-0.3.9/fp23dpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/calibration.py` & `fp23dpy-0.3.9/fp23dpy/calibration.py`

 * *Files 12% similar despite different names*

```diff
@@ -99,43 +99,74 @@
     return Calibration.calibrate(im)
 
 ## check if visual plots can be produced, if not do not try to load matplotlib stuff
 if os.environ.get('DISPLAY'):
     import matplotlib.pyplot as plt
     import matplotlib.lines as mlines
 
-    def manual(im, calibration_path):
+    def manual_symmetric(im, calibration):
+        if not 'theta' in calibration:
+            print('Error: symmetric not possible if theta is not specified in the current calibration file')
+            return {}
+
+        print("Click on points most to the left and right of the structure")
+        plt.figure()
+        plt.imshow(im)
+        points = np.array(plt.ginput(2, 0, True))
+        plt.close()
+        middle_x, middle_y = np.mean(points, axis=0)
+        radius = middle_x - points[0, 0]
+        principal_point = [middle_x, middle_y]
+        absolute_phase = [int(round(middle_x - radius * np.sin(calibration['theta']))), int(round(middle_y)), 0]
+        return { 'principal_point': principal_point, 'absolute_phase': absolute_phase }
+
+    def print_help():
+        print("Click on one of the bright lines in the figure.")
+        print("Follow the fringe pattern for !5! periods and click again on the brightest part.")
+        print("If you click in error or want to zoom use right click to undo last click.")
+        print()
+
+
+    def manual(im, calibration_path, symmetric=False):
         """
         To use for manual calibration of an image
         
         The image will be plotted in a matplotlib figure and you should click on one place in the figure and then follow the fringe pattern for 5 periods and click again. Right click is used to undo last click. A calibration dictionary is returned with the results
         """
         file_name, _ = osp.splitext(osp.basename(calibration_path))
         go = True
         if osp.isfile(calibration_path):
             string = input('Do you want to overwrite existing ' + calibration_path + ' [Yes/no]: ')
             go = True if string == '' or string.lower() == 'yes' else False
             calibration = Calibration.read(calibration_path)
         else:
             calibration = Calibration()
         if go:
+            print_help()
             fig = plt.figure()
             ax = fig.add_subplot(111)
             mpl = _ManualCalibration(ax)
             ax.imshow(im)
             ax.set_title(file_name.replace('_', '-'))
             plt.show()
             mpl.disconnect()
             T = mpl.T
             if T != 0:
                 gamma = mpl.gamma
                 calibration['T'] = float(T)
                 calibration['gamma'] = float(gamma)
                 calibration.set_theta_direction(mpl.d)
                 return calibration
+
+            if not calibration is None and symmetric:
+                calibration.update(manual_symmetric(im, calibration))
+
+            return calibration
+
+
     class _ManualCalibration:
         """Class for handling the input in the manual calibration case"""
         def __init__(self, ax):
             self.ax = ax
             self.line = None
             self.orth_line = None
             self.T = 0
```

### Comparing `fp23dpy-0.3.8/fp23dpy/wavelets.py` & `fp23dpy-0.3.9/fp23dpy/wavelets.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/fp23dpy.py` & `fp23dpy-0.3.9/fp23dpy/fp23dpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,32 +40,36 @@
         principal_point = roi.apply_to_points([calibration['principal_point']])[0] if 'principal_point' in calibration else np.array(signal.shape) / 2
     else:
         mask = np.zeros(signal.shape)
         principal_point = calibration['principal_point'] if 'principal_point' in calibration else np.array(signal.shape) / 2
 
     shape = signal.shape
 
+    # main estimation of phase here, important!
     phase_with_carrier = dd.demodulate(signal, calibration)
     carrier = h.make_carrier(signal.shape[-2:], calibration['T'], calibration['gamma'], principal_point)
     phase = (1 - 2 * negative_theta) * (phase_with_carrier - carrier)
 
     if 'absolute_phase' in calibration:
         x_a, y_a, absolute_phase = calibration['absolute_phase']
         if isMasked:
             x_a, y_a = roi.apply_to_points([[x_a, y_a]])[0]
+            if phase.mask[y_a, x_a]:
+                raise ValueError('absolute_phase point must not be masked by segmentation')
         phase += absolute_phase - carrier[y_a, x_a] - phase[y_a, x_a]
     else:
         labels, n_labels = measure.label((~mask).astype(int), return_num=True)
         sign = int(np.sign(calibration['theta'])) if 'theta' in calibration else 1
         for j in range(1, n_labels + 1):
             valid = labels == j
             points = np.sort(phase[valid].flatten())
             phase[valid] -= points[int(sign * round(_min_percentile * points.size))]
             # phase[valid] -= np.min(phase[valid])
 
+
     xscale = yscale = dscale = 1.
     if 'theta' in calibration:
         xscale *= 1 / np.cos(calibration['theta'])
         dscale *= phase_to_threeD_const(calibration['T'], calibration['theta'])
     if 'scale' in calibration:
         xscale /= calibration['scale']
         yscale /= calibration['scale']
```

### Comparing `fp23dpy-0.3.8/fp23dpy/simulation.py` & `fp23dpy-0.3.9/fp23dpy/simulation.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/helpers.py` & `fp23dpy-0.3.9/fp23dpy/helpers.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/__calibrate_main__.py` & `fp23dpy-0.3.9/fp23dpy/__calibrate_main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,29 +4,24 @@
 """
 import argparse
 import os.path as osp
 from skimage import io
 
 from . import calibration as cb
 
-def print_help():
-    print("The image will be plotted in a matplotlib figure.")
-    print("Click on one of the bright lines in the figure.")
-    print("Follow the fringe pattern for !5! periods and click again on the brightest part.")
-    print("If you click in error or want to zoom use right click to undo last click.")
-    print()
-
 def calibration_main():
     parser = argparse.ArgumentParser(description='Calibrate an image or data requisition for 3D reconstruction of Fringe Patterns using phase demodulation, for manual calibration remember to measure over 5 periods to get it correct')
     parser.add_argument('files', type=str, nargs='+',
                         help='Input image files to calibrate, image name with calibrat in it will be a global calibration for a directory')
     parser.add_argument('--auto', '-a', action='store_true',
                         help='Automatic calibration')
     parser.add_argument('--print', '-p', action='store_true',
                         help='Print the result to stdout')
+    parser.add_argument('--symmetric', action='store_true',
+                        help='Assume radial symmetric 3D object (only used for manual calibration)')
     args = parser.parse_args()
 
     to_calibrate = args.files
     if osp.isdir(to_calibrate[0]):
         output_dir = to_calibrate[0]
         cal_path_png = osp.join(output_dir, 'calibration_image.png')
         cal_path_tif = osp.join(output_dir, 'calibration_image.tif')
@@ -53,16 +48,15 @@
             calibration_path = osp.join(output_dir, 'calibration_' + file_name + '.txt')
 
         im = io.imread(image_path, as_gray=True)
 
         if args.auto:
             calibration = cb.automatic(im, calibration_path)
         else:
-            print_help()
-            calibration = cb.manual(im, calibration_path)
+            calibration = cb.manual(im, calibration_path, args.symmetric)
         
         if calibration is None:
             continue
         if args.print:
             print(calibration)
         else:
             calibration.write(calibration_path)
```

### Comparing `fp23dpy-0.3.8/fp23dpy/frequencyPeakFinder.py` & `fp23dpy-0.3.9/fp23dpy/frequencyPeakFinder.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/__main__.py` & `fp23dpy-0.3.9/fp23dpy/__main__.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/export.py` & `fp23dpy-0.3.9/fp23dpy/export.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/demodulation.py` & `fp23dpy-0.3.9/fp23dpy/demodulation.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/fp23dpy/roi.py` & `fp23dpy-0.3.9/fp23dpy/roi.py`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/README.md` & `fp23dpy-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `fp23dpy-0.3.8/PKG-INFO` & `fp23dpy-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fp23dpy
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for 3D reconstruction of Fringe Patterns captured using the Fringe Projection - Laser Induced Fluorescence technique.
 Home-page: https://gitlab.com/roth.adrian/fp23dpy
 Author: Adrian Roth
 Author-email: adrian.roth@forbrf.lth.se
 License: UNKNOWN
 Description: # Fringe Pattern to 3D python
         This is a python package for applying phase demodulation and 3D reconstruction as post processing of Fringe Pattern (FP) images recorded using the Fringe Projection - Laser Induced Fluorescence (FP-LIF) technique.
```

### Comparing `fp23dpy-0.3.8/setup.py` & `fp23dpy-0.3.9/setup.py`

 * *Files identical despite different names*

