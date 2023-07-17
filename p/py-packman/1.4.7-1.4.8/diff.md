# Comparing `tmp/py-packman-1.4.7.tar.gz` & `tmp/py-packman-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-packman-1.4.7.tar", last modified: Tue Mar 28 01:36:43 2023, max compression
+gzip compressed data, was "py-packman-1.4.8.tar", last modified: Mon Jul 17 20:50:44 2023, max compression
```

## Comparing `py-packman-1.4.7.tar` & `py-packman-1.4.8.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.506256 py-packman-1.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-28 01:36:23.000000 py-packman-1.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-28 01:36:43.506256 py-packman-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-03-28 01:36:23.000000 py-packman-1.4.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.494256 py-packman-1.4.7/packman/
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.494256 py-packman-1.4.7/packman/anm/
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/anm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/anm/anm.py
--rw-r--r--   0 runner    (1001) docker     (123)    43076 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/anm/hd_anm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.494256 py-packman-1.4.7/packman/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/apps/calculate_entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/apps/dci.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/apps/hdanm.py
--rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/apps/predict_hinge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.498256 py-packman-1.4.7/packman/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    37380 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/bin/GUI.py
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/bin/PACKMAN.py
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   200702 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/bin/logo.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.498256 py-packman-1.4.7/packman/constants/
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/constants/Constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/constants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.498256 py-packman-1.4.7/packman/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/entropy/entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.498256 py-packman-1.4.7/packman/geometry/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/geometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/geometry/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.498256 py-packman-1.4.7/packman/gnm/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/gnm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/gnm/gnm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/atom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/bond.py
--rw-r--r--   0 runner    (1001) docker     (123)    13882 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/hetmol.py
--rw-r--r--   0 runner    (1001) docker     (123)    41529 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    24406 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/molecule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8775 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/molecule/residue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/tests/anm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/anm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/anm/test_anm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/data/1prw.hng
--rw-r--r--   0 runner    (1001) docker     (123)   151551 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/data/1prw.pdb
--rw-r--r--   0 runner    (1001) docker     (123)   355003 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/data/4hla.cif
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/tests/entropy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/entropy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/entropy/test_entropy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/tests/molecule/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/molecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/tests/molecule/test_molecule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.502256 py-packman-1.4.7/packman/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-03-28 01:36:23.000000 py-packman-1.4.7/packman/utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 01:36:43.506256 py-packman-1.4.7/py_packman.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-28 01:36:43.000000 py-packman-1.4.7/py_packman.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 01:36:43.506256 py-packman-1.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-03-28 01:36:23.000000 py-packman-1.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-17 20:50:30.000000 py-packman-1.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-17 20:50:44.927688 py-packman-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-07-17 20:50:30.000000 py-packman-1.4.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.919688 py-packman-1.4.8/packman/
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/anm/
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14338 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/anm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43080 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/anm/hd_anm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/calculate_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/dci.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/hdanm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19366 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/apps/predict_hinge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    37386 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/GUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/PACKMAN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   200702 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/bin/logo.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/constants/Constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/entropy/entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/geometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/geometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4743 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/geometry/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/gnm/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/gnm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8075 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/gnm/gnm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.923688 py-packman-1.4.8/packman/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/atom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8783 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/bond.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8141 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/hetmol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41580 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24426 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/molecule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13024 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/molecule/residue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/anm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/anm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/anm/test_anm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/1prw.hng
+-rw-r--r--   0 runner    (1001) docker     (123)   151551 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/1prw.pdb
+-rw-r--r--   0 runner    (1001) docker     (123)   355003 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/4hla.cif
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/entropy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/entropy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/entropy/test_entropy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/tests/molecule/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/molecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4215 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/tests/molecule/test_molecule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/packman/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-07-17 20:50:30.000000 py-packman-1.4.8/packman/utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:50:44.927688 py-packman-1.4.8/py_packman.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:50:44.000000 py-packman-1.4.8/py_packman.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:50:44.927688 py-packman-1.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-07-17 20:50:30.000000 py-packman-1.4.8/setup.py
```

### Comparing `py-packman-1.4.7/LICENSE` & `py-packman-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/PKG-INFO` & `py-packman-1.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-packman
-Version: 1.4.7
+Version: 1.4.8
 Summary: A software package for molecular PACKing and Motion ANalysis (PACKMAN)
 Home-page: https://github.com/Pranavkhade/PACKMAN
 Author: Pranav Khade
 Author-email: pranavk@iastate.edu
 License: MIT
 Keywords: protein,dynamics,protein packing,protein domain,protein hinge
 Classifier: Intended Audience :: Education
