# Comparing `tmp/bsplines2d-0.0.4.tar.gz` & `tmp/bsplines2d-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bsplines2d-0.0.4.tar", last modified: Wed May 24 16:39:12 2023, max compression
+gzip compressed data, was "bsplines2d-0.0.5.tar", last modified: Mon Jul 17 20:52:36 2023, max compression
```

## Comparing `bsplines2d-0.0.4.tar` & `bsplines2d-0.0.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/_updateversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.571929 bsplines2d-0.0.4/bsplines2d/
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_outline.py
--rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_rect_cropping.py
--rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class01_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    31494 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_BSplines2D.py
--rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_polar.py
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_rect.py
--rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_bsplines_tri.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_contours.py
--rw-r--r--   0 runner    (1001) docker     (123)    54051 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_interpolate_all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    28950 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_Bins.py
--rw-r--r--   0 runner    (1001) docker     (123)     6344 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class03_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_class11_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_generic_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_generic_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_utils_bsplines.py
--rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/_utils_bsplines_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/bsplines2d/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_01_Mesh2D.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_02_BSplines2D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/bsplines2d/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_Poly.npz
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_trimesh.npz
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_data/trimesh_quad.npz
--rw-r--r--   0 runner    (1001) docker     (123)    26411 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/bsplines2d/tests/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:12.571929 bsplines2d-0.0.4/bsplines2d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-24 16:39:12.000000 bsplines2d-0.0.4/bsplines2d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:39:12.575929 bsplines2d-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-24 16:38:56.000000 bsplines2d-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:36.938105 bsplines2d-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-17 20:52:36.938105 bsplines2d-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/_updateversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:36.934105 bsplines2d-0.0.5/bsplines2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_checks_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12668 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11955 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_outline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7774 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_rect_cropping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16219 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22224 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class01_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31728 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_BSplines2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11187 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_operators_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14515 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_operators_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21560 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_polar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_rect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17683 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_bsplines_tri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25156 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27590 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_contours.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54560 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7348 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_interpolate_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9783 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9982 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_plot_as_profile2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class02_plot_as_profile2d_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class03_Bins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class03_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class03_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21736 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_class11_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_generic_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10430 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_generic_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11459 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_utils_bsplines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22955 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/_utils_bsplines_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:36.938105 bsplines2d-0.0.5/bsplines2d/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_01_Mesh2D.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_02_BSplines2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:36.938105 bsplines2d-0.0.5/bsplines2d/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_data/WEST_Poly.npz
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_data/WEST_trimesh.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_data/trimesh_quad.npz
+-rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/bsplines2d/tests/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:52:36.934105 bsplines2d-0.0.5/bsplines2d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-17 20:52:36.000000 bsplines2d-0.0.5/bsplines2d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:52:36.938105 bsplines2d-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-07-17 20:52:11.000000 bsplines2d-0.0.5/setup.py
```

### Comparing `bsplines2d-0.0.4/LICENSE` & `bsplines2d-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/PKG-INFO` & `bsplines2d-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.4/_updateversion.py` & `bsplines2d-0.0.5/_updateversion.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_Mesh2D.py` & `bsplines2d-0.0.5/bsplines2d/_class01_Mesh2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_checks_1d.py` & `bsplines2d-0.0.5/bsplines2d/_class01_checks_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_polar.py` & `bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_rect.py` & `bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_checks_2d_tri.py` & `bsplines2d-0.0.5/bsplines2d/_class01_checks_2d_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_outline.py` & `bsplines2d-0.0.5/bsplines2d/_class01_outline.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_plot.py` & `bsplines2d-0.0.5/bsplines2d/_class01_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_rect_cropping.py` & `bsplines2d-0.0.5/bsplines2d/_class01_rect_cropping.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_sample.py` & `bsplines2d-0.0.5/bsplines2d/_class01_sample.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class01_select.py` & `bsplines2d-0.0.5/bsplines2d/_class01_select.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_BSplines2D.py` & `bsplines2d-0.0.5/bsplines2d/_class02_BSplines2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,14 +362,15 @@
         res=None,
         mode=None,
         submesh=None,
         # domain limitation
         domain=None,
         # common ref
         ref_com=None,
