# Comparing `tmp/py3seed-0.1.2.tar.gz` & `tmp/py3seed-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3seed-0.1.2.tar", last modified: Thu Jul 13 03:24:38 2023, max compression
+gzip compressed data, was "py3seed-0.1.3.tar", last modified: Mon Jul 17 08:13:19 2023, max compression
```

## Comparing `py3seed-0.1.2.tar` & `py3seed-0.1.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.708893 py3seed-0.1.2/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.2/LICENSE
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-13 03:24:38.709233 py3seed-0.1.2/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.2/README.md
--rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.2/pyproject.toml
--rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-13 03:24:38.710668 py3seed-0.1.2/setup.cfg
--rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.2/setup.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.683329 py3seed-0.1.2/src/
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.698010 py3seed-0.1.2/src/py3seed/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.2/src/py3seed/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.2/src/py3seed/__main__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.2/src/py3seed/admin.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.2/src/py3seed/cachesupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.703729 py3seed-0.1.2/src/py3seed/commands/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.2/src/py3seed/commands/__init__.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    20279 2023-07-13 03:08:33.000000 py3seed-0.1.2/src/py3seed/commands/gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.2/src/py3seed/error.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.2/src/py3seed/inflection.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.2/src/py3seed/log.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.2/src/py3seed/merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.2/src/py3seed/model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.2/src/py3seed/mongosupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14437 2023-07-13 03:03:17.000000 py3seed-0.1.2/src/py3seed/utils.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.2/src/py3seed/websupport.py
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.702476 py3seed-0.1.2/src/py3seed.egg-info/
--rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/PKG-INFO
--rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/SOURCES.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/dependency_links.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/entry_points.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/requires.txt
--rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-13 03:24:38.000000 py3seed-0.1.2/src/py3seed.egg-info/top_level.txt
-drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-13 03:24:38.707848 py3seed-0.1.2/tests/
--rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.2/tests/test_cachesupport.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     6126 2023-07-13 03:08:09.000000 py3seed-0.1.2/tests/test_gen.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.2/tests/test_merge3.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.2/tests/test_model.py
--rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.2/tests/test_mongosupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.858812 py3seed-0.1.3/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1072 2021-08-08 16:29:42.000000 py3seed-0.1.3/LICENSE
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:13:19.858969 py3seed-0.1.3/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      288 2021-08-11 03:57:41.000000 py3seed-0.1.3/README.md
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      104 2021-09-18 08:01:25.000000 py3seed-0.1.3/pyproject.toml
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      911 2023-07-17 08:13:19.859792 py3seed-0.1.3/setup.cfg
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      214 2023-07-06 08:35:28.000000 py3seed-0.1.3/setup.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.834321 py3seed-0.1.3/src/
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.847240 py3seed-0.1.3/src/py3seed/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      743 2023-07-10 07:31:29.000000 py3seed-0.1.3/src/py3seed/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1624 2023-07-10 03:47:01.000000 py3seed-0.1.3/src/py3seed/__main__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      992 2021-09-02 08:44:38.000000 py3seed-0.1.3/src/py3seed/admin.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6458 2023-07-10 03:55:28.000000 py3seed-0.1.3/src/py3seed/cachesupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.853145 py3seed-0.1.3/src/py3seed/commands/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      151 2021-09-01 02:10:05.000000 py3seed-0.1.3/src/py3seed/commands/__init__.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    20437 2023-07-17 08:12:35.000000 py3seed-0.1.3/src/py3seed/commands/gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      732 2023-06-27 01:48:25.000000 py3seed-0.1.3/src/py3seed/error.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    11554 2023-07-10 03:49:24.000000 py3seed-0.1.3/src/py3seed/inflection.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     1166 2022-05-06 11:35:05.000000 py3seed-0.1.3/src/py3seed/log.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    17725 2023-07-11 02:10:39.000000 py3seed-0.1.3/src/py3seed/merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    57699 2023-07-13 02:24:43.000000 py3seed-0.1.3/src/py3seed/model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14489 2023-07-10 03:55:58.000000 py3seed-0.1.3/src/py3seed/mongosupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14313 2023-07-17 08:10:25.000000 py3seed-0.1.3/src/py3seed/utils.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     7471 2023-07-10 03:54:22.000000 py3seed-0.1.3/src/py3seed/websupport.py
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.852018 py3seed-0.1.3/src/py3seed.egg-info/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      859 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/PKG-INFO
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      718 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/SOURCES.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        1 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/dependency_links.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)      111 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/entry_points.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)       48 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/requires.txt
+-rw-r--r--   0 weiminfeng   (501) staff       (20)        8 2023-07-17 08:13:19.000000 py3seed-0.1.3/src/py3seed.egg-info/top_level.txt
+drwxr-xr-x   0 weiminfeng   (501) staff       (20)        0 2023-07-17 08:13:19.857980 py3seed-0.1.3/tests/
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     3216 2022-12-09 02:58:18.000000 py3seed-0.1.3/tests/test_cachesupport.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     6333 2023-07-13 03:38:58.000000 py3seed-0.1.3/tests/test_gen.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)    14977 2023-07-10 03:39:53.000000 py3seed-0.1.3/tests/test_merge3.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     5116 2023-07-05 06:36:00.000000 py3seed-0.1.3/tests/test_model.py
+-rw-r--r--   0 weiminfeng   (501) staff       (20)     2083 2023-07-05 06:36:25.000000 py3seed-0.1.3/tests/test_mongosupport.py
```

### Comparing `py3seed-0.1.2/LICENSE` & `py3seed-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/PKG-INFO` & `py3seed-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.2/setup.cfg` & `py3seed-0.1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = py3seed
-version = 0.1.2
+version = 0.1.3
 author = Samuel Feng
 author_email = okosioc@gmail.com
 description = A package that bootstraps your project by simple data models definition and auto api and user interface generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/okosioc/pyseed
 project_urls =