```

### Comparing `py-packman-1.4.7/README.md` & `py-packman-1.4.8/README.md`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/__init__.py` & `py-packman-1.4.8/packman/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 from .bin import *
 from .anm import *
 from .constants import *
 from .utilities import *
 
 
 #VERSION CHANGE HERE CHANGES IT IN docs AND setup.py
-__version__='1.4.7'
+__version__='1.4.8'
```

### Comparing `py-packman-1.4.7/packman/anm/__init__.py` & `py-packman-1.4.8/packman/anm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/anm/anm.py` & `py-packman-1.4.8/packman/anm/anm.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def __init__(self, atoms, gamma=1.0, dr=15.0, power=0, pf=None):
         self.gamma   = gamma
         self.dr      = dr
         self.power   = power
         self.pf      = pf
         self.atoms   = [i for i in atoms]
         self.coords  = numpy.array([i.get_location() for i in self.atoms])
-        if self.pf != None and self.pf <= 0:
+        if self.pf is not None and self.pf <= 0:
             raise Exception("pf value cannot be zero or negative")
         if self.gamma <= 0:
             raise Exception("gamma value cannot be zero or negative")
         if self.dr <= 0:
             raise Exception("distance cutoff value cannot be zero or negative")
 
         self.fluctuations       = None
@@ -190,15 +190,15 @@
                     hessian[j*3:j*3+3, j*3:j*3+3] = hessian[j*3:j*3+3, j*3:j*3+3] - derivative
                     #abs added to avoid negative numbers
                     d = numpy.sqrt(s_ij)
                     lobj = [[d,d,d],[d,d,d], [d,d,d]]
                     dmat = numpy.array(lobj)
                     distance_mat[i*3:i*3+3, j*3:j*3+3] = dmat
 
-        if self.pf != None:
+        if self.pf is not None:
             hessian = numpy.divide(hessian, distance_mat)
         
         self.hessian=hessian
         return True
     
     def calculate_decomposition(self):
         """Decompose the Hessian Matrix of the ANM model.
```

### Comparing `py-packman-1.4.7/packman/anm/hd_anm.py` & `py-packman-1.4.8/packman/anm/hd_anm.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.pf      = pf
         self.atoms   = atoms
         self.HNGinfo = load_hinge(hng_file)
         self.RT_eigen_vectors = None
 
         #Coords are in the same order as the atoms
         self.coords  = numpy.array([i.get_location() for i in atoms])
-        if self.pf != None and self.pf <= 0:
+        if self.pf is not None and self.pf <= 0:
             raise Exception("pf value cannot be zero or negative")
         if self.gamma <= 0:
             raise Exception("gamma value cannot be zero or negative")
         if self.dr <= 0:
             raise Exception("distance cutoff value cannot be zero or negative")
         
         ##To Verify that the hessian is same as ANM (Part 1/2)
@@ -496,15 +496,15 @@
         Note:
             - Fluctuations are calculated. use hdANM().get_fluctuations() to obtain the fluctuations.
             - Endmode needs to be put in the code if and when required.
             - hdANM().fluctuations stores the output of this function.
         """
         x0 = numpy.array([i.get_location() for i in self.atoms])
 
-        if(self.RT_eigen_vectors == None):
+        if(self.RT_eigen_vectors is None):
             self.calculate_RT_eigen_vectors()
         
         exploded_vectors = self.RT_eigen_vectors
         exploded_vectors = exploded_vectors.T
 
         mode_bfactors=[]
         for numi,i in enumerate(self.eigen_values[6:]):
