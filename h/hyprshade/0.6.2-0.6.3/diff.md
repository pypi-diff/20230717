# Comparing `tmp/hyprshade-0.6.2.tar.gz` & `tmp/hyprshade-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyprshade-0.6.2.tar", max compression
+gzip compressed data, was "hyprshade-0.6.3.tar", max compression
```

## Comparing `hyprshade-0.6.2.tar` & `hyprshade-0.6.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1065 2023-07-16 16:02:20.602370 hyprshade-0.6.2/LICENSE
--rw-r--r--   0        0        0     2440 2023-07-16 16:02:20.602370 hyprshade-0.6.2/README.md
--rw-r--r--   0        0        0      125 2023-07-16 16:02:20.606370 hyprshade-0.6.2/examples/config.toml
--rw-r--r--   0        0        0        0 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/__init__.py
--rw-r--r--   0        0        0       92 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/__main__.py
--rw-r--r--   0        0        0     2466 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/cli.py
--rw-r--r--   0        0        0     3709 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/config.py
--rw-r--r--   0        0        0      483 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/constants.py
--rw-r--r--   0        0        0      566 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/helpers.py
--rw-r--r--   0        0        0      803 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/hyprctl.py
--rw-r--r--   0        0        0      812 2023-07-16 16:02:20.606370 hyprshade-0.6.2/hyprshade/utils.py
--rw-r--r--   0        0        0     1036 2023-07-16 16:02:20.606370 hyprshade-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1986 2023-07-16 16:02:20.606370 hyprshade-0.6.2/shaders/blue-light-filter.glsl
--rw-r--r--   0        0        0     1276 2023-07-16 16:02:20.606370 hyprshade-0.6.2/shaders/vibrance.glsl
--rw-r--r--   0        0        0     2883 1970-01-01 00:00:00.000000 hyprshade-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-07-17 17:02:30.069743 hyprshade-0.6.3/LICENSE
+-rw-r--r--   0        0        0     2761 2023-07-17 17:02:30.069743 hyprshade-0.6.3/README.md
+-rw-r--r--   0        0        0      125 2023-07-17 17:02:30.069743 hyprshade-0.6.3/examples/config.toml
+-rw-r--r--   0        0        0        0 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/__main__.py
+-rw-r--r--   0        0        0     2467 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/cli.py
+-rw-r--r--   0        0        0     3709 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/config.py
+-rw-r--r--   0        0        0      483 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/constants.py
+-rw-r--r--   0        0        0      566 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/helpers.py
+-rw-r--r--   0        0        0      803 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/hyprctl.py
+-rw-r--r--   0        0        0      812 2023-07-17 17:02:30.069743 hyprshade-0.6.3/hyprshade/utils.py
+-rw-r--r--   0        0        0     1036 2023-07-17 17:02:30.073743 hyprshade-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1986 2023-07-17 17:02:30.073743 hyprshade-0.6.3/shaders/blue-light-filter.glsl
+-rw-r--r--   0        0        0     1276 2023-07-17 17:02:30.073743 hyprshade-0.6.3/shaders/vibrance.glsl
+-rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 hyprshade-0.6.3/PKG-INFO
```

### Comparing `hyprshade-0.6.2/LICENSE` & `hyprshade-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/README.md` & `hyprshade-0.6.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 ```sh
 sudo pacman -S --needed base-devel
 git clone https://aur.archlinux.org/hyprshade.git
 cd hyprshade
 makepkg -si
 ```
 
-### Other
+### PyPI
 
 If your distribution isn't officially supported, you can also install directly
 from [PyPI](https://pypi.org/project/hyprshade/) with pip:
 
 ```sh
 pip install --user hyprshade
 ```
@@ -45,14 +45,28 @@
 
 ```sh
 pipx install hyprshade
 ```
 
 ## Usage
 
+```text
+Usage: hyprshade [OPTIONS] COMMAND [ARGS]...
+
+Commands:
+  auto     Turn on/off screen shader based on schedule
+  install  Install systemd user units
+  ls       List available screen shaders
+  off      Turn off screen shader
+  on       Turn on screen shader
+  toggle   Toggle screen shader
+```
+
+### Adding Shaders
+
 Hyprshade uses the shader files in your `~/.config/hypr/shaders` directory
 (in addition to the ones installed to `/usr/share/hyprshade`) for all of its commands.
 
 ### Scheduling
 
 To have specific shaders enabled during certain periods of the day, you can
 create a config file in either `~/.config/hypr/hyprshade.toml` or `~/.config/hyprshade/config.toml`.
```

### Comparing `hyprshade-0.6.2/hyprshade/cli.py` & `hyprshade-0.6.3/hyprshade/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     if shade is not None:
         return on(shade)
     return off()
 
 
 @app.command()
 def install() -> int:
-    """Instal systemd user units"""
+    """Install systemd user units"""
 
     from .config import Config
 
     schedule = Config().to_schedule()
 
     with open(path.join(systemd_user_config_home(), "hyprshade.service"), "w") as f:
         f.write(
```

### Comparing `hyprshade-0.6.2/hyprshade/config.py` & `hyprshade-0.6.3/hyprshade/config.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/hyprshade/helpers.py` & `hyprshade-0.6.3/hyprshade/helpers.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/hyprshade/hyprctl.py` & `hyprshade-0.6.3/hyprshade/hyprctl.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/hyprshade/utils.py` & `hyprshade-0.6.3/hyprshade/utils.py`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/pyproject.toml` & `hyprshade-0.6.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyprshade"
-version = "0.6.2"
+version = "0.6.3"
 description = ""
 authors = ["John Bernard <loqusion@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "hyprshade" }]
 include = ["examples", "shaders"]
```

### Comparing `hyprshade-0.6.2/shaders/blue-light-filter.glsl` & `hyprshade-0.6.3/shaders/blue-light-filter.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/shaders/vibrance.glsl` & `hyprshade-0.6.3/shaders/vibrance.glsl`

 * *Files identical despite different names*

### Comparing `hyprshade-0.6.2/PKG-INFO` & `hyprshade-0.6.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyprshade
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 License: MIT
 Author: John Bernard
 Author-email: loqusion@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -43,15 +43,15 @@
 ```sh
 sudo pacman -S --needed base-devel
 git clone https://aur.archlinux.org/hyprshade.git
 cd hyprshade
 makepkg -si
 ```
 
-### Other
+### PyPI
 
 If your distribution isn't officially supported, you can also install directly
 from [PyPI](https://pypi.org/project/hyprshade/) with pip:
 
 ```sh
 pip install --user hyprshade
 ```
@@ -60,14 +60,28 @@
 
 ```sh
 pipx install hyprshade
 ```
 
 ## Usage
 
+```text
+Usage: hyprshade [OPTIONS] COMMAND [ARGS]...
+
+Commands:
+  auto     Turn on/off screen shader based on schedule
+  install  Install systemd user units
+  ls       List available screen shaders
+  off      Turn off screen shader
+  on       Turn on screen shader
+  toggle   Toggle screen shader
+```
+
+### Adding Shaders
+
 Hyprshade uses the shader files in your `~/.config/hypr/shaders` directory
 (in addition to the ones installed to `/usr/share/hyprshade`) for all of its commands.
 
 ### Scheduling
 
 To have specific shaders enabled during certain periods of the day, you can
 create a config file in either `~/.config/hypr/hyprshade.toml` or `~/.config/hyprshade/config.toml`.
```

