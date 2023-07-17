# Comparing `tmp/adafruit-circuitpython-rgb-display-3.9.2.tar.gz` & `tmp/adafruit-circuitpython-rgb-display-3.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-rgb-display-3.9.2.tar", last modified: Mon Apr 20 16:28:55 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-rgb-display-3.9.3.tar", last modified: Mon May 18 16:26:13 2020, max compression
```

## Comparing `adafruit-circuitpython-rgb-display-3.9.2.tar` & `adafruit-circuitpython-rgb-display-3.9.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.004967 adafruit-circuitpython-rgb-display-3.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.004967 adafruit-circuitpython-rgb-display-3.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1855 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2598 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)       85 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)    16127 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)       59 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     5991 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     7170 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4996 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.004967 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7170 2020-04-20 16:28:54.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2020-04-20 16:28:54.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-04-20 16:28:54.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2020-04-20 16:28:54.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2020-04-20 16:28:54.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.004967 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/
--rw-r--r--   0 runner    (1001) docker     (116)      104 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2758 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/hx8353.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4317 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/hx8357.py
--rw-r--r--   0 runner    (1001) docker     (116)     4274 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ili9341.py
--rw-r--r--   0 runner    (1001) docker     (116)    10712 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/rgb.py
--rw-r--r--   0 runner    (1001) docker     (116)     2865 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/s6d02a1.py
--rw-r--r--   0 runner    (1001) docker     (116)     4932 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ssd1331.py
--rw-r--r--   0 runner    (1001) docker     (116)     4593 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ssd1351.py
--rw-r--r--   0 runner    (1001) docker     (116)     8665 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/st7735.py
--rw-r--r--   0 runner    (1001) docker     (116)     4363 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/st7789.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      482 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5439 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      320 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1216 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     5718 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_fbcp.py
--rw-r--r--   0 runner    (1001) docker     (116)     1423 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_hx8357test.py
--rw-r--r--   0 runner    (1001) docker     (116)     1393 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_ili9341test.py
--rw-r--r--   0 runner    (1001) docker     (116)     3325 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_minipitftstats.py
--rw-r--r--   0 runner    (1001) docker     (116)     1309 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_minipitfttest.py
--rw-r--r--   0 runner    (1001) docker     (116)     6709 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_animated_gif.py
--rw-r--r--   0 runner    (1001) docker     (116)     3117 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (116)     3136 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_image.py
--rw-r--r--   0 runner    (1001) docker     (116)     4471 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_stats.py
--rw-r--r--   0 runner    (1001) docker     (116)     1482 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)       49 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-04-20 16:28:55.008967 adafruit-circuitpython-rgb-display-3.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1901 2020-04-20 16:28:37.000000 adafruit-circuitpython-rgb-display-3.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.924300 adafruit-circuitpython-rgb-display-3.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1855 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     2598 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       85 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)    16127 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     5991 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (116)     1110 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     7170 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     4996 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     7170 2020-05-18 16:26:13.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1211 2020-05-18 16:26:13.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-05-18 16:26:13.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-05-18 16:26:13.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       21 2020-05-18 16:26:13.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/
+-rw-r--r--   0 runner    (1001) docker     (116)      104 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2758 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/hx8353.py
+-rwxr-xr-x   0 runner    (1001) docker     (116)     4317 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/hx8357.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4274 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ili9341.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10712 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/rgb.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2865 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/s6d02a1.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4932 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ssd1331.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4593 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ssd1351.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8665 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/st7735.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4363 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/st7789.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     4414 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (116)      482 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5439 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)      320 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1216 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (116)     5718 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_fbcp.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1324 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_hx8357test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1393 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_ili9341test.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3325 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_minipitftstats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1309 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_minipitfttest.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6755 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_animated_gif.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3117 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3136 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_image.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4471 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_stats.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1435 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-05-18 16:26:13.928300 adafruit-circuitpython-rgb-display-3.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     1901 2020-05-18 16:26:05.000000 adafruit-circuitpython-rgb-display-3.9.3/setup.py
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/.github/workflows/build.yml` & `adafruit-circuitpython-rgb-display-3.9.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/.github/workflows/release.yml` & `adafruit-circuitpython-rgb-display-3.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/.pylintrc` & `adafruit-circuitpython-rgb-display-3.9.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-rgb-display-3.9.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/LICENSE` & `adafruit-circuitpython-rgb-display-3.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/PKG-INFO` & `adafruit-circuitpython-rgb-display-3.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rgb-display
-Version: 3.9.2
+Version: 3.9.3
 Summary: CircuitPython library for RGB displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RGB_Display
 Author: Radomir Dopieralski, Michael McWethy
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/README.rst` & `adafruit-circuitpython-rgb-display-3.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/PKG-INFO` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-rgb-display
-Version: 3.9.2
+Version: 3.9.3
 Summary: CircuitPython library for RGB displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_RGB_Display
 Author: Radomir Dopieralski, Michael McWethy
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_circuitpython_rgb_display.egg-info/SOURCES.txt` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_circuitpython_rgb_display.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/hx8353.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/hx8353.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/hx8357.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/hx8357.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ili9341.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ili9341.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/rgb.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/rgb.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/s6d02a1.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/s6d02a1.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ssd1331.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ssd1331.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/ssd1351.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/ssd1351.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/st7735.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/st7735.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/adafruit_rgb_display/st7789.py` & `adafruit-circuitpython-rgb-display-3.9.3/adafruit_rgb_display/st7789.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/docs/_static/favicon.ico` & `adafruit-circuitpython-rgb-display-3.9.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/docs/conf.py` & `adafruit-circuitpython-rgb-display-3.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/docs/index.rst` & `adafruit-circuitpython-rgb-display-3.9.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_fbcp.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_fbcp.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_hx8357test.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_hx8357test.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 # Quick test of 3.5" TFT FeatherWing (HX8357) with Feather M0 or M4
-# This will work even on a device running displayio
 # Will fill the TFT black and put a red pixel in the center, wait 2 seconds,
 # then fill the screen blue (with no pixel), wait 2 seconds, and repeat.
 import time
 import random
 import digitalio
 import board
