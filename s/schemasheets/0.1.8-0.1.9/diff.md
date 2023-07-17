# Comparing `tmp/schemasheets-0.1.8.tar.gz` & `tmp/schemasheets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemasheets-0.1.8.tar", max compression
+gzip compressed data, was "schemasheets-0.1.9.tar", max compression
```

## Comparing `schemasheets-0.1.8.tar` & `schemasheets-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0     1154 2022-03-04 15:09:07.935530 schemasheets-0.1.8/README.md
--rw-r--r--   0        0        0      789 2022-03-08 20:55:07.825575 schemasheets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/__init__.py
--rw-r--r--   0        0        0    14984 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/conf/configschema.py
--rw-r--r--   0        0        0     9431 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/conf/configschema.yaml
--rw-r--r--   0        0        0    28038 2022-03-08 20:47:21.753320 schemasheets-0.1.8/schemasheets/schemamaker.py
--rw-r--r--   0        0        0       97 2022-03-08 20:47:21.757320 schemasheets-0.1.8/schemasheets/schemaview_vs_examples.py
--rw-r--r--   0        0        0     3287 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/sheets_to_project.py
--rw-r--r--   0        0        0        0 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/utils/__init__.py
--rw-r--r--   0        0        0    11198 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/utils/configschema.py
--rw-r--r--   0        0        0      194 2022-03-04 15:09:07.939530 schemasheets-0.1.8/schemasheets/utils/prefixtool.py
--rw-r--r--   0        0        0     2209 2022-03-08 20:55:10.928476 schemasheets-0.1.8/setup.py
--rw-r--r--   0        0        0     1884 2022-03-08 20:55:10.928800 schemasheets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1155 2022-03-16 23:19:27.645060 schemasheets-0.1.9/README.md
+-rw-r--r--   0        0        0      851 2022-03-16 23:20:59.370195 schemasheets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/__init__.py
+-rw-r--r--   0        0        0    14984 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/conf/configschema.py
+-rw-r--r--   0        0        0     9431 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/conf/configschema.yaml
+-rw-r--r--   0        0        0     8220 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/schema_exporter.py
+-rw-r--r--   0        0        0    22436 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/schemamaker.py
+-rw-r--r--   0        0        0     7200 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/schemasheet_datamodel.py
+-rw-r--r--   0        0        0       97 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/schemaview_vs_examples.py
+-rw-r--r--   0        0        0     3287 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/sheets_to_project.py
+-rw-r--r--   0        0        0        0 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/utils/__init__.py
+-rw-r--r--   0        0        0    11198 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/utils/configschema.py
+-rw-r--r--   0        0        0      194 2022-03-16 23:19:27.653061 schemasheets-0.1.9/schemasheets/utils/prefixtool.py
+-rw-r--r--   0        0        0     2317 2022-03-16 23:21:00.220598 schemasheets-0.1.9/setup.py
+-rw-r--r--   0        0        0     1885 2022-03-16 23:21:00.221020 schemasheets-0.1.9/PKG-INFO
```

### Comparing `schemasheets-0.1.8/README.md` & `schemasheets-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Schemasheets - make datamodels using spreadsheets
 
 <p align="center">
     <a href="https://github.com/linkml/schemasheets/actions/workflows/main.yml">
-        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yml/badge.svg" />
+        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yaml/badge.svg" />
     </a>
     <a href="https://pypi.org/project/linkml">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/linkml" />
     </a>
     <a href="https://pypi.org/project/sssom">
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/sssom" />
     </a>
```

### Comparing `schemasheets-0.1.8/pyproject.toml` & `schemasheets-0.1.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schemasheets"
-version = "0.1.8"
+version = "v0.1.9"
 description = "Package to author schemas using spreadsheets"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 homepage = "https://github.com/linkml/schemasheets"
 repository = "https://github.com/linkml/schemasheets"
@@ -24,8 +24,9 @@
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 sheets2linkml = "schemasheets.schemamaker:convert"
+linkml2sheets = "schemasheets.schema_exporter:export_schema"
 sheets2project = "schemasheets.sheets_to_project:multigen"
