# Comparing `tmp/idlerich-0.2.1.tar.gz` & `tmp/idlerich-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idlerich-0.2.1.tar", last modified: Sun Jul 16 21:15:27 2023, max compression
+gzip compressed data, was "idlerich-0.3.0.tar", last modified: Sun Jul 16 22:09:03 2023, max compression
```

## Comparing `idlerich-0.2.1.tar` & `idlerich-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.552082 idlerich-0.2.1/
--rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.2.1/LICENSE
--rw-rw-rw-   0        0        0      822 2023-07-16 21:15:27.552082 idlerich-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-07-16 21:02:38.000000 idlerich-0.2.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.531095 idlerich-0.2.1/idlerich/
--rw-rw-rw-   0        0        0       13 2023-07-16 20:54:31.000000 idlerich-0.2.1/idlerich/__init__.py
--rw-rw-rw-   0        0        0     3364 2023-07-16 20:57:15.000000 idlerich-0.2.1/idlerich/__main__.py
--rw-rw-rw-   0        0        0      151 2023-07-16 21:14:36.000000 idlerich-0.2.1/idlerich/metadata.py
-drwxrwxrwx   0        0        0        0 2023-07-16 21:15:27.550083 idlerich-0.2.1/idlerich.egg-info/
--rw-rw-rw-   0        0        0      822 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 21:15:27.000000 idlerich-0.2.1/idlerich.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-16 21:15:27.553082 idlerich-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      824 2023-07-16 21:14:16.000000 idlerich-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:09:03.087857 idlerich-0.3.0/
+-rw-rw-rw-   0        0        0     1084 2023-07-16 16:33:58.000000 idlerich-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      822 2023-07-16 22:09:03.086857 idlerich-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      462 2023-07-16 21:02:38.000000 idlerich-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-16 22:09:03.067869 idlerich-0.3.0/idlerich/
+-rw-rw-rw-   0        0        0       13 2023-07-16 20:54:31.000000 idlerich-0.3.0/idlerich/__init__.py
+-rw-rw-rw-   0        0        0     2991 2023-07-16 22:03:27.000000 idlerich-0.3.0/idlerich/__main__.py
+-rw-rw-rw-   0        0        0      151 2023-07-16 22:07:38.000000 idlerich-0.3.0/idlerich/metadata.py
+drwxrwxrwx   0        0        0        0 2023-07-16 22:09:03.085858 idlerich-0.3.0/idlerich.egg-info/
+-rw-rw-rw-   0        0        0      822 2023-07-16 22:09:02.000000 idlerich-0.3.0/idlerich.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-07-16 22:09:02.000000 idlerich-0.3.0/idlerich.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-16 22:09:02.000000 idlerich-0.3.0/idlerich.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-16 22:09:02.000000 idlerich-0.3.0/idlerich.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-16 22:09:02.000000 idlerich-0.3.0/idlerich.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-16 22:09:03.087857 idlerich-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      824 2023-07-16 21:14:16.000000 idlerich-0.3.0/setup.py
```

### Comparing `idlerich-0.2.1/LICENSE` & `idlerich-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `idlerich-0.2.1/PKG-INFO` & `idlerich-0.3.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.2.1
+Version: 0.3.0
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `idlerich-0.2.1/idlerich/__main__.py` & `idlerich-0.3.0/idlerich/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 # imports?
 import sys
 import os
 import packaging.version
 import shutil
 import subprocess
 
-def regencache():
-    # regen da cache
+def main():
+    # patchin' time
     global idlepath, fdir, pyver
 
+    print("Idlerich Patcher started!")
+    print(f"Idlepath: {idlepath}")
+    print(f"Current file dir of pkg: {fdir}")
+    print(f"Currrent py ver: {pyver}")
+
     try:
         print("Yeeting old cache")
         shutil.rmtree(f"{fdir}/idlelib")
 
     except FileNotFoundError:
-        pass
+        print("FileNotFound removing old cache")
 
     print("Regenerating Cache")
     shutil.copytree(idlepath, f"{fdir}/idlelib")
     with open(f"{fdir}/idlelib/ir_version.txt", "w") as f:
         f.write(str(pyver))
 
     print("Patching Pyshell...")
@@ -26,22 +31,23 @@
         pyshellcode = f.read()
 
     pyshellcode = pyshellcode.replace("def begin(self", """\
 # New patch wrapper from Idlerich for IDLE
     def begin(self, *args, **kwargs):
         retval = self.begin_idle(*args, **kwargs)
         self.write("Python-Rich in namespace.")
-        self.interp.runcode(\"\"\"\
+        self.interp.runcode(\"\"\"\\
 import pkgutil
-module_name = "rich"
-for loader, module_name, is_pkg in pkgutil.walk_packages(__path__):
-    _module = loader.find_module(module_name).load_module(module_name)
-    globals()[module_name] = _module
+import os
+import rich
+for loader, module_name, is_pkg in pkgutil.walk_packages(rich.__path__):
+    __import__(f"rich.{module_name}")
 rich.pretty.install()
-rich.traceback.install(show_locals=False)\"\"\")
+rich.traceback.install(show_locals=False)
+del os, pkgutil\"\"\")
         return retval
 
     # Original begin() from IDLE
     def begin_idle(self""")
 
     with open(f"{fdir}/idlelib/pyshell.py", "w") as f:
         f.write(pyshellcode)
@@ -52,42 +58,21 @@
         if file.endswith(".py") or file.endswith(".pyw"):
             with open(f"{fdir}/idlelib/{file}", "r") as f:
                 script = f.read()
 
             with open(f"{fdir}/idlelib/{file}", "w") as f:
                 f.write(f"# Idlerich patch for imports\nimport sys, os\nsys.path.insert(0, os.path.abspath(os.path.dirname(os.path.abspath(__file__)) + \"/..\"))\n\n" + script)
 
-def main():
-    global idlepath, fdir, pyver
-
-    print("Idlerich Patcher started!")
-    print(f"Idlepath: {idlepath}")
-    print(f"Current file dir of pkg: {fdir}")
-    print(f"Currrent py ver: {pyver}")
-
-    try:
-        with open(f"{fdir}/idlelib/ir_version.txt", "r") as f:
-            ir_version = int(f.read())
-
-            print(f"Cache ver: {ir_version}")
-
-            if ir_version < pyver:
-                regencache()
-
-    except:
-        regencache()
-
     pywpath = list(os.path.split(os.path.abspath(sys.executable)))
     pywpath[~0] = pywpath[~0].split(".")
     pywpath[~0][0] += "w"
     pywpath[~0] = ".".join(pywpath[~0])
     pywpath = "/".join(pywpath)
-    print(f"Pythonw path: {pywpath}")
 
-    print("To run Idlerich, run pythonw on idle.pyw in idlelib in your site-packages folder, at python.")
+    print("\nTo run Idlerich, run pythonw on idle.pyw in idlelib in your site-packages folder, at python.")
     print(f"Your pythonw path is {pywpath}, and your idle script path is {fdir}/idlelib/idle.pyw .")
 
 if getattr(sys, 'frozen', False) and hasattr(sys, '_MEIPASS'):
     # idfk y u would pyinstaller idle but ok
     sys.stderr.write("WARNING: Idlerich may not run properly in a PyInstaller environment.\n")
 else:
     pass
```

### Comparing `idlerich-0.2.1/idlerich.egg-info/PKG-INFO` & `idlerich-0.3.0/idlerich.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idlerich
-Version: 0.2.1
+Version: 0.3.0
 Summary: A bootloader that caches and auto-richifies IDLE because I felt lazy.
 Home-page: https://github.com/CuboidRaptor/idlerich
 Author: Cuboid Raptor
 Author-email: fanjas112358@gmail.com
 License: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
```

### Comparing `idlerich-0.2.1/setup.py` & `idlerich-0.3.0/setup.py`

 * *Files identical despite different names*

