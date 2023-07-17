# Comparing `tmp/alphabase-1.0.2.tar.gz` & `tmp/alphabase-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphabase-1.0.2.tar", last modified: Mon Feb 13 10:21:55 2023, max compression
+gzip compressed data, was "alphabase-1.0.3.tar", last modified: Mon Jul 17 09:20:29 2023, max compression
```

## Comparing `alphabase-1.0.2.tar` & `alphabase-1.0.3.tar`

### file list

```diff
@@ -1,91 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.940995 alphabase-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-13 10:21:31.000000 alphabase-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-02-13 10:21:31.000000 alphabase-1.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-13 10:21:31.000000 alphabase-1.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-02-13 10:21:55.940995 alphabase-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-02-13 10:21:31.000000 alphabase-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.932995 alphabase-1.0.2/alphabase/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.932995 alphabase-1.0.2/alphabase/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.932995 alphabase-1.0.2/alphabase/constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/aa.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/atom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.932995 alphabase-1.0.2/alphabase/constants/const_files/
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/__emass_element.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   542725 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/__used_mod.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/amino_acid.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/common_constants.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)   153267 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/contaminants.fasta
--rw-r--r--   0 runner    (1001) docker     (123)   262552 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/modification.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/nist_element.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/protease.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/const_files/psm_reader.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/element.py
--rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/isotope.py
--rw-r--r--   0 runner    (1001) docker     (123)    12092 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/constants/modification.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/gui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/hdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/io/psm_reader/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/alphapept_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/dia_psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/dia_search_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/maxquant_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/msfragger_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/pfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/psm_reader/psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/io/tempmmap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/peptide/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/peptide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35593 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/peptide/fragment.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/peptide/mass_calc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/peptide/mobility.py
--rw-r--r--   0 runner    (1001) docker     (123)    15309 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/peptide/precursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/protein/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/protein/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42799 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/protein/fasta.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/protein/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/protein/lcp_digest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/protein/protein_level_decoy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/psm_reader/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/alphapept_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/dia_psm_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7684 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/maxquant_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6137 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/msfragger_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/pfind_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    18112 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/psm_reader/psm_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.936995 alphabase-1.0.2/alphabase/scoring/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/scoring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/scoring/fdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/scoring/feature_extraction_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/scoring/ml_scoring.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.940995 alphabase-1.0.2/alphabase/spectral_library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/decoy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/flat.py
--rw-r--r--   0 runner    (1001) docker     (123)     8643 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/reader_from_raw.py
--rw-r--r--   0 runner    (1001) docker     (123)    15030 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/spectral_library/translate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.940995 alphabase-1.0.2/alphabase/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/statistics/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-13 10:21:31.000000 alphabase-1.0.2/alphabase/yaml_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 10:21:55.932995 alphabase-1.0.2/alphabase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-13 10:21:55.000000 alphabase-1.0.2/alphabase.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 10:21:55.940995 alphabase-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-02-13 10:21:31.000000 alphabase-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 09:19:55.000000 alphabase-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11338 2023-07-17 09:19:55.000000 alphabase-1.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-17 09:19:55.000000 alphabase-1.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-07-17 09:20:29.226161 alphabase-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8362 2023-07-17 09:19:55.000000 alphabase-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.218161 alphabase-1.0.3/alphabase/
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.218161 alphabase-1.0.3/alphabase/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.218161 alphabase-1.0.3/alphabase/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/aa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/atom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.222161 alphabase-1.0.3/alphabase/constants/const_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/__emass_element.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   542725 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/__used_mod.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/amino_acid.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/common_constants.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)   153267 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/contaminants.fasta
+-rw-r--r--   0 runner    (1001) docker     (123)   262552 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/modification.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/nist_element.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/protease.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6133 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/const_files/psm_reader.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/isotope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12336 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/constants/modification.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/gui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.222161 alphabase-1.0.3/alphabase/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/hdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.222161 alphabase-1.0.3/alphabase/io/psm_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/alphapept_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/dia_psm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/dia_search_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/maxquant_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/msfragger_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/pfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/psm_reader/psm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/io/tempmmap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.222161 alphabase-1.0.3/alphabase/peptide/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/peptide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43725 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/peptide/fragment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/peptide/mass_calc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/peptide/mobility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18158 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/peptide/precursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.222161 alphabase-1.0.3/alphabase/protein/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/protein/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43152 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/protein/fasta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/protein/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/protein/lcp_digest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/protein/protein_level_decoy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/alphabase/psm_reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/alphapept_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/dia_psm_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7741 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/maxquant_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/msfragger_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/pfind_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18614 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/psm_reader/psm_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/alphabase/scoring/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/scoring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4175 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/scoring/fdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/scoring/feature_extraction_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10906 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/scoring/ml_scoring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/alphabase/spectral_library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25262 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/decoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/flat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/spectral_library/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/alphabase/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11738 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/statistics/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-07-17 09:19:55.000000 alphabase-1.0.3/alphabase/yaml_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.218161 alphabase-1.0.3/alphabase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-17 09:20:29.000000 alphabase-1.0.3/alphabase.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 09:20:29.226161 alphabase-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-07-17 09:19:55.000000 alphabase-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:20:29.226161 alphabase-1.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:19:55.000000 alphabase-1.0.3/tests/test_gui.py
```

### Comparing `alphabase-1.0.2/LICENSE` & `alphabase-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/LICENSE.txt` & `alphabase-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/PKG-INFO` & `alphabase-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabase
-Version: 1.0.2
+Version: 1.0.3
 Summary: An infrastructure Python package of the AlphaX ecosystem
 Home-page: https://github.com/MannLabs/alphabase
 Author: Mann Labs
 Author-email: jalew188@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `alphabase-1.0.2/README.md` & `alphabase-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/__init__.py` & `alphabase-1.0.3/alphabase/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!python
 
 
 __project__ = "alphabase"
-__version__ = "1.0.2"
+__version__ = "1.0.3"
 __license__ = "Apache"
 __description__ = "An infrastructure Python package of the AlphaX ecosystem"
 __author__ = "Mann Labs"
 __author_email__ = "jalew188@gmail.com"
 __github__ = "https://github.com/MannLabs/alphabase"
 __keywords__ = [
     "bioinformatics",
@@ -35,9 +35,9 @@
     "Mann Labs at MPIB": "https://www.biochem.mpg.de/mann",
     "Mann Labs at CPR": "https://www.cpr.ku.dk/research/proteomics/mann/",
     "GitHub": __github__,
     "Docs": "https://alphabase.readthedocs.io/en/latest/",
     "PyPi": "https://pypi.org/project/alphabase/",
 }
 __extra_requirements__ = {
-    "development": "requirements_development.txt",
+    "development": "extra_requirements/development.txt",
 }
```

### Comparing `alphabase-1.0.2/alphabase/__pycache__/__init__.cpython-39.pyc` & `alphabase-1.0.3/alphabase/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Feb 13 10:21:31 2023 UTC, .py size: 1388 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-00000000: 610d 0d0a 0000 0000 2b0f ea63 6c05 0000  a.......+..cl...
+00000000: 610d 0d0a 0000 0000 bb07 b564 7205 0000  a..........dr...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0006 0000 0040 0000 0073 5200 0000 6400  .....@...sR...d.
 00000030: 5a00 6401 5a01 6402 5a02 6403 5a03 6404  Z.d.Z.d.Z.d.Z.d.
 00000040: 5a04 6405 5a05 6406 5a06 6700 6407 a201  Z.d.Z.d.Z.g.d...
 00000050: 5a07 6408 5a08 6700 6409 a201 5a09 640a  Z.d.Z.g.d...Z.d.
 00000060: 6701 5a0a 640b 640c 6506 640d 640e 640f  g.Z.d.d.e.d.d.d.
 00000070: 9c05 5a0b 6410 6411 6901 5a0c 6412 5300  ..Z.d.d.i.Z.d.S.
 00000080: 2913 da09 616c 7068 6162 6173 657a 0531  )...alphabasez.1
-00000090: 2e30 2e32 5a06 4170 6163 6865 7a38 416e  .0.2Z.Apachez8An
+00000090: 2e30 2e33 5a06 4170 6163 6865 7a38 416e  .0.3Z.Apachez8An
 000000a0: 2069 6e66 7261 7374 7275 6374 7572 6520   infrastructure 
 000000b0: 5079 7468 6f6e 2070 6163 6b61 6765 206f  Python package o
 000000c0: 6620 7468 6520 416c 7068 6158 2065 636f  f the AlphaX eco
 000000d0: 7379 7374 656d 7a09 4d61 6e6e 204c 6162  systemz.Mann Lab
 000000e0: 737a 126a 616c 6577 3138 3840 676d 6169  sz.jalew188@gmai
 000000f0: 6c2e 636f 6d7a 2568 7474 7073 3a2f 2f67  l.comz%https://g
 00000100: 6974 6875 622e 636f 6d2f 4d61 6e6e 4c61  ithub.com/MannLa
@@ -48,30 +48,31 @@
 000002f0: 6573 742f 7a23 6874 7470 733a 2f2f 7079  est/z#https://py
 00000300: 7069 2e6f 7267 2f70 726f 6a65 6374 2f61  pi.org/project/a
 00000310: 6c70 6861 6261 7365 2f29 057a 114d 616e  lphabase/).z.Man
 00000320: 6e20 4c61 6273 2061 7420 4d50 4942 7a10  n Labs at MPIBz.
 00000330: 4d61 6e6e 204c 6162 7320 6174 2043 5052  Mann Labs at CPR
 00000340: 5a06 4769 7448 7562 5a04 446f 6373 5a04  Z.GitHubZ.DocsZ.
 00000350: 5079 5069 5a0b 6465 7665 6c6f 706d 656e  PyPiZ.developmen