```

### Comparing `py3seed-0.1.2/src/py3seed/__init__.py` & `py3seed-0.1.3/src/py3seed/__init__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/__main__.py` & `py3seed-0.1.3/src/py3seed/__main__.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/admin.py` & `py3seed-0.1.3/src/py3seed/admin.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/cachesupport.py` & `py3seed-0.1.3/src/py3seed/cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/commands/gen.py` & `py3seed-0.1.3/src/py3seed/commands/gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from typing import List
 
 from flask import request
 from jinja2 import Environment, TemplateSyntaxError, FileSystemLoader
 from werkzeug.urls import url_quote, url_encode
 
 from py3seed import registered_models, BaseModel, TemplateError, LayoutError
-from py3seed.utils import work_in, generate_names, iterate_layout, parse_layout
+from py3seed.utils import work_in, generate_names, get_layout_fields, parse_layout
 from py3seed.merge3 import Merge3
 
 logger = logging.getLogger('pyseed')
 
 
 def _prepare_jinja2_env():
     """ Prepare env for rendering jinja2 templates. """
@@ -96,49 +96,53 @@
         #
         for f in fields:
             if matcher.match(f):
                 return f
         # If no matching, return nothing
         return None
 
-    def parse_layout_fields(schema, action):
-        """ Parse layout fields.
+    def parse_layout_fields(layout):
+        """ Get layout fields.
 
