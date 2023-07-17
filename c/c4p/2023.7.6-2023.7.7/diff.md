# Comparing `tmp/c4p-2023.7.6.tar.gz` & `tmp/c4p-2023.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c4p-2023.7.6.tar", last modified: Thu Jul  6 12:20:11 2023, max compression
+gzip compressed data, was "c4p-2023.7.7.tar", last modified: Fri Jul  7 20:01:29 2023, max compression
```

## Comparing `c4p-2023.7.6.tar` & `c4p-2023.7.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.362035 c4p-2023.7.6/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.6/LICENSE
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       27 2023-07-02 05:18:20.000000 c4p-2023.7.6/MANIFEST.in
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-06 12:20:11.361341 c4p-2023.7.6/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.6/README.md
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.077462 c4p-2023.7.6/c4p/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.6/c4p/__init__.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1301 2023-07-06 11:39:15.000000 c4p-2023.7.6/c4p/case.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3790 2023-07-06 12:17:20.000000 c4p-2023.7.6/c4p/mapping.py
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7954 2023-07-05 20:44:40.000000 c4p-2023.7.6/c4p/rof.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.069399 c4p-2023.7.6/c4p/src/
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.177185 c4p-2023.7.6/c4p/src/cime_mapping/
--rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    12240 2023-07-06 11:09:27.000000 c4p-2023.7.6/c4p/src/cime_mapping/create_ESMF_map.sh
--rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15746 2023-07-06 11:43:56.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh
--rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15728 2023-07-05 21:44:35.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.sh
--rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)   875456 2023-07-06 12:14:46.000000 c4p-2023.7.6/c4p/src/cime_mapping/gen_domain
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.222944 c4p-2023.7.6/c4p/src/rof/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      885 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/Makefile
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    11024 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/check_inf_loop.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2633 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/create-topo_0.5x0.5deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1861 2023-07-02 02:20:03.000000 c4p-2023.7.6/c4p/src/rof/create-topo_1x1deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1700 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/create-topo_2x2deg.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12241 2023-07-02 04:22:06.000000 c4p-2023.7.6/c4p/src/rof/create_ESMF_map.sh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5321 2023-07-02 02:42:46.000000 c4p-2023.7.6/c4p/src/rof/plot_rdirc.ncl
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1613 2023-07-02 02:44:45.000000 c4p-2023.7.6/c4p/src/rof/plotrdirc.csh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3122 2023-07-02 02:45:04.000000 c4p-2023.7.6/c4p/src/rof/rdirc_template.csh
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2620 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/rtm_ncdf.pro
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      543 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map.1x1.template.nml
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760296 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_0.5deg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760360 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_1deg
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.224670 c4p-2023.7.6/c4p/src/rof/runoff_map_src/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      580 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/build.cheyenne.csh
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.357580 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      725 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Macros.cheyenne
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6226 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Makefile
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14995 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1094 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/kind_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     9525 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/main.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94853 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    36063 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1242 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12114 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14025 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60912 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/smooth_mod.F90
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.359989 c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12359 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/makdep.c
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22122 2023-07-02 02:10:44.000000 c4p-2023.7.6/c4p/src/rof/topo2rdirc_sed.F90
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2252 2023-07-06 11:40:09.000000 c4p-2023.7.6/c4p/utils.py
-drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-06 12:20:11.174154 c4p-2023.7.6/c4p.egg-info/
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/PKG-INFO
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1591 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/SOURCES.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/dependency_links.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.6/c4p.egg-info/not-zip-safe
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/requires.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-06 12:20:10.000000 c4p-2023.7.6/c4p.egg-info/top_level.txt
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-06 12:20:11.362151 c4p-2023.7.6/setup.cfg
--rw-r--r--   0 fengzhu  (40317) ncar      (1000)      912 2023-07-06 12:19:16.000000 c4p-2023.7.6/setup.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.601800 c4p-2023.7.7/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1065 2023-05-22 19:27:41.000000 c4p-2023.7.7/LICENSE
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       27 2023-07-02 05:18:20.000000 c4p-2023.7.7/MANIFEST.in
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-07 20:01:29.601372 c4p-2023.7.7/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       94 2023-07-02 04:04:59.000000 c4p-2023.7.7/README.md
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.569529 c4p-2023.7.7/c4p/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      240 2023-06-01 04:08:45.000000 c4p-2023.7.7/c4p/__init__.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1791 2023-07-07 19:55:39.000000 c4p-2023.7.7/c4p/case.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3635 2023-07-07 19:58:31.000000 c4p-2023.7.7/c4p/mapping.py
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     7954 2023-07-05 20:44:40.000000 c4p-2023.7.7/c4p/rof.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.564398 c4p-2023.7.7/c4p/src/
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.575527 c4p-2023.7.7/c4p/src/cime_mapping/
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    12240 2023-07-06 11:09:27.000000 c4p-2023.7.7/c4p/src/cime_mapping/create_ESMF_map.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15746 2023-07-06 11:43:56.000000 c4p-2023.7.7/c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)    15728 2023-07-05 21:44:35.000000 c4p-2023.7.7/c4p/src/cime_mapping/gen_cesm_maps.sh
+-rwxr-xr-x   0 fengzhu  (40317) ncar      (1000)   875456 2023-07-06 12:14:46.000000 c4p-2023.7.7/c4p/src/cime_mapping/gen_domain
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.593512 c4p-2023.7.7/c4p/src/rof/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      885 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/Makefile
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    11024 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/check_inf_loop.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2633 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/create-topo_0.5x0.5deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1861 2023-07-02 02:20:03.000000 c4p-2023.7.7/c4p/src/rof/create-topo_1x1deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1700 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/create-topo_2x2deg.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12241 2023-07-02 04:22:06.000000 c4p-2023.7.7/c4p/src/rof/create_ESMF_map.sh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     5321 2023-07-02 02:42:46.000000 c4p-2023.7.7/c4p/src/rof/plot_rdirc.ncl
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1613 2023-07-02 02:44:45.000000 c4p-2023.7.7/c4p/src/rof/plotrdirc.csh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3122 2023-07-02 02:45:04.000000 c4p-2023.7.7/c4p/src/rof/rdirc_template.csh
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     2620 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/rtm_ncdf.pro
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      543 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map.1x1.template.nml
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760296 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_0.5deg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)  7760360 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_1deg
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.594051 c4p-2023.7.7/c4p/src/rof/runoff_map_src/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      580 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/build.cheyenne.csh
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.600367 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      725 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/Macros.cheyenne
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     6226 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/Makefile
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14995 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1094 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/kind_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     9525 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/main.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94853 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    94808 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    36063 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1242 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12114 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    14025 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    60912 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/smooth_mod.F90
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.600859 c4p-2023.7.7/c4p/src/rof/runoff_map_src/tools/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    12359 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/runoff_map_src/tools/makdep.c
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)    22122 2023-07-02 02:10:44.000000 c4p-2023.7.7/c4p/src/rof/topo2rdirc_sed.F90
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     3208 2023-07-07 19:28:16.000000 c4p-2023.7.7/c4p/utils.py
+drwxr-xr-x   0 fengzhu  (40317) ncar      (1000)        0 2023-07-07 20:01:29.573096 c4p-2023.7.7/c4p.egg-info/
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      541 2023-07-07 20:01:29.570982 c4p-2023.7.7/c4p.egg-info/PKG-INFO
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)     1591 2023-07-07 20:01:29.571517 c4p-2023.7.7/c4p.egg-info/SOURCES.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-07-07 20:01:29.571919 c4p-2023.7.7/c4p.egg-info/dependency_links.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        1 2023-06-01 04:07:36.000000 c4p-2023.7.7/c4p.egg-info/not-zip-safe
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       47 2023-07-07 20:01:29.572795 c4p-2023.7.7/c4p.egg-info/requires.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)        4 2023-07-07 20:01:29.573190 c4p-2023.7.7/c4p.egg-info/top_level.txt
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)       38 2023-07-07 20:01:29.601896 c4p-2023.7.7/setup.cfg
+-rw-r--r--   0 fengzhu  (40317) ncar      (1000)      912 2023-07-07 19:30:25.000000 c4p-2023.7.7/setup.py
```

### Comparing `c4p-2023.7.6/LICENSE` & `c4p-2023.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/PKG-INFO` & `c4p-2023.7.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.6/c4p/case.py` & `c4p-2023.7.7/c4p/case.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 from . import utils
 from .rof import ROF
 from .mapping import Mapping
 
 cwd = os.path.dirname(__file__)
 
 class PaleoCase:
-    def __init__(self, casename=None, work_dirpath=None, esmfbin_path=None, netcdf_lib_path=None, netcdf_inc_path=None, account=None):
+    def __init__(self, casename=None, work_dirpath=None, account=None, lmod_path=None, esmfbin_path=None, netcdf_lib_path=None, netcdf_inc_path=None):
         self.casename = casename
         self.account = account
         self.work_dirpath = work_dirpath
+        self.lmod_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/lmod/8.7.20/gcc/7.5.0/pdxb/lmod' if lmod_path is None else lmod_path
         self.esmfbin_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/esmf/8.4.2/cray-mpich/8.1.25/oneapi/2023.0.0/fslf/bin' if esmfbin_path is None else esmfbin_path
         self.netcdf_lib_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/lib' if netcdf_lib_path is None else netcdf_lib_path
         self.netcdf_inc_path = '/glade/u/apps/derecho/23.06/spack/opt/spack/netcdf/4.9.2/oneapi/2023.0.0/iijr/include' if netcdf_inc_path is None else netcdf_inc_path
         if not os.path.exists(work_dirpath):
             os.makedirs(work_dirpath, exist_ok=True)
             utils.p_success(f'>>> {work_dirpath} created')
         os.chdir(work_dirpath)
         utils.p_success(f'>>> Current directory switched to: {work_dirpath}')
 
