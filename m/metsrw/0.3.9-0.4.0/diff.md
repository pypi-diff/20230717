# Comparing `tmp/metsrw-0.3.9.tar.gz` & `tmp/metsrw-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/metsrw-0.3.9.tar", last modified: Fri Jun 21 17:23:24 2019, max compression
+gzip compressed data, was "metsrw-0.4.0.tar", last modified: Mon Jul 17 21:41:54 2023, max compression
```

## Comparing `metsrw-0.3.9.tar` & `metsrw-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        7 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     2651 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      598 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1810 2019-04-08 18:55:47.000000 metsrw-0.3.9/setup.py
--rw-r--r--   0 root         (0) root         (0)    34520 2018-08-26 17:08:43.000000 metsrw-0.3.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       42 2018-08-26 17:08:43.000000 metsrw-0.3.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1649 2018-08-26 17:08:43.000000 metsrw-0.3.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/
--rw-r--r--   0 root         (0) root         (0)     1730 2019-06-21 14:47:14.000000 metsrw-0.3.9/metsrw/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20702 2019-06-07 12:48:19.000000 metsrw-0.3.9/metsrw/metadata.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/plugins/
--rw-r--r--   0 root         (0) root         (0)       26 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/plugins/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/plugins/premisrw/
--rw-r--r--   0 root         (0) root         (0)     2054 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35038 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/premis.py
--rw-r--r--   0 root         (0) root         (0)     2866 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/plugins/premisrw/utils.py
--rw-r--r--   0 root         (0) root         (0)      348 2018-09-25 23:11:23.000000 metsrw-0.3.9/metsrw/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)    21931 2019-06-07 12:48:19.000000 metsrw-0.3.9/metsrw/mets.py
--rw-r--r--   0 root         (0) root         (0)     1785 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-06-21 17:23:24.000000 metsrw-0.3.9/metsrw/resources/
--rw-r--r--   0 root         (0) root         (0)   155309 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/mets.xsd
--rw-r--r--   0 root         (0) root         (0)    12087 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/archivematica_mets_schematron.xml
--rw-r--r--   0 root         (0) root         (0)    12177 2018-08-26 17:08:43.000000 metsrw-0.3.9/metsrw/resources/archivematica_mets_pointer_file_schematron.xml
--rw-r--r--   0 root         (0) root         (0)    19559 2019-06-21 14:47:14.000000 metsrw-0.3.9/metsrw/fsentry.py
--rw-r--r--   0 root         (0) root         (0)     5652 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/validate.py
--rw-r--r--   0 root         (0) root         (0)     7050 2019-04-08 18:55:47.000000 metsrw-0.3.9/metsrw/di.py
--rw-r--r--   0 root         (0) root         (0)       38 2019-06-21 17:23:24.000000 metsrw-0.3.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2651 2019-06-21 17:23:24.000000 metsrw-0.3.9/PKG-INFO
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    34520 2023-04-12 15:05:15.000000 metsrw-0.4.0/LICENSE
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)       42 2023-04-12 15:05:15.000000 metsrw-0.4.0/MANIFEST.in
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     2247 2023-07-17 21:41:54.118139 metsrw-0.4.0/PKG-INFO
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     1526 2023-07-04 15:46:47.000000 metsrw-0.4.0/README.md
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/metsrw/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     2153 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/__init__.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     6927 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/di.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)      318 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/exceptions.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    21862 2023-07-17 21:34:46.000000 metsrw-0.4.0/metsrw/fsentry.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    21224 2023-07-17 21:34:46.000000 metsrw-0.4.0/metsrw/metadata.py
+-rwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)    25470 2023-07-17 21:34:46.000000 metsrw-0.4.0/metsrw/mets.py
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/metsrw/plugins/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)       26 2023-04-12 15:05:15.000000 metsrw-0.4.0/metsrw/plugins/__init__.py
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/metsrw/plugins/premisrw/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     2500 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/plugins/premisrw/__init__.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    35132 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/plugins/premisrw/premis.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     3238 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/plugins/premisrw/utils.py
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/metsrw/resources/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    12177 2023-06-28 14:32:50.000000 metsrw-0.4.0/metsrw/resources/archivematica_mets_pointer_file_schematron.xml
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)    12087 2023-06-28 14:32:50.000000 metsrw-0.4.0/metsrw/resources/archivematica_mets_schematron.xml
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)   136472 2023-04-12 15:05:15.000000 metsrw-0.4.0/metsrw/resources/mets.xsd
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     2056 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/utils.py
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     5580 2023-07-04 15:46:47.000000 metsrw-0.4.0/metsrw/validate.py
+drwxrwxr-x   0 replaceafill  (1000) replaceafill  (1000)        0 2023-07-17 21:41:54.118139 metsrw-0.4.0/metsrw.egg-info/
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     2247 2023-07-17 21:41:54.000000 metsrw-0.4.0/metsrw.egg-info/PKG-INFO
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)      598 2023-07-17 21:41:54.000000 metsrw-0.4.0/metsrw.egg-info/SOURCES.txt
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)        1 2023-07-17 21:41:54.000000 metsrw-0.4.0/metsrw.egg-info/dependency_links.txt
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)        5 2023-07-17 21:41:54.000000 metsrw-0.4.0/metsrw.egg-info/requires.txt
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)        7 2023-07-17 21:41:54.000000 metsrw-0.4.0/metsrw.egg-info/top_level.txt
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)       38 2023-07-17 21:41:54.118139 metsrw-0.4.0/setup.cfg
+-rw-rw-r--   0 replaceafill  (1000) replaceafill  (1000)     1860 2023-07-04 15:46:47.000000 metsrw-0.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `metsrw-0.3.9/metsrw.egg-info/SOURCES.txt` & `metsrw-0.4.0/metsrw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.9/setup.py` & `metsrw-0.4.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 """A setuptools based setup module.
 
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
-
 import codecs
-from os import path
 import re
+from os import path
 
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
 here = path.abspath(path.dirname(__file__))
 
 
 def read(*parts):
     with codecs.open(path.join(here, *parts), "r") as fp:
         return fp.read()
@@ -34,26 +33,28 @@
 
 
 setup(
     name="metsrw",
     version=find_version("metsrw", "__init__.py"),
     description="Library for dealing with METS files.",
     long_description=long_description,
+    long_description_content_type="text/markdown",
     url="https://github.com/artefactual-labs/mets-reader-writer/",
     author="Artefactual",
     author_email="info@artefactual.com",
     license="AGPL",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: GNU Affero General Public License v3",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
     ],
     keywords="mets",
     packages=find_packages(exclude=["docs", "fixtures", "requirements", "tests*"]),
-    install_requires=["future", "lxml", "six"],
+    install_requires=["lxml"],
     include_package_data=True,
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*",
+    python_requires=">=3.6",
 )
```

