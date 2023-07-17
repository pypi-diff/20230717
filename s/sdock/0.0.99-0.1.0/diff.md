# Comparing `tmp/sdock-0.0.99.tar.gz` & `tmp/sdock-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdock-0.0.99.tar", last modified: Mon Jan 30 20:32:17 2023, max compression
+gzip compressed data, was "sdock-0.1.0.tar", last modified: Mon Jul 17 02:44:12 2023, max compression
```

## Comparing `sdock-0.0.99.tar` & `sdock-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-30 20:32:13.000000 sdock-0.0.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 20:32:17.570637 sdock-0.0.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-30 20:32:13.000000 sdock-0.0.99/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/sdock/
--rw-r--r--   0 runner    (1001) docker     (123)    13258 2023-01-30 20:32:13.000000 sdock-0.0.99/sdock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 20:32:17.570637 sdock-0.0.99/sdock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-01-30 20:32:17.000000 sdock-0.0.99/sdock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 20:32:17.570637 sdock-0.0.99/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3161 2023-01-30 20:32:13.000000 sdock-0.0.99/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:44:12.914511 sdock-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-17 02:44:08.000000 sdock-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 02:44:12.914511 sdock-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 02:44:08.000000 sdock-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:44:12.910511 sdock-0.1.0/sdock/
+-rw-r--r--   0 runner    (1001) docker     (123)    25907 2023-07-17 02:44:08.000000 sdock-0.1.0/sdock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24771 2023-07-17 02:44:08.000000 sdock-0.1.0/sdock/vbgen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 02:44:12.914511 sdock-0.1.0/sdock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-17 02:44:12.000000 sdock-0.1.0/sdock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 02:44:12.000000 sdock-0.1.0/sdock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 02:44:12.000000 sdock-0.1.0/sdock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-17 02:44:12.000000 sdock-0.1.0/sdock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 02:44:12.000000 sdock-0.1.0/sdock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 02:44:12.914511 sdock-0.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3172 2023-07-17 02:44:08.000000 sdock-0.1.0/setup.py
```

### Comparing `sdock-0.0.99/LICENSE` & `sdock-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sdock-0.0.99/setup.py` & `sdock-0.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.7.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.99"
+VERSION = "0.1.0"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
@@ -101,15 +101,16 @@
 	python_requires=REQUIRES_PYTHON,
 	url=URL,
 	packages=find_packages(
 		exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
 	entry_points={
 	},
 	install_requires=[
-		"requests"
+		"requests",
+		"xsdata"
 	],
 	include_package_data=True,
 	classifiers=[
 		'Programming Language :: Python',
 		'Programming Language :: Python :: 3',
 		'Programming Language :: Python :: 3.8',
 	],
```