+        ref_vector_strategy=None,
         # bsplines-specific
         details=None,
         indbs_tf=None,
         # rect-specific
         crop=None,
         # parameters
         deg=None,
@@ -377,14 +378,15 @@
         val_out=None,
         log_log=None,
         nan0=None,
         # store vs return
         returnas=None,
         return_params=None,
         store=None,
+        store_keys=None,
         inplace=None,
         # debug
         debug=None,
         # # bsplines
         # res=None,
         # imshow=None,
     ):
@@ -402,28 +404,30 @@
             res=res,
             mode=mode,
             submesh=submesh,
             # domain limitation
             domain=domain,
             # common ref
             ref_com=ref_com,
+            ref_vector_strategy=ref_vector_strategy,
             # bsplines-specific
             details=details,
             indbs_tf=indbs_tf,
             # rect-specific
             crop=crop,
             # parameters
             deg=deg,
             deriv=deriv,
             val_out=val_out,
             log_log=log_log,
             # store vs return
             returnas=returnas,
             return_params=return_params,
             store=store,
+            store_keys=store_keys,
             inplace=inplace,
             # debug
             debug=debug,
         )
 
     def interpolate_all_bsplines(
         self,
@@ -935,14 +939,15 @@
         dlevels=None,
         ref_com=None,
         # details
         plot_details=None,
         # ref vectors
         dref_vectorZ=None,
         dref_vectorU=None,
+        ref_vector_strategy=None,
         # interpolation
         val_out=None,
         nan0=None,
         # plot options
         vmin=None,
         vmax=None,
         cmap=None,
@@ -966,14 +971,15 @@
             dlevels=dlevels,
             ref_com=ref_com,
             # details
             plot_details=plot_details,
             # ref vectors
             dref_vectorZ=dref_vectorZ,
             dref_vectorU=dref_vectorU,
+            ref_vector_strategy=ref_vector_strategy,
             # interpolation
             val_out=val_out,
             nan0=nan0,
             # plot options
             vmin=vmin,
             vmax=vmax,
             cmap=cmap,
```

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_1d.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_1d.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_operators_1d.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_operators_rect.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_operators_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_polar.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_polar.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_rect.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_rect.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_bsplines_tri.py` & `bsplines2d-0.0.5/bsplines2d/_class02_bsplines_tri.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_checks.py` & `bsplines2d-0.0.5/bsplines2d/_class02_checks.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_compute.py` & `bsplines2d-0.0.5/bsplines2d/_class02_compute.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_contours.py` & `bsplines2d-0.0.5/bsplines2d/_class02_contours.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_interpolate.py` & `bsplines2d-0.0.5/bsplines2d/_class02_interpolate.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     res=None,
     mode=None,
     submesh=None,
     # domain limitation
     domain=None,
     # common ref
     ref_com=None,
+    ref_vector_strategy=None,
     # bsplines-specific
     details=None,
     indbs_tf=None,
     # rect-specific
     crop=None,
     # parameters
     deg=None,
@@ -48,14 +49,15 @@
     val_out=None,
     log_log=None,
     nan0=None,
     # store vs return
     returnas=None,
     return_params=None,
     store=None,
+    store_keys=None,
     inplace=None,
     # debug or unit tests
     debug=None,
 ):
     """ Interpolate at desired points on desired data
 
     Interpolate quantities (keys) on coordinates (ref_keys)
@@ -252,14 +254,15 @@
         x1=x1,
         # useful for shapes
         daxis=daxis,
         dunits=dunits,
         domain=domain,
         # common ref
         ref_com=ref_com,
+        # ref_vector_strategy=ref_vector_strategy,
         # parameters
         grid=grid,
         deg=None,
         deriv=deriv,
         log_log=None,
         nan0=nan0,
         # return vs store
@@ -330,24 +333,38 @@
     if details is True:
         coll.remove_data(ktemp)
 
     # ------------------------------
     # adjust data and ref if xunique
 
     if xunique:
+        # try:
         ds._class1_interpolate._xunique(dout)
-
+        # except Exception as err:
+        #     msg = (
+        #         err.args[0]
+        #         + "\n\n"
+        #         f"keys = {keys}\n"
+        #         f"ref_key = {ref_key}\n"
+        #         f"x0 = {x0}\n"
+        #         f"x1 = {x1}\n"
+        #     )
+        #     err.args = (msg,)
+        #     raise err
+            
+            
     # ----------
     # store
 
     if store is True:
         coll2 = ds._class1_interpolate._store(
             coll=coll,
             dout=dout,
             inplace=inplace,
+            store_keys=store_keys,
         )
 
     # -------
     # return
 
     if returnas is object:
         return coll2
```

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_interpolate_all.py` & `bsplines2d-0.0.5/bsplines2d/_class02_interpolate_all.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_operators.py` & `bsplines2d-0.0.5/bsplines2d/_class02_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_plot.py` & `bsplines2d-0.0.5/bsplines2d/_class02_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d.py` & `bsplines2d-0.0.5/bsplines2d/_class02_plot_as_profile2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     dlevels=None,
     ref_com=None,
     # details
     plot_details=None,
     # ref vectors
     dref_vectorZ=None,
     dref_vectorU=None,
+    ref_vector_strategy=None,
     # interpolation
     val_out=None,
     nan0=None,
     # figure
     vmin=None,
     vmax=None,
     cmap=None,
@@ -133,14 +134,15 @@
                 coll=coll,
                 collax=collax,
                 key=k0,
                 keym=v0['keym'],
                 keybs=v0['keybs'],
                 # ref vector
                 dref_vector=dref_vectorZ,
+                ref_vector_strategy=ref_vector_strategy,
                 # details
                 plot_details=plot_details,
                 # plotting
                 vmin=vmin,
                 vmax=vmax,
                 cmap=cmap,
                 color_dict=color_dict[k0],
@@ -735,14 +737,15 @@
     coll=None,
     collax=None,
     key=None,
     keym=None,
     keybs=None,
     # ref vetcor
     dref_vector=None,
+    ref_vector_strategy=None,
     # plot_details
     plot_details=None,
     # figure
     vmin=None,
     vmax=None,
     cmap=None,
     color_dict=None,
@@ -798,18 +801,27 @@
     kradius, lkradial, lkdet, reft = _plot_profile2d_polar_add_radial(
         coll=coll,
         key=key,
         keym=keym,
         keybs=keybs,
         collax=collax,
         dref_vector=dref_vector,
+        ref_vector_strategy=ref_vector_strategy,
         plot_details=plot_details,
     )
 
-    assert (reft is not None) == ('Z' in dgroup.keys())
+    if (reft is not None) != ('Z' in dgroup.keys()):
+        msg = (
+            "(reft is not None) != ('Z' in dgroup.keys()):\n"
+            f"reft = {reft}\n"
+            f"dgroup.keys() = {dgroup.keys()}\n"
+            f"dref_vector = {dref_vector}"
+        )
+        raise Exception(msg)
+    
     if reft is not None and reft not in dgroup['Z']['ref']:
         dgroup['Z']['ref'].append(reft)
         dgroup['Z']['data'].append('index')
 
     # ------------------
     # add radial profile
 
@@ -893,14 +905,15 @@
     coll=None,
     key=None,
     keym=None,
     keybs=None,
     collax=None,
     # ref_vector
     dref_vector=None,
+    ref_vector_strategy=None,
     # details
     plot_details=None,
 ):
 
     # ----------
     # check
 