@@ -521,15 +521,15 @@
         Pseudoinverse is calculated using this methd. Please note that first 6 rigid modes are eliminated in this calculation.
 
         Note:
             - Can be called on demand or can be called from get method automatically (Needs thinking)
         """
         
             
-        if(self.RT_eigen_vectors == None):
+        if(self.RT_eigen_vectors is None):
             self.calculate_RT_eigen_vectors()
         EVec=self.get_RT_eigen_vectors().T
         if(n_modes=="all"):
             self.hessian_pseudoinverse = numpy.matmul(  numpy.matmul( EVec[6:].transpose() , numpy.diag(1/self.get_eigenvalues()[6:]) )  , EVec[6:]  )
         else:
             self.hessian_pseudoinverse = numpy.matmul(  numpy.matmul( EVec[6:6+n_modes].transpose() , numpy.diag(1/self.get_eigenvalues()[6:6+n_modes]) )  , EVec[6:6+n_modes]  )
```

### Comparing `py-packman-1.4.7/packman/apps/__init__.py` & `py-packman-1.4.8/packman/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/apps/calculate_entropy.py` & `py-packman-1.4.8/packman/apps/calculate_entropy.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/apps/dci.py` & `py-packman-1.4.8/packman/apps/dci.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,18 +42,18 @@
         
     def __init__(self, mol, cutoff = 7.0, chain = None, n_com = None):
         self.molObj = mol
         assert type( self.molObj ) == Protein, "mol should be a packman.molecule.Protein object."
 
         if chain:
             self.atoms = [i for i in self.molObj[0][chain].get_calpha()]
-            collect_resi = [i.get_atoms() for i in self.molObj[0][chain].get_residues() if i.get_calpha() != None]
+            collect_resi = [i.get_atoms() for i in self.molObj[0][chain].get_residues() if i.get_calpha() is not None]
         else:
             self.atoms = [i for i in self.molObj[0].get_calpha()]
-            collect_resi = [i.get_atoms() for i in self.molObj[0].get_residues() if i.get_calpha() != None]
+            collect_resi = [i.get_atoms() for i in self.molObj[0].get_residues() if i.get_calpha() is not None]
             
         if n_com:
             if (n_com < 2) or (n_com > len(self.atoms)):
                 raise ValueError("Value of n_com should be 2 or greater but less than or equal to the maximum number of residues in the protein")
                 
         if cutoff <= 0:
             raise ValueError("Value of cutoff can only be a positive integer")
```

### Comparing `py-packman-1.4.7/packman/apps/hdanm.py` & `py-packman-1.4.8/packman/apps/hdanm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/apps/predict_hinge.py` & `py-packman-1.4.8/packman/apps/predict_hinge.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,15 +317,15 @@
             Hinges.append( Hinge(numi,Alpha,i,hstats,p_value))
         
         #Assigning domain IDs
         AllChainResidues = [i for i in HingeResidues[0].get_parent().get_residues()]
         #If sorting is needed
         DomainNumber, flag = 0, True
         for i in AllChainResidues:
-            if(i.get_domain_id() == None):
+            if(i.get_domain_id() is None):
                 i.set_domain_id('DM'+str(DomainNumber))
                 flag=True
             elif(i.get_domain_id()[:2] == 'FL' and flag):
                 DomainNumber+=1
                 flag=False
         
         AllChainResidues[0].get_parent().set_hinges(Hinges)
```

### Comparing `py-packman-1.4.7/packman/bin/GUI.py` & `py-packman-1.4.8/packman/bin/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -327,15 +327,15 @@
         self.output_filename.insert(END,self.Box1.get()+'.hng')
         self.output_filename.grid(row=2,column=2,sticky=N+S+E+W, padx=10, pady=10 )
 
         def write_hng_file():
             ALL_RESIDUES = {}
             for i in mol[0].get_chains():
                 try:
-                    ALL_RESIDUES[i.get_id()] = sorted([i.get_id() for i in mol[0][i.get_id()].get_residues() if i!=None])
+                    ALL_RESIDUES[i.get_id()] = sorted([i.get_id() for i in mol[0][i.get_id()].get_residues() if i is not None])
                 except:
                     None
 
             select_count = 0
             last_hinge_end = 0
             fh = open(self.output_filename.get(), 'w')
             for numi, i in enumerate(Selected_Hinges):
```

### Comparing `py-packman-1.4.7/packman/bin/PACKMAN.py` & `py-packman-1.4.8/packman/bin/PACKMAN.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
     Todo:
         * Change the main() to accomodate iterative alpha shape search
     
     """
     args=IO()
 
-    if(args.command==None):
+    if(args.command is None):
         logging.error('Please provide the appropriate input. Enter "python -m packman -h" for more details.')
         exit()
 
     logging.basicConfig(stream=args.logfile)
 
     if(args.pdbid is not None):
         molecule.download_structure(args.pdbid, save_name=args.filename.split('.')[0], ftype=args.filename.split('.')[1])