-00000360: 747a 1c72 6571 7569 7265 6d65 6e74 735f  tz.requirements_
-00000370: 6465 7665 6c6f 706d 656e 742e 7478 744e  development.txtN
-00000380: 290d da0b 5f5f 7072 6f6a 6563 745f 5fda  )...__project__.
-00000390: 0b5f 5f76 6572 7369 6f6e 5f5f da0b 5f5f  .__version__..__
-000003a0: 6c69 6365 6e73 655f 5fda 0f5f 5f64 6573  license__..__des
-000003b0: 6372 6970 7469 6f6e 5f5f da0a 5f5f 6175  cription__..__au
-000003c0: 7468 6f72 5f5f da10 5f5f 6175 7468 6f72  thor__..__author
-000003d0: 5f65 6d61 696c 5f5f da0a 5f5f 6769 7468  _email__..__gith
-000003e0: 7562 5f5f da0c 5f5f 6b65 7977 6f72 6473  ub__..__keywords
-000003f0: 5f5f da12 5f5f 7079 7468 6f6e 5f76 6572  __..__python_ver
-00000400: 7369 6f6e 5f5f da0f 5f5f 636c 6173 7369  sion__..__classi
-00000410: 6669 6572 735f 5fda 135f 5f63 6f6e 736f  fiers__..__conso
-00000420: 6c65 5f73 6372 6970 7473 5f5f da08 5f5f  le_scripts__..__
-00000430: 7572 6c73 5f5f da16 5f5f 6578 7472 615f  urls__..__extra_
-00000440: 7265 7175 6972 656d 656e 7473 5f5f a900  requirements__..
-00000450: 720f 0000 0072 0f00 0000 fa3b 2f68 6f6d  r....r.....;/hom
-00000460: 652f 7275 6e6e 6572 2f77 6f72 6b2f 616c  e/runner/work/al
-00000470: 7068 6162 6173 652f 616c 7068 6162 6173  phabase/alphabas
-00000480: 652f 616c 7068 6162 6173 652f 5f5f 696e  e/alphabase/__in
-00000490: 6974 5f5f 2e70 79da 083c 6d6f 6475 6c65  it__.py..<module
-000004a0: 3e04 0000 0073 2600 0000 0401 0401 0401  >....s&.........
-000004b0: 0401 0401 0401 0401 0805 0401 080f 02ff  ................
-000004c0: 0404 0201 0201 0201 0201 02fb 0608 04ff  ................
+00000360: 747a 2265 7874 7261 5f72 6571 7569 7265  tz"extra_require
+00000370: 6d65 6e74 732f 6465 7665 6c6f 706d 656e  ments/developmen
+00000380: 742e 7478 744e 290d da0b 5f5f 7072 6f6a  t.txtN)...__proj
+00000390: 6563 745f 5fda 0b5f 5f76 6572 7369 6f6e  ect__..__version
+000003a0: 5f5f da0b 5f5f 6c69 6365 6e73 655f 5fda  __..__license__.
+000003b0: 0f5f 5f64 6573 6372 6970 7469 6f6e 5f5f  .__description__
+000003c0: da0a 5f5f 6175 7468 6f72 5f5f da10 5f5f  ..__author__..__
+000003d0: 6175 7468 6f72 5f65 6d61 696c 5f5f da0a  author_email__..
+000003e0: 5f5f 6769 7468 7562 5f5f da0c 5f5f 6b65  __github__..__ke
+000003f0: 7977 6f72 6473 5f5f da12 5f5f 7079 7468  ywords__..__pyth
+00000400: 6f6e 5f76 6572 7369 6f6e 5f5f da0f 5f5f  on_version__..__
+00000410: 636c 6173 7369 6669 6572 735f 5fda 135f  classifiers__.._
+00000420: 5f63 6f6e 736f 6c65 5f73 6372 6970 7473  _console_scripts
+00000430: 5f5f da08 5f5f 7572 6c73 5f5f da16 5f5f  __..__urls__..__
+00000440: 6578 7472 615f 7265 7175 6972 656d 656e  extra_requiremen
+00000450: 7473 5f5f a900 720f 0000 0072 0f00 0000  ts__..r....r....
+00000460: fa3b 2f68 6f6d 652f 7275 6e6e 6572 2f77  .;/home/runner/w
+00000470: 6f72 6b2f 616c 7068 6162 6173 652f 616c  ork/alphabase/al
+00000480: 7068 6162 6173 652f 616c 7068 6162 6173  phabase/alphabas
+00000490: 652f 5f5f 696e 6974 5f5f 2e70 79da 083c  e/__init__.py..<
+000004a0: 6d6f 6475 6c65 3e04 0000 0073 2600 0000  module>....s&...
+000004b0: 0401 0401 0401 0401 0401 0401 0401 0805  ................
+000004c0: 0401 080f 02ff 0404 0201 0201 0201 0201  ................
+000004d0: 02fb 0608 04ff                           ......
```

### Comparing `alphabase-1.0.2/alphabase/constants/aa.py` & `alphabase-1.0.3/alphabase/constants/aa.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/atom.py` & `alphabase-1.0.3/alphabase/constants/atom.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import os
 import numpy as np
 import numba
 
 from alphabase.yaml_utils import load_yaml
 