@@ -954,14 +967,15 @@
     else:
         refc = None
 
     # find reft
     reft, keyt, _, dind = coll.get_ref_vector_common(
         keys=[key, kr2d],
         ref=refc,
+        strategy=ref_vector_strategy,
         **dref_vector,
     )[1:]
 
     # radial total profile
     # radial, t_radial, _ = coll.interpolate(
     dout = coll.interpolate(
         keys=key,
```

### Comparing `bsplines2d-0.0.4/bsplines2d/_class02_plot_as_profile2d_compare.py` & `bsplines2d-0.0.5/bsplines2d/_class02_plot_as_profile2d_compare.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_class11_plot.py` & `bsplines2d-0.0.5/bsplines2d/_class11_plot.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_generic_check.py` & `bsplines2d-0.0.5/bsplines2d/_generic_check.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_generic_mesh.py` & `bsplines2d-0.0.5/bsplines2d/_generic_mesh.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_utils_bsplines.py` & `bsplines2d-0.0.5/bsplines2d/_utils_bsplines.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/_utils_bsplines_operators.py` & `bsplines2d-0.0.5/bsplines2d/_utils_bsplines_operators.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_01_Mesh2D.py` & `bsplines2d-0.0.5/bsplines2d/tests/test_01_Mesh2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_02_BSplines2D.py` & `bsplines2d-0.0.5/bsplines2d/tests/test_02_BSplines2D.py`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_Poly.npz` & `bsplines2d-0.0.5/bsplines2d/tests/test_data/WEST_Poly.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_data/WEST_trimesh.npz` & `bsplines2d-0.0.5/bsplines2d/tests/test_data/WEST_trimesh.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_data/trimesh_quad.npz` & `bsplines2d-0.0.5/bsplines2d/tests/test_data/trimesh_quad.npz`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/bsplines2d/tests/test_input.py` & `bsplines2d-0.0.5/bsplines2d/tests/test_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -782,16 +782,14 @@
                 + "\n".join(lstr)
             )
             raise Exception(msg)
 
 
 def _bin_bs(bs, nd=None, kind=None):
     dkd = _get_data(bs, nd=nd, kind=kind, maxref=3)
