# Comparing `tmp/sv_ttk-2.5.3.tar.gz` & `tmp/sv_ttk-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sv_ttk-2.5.3.tar", last modified: Tue Jul  4 19:08:16 2023, max compression
+gzip compressed data, was "sv_ttk-2.5.4.tar", last modified: Mon Jul 17 13:55:31 2023, max compression
```

## Comparing `sv_ttk-2.5.3.tar` & `sv_ttk-2.5.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/sv_ttk/
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/sv.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/sv_ttk/theme/
--rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/sprites_dark.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/sprites_light.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/spritesheet_dark.png
--rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-07-04 19:08:04.000000 sv_ttk-2.5.3/sv_ttk/theme/spritesheet_light.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 19:08:16.519845 sv_ttk-2.5.3/sv_ttk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-04 19:08:16.000000 sv_ttk-2.5.3/sv_ttk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-04 19:08:16.000000 sv_ttk-2.5.3/sv_ttk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 19:08:16.000000 sv_ttk-2.5.3/sv_ttk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-04 19:08:16.000000 sv_ttk-2.5.3/sv_ttk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.252154 sv_ttk-2.5.4/sv_ttk/
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/sv.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.256154 sv_ttk-2.5.4/sv_ttk/theme/
+-rw-r--r--   0 runner    (1001) docker     (123)    16187 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    16295 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/sprites_dark.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/sprites_light.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    18371 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/spritesheet_dark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18388 2023-07-17 13:55:19.000000 sv_ttk-2.5.4/sv_ttk/theme/spritesheet_light.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:55:31.252154 sv_ttk-2.5.4/sv_ttk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 13:55:31.000000 sv_ttk-2.5.4/sv_ttk.egg-info/top_level.txt
```

### Comparing `sv_ttk-2.5.3/LICENSE` & `sv_ttk-2.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/PKG-INFO` & `sv_ttk-2.5.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv_ttk
-Version: 2.5.3
+Version: 2.5.4
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

### Comparing `sv_ttk-2.5.3/README.md` & `sv_ttk-2.5.4/README.md`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/setup.py` & `sv_ttk-2.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     '<img alt="Cover image" src="https://raw.githubusercontent.com/rdbende/Sun-Valley-ttk-theme/master/assets/hero_light.png">',
     (Path(__file__).parent / "README.md").read_text(),
 )
 
 
 setup(
     name="sv_ttk",
-    version="2.5.3",
+    version="2.5.4",
     license="MIT",
     author="rdbende",
     author_email="rdbende@proton.me",
     url="https://github.com/rdbende/Sun-Valley-ttk-theme",
     project_urls={
         "Source": "https://github.com/rdbende/Sun-Valley-ttk-theme",
         "Documentation": "https://github.com/rdbende/Sun-Valley-ttk-theme/wiki",
```

### Comparing `sv_ttk-2.5.3/sv_ttk/__init__.py` & `sv_ttk-2.5.4/sv_ttk/__init__.py`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/sv.tcl` & `sv_ttk-2.5.4/sv_ttk/sv.tcl`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 font create SunValleyBodyLargeFont -family "Segoe UI Variable$static Text" -size -18
 font create SunValleySubtitleFont -family "Segoe UI Variable$static Display Semibold" -size -20
 font create SunValleyTitleFont -family "Segoe UI Variable$static Display Semibold" -size -28
 font create SunValleyTitleLargeFont -family "Segoe UI Variable$static Display Semibold" -size -40
 font create SunValleyDisplayFont -family "Segoe UI Variable$static Display Semibold" -size -68
 
 proc config_input_font {w} {
-  set font_config [w config -font]
+  set font_config [$w config -font]
   if {[lindex $font_config 3] != [lindex $font_config 4]} {
     return
   }
   if {[ttk::style theme use] in [list "sun-valley-dark" "sun-valley-light"]} {
     $w configure -font SunValleyBodyFont
   }
 }
```

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/dark.tcl` & `sv_ttk-2.5.4/sv_ttk/theme/dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/light.tcl` & `sv_ttk-2.5.4/sv_ttk/theme/light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/sprites_dark.tcl` & `sv_ttk-2.5.4/sv_ttk/theme/sprites_dark.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/sprites_light.tcl` & `sv_ttk-2.5.4/sv_ttk/theme/sprites_light.tcl`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/spritesheet_dark.png` & `sv_ttk-2.5.4/sv_ttk/theme/spritesheet_dark.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk/theme/spritesheet_light.png` & `sv_ttk-2.5.4/sv_ttk/theme/spritesheet_light.png`

 * *Files identical despite different names*

### Comparing `sv_ttk-2.5.3/sv_ttk.egg-info/PKG-INFO` & `sv_ttk-2.5.4/sv_ttk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sv-ttk
-Version: 2.5.3
+Version: 2.5.4
 Summary: A gorgeous theme for Tkinter, based on Windows 11's UI
 Home-page: https://github.com/rdbende/Sun-Valley-ttk-theme
 Author: rdbende
 Author-email: rdbende@proton.me
 License: MIT
 Project-URL: Source, https://github.com/rdbende/Sun-Valley-ttk-theme
 Project-URL: Documentation, https://github.com/rdbende/Sun-Valley-ttk-theme/wiki
```

