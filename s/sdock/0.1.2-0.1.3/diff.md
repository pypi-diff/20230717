# Comparing `tmp/sdock-0.1.2.tar.gz` & `tmp/sdock-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.1.2.tar", last modified: Mon Jul 17 02:59:23 2023, max compression
+gzip compressed data, was "sdock-0.1.3.tar", last modified: Mon Jul 17 03:47:57 2023, max compression
```

## Comparing `sdock-0.1.2.tar` & `sdock-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:59:23.324257 sdock-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 02:59:18.000000 sdock-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 02:59:23.324257 sdock-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 02:59:18.000000 sdock-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:59:23.324257 sdock-0.1.2/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    26012 2023-07-17 02:59:18.000000 sdock-0.1.2/sdock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-17 02:59:18.000000 sdock-0.1.2/sdock/vbgen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:59:23.324257 sdock-0.1.2/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 02:59:23.000000 sdock-0.1.2/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 02:59:23.000000 sdock-0.1.2/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:59:23.000000 sdock-0.1.2/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 02:59:23.000000 sdock-0.1.2/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 02:59:23.000000 sdock-0.1.2/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 02:59:23.324257 sdock-0.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-17 02:59:18.000000 sdock-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:47:57.313403 sdock-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 03:47:51.000000 sdock-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 03:47:57.313403 sdock-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 03:47:51.000000 sdock-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:47:57.313403 sdock-0.1.3/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    26039 2023-07-17 03:47:51.000000 sdock-0.1.3/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-17 03:47:51.000000 sdock-0.1.3/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 03:47:57.313403 sdock-0.1.3/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 03:47:57.000000 sdock-0.1.3/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 03:47:57.000000 sdock-0.1.3/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 03:47:57.000000 sdock-0.1.3/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 03:47:57.000000 sdock-0.1.3/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 03:47:57.000000 sdock-0.1.3/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 03:47:57.313403 sdock-0.1.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-17 03:47:51.000000 sdock-0.1.3/setup.py
```

### Comparing `sdock-0.1.2/LICENSE` & `sdock-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.1.2/sdock/__init__.py` & `sdock-0.1.3/sdock/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
 		if self.shared:
 			exchanged = "-e EXCHANGE_PATH=" + os.path.abspath(os.curdir)
 		else:
 			exchanged = ""
 
 		no_mount = (self.mountto is None or self.mountto.strip() == '') and (self.mountfrom is None or self.mountfrom.strip() == '')
 		dir = cur_dir()
-		use_dir = "$EXCHANGE_PATH" if self.shared else (self.mountfrom if self.mountfrom else dir)
+		use_dir = "$EXCHANGE_PATH" if self.shared else (self.mountfrom if self.mountfrom and self.mountfrom != ':!' else dir)
 
 		if self.cmd:
 			if isinstance(self.cmd, list):
 				cmd = ' '.join(self.cmd)
 			else:
 				cmd = self.cmd 
 		else:
```

### Comparing `sdock-0.1.2/sdock/vbgen.py` & `sdock-0.1.3/sdock/vbgen.py`

 * *Files identical despite different names*

### Comparing `sdock-0.1.2/setup.py` & `sdock-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.7.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.1.2"
+VERSION = "0.1.3"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