-import displayio
 
 from adafruit_rgb_display.rgb import color565
 import adafruit_rgb_display.hx8357 as hx8357
 
-displayio.release_displays()
-
 # Configuration for CS and DC pins (these are TFT FeatherWing defaults):
 cs_pin = digitalio.DigitalInOut(board.D9)
 dc_pin = digitalio.DigitalInOut(board.D10)
 
 # Config for display baudrate (default max is 24mhz):
 BAUDRATE = 24000000
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_ili9341test.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_ili9341test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_minipitftstats.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_minipitftstats.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_minipitfttest.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_minipitfttest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_animated_gif.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_animated_gif.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 Author(s): Melissa LeBlanc-Williams for Adafruit Industries
 """
 import os
 import time
 import digitalio
 import board
 from PIL import Image, ImageOps
+import numpy  # pylint: disable=unused-import
 import adafruit_rgb_display.ili9341 as ili9341
 import adafruit_rgb_display.st7789 as st7789  # pylint: disable=unused-import
 import adafruit_rgb_display.hx8357 as hx8357  # pylint: disable=unused-import
 import adafruit_rgb_display.st7735 as st7735  # pylint: disable=unused-import
 import adafruit_rgb_display.ssd1351 as ssd1351  # pylint: disable=unused-import
 import adafruit_rgb_display.ssd1331 as ssd1331  # pylint: disable=unused-import
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_demo.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_image.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_image.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_pillow_stats.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_pillow_stats.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/examples/rgb_display_simpletest.py` & `adafruit-circuitpython-rgb-display-3.9.3/examples/rgb_display_simpletest.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,21 +2,18 @@
 # This will work even on a device running displayio
 # Will fill the TFT black and put a red pixel in the center, wait 2 seconds,
 # then fill the screen blue (with no pixel), wait 2 seconds, and repeat.
 import time
 import random
 import digitalio
 import board
-import displayio
 
 from adafruit_rgb_display.rgb import color565
 import adafruit_rgb_display.st7789 as st7789
 
-displayio.release_displays()
-
 # Configuratoin for CS and DC pins (these are FeatherWing defaults on M0/M4):
 cs_pin = digitalio.DigitalInOut(board.D5)
 dc_pin = digitalio.DigitalInOut(board.D6)
 reset_pin = digitalio.DigitalInOut(board.D9)
 
 # Config for display baudrate (default max is 24mhz):
 BAUDRATE = 24000000
```

### Comparing `adafruit-circuitpython-rgb-display-3.9.2/setup.py` & `adafruit-circuitpython-rgb-display-3.9.3/setup.py`

 * *Files identical despite different names*