-    def mapping(self):
-        return Mapping(**self.__dict__)
+    def mapping(self, atm_grid, ocn_grid, rof_grid, gen_cesm_maps_script=None, gen_esmf_map_script=None, gen_domain_exe=None):
+        return Mapping(
+            atm_grid=atm_grid, ocn_grid=ocn_grid, rof_grid=rof_grid,
+            gen_cesm_maps_script=gen_cesm_maps_script,
+            gen_esmf_map_script=gen_esmf_map_script,
+            gen_domain_exe=gen_domain_exe, **self.__dict__,
+        )
 
     def setup_runoff(self):
         return ROF(**self.__dict__)
```

### Comparing `c4p-2023.7.6/c4p/mapping.py` & `c4p-2023.7.7/c4p/mapping.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,31 +2,30 @@
 from datetime import date
 
 from . import utils
 
 cwd = os.path.dirname(__file__)
 
 class Mapping:
-    '''Generate mapping and domain files'''
-    def __init__(self, atm_scrip=None, ocn_scrip=None, rof_scrip=None, atm_grid_name=None, ocn_grid_name=None, rof_grid_name=None,
-                 gen_cesm_maps_script=None, gen_esmf_map_script=None, gen_domain_exe=None, job_name=None, **kwargs):
-
+    def __init__(self, atm_grid, ocn_grid, rof_grid, job_name=None,
+                 gen_cesm_maps_script=None, gen_esmf_map_script=None, gen_domain_exe=None, **kwargs):
+        '''Generate mapping and domain files
+
+        Args:
+            atm_grid (dict): grid information for atm in the format of {grid_name: path_to_scrip_file}
+            ocn_grid (dict): grid information for ocn in the format of {grid_name: path_to_scrip_file}
+            rof_grid (dict): grid information for rof in the format of {grid_name: path_to_scrip_file}
+        '''
         for k, v in kwargs.items():
             self.__dict__[k] = v
 
         self.job_name = 'mapping' if job_name is None else job_name
