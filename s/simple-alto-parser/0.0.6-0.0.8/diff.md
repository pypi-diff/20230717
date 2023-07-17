# Comparing `tmp/simple-alto-parser-0.0.6.tar.gz` & `tmp/simple-alto-parser-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-alto-parser-0.0.6.tar", last modified: Thu Jun  1 12:43:53 2023, max compression
+gzip compressed data, was "simple-alto-parser-0.0.8.tar", last modified: Mon Jul 17 13:30:49 2023, max compression
```

## Comparing `simple-alto-parser-0.0.6.tar` & `simple-alto-parser-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/simple_alto_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/alto_file_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/dictionary_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/dictionary_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/nlp_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/pattern_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-06-01 12:43:44.000000 simple-alto-parser-0.0.6/simple_alto_parser/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:43:53.372317 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 12:43:53.000000 simple-alto-parser-0.0.6/simple_alto_parser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/simple_alto_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8401 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9717 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/alto_file_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/dictionary_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/dictionary_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/nlp_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/pattern_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-17 13:30:38.000000 simple-alto-parser-0.0.8/simple_alto_parser/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:30:49.235575 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 13:30:49.000000 simple-alto-parser-0.0.8/simple_alto_parser.egg-info/top_level.txt
```

### Comparing `simple-alto-parser-0.0.6/LICENSE` & `simple-alto-parser-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/PKG-INFO` & `simple-alto-parser-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.6
+Version: 0.0.8
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `simple-alto-parser-0.0.6/setup.cfg` & `simple-alto-parser-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/alto_file.py` & `simple-alto-parser-0.0.8/simple_alto_parser/alto_file.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/alto_file_exporter.py` & `simple-alto-parser-0.0.8/simple_alto_parser/alto_file_exporter.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/alto_file_parser.py` & `simple-alto-parser-0.0.8/simple_alto_parser/alto_file_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains the class AltoTextParser, which is used to parse text from ALTO files."""
+import logging
 import os
 import re
 import sys
 import xml.etree.ElementTree as ETree
 from simple_alto_parser.alto_file import AltoFile, AltoFileElement
 from simple_alto_parser.utils import get_logger
 
@@ -19,33 +20,37 @@
     """A list of the attributes that should be stored in the element_data dictionary."""
 
     files = []
 
     def __init__(self, directory_path=None, parser_config=None):
         """The constructor of the class."""
 
-        self.logger = get_logger()
-
         self.parser_config = {
             'line_type': 'TextLine',
             'file_ending': '.xml',
             'export': {                            # Options for exporting the parsed data.
                 'csv': {
                     'print_manipulated': False,      # Print the manipulated text to the csv.
                     'print_filename': False,         # Print the filename to the csv.
                     'print_attributes': True,       # Print the attributes to the csv.
                     'print_parser_results': True,   # Print the parser results to the csv.
                     'print_file_meta_data': False,   # Print the file meta data to the csv.
                 }
+            },
+            'batches': [],
+            'logging': {
+                'level': logging.DEBUG,
             }
         }
 
         if parser_config:
             self.parser_config.update(parser_config)
 
+        self.logger = get_logger(self.parser_config['logging']['level'])
+
         self.logger.debug("Parser config: %s", self.parser_config)
 
         if directory_path:
             self.add_files(directory_path, self.get_config_value('file_ending'))
         else:
             self.files = []
 
@@ -89,14 +94,34 @@
     def parse(self):
         """Parse the text from all files in the list of files."""
 
         for alto_file in self.files:
             self.parse_file(alto_file)
         self.logger.info(f"Parsed text from {len(self.files)} files.")
 
+    def parse_part(self, parsing_function, name, pages):
+        page_list = self.get_page_list(pages)
+        executed_pages = []
+
+        for alto_file in self.files:
+            for line in alto_file.get_text_lines():
+                current_page = int(alto_file.file_meta_data['page'])
+                if current_page in page_list:
+                    parsing_function(self)
+                    executed_pages.append(current_page)
+
+        items_to_remove = set(executed_pages)
+        remaining = list(filter(lambda x: x not in items_to_remove, page_list))
+
+        if len(remaining) > 0:
+            self.logger.warning(f"Could not parse '{name}' pages {remaining}.")
+
+
+
+
     def parse_file(self, alto_file):
         """This function parses the alto file and stores the data in the class."""
 
         xml_tree, xmlns = self._xml_parse_file(alto_file.file_path)
         if xml_tree is None:
             raise ValueError("The given file is not a valid xml file.")
```

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/base_parser.py` & `simple-alto-parser-0.0.8/simple_alto_parser/pattern_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,57 +1,69 @@
-from simple_alto_parser.utils import get_logger
+import re
 