-from alphabase.constants._const import CONST_FILE_FOLDER
-
-common_const_dict:dict = load_yaml(
-    os.path.join(CONST_FILE_FOLDER, 'common_constants.yaml')
+from alphabase.constants._const import (
+    CONST_FILE_FOLDER,
+    common_const_dict
 )
 
 MASS_PROTON:float = common_const_dict['MASS_PROTON']
 MASS_ISOTOPE:float = common_const_dict['MASS_ISOTOPE']
 
 MAX_ISOTOPE_LEN:int = common_const_dict['MAX_ISOTOPE_LEN']
 EMPTY_DIST:np.ndarray = np.zeros(MAX_ISOTOPE_LEN)
```

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/__emass_element.yaml` & `alphabase-1.0.3/alphabase/constants/const_files/__emass_element.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/__used_mod.yaml` & `alphabase-1.0.3/alphabase/constants/const_files/__used_mod.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/amino_acid.yaml` & `alphabase-1.0.3/alphabase/constants/const_files/amino_acid.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/contaminants.fasta` & `alphabase-1.0.3/alphabase/constants/const_files/contaminants.fasta`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/modification.tsv` & `alphabase-1.0.3/alphabase/constants/const_files/modification.tsv`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/nist_element.yaml` & `alphabase-1.0.3/alphabase/constants/const_files/nist_element.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/const_files/protease.yaml` & `alphabase-1.0.3/alphabase/constants/const_files/protease.yaml`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/isotope.py` & `alphabase-1.0.3/alphabase/constants/isotope.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/constants/modification.py` & `alphabase-1.0.3/alphabase/constants/modification.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,14 +80,19 @@
 def load_mod_df(
     tsv:str=os.path.join(CONST_FILE_FOLDER, 'modification.tsv'),
     *,
     modloss_importance_level=1,
 ):
     global MOD_DF
     MOD_DF = pd.read_table(tsv)
+    _df = MOD_DF[MOD_DF.mod_name.str.contains(' ', regex=False)].copy()
+    _df["mod_name"] = MOD_DF.mod_name.str.replace(' ', '_', regex=False)
+    MOD_DF = pd.concat(
+        [MOD_DF, _df], ignore_index=True
+    ).drop_duplicates("mod_name")
     MOD_DF.fillna('',inplace=True)
     MOD_DF['unimod_id'] = MOD_DF.unimod_id.astype(np.int32)
     MOD_DF.set_index('mod_name', drop=False, inplace=True)
     MOD_DF['mass'] = MOD_DF.composition.apply(calc_mass_from_formula)
     MOD_DF['modloss_original'] = MOD_DF.modloss_composition.apply(calc_mass_from_formula)
     MOD_DF['modloss'] = MOD_DF['modloss_original']
     keep_modloss_by_importance(modloss_importance_level)
```

### Comparing `alphabase-1.0.2/alphabase/io/hdf.py` & `alphabase-1.0.3/alphabase/io/hdf.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/peptide/fragment.py` & `alphabase-1.0.3/alphabase/peptide/fragment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 import pandas as pd
 from typing import List, Union, Tuple, Dict, TYPE_CHECKING
 import warnings
 import numba as nb
 import logging
 
+from alphabase.constants._const import (
+    PEAK_MZ_DTYPE, PEAK_INTENSITY_DTYPE
+)
 from alphabase.peptide.mass_calc import *
 from alphabase.constants.modification import (
     calc_modloss_mass
 )
 from alphabase.constants.element import (
     MASS_H2O, MASS_PROTON, 
     MASS_NH3, MASS_H, MASS_C, MASS_O,
@@ -125,15 +128,15 @@
     '''
     _type, _ch = charged_frag_type.split('_z')
     return _type, int(_ch)
 
 def init_zero_fragment_dataframe(
     peplen_array:np.ndarray,
     charged_frag_types:List[str], 
-    dtype=np.float64
+    dtype=PEAK_MZ_DTYPE
 )->Tuple[pd.DataFrame, np.ndarray, np.ndarray]: 
     '''Initialize a zero dataframe based on peptide length 
     (nAA) array (peplen_array) and charge_frag_types (column number).
     The row number of returned dataframe is np.sum(peplen_array-1).
 
     Parameters
     ----------
@@ -159,30 +162,30 @@
         np.zeros((indices[-1],len(charged_frag_types)), dtype=dtype),
         columns = charged_frag_types
     )
     return fragment_df, indices[:-1], indices[1:]
 
 def init_fragment_dataframe_from_other(
     reference_fragment_df: pd.DataFrame,
-    dtype=np.float64
+    dtype=PEAK_MZ_DTYPE
 ):
     '''
     Init zero fragment dataframe from the `reference_fragment_df` (same rows and same columns)
     '''
     return pd.DataFrame(
         np.zeros_like(reference_fragment_df.values, dtype=dtype),
         columns = reference_fragment_df.columns
     )
 
 def init_fragment_by_precursor_dataframe(
     precursor_df,
     charged_frag_types: List[str],
     *,
     reference_fragment_df: pd.DataFrame = None,
-    dtype:np.dtype=np.float64,
+    dtype:np.dtype=PEAK_MZ_DTYPE,
     inplace_in_reference:bool=False,
 ):
     '''
     Init zero fragment dataframe for the `precursor_df`. If 
     the `reference_fragment_df` is provided, the result dataframe's 
     length will be the same as reference_fragment_df. Otherwise it 
     generates the dataframe from scratch.
@@ -201,14 +204,17 @@
 
     reference_fragment_df : pd.DataFrame
         init zero fragment_mz_df based
         on this reference. If None, fragment_mz_df will be 
         initialized by :func:`alphabase.peptide.fragment.init_zero_fragment_dataframe`.
         Defaults to None.
 
+    dtype: np.dtype
+        dtype of fragment mz values, Defaults to :data:`PEAK_MZ_DTYPE`.
+
     inplace_in_reference : bool, optional
         if calculate the fragment mz 
         inplace in the reference_fragment_df (default: False)
 
     Returns
     -------
     pd.DataFrame
@@ -230,29 +236,29 @@
             #     "`precursor_df` contains 'frag_start_idx' column, "\
             #     "please provide `reference_fragment_df` argument"
             # )
             fragment_df = pd.DataFrame(
                 np.zeros((
                     precursor_df.frag_stop_idx.max(), 
                     len(charged_frag_types)
-                )),
+                ), dtype=dtype),
                 columns = charged_frag_types
             )
         else:
             if inplace_in_reference: 
                 fragment_df = reference_fragment_df[[
                     _fr for _fr in charged_frag_types 
                     if _fr in reference_fragment_df.columns
                 ]]
             else:
                 fragment_df = pd.DataFrame(
                     np.zeros((
                         len(reference_fragment_df), 
                         len(charged_frag_types)
-                    )),
+                    ), dtype=dtype),
                     columns = charged_frag_types
                 )
     return fragment_df
 
 def update_sliced_fragment_dataframe(
     fragment_df: pd.DataFrame,
     values: np.ndarray,
@@ -285,18 +291,20 @@
     -------
     pd.DataFrame
         fragment_df after the values are set into slices
     '''
     frag_slice_list = [slice(start,end) for start,end in frag_start_end_list]
     frag_slices = np.r_[tuple(frag_slice_list)]
     if charged_frag_types is None or len(charged_frag_types)==0:
-        fragment_df.values[frag_slices, :] = values
+        fragment_df.values[frag_slices, :] = values.astype(fragment_df.dtypes[0])
     else:
         charged_frag_idxes = [fragment_df.columns.get_loc(c) for c in charged_frag_types]
-        fragment_df.iloc[frag_slices, charged_frag_idxes] = values
+        fragment_df.iloc[
+            frag_slices, charged_frag_idxes
+        ] = values.astype(fragment_df.dtypes[0])
     return fragment_df
 
 def get_sliced_fragment_dataframe(
     fragment_df: pd.DataFrame,
     frag_start_end_list:Union[List,np.ndarray],
     charged_frag_types:List = None,
 )->pd.DataFrame:
@@ -542,30 +550,31 @@
 
 def flatten_fragments(
     precursor_df: pd.DataFrame, 
     fragment_mz_df: pd.DataFrame,
     fragment_intensity_df: pd.DataFrame,
     min_fragment_intensity: float = -1,
     keep_top_k_fragments: int = 1000,
-    custom_columns:list = [
+    custom_columns : list = [
         'type','number','position','charge','loss_type'
     ],
+    custom_df : Dict[str, pd.DataFrame] = {}
 )->Tuple[pd.DataFrame, pd.DataFrame]:
     """
     Converts the tabular fragment format consisting of 
     the `fragment_mz_df` and the `fragment_intensity_df` 
     into a linear fragment format.
     The linear fragment format will only retain fragments 
     above a given intensity treshold with `mz > 0`. 
     It consists of columns: `mz`, `intensity`, 
     `type`, `number`, `charge` and `loss_type`,  
     where each column refers to:
 
-    - mz:        float64, fragment mz value
-    - intensity: float32, fragment intensity value
+    - mz:        :data:`PEAK_MZ_DTYPE`, fragment mz value
+    - intensity: :data:`PEAK_INTENSITY_DTYPE`, fragment intensity value
     - type:      int8, ASCII code of the ion type (97=a, 98=b, 99=c, 120=x, 121=y, 122=z), or more ion types in the future. See https://en.wikipedia.org/wiki/ASCII for more ASCII information
     - number:    uint32, fragment series number
     - position:  uint32, fragment position in sequence (from left to right, starts with 0)
     - charge:    int8, fragment charge
     - loss_type: int16, fragment loss type, 0=noloss, 17=NH3, 18=H2O, 98=H3PO4 (phos), ...
     
     The fragment pointers `frag_start_idx` and `frag_stop_idx` 
@@ -586,43 +595,53 @@
     
     min_fragment_intensity : float, optional
         minimum intensity which should be retained. Defaults to -1
     
     custom_columns : list, optional
         'mz' and 'intensity' columns are required. Others could be customized. 
         Defaults to ['type','number','position','charge','loss_type']
+
+    custom_df : Dict[str, pd.DataFrame], optional
+        Append custom columns by providing additional dataframes of the same shape as fragment_mz_df and fragment_intensity_df. Defaults to {}.
     
     Returns
     -------
     pd.DataFrame
         precursor dataframe with added `flat_frag_start_idx` and `flat_frag_stop_idx` columns
     pd.DataFrame
         fragment dataframe with columns: `mz`, `intensity`, `type`, `number`, 
         `charge` and `loss_type`, where each column refers to:
         
-        - mz:        float, fragment mz value
-        - intensity: float32, fragment intensity value
+        - mz:        :data:`PEAK_MZ_DTYPE`, fragment mz value
+        - intensity: :data:`PEAK_INTENSITY_DTYPE`, fragment intensity value
         - type:      int8, ASCII code of the ion type (97=a, 98=b, 99=c, 120=x, 121=y, 122=z), or more ion types in the future. See https://en.wikipedia.org/wiki/ASCII for more ASCII information
         - number:    uint32, fragment series number
         - position:  uint32, fragment position in sequence (from left to right, starts with 0)
         - charge:    int8, fragment charge
         - loss_type: int16, fragment loss type, 0=noloss, 17=NH3, 18=H2O, 98=H3PO4 (phos), ...
     """
     
     if len(precursor_df) == 0:
         return precursor_df, pd.DataFrame()
     # new dataframes for fragments and precursors are created
     frag_df = pd.DataFrame()
     frag_df['mz'] = fragment_mz_df.values.reshape(-1)
     if len(fragment_intensity_df) > 0:
-        frag_df['intensity'] = fragment_intensity_df.values.astype(np.float32).reshape(-1)
+        frag_df['intensity'] = fragment_intensity_df.values.astype(
+            PEAK_INTENSITY_DTYPE
+        ).reshape(-1)
         use_intensity = True
     else:
         use_intensity = False
 
+    # add additional columns to the fragment dataframe
+    # each column in the flat fragment dataframe is a whole pandas dataframe in the dense representation
+    for col_name, df in custom_df.items():
+        frag_df[col_name] = df.values.reshape(-1)
+
     frag_types = []
     frag_loss_types = []
     frag_charges = []
     frag_directions = [] # 'abc': direction=1, 'xyz': direction=-1, otherwise 0
     
     for col in fragment_mz_df.columns.values:
         _types = col.split('_')
@@ -768,22 +787,27 @@
 
     precursor_df[['frag_start_idx','frag_stop_idx']] = new_frag_idx
     precursor_df = precursor_df.sort_index()
 
     output_tuple = []
 
     for i in range(len(fragment_df_list)):
-        output_tuple.append(fragment_df_list[i].iloc[fragment_pointer].copy().reset_index(drop=True))
+        output_tuple.append(
+            fragment_df_list[i].iloc[
+                fragment_pointer
+            ].copy().reset_index(drop=True)
+        )
 
     return precursor_df, tuple(output_tuple)
 
 def create_fragment_mz_dataframe_by_sort_precursor(
     precursor_df: pd.DataFrame,
     charged_frag_types:List,
     batch_size:int=500000,
+    dtype:np.dtype=PEAK_MZ_DTYPE,
 )->pd.DataFrame:
     """Sort nAA in precursor_df for faster fragment mz dataframe creation.
     
     Because the fragment mz values are continous in memory, so it is faster
     when setting values in pandas.
     
     Note that this function will change the order and index of precursor_df
@@ -804,15 +828,16 @@
         precursor_df.drop(columns=[
             'frag_start_idx','frag_stop_idx'
         ], inplace=True)
 
     refine_precursor_df(precursor_df)
 
     fragment_mz_df = init_fragment_by_precursor_dataframe(
-        precursor_df, charged_frag_types
+        precursor_df, charged_frag_types, 
+        dtype=dtype,
     )
 
     _grouped = precursor_df.groupby('nAA')
     for nAA, big_df_group in _grouped:
         for i in range(0, len(big_df_group), batch_size):
             batch_end = i+batch_size
             
@@ -821,28 +846,29 @@
             mz_values = calc_fragment_mz_values_for_same_nAA(
                 df_group, nAA, charged_frag_types
             )
 
             fragment_mz_df.iloc[
                 df_group.frag_start_idx.values[0]:
                 df_group.frag_stop_idx.values[-1], :
-            ] = mz_values
+            ] = mz_values.astype(PEAK_MZ_DTYPE)
     return mask_fragments_for_charge_greater_than_precursor_charge(
             fragment_mz_df,
             precursor_df.charge.values,
             precursor_df.nAA.values,
         )
 
 def create_fragment_mz_dataframe(
     precursor_df: pd.DataFrame,
     charged_frag_types:List,
     *,
     reference_fragment_df: pd.DataFrame = None,
     inplace_in_reference:bool = False,
     batch_size:int=500000,
+    dtype:np.dtype=PEAK_MZ_DTYPE,
 )->pd.DataFrame:
     '''
     Generate fragment mass dataframe for the precursor_df. If 
     the `reference_fragment_df` is provided and precursor_df contains `frag_start_idx`, 
     it will generate  the mz dataframe based on the reference. Otherwise it 
     generates the mz dataframe from scratch.
     
@@ -878,34 +904,38 @@
         if 'frag_start_idx' in precursor_df.columns:
             # raise ValueError(
             #     "`precursor_df` contains 'frag_start_idx' column, "\
             #     "please provide `reference_fragment_df` argument"
             # )
             fragment_mz_df = init_fragment_by_precursor_dataframe(
                 precursor_df, charged_frag_types,
+                dtype=dtype,
             )
             return create_fragment_mz_dataframe(
                 precursor_df=precursor_df, 
                 charged_frag_types=charged_frag_types,
                 reference_fragment_df=fragment_mz_df,
                 inplace_in_reference=True,
                 batch_size=batch_size,
+                dtype=dtype,
             )
     if 'nAA' not in precursor_df.columns:
         # fast
         return create_fragment_mz_dataframe_by_sort_precursor(
-            precursor_df, charged_frag_types, batch_size
+            precursor_df, charged_frag_types, 
+            batch_size, dtype=dtype,
         )
 
     if (is_precursor_sorted(precursor_df) and 
         reference_fragment_df is None
     ):
         # fast
         return create_fragment_mz_dataframe_by_sort_precursor(
-            precursor_df, charged_frag_types, batch_size
+            precursor_df, charged_frag_types, 
+            batch_size, dtype=dtype
         )
 
     else:
         # slow
         if reference_fragment_df is not None:
             if inplace_in_reference:
                 fragment_mz_df = reference_fragment_df.loc[:,[
@@ -913,20 +943,21 @@
                     if _fr in reference_fragment_df.columns
                 ]]
             else:
                 fragment_mz_df = pd.DataFrame(
                     np.zeros((
                         len(reference_fragment_df), 
                         len(charged_frag_types)
-                    )),
+                    ), dtype=dtype),
                     columns = charged_frag_types
                 )
         else:
             fragment_mz_df = init_fragment_by_precursor_dataframe(
                 precursor_df, charged_frag_types,
+                dtype=dtype,
             )
 
         _grouped = precursor_df.groupby('nAA')
         for nAA, big_df_group in _grouped:
             for i in range(0, len(big_df_group), batch_size):
                 batch_end = i+batch_size
                 
@@ -1000,7 +1031,198 @@
     # First, the indices pointing to the right side are restored by masking the array for hits and looking up the right side
     joined_index[joined_index >= 0] = right_indices[joined_index[joined_index >= 0]]
 
     # Next, the left side is restored by arranging the items
     joined_index[left_indices] =  joined_index
 
     return joined_index
+
+def calc_fragment_count(
+        precursor_df : pd.DataFrame, 
+        fragment_intensity_df : pd.DataFrame
+    ):
+
+    """
+    Calculates the number of fragments for each precursor.
+
+    Parameters
+    ----------
+
+    precursor_df : pd.DataFrame
+        precursor dataframe which contains the frag_start_idx and frag_stop_idx columns
+
+    fragment_intensity_df : pd.DataFrame
+        fragment intensity dataframe which contains the fragment intensities
+
+    Returns
+    ------- 
+    numpy.ndarray
+        array with the number of fragments for each precursor
+    """
+    if not set(['frag_start_idx', 'frag_stop_idx']).issubset(precursor_df.columns):
+        raise KeyError('frag_start_idx and frag_stop_idx not in dataframe')
+    
+    n_fragments = []
+    
+    for start, stop in zip(precursor_df['frag_start_idx'].values, precursor_df['frag_stop_idx'].values):
+        n_fragments += [np.sum(fragment_intensity_df.iloc[start:stop].values > 0)]
+
+    return np.array(n_fragments)
+  
+def filter_fragment_number(
+        precursor_df : pd.DataFrame, 
+        fragment_intensity_df : pd.DataFrame,
+        n_fragments_allowed_column_name : str = 'n_fragments_allowed',
+        n_allowed : int = 999
+    ):
+
+    """
+    Filters the number of fragments for each precursor.
+        
+    Parameters
+    ----------
+
+    precursor_df : pd.DataFrame
+
+        precursor dataframe which contains the frag_start_idx and frag_stop_idx columns
+
+    fragment_intensity_df : pd.DataFrame
+        fragment intensity dataframe which contains the fragment intensities
+
+    n_fragments_allowed_column_name : str, default = 'n_fragments_allowed'
+        column name in precursor_df which contains the number of allowed fragments
+
+    n_allowed : int, default = 999
+        number of fragments which should be allowed
+
+    Returns
+    -------
+    None
+    """
+
+    if not set(['frag_start_idx', 'frag_stop_idx']).issubset(precursor_df.columns):
+        raise KeyError('frag_start_idx and frag_stop_idx not in dataframe')
+
+    for i, (start_idx, stop_idx, n_allowed_lib) in enumerate(
+        zip(
+            precursor_df['frag_start_idx'].values, 
+            precursor_df['frag_stop_idx'].values, 
+            precursor_df[n_fragments_allowed_column_name].values
+            )
+        ):
+
+        _allowed = min(n_allowed_lib, n_allowed)
+
+        intensies = fragment_intensity_df.iloc[start_idx:stop_idx].values
+        flat_intensities = np.sort(intensies.flatten())[::-1]
+        intensies[intensies <= flat_intensities[_allowed]] = 0
+        fragment_intensity_df.iloc[start_idx:stop_idx] = intensies
+        
+def calc_fragment_cardinality(
+        precursor_df,
+        fragment_mz_df,
+        group_column = 'elution_group_idx',
+        split_target_decoy = True
+    ):
+
+    """
+    Calculate the cardinality for a given fragment across a group of precursors.
+    The cardinality is the number of precursors that have a given fragment at a given position.
+
+    All precursors within a group are expected to have the same number of fragments.    
+    The precursor dataframe.
+
+    fragment_mz_df : pd.DataFrame
+        The fragment mz dataframe.
+
+    group_column : str
+        The column to group the precursors by. Integer column is expected.
+
+    split_target_decoy : bool
+        If True, the cardinality is calculated for the target and decoy precursors separately.
+
+    """
+    
+    if len(precursor_df) == 0:
+        raise ValueError('Precursor dataframe is empty.')
+    
+    if len(fragment_mz_df) == 0:
+        raise ValueError('Fragment dataframe is empty.')
+    
+    if group_column not in precursor_df.columns:
+        raise KeyError('Group column not in precursor dataframe.')
+    
+    if ('frag_start_idx' not in precursor_df.columns) or ('frag_stop_idx' not in precursor_df.columns):
+        raise KeyError('Precursor dataframe does not contain fragment indices.')
+    
+    precursor_df = precursor_df.sort_values(group_column)
+    fragment_mz = fragment_mz_df.values
+    fragment_cardinality = np.ones(fragment_mz.shape, dtype=np.uint8)
+
+    @nb.njit
+    def _calc_fragment_cardinality(
+        elution_group_idx,
+        start_idx,
+        stop_idx,
+        fragment_mz,
+        fragment_cardinality,
+    ):
+        elution_group = elution_group_idx[0]
+        elution_group_start = 0
+
+        for i in range(len(elution_group_idx)):
+            if i == len(elution_group_idx)-1 or elution_group_idx[i] != elution_group_idx[i+1]:
+                elution_group_stop = i+1
+
+            # check if whole elution group is covered
+            n_precursor = elution_group_stop - elution_group_start
+            
+            # Check that all precursors within a group have the same number of fragments.
+            nAA = stop_idx[elution_group_start:elution_group_stop] - start_idx[elution_group_start:elution_group_stop]
+            if not np.all(nAA[0] == nAA):
+                raise ValueError('All precursors within a group must have the same number of fragments.')
+
+            # within a group, check for each precursor if it has the same fragment as another precursor
+            for i in range(n_precursor):
+
+                precursor_start_idx = start_idx[elution_group_start + i]
+                precursor_stop_idx = stop_idx[elution_group_start + i]
+
+                precursor_fragment_mz = fragment_mz[precursor_start_idx:precursor_stop_idx]
+
+                for j in range(n_precursor):
+                    if i == j:
+                        continue
+
+                    other_precursor_start_idx = start_idx[elution_group_start + j]
+                    other_precursor_stop_idx = stop_idx[elution_group_start + j]
+                    other_precursor_fragment_mz = fragment_mz[other_precursor_start_idx:other_precursor_stop_idx]
+                    
+                    binary_mask = np.abs(precursor_fragment_mz - other_precursor_fragment_mz) < 0.00001
+                    
+                    fragment_cardinality[precursor_start_idx:precursor_stop_idx] += binary_mask.astype(np.uint8)
+                    
+            elution_group_start = elution_group_stop
+    if ('decoy' in precursor_df.columns) and (split_target_decoy):
+        decoy_classes = precursor_df['decoy'].unique()
+        for decoy_class in decoy_classes:
+            df = precursor_df[precursor_df['decoy'] == decoy_class]
+            _calc_fragment_cardinality(
+                df[group_column].values,
+                df['frag_start_idx'].values,
+                df['frag_stop_idx'].values,
+                fragment_mz,
+                fragment_cardinality,
+            )
+    else:
+        _calc_fragment_cardinality(
+            precursor_df[group_column].values,
+            precursor_df['frag_start_idx'].values,
+            precursor_df['frag_stop_idx'].values,
+            fragment_mz,
+            fragment_cardinality,
+        )
+
+    return pd.DataFrame(
+        fragment_cardinality, 
+        columns = fragment_mz_df.columns
+    )
```

### Comparing `alphabase-1.0.2/alphabase/peptide/mass_calc.py` & `alphabase-1.0.3/alphabase/peptide/mass_calc.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/peptide/mobility.py` & `alphabase-1.0.3/alphabase/peptide/mobility.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/peptide/precursor.py` & `alphabase-1.0.3/alphabase/peptide/precursor.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import pandas as pd
 import numpy as np
 import numba
 import multiprocessing as mp
+from tqdm import tqdm
 
 from xxhash import xxh64_intdigest
 from functools import partial
 
 from alphabase.constants.element import (
     MASS_PROTON, MASS_ISOTOPE
 )
@@ -538,7 +539,113 @@
                 processing, _count_batchify_df(
                     df_group, mp_batch_size
                 )
             )
         for df in processing:
             df_list.append(df)
     return pd.concat(df_list)
+
+def calc_precursor_isotope_intensity(
+    precursor_df,
+    max_isotope = 6, 
+    min_right_most_intensity = 0.001
+    ):
+    """Calculate isotope intensity values for precursor_df inplace.
+
+    Parameters
+    ----------
+
+    precursor_df : pd.DataFrame
+        Precursor_df to calculate isotope intensity
+
+    max_isotope : int
+        Max isotope number to calculate. Optional, by default 6
+
+    min_right_most_intensity : float
+        The minimal intensity value of the right-most peak relative to apex peak.
+
+    Returns
+    -------
+
+    pd.DataFrame
+        precursor_df with additional columns:
+    
+    """
+
+    isotope_dist = IsotopeDistribution()
+
+    col_names = ['i_{}'.format(i) for i in range(max_isotope)]
+
+    precursor_dist = np.zeros((len(precursor_df), max_isotope), dtype=np.float32)
+
+    for i in range(len(precursor_df)):
+
+        row = precursor_df.iloc[i]
+        dist, mono = isotope_dist.calc_formula_distribution(
+            get_mod_seq_formula(row['sequence'], row['mods'])
+        )
+        dist[dist <= min_right_most_intensity] = 0.
+        dist = dist / dist.sum()
+        precursor_dist[i] = dist[:max_isotope]
+
+    precursor_df[col_names] = precursor_dist
+
+    return precursor_df
+
+def calc_precursor_isotope_intensity_mp(
+    precursor_df,
+    max_isotope = 6,
+    min_right_most_intensity = 0.001,
+    mp_batch_size = 1000,
+    mp_process_num = 8,
+    progress_bar = True
+    ):
+
+    """Calculate isotope intensity values for precursor_df using multiprocessing.
+
+    Parameters
+    ----------
+
+    precursor_df : pd.DataFrame
+        Precursor_df to calculate isotope intensity
+
+    max_isotope : int
+        Max isotope number to calculate. Optional, by default 6
+
+    min_right_most_intensity : float
+        The minimal intensity value of the right-most peak relative to apex peak.
+
+    mp_batch_size : int
+        Multiprocessing batch size. Optional, by default 1000.
+
+    mp_process_num : int
+        Process number. Optional, by default 8
+
+    progress_bar : bool
+        Whether to show progress bar. Optional, by default True
+
+    Returns
+    -------
+
+    pd.DataFrame
+        precursor_df with additional columns i_0, i_1, i_2, ... i_{max_isotope-1}
+    
+    """
+
+    df_list = []
+    df_group = precursor_df.groupby('nAA')
+
+    with mp.get_context("spawn").Pool(mp_process_num) as p:
+        processing = p.imap(
+            partial(
+                calc_precursor_isotope_intensity,
+                max_isotope=max_isotope,
+                min_right_most_intensity=min_right_most_intensity
+            ), _batchify_df(df_group, mp_batch_size)
+        )
+
+        if progress_bar:
+            df_list = list(tqdm(processing, total=_count_batchify_df(df_group, mp_batch_size)))
+        else:
+            df_list = list(processing)
+
+    return pd.concat(df_list, ignore_index=True)
```

### Comparing `alphabase-1.0.2/alphabase/protein/fasta.py` & `alphabase-1.0.3/alphabase/protein/fasta.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,20 @@
 def load_all_proteins(fasta_file_list:list):
     protein_dict = {}
     for fasta in fasta_file_list:
         for protein in read_fasta_file(fasta):
             protein_dict[protein['full_name']] = protein
     return protein_dict
 
+def load_fasta_list_as_protein_df(fasta_list:list):
+    protein_dict = load_all_proteins(fasta_list)
+    return pd.DataFrame().from_dict(
+        protein_dict, orient="index"
+    ).reset_index(drop=True)
+
 def concat_proteins(protein_dict:dict, sep='$')->str:
     """Concatenate all protein sequences into a single sequence, 
     seperated by `sep ($ by default)`.
 
     Parameters
     ----------
     protein_dict : dict
@@ -462,17 +468,17 @@
     nterm_label_mod = ''
     cterm_label_mod = ''
     for label in labels:
         _, aa = label.split('@')
         if len(aa) == 1:
             label_aas += aa
             label_mod_dict[aa] = label
-        elif aa == 'Any N-term':
+        elif aa == 'Any N-term' or aa == "Any_N-term":
             nterm_label_mod = label
-        elif aa == 'Any C-term':
+        elif aa == 'Any C-term' or aa == "Any_C-term":
             cterm_label_mod = label
     return label_aas, label_mod_dict, nterm_label_mod, cterm_label_mod
         
 def create_labeling_peptide_df(peptide_df:pd.DataFrame, labels:list):
     if len(peptide_df) == 0: return peptide_df
 
     df = peptide_df.copy()
@@ -634,15 +640,15 @@
         max_missed_cleavages:int = 2,
         peptide_length_min:int = 7,
         peptide_length_max:int = 35,
         precursor_charge_min:int = 2,
         precursor_charge_max:int = 4,
         precursor_mz_min:float = 400.0, 
         precursor_mz_max:float = 2000.0,
-        var_mods:list = ['Acetyl@Protein N-term','Oxidation@M'],
+        var_mods:list = ['Acetyl@Protein_N-term','Oxidation@M'],
         min_var_mod_num:int = 0,
         max_var_mod_num:int = 2,
         fix_mods:list = ['Carbamidomethyl@C'],
         labeling_channels:dict = None,
         special_mods:list = [],
         min_special_mod_num:int = 0,
         max_special_mod_num:int = 1,
@@ -683,15 +689,15 @@
             Minimal precursor mz, by default 200.0
 
         precursor_mz_max : float, optional
             Maximal precursor mz, by default 2000.0
 
         var_mods : list, optional
             list of variable modifications, 
-            by default ['Acetyl@Protein N-term','Oxidation@M']
+            by default ['Acetyl@Protein_N-term','Oxidation@M']
 
         max_var_mod_num : int, optional
             Minimal number of variable modifications on a peptide sequence, 
             by default 0
 
         max_var_mod_num : int, optional
             Maximal number of variable modifications on a peptide sequence, 
@@ -791,27 +797,27 @@
                     if site in term_dict:
                         term_dict[site].append(term_mod)
                     else:
                         term_dict[site] = [term_mod]
                 else:
                     term_dict[site] = term_mod
             site, term = parse_term_mod(term_mod)
-            if term == "Any N-term":
+            if term == "Any N-term" or term == "Any_N-term":
                 _set_dict(pep_nterm, site, term_mod, 
                     allow_conflicts
                 )
-            elif term == 'Protein N-term':
+            elif term == 'Protein N-term' or term == "Protein_N-term":
                 _set_dict(prot_nterm, site, term_mod, 
                     allow_conflicts
                 )
-            elif term == 'Any C-term':
+            elif term == 'Any C-term' or term == "Any_C-term":
                 _set_dict(pep_cterm, site, term_mod, 
                     allow_conflicts
                 )
-            elif term == 'Protein C-term':
+            elif term == 'Protein C-term' or term == "Protein_C-term":
                 _set_dict(prot_cterm, site, term_mod, 
                     allow_conflicts
                 )
         
         for mod in self.fix_mods:
             if mod.find('@')+2 == len(mod):
                 self.fix_mod_aas += mod[-1]
@@ -1203,17 +1209,17 @@
         Parameters
         ----------
         labeling_channel_dict : dict, optional
             For example:
             ```
             {
             -1: [], # not labeled
-            0: ['Dimethyl@Any N-term','Dimethyl@K'],
-            4: ['Dimethyl:2H(4)@Any N-term','Dimethyl:2H(4)@K'],
-            8: ['Dimethyl:2H(6)13C(2)@Any N-term','Dimethyl:2H(6)13C(2)@K'],
+            0: ['Dimethyl@Any_N-term','Dimethyl@K'],
+            4: ['Dimethyl:2H(4)@Any_N-term','Dimethyl:2H(4)@K'],
+            8: ['Dimethyl:2H(6)13C(2)@Any_N-term','Dimethyl:2H(6)13C(2)@K'],
             }
             ```.
             The key name could be int (highly recommended or 
             must be in the future) or str, and the value must be 
             a list of modification names (str) in alphabase format.
             It is set to `self.labeling_channels` if None.
             Defaults to None
```

### Comparing `alphabase-1.0.2/alphabase/protein/lcp_digest.py` & `alphabase-1.0.3/alphabase/protein/lcp_digest.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/protein/protein_level_decoy.py` & `alphabase-1.0.3/alphabase/protein/protein_level_decoy.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/psm_reader/__init__.py` & `alphabase-1.0.3/alphabase/psm_reader/__init__.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/psm_reader/alphapept_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/alphapept_reader.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/psm_reader/dia_psm_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/dia_psm_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
             mod_seq_columns = mod_seq_columns,
             fixed_C57=fixed_C57,
             rt_unit=rt_unit,
             **kwargs,
         )
 
         self.mod_seq_column = 'ModifiedPeptide'
-
         self._min_max_rt_norm = True
 
     def _init_column_mapping(self):
         self.column_mapping = psm_reader_yaml[
             'spectronaut'
         ]['column_mapping']
```

### Comparing `alphabase-1.0.2/alphabase/psm_reader/maxquant_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/maxquant_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,16 @@
 
     def _init_column_mapping(self):
         self.column_mapping = psm_reader_yaml[
             'maxquant'
         ]['column_mapping']
 
     def _load_file(self, filename):
-        df = pd.read_csv(filename, sep='\t')
+        csv_sep = self._get_table_delimiter(filename)
+        df = pd.read_csv(filename, sep=csv_sep)
         self._find_mod_seq_column(df)
         df = df[~pd.isna(df['Retention time'])]
         df.fillna('', inplace=True)
         # if 'K0' in df.columns:
         #     df['Mobility'] = df['K0'] # Bug in MaxQuant? It should be 1/K0
         # min_rt = df['Retention time'].min()
         return df
```

### Comparing `alphabase-1.0.2/alphabase/psm_reader/msfragger_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/msfragger_reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pandas as pd
 
 from alphabase.psm_reader.psm_reader import (
     PSMReaderBase, psm_reader_yaml,
     psm_reader_provider
 )
 from alphabase.constants.aa import AA_ASCII_MASS
-from alphabase.constants.atom import MASS_H
+from alphabase.constants.atom import MASS_H, MASS_O, MASS_PROTON
 from alphabase.constants.modification import MOD_MASS
 
 try:
     import pyteomics.pepxml as pepxml
 except:
     pepxml = None
 
@@ -28,30 +28,40 @@
     mod_sites = []
     aa_mass_diffs = []
     aa_mass_diff_sites = []
     for mod in msf_aa_mods:
         _mass_str, site_str = mod.split('@')
         mod_mass = float(_mass_str)
         site = int(site_str)
+        cterm_position = len(sequence) + 1
         if site > 0:
-            mod_mass = mod_mass - AA_ASCII_MASS[ord(sequence[site-1])]
+            if site < cterm_position:
+                mod_mass = mod_mass - AA_ASCII_MASS[ord(sequence[site-1])]
+            else:
+                mod_mass -= (2* MASS_H + MASS_O)
         else:
             mod_mass -= MASS_H
 
         mod_translated = False
         for mod_name in mass_mapped_mods:
             if abs(mod_mass-MOD_MASS[mod_name])<mod_mass_tol:
                 if site==0:
                     _mod = mod_name.split('@')[0]+'@Any N-term'
                 elif site==1:
                     if mod_name.endswith('^Any N-term'):
                         _mod = mod_name
                         site_str = '0'
                     else:
                         _mod = mod_name.split('@')[0]+'@'+sequence[0]
+                elif site==cterm_position:
+                    if mod_name.endswith('C-term'):
+                        _mod = mod_name
+                    else:
+                        _mod = mod_name.split('@')[0]+'@Any C-term' #what if only Protein C-term is listed?
+                    site_str = '-1'
                 else:
                     _mod = mod_name.split('@')[0]+'@'+sequence[site-1]
                 if _mod in MOD_MASS:
                     mods.append(_mod)
                     mod_sites.append(site_str)
                     mod_translated = True
                     break
```

### Comparing `alphabase-1.0.2/alphabase/psm_reader/pfind_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/pfind_reader.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/psm_reader/psm_reader.py` & `alphabase-1.0.3/alphabase/psm_reader/psm_reader.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,28 +6,17 @@
 
 import alphabase.peptide.mobility as mobility
 from alphabase.peptide.precursor import (
     update_precursor_mz, reset_precursor_df
 )
 from alphabase.constants._const import CONST_FILE_FOLDER
 
+from alphabase.utils import get_delimiter
 from alphabase.yaml_utils import load_yaml
 
-def _get_delimiter(tsv_file:str):
-    if isinstance(tsv_file, io.StringIO):
-        # for unit tests
-        line = tsv_file.readline().strip()
-        tsv_file.seek(0)
-    else:
-        with open(tsv_file, "r") as f:
-            line = f.readline().strip()
-    if '\t' in line: return '\t'
-    elif ',' in line: return ','
-    else: return '\t'
-
 def translate_other_modification(
     mod_str: str, 
     mod_dict: dict
 )->str:
     '''
     Translate modifications of `mod_str` to the AlphaBase 
     format mapped by mod_dict.
@@ -175,57 +164,21 @@
             self._init_column_mapping()
 
         self._psm_df = pd.DataFrame()
         self.keep_fdr = fdr
         self.keep_decoy = keep_decoy
         self._min_max_rt_norm = False
         self._engine_rt_unit = rt_unit
+        self._min_irt_value = -100
+        self._max_irt_value = 200
 
     @property
     def psm_df(self)->pd.DataFrame:
         return self._psm_df
 
-    def import_files(self, file_list:list):
-        df_list = []
-        for _file in file_list:
-            df_list.append(self.import_file(_file))
-        self._psm_df = pd.concat(df_list, ignore_index=True)
-        return self._psm_df
-
-    def import_file(self, _file:str)->pd.DataFrame:
-        """
-        This is the main entry function of PSM readers, 
-        it imports the file with following steps:
-        ```
-        origin_df = self._load_file(_file)
-        self._translate_columns(origin_df)
-        self._translate_decoy(origin_df)
-        self._translate_score(origin_df)
-        self._load_modifications(origin_df)
-        self._translate_modifications()
-        self._post_process(origin_df)
-        ```
-        
-        Parameters
-        ----------
-        _file: str
-            file path or file stream (io).
-        """
-        origin_df = self._load_file(_file)
-        if len(origin_df) == 0:
-            self._psm_df = pd.DataFrame()
-        else:
-            self._translate_columns(origin_df)
-            self._translate_decoy(origin_df)
-            self._translate_score(origin_df)
-            self._load_modifications(origin_df)
-            self._translate_modifications()
-            self._post_process(origin_df)
-        return self._psm_df
-
     def add_modification_mapping(self, modification_mapping:dict):
         """
         Append additional modification mappings for the search engine.
 
         Parameters
         ----------
         modification_mapping : dict
@@ -310,14 +263,53 @@
     def load(self, _file)->pd.DataFrame:
         """ Wrapper for import_file() """
         if isinstance(_file, list): 
             return self.import_files(_file)
         else: 
             return self.import_file(_file)
 
+    def import_files(self, file_list:list):
+        df_list = []
+        for _file in file_list:
+            df_list.append(self.import_file(_file))
+        self._psm_df = pd.concat(df_list, ignore_index=True)
+        return self._psm_df
+
+    def import_file(self, _file:str)->pd.DataFrame:
+        """
+        This is the main entry function of PSM readers, 
+        it imports the file with following steps:
+        ```
+        origin_df = self._load_file(_file)
+        self._translate_columns(origin_df)
+        self._translate_decoy(origin_df)
+        self._translate_score(origin_df)
+        self._load_modifications(origin_df)
+        self._translate_modifications()
+        self._post_process(origin_df)
+        ```
+        
+        Parameters
+        ----------
+        _file: str
+            file path or file stream (io).
+        """
+        origin_df = self._load_file(_file)
+        if len(origin_df) == 0:
+            self._psm_df = pd.DataFrame()
+        else:
+            self._translate_columns(origin_df)
+            self._transform_table(origin_df)
+            self._translate_decoy(origin_df)
+            self._translate_score(origin_df)
+            self._load_modifications(origin_df)
+            self._translate_modifications()
+            self._post_process(origin_df)
+        return self._psm_df
+
     def _translate_decoy(
         self, 
         origin_df:pd.DataFrame=None
     ):
         pass
 
     def _translate_score(
@@ -325,29 +317,37 @@
         origin_df:pd.DataFrame=None
     ):
         # some scores are evalue/pvalue, it should be translated
         # to -log(evalue), as score is the larger the better
         pass
 
     def _get_table_delimiter(self, _filename):
-        return _get_delimiter(_filename)
+        return get_delimiter(_filename)
 
     def normalize_rt(self):
         if 'rt' in self.psm_df.columns:
             if self._engine_rt_unit == 'second':
                 # self.psm_df['rt_sec'] = self.psm_df.rt
                 self.psm_df['rt'] = self.psm_df.rt/60
             # elif self._engine_rt_unit == 'minute':
                 # self.psm_df['rt_sec'] = self.psm_df.rt*60
             min_rt = self.psm_df.rt.min()
-            if not self._min_max_rt_norm or min_rt > 0:
+            max_rt = self.psm_df.rt.max()
+            if min_rt < 0: # iRT
+                if min_rt < self._min_irt_value:
+                    min_rt = self._min_irt_value
+                if max_rt > self._max_irt_value:
+                    max_rt = self._max_irt_value
+
+            elif not self._min_max_rt_norm :
                 min_rt = 0
-            self.psm_df['rt_norm'] = (
+            
+            self.psm_df['rt_norm'] = ((
                 self.psm_df.rt - min_rt
-            ) / (self.psm_df.rt.max()-min_rt)
+            ) / (max_rt-min_rt)).clip(0, 1)
 
     def norm_rt(self):
         self.normalize_rt()
 
     def normalize_rt_by_raw_name(self):
         if not 'rt' in self.psm_df.columns:
             return
@@ -412,21 +412,37 @@
         None
             Add information inplace into self._psm_df
         """
         mapped_columns = self._find_mapped_columns(origin_df)
         self._psm_df = pd.DataFrame()
         for col, map_col in mapped_columns.items():
             self._psm_df[col] = origin_df[map_col]
-                
+               
         if (
             'scan_num' in self._psm_df.columns and 
             not 'spec_idx' in self._psm_df.columns
         ):
             self._psm_df['spec_idx'] = self._psm_df.scan_num - 1
     
+    def _transform_table(self, origin_df:pd.DataFrame):
+        """
+        Transform the dataframe format if needed.
+        Usually only needed in combination with spectral libraries.
+
+        Parameters
+        ----------
+        origin_df : pd.DataFrame
+            df of other search engines
+
+        Returns
+        -------
+        None
+            Add information inplace into self._psm_df
+        """
+        pass
 
     def _load_modifications(self, origin_df:pd.DataFrame):
         """Read modification information from 'origin_df'. 
         Some of search engines use modified_sequence, some of them
         use additional columns to store modifications and the sites.
 
         Parameters
```

### Comparing `alphabase-1.0.2/alphabase/scoring/fdr.py` & `alphabase-1.0.3/alphabase/scoring/fdr.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/scoring/feature_extraction_base.py` & `alphabase-1.0.3/alphabase/scoring/feature_extraction_base.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/scoring/ml_scoring.py` & `alphabase-1.0.3/alphabase/scoring/ml_scoring.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/spectral_library/base.py` & `alphabase-1.0.3/alphabase/spectral_library/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import pandas as pd
 import numpy as np
 import typing
 import logging
+import copy
+import warnings
 
 import alphabase.peptide.fragment as fragment
 import alphabase.peptide.precursor as precursor
 from alphabase.io.hdf import HDF_File
 
 class SpecLibBase(object):
     """
@@ -127,14 +129,142 @@
     @property
     def fragment_intensity_df(self)->pd.DataFrame:
         """
         The fragment intensity dataframe with 
         fragment types as columns (['b_z1', 'y_z2', ...])
         """
         return self._fragment_intensity_df
+    
+    def copy(self):
+        """
+        Return a copy of the spectral library object.
+        
+        Returns
+        -------
+        SpecLibBase
+            A copy of the spectral library object.
+        """
+        new_instance = self.__class__()
+        new_instance.__dict__ = copy.deepcopy(self.__dict__)
+
+        return new_instance
+    
+    def append(
+            self, 
+            other : 'SpecLibBase',
+            dfs_to_append : typing.List[str] = ['_precursor_df','_fragment_intensity_df', '_fragment_mz_df','_fragment_intensity_predicted_df'],
+        ):
+        """
+
+        Append another SpecLibBase object to the current one in place. 
+        All matching dataframes in the second object will be appended to the current one. Dataframes missing in the current object will be ignored.
+        All matching columns in the second object will be appended to the current one. Columns missing in the current object will be ignored.
+        Dataframes and columns missing in the second object will raise an error.
+        
+        Parameters
+        ----------
+        other : SpecLibBase
+            Second SpecLibBase object to be appended.
+            
+        dfs_to_append : list, optional
+            List of dataframes to be appended.
+            Defaults to ['_precursor_df','_fragment_intensity_df', '_fragment_mz_df','_fragment_intensity_predicted_df'].
+            
+        Returns
+        -------
+        None
+            
+        """
+
+        def check_matching_columns(df1, df2):
+            # check if the columns are compatible
+            # the first dataframe should have all the columns of the second dataframe, otherwise raise error
+            # the second dataframe may have more columns, but they will be dropped with a warning
+            missing_columns = set(df1.columns) - set(df2.columns)
+            if len(missing_columns) > 0:
+                raise ValueError(
+                    f"The columns are not compatible. {missing_columns} are missing in the dataframe which should be appended."
+                )
+            
+            missing_columns = set(df2.columns) - set(df1.columns)
+            if len(missing_columns) > 0:
+                warnings.warn(
+                    f"Unmatched columns in second dataframe will be dropped: {missing_columns}."
+                )
+
+            return df1.columns.values
+        
+        # get subset of dataframes and columns to append
+        # will fail if the speclibs are not compatible
+        matching_columns = []
+        for attr in dfs_to_append:
+            if hasattr(self, attr) and hasattr(other, attr):
+                matching_columns.append(
+                    check_matching_columns(
+                        getattr(self, attr), getattr(other, attr)
+                    )
+                )
+            elif hasattr(self, attr) and not hasattr(other, attr):
+                raise ValueError(
+                    f"The libraries can't be appended as {attr} is missing in the second library."
+                )
+            else:
+                matching_columns.append([])
+
+        n_fragments = []
+        # get subset of dfs_to_append starting with _fragment
+        for attr in dfs_to_append:
+            if attr.startswith('_fragment'):
+                if hasattr(self, attr):
+                    n_current_fragments = len(getattr(self, attr))
+                    if n_current_fragments > 0:
+                        n_fragments += [n_current_fragments]
+
+        if not np.all(np.array(n_fragments) == n_fragments[0]):
+            raise ValueError(
+                f"The libraries can't be appended as the number of fragments in the current libraries are not the same."
+            )
+        
+        for attr, matching_columns in zip(
+            dfs_to_append,
+            matching_columns
+        ):
+            if hasattr(self, attr) and hasattr(other, attr):
+                
+                current_df = getattr(self, attr)
+
+                # copy dataframes to avoid changing the original ones
+                other_df = getattr(other, attr)[matching_columns].copy()
+
+                if attr.startswith('_precursor'):
+                    
+                    frag_idx_increment = 0
+                    for fragment_df in ['_fragment_intensity_df', '_fragment_mz_df']:
+                        if hasattr(self, fragment_df):
+                            if len(getattr(self, fragment_df)) > 0:
+                                frag_idx_increment = len(getattr(self, fragment_df))
+   
+                    if 'frag_start_idx' in other_df.columns:
+                        other_df['frag_start_idx'] += frag_idx_increment
+
+                    if 'frag_stop_idx' in other_df.columns:
+                        other_df['frag_stop_idx'] += frag_idx_increment
+
+                setattr(
+                    self, attr,
+                    pd.concat(
+                        [
+                            current_df,
+                            other_df
+                        ],
+                        axis=0,
+                        ignore_index=True,
+                        sort=False
+                    ).reset_index(drop=True)
+                )
 
     def refine_df(self):
         """
         Sort nAA and reset_index for faster calculation (or prediction)
         """
         precursor.refine_precursor_df(
             self._precursor_df
@@ -188,14 +318,65 @@
 
     def update_precursor_mz(self):
         """
         Calculate precursor mz for self._precursor_df,
         and clip the self._precursor_df using `self.clip_by_precursor_mz_`
         """
         self.calc_precursor_mz()
+
+    def calc_precursor_isotope_intensity(self,
+        multiprocessing : bool=True,
+        max_isotope = 6,
+        min_right_most_intensity = 0.001,
+        mp_batch_size = 1000,
+        mp_process_num = 8
+        ):
+        """
+        Calculate and append the isotope intensity columns into self.precursor_df.
+        See `alphabase.peptide.precursor.calc_precursor_isotope_intensity` for details.
+    
+        Parameters
+        ----------
+
+        max_isotope : int, optional
+            The maximum isotope to calculate.
+
+        min_right_most_intensity : float, optional
+            The minimum intensity of the right most isotope.
+
+        mp_batch_size : int, optional
+            The batch size for multiprocessing.
+
+        mp_processes : int, optional
+            The number of processes for multiprocessing.
+        
+        """
+
+        if 'precursor_mz' not in self._precursor_df.columns:
+            self.calc_precursor_mz()
+            self.clip_by_precursor_mz_()
+
+        if multiprocessing and len(self.precursor_df)>mp_batch_size:
+            (
+                self._precursor_df
+            ) = precursor.calc_precursor_isotope_intensity_mp(
+                self.precursor_df, 
+                max_isotope = max_isotope,
+                min_right_most_intensity = min_right_most_intensity,
+                mp_process_num = mp_process_num,
+            )
+        else:
+            (
+                self._precursor_df
+            ) = precursor.calc_precursor_isotope_intensity(
+                self.precursor_df, 
+                max_isotope = max_isotope,
+                min_right_most_intensity = min_right_most_intensity,
+            )
+            
     
     def calc_precursor_isotope(self, 
         multiprocessing:bool=True,
         mp_process_num:int=8,
         mp_process_bar=None,
         min_precursor_num_to_run_mp:int=1000,
     ):
@@ -286,15 +467,49 @@
                 )
             # only update fragment mz df
             else:
                 (self._precursor_df, (self._fragment_mz_df,)) = fragment.remove_unused_fragments(
                     self._precursor_df, (self._fragment_mz_df,)
                 )
 
+    def calc_fragment_count(self):
+        """
+        Count the number of non-zero fragments for each precursor.
+        Creates the column 'n_fragments' in self._precursor_df.
+        """
+
+        self._precursor_df['n_fragments'] = fragment.calc_fragment_count(
+            self._precursor_df,
+            self._fragment_intensity_df
+        )
+    
+    def filter_fragment_number(
+            self, 
+            n_fragments_allowed_column_name='n_fragments_allowed', 
+            n_allowed=999
+        ):
+        """
+        Filter the top k fragments for each precursor based on a global setting and a precursor wise column.
+        The smaller one will be used. Can be used to make sure that target and decoy have the same number of fragments.
+
+        Parameters
+        ----------
+        n_fragments_allowed_column_name : str, optional, default 'n_fragments_allowed'
+            The column name in self._precursor_df that contains the number of fragments allowed for each precursor.
+
+        n_allowed : int, optional, default 999
+            The global setting for the number of fragments allowed for each precursor.
+        """
 
+        fragment.filter_fragment_number(
+            self._precursor_df,
+            self._fragment_intensity_df,
+            n_fragments_allowed_column_name=n_fragments_allowed_column_name,
+            n_allowed=n_allowed
+        )
 
     def _get_hdf_to_save(self, 
         hdf_file, 
         delete_existing=False
     ):
         """Internal function to get a HDF group to write"""
         _hdf = HDF_File(
```

### Comparing `alphabase-1.0.2/alphabase/spectral_library/decoy.py` & `alphabase-1.0.3/alphabase/spectral_library/decoy.py`

 * *Files identical despite different names*

### Comparing `alphabase-1.0.2/alphabase/spectral_library/flat.py` & `alphabase-1.0.3/alphabase/spectral_library/flat.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         """ Protein dataframe """
         return self._protein_df
 
     def parse_base_library(self, 
         library:SpecLibBase,
         keep_original_frag_dfs:bool=True,
         copy_precursor_df:bool=False,
+        **kwargs
     ):
         """ 
         Flatten an library object of SpecLibBase or its inherited class. 
         This method will generate :attr:`precursor_df` and :attr:`fragment_df`
         The fragments in fragment_df can be located by 
         `flat_frag_start_idx` and `flat_frag_stop_idx` in precursor_df. 
 
@@ -107,14 +108,15 @@
         self._precursor_df, self._fragment_df = flatten_fragments(
             library.precursor_df.copy() if copy_precursor_df else library.precursor_df, 
             library.fragment_mz_df, 
             library.fragment_intensity_df,
             min_fragment_intensity=self.min_fragment_intensity,
             keep_top_k_fragments=self.keep_top_k_fragments,
             custom_columns=self.custom_fragment_df_columns,
+            **kwargs
         )
         
         if hasattr(library, 'protein_df'):
             self._protein_df = library.protein_df
         else:
             self._protein_df = pd.DataFrame()
```

### Comparing `alphabase-1.0.2/alphabase/spectral_library/reader.py` & `alphabase-1.0.3/alphabase/spectral_library/reader.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,119 +1,191 @@
 import typing
+import os
 import numpy as np
 import pandas as pd
 
 from alphabase.peptide.mobility import mobility_to_ccs_for_df
 from alphabase.io.psm_reader.dia_search_reader import SpectronautReader
+from alphabase.io.psm_reader.maxquant_reader import MaxQuantReader
 from alphabase.spectral_library.base import SpecLibBase
 from alphabase.psm_reader.psm_reader import psm_reader_yaml
 from alphabase.psm_reader import psm_reader_provider
 
-class SWATHLibraryReader(SpectronautReader, SpecLibBase):
+from alphabase.constants._const import CONST_FILE_FOLDER, PEAK_INTENSITY_DTYPE
+from alphabase.yaml_utils import load_yaml
+
+class LibraryReaderBase(MaxQuantReader, SpecLibBase):
     def __init__(self,
         charged_frag_types:typing.List[str] = [
             'b_z1','b_z2','y_z1', 'y_z2', 
             'b_modloss_z1','b_modloss_z2',
             'y_modloss_z1', 'y_modloss_z2'
         ],
         column_mapping:dict = None,
         modification_mapping:dict = None,
         fdr = 0.01,
         fixed_C57 = False,
         mod_seq_columns=psm_reader_yaml[
-            'spectronaut'
+            'library_reader_base'
         ]['mod_seq_columns'],
         rt_unit='irt',
         precursor_mz_min:float = 400,
         precursor_mz_max:float = 2000,
         decoy:str = None,
         **kwargs
     ):
+        """
+
+        Base class for reading spectral libraries from long format csv files.
+
+        Parameters
+        ----------
+
+        charged_frag_types: list of str
+            List of fragment types to be used in the spectral library.
+            The default is ['b_z1','b_z2','y_z1', 'y_z2', 'b_modloss_z1','b_modloss_z2','y_modloss_z1', 'y_modloss_z2']
+
+        column_mapping: dict
+            Dictionary mapping the column names in the csv file to the column names in the spectral library.
+            The default is None, which uses the `library_reader_base` column mapping in `psm_reader.yaml` 
+
+        modification_mapping: dict
+            Dictionary mapping the modification names in the csv file to the modification names in the spectral library.
+
+        fdr: float
+            False discovery rate threshold for filtering the spectral library.
+            default is 0.01
+
+        fixed_C57: bool
+    
+        mod_seq_columns: list of str
+            List of column names in the csv file containing the modified sequence.
+            By default the mapping is taken from `psm_reader.yaml`
+
+        rt_unit: str
+            Unit of the retention time column in the csv file.
+            The default is 'irt'
+
+        precursor_mz_min: float
+            Minimum precursor m/z value for filtering the spectral library.
+
+        precursor_mz_max: float
+            Maximum precursor m/z value for filtering the spectral library.
+
+        decoy: str
+            Decoy type for the spectral library.
+            Can be either `pseudo_reverse` or `diann`
+
+        """
         SpecLibBase.__init__(self,
             charged_frag_types = charged_frag_types,
             precursor_mz_min=precursor_mz_min,
             precursor_mz_max=precursor_mz_max,
             decoy=decoy
         )
 
-        SpectronautReader.__init__(self, 
+        MaxQuantReader.__init__(self, 
             column_mapping = column_mapping,
             modification_mapping = modification_mapping,
             fdr = fdr,
             keep_decoy = False,
             fixed_C57 = fixed_C57,
             mod_seq_columns=mod_seq_columns,
             rt_unit=rt_unit,
         )
 
-        self._frag_type_columns = "FragmentType FragmentIonType ProductType ProductIonType".split(' ')
-        self._frag_number_columns = "FragmentNumber FragmentSeriesNumber".split(' ')
-        self._frag_charge_columns = "FragmentCharge FragmentIonCharge ProductCharge ProductIonCharge".split(' ')
-        self._frag_loss_type_columns = "FragmentLossType FragmentIonLossType ProductLossType ProductIonLossType".split(' ')
-        self._frag_inten_columns = "RelativeIntensity RelativeFragmentIntensity RelativeFragmentIonIntensity LibraryIntensity".split(' ')
+    def _init_column_mapping(self):
+        """
+        Initialize the column mapping from the `psm_reader.yaml` file.
+        """
+        self.column_mapping = psm_reader_yaml[
+            'library_reader_base'
+        ]['column_mapping']
 
     def _find_key_columns(self, lib_df:pd.DataFrame):
-        def find_col(target_columns, df_columns):
-            for col in target_columns:
-                if col in df_columns:
-                    return col
-            return None
-
-        self.mod_seq_col = find_col(self._mod_seq_columns, lib_df.columns)
-        
-        self.mapped_peptide_columns = self._find_mapped_columns(lib_df)
-
-        self.frag_type_col = find_col(self._frag_type_columns, lib_df.columns)
-        self.frag_num_col = find_col(self._frag_number_columns, lib_df.columns)
-        self.frag_charge_col = find_col(self._frag_charge_columns, lib_df.columns)
-        self.frag_loss_type_col = find_col(self._frag_loss_type_columns, lib_df.columns)
-        self.frag_inten_col = find_col(self._frag_inten_columns, lib_df.columns)
-
-        if self.frag_loss_type_col is None:
-            self.frag_loss_type_col = 'FragmentLossType'
-            lib_df[self.frag_loss_type_col] = ''
+
+        """
+        Find and create the key columns for the spectral library.
+
+        Parameters
+        ----------
+
+        lib_df: pd.DataFrame
+            Dataframe containing the spectral library.
+        
+        """
+
+        if 'fragment_loss_type' not in lib_df.columns:
+            lib_df['fragment_loss_type'] = ''
+
+        lib_df['fragment_loss_type'].fillna('', inplace=True)
+        lib_df['fragment_loss_type'].replace('noloss','',inplace=True)
+
+
+        if 'mods' not in lib_df.columns:
+            lib_df['mods'] = ''
+
+        if 'mod_sites' not in lib_df.columns:
+            lib_df['mod_sites'] = ''
 
     def _get_fragment_intensity(self, lib_df:pd.DataFrame):
+        """
+
+        Create the self._fragment_intensity dataframe from a given spectral library.
+        In the process, the input dataframe is converted from long format to a precursor dataframe and returned.
+
+        Parameters
+        ----------
+        lib_df: pd.DataFrame
+            Dataframe containing the spectral library.
+
+        Returns
+        -------
+        precursor_df: pd.DataFrame
+            Dataframe containing the fragment intensity.
+        
+        """
         frag_col_dict = dict(zip(
             self.charged_frag_types, 
             range(len(self.charged_frag_types))
         ))
 
         self._find_key_columns(lib_df)
-        lib_df[self.frag_loss_type_col].fillna('', inplace=True)
-        lib_df[self.frag_loss_type_col].replace('noloss','',inplace=True)
 
-        group_cols = [
-            self.mod_seq_col, 
-            self.mapped_peptide_columns['sequence'], 
-            self.mapped_peptide_columns['charge'],
-        ]
-
-        if 'raw_name' in self.mapped_peptide_columns:
-            group_cols.append(self.mapped_peptide_columns['raw_name'])
+        # drop all columns which are all NaN as they prohibit grouping
+        lib_df = lib_df.dropna(axis=1, how='all')
 
-        col_list_dict = dict([(col, []) for col in self.mapped_peptide_columns.values()])
-        col_list_dict[self.mod_seq_col] = []
+        precursor_df_list = []
 
         frag_intens_list = []
         nAA_list = []
+
+        fragment_columns = [
+            'fragment_mz','fragment_type','fragment_charge','fragment_series','fragment_loss_type','fragment_intensity'
+        ]
+
+        # by default, all non-fragment columns are used to group the library
+        non_fragment_columns = list(set(lib_df.columns) - set(fragment_columns))
+
         
         for keys, df_group in lib_df.groupby(
-            group_cols
+            non_fragment_columns
         ):
+            precursor_columns = dict(zip(non_fragment_columns, keys))
+
+            nAA = len(precursor_columns['sequence'])
 
-            nAA = len(keys[1])
-            nAA_list.append(nAA)
             intens = np.zeros(
-                (nAA-1, len(self.charged_frag_types)),dtype=np.float32
+                (nAA-1, len(self.charged_frag_types)),
+                dtype=PEAK_INTENSITY_DTYPE,
             )
             for frag_type, frag_num, loss_type, frag_charge, inten in df_group[
                 [
-                    self.frag_type_col,self.frag_num_col,self.frag_loss_type_col,
-                    self.frag_charge_col,self.frag_inten_col
+                    'fragment_type','fragment_series','fragment_loss_type',
+                    'fragment_charge','fragment_intensity'
                 ]
             ].values:
                 if frag_type in 'abc':
                     frag_num -= 1
                 elif frag_type in 'xyz':
                     frag_num = nAA-frag_num-1
                 else:
@@ -123,30 +195,33 @@
                     frag_type = f'{frag_type}_z{frag_charge}'
                 elif loss_type == 'H3PO4':
                     frag_type = f'{frag_type}_modloss_z{frag_charge}'
                 elif loss_type == 'H2O':
                     frag_type = f'{frag_type}_H2O_z{frag_charge}'
                 elif loss_type == 'NH3':
                     frag_type = f'{frag_type}_NH3_z{frag_charge}'
+                elif loss_type == 'unknown': # DiaNN+fragger
+                    frag_type = f'{frag_type}_z{frag_charge}'
                 else:
                     continue
                 
                 if frag_type not in frag_col_dict:
                     continue
                 frag_col_idx = frag_col_dict[frag_type]
                 intens[frag_num, frag_col_idx] = inten
             max_inten = np.max(intens)
             if max_inten <= 0: continue
             intens /= max_inten
 
-            for col, col_list in col_list_dict.items():
-                col_list.append(df_group[col].values[0])
+            precursor_df_list.append(precursor_columns) 
             frag_intens_list.append(intens)
-        
-        df = pd.DataFrame(col_list_dict)
+            nAA_list.append(nAA)
+
+        df = pd.DataFrame(precursor_df_list)
+
 
         self._fragment_intensity_df = pd.DataFrame(
             np.concatenate(frag_intens_list),
             columns = self.charged_frag_types
         )
 
         indices = np.zeros(len(nAA_list)+1, dtype=np.int64)
@@ -154,51 +229,61 @@
         indices = np.cumsum(indices)
 
         df['frag_start_idx'] = indices[:-1]
         df['frag_stop_idx'] = indices[1:]
 
         return df
 
-    def _load_file(self, filename):
-        self.csv_sep = self._get_table_delimiter(filename)
-        df = pd.read_csv(filename, sep=self.csv_sep)
-        self._find_mod_seq_column(df)
+    def _load_file(
+            self, 
+            filename:str
+        ):
+        """
+        Load the spectral library from a csv file.
+        Reimplementation of `PSMReaderBase._translate_columns`.
+        """
 
-        df = self._get_fragment_intensity(df)
+        csv_sep = self._get_table_delimiter(filename)
 
+        df = pd.read_csv(filename, sep=csv_sep)
+        self._find_mod_seq_column(df)
+        
         return df
-
-    def _post_process(self, 
-        lib_df
+        
+    def _post_process(
+        self, 
+        lib_df:pd.DataFrame,
     ):  
-        self._psm_df['nAA'] = self._psm_df.sequence.str.len()
-        self._psm_df[
-            ['frag_start_idx','frag_stop_idx']
-        ] = lib_df[['frag_start_idx','frag_stop_idx']]
+        """
+        Process the spectral library and create the `fragment_intensity`, `fragment_mz`dataframe.
+        Reimplementation of `PSMReaderBase._post_process`.
+        """
+        
+        if 'nAA' not in self._psm_df.columns:
+            self._psm_df['nAA'] = self._psm_df.sequence.str.len()
 
+        self._psm_df = self._get_fragment_intensity(self._psm_df)
+        
         self.normalize_rt_by_raw_name()
-
-        if (
-            'mobility' in self._psm_df.columns
-        ):
+        
+        if 'mobility' in self._psm_df.columns:
             self._psm_df['ccs'] = (
                 mobility_to_ccs_for_df(
                     self._psm_df,
                     'mobility'
                 )
             )
-        
-        self._psm_df = self._psm_df[
-            ~self._psm_df.mods.isna()
-        ].reset_index(drop=True)
 
+        self._psm_df.drop('modified_sequence', axis=1, inplace=True)
         self._precursor_df = self._psm_df
 
         self.calc_fragment_mz_df()
 
+# legacy
+SWATHLibraryReader = LibraryReaderBase
 
 class LibraryReaderFromRawData(SpecLibBase):
     def __init__(self, 
         charged_frag_types:typing.List[str] = [
             'b_z1','b_z2','y_z1', 'y_z2', 
             'b_modloss_z1','b_modloss_z2',
             'y_modloss_z1', 'y_modloss_z2'
```

### Comparing `alphabase-1.0.2/alphabase/spectral_library/translate.py` & `alphabase-1.0.3/alphabase/spectral_library/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,16 +89,16 @@
     fragment_mz_df:pd.DataFrame, 
     fragment_inten_df:pd.DataFrame, 
     top_n_inten:int,
     frag_type_head:str='FragmentType',
     frag_mass_head:str='FragmentMz',
     frag_inten_head:str='RelativeIntensity',
     frag_charge_head:str='FragmentCharge',
+    frag_series_head:str='FragmentNumber',
     frag_loss_head:str='FragmentLossType',
-    frag_num_head:str='FragmentNumber',
     verbose=True,
 ):
     '''
     Convert alphabase library into a single dataframe. 
     This method is not important, as it will be only 
     used by DiaNN, or spectronaut, or others
     '''
@@ -139,25 +139,25 @@
         frag_inten_list.append(intens[idx_in_df])
         frag_num_list.append(frag_nums)
     
     df[frag_type_head] = frag_type_list
     df[frag_mass_head] = frag_mass_list
     df[frag_inten_head] = frag_inten_list
     df[frag_charge_head] = frag_charge_list
+    df[frag_series_head] = frag_num_list
     df[frag_loss_head] = frag_loss_list
-    df[frag_num_head] = frag_num_list
 
     return explode_multiple_columns(df, 
         [
             frag_type_head,
             frag_mass_head,
             frag_inten_head,
             frag_charge_head,
+            frag_series_head,
             frag_loss_head,
-            frag_num_head
         ]
     )
 
     # try:
     #     return df.explode([
     #         frag_type_head,
     #         frag_mass_head,
@@ -237,15 +237,15 @@
     min_frag_nAA = 0,
     modloss:str='H3PO4',
     frag_type_head:str='FragmentType',
     frag_mass_head:str='FragmentMz',
     frag_inten_head:str='RelativeIntensity',
     frag_charge_head:str='FragmentCharge',
     frag_loss_head:str='FragmentLossType',
-    frag_num_head:str='FragmentNumber',
+    frag_series_head:str='FragmentNumber',
     verbose = True,
 )->pd.DataFrame:
     '''
     Convert alphabase library to diann (or Spectronaut) library dataframe
     This method is not important, as it will be only 
     used by DiaNN, or spectronaut, or others
 
@@ -349,15 +349,15 @@
         speclib._fragment_intensity_df,
         top_n_inten=keep_k_highest_fragments,
         frag_type_head=frag_type_head,
         frag_mass_head=frag_mass_head,
         frag_inten_head=frag_inten_head,
         frag_charge_head=frag_charge_head,
         frag_loss_head=frag_loss_head,
-        frag_num_head=frag_num_head,
+        frag_series_head=frag_series_head,
         verbose=verbose
     )
     df = df[df['RelativeIntensity']>min_frag_intensity]
     df.loc[df[frag_loss_head]=='modloss',frag_loss_head] = modloss
 
     return df.drop(['frag_start_idx','frag_stop_idx'], axis=1)
 
