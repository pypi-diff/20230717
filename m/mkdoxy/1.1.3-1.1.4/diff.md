# Comparing `tmp/mkdoxy-1.1.3.tar.gz` & `tmp/mkdoxy-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdoxy-1.1.3.tar", last modified: Thu Jul 13 15:16:30 2023, max compression
+gzip compressed data, was "mkdoxy-1.1.4.tar", last modified: Mon Jul 17 11:27:48 2023, max compression
```

## Comparing `mkdoxy-1.1.3.tar` & `mkdoxy-1.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.307375 mkdoxy-1.1.3/
--rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.3/LICENSE
--rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-13 15:16:30.307116 mkdoxy-1.1.3/PKG-INFO
--rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.3/README.md
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.294628 mkdoxy-1.1.3/mkdoxy/
--rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/DoxyTagParser.py
--rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.3/mkdoxy/__init__.py
--rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.3/mkdoxy/cache.py
--rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.3/mkdoxy/constants.py
--rw-r--r--   0 kuba       (501) staff       (20)     4415 2023-07-13 14:02:59.000000 mkdoxy-1.1.3/mkdoxy/doxygen.py
--rw-r--r--   0 kuba       (501) staff       (20)     4326 2023-06-30 13:10:28.000000 mkdoxy-1.1.3/mkdoxy/doxyrun.py
--rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/finder.py
--rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/generatorAuto.py
--rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-13 14:03:01.000000 mkdoxy-1.1.3/mkdoxy/generatorBase.py
--rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.3/mkdoxy/generatorSnippets.py
--rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.3/mkdoxy/markdown.py
--rw-r--r--   0 kuba       (501) staff       (20)    21270 2023-07-13 14:03:05.000000 mkdoxy-1.1.3/mkdoxy/node.py
--rw-r--r--   0 kuba       (501) staff       (20)     7660 2023-07-13 13:39:26.000000 mkdoxy-1.1.3/mkdoxy/plugin.py
--rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-13 14:03:06.000000 mkdoxy-1.1.3/mkdoxy/property.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.306417 mkdoxy-1.1.3/mkdoxy/templates/
--rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/annotated.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.3/mkdoxy/templates/classes.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/code.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/error.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/example.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/examples.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/files.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/hierarchy.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/index.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/memDef.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/memTab.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     4572 2023-07-13 13:55:16.000000 mkdoxy-1.1.3/mkdoxy/templates/member.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.3/mkdoxy/templates/modules.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/namespaces.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/page.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/programlisting.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/templates/relatedPages.jinja2
--rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.3/mkdoxy/utils.py
--rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-13 14:03:08.000000 mkdoxy-1.1.3/mkdoxy/xml_parser.py
-drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-13 15:16:30.296345 mkdoxy-1.1.3/mkdoxy.egg-info/
--rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/PKG-INFO
--rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/SOURCES.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/dependency_links.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/entry_points.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)      131 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/requires.txt
--rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-13 15:16:30.000000 mkdoxy-1.1.3/mkdoxy.egg-info/top_level.txt
--rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-13 15:16:30.308850 mkdoxy-1.1.3/setup.cfg
--rwxr-xr-x   0 kuba       (501) staff       (20)     1838 2023-07-13 14:53:59.000000 mkdoxy-1.1.3/setup.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.756512 mkdoxy-1.1.4/
+-rw-r--r--   0 kuba       (501) staff       (20)     1071 2023-01-24 19:48:21.000000 mkdoxy-1.1.4/LICENSE
+-rw-r--r--   0 kuba       (501) staff       (20)     5587 2023-07-17 11:27:48.756381 mkdoxy-1.1.4/PKG-INFO
+-rw-r--r--   0 kuba       (501) staff       (20)     4585 2023-07-13 14:42:53.000000 mkdoxy-1.1.4/README.md
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.752667 mkdoxy-1.1.4/mkdoxy/
+-rw-r--r--   0 kuba       (501) staff       (20)     2628 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/DoxyTagParser.py
+-rw-r--r--   0 kuba       (501) staff       (20)        0 2023-01-24 19:46:54.000000 mkdoxy-1.1.4/mkdoxy/__init__.py
+-rw-r--r--   0 kuba       (501) staff       (20)      252 2023-01-25 07:25:08.000000 mkdoxy-1.1.4/mkdoxy/cache.py
+-rw-r--r--   0 kuba       (501) staff       (20)     2947 2023-07-13 13:55:16.000000 mkdoxy-1.1.4/mkdoxy/constants.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4393 2023-07-17 11:27:23.000000 mkdoxy-1.1.4/mkdoxy/doxygen.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4443 2023-07-17 11:24:21.000000 mkdoxy-1.1.4/mkdoxy/doxyrun.py
+-rw-r--r--   0 kuba       (501) staff       (20)     1980 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/finder.py
+-rw-r--r--   0 kuba       (501) staff       (20)    11316 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/generatorAuto.py
+-rw-r--r--   0 kuba       (501) staff       (20)    16236 2023-07-17 11:27:25.000000 mkdoxy-1.1.4/mkdoxy/generatorBase.py
+-rw-r--r--   0 kuba       (501) staff       (20)    12051 2023-07-13 14:03:02.000000 mkdoxy-1.1.4/mkdoxy/generatorSnippets.py
+-rw-r--r--   0 kuba       (501) staff       (20)     4471 2023-01-25 07:25:08.000000 mkdoxy-1.1.4/mkdoxy/markdown.py
+-rw-r--r--   0 kuba       (501) staff       (20)    21472 2023-07-17 11:27:29.000000 mkdoxy-1.1.4/mkdoxy/node.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7770 2023-07-17 11:24:21.000000 mkdoxy-1.1.4/mkdoxy/plugin.py
+-rw-r--r--   0 kuba       (501) staff       (20)     9288 2023-07-17 11:27:30.000000 mkdoxy-1.1.4/mkdoxy/property.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.756165 mkdoxy-1.1.4/mkdoxy/templates/
+-rw-r--r--   0 kuba       (501) staff       (20)      517 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/annotated.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      380 2023-07-13 13:55:29.000000 mkdoxy-1.1.4/mkdoxy/templates/classes.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      544 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/code.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      613 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/error.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      164 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/example.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      581 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/examples.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      407 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/files.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      498 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/hierarchy.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      437 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/index.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      741 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/memDef.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     1698 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/memTab.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     4632 2023-07-17 11:23:05.000000 mkdoxy-1.1.4/mkdoxy/templates/member.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      426 2023-07-13 13:55:51.000000 mkdoxy-1.1.4/mkdoxy/templates/modules.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      413 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/namespaces.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/page.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      456 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/programlisting.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)      232 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/templates/relatedPages.jinja2
+-rw-r--r--   0 kuba       (501) staff       (20)     3184 2023-06-30 11:43:03.000000 mkdoxy-1.1.4/mkdoxy/utils.py
+-rw-r--r--   0 kuba       (501) staff       (20)     7390 2023-07-17 11:27:32.000000 mkdoxy-1.1.4/mkdoxy/xml_parser.py
+drwxr-xr-x   0 kuba       (501) staff       (20)        0 2023-07-17 11:27:48.753476 mkdoxy-1.1.4/mkdoxy.egg-info/
+-rwxr-xr-x   0 kuba       (501) staff       (20)     5587 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/PKG-INFO
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1072 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/SOURCES.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        1 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/dependency_links.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)       47 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/entry_points.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)      131 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/requires.txt
+-rwxr-xr-x   0 kuba       (501) staff       (20)        7 2023-07-17 11:27:48.000000 mkdoxy-1.1.4/mkdoxy.egg-info/top_level.txt
+-rw-r--r--   0 kuba       (501) staff       (20)       38 2023-07-17 11:27:48.756546 mkdoxy-1.1.4/setup.cfg
+-rwxr-xr-x   0 kuba       (501) staff       (20)     1838 2023-07-17 11:24:52.000000 mkdoxy-1.1.4/setup.py
```

### Comparing `mkdoxy-1.1.3/LICENSE` & `mkdoxy-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/PKG-INFO` & `mkdoxy-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.3
+Version: 1.1.4
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.3 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.4 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.3/README.md` & `mkdoxy-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/DoxyTagParser.py` & `mkdoxy-1.1.4/mkdoxy/DoxyTagParser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/constants.py` & `mkdoxy-1.1.4/mkdoxy/constants.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/doxygen.py` & `mkdoxy-1.1.4/mkdoxy/doxygen.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import logging
 import os
 from xml.etree import ElementTree
 