+from simple_alto_parser import BaseParser
+from simple_alto_parser.base_parser import ParserMatch
 
-class BaseParser:
 
-    logger = None
+class AltoPatternParser(BaseParser):
+
     matches = []
 
     def __init__(self, parser):
-        """The constructor of the class. It initializes the list of files.
-        The lines are a list of AltoXMLElement objects."""
-        self.logger = get_logger()
-        self.parser = parser
-        self.matches = []
+        """The constructor of the class."""
+        super().__init__(parser)
+
+    def find(self, pattern):
+        """Find a pattern in the text lines."""
+        self.clear()
+
+        fidx = 0
+        for file in self.parser.get_alto_files():
+            if self.is_in_batch(file):
+                lidx = 0
+                for line in file.get_text_lines():
+                    print(f"Search in file: {pattern}")
+                    match = re.search(pattern, line.get_text())
+                    if match:
+                        self.matches.append(PatternMatch(pattern, fidx, lidx, match))
+                    lidx += 1
+            else:
+                print("Not in batch")
+
+            fidx += 1
 
-    def mark(self, name, value):
+        return self
+
+    def categorize(self, category):
         """Add the given category to all matches."""
         for match in self.matches:
-            self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].add_parser_data(name, value)
+            if type(category) == str:
+                self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id]\
+                    .add_parser_data(category, match.match.group(1))
+            if type(category) == list:
+                c_id = 1
+                for c in category:
+                    self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id]\
+                        .add_parser_data(c, match.match.group(c_id))
+                    c_id += 1
         return self
 
-    def clear(self):
-        self.matches = []
+    def remove(self, replacement=''):
+        """Remove all matched patterns from matching lines."""
+        for match in self.matches:
+            self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].set_text(
+                re.sub(match.pattern, replacement,
+                       self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].get_text()))
         return self
 
-    def print_matches(self):
-        """Print all matches."""
-        for match in self.matches:
-            print("Found pattern '%s' in line '%s'." %
-                  (match,
-                   self.parser.get_alto_files()[match.file_id].get_text_lines()[match.line_id].get_text()))
+    def replace(self, replacement):
+        self.remove(replacement)
         return self
 
-    def get_unmatched(self):
-        """Return all unmatched lines."""
-        match_ids = []
-        for match in self.matches:
-            match_ids.append((match.file_id, match.line_id))
 
-        unmatched = []
-        file_id = 0
-        for file in self.parser.get_alto_files():
-            line_id = 0
-            for line in file.get_text_lines():
-                if (file_id, line_id) not in match_ids:
-                    unmatched.append(line.get_text())
-                line_id += 1
-            file_id += 1
-        return unmatched
+class PatternMatch(ParserMatch):
 
+    pattern = None
 