@@ -384,15 +384,15 @@
         self.tsv = tsv
         super().__init__(*args, **kwargs)
 
     def run(self):
         while True:
             df, batch = self.task_queue.get()
             if df is None: break
-            df.to_csv(self.tsv, header=(batch==0), sep="\t", mode="a", index=False)
+            df.to_csv(self.tsv, header=(batch==0), sep="\t", mode="a", index=False, lineterminator="\n")
 
 def translate_to_tsv(
     speclib:SpecLibBase,
     tsv:str,
     *,
     keep_k_highest_fragments:int=12,
     min_frag_mz:float = 200,
@@ -439,13 +439,13 @@
             min_frag_intensity=min_frag_intensity,
             min_frag_nAA=0,
             verbose=False
         )
         if multiprocessing:
             df_head_queue.put((df, i))
         else:
-            df.to_csv(tsv, header=(i==0), sep="\t", mode='a', index=False)
+            df.to_csv(tsv, header=(i==0), sep="\t", mode='a', index=False, lineterminator="\n")
     if multiprocessing:
         df_head_queue.put((None, None))
         print("Translation finished, it will take several minutes to export the rest precursors to the tsv file...")
         writing_process.join()
```

### Comparing `alphabase-1.0.2/alphabase/statistics/regression.py` & `alphabase-1.0.3/alphabase/statistics/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,21 +180,28 @@
 
         # reshape both arrays to column arrays
         if len(x.shape) == 1:
             x = x[...,np.newaxis]
 
         if len(y.shape) == 1:
             y = y[...,np.newaxis]