```

### Comparing `schemasheets-0.1.8/schemasheets/conf/configschema.py` & `schemasheets-0.1.9/schemasheets/conf/configschema.py`

 * *Files identical despite different names*

### Comparing `schemasheets-0.1.8/schemasheets/conf/configschema.yaml` & `schemasheets-0.1.9/schemasheets/conf/configschema.yaml`

 * *Files identical despite different names*

### Comparing `schemasheets-0.1.8/schemasheets/schemamaker.py` & `schemasheets-0.1.9/schemasheets/schemamaker.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,190 +1,37 @@
 import sys
 import csv
 import logging
-import pkgutil
-from pathlib import PurePath
-from functools import lru_cache
+
 
 import click
 import yaml
 from dataclasses import dataclass
 from typing import List, Union, Any, Dict, Tuple, Generator, TextIO
 
 from linkml_runtime.dumpers import yaml_dumper
 from linkml_runtime.linkml_model import Annotation, Example
 from linkml_runtime.linkml_model.meta import SchemaDefinition, ClassDefinition, Prefix, \
     SlotDefinition, EnumDefinition, PermissibleValue, SubsetDefinition, TypeDefinition, Element
 from linkml_runtime.utils.schemaview import SchemaView, re
 
-from schemasheets.conf.configschema import ColumnSettings, Shortcuts, Cardinality
+from schemasheets.schemasheet_datamodel import ColumnConfig, TableConfig, get_configmodel, get_metamodel, COL_NAME, \
+    DESCRIPTOR, \
+    tmap, T_CLASS, T_PV, T_SLOT, T_SUBSET, T_SCHEMA, T_ENUM, T_PREFIX, T_TYPE, SchemaSheet
+from schemasheets.conf.configschema import Cardinality
 from schemasheets.utils.prefixtool import guess_prefix_expansion
 
 
 class SchemaSheetRowException(Exception):
     pass
 
 