```

### Comparing `py-packman-1.4.7/packman/bin/__init__.py` & `py-packman-1.4.8/packman/bin/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/bin/logo.ico` & `py-packman-1.4.8/packman/bin/logo.ico`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/constants/Constants.py` & `py-packman-1.4.8/packman/constants/Constants.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/entropy/entropy.py` & `py-packman-1.4.8/packman/entropy/entropy.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     Args:
         atoms ([packman.molecule.Atom]) : The group of atoms user wisher to calculate Packing Entropy with.
         chains ([str]/str)              : Chain IDs for the Entropy calculation (None means all the chains are included; single string means only one chain ID; multiple chains should be an array of strings).
         probe_size (float)              : Radius of the probe to generate the surface points (This value should not be less than 1;Read the Publication for more details)
         onspherepoints (int)            : Number of points to be generated around each point for the surface (Read the Publication for more details)
     """
     def __init__(self, atoms, chains=None, probe_size=1.4, onspherepoints=30):
-        if(chains==None):
+        if(chains is None):
             self.atoms = [i for i in atoms]
         else:
             #Single or multiple chain IDs provided. If there are multiple chain ids, they should be in an array form.
             try:
                 self.atoms = [i for i in atoms if i.get_parent().get_parent().get_id() in chains]
             except:
                 self.atoms = [i for i in atoms if i.get_parent().get_parent().get_id() == chains]
```

### Comparing `py-packman-1.4.7/packman/geometry/geometry.py` & `py-packman-1.4.8/packman/geometry/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -93,20 +93,20 @@
             return False
 
     #get_alphashape function commands.
     DelaunayTesssellations = Delaunay( [i.get_location() for i in atoms] )
     AlphaShape   = []
     ProteinGraph = Graph()
 
-    for a, b, c, d in DelaunayTesssellations.vertices:
+    for a, b, c, d in DelaunayTesssellations.simplices:
         Tetrahydron = [atoms[a],atoms[b],atoms[c],atoms[d]]
         Centre, Radius = Circumsphere(Tetrahydron)
         #Alpha Test
         if( calculate_alphafitness(alpha,Radius) ):
             ProteinGraph.add_nodes_from( [a,b,c,d] )
             ProteinGraph.add_edges_from( [(a,b),(a,c),(a,d),(b,c),(b,d),(c,d)] )
             AlphaShape.append( [atoms[a],atoms[b],atoms[c],atoms[d]] )
 
     if(get_graph):
         return AlphaShape, ProteinGraph
     else:
-        return AlphaShape
+        return AlphaShape
```

### Comparing `py-packman-1.4.7/packman/gnm/__init__.py` & `py-packman-1.4.8/packman/gnm/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/gnm/gnm.py` & `py-packman-1.4.8/packman/gnm/gnm.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             - Endmode needs to be put in the code if and when required.
         """
         '''
             inverse=inverse+(float(1)/eigen_values[i])*eigen_vectors[:,i]*eigen_vectors[:,i].transpose()
         return inverse.diagonal()
         '''
         #Initiate
-        if(endmode==None):
+        if(endmode is None):
             stop_at = len(self.eigen_values)
         else:
             try:
                 stop_at = int(endmode)
             except:
                 logging.warning('Please provide valid input for the "endmode" parameter.')
```

### Comparing `py-packman-1.4.7/packman/molecule/__init__.py` & `py-packman-1.4.8/packman/molecule/__init__.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/molecule/annotations.py` & `py-packman-1.4.8/packman/molecule/annotations.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/molecule/atom.py` & `py-packman-1.4.8/packman/molecule/atom.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/molecule/bond.py` & `py-packman-1.4.8/packman/molecule/bond.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/molecule/chain.py` & `py-packman-1.4.8/packman/molecule/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,23 +222,23 @@
         
         Returns:
             atom (:py:class:`packman.molecule.Atom`): Atom of the given ID if successful; None otherwise.
         """
         the_atom = None
         for i in self.__Residues:
             the_atom =  self.__Residues[i].get_atom(idx)
-            if(the_atom!=None):
+            if(the_atom is not None):
                 break
             
-        if(the_atom==None):
+        if(the_atom is None):
             for i in self.__HetMols:
                 the_atom =  self.__HetMols[i].get_atom(idx)
-                if(the_atom!=None):
+                if(the_atom is not None):
                     break