+
+        # remove outliers by using only the 0.5 to 99.5 percentile
+        percentiles = np.percentile(x, [0.1, 99.9])
+        mask = (percentiles[0] < x[:,0]) & (x[:,0] < percentiles[1])
+        x = x[mask,...]
+        y = y[mask,...]
         
         # === end === sanity checks ===
 
         # create flat version of the array for 
         idx_sorted = np.argsort(x.flat)
         x_sorted = x.flat[idx_sorted]
 
+
         # stores if uniform training is still possible this round
         uniform = self.uniform
 
         # === start === kernel indices ===
         # get kernel indices matrix of shape (n_kernels, 2)
         if uniform:
             kernel_indices = self.kernel_indices_uniform(x_sorted)
```

### Comparing `alphabase-1.0.2/alphabase.egg-info/PKG-INFO` & `alphabase-1.0.3/alphabase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphabase
-Version: 1.0.2
+Version: 1.0.3
 Summary: An infrastructure Python package of the AlphaX ecosystem
 Home-page: https://github.com/MannLabs/alphabase
 Author: Mann Labs
 Author-email: jalew188@gmail.com
 License: Apache
 Project-URL: Mann Labs at MPIB, https://www.biochem.mpg.de/mann
 Project-URL: Mann Labs at CPR, https://www.cpr.ku.dk/research/proteomics/mann/
