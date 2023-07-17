# Comparing `tmp/mappings_utility-0.1.6.tar.gz` & `tmp/mappings_utility-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mappings_utility-0.1.6.tar", max compression
+gzip compressed data, was "mappings_utility-0.2.0.tar", max compression
```

## Comparing `mappings_utility-0.1.6.tar` & `mappings_utility-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0        0 2022-10-06 19:15:16.027748 mappings_utility-0.1.6/mappings_utility/__init__.py
--rw-r--r--   0        0        0     4978 2023-02-18 15:14:36.395456 mappings_utility-0.1.6/mappings_utility/mapping_svc.py
--rw-r--r--   0        0        0     4372 2023-01-09 22:28:12.367710 mappings_utility-0.1.6/mappings_utility/mapping_utility.py
--rw-r--r--   0        0        0     9619 2023-02-18 15:15:13.948699 mappings_utility-0.1.6/mappings_utility/sdmx_mapping_utility.py
--rw-r--r--   0        0        0     7175 2023-02-18 14:52:01.562237 mappings_utility-0.1.6/mappings_utility/sdmx_structures.py
--rw-r--r--   0        0        0      527 2023-02-18 15:33:51.998770 mappings_utility-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      631 2023-01-06 11:55:11.601523 mappings_utility-0.1.6/README.md
--rw-r--r--   0        0        0     1376 1970-01-01 00:00:00.000000 mappings_utility-0.1.6/setup.py
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 mappings_utility-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-04 11:47:40.082954 mappings_utility-0.2.0/mappings_utility/__init__.py
+-rw-r--r--   0        0        0     4978 2023-07-04 11:47:40.084953 mappings_utility-0.2.0/mappings_utility/mapping_svc.py
+-rw-r--r--   0        0        0     4372 2023-07-04 11:47:40.097956 mappings_utility-0.2.0/mappings_utility/mapping_utility.py
+-rw-r--r--   0        0        0     9802 2023-07-11 14:17:10.885113 mappings_utility-0.2.0/mappings_utility/sdmx_mapping_utility.py
+-rw-r--r--   0        0        0     7449 2023-07-11 11:53:53.486108 mappings_utility-0.2.0/mappings_utility/sdmx_structures.py
+-rw-r--r--   0        0        0      748 2023-07-11 14:59:06.287248 mappings_utility-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      631 2023-07-04 11:47:40.072953 mappings_utility-0.2.0/README.md
+-rw-r--r--   0        0        0     1282 1970-01-01 00:00:00.000000 mappings_utility-0.2.0/PKG-INFO
```

### Comparing `mappings_utility-0.1.6/mappings_utility/mapping_svc.py` & `mappings_utility-0.2.0/mappings_utility/mapping_svc.py`

 * *Files identical despite different names*

### Comparing `mappings_utility-0.1.6/mappings_utility/mapping_utility.py` & `mappings_utility-0.2.0/mappings_utility/mapping_utility.py`

 * *Files identical despite different names*

### Comparing `mappings_utility-0.1.6/mappings_utility/sdmx_mapping_utility.py` & `mappings_utility-0.2.0/mappings_utility/sdmx_mapping_utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,15 +158,18 @@
                # copy identical with target component-name
                logging.info(f'copying source to target {cm.sources} -> {cm.targets}')
                df[cm.targets[0]] = df[cm.sources[0]]
             else:
                # only those cases can be mapped safely where there are valid inputs in all source columns
                logging.info(f'applying representation map {cm.sources} -> {cm.targets}')
                rm = self.get_representation_by_urn(cm.representation)
-               df[cm.targets] = df.apply(lambda x: rm.get_target_values_by_sourcelist([x[c] for c in cm.sources]), axis=1, result_type='expand')
+               try:
+                  df[cm.targets] = df.apply(lambda x: rm.get_target_values_by_sourcelist([x[c] for c in cm.sources]), axis=1, result_type='expand')
+               except:
+                  logging.debug(f'error in representation map {cm.sources} -> {cm.targets};\n {cm.representation};\n {df.head(2)}')  
 
          # Add target missing columns mapped as fixed value
          for fvm in self.fixedvalue_maps:
             if not nulledFixedTargets:
                df[fvm.target] = fvm.value
             else:
                df[fvm.target] = ''
```

### Comparing `mappings_utility-0.1.6/mappings_utility/sdmx_structures.py` & `mappings_utility-0.2.0/mappings_utility/sdmx_structures.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
 from typing import NamedTuple, Union
 from dataclasses import dataclass
 from enum import Enum
 import re
 import xml.etree.ElementTree as ET
+import logging
 
 NS = {"xsi": "http://www.w3.org/2001/XMLSchema-instance",
         "message": "http://www.sdmx.org/resources/sdmxml/schemas/v3_0/message",
         "str": "http://www.sdmx.org/resources/sdmxml/schemas/v3_0/structure",
         "com": "http://www.sdmx.org/resources/sdmxml/schemas/v3_0/common"
         }
 