-        if(the_atom!=None):
+        if(the_atom is not None):
             return the_atom
         else:
             logging.info('The atom with the given ID is not found in the Residues/HetMols')
             return None
     
     def get_residue(self,idx):
         """Get the residue of the given ID.
```

### Comparing `py-packman-1.4.7/packman/molecule/hetmol.py` & `py-packman-1.4.8/packman/molecule/hetmol.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/molecule/model.py` & `py-packman-1.4.8/packman/molecule/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,18 +86,18 @@
         self.__AllHetMols=AllHetMols
         self.__parent = None
         
         #Properties are the entities that are not included in the PDB files and are obtained by calculations
         self.__properties = {}
 
     def __getitem__(self,ChainID):
-        try:
-            return self.__AllChains[ChainID]
-        except KeyError:
-            logging.warning('Please provide a valid chain ID.')
+        #try:
+        return self.__AllChains[ChainID]
+        #except KeyError:
+        #    logging.warning('Please provide a valid chain ID.')
     
     #Get Functions
     def get_id(self):
         """Get the ID of the 'Model'
 
         Returns:
             int if successful, None otherwise.
@@ -146,23 +146,23 @@
         
         Returns:
             atom (:py:class:`packman.molecule.Atom`): Atom of the given ID if successful; None otherwise.
         """
         the_atom = None
         for i in self.__AllResidues:
             the_atom =  self.__AllResidues[i].get_atom(idx)
-            if(the_atom!=None):
+            if(the_atom is not None):
                 break
             
-        if(the_atom==None):
+        if(the_atom is None):
             for i in self.__AllHetMols:
                 the_atom =  self.__AllHetMols[i].get_atom(idx)
-                if(the_atom!=None):
+                if(the_atom is not None):
                     break
-        if(the_atom!=None):
+        if(the_atom is not None):
             return the_atom
         else:
             logging.info('The atom with the given ID is not found in this Model')
             return None
     
     def get_chain(self,ChainID):
         """Get the corresponding 'Chain' object
@@ -307,19 +307,19 @@
                 return None
         except:
             logging.warning('Please check if the Model.calculate_bonds() was executed successfully.')
             return None
         
         atom1, atom2 = bond.get_atoms()
 
-        if( neighbor1 == None ):
+        if( neighbor1 is None ):
             logging.error('neighbour1 not selected. Options available for neighbour1: ' +  ', '.join( [str(i) for i in self.__ModelGraph[atom1.get_id()] if i != atom2.get_id() ] ) )
             return None
 
-        if( neighbor2 == None ):
+        if( neighbor2 is None ):
             logging.error('neighbour2 not selected. Options available for neighbour2: ' + ', '.join( [str(i) for i in self.__ModelGraph[atom2.get_id()] if i != atom1.get_id() ]  ) )
             return None
         
         if(type(neighbor1)==int):
             neighbor1 = self.__AllAtoms[neighbor1]
         elif(type(neighbor1)==type(atom1)):
             None
@@ -435,19 +435,19 @@
                 return None
         except:
             logging.warning('Please check if the Model.calculate_bonds() was executed successfully.')
             return None
         
         atom1, atom2 = bond.get_atoms()
 
-        if( neighbor1 == None ):
+        if( neighbor1 is None ):
             logging.error('neighbour1 not selected. Options available for neighbour1: ' +  ', '.join( [str(i) for i in self.__ModelGraph[atom1.get_id()] if i != atom2.get_id() ] ) )
             return None
 
-        if( neighbor2 == None ):
+        if( neighbor2 is None ):
             logging.error('neighbour2 not selected. Options available for neighbour2: ' + ', '.join( [str(i) for i in self.__ModelGraph[atom2.get_id()] if i != atom1.get_id() ]  ) )
             return None
         
         if(type(neighbor1)==int):
             neighbor1 = self.__AllAtoms[neighbor1]
         elif(type(neighbor1)==type(atom1)):
             None
@@ -589,26 +589,26 @@
                                         col_seq.append( k )
                                     else:
                                         temp_dict = {col_seq[numl]:l for numl,l in enumerate(k.split())}
                                         #Actual approach: find chains -> residue/hetatm -> get the atom with the same name
                                         chain1, chain2 = self[temp_dict['_struct_conn.ptnr1_label_asym_id']], self[temp_dict['_struct_conn.ptnr2_label_asym_id']]
                                                                                 
                                         ptnr1 = chain1.get_residue( int(temp_dict['_struct_conn.ptnr1_auth_seq_id']) )