-import path as path
-
 from mkdoxy.cache import Cache
 from mkdoxy.constants import Kind, Visibility
 from mkdoxy.node import Node
 from mkdoxy.xml_parser import XmlParser
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 
 class Doxygen:
-	def __init__(self, index_path: path, parser: XmlParser, cache: Cache):
+	def __init__(self, index_path: str, parser: XmlParser, cache: Cache):
 		self.debug = parser.debug
 		path_xml = os.path.join(index_path, 'index.xml')
 		if self.debug:
 			log.info(f'Loading XML from: {path_xml}')
 		xml = ElementTree.parse(path_xml).getroot()
 
 		self.parser = parser
```

### Comparing `mkdoxy-1.1.3/mkdoxy/doxyrun.py` & `mkdoxy-1.1.4/mkdoxy/doxyrun.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import hashlib
 import logging
 import tempfile
 from pathlib import Path, PurePath
 from subprocess import Popen, PIPE
+from typing import Optional
 
 log: logging.Logger = logging.getLogger("mkdocs")
 
 
 class DoxygenRun:
 	"""! Class for running Doxygen.
 	@details This class is used to run Doxygen and parse the XML output.
 	"""
-	def __init__(self, doxygenBinPath: str, doxygenSource: str, tempDoxyFolder: str, doxyCfgNew):
+	def __init__(self, doxygenBinPath: str, doxygenSource: str, tempDoxyFolder: str, doxyCfgNew, runPath: Optional[str] = None):
 		"""! Constructor.
 		Default Doxygen config options:
 
 		- INPUT: <doxygenSource>
 		- OUTPUT_DIRECTORY: <tempDoxyFolder>
 		- DOXYFILE_ENCODING: UTF-8
 		- GENERATE_XML: YES
@@ -33,14 +34,15 @@
 		"""
 		self.doxygenBinPath: str = doxygenBinPath
 		self.doxygenSource: str = doxygenSource
 		self.tempDoxyFolder: str = tempDoxyFolder
 		self.doxyCfgNew: dict = doxyCfgNew
 		self.hashFileName: str = "hashChanges.yaml"
 		self.hashFilePath: PurePath = PurePath.joinpath(Path(self.tempDoxyFolder), Path(self.hashFileName))