```

### Comparing `alphabase-1.0.2/alphabase.egg-info/SOURCES.txt` & `alphabase-1.0.3/alphabase.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -65,11 +65,13 @@
 alphabase/scoring/feature_extraction_base.py
 alphabase/scoring/ml_scoring.py
 alphabase/spectral_library/__init__.py
 alphabase/spectral_library/base.py
 alphabase/spectral_library/decoy.py
 alphabase/spectral_library/flat.py
 alphabase/spectral_library/reader.py
-alphabase/spectral_library/reader_from_raw.py
 alphabase/spectral_library/translate.py
+alphabase/spectral_library/validate.py
 alphabase/statistics/__init__.py
-alphabase/statistics/regression.py
+alphabase/statistics/regression.py
+tests/test_cli.py
+tests/test_gui.py
```

### Comparing `alphabase-1.0.2/alphabase.egg-info/requires.txt` & `alphabase-1.0.3/alphabase.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 contextlib2
 xxhash
 biopython
 psutil
 tqdm
 scikit-learn
 regex
-pydivsufsort
 
 [:sys_platform == "win32"]
 pywin32
 
 [development]
 jupyter
 twine
@@ -86,8 +85,7 @@
 contextlib2
 xxhash
 biopython
 psutil
 tqdm
 scikit-learn
 regex
-pydivsufsort
```

### Comparing `alphabase-1.0.2/setup.py` & `alphabase-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,19 +20,15 @@
 
 
 def get_requirements():
     extra_requirements = {}
     requirement_file_names = package2install.__extra_requirements__
     requirement_file_names[""] = "requirements.txt"
     for extra, requirement_file_name in requirement_file_names.items():
-        full_requirement_file_name = os.path.join(
-            "requirements",
-            requirement_file_name,
-        )
-        with open(full_requirement_file_name) as requirements_file:
+        with open(requirement_file_name) as requirements_file:
             if extra != "":
                 extra_stable = f"{extra}-stable"
             else:
                 extra_stable = "stable"
             extra_requirements[extra_stable] = []
             extra_requirements[extra] = []
             for line in requirements_file:
```