-
-
     wbs = bs._which_bsplines
     for ii, (kd, vd) in enumerate(dkd.items()):
 
 
         if len(bs.ddata[kd]['ref']) > 3:
             continue
 
@@ -813,29 +811,30 @@
 
         dd = np.abs(np.mean(np.diff(vect)))
         DD = vect[-1] - vect[0]
         nbins = int(DD/dd)
         bins = np.linspace(vect[0] - 0.1*DD, vect[0]+0.5*DD, nbins)
 
         dout = bs.binning(
-            keys=kd,
-            ref_key=ref_key,
-            bins=bins,
+            data=kd,
+            bin_data0=ref_key,
+            bins0=bins,
             # store vs return
             store=False,
             returnas=True,
         )
+        kd = list(dout.keys())[0]
 
         shape = list(bs.ddata[kd]['shape'])
-        shape[ax] = nbins - 1
+        shape[ax] = nbins
         shape = tuple(shape)
         if dout[kd]['data'].shape != shape:
             shd = bs.ddata[kd]['data'].shape
             msg = (
-                "Binnign of data '{kd}' along ref 'ref_key' has wrong shape:\n"
+                "Binning of data '{kd}' along ref 'ref_key' has wrong shape:\n"
                 f"\t- ddata['{kd}']['data'].shape = {shd}\n"
                 f"\t- dout['{kd}']['data'].shape = {dout[kd]['data'].shape}\n"
                 f"\t- expected shape = {shape}\n"
             )
             raise Exception(msg)
```

### Comparing `bsplines2d-0.0.4/bsplines2d.egg-info/PKG-INFO` & `bsplines2d-0.0.5/bsplines2d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bsplines2d
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library for generic multidimensional bsplines on various meshes, using datastock
 Home-page: https://github.com/ToFuProject/bsplines2d
 Author: Didier VEZINET
 Author-email: didier.vezinet@gmail.com
 License: MIT
 Keywords: bsplines data analysis modelling mesh plot
 Classifier: Development Status :: 4 - Beta
```

### Comparing `bsplines2d-0.0.4/bsplines2d.egg-info/SOURCES.txt` & `bsplines2d-0.0.5/bsplines2d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bsplines2d-0.0.4/setup.py` & `bsplines2d-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     # your project is installed. For an analysis of "install_requires" vs pip's
     # requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
     install_requires=[
         "numpy",
         "scipy",
         "matplotlib",
-        "datastock>=0.0.26",
+        "datastock>=0.0.30",
     ],
     python_requires=">=3.6",
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). You can install these using the following syntax,
     # for example:
     # $ pip install -e .[dev,test]
```