-        each column in layout can be blank('')/hyphen(-)/group(integer&float)/field(string) suffixed with query and span string
+        each column in layout can be blank('')/hyphen(-)/group(integer&float)/field(string) suffixed with query and format-span string
         this function will return a list of field names.
         """
-        return list(iterate_layout(schema[action], schema['groups']))
+        return list(get_layout_fields(layout))
 
     env.globals['update_query'] = update_query
     env.globals['new_model'] = new_model
     env.globals['match_field'] = match_field
     env.globals['parse_layout_fields'] = parse_layout_fields
     #
     return env
 
 
 def _gen(ms: str, ds: str):
     """ Gen. """
-    logger.info(f'Gen for domain(s) {ms} under domain(s) {ds}')
     include_models = [m.strip() for m in ms.split(',')] if ms else []
     include_domains = [d.strip() for d in ds.split(',')] if ds else []
+    logger.info(f'Gen for domain(s) {include_models} under domain(s) {include_domains}')
     # Domains should be project folders, i.e, [www, miniapp, android, ios, ...]
     for d in include_domains:
         if not os.path.exists(d):
             logger.error(f'Can not find domain {d}')
             return False
     #
     # Load all model's schema and views
     # 1. Find all the models definition in core.models package, please import all models in __init__.py
     # 2. Load each models' schema and views, filtering models and views that needs to be generated
     #
     model_settings = {}
     domain_names, view_names = set(), set()
     module_name = 'models'
-    module_spec = importlib.util.spec_from_file_location(module_name, os.path.join('core', module_name, '__init__.py'))
+    module_path = os.path.join('core', module_name, '__init__.py')
+    if not os.path.exists(module_path):
+        logger.error(f'Package does NOT exist at {module_path}')
+        return False
+    module_spec = importlib.util.spec_from_file_location(module_name, module_path)
     module = importlib.util.module_from_spec(module_spec)
     sys.modules[module_name] = module
     module_spec.loader.exec_module(module)
     logger.info(f'Load models:')
     for attr in dir(module):
         attribute = getattr(module, attr)
         if inspect.isclass(attribute) and issubclass(attribute, BaseModel):
```

### Comparing `py3seed-0.1.2/src/py3seed/error.py` & `py3seed-0.1.3/src/py3seed/error.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/inflection.py` & `py3seed-0.1.3/src/py3seed/inflection.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/log.py` & `py3seed-0.1.3/src/py3seed/log.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/merge3.py` & `py3seed-0.1.3/src/py3seed/merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/model.py` & `py3seed-0.1.3/src/py3seed/model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/mongosupport.py` & `py3seed-0.1.3/src/py3seed/mongosupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed/utils.py` & `py3seed-0.1.3/src/py3seed/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -103,18 +103,18 @@
     Return {action, params, rows}
     e.g,
     {
         action: form
         params: {
             param: 1,
         },
-        rows: [                         # each column is a dict, which has name/params/span and inner rows
+        rows: [[                         # each column is a dict, which has name/params/format/span and inner rows
             {name: $, rows:[...]},
             {name: 0, rows:[...]},
-        ]
+        ]]
     }
     """
 
     def _parse_lines(level, _lines, _schema):
         """ Recursively parse lines. """
         leading = '-' * ((level + 1) * 2)  # 2 spaces for each level
         # logger.debug('Parse lines:\n' + '\n'.join(_lines))
@@ -157,15 +157,15 @@
                     pass
                 else:
                     keys = _schema['properties'].keys()  # type of _schema is always a object
                     if col_name not in keys:
                         raise LayoutError(f'Field {col_name} not found in schema')
             # Has inner layout
             if len(segment) > 1:
-                logger.debug(f'{leading} Parsing level {level} segment:\n' + '\n'.join(segment))
+                # logger.debug(f'{leading} Parsing level {level} segment:\n' + '\n'.join(segment))
                 body_lines = segment[1:]
                 # Inject layout for each column
                 for j in range(0, len(columns)):
                     column = columns[j]
                     col_name = column['name']
                     start_position = index_line.index(column['raw'])
                     if j < len(columns) - 1:
@@ -311,31 +311,28 @@
     return {
         'action': action,
         'params': params,
         'rows': rows
     }
 
 
-def iterate_layout(layout, groups=[]):
-    """ Each column in layout can be blank('')/hyphen(-)/summary($)/group(number)/field(string)/inner fields(has children), iterate the whole layout and return field names only.
-
-    :param layout: Parsed layout
-    :param groups: Group index in layout need to refer to this list
-    :return:
-    """
+def get_layout_fields(layout):
+    """ Do not recursively parse inner object/array, only return current level field names. """
     for row in layout:
         for col in row:
             col_name = col['name']
