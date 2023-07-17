# Comparing `tmp/plasmid_design-0.0.3.tar.gz` & `tmp/plasmid_design-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plasmid_design-0.0.3.tar", last modified: Sun Jun 11 21:29:14 2023, max compression
+gzip compressed data, was "plasmid_design-0.0.4.tar", last modified: Mon Jul 17 06:46:19 2023, max compression
```

## Comparing `plasmid_design-0.0.3.tar` & `plasmid_design-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.581647 plasmid_design-0.0.3/
--rw-r--r--   0 davidfeldman   (501) staff       (20)     1056 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/LICENSE.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:29:14.581510 plasmid_design-0.0.3/PKG-INFO
--rw-r--r--   0 davidfeldman   (501) staff       (20)     1861 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/README.md
--rw-r--r--   0 davidfeldman   (501) staff       (20)      878 2023-06-11 21:28:59.000000 plasmid_design-0.0.3/pyproject.toml
--rw-r--r--   0 davidfeldman   (501) staff       (20)       38 2023-06-11 21:29:14.581692 plasmid_design-0.0.3/setup.cfg
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.578857 plasmid_design-0.0.3/src/
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.580234 plasmid_design-0.0.3/src/plasmid_design/
--rw-r--r--   0 davidfeldman   (501) staff       (20)        0 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/__init__.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)      844 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/constants.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3333 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/drive.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     4285 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/idt_api.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)    15311 2023-06-11 21:25:25.000000 plasmid_design-0.0.3/src/plasmid_design/plasmid_design.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3057 2023-06-11 20:51:05.000000 plasmid_design-0.0.3/src/plasmid_design/sequence.py
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3076 2023-06-11 21:11:24.000000 plasmid_design-0.0.3/src/plasmid_design/utils.py
-drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-06-11 21:29:14.581290 plasmid_design-0.0.3/src/plasmid_design.egg-info/
--rw-r--r--   0 davidfeldman   (501) staff       (20)     3629 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/PKG-INFO
--rw-r--r--   0 davidfeldman   (501) staff       (20)      507 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/SOURCES.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)        1 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/dependency_links.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       70 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/entry_points.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       69 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/requires.txt
--rw-r--r--   0 davidfeldman   (501) staff       (20)       15 2023-06-11 21:29:14.000000 plasmid_design-0.0.3/src/plasmid_design.egg-info/top_level.txt
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-07-17 06:46:19.508355 plasmid_design-0.0.4/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     1056 2023-06-11 20:51:05.000000 plasmid_design-0.0.4/LICENSE.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     4246 2023-07-17 06:46:19.508233 plasmid_design-0.0.4/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     2478 2023-07-17 06:36:04.000000 plasmid_design-0.0.4/README.md
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      878 2023-07-17 06:41:25.000000 plasmid_design-0.0.4/pyproject.toml
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       38 2023-07-17 06:46:19.508386 plasmid_design-0.0.4/setup.cfg
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-07-17 06:46:19.505494 plasmid_design-0.0.4/src/
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-07-17 06:46:19.507319 plasmid_design-0.0.4/src/plasmid_design/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        0 2023-06-11 20:51:05.000000 plasmid_design-0.0.4/src/plasmid_design/__init__.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      844 2023-06-11 20:51:05.000000 plasmid_design-0.0.4/src/plasmid_design/constants.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3673 2023-07-17 06:39:08.000000 plasmid_design-0.0.4/src/plasmid_design/drive.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     4285 2023-06-11 20:51:05.000000 plasmid_design-0.0.4/src/plasmid_design/idt_api.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)    15356 2023-07-17 06:36:04.000000 plasmid_design-0.0.4/src/plasmid_design/plasmid_design.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3057 2023-06-11 20:51:05.000000 plasmid_design-0.0.4/src/plasmid_design/sequence.py
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     3076 2023-07-17 06:35:50.000000 plasmid_design-0.0.4/src/plasmid_design/utils.py
+drwxr-xr-x   0 davidfeldman   (501) staff       (20)        0 2023-07-17 06:46:19.508075 plasmid_design-0.0.4/src/plasmid_design.egg-info/
+-rw-r--r--   0 davidfeldman   (501) staff       (20)     4246 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/PKG-INFO
+-rw-r--r--   0 davidfeldman   (501) staff       (20)      507 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/SOURCES.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)        1 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/dependency_links.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       70 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/entry_points.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       69 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/requires.txt
+-rw-r--r--   0 davidfeldman   (501) staff       (20)       15 2023-07-17 06:46:19.000000 plasmid_design-0.0.4/src/plasmid_design.egg-info/top_level.txt
```

### Comparing `plasmid_design-0.0.3/LICENSE.txt` & `plasmid_design-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.3/pyproject.toml` & `plasmid_design-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plasmid_design"
-version = "0.0.3"
+version = "0.0.4"
 description = "Automated plasmid design from speadsheet specification"
 authors = [
   { name="David Feldman" },
 ]
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `plasmid_design-0.0.3/src/plasmid_design/constants.py` & `plasmid_design-0.0.4/src/plasmid_design/constants.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.3/src/plasmid_design/drive.py` & `plasmid_design-0.0.4/src/plasmid_design/drive.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from pathlib import Path
 
 import numpy as np
 import pandas as pd
 import pygsheets
 
 
-CSV_EXPORT_URL = ('https://docs.google.com/spreadsheets/d/{key}/gviz/'
-                  'tq?tqx=out:csv&sheet={sheet_name}')
+BASE_URL = 'https://docs.google.com/spreadsheets/d/{key}'
+CSV_EXPORT_URL = f'{BASE_URL}/gviz/tq?tqx=out:csv&sheet={{sheet_name}}'
 
 
 def find_service_file(search='*service*.json'):
     """Searches current path, then parent directories, then user home.
     """
     parent_paths = [os.getcwd()] + [str(x) for x in Path(os.getcwd()).parents]
     # ~/bii/cloud kept for cross-compatibility
@@ -33,15 +33,23 @@
         raise FileNotFoundError(f'no file matching {search}')
     
     return matches[0]
 
 
 def read_csv_from_url(key, sheet_name, skiprows=0, **kwargs):
     url = CSV_EXPORT_URL.format(key=key, sheet_name=sheet_name)
-    df = pd.read_csv(url, skiprows=skiprows)
+    try:
+        df = pd.read_csv(url, skiprows=skiprows)
+    except pd.errors.ParserError as e:
+        base_url = BASE_URL.format(key=key)
+        extra_info = (
+            '\n\nDid you remember to make this sheet public? '
+            f'\n{base_url}'
+            '\nClick Share > General access > Anyone with the link')
+        raise pd.errors.ParserError(str(e) + extra_info)
     return Drive.clean(df, **kwargs)
 
 
 class Drive():
     def __init__(self):
         if not os.path.exists(SERVICE_FILE):
             SERVICE_FILE = find_service_file()
```

