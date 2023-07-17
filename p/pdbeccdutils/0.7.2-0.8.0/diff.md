# Comparing `tmp/pdbeccdutils-0.7.2.tar.gz` & `tmp/pdbeccdutils-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbeccdutils-0.7.2.tar", last modified: Wed Apr 12 07:41:40 2023, max compression
+gzip compressed data, was "pdbeccdutils-0.8.0.tar", last modified: Mon Jul 17 12:20:04 2023, max compression
```

## Comparing `pdbeccdutils-0.7.2.tar` & `pdbeccdutils-0.8.0.tar`

### file list

```diff
@@ -1,78 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils/computations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/computations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/computations/parity_method.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19810 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/bm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    13337 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    44291 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    25946 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15066 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/depictions.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/fragment_library.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7973 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/templates.mae
--rw-r--r--   0 runner    (1001) docker     (123)   160441 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/fragment_library.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/adamantane.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/cube.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/hem.sdf
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/nonbornane.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/phorbine.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphin.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphycene.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex.sdf
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex2.sdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/cif_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/helpers/mol_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.398847 pdbeccdutils-0.7.2/pdbeccdutils/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14092 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/scripts/setup_pubchem_library_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/pdbeccdutils/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_bound_molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_file_writing.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_fragment_library.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_inchi_key_matches.py
--rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_load_eoh_cif.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_parity.py
--rw-r--r--   0 runner    (1001) docker     (123)     5391 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_process_components_cif_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_property_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_rdkit_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_scaffold_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_web_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/test_write_img.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/tests/tst_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/pdbeccdutils/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4362 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/pubchem_downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/pdbeccdutils/utils/web_services.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 07:41:40.394847 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4829 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-12 07:41:40.000000 pdbeccdutils-0.7.2/pdbeccdutils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 07:41:40.402848 pdbeccdutils-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-12 07:41:30.000000 pdbeccdutils-0.7.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.353982 pdbeccdutils-0.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-17 12:20:04.353982 pdbeccdutils-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.337982 pdbeccdutils-0.8.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     5104 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/doc/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.337982 pdbeccdutils-0.8.0/pdbeccdutils/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.341982 pdbeccdutils-0.8.0/pdbeccdutils/computations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/computations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/computations/parity_method.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.341982 pdbeccdutils-0.8.0/pdbeccdutils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/boundmolecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/ccd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44183 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/ccd_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21301 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/clc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17458 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/clc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26896 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15219 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/depictions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4029 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/fragment_library.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12504 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/prd_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14037 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/core/prd_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.341982 pdbeccdutils-0.8.0/pdbeccdutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.341982 pdbeccdutils-0.8.0/pdbeccdutils/data/coordgen_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10551 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/coordgen_templates/templates.mae
+-rw-r--r--   0 runner    (1001) docker     (123)   160441 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/fragment_library.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.345982 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/adamantane.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/cube.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/decahydrocorrin.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/hem.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/nonbornane.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/phorbine.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/porphin.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/porphycene.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/ru_complex.sdf
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/ru_complex2.sdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.345982 pdbeccdutils-0.8.0/pdbeccdutils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/cif_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11760 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4485 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9761 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/helpers/mol_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.345982 pdbeccdutils-0.8.0/pdbeccdutils/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/scripts/boundmolecule_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14897 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/scripts/process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/scripts/setup_pubchem_library_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.353982 pdbeccdutils-0.8.0/pdbeccdutils/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_bound_molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_boundmolecule_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_clc_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_clc_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10398 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_file_writing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_fragment_library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_inchi_key_matches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_load_eoh_cif.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_parity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5443 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_process_components_cif_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_property_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_rdkit_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_residue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_scaffold_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_web_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/test_write_img.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/tests/tst_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.353982 pdbeccdutils-0.8.0/pdbeccdutils/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/utils/pubchem_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/pdbeccdutils/utils/web_services.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:20:04.337982 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 12:20:04.000000 pdbeccdutils-0.8.0/pdbeccdutils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 12:20:04.353982 pdbeccdutils-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-17 12:19:43.000000 pdbeccdutils-0.8.0/setup.py
```

### Comparing `pdbeccdutils-0.7.2/LICENSE` & `pdbeccdutils-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/PKG-INFO` & `pdbeccdutils-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.7.2
+Version: 0.8.0
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
 Keywords: PDB CCD wwPDB small molecule
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 [![CodeFactor](https://www.codefactor.io/repository/github/pdbeurope/ccdutils/badge/master)](https://www.codefactor.io/repository/github/pdbeurope/ccdutils/overview/master)  ![PYPi](https://img.shields.io/pypi/v/pdbeccdutils?color=green&style=flat)  ![GitHub](https://img.shields.io/github/license/pdbeurope/ccdutils)   ![ccdutils documentation](https://github.com/PDBeurope/ccdutils/workflows/ccdutils%20documentation/badge.svg) ![ccdutils tests](https://github.com/PDBeurope/ccdutils/workflows/ccdutils%20tests/badge.svg)
```

### Comparing `pdbeccdutils-0.7.2/README.md` & `pdbeccdutils-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/doc/conf.py` & `pdbeccdutils-0.8.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/computations/parity_method.py` & `pdbeccdutils-0.8.0/pdbeccdutils/computations/parity_method.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/bm_reader.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/clc_reader.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,44 +12,62 @@
 # software distributed under the License is distributed on
 # an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """
-A set of methods for reading in data of PDB model cif files and creating an array of
-internal representation of bound molecules. The basic use can be as easy as this:
-
-    from pdbeccdutils.core import bm_reader
-
-    bound_molecules = bm_reader.read_pdb_updated_cif_file('/path/to/cif/xxx_updated.cif')
-    for i in bound_molecules:
-        rdkit_mol = i.component.mol
-        rdkit_inchikey = i.component.inchikey_from_rdkit
+A set of methods for identifying bound-molecules (covalently bonded CCDs ) from mmCIF files
+of proteins and creating Component representation of molecules.
 """
 
 import os
 import rdkit
+import logging
+from datetime import date
+from collections import namedtuple
+from gemmi import cif
+from networkx import MultiDiGraph
+
 from rdkit.Chem.rdMolDescriptors import CalcMolFormula
-from pdbeccdutils.core import ccd_reader
+from pdbeccdutils.core.exceptions import CCDUtilsError
+from pdbeccdutils.core import ccd_reader, models
+from pdbeccdutils.core.boundmolecule import infer_bound_molecules
+from pdbeccdutils.utils import config
 from pdbeccdutils.core.component import Component
-
 from pdbeccdutils.core.models import (
     CCDProperties,
     ConformerType,
+    ReleaseStatus,
     Descriptor,
-    Residue,
-    BoundMolecule,
 )
 from pdbeccdutils.helpers import cif_tools, conversions, mol_tools, helper
-from gemmi import cif
-from networkx import DiGraph, connected_components
 
+# categories that need to be 'fixed'
+# str => list[str]
+
+preprocessable_categories = [
+    "_chem_comp_atom.",
+    "_chem_comp_bond.",
+    "_pdbx_chem_comp_descriptor.",
+    "_chem_comp.",
+]
+
+
+CLCReaderResult = namedtuple(
+    "CLCReaderResult", ccd_reader.CCDReaderResult._fields + ("bound_molecule",)
+)
 
-def read_pdb_updated_cif_file(path_to_cif: str, sanitize: bool = True):
+
+def read_pdb_cif_file(
+    path_to_cif: str,
+    to_discard: set[str] = config.DISCARDED_RESIDUES,
+    sanitize: bool = True,
+    assembly: bool = False,
+) -> list[CLCReaderResult]:
     """
     Read in single wwPDB Model CIF and create internal
     representation of its bound-molecules with multiple components.
 
     Args:
         path_to_cif (str): Path to the cif file
         sanitize (bool): [Defaults: True]
@@ -60,522 +78,592 @@
     Returns:
         A list of CCDResult representations of each bound-molecule.
     """
     if not os.path.isfile(path_to_cif):
         raise ValueError(f"File '{path_to_cif}' does not exists")
 
     biomolecule_result = []
-    bms = infer_bound_molecules(path_to_cif, ["HOH"])
-    for bm in bms:
-        reader_result = infer_multiple_chem_comp(path_to_cif, bm.to_dict(), sanitize)
+    bms = infer_bound_molecules(path_to_cif, to_discard, assembly)
+    for i, bm in enumerate(bms, start=1):
+        bm_id = f"bm{i}"
+        reader_result = infer_multiple_chem_comp(path_to_cif, bm, bm_id, sanitize)
         if reader_result:
             biomolecule_result.append(reader_result)
 
     return biomolecule_result
 
 
-def infer_multiple_chem_comp(path_to_cif: str, bm: dict, sanitize: bool = True):
-    """
-    Read in single wwPDB Model CIF and single bound-molecule to create internal
-    representation of the bound molecule.
-
-    Args:
-        path_to_cif (str): Path to the cif file
-        bm (dict): Dictionary representation of bound-molecule
-        sanitize (bool): [Defaults: True]
+def infer_multiple_chem_comp(path_to_cif, bm, bm_id, sanitize=True):
 
+    """Args:
+        path_to_cif: Path to input structure
+        bm: bound-molecules identified from input structure
+        bm_id: ID of bound-molecule
+        sanitize: True if bound-molecule need to be sanitized
 
     Returns:
-        A dictionary of CCDResult representation of bound-molecule.
+        CLCReaderResult: Namedtuple containing Component representation of bound-molecule
+
     """
 
-    if len(bm["residues"]) <= 1:
+    if bm.graph.number_of_nodes() <= 1 or bm.id != bm.orig_id:
         return
 
+    cif_block = cif.read(path_to_cif).sole_block()
+    (mol, warnings, errors) = _parse_pdb_mmcif(cif_block, bm.graph)
+    sanitized = False
+    if sanitize:
+        sanitized = mol_tools.sanitize(mol)
+
+    inchi_result = mol_tools.inchi_from_mol(mol)
+    if inchi_result.warnings:
+        warnings.append(inchi_result.warnings)
+    if inchi_result.errors:
+        errors.append(inchi_result.errors)
+
+    inchikey = mol_tools.inchikey_from_inchi(inchi_result.inchi)
+    descriptors = [
+        Descriptor(
+            type="SMILES",
+            program="rdkit",
+            program_version=rdkit.__version__,
+            value=rdkit.Chem.MolToSmiles(mol),
+        ),
+        Descriptor(
+            type="InChI",
+            program="rdkit",
+            program_version=rdkit.__version__,
+            value=inchi_result.inchi,
+        ),
+        Descriptor(
+            type="InChIKey",
+            program="rdkit",
+            program_version=rdkit.__version__,
+            value=inchikey,
+        ),
+    ]
+
+    # define release category based on warnings or errors
+    pdbx_release_status = models.ReleaseStatus.NOT_SET
+    if warnings or errors:
+        pdbx_release_status = models.ReleaseStatus.HOLD
     else:
-        warnings = []
-        errors = []
-        sanitized = False
-        cif_block = cif.read(path_to_cif).sole_block()
-        cif_tools.preprocess_cif_category(cif_block, "_atom_site.")
-        cif_tools.preprocess_cif_category(cif_block, "_chem_comp_bond.")
-
-        mol = rdkit.Chem.RWMol()
-        index_atoms, bm_atoms_dict = _parse_pdb_atom_site(
-            mol, cif_block.get_mmcif_category("_atom_site."), bm
-        )
-        _parse_pdb_conformers_site(mol, bm_atoms_dict, index_atoms)
-        _parse_pdb_bonds_site(
-            mol,
-            cif_block.get_mmcif_category("_chem_comp_bond."),
-            bm_atoms_dict,
-            errors,
-            index_atoms,
-            bm,
-        )
+        pdbx_release_status = models.ReleaseStatus.REL
 
-        _handle_disconnected_hydrogens(mol)
-        if sanitize:
-            sanitized = mol_tools.sanitize(mol)
-
-        comp = Component(mol.GetMol(), cif_block)
-        descriptors = [
-            Descriptor(type="InChI", program="rdkit", value=comp.inchi_from_rdkit),
-            Descriptor(
-                type="InChIKey", program="rdkit", value=comp.inchikey_from_rdkit
-            ),
-        ]
-        properties = CCDProperties(
-            id="",
-            name="",
-            formula=CalcMolFormula(comp.mol),
-            modified_date="",
-            pdbx_release_status="",
-            weight="",
-        )
-        comp = Component(mol.GetMol(), cif_block, properties, descriptors)
-        reader_result = ccd_reader.CCDReaderResult(
-            warnings=warnings, errors=errors, component=comp, sanitized=sanitized
-        )
+    properties = CCDProperties(
+        id=bm_id,
+        name=bm.name,
+        formula=CalcMolFormula(mol),
+        modified_date=date.today(),
+        pdbx_release_status=pdbx_release_status,
+        weight="",
+    )
+
+    comp = Component(mol, None, properties, descriptors)
+
+    reader_result = CLCReaderResult(
+        warnings=warnings,
+        errors=errors,
+        component=comp,
+        bound_molecule=bm,
+        sanitized=sanitized,
+    )
 
-        return reader_result
+    return reader_result
 
 
-def _handle_disconnected_hydrogens(mol):
+def _parse_pdb_mmcif(
+    cif_block: cif.Block, bm: models.BoundMolecule
+) -> tuple[rdkit.Chem.rdchem.Mol, list[str], list[str]]:
     """
-    Delete hydrogens without neighbours (degree = 0).
-    RDKit works but gives warning for these ("WARNING: not removing hydrogen atom without neighbors").
-    However we wouldn't want these hydrogens as they affect molecular properties.
+    Create internal representation of the molecule from mmcif format.
 
     Args:
-        mol (rdkit.Chem.rchem.Mol): Rdkit Mol object with the
-            compound representation.
+        cif_block (cif.Block): mmcif block object from gemmi
+        sanitize (bool): Whether or not the rdkit component should
+            be sanitized. Defaults to True.
+
+    Returns:
+        CCDReaderResult: internal representation with the results
+            of parsing and Mol object.
     """
-    disconnected_hydrogens = [
-        atom
-        for atom in mol.GetAtoms()
-        if atom.GetAtomicNum() == 1 and atom.GetDegree() == 0
-    ]
-    atoms_to_remove = [atom.GetIdx() for atom in disconnected_hydrogens]
-    atoms_to_remove.sort(reverse=True)
+    warnings = []
+    errors = []
+    mol = rdkit.Chem.RWMol()
+    preprocessable_categories = ["_atom_site.", "_chem_comp_bond."]
 
-    for atom in atoms_to_remove:
-        mol.RemoveAtom(atom)
+    for c in preprocessable_categories:
+        w = cif_tools.preprocess_cif_category(cif_block, c)
 
+        if w:
+            warnings.append(w)
 
-def _parse_pdb_atom_site(mol, atoms, bm):
-    """
-    Setup atoms in the bound molecule
+    bm_atoms = _get_boundmolecule_atoms(cif_block, bm)
 
-    Args:
-        mol (rdkit.Chem.rchem.Mol): RDkit Mol object with the
-            compound representation.
-        atoms (dict): dictionary with parsed _chem_comp_atom
-            category.
-        bm (dict): dictionary representation of bound-molecule
-    """
-    if not atoms:
-        return
+    _parse_pdb_atoms(mol, bm_atoms)
+    _parse_pdb_conformers(mol, bm_atoms)
+    _parse_pdb_bonds(mol, bm, cif_block, errors)
+    _add_connections(mol, bm, errors)
+    mol = _handle_hydrogens(mol)
+    return (mol, warnings, errors)
 
-    exclude_alternate_atoms = True
-    if exclude_alternate_atoms:
-        seen = {}
 
-    index_atoms = []
-    bm_atoms_dict = {}
+def _get_boundmolecule_atoms(cif_block, bm):
+    if "_atom_site." not in cif_block.get_mmcif_category_names():
+        return
 
+    atoms = cif_block.get_mmcif_category("_atom_site.")
+    bm_atoms = {key: [] for key in atoms}
     for i in range(len(atoms["id"])):
-        if atoms["group_PDB"][i] != "HETATM":  # only consider nonpolys
-            continue
-        for j in bm["residues"]:
-            if (
-                atoms["label_comp_id"][i] == j["label_comp_id"]
-                and atoms["auth_asym_id"][i] == j["auth_asym_id"]
-                and atoms["auth_seq_id"][i] == j["auth_seq_id"]
-            ):
-                atom_tuple = (
-                    atoms["auth_seq_id"][i],
-                    atoms["auth_atom_id"][i],
-                    atoms["auth_comp_id"][i],
-                )
-                if exclude_alternate_atoms:
-                    if atom_tuple in seen:
-                        continue
-                    seen[atom_tuple] = True
-
-                for categories in atoms:
-                    if categories not in bm_atoms_dict:
-                        bm_atoms_dict[categories] = []
-                    else:
-                        bm_atoms_dict[categories].append(atoms[categories][i])
-
-                element = atoms["type_symbol"][i]
-                element = (
-                    element if len(element) == 1 else element[0] + element[1].lower()
-                )
-                isotope = None
+        if atoms["group_PDB"][i] == "HETATM":
+            for residue in bm.nodes():
+                if (
+                    atoms["label_comp_id"][i] == residue.name
+                    and atoms["auth_asym_id"][i] == residue.chain
+                    and atoms["auth_seq_id"][i] == residue.res_id
+                ):
+                    for key in bm_atoms:
+                        bm_atoms[key].append(atoms[key][i])
 
-                if element == "D":
-                    element = "H"
-                    isotope = 2
-                elif element == "X":
-                    element = "*"
-
-                atom = rdkit.Chem.Atom(element)
-                atom.SetProp("name", "/".join(atom_tuple))
-                index_atoms.append(
-                    (
-                        f"{atoms['auth_asym_id'][i]}/{atoms['auth_seq_id'][i]}",
-                        atoms["auth_comp_id"][i],
-                        atoms["auth_atom_id"][i],
-                    )
-                )
+    return bm_atoms
 
-                if isotope is not None:
-                    atom.SetIsotope(isotope)
 
-                mol.AddAtom(atom)
+def _parse_pdb_atoms(mol: rdkit.Chem.rdchem.Mol, atoms: dict[str, list[str]]):
+    """Setup atoms of bound-molecules in the Component
 
-    return index_atoms, bm_atoms_dict
+    Args:
+        mol: Rdkit Mol object of bound-molecule
+        atoms: atoms of bound-molecules
+    """
 
+    for i in range(len(atoms["id"])):
+        atom_id = atoms["label_atom_id"][i]
+        chain = atoms["auth_asym_id"][i]
+        res_name = atoms["label_comp_id"][i]
+        res_id = atoms["auth_seq_id"][i]
+        ins_code = (
+            "" if not atoms["pdbx_PDB_ins_code"][i] else atoms["pdbx_PDB_ins_code"][i]
+        )
+        residue_id = f"{chain}{res_id}{ins_code}"
+        element = atoms["type_symbol"][i]
+        element = element if len(element) == 1 else element[0] + element[1].lower()
+        isotope = None
+        if element == "D":
+            element = "H"
+            isotope = 2
+        elif element == "X":
+            element = "*"
+
+        atom_name = f"{element}{i}"
+        atom = rdkit.Chem.Atom(element)
+        atom.SetProp("name", atom_name)
+        atom.SetProp("component_atom_id", atom_id)
+        atom.SetProp("residue_id", residue_id)
+        # _atom_site.auth_seq_id is not necessary to be a number (https://mmcif.wwpdb.org/dictionaries/mmcif_pdbx_v50.dic/Items/_atom_site.auth_seq_id.html)
+
+        res_info = rdkit.Chem.AtomPDBResidueInfo()
+        res_info.SetResidueName(res_name)
+        res_info.SetIsHeteroAtom(True)
+        atom.SetMonomerInfo(res_info)
+
+        if isotope is not None:
+            atom.SetIsotope(isotope)
+
+        mol.AddAtom(atom)
 
-def _parse_pdb_conformers_site(mol, atoms, index_atoms):
-    """
-    Setup model cooordinates in the rdkit Mol object.
+
+def _parse_pdb_conformers(mol: rdkit.Chem.rdchem.Mol, atoms: dict[str, list[str]]):
+    """Setup model cooordinates in the rdkit Mol object.
 
     Args:
-        mol (rdkit.Chem.rdchem.Mol): RDKit Mol object with the compound
-            representation.
-        atoms (dict): mmcif category with atom info category.
-        index_atoms (list): List of intx atoms
+        mol: RDKit Mol object of bound-molecule
+        atoms: atoms of bound-molecule
     """
     if not atoms:
         return
 
-    model = _setup_pdb_conformer_site(
-        atoms, "Cartn_{}", ConformerType.Model.name, index_atoms
-    )
-
+    model = _setup_pdb_conformer(atoms)
     mol.AddConformer(model, assignId=True)
 
 
-def _setup_pdb_conformer_site(atoms, label, name, index_atoms):
-    """
-    Setup a conformer
-
-    Args:
-        atoms (dict): mmcif category with the atom info.
-        label (str): Namespace with the [x,y,z] coordinates.
-        name (str): Conformer name.
-        index_atoms (lsit): List of index atoms
-
-    Returns:
-        rdkit.Chem.rdchem.Conformer: Conformer of the component.
-    """
+def _setup_pdb_conformer(atoms):
     if not atoms:
         return
 
-    conformer = rdkit.Chem.Conformer(len(index_atoms))
-
-    j = 0
+    conformer = rdkit.Chem.Conformer(len(atoms["id"]))
     for i in range(len(atoms["id"])):
-        if atoms["group_PDB"][i] != "HETATM":
-            continue
-        x = conversions.str_to_float(atoms[label.format(("x"))][i])
-        y = conversions.str_to_float(atoms[label.format(("y"))][i])
-        z = conversions.str_to_float(atoms[label.format(("z"))][i])
-        index = helper.find_element_in_list(
-            index_atoms,
-            (
-                f"{atoms['auth_asym_id'][i]}/{atoms['auth_seq_id'][i]}",
-                atoms["auth_comp_id"][i],
-                atoms["auth_atom_id"][i],
-            ),
-        )
-
+        x = conversions.str_to_float(atoms["Cartn_x"][i])
+        y = conversions.str_to_float(atoms["Cartn_y"][i])
+        z = conversions.str_to_float(atoms["Cartn_z"][i])
         atom_position = rdkit.Chem.rdGeometry.Point3D(x, y, z)
-        conformer.SetAtomPosition(index, atom_position)
-        j = j + 1
-
-        conformer.SetProp("name", name)
+        conformer.SetAtomPosition(i, atom_position)
 
+    conformer.SetProp("name", ConformerType.Model.name)
     return conformer
 
 
-def _parse_pdb_bonds_site(mol, bonds, atoms, errors, index_atoms, bm):
-    """
-    Setup bonds in the compound
+def _parse_pdb_bonds(
+    mol: rdkit.Chem.rdchem.Mol,
+    bm: MultiDiGraph,
+    cif_block: cif.Block,
+    errors: list[str],
+):
+    """Setup bonds in the rdkit Mol object
 
     Args:
-        mol (rdkit.Chem.rdchem.Mol): Molecule which receives bonds.
-        bonds (dict): mmcif category with the bonds info. TODO not being used
-        atoms (dict): mmcif category with the atom info. TODO not being used
-        errors (list[str]): Issues encountered while parsing.
-        index_atoms (list): List of index atoms
-        bm (dict): Dictionary representation of bound-molecule
+        mol: RDKit Mol object of bound-molecule
+        bm: bound-molecule
+        errors: list of errors encountered while parsing.
     """
-    if not bonds:
+    if (
+        "_atom_site." not in cif_block.get_mmcif_category_names()
+        or "_chem_comp_bond." not in cif_block.get_mmcif_category_names()
+    ):
         return
 
-    bond_per_type = {}
-    for i in range(len(bonds["atom_id_1"])):
-        content = (
-            bonds["atom_id_1"][i],
-            bonds["atom_id_2"][i],
-            bonds["value_order"][i],
-        )
-        if bonds["comp_id"][i] in bond_per_type:
-            bond_per_type[bonds["comp_id"][i]].append(content)
-        else:
-            bond_per_type[bonds["comp_id"][i]] = [content]
+    for residue in bm.nodes():
+        resiude_bonds = get_chem_comp_bonds(cif_block, residue.name)
+        for i in range(len(resiude_bonds.atom_id_1)):
+            try:
+                atom_1 = resiude_bonds.atom_id_1[i]
+                mol_atom_1_idx = helper.find_atom_index(mol, residue.id, atom_1)
+                atom_2 = resiude_bonds.atom_id_2[i]
+                mol_atom_2_idx = helper.find_atom_index(mol, residue.id, atom_2)
+                bond_order = helper.bond_pdb_order(resiude_bonds.value_order[i])
+                if (mol_atom_1_idx is not None) and (mol_atom_2_idx is not None):
+                    mol.AddBond(mol_atom_1_idx, mol_atom_2_idx, bond_order)
+            except ValueError:
+                errors.append(
+                    f"Error perceiving {atom_1} - {atom_2} bond from _chem_comp_bond"
+                )
+            except RuntimeError:
+                errors.append(f"Duplicit bond {atom_1} - {atom_2}")
+
 
-    # get connection mapping
-    connection_mapping = {}
-    for j in bm["residues"]:
-        connection_mapping[j["id"]] = j
-
-    for j in bm["residues"]:
-        lig = j["label_comp_id"]
-        if lig not in bond_per_type:  # ions
-            continue
-        chain_res = f"{j['auth_asym_id']}/{j['auth_seq_id']}"
+def _add_connections(
+    mol: rdkit.Chem.rdchem.Mol, bm: MultiDiGraph, errors: list[str]
+) -> None:
+    """Add bonds between CCDs in the bound-molecule
+
+    Args:
+        mol: RDKit Mol object of bound-molecule
+        bm: bound-molecule
+        errors: list of errors encountered while parsing
+
+    """
+    for residue_1, residue_2, atoms in bm.edges(data=True):
         try:
-            for pairs in bond_per_type[lig]:
-                tuple_to_find_1 = (chain_res, lig, pairs[0])
-                tuple_to_find_2 = (chain_res, lig, pairs[1])
-                atom_1 = helper.find_element_in_list(index_atoms, tuple_to_find_1)
-                atom_2 = helper.find_element_in_list(index_atoms, tuple_to_find_2)
-                bond_order = ccd_reader._bond_pdb_order(pairs[2])
-                if any(a is None for a in [atom_1, atom_2, bond_order]):
-                    pass
-                else:
-                    mol.AddBond(atom_1, atom_2, bond_order)
+            atom_1 = atoms["atom_id_1"]
+            mol_atom_1_idx = helper.find_atom_index(mol, residue_1.id, atom_1)
+            atom_2 = atoms["atom_id_2"]
+            mol_atom_2_idx = helper.find_atom_index(mol, residue_2.id, atom_2)
+            bond_order = helper.bond_pdb_order("SING")
+            if (mol_atom_1_idx is not None) and (mol_atom_2_idx is not None):
+                mol.AddBond(mol_atom_1_idx, mol_atom_2_idx, bond_order)
         except ValueError:
             errors.append(
-                f"Error perceiving {atom_1} - {atom_2} bond in _chem_comp_bond"
+                f"Error perceiving {atom_1} - {atom_2} bond from Boundmolecule connections"
             )
         except RuntimeError:
             errors.append(f"Duplicit bond {atom_1} - {atom_2}")
 
-    # Add bound molecule connections
-    try:
-        for connection in bm["connections"]:
-            first_res = connection_mapping[connection[0]]
-            second_res = connection_mapping[connection[1]]
-            chain_res_1 = f"{first_res['auth_asym_id']}/{first_res['auth_seq_id']}"
-            chain_res_2 = f"{second_res['auth_asym_id']}/{second_res['auth_seq_id']}"
-            lig_1 = first_res["label_comp_id"]
-            lig_2 = second_res["label_comp_id"]
-            tuple_to_find_1 = (chain_res_1, lig_1, connection[2]["atom_id_1"])
-            tuple_to_find_2 = (chain_res_2, lig_2, connection[2]["atom_id_2"])
-            atom_1 = helper.find_element_in_list(index_atoms, tuple_to_find_1)
-            atom_2 = helper.find_element_in_list(index_atoms, tuple_to_find_2)
-
-            if any(a is None for a in [atom_1, atom_2]):
-                pass
-            else:
-                mol.AddBond(atom_1, atom_2, ccd_reader._bond_pdb_order("SING"))
-    except ValueError:
-        errors.append(f"Error perceiving {atom_1} - {atom_2} bond in _struct_conn")
-    except RuntimeError:
-        errors.append(f"Duplicit bond {atom_1} - {atom_2}")
-
-
-def infer_bound_molecules(structure, to_discard):
-    """Identify bound molecules in the input protein structure.
-
-    Args:
-        structure (str): Path to the structure.
-        to_discard (list of str): List of residue names to be discarded
-    """
-
-    bms = parse_bound_molecules(structure, to_discard)
-    bound_molecules = []
-
-    for bm_nodes in connected_components(bms.to_undirected()):
-        subgraph = bms.subgraph(bm_nodes)
-        bm = BoundMolecule(subgraph)
-        bound_molecules.append(bm)
-
-    bound_molecules = sorted(bound_molecules, key=lambda l: -len(l.graph.nodes))
-    return bound_molecules
-
-
-def __add_connections(struct_conn, bms):
-    for i in range(len(struct_conn["id"])):
-        (ptnr1, atom1) = find_pntr_entry(struct_conn, bms.nodes, 1, i)
-        (ptnr2, atom2) = find_pntr_entry(struct_conn, bms.nodes, 2, i)
-
-        # we want covalent connections among ligands only.
-        if ptnr1 and ptnr2 and struct_conn["conn_type_id"][i] != "metalc":
-            bms.add_edge(ptnr1, ptnr2, atom_id_1=atom1, atom_id_2=atom2)
-
-
-def __add_con_branch_link(entity_branch_link, branch_scheme, bms):
-    entities = {}
-    for i in range(len(branch_scheme["entity_id"])):
-        if branch_scheme["entity_id"][i] not in entities:
-            entities[branch_scheme["entity_id"][i]] = [branch_scheme["pdb_asym_id"][i]]
-        elif (
-            branch_scheme["pdb_asym_id"][i]
-            not in entities[branch_scheme["entity_id"][i]]
-        ):
-            entities[branch_scheme["entity_id"][i]].append(
-                branch_scheme["pdb_asym_id"][i]
-            )
 
-    for i in range(len(entity_branch_link["link_id"])):
-        ent_id = entity_branch_link["entity_id"][i]
-        for chain in entities[ent_id]:
-            for node in bms.nodes:
-                prtnr1 = False
-                prtnr2 = False
-                atom1 = False
-                atom2 = False
-                if (
-                    node.name == entity_branch_link["comp_id_1"][i]
-                    and node.chain == chain
-                    and node.res_id == entity_branch_link["entity_branch_list_num_1"][i]
-                ):
-                    prtnr1 = node
-                    atom1 = node.name
-                elif (
-                    node.name == entity_branch_link["comp_id_2"][i]
-                    and node.chain == chain
-                    and node.res_id == entity_branch_link["entity_branch_list_num_2"][i]
-                ):
-                    prtnr2 = node
-                    atom2 = node.name
-            if prtnr1 and prtnr2:
-                bms.add_edge(prtnr1, prtnr2, atom_id_1=atom1, atom_id_2=atom2)
+def get_chem_comp_bonds(cif_block: cif.Block, residue: str):
+    """Returns _chem_comp_bond associated with a residue
 
+    Args:
+        cif_block: gemmi.cif.Block object of protein mmCIF file
+        residue: CCD ID
+    """
 
-def parse_bound_molecules(path, to_discard):
-    """Parse information from the information about HETATMS from the
-    `_pdbx_nonpoly_scheme` and connectivity among them from `_struct_conn`.
+    if "_chem_comp_bond." not in cif_block.get_mmcif_category_names():
+        return
+    chem_comp_bonds = cif_block.get_mmcif_category("_chem_comp_bond.")
+    ResidueBonds = namedtuple("ResidueBonds", "residue atom_id_1 atom_id_2 value_order")
+    atom_id_1 = []
+    atom_id_2 = []
+    value_order = []
+    last_comp_id = None
+    residue_found = False
+    for i in range(len(chem_comp_bonds["comp_id"])):
+        chem_comp_id = chem_comp_bonds["comp_id"][i]
+        if chem_comp_id == residue:
+            residue_found = True
+            atom_id_1.append(chem_comp_bonds["atom_id_1"][i])
+            atom_id_2.append(chem_comp_bonds["atom_id_2"][i])
+            value_order.append(chem_comp_bonds["value_order"][i])
+        last_comp_id = chem_comp_id
+        if last_comp_id != residue and residue_found:
+            break
+
+    residue_bonds = ResidueBonds(residue, atom_id_1, atom_id_2, value_order)
+    return residue_bonds
+
+
+def _handle_hydrogens(mol):
+    """
+    Returns a rdkit.Chem.rdchem.Mol after adding hydrogens
 
     Args:
-        path (str): Path to the mmCIF structure
-        to_discard (list of str): List of residue names to be discarded.
+        mol: Rdkit Mol object
+    """
+
+    hydrogen_indices = [
+        atom.GetIdx() for atom in mol.GetAtoms() if atom.GetAtomicNum() == 1
+    ]
+
+    hydrogen_indices.sort(reverse=True)
+    for index in hydrogen_indices:
+        mol.RemoveAtom(index)
+
+    mol.UpdatePropertyCache(strict=False)
+    mol = rdkit.Chem.AddHs(mol, addCoords=True, addResidueInfo=True)
+    conformer = mol.GetConformer()
+    for atom in mol.GetAtoms():
+        if atom.GetAtomicNum() == 1:
+            atom_id = atom.GetSymbol() + str(atom.GetIdx())
+            atom.SetProp("name", atom_id)
+            mol_tools.correct_atom_coords(conformer, atom.GetIdx())
+            for bond in atom.GetBonds():
+                other = bond.GetOtherAtom(atom)
+                residue_id = other.GetProp("residue_id")
+                atom.SetProp("residue_id", residue_id)
+    return mol
+
+
+def read_clc_cif_file(
+    path_to_cif: str, sanitize: bool = True
+) -> ccd_reader.CCDReaderResult:
+    """
+    Read in single CLC CIF component and create its internal
+    representation.
+
+    Args:
+        path_to_cif (str): Path to the cif file
+        sanitize (bool): [Defaults: True]
+
+    Raises:
+        ValueError: if file does not exist
 
     Returns:
-        DiGraph: All the bound molecules in a given entry.
+        CCDReaderResult: Results of the parsing altogether with
+        the internal representation of the component.
     """
-    doc = cif.read(path)
+    if not os.path.isfile(path_to_cif):
+        raise ValueError("File '{}' does not exists".format(path_to_cif))
+
+    doc = cif.read(path_to_cif)
     cif_block = doc.sole_block()
 
-    if (
-        "_pdbx_nonpoly_scheme." not in cif_block.get_mmcif_category_names()
-        and "_pdbx_branch_scheme." not in cif_block.get_mmcif_category_names()
-    ):
-        return DiGraph()
+    return _parse_clc_mmcif(cif_block, sanitize)
 
-    if "_pdbx_nonpoly_scheme." in cif_block.get_mmcif_category_names():
-        bms = parse_ligands_from_nonpoly_scheme(
-            cif_block.get_mmcif_category("_pdbx_nonpoly_scheme."), to_discard
-        )
 
-    else:
-        bms = DiGraph()
+def read_clc_components_file(
+    path_to_cif: str, sanitize: bool = True
+) -> dict[str, ccd_reader.CCDReaderResult]:
+    """
+    Process multiple compounds stored in the wwPDB CCD
+    `components.cif` file.
 
-    if "_pdbx_branch_scheme." in cif_block.get_mmcif_category_names():
-        if bms:
-            bms = parse_ligands_from_branch_scheme(
-                cif_block.get_mmcif_category("_pdbx_branch_scheme."), to_discard, bms
-            )
-        else:
-            bms = parse_ligands_from_branch_scheme(
-                cif_block.get_mmcif_category("_pdbx_branch_scheme."),
-                to_discard,
-                DiGraph(),
-            )
+    Args:
+        path_to_cif (str): Path to the `clc-all.cif` file with
+            multiple ligands in it.
+        sanitize (bool): Whether or not the components should be sanitized
+            Defaults to True.
 
-    if "_struct_conn." in cif_block.get_mmcif_category_names():
-        __add_connections(cif_block.get_mmcif_category("_struct_conn."), bms)
+    Raises:
+        ValueError: if the file does not exist.
 
-    if "_pdbx_branch_scheme." in cif_block.get_mmcif_category_names():
-        __add_con_branch_link(
-            cif_block.get_mmcif_category("_pdbx_entity_branch_link."),
-            cif_block.get_mmcif_category("_pdbx_branch_scheme."),
-            bms,
-        )
+    Returns:
+        dict[str, CCDReaderResult]: Internal representation of all
+        the components in the `components.cif` file.
+    """
+    if not os.path.isfile(path_to_cif):
+        raise ValueError("File '{}' does not exists".format(path_to_cif))
 
-    return bms
+    result_bag = {}
 
+    for block in cif.read(path_to_cif):
+        try:
+            result_bag[block.name] = _parse_clc_mmcif(block, sanitize)
+        except CCDUtilsError as e:
+            logging.error(
+                f"ERROR: Data block {block.name} not processed. Reason: ({str(e)})."
+            )
 
-def find_pntr_entry(struct_conn, residue_pool, partner, i):
-    """Helper method to find ligand residue in parsed ligands and check
-    its connections.
+    return result_bag
 
-    Just because it is chatty and used throughout the code quite often.
+
+# region parse mmcif
+
+
+def _parse_clc_mmcif(cif_block, sanitize=True):
+    """
+    Create internal representation of the molecule from mmcif format.
 
     Args:
-        struct_conn (dict of str: str): struct_conn table.
-        residue_pool (List of Residue): List of all the parsed residues.
-        partner (str): Identification of the partner (should be 1 or 2)
-        i (int): Index in the struct_conn table
+        cif_block (cif.Block): mmcif block object from gemmi
+        sanitize (bool): Whether or not the rdkit component should
+            be sanitized. Defaults to True.
+
+    Returns:
+        CCDReaderResult: internal representation with the results
+            of parsing and Mol object.
     """
-    atom_name = struct_conn[f"ptnr{partner}_label_atom_id"][i]
-    for residue in residue_pool:
-        if (
-            residue.name == struct_conn[f"ptnr{partner}_label_comp_id"][i]
-            and residue.chain == struct_conn[f"ptnr{partner}_auth_asym_id"][i]
-            and residue.res_id == struct_conn[f"ptnr{partner}_auth_seq_id"][i]
-        ):
-            return (residue, atom_name)
+    warnings = []
+    errors = []
+    sanitized = False
+    mol = rdkit.Chem.RWMol()
+
+    for c in preprocessable_categories:
+        w = cif_tools.preprocess_cif_category(cif_block, c)
+
+        if w:
+            warnings.append(w)
+
+    _parse_clc_atoms(mol, cif_block)
+    _parse_clc_conformers(mol, cif_block)
+    ccd_reader._parse_pdb_bonds(mol, cif_block, errors)
+    ccd_reader._handle_implicit_hydrogens(mol)
 
-    return (None, atom_name)
+    if sanitize:
+        sanitized = mol_tools.sanitize(mol)
 
+    descriptors = ccd_reader._parse_pdb_descriptors(
+        cif_block, "_pdbx_chem_comp_descriptor.", "descriptor"
+    )
+    descriptors += ccd_reader._parse_pdb_descriptors(
+        cif_block, "_pdbx_chem_comp_identifier.", "identifier"
+    )
+    properties = _parse_clc_properties(cif_block)
 
-def parse_ligands_from_branch_scheme(branch_scheme, to_discard, g):
-    """Parse ligands from the mmcif file.
+    comp = Component(mol.GetMol(), cif_block, properties, descriptors)
+    reader_result = ccd_reader.CCDReaderResult(
+        warnings=warnings, errors=errors, component=comp, sanitized=sanitized
+    )
 
-    Args:
-        nonpoly_scheme (dict of str: list of str): mmcif _nonpoly_scheme
-            category.
-        to_discard (list of str): List of residue names to be discarded.
+    return reader_result
 
-    Returns:
-        DiGraph: Ligands and their connectivity in a PDB entry
+
+def _parse_clc_atoms(mol, cif_block):
     """
+    Setup atoms in the component
 
-    for i in range(len(branch_scheme["asym_id"])):
-        n = Residue(
-            branch_scheme["pdb_mon_id"][i],  # aka label_comp_id
-            branch_scheme["pdb_asym_id"][i],  # aka auth_asym_id
-            branch_scheme["num"][i],  # aka auth_seq_id
-            None,  # aka pdbx_PDB_ins_code
-            branch_scheme["entity_id"][i],
-        )
+    Args:
+        mol (rdkit.Chem.rdchem.Mol): Rdkit Mol object with the
+            compound representation.
+        cif_block (cif.Block): mmCIF block object from gemmi.
+    """
+    if "_chem_comp_atom." not in cif_block.get_mmcif_category_names():
+        return
+
+    atoms = cif_block.find(
+        "_chem_comp_atom.",
+        [
+            "atom_id",
+            "type_symbol",
+            "alt_atom_id",
+            "pdbx_leaving_atom_flag",
+            "charge",
+            "pdbx_component_comp_id",
+            "pdbx_residue_numbering",
+            "pdbx_component_atom_id",
+        ],
+    )
+    for row in atoms:
+        atom_id = cif.as_string(row["_chem_comp_atom.atom_id"])
+        element = cif.as_string(row["_chem_comp_atom.type_symbol"])
+        alt_atom_id = cif.as_string(row["_chem_comp_atom.alt_atom_id"])
+        leaving_atom = cif.as_string(row["_chem_comp_atom.pdbx_leaving_atom_flag"])
+        charge = cif.as_string(row["_chem_comp_atom.charge"])
+        comp_atom_id = cif.as_string(row["_chem_comp_atom.pdbx_component_atom_id"])
+        res_name = cif.as_string(row["_chem_comp_atom.pdbx_component_comp_id"])
+        residue_id = cif.as_string(row["_chem_comp_atom.pdbx_residue_numbering"])
+
+        element = element if len(element) == 1 else element[0] + element[1].lower()
+        isotope = None
+
+        if element == "D":
+            element = "H"
+            isotope = 2
+        elif element == "X":
+            element = "*"
+
+        atom = rdkit.Chem.Atom(element)
+        atom.SetProp("name", atom_id)
+        atom.SetProp("alt_name", alt_atom_id)
+        atom.SetBoolProp("leaving_atom", leaving_atom == "Y")
+        atom.SetProp("component_atom_id", comp_atom_id)
+        atom.SetProp("residue_id", residue_id)
+        atom.SetFormalCharge(conversions.str_to_int(charge))
+
+        res_info = rdkit.Chem.AtomPDBResidueInfo()
+        res_info.SetResidueName(res_name)
+        res_info.SetIsHeteroAtom(True)
+        atom.SetMonomerInfo(res_info)
 
-        if n.name not in to_discard:
-            g.add_node(n)
+        if isotope is not None:
+            atom.SetIsotope(isotope)
 
-    return g
+        mol.AddAtom(atom)
 
 
-def parse_ligands_from_nonpoly_scheme(nonpoly_scheme, to_discard):
-    """Parse ligands from the mmcif file.
+def _parse_clc_conformers(mol, cif_block):
+    """Setup model cooordinates in the rdkit Mol object.
 
     Args:
-        nonpoly_scheme (dict of str: list of str): mmcif _nonpoly_scheme
-            category.
-        to_discard (list of str): List of residue names to be discarded.
+        mol (rdkit.Chem.rdchem.Mol): RDKit Mol object with the compound
+            representation.
+        cif_block (cif.Block): mmCIF block object from gemmi.
+    """
+
+    if "_chem_comp_atom." not in cif_block.get_mmcif_category_names():
+        return
+
+    required_fields = [
+        "model_Cartn_x",
+        "model_Cartn_y",
+        "model_Cartn_z",
+    ]
+    atoms = cif_block.find("_chem_comp_atom.", required_fields)
+    model = ccd_reader._setup_pdb_conformer(
+        atoms, "model_Cartn_{}", ConformerType.Model.name
+    )
+    mol.AddConformer(model, assignId=True)
+
+
+def _parse_clc_properties(cif_block):
+    """Parse useful information from _chem_comp category
+
+    Args:
+        cif_block (cif.Block): mmcif block object from gemmi
 
     Returns:
-        DiGraph: Ligands and their connectivity in a PDB entry
+        Properties: dataclass with the CCD properties.
     """
-    g = DiGraph()
+    properties = None
+    if "_chem_comp." in cif_block.get_mmcif_category_names():
+        mod_date = cif_block.find_value("_chem_comp.pdbx_modified_date")
+        if cif.is_null(mod_date):
+            d = date(1970, 1, 1)
+        else:
+            mod_date = mod_date.split("-")
+            d = date(int(mod_date[0]), int(mod_date[1]), int(mod_date[2]))
 
-    for i in range(len(nonpoly_scheme["asym_id"])):
-        n = Residue(
-            nonpoly_scheme["pdb_mon_id"][i],  # aka label_comp_id
-            nonpoly_scheme["pdb_strand_id"][i],  # aka auth_asym_id
-            nonpoly_scheme["pdb_seq_num"][i],  # aka auth_seq_id
-            nonpoly_scheme["pdb_ins_code"][i],  # aka pdbx_PDB_ins_code
-            nonpoly_scheme["entity_id"][i],
+        rel_status = ReleaseStatus.from_str(
+            cif_block.find_value("_chem_comp.pdbx_release_status")
+        )
+        formula_weight = cif_block.find_value("_chem_comp.formula_weight")
+        weight = 0.0 if cif.is_null(formula_weight) else cif.as_number(formula_weight)
+
+        properties = CCDProperties(
+            id=cif.as_string(cif_block.find_value("_chem_comp.id")),
+            name="",
+            formula=cif.as_string(cif_block.find_value("_chem_comp.formula")),
+            modified_date=d,
+            pdbx_release_status=rel_status,
+            weight=weight,
         )
+    return properties
 
-        if n.name not in to_discard:
-            g.add_node(n)
 
-    return g
+# endregion parse mmcif
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_reader.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/ccd_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from pdbeccdutils.core.exceptions import CCDUtilsError
 from pdbeccdutils.core.models import (
     CCDProperties,
     ConformerType,
     Descriptor,
     ReleaseStatus,
 )
-from pdbeccdutils.helpers import cif_tools, conversions, mol_tools
+from pdbeccdutils.helpers import cif_tools, conversions, mol_tools, helper
 from gemmi import cif
 
 # categories that need to be 'fixed'
 # str => list[str]
 preprocessable_categories = [
     "_chem_comp_atom.",
     "_chem_comp_bond.",
@@ -188,31 +188,31 @@
 
 
 def _parse_pdb_atoms(mol, cif_block):
     """
     Setup atoms in the component
 
     Args:
-        mol (rdkit.Chem.rchem.Mol): Rdkit Mol object with the
+        mol (rdkit.Chem.rdchem.Mol): Rdkit Mol object with the
             compound representation.
         cif_block (cif.Block): mmCIF block object from gemmi.
     """
     if "_chem_comp_atom." not in cif_block.get_mmcif_category_names():
         return
 
     atoms = cif_block.find(
         "_chem_comp_atom.",
         ["atom_id", "type_symbol", "alt_atom_id", "pdbx_leaving_atom_flag", "charge"],
     )
     for row in atoms:
-        atom_id = row["_chem_comp_atom.atom_id"].strip('"')
-        element = row["_chem_comp_atom.type_symbol"].strip('"')
-        alt_atom_id = row["_chem_comp_atom.alt_atom_id"].strip('"')
-        leaving_atom = row["_chem_comp_atom.pdbx_leaving_atom_flag"].strip('"')
-        charge = row["_chem_comp_atom.charge"].strip('"')
+        atom_id = cif.as_string(row["_chem_comp_atom.atom_id"])
+        element = cif.as_string(row["_chem_comp_atom.type_symbol"])
+        alt_atom_id = cif.as_string(row["_chem_comp_atom.alt_atom_id"])
+        leaving_atom = cif.as_string(row["_chem_comp_atom.pdbx_leaving_atom_flag"])
+        charge = cif.as_string(row["_chem_comp_atom.charge"])
 
         element = element if len(element) == 1 else element[0] + element[1].lower()
         isotope = None
 
         if element == "D":
             element = "H"
             isotope = 2
@@ -317,15 +317,15 @@
     atoms_ids = list(atoms.find_column("_chem_comp_atom.atom_id"))
     for row in bonds:
         try:
             atom_1 = row["_chem_comp_bond.atom_id_1"]
             atom_1_id = atoms_ids.index(atom_1)
             atom_2 = row["_chem_comp_bond.atom_id_2"]
             atom_2_id = atoms_ids.index(atom_2)
-            bond_order = _bond_pdb_order(row["_chem_comp_bond.value_order"])
+            bond_order = helper.bond_pdb_order(row["_chem_comp_bond.value_order"])
 
             mol.AddBond(atom_1_id, atom_2_id, bond_order)
         except ValueError:
             errors.append(
                 f"Error perceiving {atom_1} - {atom_2} bond in _chem_comp_bond"
             )
         except RuntimeError:
@@ -367,20 +367,23 @@
         Descriptor: namedtuple with the property info
     """
     descriptors = []
 
     if cat_name not in cif_block.get_mmcif_category_names():
         return descriptors
 
-    descriptors_block = cif_block.find(cat_name, [label, "type", "program"])
+    descriptors_block = cif_block.find(
+        cat_name, [label, "type", "program", "program_version"]
+    )
     for row in descriptors_block:
         d = Descriptor(
-            type=row[f"{cat_name}type"],
-            program=row[f"{cat_name}program"],
-            value=row[f"{cat_name}{label}"],
+            type=cif.as_string(row[f"{cat_name}type"]),
+            program=cif.as_string(row[f"{cat_name}program"]),
+            program_version=cif.as_string(row[f"{cat_name}program_version"]),
+            value=cif.as_string(row[f"{cat_name}{label}"]),
         )
         descriptors.append(d)
 
     return descriptors
 
 
 def _parse_pdb_properties(cif_block):
@@ -404,38 +407,18 @@
         rel_status = ReleaseStatus.from_str(
             cif_block.find_value("_chem_comp.pdbx_release_status")
         )
         formula_weight = cif_block.find_value("_chem_comp.formula_weight")
         weight = 0.0 if cif.is_null(formula_weight) else cif.as_number(formula_weight)
 
         properties = CCDProperties(
-            id=cif_block.find_value("_chem_comp.id"),
-            name=cif_block.find_value("_chem_comp.name").strip('"'),
-            formula=cif_block.find_value("_chem_comp.formula").strip('"'),
+            id=cif.as_string(cif_block.find_value("_chem_comp.id")),
+            name=cif.as_string(cif_block.find_value("_chem_comp.name")),
+            formula=cif.as_string(cif_block.find_value("_chem_comp.formula")),
             modified_date=d,
             pdbx_release_status=rel_status,
             weight=weight,
         )
     return properties
 
 
-def _bond_pdb_order(value_order):
-    """
-    Transpils mmcif bond order into rdkit language
-
-    Args:
-        value_order (str): bond type as a str
-
-    Returns:
-        rdkit.Chem.rdchem.BondType: -- bond type
-    """
-    if value_order == "SING":
-        return rdkit.Chem.rdchem.BondType(1)
-    if value_order == "DOUB":
-        return rdkit.Chem.rdchem.BondType(2)
-    if value_order == "TRIP":
-        return rdkit.Chem.rdchem.BondType(3)
-
-    return None
-
-
 # endregion parse mmcif
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/ccd_writer.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/ccd_writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,46 +301,47 @@
 
     xml = ET.tostring(root, encoding="utf-8", method="xml")
     xmls_tring = minidom.parseString(xml)
 
     return xmls_tring.toprettyxml(indent="  ")
 
 
+def remove_hydrogens(cif_block_copy):
+    cif_tools.preprocess_cif_category(cif_block_copy, "_chem_comp_atom.")
+    cif_tools.preprocess_cif_category(cif_block_copy, "_chem_comp_bond.")
+
+    # scrap hydrogen atoms
+    h_names: List[str] = []
+    atom_table = cif_block_copy.find("_chem_comp_atom.", ["type_symbol", "atom_id"])
+    for i in range(len(atom_table) - 1, -1, -1):
+        if atom_table[i][0] == "H":
+            h_names.append(atom_table[i][1])
+            del atom_table[i]
+
+    # scrap bonds to hydrogen atoms
+    if "_chem_comp_bond." not in cif_block_copy.get_mmcif_category_names():
+        return
+
+    bond_table = cif_block_copy.find("_chem_comp_bond.", ["atom_id_1", "atom_id_2"])
+    for j in range(len(bond_table) - 1, -1, -1):
+        if (bond_table[j][0] in h_names) or (bond_table[j][1] in h_names):
+            del bond_table[j]
+
+
 def to_pdb_ccd_cif_file(path, component: Component, remove_hs=True):
     """Converts structure to the PDB CIF format. Both model and ideal
     coordinates are stored. In case ideal coordinates are missing, rdkit
     attempts to generate 3D coordinates of the conformer.
 
     Args:
         path (str): Path to save cif file.
         component (Component): Component to be exported.
         remove_hs (bool, optional): Defaults to True.
     """
 
-    def remove_hydrogens(cif_block_copy):
-        cif_tools.preprocess_cif_category(cif_block_copy, "_chem_comp_atom.")
-        cif_tools.preprocess_cif_category(cif_block_copy, "_chem_comp_bond.")
-
-        # scrap hydrogen atoms
-        h_names: List[str] = []
-        atom_table = cif_block_copy.find("_chem_comp_atom.", ["type_symbol", "atom_id"])
-        for i in range(len(atom_table) - 1, -1, -1):
-            if atom_table[i][0] == "H":
-                h_names.append(atom_table[i][1])
-                del atom_table[i]
-
-        # scrap bonds to hydrogen atoms
-        if "_chem_comp_bond." not in cif_block_copy.get_mmcif_category_names():
-            return
-
-        bond_table = cif_block_copy.find("_chem_comp_bond.", ["atom_id_1", "atom_id_2"])
-        for j in range(len(bond_table) - 1, -1, -1):
-            if (bond_table[j][0] in h_names) or (bond_table[j][1] in h_names):
-                del bond_table[j]
-
     if not isinstance(component.ccd_cif_block, gemmi.cif.Block):
         component.ccd_cif_block = _to_pdb_ccd_cif_block(component)
 
     temp_doc = cif.Document()
     cif_block_copy = temp_doc.add_copied_block(component.ccd_cif_block)
 
     _add_sw_info_cif(cif_block_copy)
@@ -595,25 +596,22 @@
 
     label = "_chem_comp."
     cif_block.set_pairs(
         label,
         {
             "id": component.id,
             "type": "NON-POLYMER",
-            "pdbx_type": "HETAIN",
-            "formula": cif.quote(component.formula)
-            if component.formula
-            else cif.quote(calc_formula),
+            "formula": component.formula or calc_formula,
             "formula_weight": f"{calc_weight:.3f}",
             "three_letter_code": component.id,
             "pdbx_type": "HETAIN",
             "pdbx_modified_date": mod_date,
             "pdbx_release_status": component.pdbx_release_status.name,
         },
-        raw=True,
+        raw=False,
     )
 
 
 def _write_pdb_ccd_cif_atoms(cif_block, component):
     """Writes the _chem_comp_atom namespace with atom details.
     Controlled dictionary:
     http://mmcif.wwpdb.org/dictionaries/mmcif_pdbx_v50.dic/Categories/chem_comp_atom.html
@@ -663,15 +661,15 @@
 
         new_row = [
             component.id,
             _get_atom_name(atom),
             _get_alt_atom_name(atom),
             atom.GetSymbol(),
             str(atom.GetFormalCharge()),
-            "?",
+            None,
             "Y" if atom.GetIsAromatic() else "N",
             "N",
             _get_ccd_cif_chiral_type(atom),
             f"{model_atom.x:.3f}",
             f"{model_atom.y:.3f}",
             f"{model_atom.z:.3f}",
             f"{ideal_atom.x:.3f}",
@@ -734,19 +732,25 @@
     """
 
     if not component.descriptors:
         return
 
     label = "_pdbx_chem_comp_descriptor."
 
-    descriptor_fields = ["comp_id", "type", "program", "descriptor"]
+    descriptor_fields = ["comp_id", "type", "program", "program_version", "descriptor"]
     descriptor_loop = cif_block.init_loop(label, descriptor_fields)
 
     for entry in component.descriptors:
-        new_row = [component.id, entry.type, entry.program, entry.value]
+        new_row = [
+            component.id,
+            entry.type,
+            entry.program,
+            entry.program_version,
+            entry.value,
+        ]
         descriptor_loop.add_row(cif.quote_list(new_row))
 
 
 def _get_atom_name(atom):
     """Gets atom name. If not set ElementSymbol + Id is used.
 
     Args:
@@ -1190,31 +1194,31 @@
         inchikey = rdkit.Chem.MolToInchiKey(mol)
         new_row = [
             component.id,
             scaffold.name,
             f"S{i+1}",
             "scaffold",
             scaffold.smiles,
-            inchi if inchi else None,
-            inchikey if inchikey else None,
+            inchi or None,
+            inchikey or None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     for j, fragment in enumerate(component.fragments):
         mol = rdkit.Chem.MolFromSmiles(fragment.smiles)
         inchi = rdkit.Chem.MolToInchi(mol)
         inchikey = rdkit.Chem.MolToInchiKey(mol)
         new_row = [
             component.id,
             fragment.name,
             f"F{j+1}",
             "fragment",
             fragment.smiles,
-            inchi if inchi else None,
-            inchikey if inchikey else None,
+            inchi or None,
+            inchikey or None,
         ]
         substructure_loop.add_row(cif.quote_list(new_row))
 
     mapping_category = "_pdbe_chem_comp_substructure_mapping."
     mapping_fields = ["comp_id", "atom_id", "substructure_id", "substructure_ordinal"]
     mapping_loop = cif_block_copy.init_loop(mapping_category, mapping_fields)
 
@@ -1353,15 +1357,15 @@
         from gemmi.
     remove_hs (boolean): Whether or not hydrogen atoms should be written
     """
 
     try:
         conformer = component.get_conformer(ConformerType.Computed)
     except ValueError:
-        logging.warning(f"Computed conformer for {component.id} does not exist.")
+        logging.warning(f"{component.id} | Computed conformer does not exist.")
         return  # no conformer nothing to write, we quit
 
     category = "_pdbe_chem_comp_rdkit_conformer."
     rdkit_conformer_fields = [
         "comp_id",
         "atom_id",
         "Cartn_x_rdkit",
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/component.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/component.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 from pdbeccdutils.core.models import (
     CCDProperties,
     ConformerType,
     Descriptor,
     ReleaseStatus,
     ScaffoldingMethod,
     SubstructureMapping,
+    Subcomponent,
 )
 from pdbeccdutils.helpers import conversions, drawing
 from pdbeccdutils.utils import web_services
 
 
 class Component:
     """
@@ -89,14 +90,24 @@
         If not defined then the empty string '' will be returned.
 
         Returns:
             str: the _chem_comp.id or ''.
         """
         return self._cif_properties.id
 
+    @id.setter
+    def id(self, value):
+        """Set mapping for this component obtained with a different mean
+        but internal use of UniChem.
+
+        Args:
+            list[tuple[str]]: UniChem mappings
+        """
+        self._cif_properties.id = value
+
     @property
     def name(self) -> str:
         """Supply the 'full name' of the PDB-CCD, for example 'ETHANOL'.
         Obtained from PDB-CCD's _chem_comp.name:
 
         http://mmcif.wwpdb.org/dictionaries/mmcif_std.dic/Items/_chem_comp.name.html
 
@@ -133,28 +144,30 @@
             pdbeccdutils.core.enums.ReleaseStatus: enum of the release
             status (this includes NOT_SET if no value is defined).
         """
         return self._cif_properties.pdbx_release_status
 
     @property
     def modified_date(self) -> date:
-        """Supply the _pdbx_chem_comp_descriptor category for the PDB-CCD
-        Obtained from PDB-CCD's _pdbx_chem_comp_descriptor:
+        """Supply the pdbx_modified_date for the PDB-CCD
+        Obtained from PDB-CCD's _chem_comp.pdbx_modified_date:
+
 
         http://mmcif.wwpdb.org/dictionaries/mmcif_pdbx_v50.dic/Items/_chem_comp.pdbx_modified_date.html
 
         Returns:
             datetime.date: Date of the last entrie's modification.
         """
         return self._cif_properties.modified_date
 
     @property
     def descriptors(self) -> List[Descriptor]:
-        """Supply the pdbx_modified_date for the PDB-CCD
-        Obtained from PDB-CCD's _chem_comp.pdbx_modified_date:
+        """Supply the _pdbx_chem_comp_descriptor category for the PDB-CCD
+        Obtained from PDB-CCD's _pdbx_chem_comp_descriptor:
+
 
         http://mmcif.rcsb.org/dictionaries/mmcif_pdbx.dic/Items/_pdbx_chem_comp_descriptor.program_version.html
 
         Returns:
             list[Descriptor]: List of descriptors for a given entry.
         """
         return self._descriptors
@@ -550,59 +563,59 @@
             conformer.SetProp("name", ConformerType.Computed.name)
             conformer.SetProp("coord_generation", f"ETKDG{version}")
 
             return True
 
         return False
 
-    def has_degenerated_conformer(self, c_type: ConformerType) -> bool:
-        """
-        Determine if given conformer has missing coordinates or is
-        missing completelly from the rdkit.Mol object. This can
-        be used to determine, whether or not the coordinates should be
-        regenerated.
-
-        Args:
-            type (ConformerType): type of conformer
-                to be inspected.
-
-        Returns:
-            bool: True if more then 1 atom has coordinates [0, 0, 0]
-        """
-        ok_conformer = False
-
-        for c in self.mol.GetConformers():
-            if c.GetProp("name") == c_type.name:
-                ok_conformer = mol_tools.is_degenerate_conformer(c)
-                break
-
-        return ok_conformer
-
     def get_conformer(self, c_type) -> rdkit.Chem.rdchem.Conformer:
-        """
-        Retrieve an rdkit object for a deemed conformer.
+        """Retrieve an rdkit object for a deemed conformer.
 
         Args:
             c_type (ConformerType): Conformer type to be retrieved.
 
         Raises:
             ValueError: If conformer does not exist
 
         Returns:
             rdkit.Chem.rdchem.Conformer: RDKit conformer object
         """
+
         for c in self.mol.GetConformers():
             try:
                 if c.GetProp("name") == c_type.name:
                     return c
             except KeyError:
                 pass
 
         raise ValueError(f"Conformer {c_type.name} does not exist.")
 
+    def has_degenerated_conformer(self, c_type: ConformerType) -> bool:
+        """Determine if given conformer has missing coordinates or is
+        missing completelly from the rdkit.Mol object. This can
+        be used to determine, whether or not the coordinates should be
+        regenerated.
+
+        Args:
+            type (ConformerType): type of conformer
+                to be inspected.
+
+        Returns:
+            bool: True if more than 1 atom has coordinates [0, 0, 0] or the Conformer is not present
+        """
+        degenerate_conformer = True
+
+        try:
+            conformer = self.get_conformer(c_type)
+            degenerate_conformer = mol_tools.is_degenerate_conformer(conformer)
+        except ValueError:
+            pass
+
+        return degenerate_conformer
+
     def locate_fragment(
         self, mol: rdkit.Chem.rdchem.Mol
     ) -> List[List[rdkit.Chem.rdchem.Atom]]:
         """
         Identify substructure match in the component.
 
         Args:
@@ -732,14 +745,31 @@
             return scaffolds
 
         except (RuntimeError, ValueError):
             raise CCDUtilsError(
                 f"Computing scaffolds using method {scaffolding_method.name} failed."
             )
 
+    def get_subcomponents(self):
+        subcomponents = []
+        res_ids_seen = []
+        for atom in self.mol.GetAtoms():
+            if not atom.HasProp("residue_id"):
+                continue
+            else:
+                res_id = atom.GetProp("residue_id")
+                if res_id not in res_ids_seen:
+                    res_info = atom.GetPDBResidueInfo()
+                    res_name = res_info.GetResidueName()
+                    subcomponent = Subcomponent(res_name, res_id)
+                    subcomponents.append(subcomponent)
+                    res_ids_seen.append(res_id)
+
+        return subcomponents
+
     def _id_to_name_mapping(self, struct_mapping):
         """Lists matched scaffolds and atom names
 
         Args:
             struct_mapping (dict[str, SubstructureMapping]): Basic mapping
                 for fragments/scaffolds.
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/depictions.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/depictions.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         """
         self.coordgen_params = rdCoordGen.CoordGenParams()
         self.coordgen_params.coordgenScaling = 50 / 1.5
         self.coordgen_params.templateFileDir = config.coordgen_templates
 
         self.pubchem_templates = (
-            pubchem_templates_path if os.path.isdir(pubchem_templates_path) else ""
+            pubchem_templates_path if os.path.isdir(str(pubchem_templates_path)) else ""
         )
         self.templates: Dict[str, rdkit.Chem.rdchem.Mol] = OrderedDict()
 
         if os.path.isdir(general_templates_path):
             for k in sorted(os.listdir(general_templates_path)):
                 template = self._load_template(os.path.join(general_templates_path, k))
                 template_name = k.split(".")[0]
@@ -123,15 +123,18 @@
         if results:
             to_return = results[0]
             fix_conformer(to_return.mol.GetConformer(0))
 
             return to_return
 
         return DepictionResult(
-            source=DepictionSource.Failed, template_name="", mol=None, score=1000
+            source=DepictionSource.Failed,
+            template_name="",
+            mol=None,
+            score=float("inf"),
         )
 
     def _get_pubchem_template_path(self, het_id):
         """Get path to the PubChem template if it exists.
 
         Args:
             het_id (str): Ligand in.
@@ -189,15 +192,18 @@
             rdCoordGen.AddCoords(mol, self.coordgen_params)
             flaws = DepictionValidator(mol).depiction_score()
             return DepictionResult(
                 source=DepictionSource.RDKit, template_name=None, mol=mol, score=flaws
             )
         except Exception:
             return DepictionResult(
-                source=DepictionSource.Failed, template_name=None, mol=None, score=1000
+                source=DepictionSource.Failed,
+                template_name=None,
+                mol=None,
+                score=float("inf"),
             )
 
     def _get_2D_by_pubchem(self, code, mol):
         """
         Depict ligand using Pubchem templates.
 
         Args:
@@ -221,23 +227,26 @@
                         mol=mol,
                         score=flaws,
                     )
         except Exception as e:
             print(str(e), file=sys.stderr)
 
         return DepictionResult(
-            source=DepictionSource.Failed, template_name=None, mol=None, score=1000
+            source=DepictionSource.Failed,
+            template_name=None,
+            mol=None,
+            score=float("inf"),
         )
 
     def _get_2D_by_template(self, mol):
         """
         Depict ligand using user-provided templates
 
         Args:
-            mol (rdkit.Chem.rchem.Mol): Mol to be depicted
+            mol (rdkit.Chem.rdchem.Mol): Mol to be depicted
 
         Returns:
             :obj:`list` of :obj:`DepictionResult`: Depictions with their
             quality and metadata.
         """
         results = list()
         try:
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/fragment_library.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/core/models.py` & `pdbeccdutils-0.8.0/pdbeccdutils/core/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,15 +19,31 @@
 pdbeccdutils application.
 """
 
 from dataclasses import dataclass
 from datetime import date
 from enum import IntEnum
 from typing import Any, List, NamedTuple, Dict
-import rdkit
+from rdkit import Chem
+
+
+class LogType(IntEnum):
+    """Type of logged output
+
+    Attributes:
+        ERROR: RDKit generated error
+        WARNING: RDKit generated warning
+        DEPICTION_FAILED: If 2D depiction failed
+        DEPICTION_SCORE: 2D depiction score from DepictionValidator
+    """
+
+    ERROR = 1
+    WARNING = 2
+    DEPICTION_FAILED = 3
+    DEPICTION_SCORE = 4
 
 
 class DepictionSource(IntEnum):
     """Where does the depiction come from.
 
     Attributes:
         Pubchem - Pubchem layout used
@@ -125,34 +141,68 @@
         mol (rdkit.Chem.rdchem.Mol): RDKit mol object.
         score (float): Quality of the depiction, lower is better.
 
     """
 
     source: DepictionSource
     template_name: str
-    mol: rdkit.Chem.rdchem.Mol
+    mol: Chem.rdchem.Mol
     score: float
 
 
 class Descriptor(NamedTuple):
     """
     Descriptor obtained from the cif file. This is essentially
     _pdbx_chem_comp_descriptor field.
 
     Args:
         type (str): `_pdbx_chem_comp_descriptor.type` in CIF language.
         program (str): `_pdbx_chem_comp_descriptor.program` in CIF language.
+        program_version (str): `_pdbx_chem_comp_descriptor.program_version` in CIF language.
         value (str): `_pdbx_chem_comp_descriptor.descriptor` in CIF language.
     """
 
     type: str
     program: str
+    program_version: str
     value: str
 
 
+class InChIFromRDKit(NamedTuple):
+    """
+    InChI calculated by RDKit from rdkit.Chem.rdchem.Mol
+
+    Args:
+        inchi: InChI calculated by RDKit
+        warnings: WARNINGS generated by rdkit.Chem.inchi.MolToInchi API
+        errors: ERRORS generated by rdkit.Chem.inchi.MolToInchi API
+
+    """
+
+    inchi: str
+    warnings: str
+    errors: str
+
+
+class MolFromRDKit(NamedTuple):
+    """
+    rdkit.Chem.rdchem.Mol object generated from RDKit
+
+    Args:
+        mol: mol object geenrated by RDKit
+        warnings: WARNINGS generated by rdkit's API
+        errors: ERRORS generated by rdkit's API
+
+    """
+
+    mol: str
+    warnings: str
+    errors: str
+
+
 @dataclass
 class ParityResult:
     """
     NamedTuple for the result of parity method along with the details
     necessary for calculating the similarity score.
 
     Attributes:
@@ -194,15 +244,15 @@
         name (str): Name or id of the fragment.
         source (str): where does this fragment come from.
         mol (rdkit.Chem.rdchem.Mol): rdkit mol object with the fragment.
     """
 
     name: str
     source: str
-    mol: rdkit.Chem.rdchem.Mol
+    mol: Chem.rdchem.Mol
 
 
 @dataclass
 class SubstructureMapping:
     """Represents a fragment hit in the component
 
     Args:
@@ -214,31 +264,88 @@
 
     name: str
     smiles: str
     source: str
     mappings: List[List[Any]]
 
 
+class Subcomponent:
+    """Represents a subcompoent in a component
+
+    Args:
+        name: Name of the subcomponent
+        id: Id of the subcomponent
+    """
+
+    def __init__(self, name, id):
+        self.name = name
+        self.id = id
+
+    def __eq__(self, other) -> bool:
+        """Checks the equality of two Subcomponent objects
+
+        Returns:
+            True if id of the BoundMolecules are same else False
+        """
+        if (self.name == other.name) and (self.id == other.id):
+            return False
+
+        return True
+
+
 class BoundMolecule:
     def __init__(self, graph):
         self.graph = graph
+        self.id = "-".join(x.id for x in graph.nodes)
+        self.orig_id = "-".join(
+            x.orig_id if isinstance(x, AssemblyResidue) else x.id for x in graph.nodes
+        )
+        self.name = "_".join(x.name for x in graph.nodes)
+
+    def __eq__(self, other) -> bool:
+        """Checks the equality of two BoundMolecule objects
+
+        Returns:
+            True if id of the BoundMolecules are same else False
+        """
+        if self.id != other.id:
+            return False
+
+        return True
+
+    def is_equivalent(self, other) -> bool:
+        """Checks the equivalence of two BoundMolecule objects
+
+        Return:
+            True if orig_id or id of two BoundMolecules are same else False
+        """
+        if self.orig_id != other.orig_id:
+            return False
+
+        return True
 
     def to_dict(self):
         """Return dictionary style representation of the bound molecule.
 
         Returns:
             dict of `str`: dict representation of the object
         """
 
         nodes = sorted(self.graph, key=lambda l: (int(l.res_id), l.chain))
 
-        results_bag = {"residues": [], "connections": []}
+        results_bag = {}
         results_bag["residues"] = [x.to_dict() for x in nodes]
         results_bag["connections"] = [
-            [e.id, f.id, a] for e, f, a in self.graph.edges(data=True)
+            {
+                "residue_id_1": residue_1.id,
+                "residue_id_2": residue_2.id,
+                "atom_id_1": atoms["atom_id_1"],
+                "atom_id_2": atoms["atom_id_2"],
+            }
+            for residue_1, residue_2, atoms in self.graph.edges(data=True)
         ]
 
         return results_bag
 
     def to_list(self):
         results_bag = [
             (e.to_dict(), f.to_dict(), a) for e, f, a in self.graph.edges(data=True)
@@ -254,31 +361,55 @@
         return [x.to_arpeggio() for x in self.graph.nodes]
 
     def __str__(self):
         return "-".join(self.to_arpeggio())
 
 
 class Residue:
-    """Represents a single residue."""
+    """Represents a single residue.
 
-    def __init__(self, name, chain, res_id, ins_code, ent_id):
+    Attributes:
+    name: Corresponds to `_atom_site.label_comp_id`
+    chain: Corresponds to `_atom_site.auth_asym_id`
+    res_id: Corresponds to `_atom_site.auth_seq_id`
+    ins_code: Corresponds to `_atom_site.pdbx_PDB_ins_code`
+    ent_id: Entity id
+    id: ID of the Residue
+    """
+
+    def __init__(self, name: str, chain: str, res_id: str, ins_code: str, ent_id: str):
+        """Initializes Residue
+
+        Args:
+            name: Corresponds to `_atom_site.label_comp_id`
+            chain: Corresponds to `_atom_site.auth_asym_id`
+            res_id: Corresponds to `_atom_site.auth_seq_id`
+            ins_code: Corresponds to `_atom_site.pdbx_PDB_ins_code`
+            ent_id: Entity id
+            id: ID of the Residue
+        """
         self.name = name
         self.chain = chain
         self.res_id = res_id
         self.ins_code = "" if not ins_code else ins_code
         self.ent_id = ent_id
         self.id = f"{chain}{res_id}{self.ins_code}"
 
-    def __eq__(self, other):
+    def __eq__(self, other) -> bool:
+        """Checks the equality of two Residue objects
+
+        Returns:
+            True if id of the Residues are same else False
+        """
         if self.id != other.id:
             return False
 
         return True
 
-    def to_dict(self):
+    def to_dict(self) -> dict[str, str]:
         """Returns a dictionary representation of a given residue.
 
         Returns:
             (:obj:`dict` of :obj:`str`): Dictionary representation along
             with the mmCIF keys.
         """
         return {
@@ -300,7 +431,41 @@
         """Gets Arpeggio style representation of a residue e.g. `/A/129/`
         or /A/129A/ in case there is an insertion code.
 
         Returns:
             str: Residue description in Arpeggio style.
         """
         return f"/{self.chain}/{self.res_id}{self.ins_code}/"
+
+
+class AssemblyResidue(Residue):
+    def __init__(
+        self,
+        name: str,
+        chain: str,
+        res_id: str,
+        ins_code: str,
+        ent_id: str,
+        orig_chain: str,
+        operator: str,
+    ):
+        super().__init__(name, chain, res_id, ins_code, ent_id)
+        self.orig_chain = orig_chain
+        self.operator = operator
+        self.orig_id = f"{orig_chain}{self.res_id}{self.ins_code}"
+
+    def to_dict(self) -> dict[str, str]:
+        """Returns a dictionary representation of a given Residue.
+
+        Returns:
+            Dictionary representation with the mmCIF keys.
+        """
+        return {
+            "id": self.id,
+            "label_comp_id": self.name,
+            "auth_asym_id": self.chain,
+            "auth_seq_id": self.res_id,
+            "pdbx_PDB_ins_code": " " if not self.ins_code else self.ins_code,
+            "entity_id": self.ent_id,
+            "orig_auth_asym_id": self.orig_chain,
+            "operator": self.operator,
+        }
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/coordgen_templates/templates.mae` & `pdbeccdutils-0.8.0/pdbeccdutils/data/coordgen_templates/templates.mae`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/fragment_library.tsv` & `pdbeccdutils-0.8.0/pdbeccdutils/data/fragment_library.tsv`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/adamantane.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/adamantane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/cube.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/cube.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/decahydrocorrin.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/decahydrocorrin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/hem.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/hem.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/nonbornane.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/nonbornane.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/phorbine.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/phorbine.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphin.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/porphin.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/porphycene.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/porphycene.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/ru_complex.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/data/general_templates/ru_complex2.sdf` & `pdbeccdutils-0.8.0/pdbeccdutils/data/general_templates/ru_complex2.sdf`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/helpers/conversions.py` & `pdbeccdutils-0.8.0/pdbeccdutils/helpers/conversions.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/helpers/drawing.py` & `pdbeccdutils-0.8.0/pdbeccdutils/helpers/drawing.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/scripts/process_components_cif_cli.py` & `pdbeccdutils-0.8.0/pdbeccdutils/scripts/process_components_cif_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,20 +27,19 @@
 More detailed description can be found here:
 
 https://gitlab.ebi.ac.uk/pdbe/release/pdbechem
 """
 import argparse
 import logging
 import os
-import traceback
 from pathlib import Path
 
 import pdbeccdutils
 import rdkit
-from pdbeccdutils.core import ccd_reader, ccd_writer
+from pdbeccdutils.core import ccd_reader, ccd_writer, prd_reader, prd_writer
 from pdbeccdutils.core.component import Component
 from pdbeccdutils.core.depictions import DepictionManager
 from pdbeccdutils.core.exceptions import CCDUtilsError
 from pdbeccdutils.core.fragment_library import FragmentLibrary
 from pdbeccdutils.core.models import ConformerType, DepictionSource
 from pdbeccdutils.utils import config
 from pdbeccdutils.utils.pubchem_downloader import PubChemDownloader
@@ -61,14 +60,15 @@
     """
 
     def __init__(
         self,
         pubchem_templates="",
         general_templates=config.general_templates,
         library_path=config.fragment_library,
+        procedure="ccd",
     ):
         """Initialize manager
 
         Args:
             pubchem_templates (str): Path to the pubchem templates
             general_templates (str, optional): Path to the general templates.
                 Defaults to config.general_templates.
@@ -82,70 +82,65 @@
 
         # helper class to get nice depictions
         self.depictions = DepictionManager(pubchem_templates, general_templates)
 
         # Fragments library to get substructure matches
         self.fragment_library = FragmentLibrary(library_path)
 
+        self.procedure = procedure
+
     def run(self, components_path, out_dir):
         """Process components
 
         Args:
             components_path (Path): Path to the components.cif file.
             out_dir (Path): Path to the out_dir
         """
-        logging.info("Reading in components...")
-        data = ccd_reader.read_pdb_components_file(components_path)
-
-        for key, ccd_reader_result in data.items():
-            ccd_out = out_dir / key[0] / key
-            os.makedirs(ccd_out, exist_ok=True)
-            self.process_single_component(ccd_reader_result, ccd_out)
-
-            data[key] = None
+        logging.info("Reading in component")
+        if self.procedure == "ccd":
+            ccd_reader_result = ccd_reader.read_pdb_cif_file(components_path)
+        else:
+            ccd_reader_result = prd_reader.read_pdb_cif_file(components_path)
 
-        logging.debug("All is done!")
+        component = ccd_reader_result.component
+        component_output_dir = Path(out_dir, component.id)
+        os.makedirs(component_output_dir, exist_ok=True)
+        self.process_single_component(ccd_reader_result, component_output_dir)
+        logging.info(f"Processing of {component.id} is complete")
 
     def process_single_component(self, ccd_reader_result, out_dir):
         """Process single PDB-CCD component.
 
         Args:
             ccd_reader_result (CCDReaderResult): pdbeccdutils parser output.
             out_dir (Path): Out directory
 
         Return:
             bool: Whether or not all the files were succesfully written.
         """
-        try:
-            component = ccd_reader_result.component
-            logging.info(f"{component.id} | processing...")
+        component = ccd_reader_result.component
+        logging.info(f"{component.id} | processing...")
 
-            # check parsing and conformer degeneration
-            self._check_component_parsing(ccd_reader_result)
-            self._generate_ideal_structure(component)
-
-            # download templates if the user wants them.
-            if self.pubchem is not None:
-                self._download_template(component)
-
-            # search fragment library
-            self._search_fragment_library(component)
-
-            # get scaffolds
-            self._compute_component_scaffolds(component)
-
-            # write out files
-            self._generate_depictions(component, out_dir)
-            self._export_structure_formats(component, out_dir)
-            return True
-        except Exception:
-            logging.error(
-                f"{ccd_reader_result.component.id} | FAILURE {traceback.format_exc()}."
-            )
-            return False
+        # check parsing and conformer degeneration
+        self._check_component_parsing(ccd_reader_result)
+        self._generate_ideal_structure(component)
+
+        # download templates if the user wants them.
+        if self.pubchem is not None:
+            self._download_template(component)
+
+        # search fragment library
+        self._search_fragment_library(component)
+
+        # get scaffolds
+        self._compute_component_scaffolds(component)
+
+        # write out files
+        self._generate_depictions(component, out_dir)
+        self._export_structure_formats(component, out_dir)
 
     def _check_component_parsing(self, ccd_reader_result):
         """Checks components parsing and highlights issues encountered with
         the molecule: errors/warnings during the parsing process,
         unrecoverable sanitization issues, inchikey mismatch between what
         was in the source file and is reproduced by rdkit.
 
@@ -185,18 +180,18 @@
         Return:
             bool: Whether the ideal coordinates have been successfully
             recalculated, false otherwise.
         """
         result = component.compute_3d()
 
         if component.has_degenerated_conformer(ConformerType.Ideal):
-            logging.debug("has degenerated ideal coordinates.")
+            logging.debug(f"{component.id} has degenerated ideal coordinates.")
 
         if not result:
-            logging.debug("error in generating 3D conformation.")
+            logging.debug(f"{component.id} has error in generating 3D conformation.")
 
         return result
 
     def _search_fragment_library(self, component: Component):
         """Search fragment library to find hits
 
         Args:
@@ -235,19 +230,19 @@
         Args:
             component (Component): Component to be depicted.
             out_dir (str): Where the depictions should be stored.
         """
         depiction_result = component.compute_2d(self.depictions)
 
         if depiction_result.source == DepictionSource.Failed:
-            logging.debug("failed to generate 2D image.")
+            logging.info("failed to generate 2D image.")
         else:
             if depiction_result.score > 0.99:
-                logging.debug("collision free image could not be generated.")
-            logging.debug(
+                logging.info("collision free image could not be generated.")
+            logging.info(
                 f"2D generated using {depiction_result.source.name} with score {depiction_result.score}."
             )
 
         wedge_bonds = depiction_result.template_name != "cube"
 
         for i in range(100, 600, 100):
             component.export_2d_svg(
@@ -332,21 +327,30 @@
             path (Path): Path where the molecule will be stored.
             component (Component): Component to be written.
             alt_names (bool): Whether or not molecule will be written with
                 alternate names.
             conformer_type (Component): Conformer to be written.
         """
         try:
-            ccd_writer.write_molecule(
-                path,
-                component,
-                remove_hs=False,
-                alt_names=alt_names,
-                conf_type=conformer_type,
-            )
+            if self.procedure == "ccd":
+                ccd_writer.write_molecule(
+                    path,
+                    component,
+                    remove_hs=False,
+                    alt_names=alt_names,
+                    conf_type=conformer_type,
+                )
+            else:
+                prd_writer.write_molecule(
+                    path,
+                    component,
+                    remove_hs=False,
+                    alt_names=alt_names,
+                    conf_type=conformer_type,
+                )
         except Exception:
             logging.error(f"error writing {path}.")
 
             with open(path, "w") as f:
                 f.write("")
 
 
@@ -358,17 +362,15 @@
     Returns:
          argparse.Namespace parser
     """
     parser = argparse.ArgumentParser(
         description=__doc__, formatter_class=argparse.RawTextHelpFormatter
     )
 
-    parser.add_argument(
-        "components_cif", help="Input PDB-CCD components.cif file (must be specified)"
-    )
+    parser.add_argument("-i", "--input-cif", help="Input PDB-CCD/PDB-PRD cif file")
     parser.add_argument(
         "-g",
         "--general-templates",
         type=is_valid_path,
         default=config.general_templates,
         help="Use general templates in SDF format instead of those supplied with the code.",
     )
@@ -379,27 +381,47 @@
         help="Path to the directory with pubchem templates in sdf format.",
     )
     parser.add_argument(
         "-o",
         "--output-dir",
         type=is_valid_path,
         required=True,
-        help="Create an output directory with files suitable for PDBeChem ftp directory",
+        help="Path to output directory",
     )
     parser.add_argument(
         "-fl",
         "--fragment-library",
         type=is_valid_path,
         default=config.fragment_library,
         help="Use this fragment library in place of the one supplied with the code.",
     )
     parser.add_argument(
         "--debug", action="store_true", help="Turn on debug message logging output"
     )
 
+    # region parse procedure
+    procedure = parser.add_mutually_exclusive_group()
+    procedure.add_argument(
+        "--ccd",
+        action="store_const",
+        const="ccd",
+        dest="procedure",
+        help="Pipeline is going to process CCD mmCIF files.",
+    )
+    procedure.add_argument(
+        "--prd",
+        action="store_const",
+        const="prd",
+        dest="procedure",
+        help="Pipeline is going to process PRD mmCIF files.",
+    )
+
+    procedure.set_defaults(procedure="ccd")
+    # endregion parse procedure
+
     return parser
 
 
 # endregion
 
 
 def main():
@@ -417,14 +439,17 @@
     )
 
     logging.info("Settings:")
     for k, v in vars(args).items():
         logging.info(f'{"":5s}{k:25s}{v}')
 
     pdbechem = PDBeChemManager(
-        args.pubchem_templates, args.general_templates, args.fragment_library
+        args.pubchem_templates,
+        args.general_templates,
+        args.fragment_library,
+        args.procedure,
     )
-    pdbechem.run(args.components_cif, args.output_dir)
+    pdbechem.run(args.input_cif, args.output_dir)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/scripts/setup_pubchem_library_cli.py` & `pdbeccdutils-0.8.0/pdbeccdutils/scripts/setup_pubchem_library_cli.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_file_writing.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_file_writing.py`

 * *Files 5% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 
     @staticmethod
     @pytest.mark.parametrize("rem_hs", [True, False])
     def test_plain_cif_write(component: Component, tmpdir, rem_hs):
         path = tmpdir.join(f"{component.id}.cif")
         to_check = must_have_categories.copy()
 
-        component.ccd_cif_dict = None
+        component.ccd_cif_block = None
         ccd_writer.write_molecule(str(path), component, remove_hs=rem_hs)
         cif_block = cif.read(str(path)).sole_block()
 
         if component.id == "NA":  # Na is an atom!
             to_check.pop(2)  # remove "_chem_comp_bond"
 
         if component.id == "D3O" and rem_hs:  # D3O has single heavy atom
@@ -247,7 +247,29 @@
                 )
                 for _, values in substructure.items():
                     for value in values:
                         if value is not None:
                             assert len(value) > 0
         except CCDUtilsError:
             assert True
+
+    @staticmethod
+    def test_rdkit_conformer_writing(component: Component, tmpdir):
+        path = tmpdir.join(f"{component.id}.cif")
+        try:
+            rdkit_conformer_generated = component.compute_3d()
+            ccd_writer.write_molecule(str(path), component)
+            cif_block = cif.read(str(path)).sole_block()
+            assert cif_block
+            assert component.id == cif_block.name
+            cif_categories = cif_block.get_mmcif_category_names()
+            if rdkit_conformer_generated:
+                assert "_pdbe_chem_comp_rdkit_conformer." in cif_categories
+                rdkit_conformer = cif_block.get_mmcif_category(
+                    "_pdbe_chem_comp_rdkit_conformer."
+                )
+                for _, values in rdkit_conformer.items():
+                    for value in values:
+                        if value is not None:
+                            assert len(value) > 0
+        except CCDUtilsError:
+            assert True
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_fragment_library.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_fragment_library.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_load_eoh_cif.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_load_eoh_cif.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_parity.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_parity.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_process_components_cif_cli.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_process_components_cif_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 import pytest
 from pdbeccdutils.helpers.drawing import svg_namespace
 from pdbeccdutils.scripts.process_components_cif_cli import (
     PDBeChemManager,
     create_parser,
 )
-from pdbeccdutils.tests.tst_utilities import test_cut_down_components_cif
+from pdbeccdutils.tests.tst_utilities import cif_filename
 
 
 class TestCommandLineArgs:
     @staticmethod
     def test_with_empty_args():
         """
         User passes no args, should produce a usage statement and then
@@ -34,15 +34,15 @@
     @staticmethod
     def test_input_file_that_cannot_exist_raises_system_exit():
         parser = create_parser()
         with pytest.raises(SystemExit):
             parser.parse_args(["-o foo", "/////impossible_to_open_file", "--debug"])
 
 
-class TestCutDownComponentsCif:
+class ProcessComponentsCif:
     """
     run process_components_cif_cli on test file:
 
     cut_down_components.cif
 
     that is a cutdown components cif with just the first 5 chemical
     components definitions.
@@ -51,19 +51,20 @@
     for the creation of each directory file that is required in the
     ftp area.
     """
 
     CHEM_COMP_IDS = ["000", "001", "002", "003", "004", "ZPN"]
 
     @pytest.fixture(scope="class")
-    def pipeline_wd(self, tmpdir_factory):
+    @pytest.mark.parametrize("chem_comp_id", CHEM_COMP_IDS)
+    def pipeline_wd(self, tmpdir_factory, chem_comp_id):
         wd = tmpdir_factory.mktemp("pdbechem_test")
 
         parser = create_parser()
-        args = parser.parse_args(["-o", str(wd), test_cut_down_components_cif])
+        args = parser.parse_args(["-o", str(wd), cif_filename(chem_comp_id)])
 
         m = PDBeChemManager()
         m.run(args.components_cif, args.output_dir)
 
         return args.output_dir
 
     @staticmethod
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_property_generation.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_property_generation.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_rdkit_fixtures.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_rdkit_fixtures.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_scaffold_generation.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_scaffold_generation.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_web_services.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_web_services.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/test_write_img.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/test_write_img.py`

 * *Files identical despite different names*

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/tests/tst_utilities.py` & `pdbeccdutils-0.8.0/pdbeccdutils/tests/tst_utilities.py`

 * *Files 19% similar despite different names*

```diff
@@ -30,44 +30,69 @@
 
 test_cif = os.path.join(tests_dir(), "ccd_mmcif_test_files", "random_sample")
 test_depiction = os.path.join(tests_dir(), "ccd_mmcif_test_files", "depiction_test")
 test_cut_down_components_cif = os.path.join(
     tests_dir(), "components_cif", "cut_down_components.cif"
 )
 test_boundmolecules = os.path.join(
-    tests_dir(), "ccd_mmcif_test_files", "boundMolecule_sample"
+    tests_dir(),
+    "updated_mmcif_test_files",
 )
 
 
 def cif_filename(code):
     path = os.path.join(test_cif, f"{code}.cif")
 
     return path if os.path.isfile(path) else os.path.join(test_depiction, f"{code}.cif")
 
 
+def updated_mmcif_filename(pdb_id):
+    path = os.path.join(test_boundmolecules, pdb_id, f"{pdb_id}_processed.cif.gz")
+    if os.path.isfile(path):
+        return path
+
+
+def fixed_mmcif_filename(pdb_id):
+    path = os.path.join(test_boundmolecules, pdb_id, f"{pdb_id}_processed.cif.gz")
+    if os.path.isfile(path):
+        return path
+
+
+def bio_assembly_filename(pdb_id, au_fallback):
+    if not au_fallback:
+        path = os.path.join(test_boundmolecules, pdb_id, f"{pdb_id}_bio.cif.gz")
+    else:
+        path = os.path.join(test_boundmolecules, pdb_id, f"{pdb_id}_processed.cif.gz")
+    if os.path.isfile(path):
+        return path
+
+
+def bms_filename(pdb_id):
+    path = os.path.join(test_boundmolecules, pdb_id, "bound_molecules.json")
+    if os.path.isfile(path):
+        return path
+
+
+def remove_discarded_ligands(category, field, discarded_ligands):
+    new_category = {key: [] for key in category}
+    for i in range(len(category[field])):
+        if category[field][i] not in discarded_ligands:
+            for key in new_category:
+                new_category[key].append(category[key][i])
+
+    return new_category
+
+
 def unl_model():
     return os.path.join(tests_dir(), "ccd_mmcif_test_files", "UNL.cif")
 
 
 def supply_list_of_sample_cifs():
     """
     returns the list of sample pdb ccd cifs for test.
 
     Args:
 
     Returns:
         list of filenames
     """
     return sorted(glob.glob(os.path.join(test_cif, "*.cif")))
-
-
-def supply_list_of_cifs_with_boundmolecules():
-    """
-    returns a list of cif files with boundmolecules
-
-    Args:
-
-    Returns:
-        list of filenames
-    """
-
-    return sorted(glob.glob(os.path.join(test_boundmolecules, "*.cif")))
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/utils/pubchem_downloader.py` & `pdbeccdutils-0.8.0/pdbeccdutils/utils/pubchem_downloader.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 # specific language governing permissions and limitations
 # under the License.
 
 
 import os
 
 import numpy
-import requests
 from pdbeccdutils.core import ccd_reader
 from rdkit import Chem
 from rdkit.Chem import AllChem
+from pdbeccdutils.helpers import helper
 
 import logging
 
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
 
 def rescale_molecule(path, factor):
@@ -61,24 +61,24 @@
     """
     pubchem_api = "https://pubchem.ncbi.nlm.nih.gov/rest/pug/compound"
 
     if os.path.isfile(destination):
         return False
 
     inchi_url = f"{pubchem_api}/inchikey/{inchikey}/cids/json"
-    response = requests.get(inchi_url)
+    response = helper.requests_retry_session().get(inchi_url)
 
     if response.status_code != 200:
         return False
 
     json_file = response.json()
     cid = json_file["IdentifierList"]["CID"][0]
 
     structure_url = f"{pubchem_api}/cid/{cid}/record/SDF/?record_type=2d&response_type=save&response_basename={template_id}.sdf"
-    response = requests.get(structure_url)
+    response = helper.requests_retry_session().get(structure_url)
 
     if response.status_code != 200:
         return False
 
     with open(destination, "wb") as fp:
         fp.write(response.content)
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils/utils/web_services.py` & `pdbeccdutils-0.8.0/pdbeccdutils/utils/web_services.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # KIND, either express or implied. See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 """module handling UniChem mapping
 """
 
-import requests
+from pdbeccdutils.helpers import helper
 
 # these are the resources we agreed on providing as part of the PDBeChem
 agreed_resources = {
     "1": ("ChEMBL", "ChEMBL"),
     "2": ("DrugBank", "DrugBank"),
     "4": ("Guide to Pharmacology", "Guide to Pharmacology"),
     "6": ("KEGG LIGAND", "KEGG (Kyoto Encyclopedia of Genes and Genomes) Ligand"),
@@ -128,16 +128,17 @@
         dict of str: [str]: Resource mapping. Key is a resource name,
             value is the list of internal identifiers.
     """
     mapping = []
     url = f"{url_prefix}/{inchikey}"
 
     try:
-        headers = {"Content-Type": "application/json"}
-        r = requests.get(url, headers)
+        r = helper.requests_retry_session().get(
+            url, headers={"Content-Type": "application/json"}
+        )
         jsonFile = r.json()
 
         for entity in jsonFile:
             if entity["src_id"] not in resources:
                 continue
 
             resource = resources[entity["src_id"]]
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils.egg-info/PKG-INFO` & `pdbeccdutils-0.8.0/pdbeccdutils.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: pdbeccdutils
-Version: 0.7.2
+Version: 0.8.0
 Summary: Toolkit to deal with wwPDB chemical components definitions for small molecules.
 Home-page: http://pypi.python.org/pypi/pdbeccdutils/
 Author: Protein Data Bank in Europe
 Author-email: pdbehelp@ebi.ac.uk
 License: Apache License 2.0.
 Project-URL: Source code, https://github.com/PDBeurope/ccdutils
 Project-URL: Documentation, https://pdbeurope.github.io/ccdutils/
 Keywords: PDB CCD wwPDB small molecule
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
 
 [![CodeFactor](https://www.codefactor.io/repository/github/pdbeurope/ccdutils/badge/master)](https://www.codefactor.io/repository/github/pdbeurope/ccdutils/overview/master)  ![PYPi](https://img.shields.io/pypi/v/pdbeccdutils?color=green&style=flat)  ![GitHub](https://img.shields.io/github/license/pdbeurope/ccdutils)   ![ccdutils documentation](https://github.com/PDBeurope/ccdutils/workflows/ccdutils%20documentation/badge.svg) ![ccdutils tests](https://github.com/PDBeurope/ccdutils/workflows/ccdutils%20tests/badge.svg)
```

### Comparing `pdbeccdutils-0.7.2/pdbeccdutils.egg-info/SOURCES.txt` & `pdbeccdutils-0.8.0/pdbeccdutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,22 +10,26 @@
 pdbeccdutils.egg-info/entry_points.txt
 pdbeccdutils.egg-info/not-zip-safe
 pdbeccdutils.egg-info/requires.txt
 pdbeccdutils.egg-info/top_level.txt
 pdbeccdutils/computations/__init__.py
 pdbeccdutils/computations/parity_method.py
 pdbeccdutils/core/__init__.py
-pdbeccdutils/core/bm_reader.py
+pdbeccdutils/core/boundmolecule.py
 pdbeccdutils/core/ccd_reader.py
 pdbeccdutils/core/ccd_writer.py
+pdbeccdutils/core/clc_reader.py
+pdbeccdutils/core/clc_writer.py
 pdbeccdutils/core/component.py
 pdbeccdutils/core/depictions.py
 pdbeccdutils/core/exceptions.py
 pdbeccdutils/core/fragment_library.py
 pdbeccdutils/core/models.py
+pdbeccdutils/core/prd_reader.py
+pdbeccdutils/core/prd_writer.py
 pdbeccdutils/data/fragment_library.tsv
 pdbeccdutils/data/coordgen_templates/templates.mae
 pdbeccdutils/data/general_templates/adamantane.sdf
 pdbeccdutils/data/general_templates/cube.sdf
 pdbeccdutils/data/general_templates/decahydrocorrin.sdf
 pdbeccdutils/data/general_templates/hem.sdf
 pdbeccdutils/data/general_templates/nonbornane.sdf
@@ -37,26 +41,32 @@
 pdbeccdutils/helpers/__init__.py
 pdbeccdutils/helpers/cif_tools.py
 pdbeccdutils/helpers/conversions.py
 pdbeccdutils/helpers/drawing.py
 pdbeccdutils/helpers/helper.py
 pdbeccdutils/helpers/mol_tools.py
 pdbeccdutils/scripts/__init__.py
+pdbeccdutils/scripts/boundmolecule_cli.py
 pdbeccdutils/scripts/process_components_cif_cli.py
 pdbeccdutils/scripts/setup_pubchem_library_cli.py
 pdbeccdutils/tests/conftest.py
 pdbeccdutils/tests/test_bound_molecule.py
+pdbeccdutils/tests/test_boundmolecule_cli.py
+pdbeccdutils/tests/test_clc_reader.py
+pdbeccdutils/tests/test_clc_writer.py
 pdbeccdutils/tests/test_file_writing.py
 pdbeccdutils/tests/test_fragment_library.py
+pdbeccdutils/tests/test_helper_methods.py
 pdbeccdutils/tests/test_inchi_key_matches.py
 pdbeccdutils/tests/test_load_eoh_cif.py
 pdbeccdutils/tests/test_parity.py
 pdbeccdutils/tests/test_process_components_cif_cli.py
 pdbeccdutils/tests/test_property_generation.py
 pdbeccdutils/tests/test_rdkit_fixtures.py
+pdbeccdutils/tests/test_residue.py
 pdbeccdutils/tests/test_scaffold_generation.py
 pdbeccdutils/tests/test_web_services.py
 pdbeccdutils/tests/test_write_img.py
 pdbeccdutils/tests/tst_utilities.py
 pdbeccdutils/utils/__init__.py
 pdbeccdutils/utils/config.py
 pdbeccdutils/utils/pubchem_downloader.py
```

### Comparing `pdbeccdutils-0.7.2/setup.py` & `pdbeccdutils-0.8.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,38 +30,36 @@
     author_email="pdbehelp@ebi.ac.uk",
     license="Apache License 2.0.",
     keywords="PDB CCD wwPDB small molecule",
     url="http://pypi.python.org/pypi/pdbeccdutils/",
     packages=find_namespace_packages(),
     zip_safe=False,
     include_package_data=True,
-    python_requires=">=3.6",
+    python_requires=">=3.9",
     install_requires=["Pillow", "scipy", "numpy", "requests", "gemmi", "networkx"],
     extras_require={
         "tests": ["pytest", "pytest-cov", "pre-commit"],
         "docs": [
-            "sphinx",
+            "sphinx<7.0.0",
             "sphinx_rtd_theme",
             "sphinx-autodoc-typehints",
             "sphinx-markdown-tables",
             "myst-parser",
         ],
     },
     entry_points={
         "console_scripts": [
             "process_components_cif=pdbeccdutils.scripts.process_components_cif_cli:main",
             "setup_pubchem_library=pdbeccdutils.scripts.setup_pubchem_library_cli:main",
+            "read_boundmolecule=pdbeccdutils.scripts.boundmolecule_cli:run",
         ]
     },
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: Unix",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
```