-
-        # a set of default scrip files and grid names for ne16_g16
-        scripgrids_dir = '/glade/p/cesmdata/inputdata/share/scripgrids'
-        self.atm_scrip = os.path.join(scripgrids_dir, 'ne16np4_scrip_171002.nc') if atm_scrip is None else atm_scrip
-        self.ocn_scrip = os.path.join(scripgrids_dir, 'gx1v6_090205.nc') if ocn_scrip is None else ocn_scrip
-        self.rof_scrip = os.path.join(scripgrids_dir, '1x1d.nc') if rof_scrip is None else rof_scrip
-        self.atm_grid_name = 'ne16np4' if atm_grid_name is None else atm_grid_name
-        self.ocn_grid_name = 'gx1v6' if ocn_grid_name is None else ocn_grid_name
-        self.rof_grid_name = 'r1_nomask' if rof_grid_name is None else rof_grid_name
+        self.atm_grid_name, self.atm_scrip  = list(atm_grid.keys())[0], list(atm_grid.values())[0]
+        self.ocn_grid_name, self.ocn_scrip  = list(ocn_grid.keys())[0], list(ocn_grid.values())[0]
+        self.rof_grid_name, self.rof_scrip  = list(rof_grid.keys())[0], list(rof_grid.values())[0]
 
         # paths for mapping and domain generation scripts
         self.gen_cesm_maps_script = os.path.join(cwd, './src/cime_mapping/gen_cesm_maps.ncpu36.sh') if gen_cesm_maps_script is None else gen_cesm_maps_script
         self.gen_esmf_map_script = os.path.join(cwd, './src/cime_mapping/create_ESMF_map.sh') if gen_esmf_map_script is None else gen_esmf_map_script
         self.gen_domain_exe = os.path.join(cwd, './src/cime_mapping/gen_domain') if gen_domain_exe is None else gen_domain_exe
 
         for k, v in self.__dict__.items():
@@ -70,8 +69,8 @@
         utils.qsub_script(
             self.gen_domain_exe,
             args=f'-m map_{self.ocn_grid_name}_TO_{self.atm_grid_name}_aave.{date_today}.nc -o {self.ocn_grid_name} -l {self.atm_grid_name}',
             name=self.job_name, account=self.account,
         )
 
     def clean(self):
-        utils.run_shell(f'rm -rf {self.job_name}.* PET*')
+        utils.run_shell(f'rm -rf {self.job_name}.* PET* pbs_*')
```

### Comparing `c4p-2023.7.6/c4p/rof.py` & `c4p-2023.7.7/c4p/rof.py`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/cime_mapping/create_ESMF_map.sh` & `c4p-2023.7.7/c4p/src/cime_mapping/create_ESMF_map.sh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh` & `c4p-2023.7.7/c4p/src/cime_mapping/gen_cesm_maps.ncpu36.sh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/cime_mapping/gen_cesm_maps.sh` & `c4p-2023.7.7/c4p/src/cime_mapping/gen_cesm_maps.sh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/cime_mapping/gen_domain` & `c4p-2023.7.7/c4p/src/cime_mapping/gen_domain`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/Makefile` & `c4p-2023.7.7/c4p/src/rof/Makefile`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/check_inf_loop.F90` & `c4p-2023.7.7/c4p/src/rof/check_inf_loop.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/create-topo_0.5x0.5deg.ncl` & `c4p-2023.7.7/c4p/src/rof/create-topo_0.5x0.5deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/create-topo_1x1deg.ncl` & `c4p-2023.7.7/c4p/src/rof/create-topo_1x1deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/create-topo_2x2deg.ncl` & `c4p-2023.7.7/c4p/src/rof/create-topo_2x2deg.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/create_ESMF_map.sh` & `c4p-2023.7.7/c4p/src/rof/create_ESMF_map.sh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/plot_rdirc.ncl` & `c4p-2023.7.7/c4p/src/rof/plot_rdirc.ncl`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/plotrdirc.csh` & `c4p-2023.7.7/c4p/src/rof/plotrdirc.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/rdirc_template.csh` & `c4p-2023.7.7/c4p/src/rof/rdirc_template.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/rtm_ncdf.pro` & `c4p-2023.7.7/c4p/src/rof/rtm_ncdf.pro`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map.1x1.template.nml` & `c4p-2023.7.7/c4p/src/rof/runoff_map.1x1.template.nml`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_0.5deg` & `c4p-2023.7.7/c4p/src/rof/runoff_map_0.5deg`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_1deg` & `c4p-2023.7.7/c4p/src/rof/runoff_map_1deg`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/build.cheyenne.csh` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/build.cheyenne.csh`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Macros.cheyenne` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/Macros.cheyenne`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/Makefile` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/Makefile`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/fixroff_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/kind_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/kind_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/main.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/main.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod_0.5deg.F90.save`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/map_mod_1deg.F90.save`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/mapsort_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_kind_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_sys_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/shr_timer_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/src/smooth_mod.F90` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/src/smooth_mod.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/runoff_map_src/tools/makdep.c` & `c4p-2023.7.7/c4p/src/rof/runoff_map_src/tools/makdep.c`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/src/rof/topo2rdirc_sed.F90` & `c4p-2023.7.7/c4p/src/rof/topo2rdirc_sed.F90`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/c4p/utils.py` & `c4p-2023.7.7/c4p/utils.py`

 * *Files 21% similar despite different names*