-class ParserMatch:
-
-    def __init__(self, file_id, line_id, match):
-        self.file_id = file_id
-        self.line_id = line_id
-        self.match = match
+    def __init__(self, pattern, file_id, line_id, match):
+        super().__init__(file_id, line_id, match)
+        self.pattern = pattern
```

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/dictionary_creator.py` & `simple-alto-parser-0.0.8/simple_alto_parser/dictionary_creator.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/dictionary_parser.py` & `simple-alto-parser-0.0.8/simple_alto_parser/dictionary_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,59 +13,61 @@
 
     def __init__(self, parser):
         """The constructor of the class. It initializes the list of files.
         The lines are a list of AltoXMLElement objects."""
         super().__init__(parser)
 
     def load(self, dictionary_file):
-        self.logger.debug(f"PROBLEM: {dictionary_file}")
-        print("LOAD", dictionary_file)
-
+        """Load a dictionary from a json file."""
+        self.logger.info(f'Loading dictionary "{dictionary_file}"...')
+        all_variants = []
         dictionary = json.load(open(dictionary_file, encoding='utf-8'))
         for entry in dictionary:
             if 'label' in entry:
                 if 'variants' not in entry:
                     entry['variants'] = [entry['label']]
                 if 'type' not in entry:
                     entry['type'] = 'undefined'
 
                 entry['variants'] = [v.strip() for v in entry['variants']]
                 entry['variants'] = sorted(entry['variants'], key=len, reverse=True)
+
+                extended_variants = []
+                for v in entry['variants']:
+                    extended_variants.append((v, entry))
+                all_variants.extend(extended_variants)
             else:
                 self.logger.error(f'Dictionary Entry "{entry}" from dictionary "{dictionary_file}" has no label.')
                 sys.exit()
 
-        self.dictionaries.append(dictionary)
-        self.logger.debug(f"Loaded dictionary: {dictionary_file}")
+        all_variants = sorted(all_variants, key=len, reverse=True)
+        self.dictionaries.append(Dictionary(dictionary, all_variants))
+        self.logger.info(f"Loaded dictionary: {dictionary_file}")
 
     def find(self, strict=True, restrict_to=None):
         """Find a pattern in the text lines."""
         self.clear()
         file_id = 0
         for file in self.parser.get_alto_files():
             line_id = 0
             for line in file.get_text_lines():
                 for dictionary in self.dictionaries:
-                    for entry in dictionary:
-                        if restrict_to is not None and entry['type'] == restrict_to:
-                            match = None
-                            if strict:
-                                for v in entry['variants']:
-                                    match = v.strip('.').lower() == line.get_text().strip().strip('.').lower()
-                                    if match:
-                                        match = v
-                                        break
-                            else:
-                                for v in entry['variants']:
-                                    match = re.search(re.escape(v), line.get_text().strip())
-                                    if match:
-                                        break
-
+                    for variant in dictionary.all_variants:
+                        if restrict_to is not None and variant[1]['type'] != restrict_to:
+                            continue
+                        if strict:
+                            match = variant[0].strip('.').lower() == line.get_text().strip().strip('.').lower()
                             if match:
-                                self.matches.append(DictionaryMatch(file_id, line_id, match, entry))
+                                match = variant[0]
+                        else:
+                            match = re.search(re.escape(variant[0]), line.get_text().strip())
+
+                        if match:
+                            self.logger.debug(f"Found dictionary match '{variant[0]}' in line '{line.get_text()}'")
+                            self.matches.append(DictionaryMatch(file_id, line_id, match, variant[1]))
                 line_id += 1
             file_id += 1
         return self
 
     def categorize(self):
         """Add the given category to all matches."""
         for match in self.matches:
@@ -100,7 +102,16 @@
     def __init__(self, file_id, line_id, match, dict_entry={}):
         super().__init__(file_id, line_id, match)
         self.dict_entry = dict_entry
 
     def __str__(self):
         return super().__str__()
         # return self.match.group(0)
+
+class Dictionary:
+
+    dictionary = []
+    all_variants = []
+
+    def __init__(self, dictionary, all_variants):
+        self.dictionary = dictionary
+        self.all_variants = all_variants
```

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/nlp_parser.py` & `simple-alto-parser-0.0.8/simple_alto_parser/nlp_parser.py`

 * *Files identical despite different names*

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser/utils.py` & `simple-alto-parser-0.0.8/simple_alto_parser/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 import logging
 
 LOGGER = None
 
-def get_logger():
+def get_logger(level=None):
     """This function returns a logger instance for the package."""
 
     global LOGGER
 
     if LOGGER is not None:
         return LOGGER
 
     LOGGER = logging.getLogger("simple_alto_parser")
-    LOGGER.setLevel(logging.DEBUG)
+    if level is None:
+        level = logging.INFO
+    LOGGER.setLevel(level)
 
     formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
 
     ch = logging.StreamHandler()
     ch.setLevel(logging.DEBUG)
     ch.setFormatter(formatter)
     LOGGER.addHandler(ch)
```

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser.egg-info/PKG-INFO` & `simple-alto-parser-0.0.8/simple_alto_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-alto-parser
-Version: 0.0.6
+Version: 0.0.8
 Summary: A python module to read and parse ALTO files
 Home-page: https://simple-alto-parser.readthedocs.io/en/latest/
 Author: Sorin Marti, Lea Kasper
 Author-email: sorin.marti@gmail.com, lea.kasper@unibas.ch
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
```

### Comparing `simple-alto-parser-0.0.6/simple_alto_parser.egg-info/SOURCES.txt` & `simple-alto-parser-0.0.8/simple_alto_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