### Comparing `metsrw-0.3.9/LICENSE` & `metsrw-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.9/README.md` & `metsrw-0.4.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![PyPI version](https://badge.fury.io/py/metsrw.svg)](https://badge.fury.io/py/metsrw) [![Travis CI](https://travis-ci.org/artefactual-labs/mets-reader-writer.svg?branch=master)](https://travis-ci.org/artefactual-labs/mets-reader-writer) [![Coverage status](https://img.shields.io/coveralls/artefactual-labs/mets-reader-writer/master.svg)](https://coveralls.io/r/artefactual-labs/mets-reader-writer)
+[![PyPI version](https://badge.fury.io/py/metsrw.svg)](https://badge.fury.io/py/metsrw) [![codecov](https://codecov.io/gh/artefactual-labs/mets-reader-writer/branch/master/graph/badge.svg?token=1cXYbNlgJr)](https://codecov.io/gh/artefactual-labs/mets-reader-writer)
 
 # METS Reader & Writer
 
 By [Artefactual](https://www.artefactual.com/)
 
 METSRW is a library to help with parsing and creating METS files.
 It provides an API, and abstracts away the actual creation of the XML.
@@ -16,18 +16,18 @@
 
 METSRW can be installed with pip.
 
 `pip install metsrw`
 
 METSRW has been tested with:
 
-* Python 2.7
-* Python 3.4
 * Python 3.6
-
+* Python 3.7
+* Python 3.8
+* Python 3.9
 
 ## Basic Usage
 
 Read a METS file
 
     mets = metsrw.METSDocument.fromfile('path/to/file')  # Reads a file
     mets = metsrw.METSDocument.fromstring('<mets document>')  # Parses a string
```

### Comparing `metsrw-0.3.9/metsrw/__init__.py` & `metsrw-0.4.0/metsrw/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,51 @@
-# -*- coding: utf-8 -*-
 """METS reader and writer."""
-
-from __future__ import absolute_import
 import logging
 
-from .exceptions import MetsError, ParseError
+from . import plugins
+from .di import Dependency
+from .di import feature_broker
+from .di import FeatureBroker
+from .di import has_class_methods
+from .di import has_methods
+from .di import is_class
+from .di import set_feature_broker_to_default_state
+from .exceptions import MetsError
+from .exceptions import ParseError
 from .fsentry import FSEntry
-from .metadata import Agent, AltRecordID, AMDSec, SubSection, MDRef, MDWrap
+from .metadata import Agent
+from .metadata import AltRecordID
+from .metadata import AMDSec
+from .metadata import MDRef
+from .metadata import MDWrap
+from .metadata import SubSection
 from .mets import METSDocument
-from .utils import (
-    NAMESPACES,
-    SCHEMA_LOCATIONS,
-    lxmlns,
-    FILE_ID_PREFIX,
-    GROUP_ID_PREFIX,
-    urlencode,
-    urldecode,
-)
-from .validate import (
-    METS_XSD_PATH,
-    AM_SCT_PATH,
-    AM_PNTR_SCT_PATH,
-    get_schematron,
-    validate,
-    get_xmlschema,
-    xsd_validate,
-    schematron_validate,
-    sct_report_string,
-    xsd_error_log_string,
-    report_string,
-)
-from .di import (
-    FeatureBroker,
-    set_feature_broker_to_default_state,
-    feature_broker,
-    Dependency,
-    has_class_methods,
-    has_methods,
-    is_class,
-)
-from . import plugins
+from .utils import FILE_ID_PREFIX
+from .utils import generate_mdtype_key
+from .utils import GROUP_ID_PREFIX
+from .utils import lxmlns
+from .utils import NAMESPACES
+from .utils import SCHEMA_LOCATIONS
+from .utils import urldecode
+from .utils import urlencode
+from .validate import AM_PNTR_SCT_PATH
+from .validate import AM_SCT_PATH
+from .validate import get_schematron
+from .validate import get_xmlschema
+from .validate import METS_XSD_PATH
+from .validate import report_string
+from .validate import schematron_validate
+from .validate import sct_report_string
+from .validate import validate
+from .validate import xsd_error_log_string
+from .validate import xsd_validate
 
 LOGGER = logging.getLogger(__name__)
 LOGGER.addHandler(logging.NullHandler())
-__version__ = "0.3.9"
+__version__ = "0.4.0"
 
 __all__ = [
     "Agent",
     "AltRecordID",
     "AMDSec",
     "AM_PNTR_SCT_PATH",
     "AM_SCT_PATH",
@@ -63,14 +61,15 @@
     "MetsError",
     "NAMESPACES",
     "ParseError",
     "SCHEMA_LOCATIONS",
     "SubSection",
     "__version__",
     "feature_broker",
+    "generate_mdtype_key",
     "get_schematron",
     "get_xmlschema",
     "has_class_methods",
     "has_methods",
     "is_class",
     "lxmlns",
     "plugins",
```

### Comparing `metsrw-0.3.9/metsrw/metadata.py` & `metsrw-0.4.0/metsrw/metadata.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,56 +1,50 @@
-# -*- coding: utf-8 -*-
 """
 Classes for metadata sections of the METS. Include amdSec, dmdSec, techMD, rightsMD, sourceMD, digiprovMD, mdRef and mdWrap.
 """
-from __future__ import absolute_import
-
 import copy
 import logging
-from lxml import etree
 
-import six
+from lxml import etree
 
 from . import exceptions
 from . import utils
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-class IdGenerator(six.Iterator):
-    """Helper class to generate unique, sequential ids.
-    """
+class IdGenerator:
+    """Helper class to generate unique, sequential ids."""
 
     def __init__(self, prefix):
         self.counter = 0
         self.prefix = prefix
 
     def __next__(self):
         self.counter += 1
-        return u"{}_{}".format(self.prefix, self.counter)
+        return f"{self.prefix}_{self.counter}"
 
     def clear(self):
         self.counter = 0
 
     def register_id(self, id_string):
-        """Register a manually assigned id as used, to avoid collisions.
-        """
+        """Register a manually assigned id as used, to avoid collisions."""
         try:
             prefix, count = id_string.rsplit("_", 1)
             count = int(count)
         except ValueError:
             # We don't need to worry about ids that don't match our pattern
             pass
         else:
             if prefix == self.prefix:
                 self.counter = max(count, self.counter)
 
 
-class AMDSec(object):
+class AMDSec:
     """
     An object representing a section of administrative metadata in a
     document.
 
     This is ordinarily created by :class:`metsrw.mets.METSDocument` instances and does not
     have to be instantiated directly.
 
@@ -114,27 +108,27 @@
         el = etree.Element(utils.lxmlns("mets") + self.tag, ID=self.id_string)
         self.subsections.sort()
         for child in self.subsections:
             el.append(child.serialize(now))
         return el
 
 
-class AltRecordID(object):
+class AltRecordID:
     """
     An object representing an alternative record identifier in the METS document
     (alternatives to the OBJID).
 
     This is ordinarily created by :class:`metsrw.mets.METSDocument` instances and
     does not have to be instantiated directly.
 
     :param str id: Optional unique identifer for the identifier.
     :param str type: Optional identifer type, e.g. 'Accession number'.
     """
 
-    ALT_RECORD_ID_TAG = etree.QName(utils.NAMESPACES[u"mets"], u"altRecordID")
+    ALT_RECORD_ID_TAG = etree.QName(utils.NAMESPACES["mets"], "altRecordID")
 
     def __init__(self, alt_record_id, **kwargs):
         self.text = alt_record_id
         # We use kwargs here to avoid shadowing builtins (id and type).
         self.id = kwargs.get("id", None)
         self.type = kwargs.get("type", None)
 
@@ -144,37 +138,37 @@
         Create a new AltRecordID by parsing root.
 
         :param element: Element to be parsed into an AltRecordID.
         :raises exceptions.ParseError: If element is not a valid altRecordID.
         """
         if element.tag != cls.ALT_RECORD_ID_TAG:
             raise exceptions.ParseError(
-                u"AltRecordID got unexpected tag {}; expected {}".format(
+                "AltRecordID got unexpected tag {}; expected {}".format(
                     element.tag, cls.ALT_RECORD_ID_TAG
                 )
             )
 
-        return cls(element.text, id=element.get(u"ID"), type=element.get(u"TYPE"))
+        return cls(element.text, id=element.get("ID"), type=element.get("TYPE"))
 
     def serialize(self):
         attrs = {}
 
         if self.id:
-            attrs[u"ID"] = self.id
+            attrs["ID"] = self.id
 
         if self.type:
-            attrs[u"TYPE"] = self.type
+            attrs["TYPE"] = self.type
 
         element = etree.Element(self.ALT_RECORD_ID_TAG, **attrs)
         element.text = self.text
 
         return element
 
 
-class Agent(object):
+class Agent:
     """
     An object representing an agent with a relationship to the METS record.
 
     This is ordinarily created by :class:`metsrw.mets.METSDocument` instances and does not
     have to be instantiated directly.
 
     :param str role: Agent role, e.g. 'CREATOR'.
@@ -190,76 +184,76 @@
         "ARCHIVIST",
         "PRESERVATION",
         "DISSEMINATOR",
         "CUSTODIAN",
         "IPOWNER",
     )
     TYPES = ("INDIVIDUAL", "ORGANIZATION")
-    AGENT_TAG = etree.QName(utils.NAMESPACES[u"mets"], u"agent")
-    NAME_TAG = etree.QName(utils.NAMESPACES[u"mets"], u"name")
-    NOTE_TAG = etree.QName(utils.NAMESPACES[u"mets"], u"note")
+    AGENT_TAG = etree.QName(utils.NAMESPACES["mets"], "agent")
+    NAME_TAG = etree.QName(utils.NAMESPACES["mets"], "name")
+    NOTE_TAG = etree.QName(utils.NAMESPACES["mets"], "note")
 
     def __init__(self, role, **kwargs):
         self.role = role
 
         # We use kwargs here to avoid shadowing builtins (id and type).
-        self.id = kwargs.get(u"id", None)
-        self.type = kwargs.get(u"type", None)
-        self.name = kwargs.get(u"name", None)
-        self.notes = kwargs.get(u"notes", [])
+        self.id = kwargs.get("id", None)
+        self.type = kwargs.get("type", None)
+        self.name = kwargs.get("name", None)
+        self.notes = kwargs.get("notes", [])
 
     @classmethod
     def parse(cls, element):
         """
         Create a new Agent by parsing root.
 
         :param element: Element to be parsed into an Agent.
         :raises exceptions.ParseError: If element is not a valid agent.
         """
         if element.tag != cls.AGENT_TAG:
             raise exceptions.ParseError(
-                u"Agent got unexpected tag {}; expected {}".format(
+                "Agent got unexpected tag {}; expected {}".format(
                     element.tag, cls.AGENT_TAG
                 )
             )
 
-        role = element.get(u"ROLE")
+        role = element.get("ROLE")
         if not role:
-            raise exceptions.ParseError(u"Agent must have a ROLE attribute.")
-        if role == u"OTHER":
-            role = element.get(u"OTHERROLE") or role
-        agent_type = element.get(u"TYPE")
-        if agent_type == u"OTHER":
-            agent_type = element.get(u"OTHERTYPE") or agent_type
-        agent_id = element.get(u"ID")
+            raise exceptions.ParseError("Agent must have a ROLE attribute.")
+        if role == "OTHER":
+            role = element.get("OTHERROLE") or role
+        agent_type = element.get("TYPE")
+        if agent_type == "OTHER":
+            agent_type = element.get("OTHERTYPE") or agent_type
+        agent_id = element.get("ID")
         try:
             name = element.find(cls.NAME_TAG).text
         except AttributeError:
             name = None
         notes = [note.text for note in element.findall(cls.NOTE_TAG)]
 
         return cls(role, id=agent_id, type=agent_type, name=name, notes=notes)
 
     def serialize(self):
         attrs = {}
 
         if self.id:
-            attrs[u"ID"] = self.id
+            attrs["ID"] = self.id
 
         if self.role in self.ROLES:
-            attrs[u"ROLE"] = self.role
+            attrs["ROLE"] = self.role
         else:
-            attrs[u"ROLE"] = u"OTHER"
-            attrs[u"OTHERROLE"] = self.role
+            attrs["ROLE"] = "OTHER"
+            attrs["OTHERROLE"] = self.role
 
         if self.type and self.type in self.TYPES:
-            attrs[u"TYPE"] = self.type
+            attrs["TYPE"] = self.type
         elif self.type:
-            attrs[u"TYPE"] = u"OTHER"
-            attrs[u"OTHERTYPE"] = self.type
+            attrs["TYPE"] = "OTHER"
+            attrs["OTHERTYPE"] = self.type
 
         element = etree.Element(self.AGENT_TAG, **attrs)
         if self.name:
             name_element = etree.Element(self.NAME_TAG)
             name_element.text = self.name
             element.append(name_element)
 
@@ -267,15 +261,15 @@
             note_element = etree.Element(self.NOTE_TAG)
             note_element.text = note
             element.append(note_element)
 
         return element
 
 
-class SubSection(object):
+class SubSection:
     """
     An object representing a metadata subsection in a document.
 
     This is usually created automatically and does not have to be instantiated directly.
 
     :param str subsection: Tag name for the subsection to be created.  Should be
         one of 'techMD', 'rightsMD', 'sourceMD' or 'digiprovMD' if contained in an
@@ -289,23 +283,22 @@
     _id_generators = {
         subsection_type: IdGenerator(subsection_type)
         for subsection_type in ALLOWED_SUBSECTIONS
     }
 
     def __init__(self, subsection, contents, section_id=None):
         if subsection not in self.ALLOWED_SUBSECTIONS:
-            raise ValueError(
-                "%s must be one of %s" % (subsection, self.ALLOWED_SUBSECTIONS)
-            )
+            raise ValueError(f"{subsection} must be one of {self.ALLOWED_SUBSECTIONS}")
         self.subsection = subsection
         self.contents = contents
         self.status = None
         self.older = None
         self.newer = None
         self.created = None
+        self.group_id = None
 
         if section_id is None:
             self.id_string = next(self._id_generators[self.subsection])
         else:
             self.id_string = section_id
             self._id_generators[self.subsection].register_id(section_id)
 
@@ -332,17 +325,22 @@
 
         :returns: None or the STATUS string.
         """
         if self.status is not None:
             return self.status
         if self.subsection == "dmdSec":
             if self.older is None:
-                return "original"
+                status = "original"
+                if self.newer is not None:
+                    status += "-superseded"
             else:
-                return "updated"
+                status = "update"
+                if self.newer is not None:
+                    status += "-superseded"
+            return status
         if self.subsection in ("techMD", "rightsMD"):
             # TODO how to handle ones where newer has been deleted?
             if self.newer is None:
                 return "current"
             else:
                 return "superseded"
         return None
@@ -378,29 +376,28 @@
         subsection = root.tag.replace(utils.lxmlns("mets"), "", 1)
         if subsection not in cls.ALLOWED_SUBSECTIONS:
             raise exceptions.ParseError(
                 "SubSection can only parse elements with tag in %s with METS namespace"
                 % (cls.ALLOWED_SUBSECTIONS,)
             )
         section_id = root.get("ID")
-        created = root.get("CREATED", "")
-        status = root.get("STATUS", "")
         child = root[0]
         if child.tag == utils.lxmlns("mets") + "mdWrap":
             mdwrap = MDWrap.parse(child)
             obj = cls(subsection, mdwrap, section_id)
         elif child.tag == utils.lxmlns("mets") + "mdRef":
             mdref = MDRef.parse(child)
             obj = cls(subsection, mdref, section_id)
         else:
             raise exceptions.ParseError(
                 "Child of %s must be mdWrap or mdRef" % subsection
             )
-        obj.created = created
-        obj.status = status
+        obj.created = root.get("CREATED", "")
+        obj.status = root.get("STATUS", "")
+        obj.group_id = root.get("GROUPID", "")
         return obj
 
     def serialize(self, now=None):
         """
         Serialize this SubSection and all children to lxml Element and return it.
 
         :param str now: Default value for CREATED if none set
@@ -409,20 +406,22 @@
         created = self.created if self.created is not None else now
         el = etree.Element(utils.lxmlns("mets") + self.subsection, ID=self.id_string)
         if created:  # Don't add CREATED if none was parsed
             el.set("CREATED", created)
         status = self.get_status()
         if status:
             el.set("STATUS", status)
+        if self.group_id:
+            el.set("GROUPID", self.group_id)
         if self.contents:
             el.append(self.contents.serialize())
         return el
 
 
-class MDRef(object):
+class MDRef:
     """
     An object representing an external XML document, typically associated
     with an :class:`metsrw.fsentry.FSEntry` object.
 
     :param str target: Path to the external document. MDRef does not validate
         the existence of this target.
     :param str mdtype: The string representing the mdtype of XML document being
@@ -430,24 +429,35 @@
     :param str label: Optional LABEL for the mdRef element
     :param str loctype: LOCTYPE of the mdRef.  Must be one of 'ARK', 'URN', 'URL', 'PURL', 'HANDLE', 'DOI' or 'OTHER'.
     :param str otherloctype: OTHERLOCTYPE of the mdRef. Should be provided if loctype is OTHER.
     """
 
     VALID_LOCTYPE = ("ARK", "URN", "URL", "PURL", "HANDLE", "DOI", "OTHER")
 
-    def __init__(self, target, mdtype, loctype, label=None, otherloctype=None):
+    def __init__(
+        self,
+        target,
+        mdtype,
+        loctype,
+        label=None,
+        otherloctype=None,
+        xptr=None,
+        othermdtype=None,
+    ):
         self.target = target
         self.mdtype = mdtype
         self.loctype = loctype
         if loctype not in self.VALID_LOCTYPE:
             raise ValueError(
                 "loctype must be one of {}".format(", ".join(self.VALID_LOCTYPE))
             )
         self.label = label
         self.otherloctype = otherloctype
+        self.xptr = xptr
+        self.othermdtype = othermdtype
 
     @classmethod
     def parse(cls, root):
         """
         Create a new MDWrap by parsing root.
 
         :param root: Element or ElementTree to be parsed into a MDWrap.
@@ -472,31 +482,35 @@
             )
         loctype = root.get("LOCTYPE")
         if not loctype:
             raise exceptions.ParseError("mdRef must have a LOCTYPE")
         # Optional attributes
         label = root.get("LABEL")
         otherloctype = root.get("OTHERLOCTYPE")
+        xptr = root.get("XPTR")
+        othermdtype = root.get("OTHERMDTYPE")
 
-        return cls(target, mdtype, loctype, label, otherloctype)
+        return cls(target, mdtype, loctype, label, otherloctype, xptr, othermdtype)
 
     def serialize(self):
         # If the source document is a METS document, the XPTR attribute of
         # this mdRef element should point to the IDs of each dmdSec element
         # in that document.
         XPTR = None
         try:
             target_doc = etree.parse(self.target)
             dmdsecs = [
                 item.get("ID")
                 for item in target_doc.findall(utils.lxmlns("mets") + "dmdSec")
             ]
             XPTR = "xpointer(id('{}'))".format(" ".join(dmdsecs))
         except Exception:
-            pass
+            # Otherwise use the Xpointer passed to the constructor.
+            if self.xptr is not None:
+                XPTR = self.xptr
 
         el = etree.Element(utils.lxmlns("mets") + "mdRef")
         if self.label:
             el.attrib["LABEL"] = self.label
         if self.target:
             try:
                 el.attrib[utils.lxmlns("xlink") + "href"] = utils.urlencode(self.target)
@@ -507,33 +521,35 @@
                 )
         el.attrib["MDTYPE"] = self.mdtype
         el.attrib["LOCTYPE"] = self.loctype
         if self.otherloctype:
             el.attrib["OTHERLOCTYPE"] = self.otherloctype
         if XPTR:
             el.attrib["XPTR"] = XPTR
+        if self.othermdtype:
+            el.attrib["OTHERMDTYPE"] = self.othermdtype
         return el
 
 
-class MDWrap(object):
+class MDWrap:
     """
     An object representing an XML document enclosed in a METS document.
     The entirety of the XML document will be included; to reference an
     external document, use the :class:`MDRef` class.
 
     :param str document: A string copy of the document, and will be parsed into
         an ElementTree at the time of instantiation.
     :param str mdtype: The MDTYPE of XML document being enclosed. Examples
         include "PREMIS:OBJECT", "PREMIS:EVENT,", "DC" and "OTHER".
     :param str othermdtype: The OTHERMDTYPE of the XML document. Should be set if mdtype is "OTHER".
     """
 
     def __init__(self, document, mdtype, othermdtype=None):
         parser = etree.XMLParser(remove_blank_text=True)
-        if isinstance(document, six.string_types):
+        if isinstance(document, str):
             self.document = etree.fromstring(document, parser=parser)
         elif isinstance(document, (etree._Element, list)):
             self.document = document
         self.mdtype = mdtype
         self.othermdtype = othermdtype
 
     @classmethod
```

### Comparing `metsrw-0.3.9/metsrw/plugins/premisrw/premis.py` & `metsrw-0.4.0/metsrw/plugins/premisrw/premis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,39 @@
-# -*- coding: utf-8 -*-
 """PREMIS-Reader-Writer: a small PREMIS library designed to work as a plugin
 for METS-reader-writer. Public functions and classes:
 
 - data_to_premis
 - premis_to_data
 - PREMISObject
 - PREMISEvent
 - PREMISAgent
 - PREMISRights
 
 """
-__metaclass__ = type
-
 import abc
-from datetime import datetime
+import json
 import pprint
+from datetime import datetime
 from uuid import uuid4
 
 from lxml import etree
 from lxml.builder import ElementMaker
-import six
 
 from . import utils
 
 
 def now():
     return datetime.utcnow().replace(microsecond=0).isoformat("T")
 
 
 def uuid():
     return str(uuid4())
 
 
-@six.add_metaclass(abc.ABCMeta)
-class PREMISElement:
+class PREMISElement(metaclass=abc.ABCMeta):
     """Abstract base class for PREMIS object, event and agent classes. These
     classes must implement ``schema`` and ``defaults`` properties. After that,
     initalization can proceed either by passing a ``data`` kwarg to the class
     or by passing keyword arguments implicit in the element tag names of
     ``self.schema``, e.g.,::
 
         >>> premis_obj = PREMISObject(data=('object', {...}, (...)))
@@ -150,14 +146,17 @@
         equal as should an instance and a tuple if the instance's data is equal
         to the tuple.
         """
         if isinstance(other, PREMISElement):
             return self.data == other.data
         return self.data == other
 
+    def __hash__(self):
+        return hash(json.dumps(self.data, sort_keys=True))
+
     def __getattr__(self, attr_name):
         """Dynamically retrieve and return the value of an attribute which is
         implicitly defined by the return value of ``self.generate_data()``. All
         leaf node element names and full paths (with forward slashes replaced
         by double underscores) are now valid accessors. For example,
         ``premis_object.message_digest`` returns
         ``premis_object.findtext('object_characteristics/fixity/message_digest')``
@@ -261,17 +260,18 @@
             "date_created_by_application": now,
             "relationship": lambda: [],
             "inhibitors": lambda: [],
         }
 
     @property
     def schema(self):
-        related_object_identifier, related_event_identifier = _get_relationship_tag_names(
-            self.premis_version
-        )
+        (
+            related_object_identifier,
+            related_event_identifier,
+        ) = _get_relationship_tag_names(self.premis_version)
         return (
             "object",
             (
                 "object_identifier",
                 ("object_identifier_type",),
                 ("object_identifier_value",),
             ),
@@ -371,15 +371,15 @@
         attr = (
             "event_detail_information__event_detail"
             if self.premis_version == utils.PREMIS_3_0_VERSION
             else "event_detail"
         )
         return dict(
             [
-                tuple([x.strip(' "') for x in kv.strip().split("=", 1)])
+                tuple(x.strip(' "') for x in kv.strip().split("=", 1))
                 for kv in getattr(self, attr).split(";")
             ]
         )
 
     # Compression Event Functionality
     # ==========================================================================
 
@@ -593,27 +593,34 @@
         camel_tag = utils.snake_to_camel(tag)
     func = getattr(element_maker, camel_tag)
     args = []
     attributes = {}
     for element in data[1:]:
         if isinstance(element, dict):
             for key, val in element.items():
+                if isinstance(val, bytes):
+                    val = val.decode()
                 attributes[key] = val
         elif isinstance(element, (tuple, list)):
             args.append(
                 _data_to_lxml_el(
                     element, ns, nsmap, element_maker=element_maker, snake=snake
                 )
             )
-        elif isinstance(element, six.text_type):
+        elif isinstance(element, str):
             args.append(element)
         elif isinstance(element, etree._Element):
             args.append(element)
+        elif isinstance(element, datetime):
+            args.append(element.isoformat(sep=" "))
+        elif isinstance(element, bytes):
+            args.append(element.decode())
         else:
-            args.append(six.binary_type(element))
+            # TODO: is this correct?
+            args.append(bytes(element))
     ret = func(*args)
     for attr, val in attributes.items():
         try:
             ns, attr = attr.split(":")
         except ValueError:
             ns = None
         if snake:
@@ -669,14 +676,17 @@
         attr = _to_colon_ns(attr, default_ns=ns, nsmap=nsmap)
         attrs[attr] = val
     return attrs
 
 
 def _lxml_el_to_data(lxml_el, ns, nsmap, snake=True):
     """Convert an ``lxml._Element`` instance to a Python tuple."""
+    # Ignore comments. They add no value to the data structure.
+    if isinstance(lxml_el, etree._Comment):
+        return ()
     tag_name = _to_colon_ns(lxml_el.tag, default_ns=ns, nsmap=nsmap)
     ret = [tag_name]
     attributes = _get_el_attributes(lxml_el, ns=ns, nsmap=nsmap)
     if attributes:
         ret.append(attributes)
     for sub_el in lxml_el:
         ret.append(_lxml_el_to_data(sub_el, ns, nsmap, snake=snake))
@@ -746,15 +756,15 @@
     that can be used in the ``.schema`` property of a sub-class of
     PREMISElement.
     """
     schema = []
     for element in tuple_:
         if isinstance(element, (tuple, list)):
             try:
-                if isinstance(element[1], six.string_types):
+                if isinstance(element[1], str):
                     schema.append((element[0],))
                 else:
                     schema.append(tuple_to_schema(element))
             except IndexError:
                 schema.append((element[0],))
         else:
             schema.append(element)
@@ -769,15 +779,15 @@
 
     def defaults(self):
         return {}
 
     def schema_getter(self):
         return schema
 
-    new_class_name = "PREMIS{}Element".format(schema[0].capitalize())
+    new_class_name = f"PREMIS{schema[0].capitalize()}Element"
     return type(
         new_class_name,
         (PREMISElement,),
         {"defaults": property(defaults), "schema": property(schema_getter)},
     )
 
 
@@ -814,23 +824,15 @@
     """
     el = data_find(data, path)
     if not isinstance(el, (list, tuple)):
         return None
     texts = [child for child in el[1:] if not isinstance(child, (tuple, list, dict))]
     if not texts:
         return None
-    return " ".join(
-        [
-            # How should we deal with decoding errors when `x` is binary?
-            # For now, we're using the ``strict`` mode. Other options here:
-            # https://docs.python.org/3/library/functions.html#open.
-            six.ensure_text(x, encoding="utf-8", errors="strict")
-            for x in texts
-        ]
-    )
+    return " ".join(texts)
 
 
 def data_find_text_or_all(data, path, dyn_cls=False):
     text = data_find_text(data, path)
     if text:
         return text
     return data_find_all(data, path, dyn_cls=dyn_cls)
```

### Comparing `metsrw-0.3.9/metsrw/plugins/premisrw/utils.py` & `metsrw-0.4.0/metsrw/plugins/premisrw/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,75 @@
-# -*- coding: utf-8 -*-
 # Namespaces, etc.
 
 XSI_NAMESPACE = "http://www.w3.org/2001/XMLSchema-instance"
 
+TOOL_NAMESPACES = {
+    "xlink": "http://www.w3.org/1999/xlink",
+    "fits": "http://hul.harvard.edu/ois/xml/ns/fits/fits_output",
+    "MediaInfo": "https://mediaarea.net/mediainfo",
+}
+
 # PREMIS v. 2.1
 PREMIS_2_1_VERSION = "2.1"
 PREMIS_2_1_NAMESPACE = "info:lc/xmlns/premis-v1"
 PREMIS_2_1_XSD = "http://www.loc.gov/standards/premis/v2/premis-v2-1.xsd"
-PREMIS_2_1_SCHEMA_LOCATION = "{} {}".format(PREMIS_2_1_NAMESPACE, PREMIS_2_1_XSD)
-PREMIS_2_1_NAMESPACES = {"premis": PREMIS_2_1_NAMESPACE, "xsi": XSI_NAMESPACE}
+PREMIS_2_1_SCHEMA_LOCATION = f"{PREMIS_2_1_NAMESPACE} {PREMIS_2_1_XSD}"
+PREMIS_2_1_NAMESPACES = {
+    "premis": PREMIS_2_1_NAMESPACE,
+    "xsi": XSI_NAMESPACE,
+}
+PREMIS_2_1_NAMESPACES.update(TOOL_NAMESPACES)
 PREMIS_2_1_META = {
     "xsi:schema_location": PREMIS_2_1_SCHEMA_LOCATION,
     "version": PREMIS_2_1_VERSION,
 }
 
 # PREMIS v. 2.2
 PREMIS_2_2_VERSION = "2.2"
 PREMIS_2_2_NAMESPACE = "info:lc/xmlns/premis-v2"
 PREMIS_2_2_XSD = "http://www.loc.gov/standards/premis/v2/premis-v2-2.xsd"
-PREMIS_2_2_SCHEMA_LOCATION = "{} {}".format(PREMIS_2_2_NAMESPACE, PREMIS_2_2_XSD)
-PREMIS_2_2_NAMESPACES = {"premis": PREMIS_2_2_NAMESPACE, "xsi": XSI_NAMESPACE}
+PREMIS_2_2_SCHEMA_LOCATION = f"{PREMIS_2_2_NAMESPACE} {PREMIS_2_2_XSD}"
+PREMIS_2_2_NAMESPACES = {
+    "premis": PREMIS_2_2_NAMESPACE,
+    "xsi": XSI_NAMESPACE,
+}
+PREMIS_2_2_NAMESPACES.update(TOOL_NAMESPACES)
 PREMIS_2_2_META = {
     "xsi:schema_location": PREMIS_2_2_SCHEMA_LOCATION,
     "version": PREMIS_2_2_VERSION,
 }
 
 # PREMIS v. 3.0
 PREMIS_3_0_VERSION = "3.0"
 PREMIS_3_0_NAMESPACE = "http://www.loc.gov/premis/v3"
 PREMIS_3_0_XSD = "http://www.loc.gov/standards/premis/v3/premis.xsd"
-PREMIS_3_0_SCHEMA_LOCATION = "{} {}".format(PREMIS_3_0_NAMESPACE, PREMIS_3_0_XSD)
-PREMIS_3_0_NAMESPACES = {"premis": PREMIS_3_0_NAMESPACE, "xsi": XSI_NAMESPACE}
+PREMIS_3_0_SCHEMA_LOCATION = f"{PREMIS_3_0_NAMESPACE} {PREMIS_3_0_XSD}"
+PREMIS_3_0_NAMESPACES = {
+    "premis": PREMIS_3_0_NAMESPACE,
+    "xsi": XSI_NAMESPACE,
+}
+PREMIS_3_0_NAMESPACES.update(TOOL_NAMESPACES)
 PREMIS_3_0_META = {
     "xsi:schema_location": PREMIS_3_0_SCHEMA_LOCATION,
     "version": PREMIS_3_0_VERSION,
 }
 
 PREMIS_VERSIONS_MAP = {
-    PREMIS_2_1_VERSION: {"namespaces": PREMIS_2_2_NAMESPACES, "meta": PREMIS_2_1_META},
-    PREMIS_2_2_VERSION: {"namespaces": PREMIS_2_2_NAMESPACES, "meta": PREMIS_2_2_META},
-    PREMIS_3_0_VERSION: {"namespaces": PREMIS_3_0_NAMESPACES, "meta": PREMIS_3_0_META},
+    PREMIS_2_1_VERSION: {
+        "namespaces": PREMIS_2_2_NAMESPACES,
+        "meta": PREMIS_2_1_META,
+    },
+    PREMIS_2_2_VERSION: {
+        "namespaces": PREMIS_2_2_NAMESPACES,
+        "meta": PREMIS_2_2_META,
+    },
+    PREMIS_3_0_VERSION: {
+        "namespaces": PREMIS_3_0_NAMESPACES,
+        "meta": PREMIS_3_0_META,
+    },
 }
 
 # Treat PREMIS v. 2.2 as the default (for now).
 PREMIS_VERSION = PREMIS_2_2_VERSION
 NAMESPACES = PREMIS_VERSIONS_MAP[PREMIS_VERSION]["namespaces"]
 PREMIS_META = PREMIS_VERSIONS_MAP[PREMIS_VERSION]["meta"]
 PREMIS_SCHEMA_LOCATION = PREMIS_2_2_SCHEMA_LOCATION
```

### Comparing `metsrw-0.3.9/metsrw/mets.py` & `metsrw-0.4.0/metsrw/mets.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,62 +1,63 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import
-
-from builtins import object
-from collections import OrderedDict, namedtuple
-from datetime import datetime
 import logging
 import os
-import six
 import sys
+from collections import namedtuple
+from collections import OrderedDict
+from datetime import datetime
 
 from lxml import etree
 
-# This package
 from . import exceptions
 from . import fsentry
 from . import metadata
 from . import utils
 
+# This package
+
 
 LOGGER = logging.getLogger(__name__)
 
 AIP_ENTRY_TYPE = "archival information package"
 FPtr = namedtuple(
-    "FPtr", "file_uuid derived_from use path amdids checksum checksumtype"
+    "FPtr",
+    "file_uuid derived_from use path amdids dmdids checksum checksumtype fileid transform_files",
 )
+TRANSFORM_PREFIX = "TRANSFORM"
+TRANSFORM_PREFIX_LEN = len(TRANSFORM_PREFIX)
 
 
-class METSDocument(object):
+class METSDocument:
     def __init__(self):
         # Stores the ElementTree if this was parsed from an existing file
         self.tree = None
         # Only root-level elements are stored, since the rest
         # can be inferred via their #children attribute
         self.createdate = None
         self.objid = None
         self.alternate_ids = []
         self._root_elements = []
         self._all_files = None
         self._iter = None
         self.dmdsecs = []
         self.amdsecs = []
         self.agents = []
+        self._custom_structmaps = []
 
     @classmethod
     def read(cls, source):
         """Read ``source`` into a ``METSDocument`` instance. This is an
         instance constructor. The ``source`` may be a path to a METS file, a
         file-like object, or a string of XML.
         """
         if hasattr(source, "read"):
             return cls.fromfile(source)
         if os.path.exists(source):
             return cls.fromfile(source)
-        if isinstance(source, six.string_types):
+        if isinstance(source, str):
             source = source.encode("utf8")
         return cls.fromstring(source)
 
     # FSENTRYS
 
     def _collect_all_files(self, files=None):
         """
@@ -80,14 +81,39 @@
         :returns: Set containing all :class:`FSEntry` in this METS document,
             including descendants of ones explicitly added.
         """
         # FIXME cache this. Should not break when add_child is called on an
         # element already in the document.
         return self._collect_all_files(self._root_elements)
 
+    def get_subsections_counts(self):
+        """
+        Return a dictionary with the count of the following subsections:
+        dmdSec, amdSec, techMD, rightsMD, digiprovMD and sourceMDs.
+
+        :returns: Dict with subsections counts.
+        """
+        subsections = ("techMD", "rightsMD", "digiprovMD", "sourceMD")
+        counts = {
+            "dmdSec": 0,
+            "amdSec": 0,
+            "techMD": 0,
+            "rightsMD": 0,
+            "digiprovMD": 0,
+            "sourceMD": 0,
+        }
+        for entry in self.all_files():
+            counts["dmdSec"] += len(entry.dmdsecs)
+            counts["amdSec"] += len(entry.amdsecs)
+            for amdsec in entry.amdsecs:
+                for subsection in amdsec.subsections:
+                    if subsection.subsection in subsections:
+                        counts[subsection.subsection] += 1
+        return counts
+
     def get_file(self, **kwargs):
         """
         Return the FSEntry that matches parameters.
 
         :param str file_uuid: UUID of the target FSEntry.
         :param str label: structMap LABEL of the target FSEntry.
         :param str type: structMap TYPE of the target FSEntry.
@@ -179,22 +205,22 @@
             attrib["OBJID"] = self.objid
         return etree.Element(utils.lxmlns("mets") + "mets", nsmap=nsmap, attrib=attrib)
 
     def _mets_header(self, now):
         """
         Return the metsHdr Element.
         """
-        header_tag = etree.QName(utils.NAMESPACES[u"mets"], u"metsHdr")
+        header_tag = etree.QName(utils.NAMESPACES["mets"], "metsHdr")
         header_attrs = {}
 
         if self.createdate is None:
-            header_attrs[u"CREATEDATE"] = now
+            header_attrs["CREATEDATE"] = now
         else:
-            header_attrs[u"CREATEDATE"] = self.createdate
-            header_attrs[u"LASTMODDATE"] = now
+            header_attrs["CREATEDATE"] = self.createdate
+            header_attrs["LASTMODDATE"] = now
 
         header_element = etree.Element(header_tag, **header_attrs)
         for agent in self.agents:
             header_element.append(agent.serialize())
         for alternate_id in self.alternate_ids:
             header_element.append(alternate_id.serialize())
 
@@ -270,41 +296,68 @@
         filegrps = {}
         for file_ in files:
             if file_.type.lower() not in ("item", AIP_ENTRY_TYPE):
                 continue
             # Get fileGrp, or create if not exist
             filegrp = filegrps.get(file_.use)
             if filegrp is None:
-                filegrp = etree.SubElement(
-                    filesec, utils.lxmlns("mets") + "fileGrp", USE=file_.use
-                )
+                filegrp = etree.Element(utils.lxmlns("mets") + "fileGrp", USE=file_.use)
                 filegrps[file_.use] = filegrp
 
             file_el = file_.serialize_filesec()
             if file_el is not None:
                 filegrp.append(file_el)
+        for filegrp in self._sort_filegrps(filegrps):
+            filesec.append(filegrp)
 
         return filesec
 
-    def serialize(self, fully_qualified=True):
+    def _sort_filegrps(self, filegrps):
+        uses_order = [
+            "original",
+            "submissionDocumentation",
+            "preservation",
+            "service",
+            "access",
+            "license",
+            "text/ocr",
+            "metadata",
+            "derivative",
+        ]
+        result = []
+        count = len(filegrps)
+        for i, use in enumerate(filegrps.keys()):
+            filegrp = filegrps[use]
+            try:
+                filegrp_position = uses_order.index(use)
+            except ValueError:
+                filegrp_position = count + i
+            result.append((filegrp_position, filegrp))
+
+        return [v for i, v in sorted(result)]
+
+    def serialize(self, fully_qualified=True, normative_structmap=True):
         """
         Returns this document serialized to an xml Element.
 
         :return: Element for this document
         """
         now = datetime.utcnow().replace(microsecond=0).isoformat("T")
         files = self.all_files()
         mdsecs = self._collect_mdsec_elements(files)
         root = self._document_root(fully_qualified=fully_qualified)
         root.append(self._mets_header(now=now))
         for section in mdsecs:
             root.append(section.serialize(now=now))
         root.append(self._filesec(files))
         root.append(self._structmap())
-        root.append(self._normative_structmap())
+        if normative_structmap:
+            root.append(self._normative_structmap())
+        for struct_map in self._custom_structmaps:
+            root.append(struct_map)
         return root
 
     def tostring(self, fully_qualified=True, pretty_print=True, encoding="UTF-8"):
         """
         Serialize and return a string of this METS document.
 
         To write to file, see :meth:`write`.
@@ -361,29 +414,31 @@
             # contain direct fptrs.
             if entry_type.lower() == "directory":
                 children = self._parse_tree_structmap(
                     tree, elem, normative_parent_elem=normative_elem
                 )
                 fs_entry = fsentry.FSEntry.dir(label, children)
                 self._add_dmdsecs_to_fs_entry(elem, fs_entry, tree)
+                self._add_amdsecs_to_fs_entry(elem.get("ADMID"), fs_entry, tree)
                 siblings.append(fs_entry)
                 for fptr_elem in fptr_elems:
                     fptr = self._analyze_fptr(fptr_elem, tree, entry_type)
                     fs_entry = fsentry.FSEntry.from_fptr(
-                        label=None, type_=u"Item", fptr=fptr
+                        label=None, type_="Item", fptr=fptr
                     )
+                    self._add_dmdsecs_to_fs_entry(elem, fs_entry, fptr.dmdids)
                     self._add_amdsecs_to_fs_entry(fptr.amdids, fs_entry, tree)
                     siblings.append(fs_entry)
                 continue
             # Other types, e.g.: items, aips...
             if not len(fptr_elems):
                 continue
             fptr = self._analyze_fptr(fptr_elems[0], tree, entry_type)
             fs_entry = fsentry.FSEntry.from_fptr(label, entry_type, fptr)
-            self._add_dmdsecs_to_fs_entry(elem, fs_entry, tree)
+            self._add_dmdsecs_to_fs_entry(elem, fs_entry, tree, fptr.dmdids)
             self._add_amdsecs_to_fs_entry(fptr.amdids, fs_entry, tree)
             siblings.append(fs_entry)
         return siblings
 
     @staticmethod
     def _get_el_to_normative(parent_elem, normative_parent_elem):
         """Return ordered dict ``el_to_normative``, which maps children of
@@ -432,51 +487,86 @@
             path = utils.urldecode(path)
         except ValueError:
             raise exceptions.ParseError(
                 'Value "{}" (of attribute xlink:href) is not a valid'
                 " URL.".format(path)
             )
         amdids = file_elem.get("ADMID")
+        dmdids = file_elem.get("DMDID")
         checksum = file_elem.get("CHECKSUM")
         checksumtype = file_elem.get("CHECKSUMTYPE")
         file_id_prefix = utils.FILE_ID_PREFIX
-        # If the file is an AIP, then its prefix is not "file-" but the
-        # name of the AIP. Therefore we need to get the extension-less
+        # If the file is an AIP, then its prefix is the name of the AIP,
+        # plus `file-` on 1.10+. Therefore we need to get the extension-less
         # basename of the AIP's path and remove its UUID suffix to ge
         # the prefix to remove from the FILEID attribute value.
-        if entry_type.lower() == "archival information package":
-            file_id_prefix = os.path.splitext(os.path.basename(path))[0][:-36]
+        if entry_type.lower() in (
+            "archival information package",
+            "archival information collection",
+        ):
+            aip_name = os.path.splitext(os.path.basename(path))[0][:-36]
+            if file_id.startswith(file_id_prefix):
+                file_id_prefix = file_id_prefix + aip_name
+            else:
+                file_id_prefix = aip_name
         # If the file is part of a directory (with no intermediate item), then
         # its prefix *may not* be "file-" but the name of the file. This
         # pattern is found in old Archivematica METS files, e.g. see
         # ``fixtures/mets_dir_with_many_ptrs.xml``.
         elif entry_type.lower() == "directory" and file_id[:5] != "file-":
             file_id_prefix = os.path.basename(path) + "-"
         file_uuid = file_id.replace(file_id_prefix, "", 1)
         group_uuid = file_elem.get("GROUPID", "").replace(utils.GROUP_ID_PREFIX, "", 1)
         if group_uuid != file_uuid:
             derived_from = group_uuid  # Use group_uuid as placeholder
-        return FPtr(file_uuid, derived_from, use, path, amdids, checksum, checksumtype)
+        transform_files = []
+        for transform_file in file_elem.findall(
+            "mets:transformFile", namespaces=utils.NAMESPACES
+        ):
+            transform_file_attributes = {}
+            for attrib, value in transform_file.attrib.items():
+                # FSEntry.__init__ will make this uppercase anyway
+                key = attrib.upper()
+                if key.startswith(TRANSFORM_PREFIX):
+                    key = key[TRANSFORM_PREFIX_LEN:]
+                transform_file_attributes[key] = value
+            transform_files.append(transform_file_attributes)
+        return FPtr(
+            file_uuid,
+            derived_from,
+            use,
+            path,
+            amdids,
+            dmdids,
+            checksum,
+            checksumtype,
+            file_id,
+            transform_files,
+        )
 
     @staticmethod
-    def _add_dmdsecs_to_fs_entry(elem, fs_entry, tree):
-        dmdids = elem.get("DMDID")
-        if dmdids:
-            dmdids = dmdids.split()
-            for dmdid in dmdids:
-                dmdsec_elem = tree.find(
-                    'mets:dmdSec[@ID="' + dmdid + '"]', namespaces=utils.NAMESPACES
-                )
-                dmdsec = metadata.SubSection.parse(dmdsec_elem)
-                fs_entry.dmdsecs.append(dmdsec)
-            # Create older/newer relationships
-            fs_entry.dmdsecs.sort(key=lambda x: x.created)
-            for prev_dmdsec, dmdsec in zip(fs_entry.dmdsecs, fs_entry.dmdsecs[1:]):
-                if dmdsec.status == "updated":
-                    prev_dmdsec.replace_with(dmdsec)
+    def _add_dmdsecs_to_fs_entry(elem, fs_entry, tree, dmdids=None):
+        dmdids_to_add = elem.get("DMDID", "").split()
+        if dmdids is not None:
+            dmdids_to_add.extend(
+                [dmdid for dmdid in dmdids.split() if dmdid not in dmdids_to_add]
+            )
+        for dmdid in dmdids_to_add:
+            dmdsec_elem = tree.find(
+                'mets:dmdSec[@ID="' + dmdid + '"]', namespaces=utils.NAMESPACES
+            )
+            dmdsec = metadata.SubSection.parse(dmdsec_elem)
+            fs_entry.dmdsecs.append(dmdsec)
+        # Order by creation date and generate mapping by mdtype_othermdtype
+        fs_entry.dmdsecs.sort(key=lambda x: x.created)
+        for dmdsec in fs_entry.dmdsecs:
+            mdtype_key = utils.generate_mdtype_key(
+                dmdsec.contents.mdtype, getattr(dmdsec.contents, "othermdtype", "")
+            )
+            fs_entry.dmdsecs_by_mdtype.setdefault(mdtype_key, []).append(dmdsec)
 
     @staticmethod
     def _add_amdsecs_to_fs_entry(amdids, fs_entry, tree):
         if amdids:
             amdids = amdids.split()
             for amdid in amdids:
                 amdsec_elem = tree.find(
@@ -500,41 +590,47 @@
 
         # Parse structMap
         structMap = tree.find(
             'mets:structMap[@TYPE="physical"]', namespaces=utils.NAMESPACES
         )
         if structMap is None:
             raise exceptions.ParseError("No physical structMap found.")
+        normative_struct_map_label = "Normative Directory Structure"
         normative_struct_map = tree.find(
-            'mets:structMap[@TYPE="logical"]'
-            '[@LABEL="Normative Directory Structure"]',
+            f'mets:structMap[@TYPE="logical"][@LABEL="{normative_struct_map_label}"]',
             namespaces=utils.NAMESPACES,
         )
         self._root_elements = self._parse_tree_structmap(
             tree, structMap, normative_parent_elem=normative_struct_map
         )
+        self._custom_structmaps = [
+            e
+            for e in tree.findall(
+                'mets:structMap[@TYPE="logical"]',
+                namespaces=utils.NAMESPACES,
+            )
+            if e.attrib.get("LABEL") != normative_struct_map_label
+        ]
 
         # Associated derived files
         for entry in self.all_files():
             entry.derived_from = self.get_file(
                 file_uuid=entry.derived_from, type="Item"
             )
 
     def _parse_header(self, tree):
-        header = self.tree.find(u"mets:metsHdr", namespaces=utils.NAMESPACES)
+        header = self.tree.find("mets:metsHdr", namespaces=utils.NAMESPACES)
         # Check CREATEDATE < now
         if header is not None:
-            createdate = header.get(u"CREATEDATE")
+            createdate = header.get("CREATEDATE")
         else:
             createdate = None
         now = datetime.utcnow().isoformat("T")
         if createdate and createdate > now:
-            raise exceptions.ParseError(
-                u"CREATEDATE more recent than now ({})".format(now)
-            )
+            raise exceptions.ParseError(f"CREATEDATE more recent than now ({now})")
         self.createdate = createdate
 
         if header is not None:
             agent_elements = header.findall(
                 metadata.Agent.AGENT_TAG, namespaces=utils.NAMESPACES
             )
             for agent_element in agent_elements:
```

### Comparing `metsrw-0.3.9/metsrw/utils.py` & `metsrw-0.4.0/metsrw/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-# -*- coding: utf-8 -*-
-from six.moves.urllib.parse import quote_plus, unquote_plus, urlparse, urlunparse
+from urllib.parse import quote_plus
+from urllib.parse import unquote_plus
+from urllib.parse import urlparse
+from urllib.parse import urlunparse
 
 
 ####################################
 # LXML HELPER VALUES AND FUNCTIONS #
 ####################################
 
 NAMESPACES = {
@@ -14,20 +16,20 @@
     "fits": "http://hul.harvard.edu/ois/xml/ns/fits/fits_output",
     "xlink": "http://www.w3.org/1999/xlink",
     "dc": "http://purl.org/dc/elements/1.1/",
 }
 
 SCHEMA_LOCATIONS = (
     "http://www.loc.gov/METS/ "
-    + "http://www.loc.gov/standards/mets/version111/mets.xsd"
+    + "http://www.loc.gov/standards/mets/version1121/mets.xsd"
 )
 
 
 def lxmlns(arg):
-    """ Return XPath-usable namespace. """
+    """Return XPath-usable namespace."""
     return "{" + NAMESPACES[arg] + "}"
 
 
 ####################
 # METSRW CONSTANTS #
 ####################
 
@@ -60,7 +62,15 @@
 
 
 def urldecode(url):
     """Decode percent encoding introduced per RFC3986
     https://tools.ietf.org/html/rfc3986#section-2.1.
     """
     return _urlendecode(url, unquote_plus)
+
+
+def generate_mdtype_key(mdtype, othermdtype=""):
+    """Used to generate the keys of the FSEntry's dmdsecs_by_mdtype dict."""
+    mdtype_key = mdtype
+    if othermdtype:
+        mdtype_key += "_" + othermdtype
+    return mdtype_key
```

### Comparing `metsrw-0.3.9/metsrw/resources/mets.xsd` & `metsrw-0.4.0/metsrw/resources/mets.xsd`

 * *Files 24% similar despite different names*

#### Comparing `metsrw-0.3.9/metsrw/resources/mets.xsd` & `metsrw-0.4.0/metsrw/resources/mets.xsd`

```diff
@@ -1,266 +1,292 @@
 <?xml version="1.0" encoding="utf-8"?>
-<!-- METS: Metadata Encoding and Transmission Standard -->
-<!-- 
-This document is available under the Creative Commons CC0 1.0 Universal Public Domain Dedication (http://creativecommons.org/publicdomain/zero/1.0/). 
-The Digital Library Federation, as creator of this document, has waived all rights to it worldwide under copyright law, including 
-all related and neighboring rights, to the extent allowed by law. For the full text see http://creativecommons.org/publicdomain/zero/1.0/legalcode.
--->
-<!-- 
-Prepared for the Digital Library Federation by Jerome McDonough, New York University,
-with the assistance of Michael Alexander (British Library), Joachim Bauer (Content Conversion Specialists, Germany), 
-Rick Beaubien (University of California), Terry Catapano (Columbia University), Morgan Cundiff (Library of Congress), 
-Susan Dahl (University of Alberta), Markus Enders (State and University Library, Göttingen/British Library),  
-Richard Gartner (Bodleian Library at Oxford/King's College, London), Thomas Habing (University of Illinois at Urbana-Champaign), 
-Nancy Hoebelheinrich (Stanford University/Knowledge Motifs LLC), Arwen Hutt (U.C. San Diego), 
-Mark Kornbluh (Michigan State University), Cecilia Preston (Preston & Lynch), Merrilee Proffitt (Research Libraries Group), 
-Clay Redding (Library of Congress), Jenn Riley (Indiana University), Richard Rinehart (Berkeley Art Museum/Pacific Film Archive), 
-Mackenzie Smith (Massachusetts Institute of Technology), Tobias Steinke (German National Library), 
-Taylor Surface (OCLC), Brian Tingle (California Digital Library) and Robin Wendler (Harvard University), 
-Robert Wolfe (Massachusetts Institute of Technology), Patrick Yott (Brown University).
--->
-<!-- May, 2015 -->
-<!-- Version 1.11 -->
-<!-- Change History -->
-<!-- April 23, 2001: Alpha Draft completed -->
-<!-- June 7, 2001: Beta completed -->
-<!-- 6/7/2001 Beta Changes: 
-    1. add 'Time' as a possible time code value, as well as TCF.
-    2. Make dmdSec ID attribute required; make ID attribute optional on MDRef/MDWrap.
-    3. Add 'Label' attribute to StructMap, along with 'Type'.
-    4. Add DDI and FGDC as potential metadata schemes to enumeration.
-    5. Enable an "otherMDtype" attribute for MDWrap/MDRef and any other element where
-        there's an 'other' in the enumerated possibilities.
-    6. Add a "profile" attribute to METS element.
-    7. Revised mptr declaration so that it's like FLocat/MDRef (and not like XLink)
-    8. Extend internal documentation of <area> attributes.
-    9. Add "other" to the possible set of LOCTYPEs.
-    10. Change ADMIDS to ADMID on FileGrp.
-    11. Change "N" to "Order" on <div> element.
-    12. Change "Number" to "order label" on <div> element
-    13. Add createdate and lastmoddate attributes to mets element.
-    14. Allow <div> and <area> elements to link to administrative metadata sections.
-    15. Normalize attribute pointing facilities for file element and mdRef.
-    16. Provide a LOCTYPE of "other" and an "otherloctype" attribute for pointing to external files.
-    17. Drop PDI from enumeration of LOCTYPES.
-    18. Make MDTYPE required in mdRef and mdWrap.
-    19. Rename preservationMD to digiprovMD.
-    20. Add optional CHECKSUM attribute to FContent element.
-    21. Modularize declarations of fileGrpType and mdSecType attributes and enumerations to
-        simplify maintenance.
-    22. Add TYPE attribute to structMap.
-    23. Declare structMap element using structMapType rather than direct declaration.
-    24. Add area element as possible subelement to <div>, along with par and seq.
-    25. Change mdSec model to ALL, to enable differing order of mdRef/mdWrap elements.
-    26. Extend documentation on <par> and <seq> elements.
- -->
-<!-- October 22, 2001: Gamma completed -->
-<!-- 10/22/2001 Gamma changes:
-    1. Added optional fileSec element beneath METS root element to contain fileGrps.
-    2. Created subsidiary schema file xlink.xsd for XLink attributes, restored XLink attributes
-    to mptr element, and added XLink support to mdRef and FLocat.
-    3. Created new element metsHdr to handle metadata regarding METS document
-    itself (analogous to TEI Header).  Moved CREATEDATE and LASTMODDATE attributes
-    to metsHdr, and added new RECORDSTATUS attribute.  Added new subsidiary elements
-    agent and altRecordID to metsHdr.
-    4. Made CREATEDATE and LASTMODDATE attributes type xsd:dateTime to allow more precise
-    recording of when work was done.
-    5. Changed all attributes using data type of xsd:binary to xsd:base64Binary to conform to final
-    W3C schema recommendations.
-    6. Cleaned up annotations/documentation.
- -->
-<!-- December 19, 2001: Epsilon and PROTOFINAL completed-->
-<!-- 12/19/2001 Epsilon changes:
-    1. Changed sequence operator for StructMap so that only 1 root div element is permitted.
-    2. Add new roles to agent element's role attribute and support for extensible 'other' role.
-    3. Add support for extensible 'other' type attribute on agent element.
-    4. Yet more documentation clean up.
-    5. Relocate CHECKSUM attribute from FContent to File element.
-    6. Change the file element's CREATED attribute and fileGroup's VERSDATE attribute to 
-    a type of xsd:dateTime
-    7. Change attribute name DMD for div element to DMDID for consistency's sake.
-    8. Added new behaviorSec for support of referencing executable code from METS object
- -->
-<!-- February 8, 2002: Zeta bug fix to final -->
-<!-- 2/8/2002 Zeta changes:
- 
-    1. Eliminated redundant VRA in metadata type enumeration.
-    2. Changed mdWrap content model, adding xmlData element to eliminate
-        ambiguous content model
- -->
-<!-- June 3, 2002: Version 1.1 -->
-<!-- 6/3/2002 v1.1 changes:
- 
-    1. Add new structLink section for recording hyperlinks between media represented by structMap nodes.
-    2. Allow a <par> element to
-    contain a <seq> -->
-<!-- Dec. 27, 2002: Version 1.2 -->
-<!-- 12/27/2002 v1.2 changes:
-1. Add “USE” attribute to FileGrp, File, FLocat and FContent;
-2. Make FLocat repeatable;
-3. Have FContent mimic mdWrap in using separate binData/xmlData sections;
-4. Copyright statement added;
-5. Allow both FLocat and Fcontent in single file element;
-6. Allow behaviorSec elements to group through GROUPID attribute;
-7. allow descriptive and administrative metadata sections to be grouped through GROUPID attribute;
-8. allow <file> element to point to descriptive metadata via DMDID attribute;
-9. allow descriptive metadata and all forms of administrative metadata to point to administrative metadata via ADMID attribute;
-10. CREATED and STATUS attributes added to all desc. and adm. metadata sections; and
-11. clean up documentation in elements to reflect reality.
--->
-<!-- May 8, 2003: Version 1.3 -->
-<!-- 05/05/2003 v1.3 changes:
-
-1. Change “2. OBJID: a primary identifier assigned to the original source document” to “2. OBJID: a primary identifier assigned to the METS object.”
-2. Add MODS to MDTYPEs.
-3. Modify <file> attributes so that instead of just CHECKSUM we have CHECKSUM and CHECKSUMTYPE, where CHECKSUMTYPE is a controlled vocabulary as follows:
-     HAVAL, MD5, SHA-1, SHA-256, SHA-384, SHA-512, TIGER, WHIRLPOOL
-4.Alter BehaviorSec to make it recursive, and add a new behavior element to wrap mechanism and interfaceDef elements.
--->
-<!-- May 1, 2004: Version 1.4 -->
-<!-- 05/01/2003 v1.4 changes:
-
-1. Moved attribute documentation out of element documentation
-(thank you, Brian Tingle).
-2. New CONTENTIDS attribute (and URIs simpleType) added to div, fptr,
-mptr and area elements for mapping MPEG21 DII Identifier values
-3. XLink namespace URI changed to conform with XLink recommendation.
-4. ID Attribute added to FContent.
-5. ID Attribute addedt to structLink.
-6. ID Attribute added to smLink.
-7. "LOM" added as metadata type.
- -->
-<!-- April 12, 2005: Version 1.5 -->
-<!-- 04/12/2005 v1.5 changes:
- 
- 1. Made file element recursive to deal with PREMIS Onion Layer model and
- support XFDU-ish unpacking specification.
- 2. Add <stream> element beneath <file> to allow linking of metadata to
- subfile structures.
- 3. Modify structLink TO and FROM attributes to put them in XLink namespace.
- 4. Make processContents "lax" for all xsd:any elements.
- -->
-<!-- October 18, 2006: Version 1.6 -->
-<!-- 10/18/2006 v1.6 changes:
-    
- 1. add ID to stream and transformFile
- 2. add ADMID to metsHdr
- 3. make smLink/@xlink:to and smLink/@xlink:from required
- -->
-<!-- October 16, 2007/ Jan 20, 2008: Version 1.7 -->
-<!-- 10/16/2007 01/30/2008  v 1.7 changes:
-    
-1. create parType complex type to allow a seq to contain a par
-2. create FILECORE attribute group with MIMETYPE, SIZE, CHECKSUM, CHECKSUMTYPE;
-     change fileType, mdWrapType and mdRefType use the attribute group, so mdType and mdRef end
-     up with new SIZE, CHECKSUM, and CHECKSUMTYPE attributes (file does not change)
-20080130
-2a. CREATED added to FILECORE
-3. PREMIS:OBJECT PREMIS:AGENT PREMIS:RIGHTS PREMIS:EVENT added to MDTYPE value enumeration
--->
-<!-- April 2009: Version 1.8 -->
-<!-- Version 1.8 changes:
-    1. Add CRC32, Adler-32, MNP to the enumerated values constraining CHECKSUMTYPE to align with MIX messageDigestAlgorithm constraints.
-    2. Add TEXTMD and METSRIGHTS to the enumeration values constraining MDTYPE.
-    3. Add an MDTYPEVERSION attribute as a companion to the MDTYPE attribute in the mdRef and mdWrap elements.  
-    4. ID and STRUCTID attributes on the behavior element made optional.  Depending on whether the behavior applies to a transformFile element or div elements in the structMap, only one or the other of the attributes would pertain.
-    5. Documentation aligned with the METS Primer, and corrected.
-    6. xml:lang="en" atttribute value added to every <documentation> element
-    7. xlink:extendedLink support added to the <structLink> element by means of a new <smLinkGrp> element, and its child <smLocatorLink> and <smArcLink> elements.
--->
-<!--February 2010: Version 1.9-->
-<!--Version 1.9 Changes:
-    1. Added a <metsDocumentID> element to the <metsHdr> for recording a unique identifier for the METS document itself where this is different from the OBJID, the identifier for the entire digital object represented by the METS document.
-    2. Added "ISO 19115:2003 NAP" to the enumerated values for the MDTYPE attribute in the METADATA attribute group.
-    3. Added "XPTR" to the enumerated values for the BETYPE attribute on the areaType data type
-    4. Added BEGIN, END and BETYPE attributes to the <file> and <stream> elements for specifying the location of a nested file or a stream within it's parent file.
--->
-<!-- March 2012: Version 1.9.1 -->
-<!-- Version 1.9.1 Changes:
-    1.  Added 'EAC-CPF' as potential metadata scheme to MDTYPE enumeration
-        EAC-CPF = Encoded Archival Context - Corporate Bodies, Persons, and Families 
-        http://eac.staatsbibliothek-berlin.de/eac-cpf-schema.html
--->
-<!-- July 2013: Version 1.10 -->
-<!-- Version 1.10 Changes:
-    1.  Added 'LIDO' as potential metadata scheme to MDTYPE enumeration
-        LIDO = Lightweight Information Describing Objects 
-        http://network.icom.museum/cidoc/working-groups/data-harvesting-and-interchange/lido-technical/specification/
-    2.  Added xsd:anyAttribute with namespace ##other and processContents lax to these METS elements:
-            mets
-                metsHdr
-                dmdSec
-                amdSec
-                    techMD
-                    rightsMD
-                    sourceMD
-                    digiprovMD
-                fileSec
-                    fileGrp
-                        file
-                structMap
-                        fptr
-                structLink
-                behaviorSec
-        This will allow arbitrary new attributes to be added to these elements to support local needs.
--->
-<!-- January 2015: Version 1.10.1 -->
-<!-- Version 1.10.1 Changes:
-    1. Fixed bug:  The anyAttribute declaration was inadvertently added to the FLocat element when it should have been on the file element.  This
-       has been corrected in this version.
--->
-<!-- May 2015: Version 1.11 -->
-<!-- Version 1.11 Changes:
-    1.  Added new attributes, ORDER, ORDERLABEL, and LABEL, to these METS elements:
-            par
-            seq
-            area
-    2.  Also added xsd:anyAttribute with namespace ##other and processContents lax to these elements.  This will allow arbitrary new attributes to be added to these elements to support local needs.   
--->
 <xsd:schema xmlns="http://www.loc.gov/METS/" xmlns:xlink="http://www.w3.org/1999/xlink" xmlns:xsd="http://www.w3.org/2001/XMLSchema" targetNamespace="http://www.loc.gov/METS/" elementFormDefault="qualified" attributeFormDefault="unqualified">
   <xsd:import namespace="http://www.w3.org/1999/xlink" schemaLocation="http://www.loc.gov/standards/xlink/xlink.xsd"/>
+  <xsd:annotation>
+    <xsd:documentation xml:lang="en">METS: Metadata Encoding and Transmission Standard
+
+      This document is available under the Creative Commons CC0 1.0 Universal Public Domain Dedication (http://creativecommons.org/publicdomain/zero/1.0/).
+      The Digital Library Federation, as creator of this document, has waived all rights to it worldwide under copyright law, including
+      all related and neighboring rights, to the extent allowed by law. For the full text see http://creativecommons.org/publicdomain/zero/1.0/legalcode.
+
+      Prepared for the Digital Library Federation by Jerome McDonough, New York University,
+      with the assistance of Michael Alexander (British Library), Joachim Bauer (Content Conversion Specialists, Germany),
+      Rick Beaubien (University of California), Terry Catapano (Columbia University), Morgan Cundiff (Library of Congress),
+      Susan Dahl (University of Alberta), Markus Enders (State and University Library, Göttingen/British Library),
+      Richard Gartner (Bodleian Library at Oxford/King's College, London), Thomas Habing (University of Illinois at Urbana-Champaign),
+      Nancy Hoebelheinrich (Stanford University/Knowledge Motifs LLC), Arwen Hutt (U.C. San Diego),
+      Mark Kornbluh (Michigan State University), Cecilia Preston (Preston &amp; Lynch), Merrilee Proffitt (Research Libraries Group),
+      Clay Redding (Library of Congress), Jenn Riley (Indiana University), Richard Rinehart (Berkeley Art Museum/Pacific Film Archive),
+      Mackenzie Smith (Massachusetts Institute of Technology), Tobias Steinke (German National Library),
+      Taylor Surface (OCLC), Brian Tingle (California Digital Library) and Robin Wendler (Harvard University),
+      Robert Wolfe (Massachusetts Institute of Technology), Patrick Yott (Brown University).
+
+      October, 2019
+      Version 1.12.1</xsd:documentation>
+    <xsd:documentation xml:lang="en">Change History
+
+      April 23, 2001: Alpha Draft completed
+      June 7, 2001: Beta completed
+
+      6/7/2001 Beta Changes:
+
+      1. add 'Time' as a possible time code value, as well as TCF.
+      2. Make dmdSec ID attribute required; make ID attribute optional on MDRef/MDWrap.
+      3. Add 'Label' attribute to StructMap, along with 'Type'.
+      4. Add DDI and FGDC as potential metadata schemes to enumeration.
+      5. Enable an &quot;otherMDtype&quot; attribute for MDWrap/MDRef and any other element where
+          there's an 'other' in the enumerated possibilities.
+      6. Add a &quot;profile&quot; attribute to METS element.
+      7. Revised mptr declaration so that it's like FLocat/MDRef (and not like XLink)
+      8. Extend internal documentation of &lt;area&gt; attributes.
+      9. Add &quot;other&quot; to the possible set of LOCTYPEs.
+      10. Change ADMIDS to ADMID on FileGrp.
+      11. Change &quot;N&quot; to &quot;Order&quot; on &lt;div&gt; element.
+      12. Change &quot;Number&quot; to &quot;order label&quot; on &lt;div&gt; element
+      13. Add createdate and lastmoddate attributes to mets element.
+      14. Allow &lt;div&gt; and &lt;area&gt; elements to link to administrative metadata sections.
+      15. Normalize attribute pointing facilities for file element and mdRef.
+      16. Provide a LOCTYPE of &quot;other&quot; and an &quot;otherloctype&quot; attribute for pointing to external files.
+      17. Drop PDI from enumeration of LOCTYPES.
+      18. Make MDTYPE required in mdRef and mdWrap.
+      19. Rename preservationMD to digiprovMD.
+      20. Add optional CHECKSUM attribute to FContent element.
+      21. Modularize declarations of fileGrpType and mdSecType attributes and enumerations to
+        simplify maintenance.
+      22. Add TYPE attribute to structMap.
+      23. Declare structMap element using structMapType rather than direct declaration.
+      24. Add area element as possible subelement to &lt;div&gt;, along with par and seq.
+      25. Change mdSec model to ALL, to enable differing order of mdRef/mdWrap elements.
+      26. Extend documentation on &lt;par&gt; and &lt;seq&gt; elements.</xsd:documentation>
+    <xsd:documentation xml:lang="en">October 22, 2001: Gamma completed
+
+      10/22/2001 Gamma changes:
+        1. Added optional fileSec element beneath METS root element to contain fileGrps.
+        2. Created subsidiary schema file xlink.xsd for XLink attributes, restored XLink attributes
+        to mptr element, and added XLink support to mdRef and FLocat.
+        3. Created new element metsHdr to handle metadata regarding METS document
+        itself (analogous to TEI Header).  Moved CREATEDATE and LASTMODDATE attributes
+        to metsHdr, and added new RECORDSTATUS attribute.  Added new subsidiary elements
+        agent and altRecordID to metsHdr.
+        4. Made CREATEDATE and LASTMODDATE attributes type xsd:dateTime to allow more precise
+        recording of when work was done.
+        5. Changed all attributes using data type of xsd:binary to xsd:base64Binary to conform to final
+        W3C schema recommendations.
+        6. Cleaned up annotations/documentation.</xsd:documentation>
+    <xsd:documentation xml:lang="en">December 19, 2001: Epsilon and PROTOFINAL completed
+
+       12/19/2001 Epsilon changes:
+
+       1. Changed sequence operator for StructMap so that only 1 root div element is permitted.
+       2. Add new roles to agent element's role attribute and support for extensible 'other' role.
+       3. Add support for extensible 'other' type attribute on agent element.
+       4. Yet more documentation clean up.
+       5. Relocate CHECKSUM attribute from FContent to File element.
+       6. Change the file element's CREATED attribute and fileGroup's VERSDATE attribute to
+       a type of xsd:dateTime
+       7. Change attribute name DMD for div element to DMDID for consistency's sake.
+       8. Added new behaviorSec for support of referencing executable code from METS object</xsd:documentation>
+    <xsd:documentation xml:lang="en">February 8, 2002: Zeta bug fix to final
+
+       2/8/2002 Zeta changes
+
+       1. Eliminated redundant VRA in metadata type enumeration.
+       2. Changed mdWrap content model, adding xmlData element to eliminate
+         ambiguous content model</xsd:documentation>
+    <xsd:documentation xml:lang="en">June 3, 2002: Version 1.1
+
+      6/3/2002 v1.1 changes:
+
+      1. Add new structLink section for recording hyperlinks between media represented by structMap nodes.
+      2. Allow a &lt;par&gt; element to contain a &lt;seq&gt;</xsd:documentation>
+    <xsd:documentation xml:lang="en">Dec. 27, 2002: Version 1.2
+
+      12/27/2002 v1.2 changes:
+      1. Add “USE” attribute to FileGrp, File, FLocat and FContent;
+      2. Make FLocat repeatable;
+      3. Have FContent mimic mdWrap in using separate binData/xmlData sections;
+      4. Copyright statement added;
+      5. Allow both FLocat and Fcontent in single file element;
+      6. Allow behaviorSec elements to group through GROUPID attribute;
+      7. allow descriptive and administrative metadata sections to be grouped through GROUPID attribute;
+      8. allow &lt;file&gt; element to point to descriptive metadata via DMDID attribute;
+      9. allow descriptive metadata and all forms of administrative metadata to point to administrative metadata via ADMID attribute;
+      10. CREATED and STATUS attributes added to all desc. and adm. metadata sections; and
+      11. clean up documentation in elements to reflect reality.</xsd:documentation>
+    <xsd:documentation xml:lang="en">May 8, 2003: Version 1.3
+
+      05/05/2003 v1.3 changes:
+
+      1. Change “2. OBJID: a primary identifier assigned to the original source document” to “2. OBJID: a primary identifier assigned to the METS object.”
+      2. Add MODS to MDTYPEs.
+      3. Modify &lt;file&gt; attributes so that instead of just CHECKSUM we have CHECKSUM and CHECKSUMTYPE, where CHECKSUMTYPE is a controlled vocabulary as follows:
+      HAVAL, MD5, SHA-1, SHA-256, SHA-384, SHA-512, TIGER, WHIRLPOOL
+      4.Alter BehaviorSec to make it recursive, and add a new behavior element to wrap mechanism and interfaceDef elements.</xsd:documentation>
+    <xsd:documentation xml:lang="en">May 1, 2004: Version 1.4
+
+      05/01/2003 v1.4 changes:
+
+      1. Moved attribute documentation out of element documentation
+      (thank you, Brian Tingle).
+      2. New CONTENTIDS attribute (and URIs simpleType) added to div, fptr,
+      mptr and area elements for mapping MPEG21 DII Identifier values
+      3. XLink namespace URI changed to conform with XLink recommendation.
+      4. ID Attribute added to FContent.
+      5. ID Attribute addedt to structLink.
+      6. ID Attribute added to smLink.
+      7. &quot;LOM&quot; added as metadata type.</xsd:documentation>
+    <xsd:documentation xml:lang="en">April 12, 2005: Version 1.5
+
+      04/12/2005 v1.5 changes:
+
+      1. Made file element recursive to deal with PREMIS Onion Layer model and
+      support XFDU-ish unpacking specification.
+      2. Add &lt;stream&gt; element beneath &lt;file&gt; to allow linking of metadata to
+      subfile structures.
+      3. Modify structLink TO and FROM attributes to put them in XLink namespace.
+      4. Make processContents &quot;lax&quot; for all xsd:any elements.</xsd:documentation>
+    <xsd:documentation xml:lang="en">October 18, 2006: Version 1.6
+
+      10/18/2006 v1.6 changes:
+
+      1. add ID to stream and transformFile
+      2. add ADMID to metsHdr
+      3. make smLink/@xlink:to and smLink/@xlink:from required</xsd:documentation>
+    <xsd:documentation xml:lang="en">October 16, 2007/ Jan 20, 2008: Version 1.7
+
+      10/16/2007 01/30/2008  v 1.7 changes:
+
+      1. create parType complex type to allow a seq to contain a par
+      2. create FILECORE attribute group with MIMETYPE, SIZE, CHECKSUM, CHECKSUMTYPE;
+      change fileType, mdWrapType and mdRefType use the attribute group, so mdType and mdRef end
+      up with new SIZE, CHECKSUM, and CHECKSUMTYPE attributes (file does not change)
+      20080130
+      2a. CREATED added to FILECORE
+      3. PREMIS:OBJECT PREMIS:AGENT PREMIS:RIGHTS PREMIS:EVENT added to MDTYPE value enumeration</xsd:documentation>
+    <xsd:documentation xml:lang="en">April 2009: Version 1.8
+
+      Version 1.8 changes:
+      1. Add CRC32, Adler-32, MNP to the enumerated values constraining CHECKSUMTYPE to align with MIX messageDigestAlgorithm constraints.
+      2. Add TEXTMD and METSRIGHTS to the enumeration values constraining MDTYPE.
+      3. Add an MDTYPEVERSION attribute as a companion to the MDTYPE attribute in the mdRef and mdWrap elements.	
+      4. ID and STRUCTID attributes on the behavior element made optional.  Depending on whether the behavior applies to a transformFile element or div elements in the structMap, only one or the other of the attributes would pertain.
+      5. Documentation aligned with the METS Primer, and corrected.
+      6. xml:lang=&quot;en&quot; atttribute value added to every &lt;documentation&gt; element
+      7. xlink:extendedLink support added to the &lt;structLink&gt; element by means of a new &lt;smLinkGrp&gt; element, and its child &lt;smLocatorLink&gt; and &lt;smArcLink&gt; elements.</xsd:documentation>
+    <xsd:documentation xml:lang="en">2010: Version 1.9
+
+      Version 1.9 Changes:
+      1. Added a &lt;metsDocumentID&gt; element to the &lt;metsHdr&gt; for recording a unique identifier for the METS document itself where this is different from the OBJID, the identifier for the entire digital object represented by the METS document.
+      2. Added &quot;ISO 19115:2003 NAP&quot; to the enumerated values for the MDTYPE attribute in the METADATA attribute group.
+      3. Added &quot;XPTR&quot; to the enumerated values for the BETYPE attribute on the areaType data type
+      4. Added BEGIN, END and BETYPE attributes to the &lt;file&gt; and &lt;stream&gt; elements for specifying the location of a nested file or a stream within it's parent file.</xsd:documentation>
+    <xsd:documentation xml:lang="en">March 2012: Version 1.9.1
+
+      Version 1.9.1 Changes:
+      1.  Added 'EAC-CPF' as potential metadata scheme to MDTYPE enumeration
+      EAC-CPF = Encoded Archival Context - Corporate Bodies, Persons, and Families
+      http://eac.staatsbibliothek-berlin.de/eac-cpf-schema.html</xsd:documentation>
+    <xsd:documentation xml:lang="en">July 2013: Version 1.10
+
+       Version 1.10 Changes:
+         1.	Added 'LIDO' as potential metadata scheme to MDTYPE enumeration
+           LIDO = Lightweight Information Describing Objects
+           http://network.icom.museum/cidoc/working-groups/data-harvesting-and-interchange/lido-technical/specification/
+         2.	Added xsd:anyAttribute with namespace ##other and processContents lax to these METS elements:
+             mets
+               metsHdr
+               dmdSec
+               amdSec
+                 techMD
+                 rightsMD
+                 sourceMD
+                 digiprovMD
+               fileSec
+                 fileGrp
+                   file
+               structMap
+                   fptr
+               structLink
+               behaviorSec
+           This will allow arbitrary new attributes to be added to these elements to support local needs.</xsd:documentation>
+    <xsd:documentation xml:lang="en">January 2015: Version 1.10.1
+
+       Version 1.10.1 Changes:
+         1. Fixed bug:  The anyAttribute declaration was inadvertently added to the FLocat element when it should have been on the file element.  This
+            has been corrected in this version.</xsd:documentation>
+    <xsd:documentation xml:lang="en">May 2015: Version 1.11
+
+       Version 1.11 Changes:
+         1.	Added new attributes, ORDER, ORDERLABEL, and LABEL, to these METS elements:
+             par
+             seq
+             area
+         2.	Also added xsd:anyAttribute with namespace ##other and processContents lax to these elements.  This will allow arbitrary new attributes to be added to these elements to support local needs.</xsd:documentation>
+    <xsd:documentation xml:lang="en">May 2018: Version 1.12
+
+        Version 1.12 Changes:
+
+        1.	Added xsd:anyAttribute with namespace ##other and processContents lax to these elements:
+        agent/note
+
+        This will allow arbitrary new attributes to be added to this element to support local needs.  The original use case was to identify the type of the note.</xsd:documentation>
+    <xsd:documentation xml:lang="en">October 2019: Version 1.12.1
+
+	Version 1.12.1 Changes:
+
+	1. Move comments with version history to xsd:documentation elements
+
+	This allows tools that generate documentation from schemas to include the change history in the generated documentation.</xsd:documentation>
+  </xsd:annotation>
   <xsd:element name="mets">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">METS: Metadata Encoding and Transmission Standard.
-                METS is intended to provide a standardized XML format for transmission of complex digital library objects between systems.  As such, it can be seen as filling a role similar to that defined for the Submission Information Package (SIP), Archival Information Package (AIP) and Dissemination Information Package (DIP) in the Reference Model for an Open Archival Information System. The root element &lt;mets&gt; establishes the container for the information being stored and/or transmitted by the standard.</xsd:documentation>
+				METS is intended to provide a standardized XML format for transmission of complex digital library objects between systems.  As such, it can be seen as filling a role similar to that defined for the Submission Information Package (SIP), Archival Information Package (AIP) and Dissemination Information Package (DIP) in the Reference Model for an Open Archival Information System. The root element &lt;mets&gt; establishes the container for the information being stored and/or transmitted by the standard.</xsd:documentation>
     </xsd:annotation>
     <xsd:complexType>
       <xsd:complexContent>
         <xsd:extension base="metsType"/>
       </xsd:complexContent>
     </xsd:complexType>
   </xsd:element>
   <xsd:complexType name="metsType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">metsType: Complex Type for METS Sections
-            A METS document consists of seven possible subsidiary sections: metsHdr (METS document header), dmdSec (descriptive metadata section), amdSec (administrative metadata section), fileGrp (file inventory group), structLink (structural map linking), structMap (structural map) and behaviorSec (behaviors section).</xsd:documentation>
+			A METS document consists of seven possible subsidiary sections: metsHdr (METS document header), dmdSec (descriptive metadata section), amdSec (administrative metadata section), fileGrp (file inventory group), structLink (structural map linking), structMap (structural map) and behaviorSec (behaviors section).</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="metsHdr" minOccurs="0">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The mets header element &lt;metsHdr&gt; captures metadata about the METS document itself, not the digital object the METS document encodes. Although it records a more limited set of metadata, it is very similar in function and purpose to the headers employed in other schema such as the Text Encoding Initiative (TEI) or in the Encoded Archival Description (EAD).</xsd:documentation>
         </xsd:annotation>
         <xsd:complexType>
           <xsd:sequence>
             <xsd:element name="agent" minOccurs="0" maxOccurs="unbounded">
               <xsd:annotation>
                 <xsd:documentation xml:lang="en">agent: 
-                                The agent element &lt;agent&gt; provides for various parties and their roles with respect to the METS record to be documented.</xsd:documentation>
+								The agent element &lt;agent&gt; provides for various parties and their roles with respect to the METS record to be documented.</xsd:documentation>
               </xsd:annotation>
               <xsd:complexType>
                 <xsd:sequence>
                   <xsd:element name="name" type="xsd:string">
                     <xsd:annotation>
                       <xsd:documentation xml:lang="en">The element &lt;name&gt; can be used to record the full name of the document agent.</xsd:documentation>
                     </xsd:annotation>
                   </xsd:element>
-                  <xsd:element name="note" type="xsd:string" minOccurs="0" maxOccurs="unbounded">
+                  <xsd:element name="note" minOccurs="0" maxOccurs="unbounded">
                     <xsd:annotation>
                       <xsd:documentation xml:lang="en">The &lt;note&gt; element can be used to record any additional information regarding the agent's activities with respect to the METS document.</xsd:documentation>
                     </xsd:annotation>
+                    <xsd:complexType>
+                      <xsd:simpleContent>
+                        <xsd:extension base="xsd:string">
+                          <xsd:anyAttribute namespace="##other" processContents="lax"/>
+                        </xsd:extension>
+                      </xsd:simpleContent>
+                    </xsd:complexType>
                   </xsd:element>
                 </xsd:sequence>
                 <xsd:attribute name="ID" type="xsd:ID" use="optional">
                   <xsd:annotation>
                     <xsd:documentation xml:lang="en">ID (ID/O): This attribute uniquely identifies the element within the METS document, and would allow the element to be referenced unambiguously from another element or document via an IDREF or an XPTR. For more information on using ID attributes for internal and external linking see Chapter 4 of the METS Primer.</xsd:documentation>
                   </xsd:annotation>
                 </xsd:attribute>
@@ -477,15 +503,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="amdSecType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">amdSecType: Complex Type for Administrative Metadata Sections
-            The administrative metadata section consists of four possible subsidiary sections: techMD (technical metadata for text/image/audio/video files), rightsMD (intellectual property rights metadata), sourceMD (analog/digital source metadata), and digiprovMD (digital provenance metadata, that is, the history of migrations/translations performed on a digital library object from it's original digital capture/encoding).</xsd:documentation>
+			The administrative metadata section consists of four possible subsidiary sections: techMD (technical metadata for text/image/audio/video files), rightsMD (intellectual property rights metadata), sourceMD (analog/digital source metadata), and digiprovMD (digital provenance metadata, that is, the history of migrations/translations performed on a digital library object from it's original digital capture/encoding).</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="techMD" type="mdSecType" minOccurs="0" maxOccurs="unbounded">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">A technical metadata element &lt;techMD&gt; records technical metadata about a component of the METS object, such as a digital content file. The &lt;techMD&gt; element conforms to same generic datatype as the &lt;dmdSec&gt;, &lt;rightsMD&gt;, &lt;sourceMD&gt; and &lt;digiprovMD&gt; elements, and supports the same sub-elements and attributes.  A technical metadata element can either wrap the metadata  (mdWrap) or reference it in an external location (mdRef) or both.  METS allows multiple &lt;techMD&gt; elements; and technical metadata can be associated with any METS element that supports an ADMID attribute. Technical metadata can be expressed according to many current technical description standards (such as MIX and textMD) or a locally produced XML schema.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
@@ -511,15 +537,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="fileGrpType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">fileGrpType: Complex Type for File Groups
-                The file group is used to cluster all of the digital files composing a digital library object in a hierarchical arrangement (fileGrp is recursively defined to enable the creation of the hierarchy).  Any file group may contain zero or more file elements.  File elements in turn can contain one or more FLocat elements (a pointer to a file containing content for this object) and/or a FContent element (the contents of the file, in either XML or  Base64 encoding).</xsd:documentation>
+				The file group is used to cluster all of the digital files composing a digital library object in a hierarchical arrangement (fileGrp is recursively defined to enable the creation of the hierarchy).  Any file group may contain zero or more file elements.  File elements in turn can contain one or more FLocat elements (a pointer to a file containing content for this object) and/or a FContent element (the contents of the file, in either XML or  Base64 encoding).</xsd:documentation>
     </xsd:annotation>
     <xsd:choice>
       <xsd:element name="fileGrp" type="fileGrpType" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="file" minOccurs="0" maxOccurs="unbounded" type="fileType">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The file element &lt;file&gt; provides access to the content files for the digital object being described by the METS document. A &lt;file&gt; element may contain one or more &lt;FLocat&gt; elements which provide pointers to a content file and/or a &lt;FContent&gt; element which wraps an encoded version of the file. Embedding files using &lt;FContent&gt; can be a valuable feature for exchanging digital objects between repositories or for archiving versions of digital objects for off-site storage. All &lt;FLocat&gt; and &lt;FContent&gt; elements should identify and/or contain identical copies of a single file. The &lt;file&gt; element is recursive, thus allowing sub-files or component files of a larger file to be listed in the inventory. Alternatively, by using the &lt;stream&gt; element, a smaller component of a file or of a related file can be placed within a &lt;file&gt; element. Finally, by using the &lt;transformFile&gt; element, it is possible to include within a &lt;file&gt; element a different version of a file that has undergone a transformation for some reason, such as format migration.</xsd:documentation>
         </xsd:annotation>
@@ -546,15 +572,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="structMapType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">structMapType: Complex Type for Structural Maps
-            The structural map (structMap) outlines a hierarchical structure for the original object being encoded, using a series of nested div elements.</xsd:documentation>
+			The structural map (structMap) outlines a hierarchical structure for the original object being encoded, using a series of nested div elements.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="div" type="divType">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The structural divisions of the hierarchical organization provided by a &lt;structMap&gt; are represented by division &lt;div&gt; elements, which can be nested to any depth. Each &lt;div&gt; element can represent either an intellectual (logical) division or a physical division. Every &lt;div&gt; node in the structural map hierarchy may be connected (via subsidiary &lt;mptr&gt; or &lt;fptr&gt; elements) to content files which represent that div's portion of the whole document.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
@@ -575,15 +601,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="divType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">divType: Complex Type for Divisions
-                    The METS standard represents a document structurally as a series of nested div elements, that is, as a hierarchy (e.g., a book, which is composed of chapters, which are composed of subchapters, which are composed of text).  Every div node in the structural map hierarchy may be connected (via subsidiary mptr or fptr elements) to content files which represent that div's portion of the whole document.
+					The METS standard represents a document structurally as a series of nested div elements, that is, as a hierarchy (e.g., a book, which is composed of chapters, which are composed of subchapters, which are composed of text).  Every div node in the structural map hierarchy may be connected (via subsidiary mptr or fptr elements) to content files which represent that div's portion of the whole document.
 
 SPECIAL NOTE REGARDING DIV ATTRIBUTE VALUES:
 to clarify the differences between the ORDER, ORDERLABEL, and LABEL attributes for the &lt;div&gt; element, imagine a text with 10 roman numbered pages followed by 10 arabic numbered pages. Page iii would have an ORDER of &quot;3&quot;, an ORDERLABEL of &quot;iii&quot; and a LABEL of &quot;Page iii&quot;, while page 3 would have an ORDER of &quot;13&quot;, an ORDERLABEL of &quot;3&quot; and a LABEL of &quot;Page 3&quot;.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="mptr" minOccurs="0" maxOccurs="unbounded">
         <xsd:annotation>
@@ -677,15 +703,15 @@
         <xsd:documentation xml:lang="en">xlink:label - an xlink label to be referred to by an smLink element</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
   </xsd:complexType>
   <xsd:complexType name="parType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">parType: Complex Type for Parallel Files
-                The &lt;par&gt; or parallel files element aggregates pointers to files, parts of files, and/or sequences of files or parts of files that must be played or displayed simultaneously to manifest a block of digital content represented by an &lt;fptr&gt; element.</xsd:documentation>
+				The &lt;par&gt; or parallel files element aggregates pointers to files, parts of files, and/or sequences of files or parts of files that must be played or displayed simultaneously to manifest a block of digital content represented by an &lt;fptr&gt; element.</xsd:documentation>
     </xsd:annotation>
     <xsd:choice maxOccurs="unbounded">
       <xsd:element name="area" type="areaType" minOccurs="0"/>
       <xsd:element name="seq" type="seqType" minOccurs="0"/>
     </xsd:choice>
     <xsd:attribute name="ID" type="xsd:ID" use="optional">
       <xsd:annotation>
@@ -694,15 +720,15 @@
     </xsd:attribute>
     <xsd:attributeGroup ref="ORDERLABELS"/>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="seqType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">seqType: Complex Type for Sequences of Files
-                    The seq element should be used to link a div to a set of content files when those files should be played/displayed sequentially to deliver content to a user.  Individual &lt;area&gt; subelements within the seq element provide the links to the files or portions thereof.</xsd:documentation>
+					The seq element should be used to link a div to a set of content files when those files should be played/displayed sequentially to deliver content to a user.  Individual &lt;area&gt; subelements within the seq element provide the links to the files or portions thereof.</xsd:documentation>
     </xsd:annotation>
     <xsd:choice maxOccurs="unbounded">
       <xsd:element name="area" type="areaType" minOccurs="0"/>
       <xsd:element name="par" type="parType" minOccurs="0"/>
     </xsd:choice>
     <xsd:attribute name="ID" type="xsd:ID" use="optional">
       <xsd:annotation>
@@ -711,15 +737,15 @@
     </xsd:attribute>
     <xsd:attributeGroup ref="ORDERLABELS"/>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="areaType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">areaType: Complex Type for Area Linking
-                The area element provides for more sophisticated linking between a div element and content files representing that div, be they text, image, audio, or video files.  An area element can link a div to a point within a file, to a one-dimension segment of a file (e.g., text segment, image line, audio/video clip), or a two-dimensional section of a file   (e.g, subsection of an image, or a subsection of the  video display of a video file.  The area element has no content; all information is recorded within its various attributes.</xsd:documentation>
+				The area element provides for more sophisticated linking between a div element and content files representing that div, be they text, image, audio, or video files.  An area element can link a div to a point within a file, to a one-dimension segment of a file (e.g., text segment, image line, audio/video clip), or a two-dimensional section of a file 	(e.g, subsection of an image, or a subsection of the  video display of a video file.  The area element has no content; all information is recorded within its various attributes.</xsd:documentation>
     </xsd:annotation>
     <xsd:attribute name="ID" type="xsd:ID" use="optional">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">ID (ID/O): This attribute uniquely identifies the element within the METS document, and would allow the element to be referenced unambiguously from another element or document via an IDREF or an XPTR. For more information on using ID attributes for internal and external linking see Chapter 4 of the METS Primer.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
     <xsd:attribute name="FILEID" type="xsd:IDREF" use="required">
@@ -756,15 +782,15 @@
       <xsd:annotation>
         <xsd:documentation xml:lang="en">END (string/O): An attribute that specifies the point in the content file where the relevant section of content ends. It can only be interpreted meaningfully in conjunction with the BETYPE, which specifies the kind of ending point values being used. Typically the END attribute would only appear in conjunction with a BEGIN element.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
     <xsd:attribute name="BETYPE" use="optional">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">BETYPE: Begin/End Type.
-                    BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. For example, if BYTE is specified, then the BEGIN and END point values represent the byte offsets into a file. If IDREF is specified, then the BEGIN element specifies the ID value that identifies the element in a structured text file where the relevant section of the file begins; and the END value (if present) would specify the ID value that identifies the element with which the relevant section of the file ends. Must be one of the following values: 
+					BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. For example, if BYTE is specified, then the BEGIN and END point values represent the byte offsets into a file. If IDREF is specified, then the BEGIN element specifies the ID value that identifies the element in a structured text file where the relevant section of the file begins; and the END value (if present) would specify the ID value that identifies the element with which the relevant section of the file ends. Must be one of the following values: 
 BYTE
 IDREF
 SMIL
 MIDI
 SMPTE-25
 SMPTE-24
 SMPTE-DF30
@@ -841,15 +867,15 @@
     </xsd:attribute>
     <xsd:attributeGroup ref="ORDERLABELS"/>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="structLinkType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">structLinkType: Complex Type for Structural Map Linking
-                The Structural Map Linking section allows for the specification of hyperlinks between different components of a METS structure delineated in a structural map.  structLink contains a single, repeatable element, smLink.  Each smLink element indicates a hyperlink between two nodes in the structMap.  The structMap nodes recorded in smLink are identified using their XML ID attribute    values.</xsd:documentation>
+				The Structural Map Linking section allows for the specification of hyperlinks between different components of a METS structure delineated in a structural map.  structLink contains a single, repeatable element, smLink.  Each smLink element indicates a hyperlink between two nodes in the structMap.  The structMap nodes recorded in smLink are identified using their XML ID attribute	values.</xsd:documentation>
     </xsd:annotation>
     <xsd:choice maxOccurs="unbounded">
       <xsd:element name="smLink">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The Structural Map Link element &lt;smLink&gt; identifies a hyperlink between two nodes in the structural map. You would use &lt;smLink&gt;, for instance, to note the existence of hypertext links between web pages, if you wished to record those links within METS. NOTE: &lt;smLink&gt; is an empty element. The location of the &lt;smLink&gt; element to which the &lt;smLink&gt; element is pointing MUST be stored in the xlink:href attribute.</xsd:documentation>
         </xsd:annotation>
         <xsd:complexType>
@@ -955,15 +981,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="behaviorSecType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">behaviorSecType: Complex Type for Behavior Sections
-            Behaviors are executable code which can be associated with parts of a METS object.  The behaviorSec element is used to group individual behaviors within a hierarchical structure.  Such grouping can be useful to organize families of behaviors together or to indicate other relationships between particular behaviors.</xsd:documentation>
+			Behaviors are executable code which can be associated with parts of a METS object.  The behaviorSec element is used to group individual behaviors within a hierarchical structure.  Such grouping can be useful to organize families of behaviors together or to indicate other relationships between particular behaviors.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="behaviorSec" type="behaviorSecType" minOccurs="0" maxOccurs="unbounded"/>
       <xsd:element name="behavior" type="behaviorType" minOccurs="0" maxOccurs="unbounded">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">A behavior element &lt;behavior&gt; can be used to associate executable behaviors with content in the METS document. This element has an interface definition &lt;interfaceDef&gt; element that represents an abstract definition of a set of behaviors represented by a particular behavior. A &lt;behavior&gt; element also has a behavior mechanism &lt;mechanism&gt; element, a module of executable code that implements and runs the behavior defined abstractly by the interface definition.</xsd:documentation>
         </xsd:annotation>
@@ -985,15 +1011,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="behaviorType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">behaviorType: Complex Type for Behaviors
-             A behavior can be used to associate executable behaviors with content in the METS object.  A behavior element has an interface definition element that represents an abstract definition  of the set  of behaviors represented by a particular behavior.  A behavior element also has an behavior  mechanism which is a module of executable code that implements and runs the behavior defined abstractly by the interface definition.</xsd:documentation>
+			 A behavior can be used to associate executable behaviors with content in the METS object.  A behavior element has an interface definition element that represents an abstract definition  of the set  of behaviors represented by a particular behavior.  A behavior element also has an behavior  mechanism which is a module of executable code that implements and runs the behavior defined abstractly by the interface definition.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="interfaceDef" type="objectType" minOccurs="0">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The interface definition &lt;interfaceDef&gt; element contains a pointer to an abstract definition of a single behavior or a set of related behaviors that are associated with the content of a METS object. The interface definition object to which the &lt;interfaceDef&gt; element points using xlink:href could be another digital object, or some other entity, such as a text file which describes the interface or a Web Services Description Language (WSDL) file. Ideally, an interface definition object contains metadata that describes a set of behaviors or methods. It may also contain files that describe the intended usage of the behaviors, and possibly files that represent different expressions of the interface definition.</xsd:documentation>
         </xsd:annotation>
       </xsd:element>
@@ -1038,15 +1064,15 @@
         <xsd:documentation xml:lang="en">ADMID (IDREFS/O): An optional attribute listing the XML ID values of administrative metadata sections within the METS document pertaining to this behavior.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
   </xsd:complexType>
   <xsd:complexType name="objectType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">objectType: complexType for interfaceDef and mechanism elements
-                The mechanism and behavior elements point to external objects--an interface definition object or an executable code object respectively--which together constitute a behavior that can be applied to one or more &lt;div&gt; elements in a &lt;structMap&gt;.</xsd:documentation>
+				The mechanism and behavior elements point to external objects--an interface definition object or an executable code object respectively--which together constitute a behavior that can be applied to one or more &lt;div&gt; elements in a &lt;structMap&gt;.</xsd:documentation>
     </xsd:annotation>
     <xsd:attribute name="ID" type="xsd:ID" use="optional">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">ID (ID/O): This attribute uniquely identifies the element within the METS document, and would allow the element to be referenced unambiguously from another element or document via an IDREF or an XPTR. For more information on using ID attributes for internal and external linking see Chapter 4 of the METS Primer.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
     <xsd:attribute name="LABEL" type="xsd:string" use="optional">
@@ -1056,15 +1082,15 @@
     </xsd:attribute>
     <xsd:attributeGroup ref="LOCATION"/>
     <xsd:attributeGroup ref="xlink:simpleLink"/>
   </xsd:complexType>
   <xsd:complexType name="mdSecType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">mdSecType: Complex Type for Metadata Sections
-            A generic framework for pointing to/including metadata within a METS document, a la Warwick Framework.</xsd:documentation>
+			A generic framework for pointing to/including metadata within a METS document, a la Warwick Framework.</xsd:documentation>
     </xsd:annotation>
     <xsd:all>
       <xsd:element name="mdRef" minOccurs="0">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The metadata reference element &lt;mdRef&gt; element is a generic element used throughout the METS schema to provide a pointer to metadata which resides outside the METS document.  NB: &lt;mdRef&gt; is an empty element.  The location of the metadata must be recorded in the xlink:href attribute, supplemented by the XPTR attribute as needed.</xsd:documentation>
         </xsd:annotation>
         <xsd:complexType>
@@ -1152,15 +1178,15 @@
       </xsd:annotation>
     </xsd:attribute>
     <xsd:anyAttribute namespace="##other" processContents="lax"/>
   </xsd:complexType>
   <xsd:complexType name="fileType">
     <xsd:annotation>
       <xsd:documentation xml:lang="en">fileType: Complex Type for Files
-                The file element provides access to content files for a METS object.  A file element may contain one or more FLocat elements, which provide pointers to a content file, and/or an FContent element, which wraps an encoded version of the file. Note that ALL FLocat and FContent elements underneath a single file element should identify/contain identical copies of a single file.</xsd:documentation>
+				The file element provides access to content files for a METS object.  A file element may contain one or more FLocat elements, which provide pointers to a content file, and/or an FContent element, which wraps an encoded version of the file. Note that ALL FLocat and FContent elements underneath a single file element should identify/contain identical copies of a single file.</xsd:documentation>
     </xsd:annotation>
     <xsd:sequence>
       <xsd:element name="FLocat" minOccurs="0" maxOccurs="unbounded">
         <xsd:annotation>
           <xsd:documentation xml:lang="en">The file location element &lt;FLocat&gt; provides a pointer to the location of a content file. It uses the XLink reference syntax to provide linking information indicating the actual location of the content file, along with other attributes specifying additional linking information. NOTE: &lt;FLocat&gt; is an empty element. The location of the resource pointed to MUST be stored in the xlink:href attribute.</xsd:documentation>
         </xsd:annotation>
         <xsd:complexType>
@@ -1253,15 +1279,15 @@
                 <xsd:annotation>
                   <xsd:documentation xml:lang="en">END (string/O): An attribute that specifies the point in the parent &lt;file&gt; where the &lt;stream&gt; ends. It can only be interpreted meaningfully in conjunction with the BETYPE, which specifies the kind of ending point values being used. Typically the END attribute would only appear in conjunction with a BEGIN attribute.</xsd:documentation>
                 </xsd:annotation>
               </xsd:attribute>
               <xsd:attribute name="BETYPE" use="optional">
                 <xsd:annotation>
                   <xsd:documentation xml:lang="en">BETYPE: Begin/End Type.
-                                        BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. Currently BYTE is the only valid value that can be used in conjunction with nested &lt;file&gt; or &lt;stream&gt; elements.</xsd:documentation>
+										BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. Currently BYTE is the only valid value that can be used in conjunction with nested &lt;file&gt; or &lt;stream&gt; elements.</xsd:documentation>
                 </xsd:annotation>
                 <xsd:simpleType>
                   <xsd:restriction base="xsd:string">
                     <xsd:enumeration value="BYTE"/>
                   </xsd:restriction>
                 </xsd:simpleType>
               </xsd:attribute>
@@ -1363,15 +1389,15 @@
       <xsd:annotation>
         <xsd:documentation xml:lang="en">END (string/O): An attribute that specifies the point in the parent &lt;file&gt; where the current, nested &lt;file&gt; ends. It can only be interpreted meaningfully in conjunction with the BETYPE, which specifies the kind of ending point values being used. Typically the END attribute would only appear in conjunction with a BEGIN attribute.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
     <xsd:attribute name="BETYPE" use="optional">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">BETYPE: Begin/End Type.
-                    BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. Currently BYTE is the only valid value that can be used in conjunction with nested &lt;file&gt; or &lt;stream&gt; elements.</xsd:documentation>
+					BETYPE (string/O): An attribute that specifies the kind of BEGIN and/or END values that are being used. Currently BYTE is the only valid value that can be used in conjunction with nested &lt;file&gt; or &lt;stream&gt; elements.</xsd:documentation>
       </xsd:annotation>
       <xsd:simpleType>
         <xsd:restriction base="xsd:string">
           <xsd:enumeration value="BYTE"/>
         </xsd:restriction>
       </xsd:simpleType>
     </xsd:attribute>
@@ -1462,21 +1488,21 @@
       </xsd:annotation>
     </xsd:attribute>
   </xsd:attributeGroup>
   <xsd:attributeGroup name="LOCATION">
     <xsd:attribute name="LOCTYPE" use="required">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">LOCTYPE (string/R): Specifies the locator type used in the xlink:href attribute. Valid values for LOCTYPE are: 
-                    ARK
-                    URN
-                    URL
-                    PURL
-                    HANDLE
-                    DOI
-                    OTHER</xsd:documentation>
+					ARK
+					URN
+					URL
+					PURL
+					HANDLE
+					DOI
+					OTHER</xsd:documentation>
       </xsd:annotation>
       <xsd:simpleType>
         <xsd:restriction base="xsd:string">
           <xsd:enumeration value="ARK"/>
           <xsd:enumeration value="URN"/>
           <xsd:enumeration value="URL"/>
           <xsd:enumeration value="PURL"/>
@@ -1512,25 +1538,25 @@
       <xsd:annotation>
         <xsd:documentation xml:lang="en">CHECKSUM (string/O): Provides a checksum value for the associated file or wrapped content.</xsd:documentation>
       </xsd:annotation>
     </xsd:attribute>
     <xsd:attribute name="CHECKSUMTYPE" use="optional">
       <xsd:annotation>
         <xsd:documentation xml:lang="en">CHECKSUMTYPE (enumerated string/O): Specifies the checksum algorithm used to produce the value contained in the CHECKSUM attribute.  CHECKSUMTYPE must contain one of the following values:
-                    Adler-32
-                    CRC32
-                    HAVAL
-                    MD5
-                    MNP
-                    SHA-1
-                    SHA-256
-                    SHA-384
-                    SHA-512
-                    TIGER
-                    WHIRLPOOL</xsd:documentation>
+					Adler-32
+					CRC32
+					HAVAL
+					MD5
+					MNP
+					SHA-1
+					SHA-256
+					SHA-384
+					SHA-512
+					TIGER
+					WHIRLPOOL</xsd:documentation>
       </xsd:annotation>
       <xsd:simpleType>
         <xsd:restriction base="xsd:string">
           <xsd:enumeration value="Adler-32"/>
           <xsd:enumeration value="CRC32"/>
           <xsd:enumeration value="HAVAL"/>
           <xsd:enumeration value="MD5"/>
```

### Comparing `metsrw-0.3.9/metsrw/resources/archivematica_mets_schematron.xml` & `metsrw-0.4.0/metsrw/resources/archivematica_mets_schematron.xml`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.9/metsrw/resources/archivematica_mets_pointer_file_schematron.xml` & `metsrw-0.4.0/metsrw/resources/archivematica_mets_pointer_file_schematron.xml`

 * *Files identical despite different names*

### Comparing `metsrw-0.3.9/metsrw/fsentry.py` & `metsrw-0.4.0/metsrw/fsentry.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-# -*- coding: utf-8 -*-
-from __future__ import absolute_import
-
-from itertools import chain
 import logging
 import os
+from itertools import chain
+from uuid import uuid4
 
 from lxml import etree
-import six
 
-from .di import (
-    is_class,
-    has_methods,
-    has_class_methods,
-    Dependency,
-    DependencyPossessor,
-)
 from . import exceptions
-from .metadata import MDWrap, MDRef, SubSection, AMDSec
 from . import utils
+from .di import Dependency
+from .di import DependencyPossessor
+from .di import has_class_methods
+from .di import has_methods
+from .di import is_class
+from .metadata import AMDSec
+from .metadata import MDRef
+from .metadata import MDWrap
+from .metadata import SubSection
 
 LOGGER = logging.getLogger(__name__)
 
 
 class FSEntry(DependencyPossessor):
     """A class representing a filesystem entry - either a file or a directory.
 
@@ -117,42 +115,33 @@
 
     def __init__(
         self,
         path=None,
         fileid=None,
         label=None,
         use="original",
-        type=u"Item",
+        type="Item",
         children=None,
         file_uuid=None,
         derived_from=None,
         checksum=None,
         checksumtype=None,
         transform_files=None,
         mets_div_type=None,
     ):
-        # path can validly be any encoding; if this value needs
-        # to be spliced later on, it's better to treat it as a
-        # bytestring than as actually being encoded text.
-        if six.PY2:
-            if isinstance(path, six.text_type):
-                self.path = path.encode("utf-8")
-            else:
-                self.path = path
-        else:  # TODO: Py3 is still using Unicode.
-            if isinstance(path, six.binary_type):
-                self.path = path.decode("utf-8", errors="strict")
-            else:
-                self.path = path
+        if isinstance(path, bytes):
+            self.path = path.decode("utf-8", errors="strict")
+        else:
+            self.path = path
         if label is None and path is not None:
             label = os.path.basename(path)
         self._fileid = fileid
         self.label = label
         self.use = use
-        self.type = six.text_type(type)
+        self.type = str(type)
         self.parent = None
         self._children = []
         if not transform_files:
             transform_files = []
         self.transform_files = transform_files
         self.mets_div_type = mets_div_type or self.type
         children = children or []
@@ -162,63 +151,66 @@
         self.derived_from = derived_from
         if bool(checksum) != bool(checksumtype):
             raise ValueError(
                 "Must provide both checksum and checksumtype, or neither. Provided values: %s and %s"
                 % (checksum, checksumtype)
             )
         if checksumtype and checksumtype not in self.ALLOWED_CHECKSUMS:
-            raise ValueError(
-                "%s must be one of %s" % (checksumtype, self.ALLOWED_CHECKSUMS)
-            )
+            raise ValueError(f"{checksumtype} must be one of {self.ALLOWED_CHECKSUMS}")
         self.checksum = checksum
         self.checksumtype = checksumtype
         self.amdsecs = []
         self.dmdsecs = []
+        self.dmdsecs_by_mdtype = {}
 
     @classmethod
     def dir(cls, label, children):
         """Return ``FSEntry`` directory object."""
-        return FSEntry(label=label, children=children, type=u"Directory", use=None)
+        return FSEntry(label=label, children=children, type="Directory", use=None)
 
     @classmethod
     def from_fptr(cls, label, type_, fptr):
         """Return ``FSEntry`` object."""
         return FSEntry(
+            fileid=fptr.fileid,
             label=label,
             type=type_,
             path=fptr.path,
             use=fptr.use,
             file_uuid=fptr.file_uuid,
             derived_from=fptr.derived_from,
             checksum=fptr.checksum,
             checksumtype=fptr.checksumtype,
+            transform_files=fptr.transform_files,
         )
 
     def __str__(self):
         return "{s.type}: {s.path}".format(s=self)
 
     def __repr__(self):
-        return "FSEntry(type={s.type!r}, path={s.path!r}, use={s.use!r}, label={s.label!r}, file_uuid={s.file_uuid!r}, checksum={s.checksum!r}, checksumtype={s.checksumtype!r})".format(
+        return "FSEntry(type={s.type!r}, path={s.path!r}, use={s.use!r}, label={s.label!r}, file_uuid={s.file_uuid!r}, checksum={s.checksum!r}, checksumtype={s.checksumtype!r}, fileid={s._fileid!r})".format(
             s=self
         )
 
     # PROPERTIES
 
     def file_id(self):
-        """ Returns the fptr @FILEID if this is not a Directory. """
+        """Returns the fptr @FILEID if this is not a Directory."""
         if self.type.lower() == "directory":
             return None
         if self.file_uuid is None:
             raise exceptions.MetsError(
                 "No FILEID: File %s does not have file_uuid set" % self.path
             )
         if self.is_aip:
             if self._fileid:
                 return self._fileid
-            return os.path.splitext(os.path.basename(self.path))[0]
+            return (
+                utils.FILE_ID_PREFIX + os.path.splitext(os.path.basename(self.path))[0]
+            )
         return utils.FILE_ID_PREFIX + self.file_uuid
 
     def group_id(self):
         """
         Returns the @GROUPID.
 
         If derived_from is set, returns that group_id.
@@ -227,20 +219,20 @@
             return self.derived_from.group_id()
         if self.file_uuid is None:
             return None
         return utils.GROUP_ID_PREFIX + self.file_uuid
 
     @property
     def admids(self):
-        """ Returns a list of ADMIDs for this entry. """
+        """Returns a list of ADMIDs for this entry."""
         return [a.id_string for a in self.amdsecs]
 
     @property
     def dmdids(self):
-        """ Returns a list of DMDIDs for this entry. """
+        """Returns a list of DMDIDs for this entry."""
         return [d.id_string for d in self.dmdsecs]
 
     @property
     def children(self):
         # Read-only
         return self._children
 
@@ -267,15 +259,17 @@
         if mode.lower() == "mdwrap":
             othermdtype = kwargs.get("othermdtype")
             mdsec = MDWrap(md, mdtype, othermdtype)
         elif mode.lower() == "mdref":
             loctype = kwargs.get("loctype")
             label = kwargs.get("label")
             otherloctype = kwargs.get("otherloctype")
-            mdsec = MDRef(md, mdtype, loctype, label, otherloctype)
+            xptr = kwargs.get("xptr")
+            othermdtype = kwargs.get("othermdtype")
+            mdsec = MDRef(md, mdtype, loctype, label, otherloctype, xptr, othermdtype)
         subsection = SubSection(subsection, mdsec)
         if subsection.subsection == "dmdSec":
             self.dmdsecs.append(subsection)
         else:
             try:
                 amdsec = self.amdsecs[0]
             except IndexError:
@@ -290,31 +284,63 @@
     def add_digiprovmd(self, md, mdtype, mode="mdwrap", **kwargs):
         return self._add_metadata_element(md, "digiprovMD", mdtype, mode, **kwargs)
 
     def add_rightsmd(self, md, mdtype, mode="mdwrap", **kwargs):
         return self._add_metadata_element(md, "rightsMD", mdtype, mode, **kwargs)
 
     def add_dmdsec(self, md, mdtype, mode="mdwrap", **kwargs):
-        return self._add_metadata_element(md, "dmdSec", mdtype, mode, **kwargs)
+        """Add dmdsec.
+
+        Extension of _add_metadata_element that adds a dmdSec and updates the
+        previous dmdSecs with the same MDTYPE and OTHERMDTYPE attribute values,
+        marking them as "superseded" and using the same group_id for all of them.
+        """
+        dmdsec = self._add_metadata_element(md, "dmdSec", mdtype, mode, **kwargs)
+        dmdsec.status = kwargs.get("status") or "original"
+        mdtype_key = utils.generate_mdtype_key(mdtype, kwargs.get("othermdtype", ""))
+        if mdtype_key in self.dmdsecs_by_mdtype:
+            group_id = getattr(self.dmdsecs_by_mdtype[mdtype_key][0], "group_id")
+            if not group_id:
+                group_id = str(uuid4())
+            dmdsec.group_id = group_id
+            for previous_dmdsec in self.dmdsecs_by_mdtype[mdtype_key]:
+                previous_dmdsec.group_id = group_id
+                if not previous_dmdsec.status:
+                    previous_dmdsec.status = "original"
+                if not previous_dmdsec.status.endswith("-superseded"):
+                    previous_dmdsec.status += "-superseded"
+        self.dmdsecs_by_mdtype.setdefault(mdtype_key, []).append(dmdsec)
+        return dmdsec
+
+    def delete_dmdsec(self, mdtype, othermdtype=""):
+        """Mark latest dmdsec of mdtype_othermdtype as deleted.
+
+        It doesn't delete the dmdsec from the METS. It only sets its status
+        attribute to "deleted".
+        """
+        mdtype_key = utils.generate_mdtype_key(mdtype, othermdtype)
+        if mdtype_key in self.dmdsecs_by_mdtype:
+            self.dmdsecs_by_mdtype[mdtype_key][-1].status = "deleted"
+
+    def has_dmdsec(self, mdtype, othermdtype=""):
+        """Check if a dmdsec of mdtype_othermdtype exists for this entry."""
+        mdtype_key = utils.generate_mdtype_key(mdtype, othermdtype)
+        return mdtype_key in self.dmdsecs_by_mdtype
 
     def serialize_md_inst(self, md_inst, md_class):
         """Serialize object ``md_inst`` by transforming it into an
         ``lxml.etree._ElementTree``. If it already is such, return it. If not,
         make sure it is the correct type and return the output of calling
         ``seriaize()`` on it.
         """
-        valid_insts = tuple(
-            chain((etree._ElementTree, etree._Element), six.string_types)
-        )
+        valid_insts = tuple(chain((etree._ElementTree, etree._Element), (str,)))
         if isinstance(md_inst, valid_insts):
             return md_inst
         if not isinstance(md_inst, md_class):
-            raise TypeError(
-                "Instance {!r} must be instance of {!r}".format(md_inst, md_class)
-            )
+            raise TypeError(f"Instance {md_inst!r} must be instance of {md_class!r}")
         return md_inst.serialize()
 
     def add_premis_object(self, md, mode="mdwrap"):
         meth = self.add_techmd
         if self.is_empty_dir:
             meth = self.add_dmdsec
         return meth(
@@ -336,17 +362,17 @@
     def add_premis_rights(self, md, mode="mdwrap"):
         return self.add_rightsmd(
             self.serialize_md_inst(md, self.premis_rights_class),
             self.PREMIS_RIGHTS,
             mode,
         )
 
-    def add_dublin_core(self, md, mode="mdwrap"):
-        # TODO add extra args and create DC object here
-        return self.add_dmdsec(md, "DC", mode)
+    def add_dublin_core(self, md, mode="mdwrap", **kwargs):
+        # TODO create DC object here
+        return self.add_dmdsec(md, "DC", mode, **kwargs)
 
     def add_child(self, child):
         """Add a child FSEntry to this FSEntry.
 
         Only FSEntrys with a type of 'directory' can have children.
 
         This does not detect cyclic parent/child relationships, but that will
@@ -397,14 +423,16 @@
         ):
             return None
         el = etree.Element(utils.lxmlns("mets") + "file", ID=self.file_id())
         if self.group_id():
             el.attrib["GROUPID"] = self.group_id()
         if self.admids:
             el.set("ADMID", " ".join(self.admids))
+        if self.dmdids and self.use == "original":
+            el.set("DMDID", " ".join(self.dmdids))
         if self.checksum and self.checksumtype:
             el.attrib["CHECKSUM"] = self.checksum
             el.attrib["CHECKSUMTYPE"] = self.checksumtype
         if self.path:
             flocat = etree.SubElement(el, utils.lxmlns("mets") + "FLocat")
             # Setting manually so order is correct
             try:
@@ -417,15 +445,15 @@
             flocat.set("LOCTYPE", "OTHER")
             flocat.set("OTHERLOCTYPE", "SYSTEM")
         for transform_file in self.transform_files:
             transform_file_el = etree.SubElement(
                 el, utils.lxmlns("mets") + "transformFile"
             )
             for key, val in transform_file.items():
-                attribute = "transform{}".format(key).upper()
+                attribute = f"transform{key}".upper()
                 transform_file_el.attrib[attribute] = str(val)
         return el
 
     @property
     def is_empty_dir(self):
         """Returns ``True`` if this fs item is a directory with no children or
         a directory with only other empty directories as children.
@@ -463,16 +491,17 @@
         if self.is_empty_dir and not normative:
             return None
         el = etree.Element(utils.lxmlns("mets") + "div", TYPE=self.mets_div_type)
         el.attrib["LABEL"] = self.label
         if (not normative) and self.file_id():
             etree.SubElement(el, utils.lxmlns("mets") + "fptr", FILEID=self.file_id())
         if self.dmdids:
-            if (not normative) or (normative and self.is_empty_dir):
-                el.set("DMDID", " ".join(self.dmdids))
+            el.set("DMDID", " ".join(self.dmdids))
+        if self.mets_div_type.lower() == "directory" and self.admids:
+            el.set("ADMID", " ".join(self.admids))
         if recurse and self._children:
             for child in self._children:
                 child_el = child.serialize_structmap(
                     recurse=recurse, normative=normative
                 )
                 if child_el is not None:
                     el.append(child_el)
@@ -512,7 +541,23 @@
 
     def get_premis_rights_statement(self, rights_statement_uuid):
         for rights in self.get_premis_rights():
             for statement in rights.rights_statement:
                 if statement.rights_statement_identifier_value == rights_statement_uuid:
                     return statement
         return None
+
+    def get_path(self):
+        """Return the relative path to this FSEntry.
+
+        If the path is not set, it's generated from the ancestor labels. Raises an
+        AttributeError if the path cannot be generated. Returns None for the top
+        level FSEntry.
+        """
+        if self.path:
+            return self.path
+        if not self.label:
+            raise AttributeError("The path cannot be generated")
+        if self.parent:
+            if self.parent.parent:
+                return self.parent.get_path() + os.sep + self.label
+            return self.label
```

### Comparing `metsrw-0.3.9/metsrw/validate.py` & `metsrw-0.4.0/metsrw/validate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-# -*- coding: utf-8 -*-
 import os
 
-from lxml import etree, isoschematron
-import six
+from lxml import etree
+from lxml import isoschematron
 
 from .utils import NAMESPACES
 
 METS_XSD_PATH = "resources/mets.xsd"
 
 # Right now there are two different schematron files for validating
 # Archivematica-generated METS files vs Archivematica-generated METS pointer
@@ -15,17 +14,15 @@
 AM_PNTR_SCT_PATH = "resources/archivematica_mets_pointer_file_schematron.xml"
 
 
 def _get_file_path(path):
     if not os.path.isfile(path):
         path_2 = os.path.join(os.path.dirname(os.path.abspath(__file__)), path)
         if not os.path.isfile(path_2):
-            raise ValueError(
-                "There is no (schema) file at either {} or {}".format(path, path_2)
-            )
+            raise ValueError(f"There is no (schema) file at either {path} or {path_2}")
         return path_2
     return path
 
 
 def get_schematron(sct_path):
     """Return an lxml ``isoschematron.Schematron()`` instance using the
     schematron file at ``sct_path``.
@@ -95,15 +92,15 @@
     return is_valid, error_log
 
 
 def schematron_validate(mets_doc, schematron=AM_SCT_PATH):
     """Validate a METS file using a schematron schema. Return a boolean
     indicating validity and a report as an ``lxml.ElementTree`` instance.
     """
-    if isinstance(schematron, six.string_types):
+    if isinstance(schematron, str):
         schematron = get_schematron(schematron)
     is_valid = schematron.validate(mets_doc)
     report = schematron.validation_report
     return is_valid, report
 
 
 def sct_report_string(report):
```

### Comparing `metsrw-0.3.9/metsrw/di.py` & `metsrw-0.4.0/metsrw/di.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 """Dependency Injection logic for metsrw.
 
 Here a global singleton feature broker is instantiated. By providing features
 (i.e., dependencies) to the feature broker one can alter, for example, the
 PREMIS dependencies used by metsrw's ``FSEntry`` class when reading and writing
 PREMIS XML. Here we provide default classes for handling PREMIS using classes
 defined in plugins.premisrw::
@@ -15,21 +14,18 @@
 However, the PREMIS dependencies can be altered by providing other features
 with the same names, e.g.,::
 
     >>> feature_broker.provide('premis_object_class', MyOtherPREMISObjectClass)
 
 See http://code.activestate.com/recipes/413268/
 """
-
-from six import with_metaclass
-
 from .plugins import premisrw
 
 
-class FeatureBroker(object):
+class FeatureBroker:
     """Feature broker allows for the provisioning of features. These features
     are dependencies that can be injected. Usage::
 
         >>> feature_broker = FeatureBroker()
         >>> feature_broker.provide('premis_object_class', premisrw.PREMISObject)
     """
 
@@ -57,15 +53,15 @@
     def __len__(self):
         return len(self.providers)
 
     def __getitem__(self, feature_name):
         try:
             provider = self.providers[feature_name]
         except KeyError:
-            raise KeyError("Unknown feature named {!r}".format(feature_name))
+            raise KeyError(f"Unknown feature named {feature_name!r}")
         return provider()
 
 
 def set_feature_broker_to_default_state(fb):
     fb.clear()
     fb.provide("premis_object_class", premisrw.PREMISObject)
     fb.provide("premis_event_class", premisrw.PREMISEvent)
@@ -73,15 +69,15 @@
     fb.provide("premis_rights_class", premisrw.PREMISRights)
 
 
 feature_broker = FeatureBroker()  # global singleton feature broker
 set_feature_broker_to_default_state(feature_broker)
 
 
-class Dependency(object):
+class Dependency:
     """Non-overriding descriptor for declaring required dependencies in metsrw
     classes. In the following example usage the ``FSEntry`` class is declaring
     a dependency on a feature named 'premis_object_class' which is a class and
     which has methods ``fromtree`` and ``serialize``::
 
         >>> from .di import is_class, has_methods, Dependency
         >>> class FSEntry(object):
@@ -114,21 +110,21 @@
     that its ``dependency_name`` value should be the same as the name of the
     class attribute it was assigned to in the managed class. In short, it
     allows us to write ``premis_object_class = Dependency()`` instead of
     ``premis_object_class = Dependency('premis_object_class')``.
     """
 
     def __init__(cls, name, bases, attr_dict):
-        super(DependencyPossessorMeta, cls).__init__(name, bases, attr_dict)
+        super().__init__(name, bases, attr_dict)
         for key, attr in attr_dict.items():
             if isinstance(attr, Dependency):
                 attr.dependency_name = key
 
 
-class DependencyPossessor(with_metaclass(DependencyPossessorMeta, object)):
+class DependencyPossessor(metaclass=DependencyPossessorMeta):
     pass
 
 
 # ==============================================================================
 #   Assertions for declaring dependencies using Dependency
 # ==============================================================================
```