-            if col.get('children'):
-                yield from iterate_layout([col['children']], groups)
-            elif col_name.isdigit():
-                yield from iterate_layout(groups[int(col_name)], groups)
-            elif col_name in ('', '-', '$'):
+            if not col_name:
+                pass
+            elif col_name == '-':
                 pass
+            elif col_name.replace('.', '').isdigit():
+                # Need to get fields under a group
+                yield get_layout_fields(col['rows'])
             else:
+                # Return current level field names, do not recursively parse inner object/array
                 yield col_name
 
 
 class Pagination(object):
     """ Pagination support. """
 
     def __init__(self, page, per_page, total_count):
```

### Comparing `py3seed-0.1.2/src/py3seed/websupport.py` & `py3seed-0.1.3/src/py3seed/websupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/src/py3seed.egg-info/PKG-INFO` & `py3seed-0.1.3/src/py3seed.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3seed
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package that bootstraps your project by simple data models definition and auto api and user interface generation
 Home-page: https://github.com/okosioc/pyseed
 Author: Samuel Feng
 Author-email: okosioc@gmail.com
 Project-URL: Bug Tracker, https://github.com/okosioc/pyseed/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `py3seed-0.1.2/src/py3seed.egg-info/SOURCES.txt` & `py3seed-0.1.3/src/py3seed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/tests/test_cachesupport.py` & `py3seed-0.1.3/tests/test_cachesupport.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/tests/test_gen.py` & `py3seed-0.1.3/tests/test_gen.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,32 +18,32 @@
 from .core.models import User, Team
 
 
 def test_layout_parsing():
     """ Test layout parsing. """
     # User profile
     user_profile_layout = '''#!form?title=User
-        1#summary4,  2#8                                           
-          avatar       name  
-          name         phone                                                  
-          status       intro                                                 
-          roles        avatar                                                
-          email
+        1#summary4,    2#8                                           
+          avatar         name  
+          name           phone                                                  
+          status         intro                                                 
+          roles          avatar                                                
+          email          point#4,
           phone
           create_time
     '''
     user_schema = User.schema()
     # Team members
     team_members_layout = '''#!read?title=Members
-        1#summary4,  members#8                                                  
-          logo         avatar, name, status, roles, email, phone, team_join_time
-          name
-          phone                                                              
-          members                                                                 
-          create_time
+        1#summary4,    members#8                                                  
+          logo           avatar, name, status, roles, email, phone, team_join_time
+          name         
+          phone                                                                
+          members                                                                   
+          create_time  
     '''
     team_schema = Team.schema()
 
     #
     # Validation
     #
 
@@ -83,16 +83,19 @@
     assert len(layout['rows']) == 1
     first_row = layout['rows'][0]
     assert first_row[0]['name'] == '1'
     assert first_row[0]['format'] == 'summary'
     assert first_row[0]['span'] == 4
     assert len(first_row[0]['rows']) == 7
     assert first_row[0]['rows'][0][0]['name'] == 'avatar'
-    assert len(first_row[1]['rows']) == 4
+    assert len(first_row[1]['rows']) == 5
     assert first_row[1]['rows'][1][0]['name'] == 'phone'
+    assert first_row[1]['rows'][4][0]['name'] == 'point'
+    assert first_row[1]['rows'][4][0]['span'] == 4
+    assert first_row[1]['rows'][4][1]['name'] == ''
 
     # Team member layout
     layout = parse_layout(team_members_layout, team_schema)
     assert layout['action'] == 'read'
     first_row = layout['rows'][0]
     assert len(first_row[1]['rows'][0]) == 7
     assert first_row[1]['rows'][0][0]['name'] == 'avatar'
```

### Comparing `py3seed-0.1.2/tests/test_merge3.py` & `py3seed-0.1.3/tests/test_merge3.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/tests/test_model.py` & `py3seed-0.1.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `py3seed-0.1.2/tests/test_mongosupport.py` & `py3seed-0.1.3/tests/test_mongosupport.py`

 * *Files identical despite different names*