@@ -180,41 +181,46 @@
             rmd['targetvalues'].append(tv.text)
          padding = self.target_component_count - len(rmd['targetvalues'])
          for i in range(padding):
             rmd['targetvalues'].append(None)
          self.mappings.append(deepcopy(rmd))
       
    def _replace_matches(self, matching_groups: tuple, target_list: list[str]) -> list[str]:
+      #print("replacement checks:", matching_groups, target_list)
       sp = re.compile(r'.*(\\[1-9]).*')
       for idx, val in enumerate(target_list):
-         sm = sp.match(val)
-         if sm: 
-            for x in sm.groups():
-               # index correction to allow end-user to use 1 based indexing for matching groups
-               target_list[idx] = val.replace(x, matching_groups[int(x[1])-1], 1)
+         if val:
+            sm = sp.match(val)
+            if sm: 
+               for x in sm.groups():
+                  # index correction to allow end-user to use 1 based indexing for matching groups
+                  target_list[idx] = val.replace(x, matching_groups[int(x[1])-1], 1)
    
       return target_list
 
    def get_target_values_by_sourcelist(self, sourcelst: list) -> Union[list[str], None]:
-      
          for m in self.mappings:
-            pairs = zip(m['sourcevalues'], sourcelst)
+            
+            pairs = zip(m['sourcevalues'], sourcelst)      
             matched = True
             target = deepcopy(m['targetvalues'])
-            # assumption: only one of the fields in source has RegEx
+            
+            # assumption: only one of the fields in source has RegEx with substitution 
             for pair in pairs:
                if pair[0].isRegEx:
                   p = re.compile(pair[0].value)
                   matches = p.match(pair[1])
                   if matches:
                      target = self._replace_matches(matches.groups(), deepcopy(target))
                   else: 
                      matched = False
                else:
                   if pair[0].value != pair[1]:
                      matched = False
             if matched:
+               logging.debug(f"produced target: {target} for pair {m['sourcevalues']}, {sourcelst}")
                return target
+         
          if any([s!='' for s in sourcelst]):
             return [INVALID] * len(self.mappings[0]['targetvalues'])
          else:
             return [''] * len(self.mappings[0]['targetvalues'])
```

### Comparing `mappings_utility-0.1.6/pyproject.toml` & `mappings_utility-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 [tool.poetry]
 name = "mappings_utility"
-version = "0.1.6"
+version = "0.2.0"
 description = "mapping utility tool for sdmx based partial mappings"
 authors = ["Gyorgy Gyomai <gyorgy.gyomai@oecd.org>", "Abdel Aliaoui <abdel.aliaoui@oecd.org>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pandas = "^1.5.0"
 fastapi = "^0.87.0"
 uvicorn = "^0.20.0"
 requests = "^2.28.1"
+pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 
+[tool.pytest.ini_options]
+log_cli = true
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mappings_utility-0.1.6/README.md` & `mappings_utility-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `mappings_utility-0.1.6/setup.py` & `mappings_utility-0.2.0/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,26 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: mappings-utility
+Version: 0.2.0
+Summary: mapping utility tool for sdmx based partial mappings
+Author: Gyorgy Gyomai
+Author-email: gyorgy.gyomai@oecd.org
+Requires-Python: >=3.9,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: fastapi (>=0.87.0,<0.88.0)
+Requires-Dist: pandas (>=1.5.0,<2.0.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: uvicorn (>=0.20.0,<0.21.0)
+Description-Content-Type: text/markdown
+
+An SDMX mapping utility to generate partial key maps for referential metadata.
+Although not designed to do that, data mappings are also possible.
+
+Three methods are available:
+- *map_withFile* GET method (receiving the mapping source and mapping rules both as file references)
+- *map_withURN* GET method (receiving the mapping source  as file and the mapping rules as SDMX registry endpoint + mapping ID)
+- *map_json_withURN* POST method (receiving the mapping source as the body of the request in json - pandas dataframe dictionary style - and mapping rules as SDMX registry endpoint + mapping ID) (added in version 0.1.1)
 
-packages = \
-['mappings_utility']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['fastapi>=0.87.0,<0.88.0',
- 'pandas>=1.5.0,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'uvicorn>=0.20.0,<0.21.0']
-
-setup_kwargs = {
-    'name': 'mappings-utility',
-    'version': '0.1.6',
-    'description': 'mapping utility tool for sdmx based partial mappings',
-    'long_description': 'An SDMX mapping utility to generate partial key maps for referential metadata.\nAlthough not designed to do that, data mappings are also possible.\n\nThree methods are available:\n- *map_withFile* GET method (receiving the mapping source and mapping rules both as file references)\n- *map_withURN* GET method (receiving the mapping source  as file and the mapping rules as SDMX registry endpoint + mapping ID)\n- *map_json_withURN* POST method (receiving the mapping source as the body of the request in json - pandas dataframe dictionary style - and mapping rules as SDMX registry endpoint + mapping ID) (added in version 0.1.1)\n',
-    'author': 'Gyorgy Gyomai',
-    'author_email': 'gyorgy.gyomai@oecd.org',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