-c = ClassDefinition
-T_SCHEMA = 'schema'
-T_CLASS = 'class'
-T_SLOT = 'slot'
-T_ENUM = 'enum'
-T_PV = 'permissible_value'
-T_TYPE = 'type'
-T_SUBSET = 'subset'
-T_PREFIX = 'prefix'
-
-tmap = {
-    T_SCHEMA: SchemaDefinition,
-    T_CLASS: ClassDefinition,
-    T_SLOT: SlotDefinition,
-    T_ENUM: EnumDefinition,
-    T_PV: PermissibleValue,
-    T_TYPE: TypeDefinition,
-    T_SUBSET: SubsetDefinition,
-    T_PREFIX: Prefix
-}
-
-COL_NAME = str
-DESCRIPTOR = str
-@dataclass
-class ColumnConfig:
-    """
-    Configuration for a single column in a schema sheet
-    """
-    name: COL_NAME
-    maps_to: DESCRIPTOR = None
-    settings: ColumnSettings = None
-    metaslot: SlotDefinition = None
-    is_element_type: bool = None
-
-    def merge_settings(self, settings: ColumnSettings) -> None:
-        """
-        merges specified settings into current settings
-
-        :param settings: settings to be merged
-        """
-        for k, v in vars(settings).items():
-            if v:
-                setattr(self.settings, k, v)
-
-    def add_info(self, info: Union[Dict, DESCRIPTOR]) -> None:
-        """
-        Adds configuration/settings in the form of a dict object.
-
-        Information can be incrementally added:
-
-        - the first piece of information should be the descriptor
-        - after that individual settings can be added
-
-        :param info: configuration
-        :return:
-        """
-        if self.maps_to is None:
-            self.settings = ColumnSettings()
-            if isinstance(info, dict):
-                items = list(info.items())
-                if len(items) != 1:
-                    raise ValueError(f'Unexpected settings: {info}')
-                else:
-                    item = items[0]
-                    self.maps_to = item[0]
-                    if isinstance(item[1], dict):
-                        settings = ColumnSettings(**item[1])
-                    else:
-                        raise ValueError(f'Expected dict after first element of {items}')
-                    self.merge_settings(settings)
-            else:
-                self.maps_to = info
-            mm = get_metamodel()
-            snmap = mm.slot_name_mappings()
-            # TODO: use alias
-            snmap['uri'] = snmap['type_uri']
-            if self.maps_to in snmap:
-                self.metaslot = snmap[self.maps_to]
-            else:
-                if self.maps_to not in tmap and self.maps_to not in Shortcuts:
-                    raise ValueError(f'Cannot interpret: {self.maps_to}')
-        else:
-            settings = ColumnSettings(**info)
-            self.merge_settings(settings)
-
-
-@dataclass
-class TableConfig:
-    """
-    Configuration for an entire table / schema sheet
-
-    """
-    name: str = None
-    """table name"""
-
-    columns: Dict[COL_NAME, ColumnConfig] = None
-    """maps column names to config"""
-
-    column_by_element_type: Dict[str, COL_NAME] = None
-    """maps element types (schema, class, ...) to the name of the column that represents them"""
-
-    metatype_column: COL_NAME = None
-    name_column: COL_NAME = None
-
-    def add_info(self, col: COL_NAME, info: Union[Dict, DESCRIPTOR]) -> None:
-        """
-        Wrapper for :ref:`ColumnConfig.add_info`
 
-        :param col:
-        :param info:
-        """
-        if col not in self.columns:
-            self.columns[col] = ColumnConfig(col)
-        #print(f'ADDING: {col}')
-        self.columns[col].add_info(info)
-        if self.columns[col].maps_to == 'metatype':
-            if self.metatype_column and self.metatype_column != col:
-                raise ValueError(f'Multiple metatype columns not allowed: {self.metatype_column}, {col}')
-            self.metatype_column = col
-        if self.columns[col].maps_to == 'name':
-            if self.name_column:
-                raise ValueError(f'Multiple name columns not allowed: {self.name_column}, {col}')
-            self.name_column = col
-        if self.column_by_element_type is None:
-            self.column_by_element_type = {}
-        for c, cc in self.columns.items():
-            if cc.maps_to in tmap:
-                self.column_by_element_type[cc.maps_to] = c
-                cc.is_element_type = True
 
 
-@lru_cache()
-def get_metamodel() -> SchemaView:
-    """
-    Returns the LinkML schema metamodel as a SchemaView object
-
-    this can be retired when https://github.com/linkml/linkml-runtime/pull/100/
-    is in major release
-    :return:
-    """
-    package = 'linkml_runtime.linkml_model.meta'
-    full_path = PurePath('model') / 'schema'
-    data = pkgutil.get_data(package, f'{full_path}/meta.yaml')
-    return SchemaView(data.decode("utf-8"))
-
-@lru_cache()
-def get_configmodel() -> SchemaView:
-    """
-    Returns the Config schema metamodel as a SchemaView object
-
-    this can be retired when https://github.com/linkml/linkml-runtime/pull/100/
-    is in major release
-    :return:
-    """
-    package = 'schemasheets.conf.configschema'
-    data = pkgutil.get_data(package, f'configschema.yaml')
-    return SchemaView(data.decode("utf-8"))
 
 
 @dataclass
 class SchemaMaker:
     """
     Engine for making LinkML schemas from FAIR Schema Sheets
     """
@@ -193,15 +40,15 @@
     metamodel: SchemaView = None
     cardinality_vocabulary: str = None
     default_name: str = None
     unique_slots: bool = None
 
     def create_schema(self, csv_files: Union[str, List[str]], **kwargs) -> SchemaDefinition:
         """
-        Create a LinkML schema from a collection of FAIR Schema Sheets
+        Create a LinkML schema from a collection of Schema Sheets
 
         :param csv_files: schema sheets
         :param kwargs:
         :return: generated schema
         """
         n = self.default_name
         if n is None:
@@ -228,56 +75,39 @@
         """
         for cn, c in self.schema.classes.items():
             inapplicable_slots = [sn for sn, s in c.slot_usage.items() if 'inapplicable' in s.annotations]
             for sn in inapplicable_slots:
                 c.slots.remove(sn)
                 del c.slot_usage[sn]
 
+
     def merge_sheet(self, file_name: str, delimiter='\t') -> None:
         """
         Merge information from the given schema sheet into the current schema
 
         :param file_name: schema sheet
         :param delimiter: default is tab
         :return:
         """
         logging.info(f'READING {file_name} D={delimiter}')
-        table_config = TableConfig(columns={})
-        line_num = 1
         with open(file_name, newline='') as tsv_file:
             reader = csv.DictReader(tsv_file, delimiter=delimiter)
-            rows = []
-            for row in reader:
-                k0 = list(row.keys())[0]
-                if row[k0].startswith('>'):
+            schemasheet = SchemaSheet.from_dictreader(reader)
+            line_num = schemasheet.start_line_number
+            # TODO: check why this doesn't work
+            #while rows and all(x for x in rows[-1] if not x):
+            #    print(f'TRIMMING: {rows[-1]}')
+            #    rows.pop()
+            logging.info(f'ROWS={len(schemasheet.rows)}')
+            for row in schemasheet.rows:
+                try:
+                    self.add_row(row, schemasheet.table_config)
                     line_num += 1
-                    for k, v in row.items():
-                        if v is not None and v.startswith('>'):
-                            v = v.replace('>', '')
-                        if v:
-                            meta_obj = yaml.safe_load(v)
-                            table_config.add_info(k, meta_obj)
-                        else:
-                            if line_num == 2:
-                                # TODO: consider auto-interpreting
-                                raise ValueError(f'Enter an interpretation for {k}')
-                            logging.debug(f'Empty val for {k} in line {line_num}')
-                else:
-                    rows.append(row)
-        # TODO: check why this doesn't work
-        #while rows and all(x for x in rows[-1] if not x):
-        #    print(f'TRIMMING: {rows[-1]}')
-        #    rows.pop()
-        logging.info(f'ROWS={len(rows)}')
-        for row in rows:
-            try:
-                self.add_row(row, table_config)
-                line_num += 1
-            except ValueError as e:
-                raise SchemaSheetRowException(f'Error in line {line_num}, row={row}') from e
+                except ValueError as e:
+                    raise SchemaSheetRowException(f'Error in line {line_num}, row={row}') from e
 
 
     def add_row(self, row: Dict[str, Any], table_config: TableConfig):
         for element in self.row_focal_element(row, table_config):
             if isinstance(element, Prefix):
                 name = element.prefix_prefix
             elif isinstance(element, PermissibleValue):
```

### Comparing `schemasheets-0.1.8/schemasheets/sheets_to_project.py` & `schemasheets-0.1.9/schemasheets/sheets_to_project.py`

 * *Files identical despite different names*

### Comparing `schemasheets-0.1.8/schemasheets/utils/configschema.py` & `schemasheets-0.1.9/schemasheets/utils/configschema.py`

 * *Files identical despite different names*

### Comparing `schemasheets-0.1.8/setup.py` & `schemasheets-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,25 @@
 install_requires = \
 ['Jinja2>=3.0.3,<4.0.0',
  'bioregistry>=0.4.30,<0.5.0',
  'linkml>=1.1.15,<2.0.0',
  'ontodev-cogs>=0.3.3,<0.4.0']
 
 entry_points = \
-{'console_scripts': ['sheets2linkml = schemasheets.schemamaker:convert',
+{'console_scripts': ['linkml2sheets = '
+                     'schemasheets.schema_exporter:export_schema',
+                     'sheets2linkml = schemasheets.schemamaker:convert',
                      'sheets2project = '
                      'schemasheets.sheets_to_project:multigen']}
 
 setup_kwargs = {
     'name': 'schemasheets',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Package to author schemas using spreadsheets',
-    'long_description': '# Schemasheets - make datamodels using spreadsheets\n\n<p align="center">\n    <a href="https://github.com/linkml/schemasheets/actions/workflows/main.yml">\n        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yml/badge.svg" />\n    </a>\n    <a href="https://pypi.org/project/linkml">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/linkml" />\n    </a>\n    <a href="https://pypi.org/project/sssom">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/sssom" />\n    </a>\n    <a href="https://github.com/linkml/schemasheets/blob/main/LICENSE">\n        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/sssom" />\n    </a>\n    <a href="https://github.com/psf/black">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">\n    </a>\n</p>\n\nSchemasheets is a framework for managing your schema using\nspreadsheets (Google Sheets, Excel). It works by compiling down to\n[LinkML](https://linkml.io), which can itself be compuled to a variety\nof formalisms.\n\nFor more info, see the [documentation](https://linkml.io/schemasheets)\n',
+    'long_description': '# Schemasheets - make datamodels using spreadsheets\n\n<p align="center">\n    <a href="https://github.com/linkml/schemasheets/actions/workflows/main.yml">\n        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yaml/badge.svg" />\n    </a>\n    <a href="https://pypi.org/project/linkml">\n        <img alt="PyPI" src="https://img.shields.io/pypi/v/linkml" />\n    </a>\n    <a href="https://pypi.org/project/sssom">\n        <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/sssom" />\n    </a>\n    <a href="https://github.com/linkml/schemasheets/blob/main/LICENSE">\n        <img alt="PyPI - License" src="https://img.shields.io/pypi/l/sssom" />\n    </a>\n    <a href="https://github.com/psf/black">\n        <img src="https://img.shields.io/badge/code%20style-black-000000.svg" alt="Code style: black">\n    </a>\n</p>\n\nSchemasheets is a framework for managing your schema using\nspreadsheets (Google Sheets, Excel). It works by compiling down to\n[LinkML](https://linkml.io), which can itself be compuled to a variety\nof formalisms.\n\nFor more info, see the [documentation](https://linkml.io/schemasheets)\n',
     'author': 'cmungall',
     'author_email': 'cjm@berkeleybop.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/linkml/schemasheets',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['schemasheets', 'schemasheets.conf', 'schemasheets.utils'] package_data = \
 {'': ['*']} install_requires = \ ['Jinja2>=3.0.3,<4.0.0',
 'bioregistry>=0.4.30,<0.5.0', 'linkml>=1.1.15,<2.0.0', 'ontodev-
-cogs>=0.3.3,<0.4.0'] entry_points = \ {'console_scripts': ['sheets2linkml =
+cogs>=0.3.3,<0.4.0'] entry_points = \ {'console_scripts': ['linkml2sheets = '
+'schemasheets.schema_exporter:export_schema', 'sheets2linkml =
 schemasheets.schemamaker:convert', 'sheets2project = '
 'schemasheets.sheets_to_project:multigen']} setup_kwargs = { 'name':
-'schemasheets', 'version': '0.1.8', 'description': 'Package to author schemas
+'schemasheets', 'version': '0.1.9', 'description': 'Package to author schemas
 using spreadsheets', 'long_description': '# Schemasheets - make datamodels
 using spreadsheets\n\n
    \n \n_[Tests]\n\n \n_[PyPI]\n\n \n_[PyPI_-_Python_Version]\n\n \n_[PyPI_-
                     License]\n\n \n_[Code_style:_black]\n\n
 \n\nSchemasheets is a framework for managing your schema using\nspreadsheets
 (Google Sheets, Excel). It works by compiling down to\n[LinkML](https://
 linkml.io), which can itself be compuled to a variety\nof formalisms.\n\nFor
```

### Comparing `schemasheets-0.1.8/PKG-INFO` & `schemasheets-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemasheets
-Version: 0.1.8
+Version: 0.1.9
 Summary: Package to author schemas using spreadsheets
 Home-page: https://github.com/linkml/schemasheets
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,15 +17,15 @@
 Project-URL: Repository, https://github.com/linkml/schemasheets
 Description-Content-Type: text/markdown
 
 # Schemasheets - make datamodels using spreadsheets
 
 <p align="center">
     <a href="https://github.com/linkml/schemasheets/actions/workflows/main.yml">
-        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yml/badge.svg" />
+        <img alt="Tests" src="https://github.com/linkml/schemasheets/actions/workflows/main.yaml/badge.svg" />
     </a>
     <a href="https://pypi.org/project/linkml">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/linkml" />
     </a>
     <a href="https://pypi.org/project/sssom">
         <img alt="PyPI - Python Version" src="https://img.shields.io/pypi/pyversions/sssom" />
     </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: schemasheets Version: 0.1.8 Summary: Package to
+Metadata-Version: 2.1 Name: schemasheets Version: 0.1.9 Summary: Package to
 author schemas using spreadsheets Home-page: https://github.com/linkml/
 schemasheets Author: cmungall Author-email: cjm@berkeleybop.org Requires-
 Python: >=3.9,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.9 Requires-Dist: Jinja2 (>=3.0.3,<4.0.0) Requires-Dist: bioregistry
 (>=0.4.30,<0.5.0) Requires-Dist: linkml (>=1.1.15,<2.0.0) Requires-Dist:
 ontodev-cogs (>=0.3.3,<0.4.0) Project-URL: Documentation, https://github.com/
```