+		self.runPath: Optional[str] = runPath
 
 		self.doxyCfg: dict = {
 			"INPUT": self.doxygenSource,
 			"OUTPUT_DIRECTORY": self.tempDoxyFolder,
 			"DOXYFILE_ENCODING": "UTF-8",
 			"GENERATE_XML": "YES",
 			"RECURSIVE": "YES",
@@ -113,15 +115,15 @@
 		heshWrite(self.hashFilePath, hahsNew)
 		return True
 
 	def run(self):
 		"""! Run Doxygen with the current configuration using the Popen class.
 		@details
 		"""
-		doxyBuilder = Popen([self.doxygenBinPath, '-'], stdout=PIPE, stdin=PIPE, stderr=PIPE)
+		doxyBuilder = Popen([self.doxygenBinPath, '-'], stdout=PIPE, stdin=PIPE, stderr=PIPE, cwd=self.runPath)
 		stdout_data = doxyBuilder.communicate(self.doxyCfgStr.encode('utf-8'))[0].decode().strip()
 		# log.info(self.destinationDir)
 		# log.info(stdout_data)
 
 	def checkAndRun(self):
 		"""! Check if the source files have changed since the last run and run Doxygen if they have.
 		@details
```

### Comparing `mkdoxy-1.1.3/mkdoxy/finder.py` & `mkdoxy-1.1.4/mkdoxy/finder.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/generatorAuto.py` & `mkdoxy-1.1.4/mkdoxy/generatorAuto.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/generatorBase.py` & `mkdoxy-1.1.4/mkdoxy/generatorBase.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/generatorSnippets.py` & `mkdoxy-1.1.4/mkdoxy/generatorSnippets.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/markdown.py` & `mkdoxy-1.1.4/mkdoxy/markdown.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/node.py` & `mkdoxy-1.1.4/mkdoxy/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,21 @@
 			self._dirname = os.path.dirname(xml_file)
 			self._xml = ElementTree.parse(xml_file).getroot().find('compounddef')
 			if self._xml is None:
 				raise Exception(f'File {xml_file} has no <compounddef>')
 			self._kind = Kind.from_str(self._xml.get('kind'))
 			self._refid = self._xml.get('id')
 			self._language = self._xml.get('language')
-			self._name = self._xml.find('compoundname').text if self._xml.find('compoundname').text is not None else self._refid
+			if self._xml.find('compoundname').text is not None:
+				self._name = self._xml.find('compoundname').text
+			elif self.is_namespace:
+				location = self._xml.find("location")
+				self._name = f"anonymous namespace{{{location.get('file')}}}" if location is not None else self._refid
+			else:
+				self._name = self._refid
 			self._cache.add(self._refid, self)
 			self._static = False
 
 			if self.debug:
 				log.info(f'Parsing: {self._refid}')
 			self._check_for_children()
```

### Comparing `mkdoxy-1.1.3/mkdoxy/plugin.py` & `mkdoxy-1.1.4/mkdoxy/plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """@package mkdoxy.plugin
 MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 
 MkDoxy is a MkDocs plugin for generating documentation from Doxygen XML files.
 """
 
 import logging
+import os
 from pathlib import Path, PurePath
 
 from mkdocs import exceptions
 from mkdocs.config import base, config_options, Config
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure import files, pages
 
@@ -107,15 +108,16 @@
 
 			if self.config.get("save-api"):
 				tempDirApi = tempDir("", self.config.get("save-api"), project_name)
 			else:
 				tempDirApi = tempDir(config['site_dir'], "assets/.doxy/", project_name)
 
 			# Check src changes -> run Doxygen
-			doxygenRun = DoxygenRun(self.config['doxygen-bin-path'], project_data.get('src-dirs'), tempDirApi, project_data.get('doxy-cfg', {}))
+			runPath = os.path.dirname(config.config_file_path) if config.config_file_path else None
+			doxygenRun = DoxygenRun(self.config['doxygen-bin-path'], project_data.get('src-dirs'), tempDirApi, project_data.get('doxy-cfg', {}), runPath)
 			if doxygenRun.checkAndRun():
 				log.info("  -> generating Doxygen files")
 			else:
 				log.info("  -> skip generating Doxygen files (nothing changes)")
 
 			# Parse XML to basic structure
 			cache = Cache()
```

### Comparing `mkdoxy-1.1.3/mkdoxy/property.py` & `mkdoxy-1.1.4/mkdoxy/property.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/annotated.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/annotated.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/code.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/code.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/error.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/error.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/examples.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/examples.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/memDef.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/memDef.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/memTab.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/memTab.jinja2`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/templates/member.jinja2` & `mkdoxy-1.1.4/mkdoxy/templates/member.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Files', 'visibility': 'public', 'kinds': ['file'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Directories', 'visibility': 'public', 'kinds': ['dir'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Modules', 'visibility': 'public', 'kinds': ['group'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Namespaces', 'visibility': 'public', 'kinds': ['namespace'], 'static': False}) }}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': 'Classes', 'visibility': 'public', 'kinds': ['class', 'struct', 'interface'], 'static': False}) }}
 
 {%- for visibility in ['public', 'protected'] -%}
-{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
+{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['slots', ['slot']], ['properties', ['property']], ['signals', ['signal']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {{ templateMemTab.render({'config': {}, 'node': node, 'parent': None, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {%- for child in node.base_classes recursive -%}{%- if child is not string %}
 {{ templateMemTab.render({'config': {}, 'node': child, 'parent': node, 'title': visibility|title + ' ' + static[0]|title + query[0]|title, 'visibility': visibility, 'kinds': query[1], 'static': static[1]}) }}
 {{- loop(child.base_classes)}}
 {%- endif -%}{%- endfor -%}
 {%- endfor -%}
@@ -70,15 +70,15 @@
 {%- if node.has_details %}
 # Detailed Description
 
 {{node.details}}
 {%- endif %}
 
 {%- for visibility in ['public', 'protected'] -%}
-{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
+{%- for query in [['types', ['enum', 'union', 'typedef']], ['attributes', ['variable']], ['properties', ['property']], ['slots', ['slot']], ['signals', ['signal']], ['functions', ['function']]] -%}
 {%- for static in [['', False], ['static ', True]] %}
 {%- if node.has(visibility, query[1], static[1]) %}
 ## {{visibility|title}} {{static[0]|title}}{{query[0]|title}} Documentation
 {% for member in node.query(visibility, query[1], static[1]) -%}
 {{ templateMemDef.render({'config': {}, 'node': member, 'configMemDef': configMemDef}) }}
 {%- endfor %}
 {%- endif -%}
```

### Comparing `mkdoxy-1.1.3/mkdoxy/utils.py` & `mkdoxy-1.1.4/mkdoxy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy/xml_parser.py` & `mkdoxy-1.1.4/mkdoxy/xml_parser.py`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/mkdoxy.egg-info/PKG-INFO` & `mkdoxy-1.1.4/mkdoxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdoxy
-Version: 1.1.3
+Version: 1.1.4
 Summary: MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets
 Home-page: https://github.com/JakubAndrysek/MkDoxy
 Author: Jakub Andrýsek
 Author-email: email@kubaandrysek.cz
 License: MIT
 Project-URL: Source, https://github.com/JakubAndrysek/MkDoxy
 Project-URL: Documentation, https://mkdoxy.kubaandrysek.cz/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.3 Summary: MkDoxy â MkDocs +
+Metadata-Version: 2.1 Name: mkdoxy Version: 1.1.4 Summary: MkDoxy â MkDocs +
 Doxygen = easy documentation generator with code snippets Home-page: https://
 github.com/JakubAndrysek/MkDoxy Author: Jakub AndrÃ½sek Author-email:
 email@kubaandrysek.cz License: MIT Project-URL: Source, https://github.com/
 JakubAndrysek/MkDoxy Project-URL: Documentation, https://
 mkdoxy.kubaandrysek.cz/ Project-URL: Tracker, https://github.com/JakubAndrysek/
 MkDoxy/issues Project-URL: Funding, https://github.com/sponsors/jakubandrysek
 Keywords: mkdoxy,python,open-
```

### Comparing `mkdoxy-1.1.3/mkdoxy.egg-info/SOURCES.txt` & `mkdoxy-1.1.4/mkdoxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdoxy-1.1.3/setup.py` & `mkdoxy-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def requirements():
     with open('requirements.txt') as f:
         return f.read().splitlines()
 
 # https://pypi.org/project/mkdoxy/
 setup(
     name='mkdoxy',
-    version='1.1.3',
+    version='1.1.4',
     description='MkDoxy → MkDocs + Doxygen = easy documentation generator with code snippets',
     long_description=readme(),
     long_description_content_type='text/markdown',
     keywords='mkdoxy, python, open-source, documentation, mkdocs, doxygen, multilanguage, code-snippets, code, snippets, documentation-generator',
     url='https://github.com/JakubAndrysek/MkDoxy',
     author='Jakub Andrýsek',
     author_email='email@kubaandrysek.cz',
```