-                                        if(ptnr1==None):
+                                        if(ptnr1 is None):
                                             ptnr1 = chain1.get_hetmol( int(temp_dict['_struct_conn.ptnr1_auth_seq_id']) )
-                                            if(ptnr1==None):
+                                            if(ptnr1 is None):
                                                 ptnr1 = chain1.get_hetmol( temp_dict['_struct_conn.ptnr1_label_comp_id']+temp_dict['_struct_conn.ptnr1_auth_seq_id'] )
 
                                         ptnr2 = chain2.get_residue( int(temp_dict['_struct_conn.ptnr2_auth_seq_id']) )
-                                        if(ptnr2==None):
+                                        if(ptnr2 is None):
                                             ptnr2 = chain2.get_hetmol( int(temp_dict['_struct_conn.ptnr2_auth_seq_id']) )
-                                            if(ptnr2==None):
+                                            if(ptnr2 is None):
                                                 ptnr2 = chain2.get_hetmol( temp_dict['_struct_conn.ptnr2_label_comp_id']+temp_dict['_struct_conn.ptnr2_auth_seq_id'] )
                                         
-                                        if(ptnr1!=None and ptnr2!=None):
+                                        if(ptnr1 is not None and ptnr2 is not None):
                                             atm1 = ptnr1.get_atom(temp_dict['_struct_conn.ptnr1_label_atom_id'])
                                             atm2 = ptnr2.get_atom(temp_dict['_struct_conn.ptnr2_label_atom_id'])
 
                                             cif_vocab2pacman= {'covale':'covalent' , 'disulf':'covalent-single', 'hydrog':'hydrogen', 'metalc':'non-covalent'}
 
                                             bond_type = None
                                             try:        
@@ -641,15 +641,15 @@
                 continue
             #This section is for the default bonds (Not in the connect record)
             for i in resi:
                 try:
                     for j in aa_connectivity[i.get_name()]:
                         try:
                             atom1, atom2 =  i.get_atom(j[0]), i.get_atom(j[1])
-                            if(atom1!=None and atom2!=None and atom1.get_parent().get_parent().get_id() == atom2.get_parent().get_parent().get_id() ):
+                            if(atom1 is not None and atom2 is not None and atom1.get_parent().get_parent().get_id() == atom2.get_parent().get_parent().get_id() ):
                                 counter += 1
                                 if(j[2]=='SING'):
                                     bond = Bond(counter, atom1, atom2, 'covalent-single', source='RCSB/aa-variants-v1.cif')
                                 elif(j[2]=='DOUB'):
                                     bond = Bond(counter, atom1, atom2, 'covalent-double', source='RCSB/aa-variants-v1.cif')
                                 else:
                                     bond = Bond(counter, atom1, atom2, 'covalent', source='RCSB/aa-variants-v1.cif')
```

### Comparing `py-packman-1.4.7/packman/molecule/molecule.py` & `py-packman-1.4.8/packman/molecule/molecule.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
                             Occupancy = float(_[ column_names['_atom_site.occupancy'] ])
                             bfactor = float(_[ column_names['_atom_site.B_iso_or_equiv'] ])
                             Element = _[ column_names['_atom_site.type_symbol'] ]
                             Charge = _[ column_names['_atom_site.pdbx_formal_charge'] ]
 
                             #If particular atom is already present, dont add it again; alternate id must be present (_atom_site.label_alt_id)
                             try:
-                                if( AllResidues[FrameNumber-1][str(ResidueNumber)+ChainID].get_atom(AtomName)!= None ):
+                                if( AllResidues[FrameNumber - 1][str(ResidueNumber) + ChainID].get_atom(AtomName) is not None ):
                                     continue
                             except Exception as e:
                                 #Alternate atom exists
                                 None
 
                             try:
                                 AllAtoms[FrameNumber-1][AtomID] = Atom(AtomID,AtomName,Coordinates,Occupancy,bfactor,Element,Charge, AllResidues[FrameNumber-1][str(ResidueNumber)+ChainID] )
@@ -333,15 +333,15 @@
                             Occupancy = float(_[ column_names['_atom_site.occupancy'] ])
                             bfactor = float(_[ column_names['_atom_site.B_iso_or_equiv'] ])
                             Element = _[ column_names['_atom_site.type_symbol'] ]
                             Charge = _[ column_names['_atom_site.pdbx_formal_charge'] ]
 
                             #If particular atom is already present, dont add it again; alternate id must be present (_atom_site.label_alt_id)
                             try:
-                                if( AllHetMols[FrameNumber-1][str(HetMolNumber)+ChainID].get_atom(AtomName)!= None ):
+                                if( AllHetMols[FrameNumber - 1][str(HetMolNumber) + ChainID].get_atom(AtomName) is not None ):
                                     continue
                             except Exception as e:
                                 #Alternate atom exists
                                 None
 
                             try:
                                 AllHetAtoms[FrameNumber-1][AtomID] = Atom(AtomID,AtomName,Coordinates,Occupancy,bfactor,Element,Charge, AllHetMols[FrameNumber-1][str(HetMolNumber)+ChainID] )
@@ -508,15 +508,15 @@
     if(ftype=='cif'):
         response=ur.urlopen('https://files.rcsb.org/view/'+pdbid+'.cif')
     elif(ftype=='pdb'):
         response=ur.urlopen('https://files.rcsb.org/view/'+pdbid+'.pdb')
     else:
         print('Please provide appropriate "ftype" argument. (cif/pdb).')
 
-    if(save_name==None):
+    if(save_name is None):
         try:
             open(pdbid+'.'+ftype,'wb').write(response.read())
         except(IOError):
             None
     else:
         try:
             open(save_name+'.'+ftype,'wb').write(response.read())
```

### Comparing `py-packman-1.4.7/packman/molecule/protein.py` & `py-packman-1.4.8/packman/molecule/protein.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,20 +82,20 @@
 
         Args:
             all_models (bool, optional): Get sequence of the all frames; useless if sequence accross the models is identical. Defaults to False.
 
         Returns:
             Protein sequence in FASTA format.
         """
-        for model in self:
+        for model_ in self:
             try:
-                return model.get_sequence()
-            except:
+                return model_.get_sequence()
+            except Exception:
                 None
-            if(all_models==False):
+            if(all_models is False):
                 break
 
     #Set functions
     def set_data(self,data):
         """Set the misc data (other than coordiantes) to the Protein object.
 
         Args:
@@ -137,15 +137,15 @@
         
         Args:
             filename (str): Name of the output file user wishes to assign.
         """
         #Annotations
         open(filename,'w').write('data_'+filename+'\n#\n')
         fh=open(filename,'a')
-        if(self.__Data != None):
+        if(self.__Data is not None):
             
             #To check what was the input format so that annotation can be written accordingly (currently only supports PDB an mmCIF) | if first line has '#' or '_', it is assumed to be mmCIF file; PDB otherwise.
             input_ftype = None
             first_characters_of_annotations = [i[0] for i in self.__Data if i != '']
             if('#' in first_characters_of_annotations and '_' in first_characters_of_annotations):
                 input_ftype = 'cif'
             else:
```

### Comparing `py-packman-1.4.7/packman/molecule/residue.py` & `py-packman-1.4.8/packman/molecule/residue.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/tests/anm/test_anm.py` & `py-packman-1.4.8/packman/tests/anm/test_anm.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/tests/data/1prw.pdb` & `py-packman-1.4.8/packman/tests/data/1prw.pdb`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/tests/data/4hla.cif` & `py-packman-1.4.8/packman/tests/data/4hla.cif`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/tests/entropy/test_entropy.py` & `py-packman-1.4.8/packman/tests/entropy/test_entropy.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/tests/molecule/test_molecule.py` & `py-packman-1.4.8/packman/tests/molecule/test_molecule.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/packman/utilities/utilities.py` & `py-packman-1.4.8/packman/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/py_packman.egg-info/PKG-INFO` & `py-packman-1.4.8/py_packman.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-packman
-Version: 1.4.7
+Version: 1.4.8
 Summary: A software package for molecular PACKing and Motion ANalysis (PACKMAN)
 Home-page: https://github.com/Pranavkhade/PACKMAN
 Author: Pranav Khade
 Author-email: pranavk@iastate.edu
 License: MIT
 Keywords: protein,dynamics,protein packing,protein domain,protein hinge
 Classifier: Intended Audience :: Education
```

### Comparing `py-packman-1.4.7/py_packman.egg-info/SOURCES.txt` & `py-packman-1.4.8/py_packman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-packman-1.4.7/setup.py` & `py-packman-1.4.8/setup.py`

 * *Files identical despite different names*