### Comparing `plasmid_design-0.0.3/src/plasmid_design/idt_api.py` & `plasmid_design-0.0.4/src/plasmid_design/idt_api.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.3/src/plasmid_design/plasmid_design.py` & `plasmid_design-0.0.4/src/plasmid_design/plasmid_design.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 config_file = 'config.yaml'
 parts_table = 'parts.csv'
 binder_table = 'binders.csv'
 target_table = 'targets.csv'
 feature_table = 'features.csv'
 template_table = 'templates.csv'
-sites_to_avoid = 'reverse_translations/sites_to_avoid.csv'
+restriction_enzyme_table = 'reverse_translations/restriction_enzymes.csv'
 rt_input_fasta = 'reverse_translations/input.fa'
 rt_output_fasta = 'reverse_translations/output.fa'
 rt_idt_scores = 'reverse_translations/idt_scores.csv'
 gene_order_fasta = 'gene_order.fa'
 gene_idt_scores = 'gene_order_idt_scores.csv'
 
 always_avoid = '6xA', '5xG'
@@ -70,15 +70,15 @@
      .pipe(convert_benchling_features)
      .to_csv(feature_table, index=None)
     )
     load_yaml_table(c['templates']).to_csv(template_table, index=None)
     (load_yaml_table(c['restriction_enzymes'])
      .assign(site=lambda x: x['name'].apply(
         lambda y: getattr(Restriction, y).site))
-     .to_csv(sites_to_avoid, index=None)
+     .to_csv(restriction_enzyme_table, index=None)
     )
 
 
 def validate_template_table():
     """Check that templates are unique and that for each row,
     all of the parts occur in the template string. Helps to catch
     spreadsheet copying errors.
@@ -111,24 +111,24 @@
     write_fasta(rt_input_fasta, needs_rt[['name', 'aa']])
     
     # backwards compatibility
     if 'white_list' in df_features:
         (df_features['white_list'].dropna().rename('enzyme').pipe(pd.DataFrame)
         .assign(site=lambda x: x['enzyme'].apply(
             lambda y: getattr(Bio.Restriction, y).site))
-        .to_csv(sites_to_avoid, index=None)
+        .to_csv(restriction_enzyme_table, index=None)
         )
 
 
 def do_reverse_translations(skip_existing=False, **rt_args):
     """Use DNA Chisel to codon optimize with constraints. Save to fasta and individual 
     genbanks with DNA Chisel annotations. Only coding sequences!!
     """
     df_seqs = pd.DataFrame(read_fasta(rt_input_fasta), columns=('name', 'aa_seq'))
-    df_sites = pd.read_csv(sites_to_avoid)
+    df_sites = pd.read_csv(restriction_enzyme_table)
     
     translations = {}
     if skip_existing:
         if not os.path.exists(rt_output_fasta):
             skip_existing = False
         else:
             existing = dict(read_fasta(rt_output_fasta))
```

### Comparing `plasmid_design-0.0.3/src/plasmid_design/sequence.py` & `plasmid_design-0.0.4/src/plasmid_design/sequence.py`

 * *Files identical despite different names*

### Comparing `plasmid_design-0.0.3/src/plasmid_design/utils.py` & `plasmid_design-0.0.4/src/plasmid_design/utils.py`

 * *Files identical despite different names*