```diff
@@ -68,21 +68,52 @@
     if args is None:
         cmd = fpath
     else:
         cmd = f'{fpath} {args}'
 
     run_shell(cmd, timeout=timeout)
 
-def qsub_script(fpath, args=None, name='test', queue='main', select=1, ncpus=36, mpiprocs=36, mem=64, walltime='06:00:00', account=None):
+def make_pbs(fpath, args=None, name='test', queue='main', select=1, ncpus=36, mpiprocs=36, mem=64, walltime='06:00:00', account=None):
+    if account is None:
+        raise ValueError('account must be specified')
+
+    if args is None:
+        cmd = fpath
+    else:
+        cmd = f'{fpath} {args}'
+
+    fname = f'pbs_{name}.zsh'
+    with open(fname, 'w') as f:
+        f.write(f'''#!/bin/zsh
+#PBS -N {name}
+#PBS -q {queue}
+#PBS -l select={select}:ncpus={ncpus}:mpiprocs={mpiprocs}:mem={mem}GB
+#PBS -l walltime={walltime}
+#PBS -A {account}
+
+{cmd}
+                ''')
+
+    p_success(f'>>> {fname} created')
+
+def qsub_script(fpath, args=None, name='test', queue='main', select=1, ncpus=36, mpiprocs=36, mem=64, walltime='06:00:00', account=None, create_pbs=True, **env_vars):
+    env_str = ''
+    for k, v in env_vars.items():
+        env_str += f'{k}="{v},"'
+        
     if account is None:
         raise ValueError('account must be specified')
 
     if args is None:
         cmd = fpath
     else:
         cmd = f'{fpath} {args}'
 
     l1 = f'select={select}:ncpus={ncpus}:mpiprocs={mpiprocs}:mem={mem}GB'
     l2 = f'walltime={walltime}'
-    
-    run_shell(f'echo -e {cmd} | qsub -N {name} -q {queue} -l {l1} -l {l2} -A {account}')
+
+    if create_pbs:
+        make_pbs(fpath, args=args, name=name, queue=queue, select=select, ncpus=ncpus, mpiprocs=mpiprocs, mem=mem, walltime=walltime, account=account)
+        run_shell(f'qsub pbs_{name}.zsh')
+    else:
+        run_shell(f'qsub -N {name} -q {queue} -l {l1} -l {l2} -A {account} -v {env_str} -- {cmd}')
```

### Comparing `c4p-2023.7.6/c4p.egg-info/PKG-INFO` & `c4p-2023.7.7/c4p.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c4p
-Version: 2023.7.6
+Version: 2023.7.7
 Summary: c4p: CESM for Paleo
 Home-page: https://github.com/fzhu2e/cesm4paleo
 Author: Feng Zhu, Jiang Zhu
 Author-email: fengzhu@ucar.edu, jiangzhu@ucar.edu
 License: MIT
 Keywords: CESM,paleoclimate
 Classifier: Natural Language :: English
```

### Comparing `c4p-2023.7.6/c4p.egg-info/SOURCES.txt` & `c4p-2023.7.7/c4p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `c4p-2023.7.6/setup.py` & `c4p-2023.7.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setup(
     name='c4p',  # required
-    version='2023.7.6',
+    version='2023.7.7',
     description='c4p: CESM for Paleo',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Feng Zhu, Jiang Zhu',
     author_email='fengzhu@ucar.edu, jiangzhu@ucar.edu',
     url='https://github.com/fzhu2e/cesm4paleo',
     packages=find_packages(),
```

