# Comparing `tmp/pyg2p-3.2.4.tar.gz` & `tmp/pyg2p-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyg2p-3.2.4.tar", last modified: Fri May 19 09:37:07 2023, max compression
+gzip compressed data, was "dist/pyg2p-3.2.5.tar", last modified: Mon Jul 17 09:18:32 2023, max compression
```

## Comparing `pyg2p-3.2.4.tar` & `pyg2p-3.2.5.tar`

### file list

```diff
@@ -1,167 +1,167 @@
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-02-15 12:18:09.000000 pyg2p-3.2.4/LICENSE
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-02-20 17:30:36.000000 pyg2p-3.2.4/MANIFEST.in
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    47858 2023-05-19 09:37:07.000000 pyg2p-3.2.4/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    46863 2023-04-26 09:56:42.000000 pyg2p-3.2.4/README.md
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/bin/
--rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-02-15 12:18:09.000000 pyg2p-3.2.4/bin/pyg2p
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/configuration/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/geopotentials.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/configuration/global/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/ftp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3225 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/geopotentials.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/global_conf.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    41874 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8250 2023-05-19 09:35:08.000000 pyg2p-3.2.4/configuration/global/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/global/test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/intertables.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-02-15 12:18:09.000000 pyg2p-3.2.4/configuration/parameters.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      214 2023-02-15 12:18:09.000000 pyg2p-3.2.4/requirements.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-05-19 09:37:07.000000 pyg2p-3.2.4/setup.cfg
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7115 2023-05-19 09:35:08.000000 pyg2p-3.2.4/setup.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-05-19 09:35:08.000000 pyg2p-3.2.4/src/pyg2p/VERSION
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     7644 2023-05-17 14:15:45.000000 pyg2p-3.2.4/src/pyg2p/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/exceptions.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    15678 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/config.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    22879 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/context.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/controller.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    19605 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/grib_interpolation_lib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/latlong.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    50993 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    14068 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/manipulation/correction.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/readers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    11805 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/readers/grib.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     3116 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/main/readers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/main/writers/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/writers/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-04-26 09:56:42.000000 pyg2p-3.2.4/src/pyg2p/main/writers/netcdf.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2012 2023-05-19 09:35:08.000000 pyg2p-3.2.4/src/pyg2p/main/writers/pcr.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/util/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/files.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/generics.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/numeric.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/__init__.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/profiling/profilehooks.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p/util/strings.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)    47858 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/PKG-INFO
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4419 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/SOURCES.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/dependency_links.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      132 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/requires.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-05-19 09:37:07.000000 pyg2p-3.2.4/src/pyg2p.egg-info/top_level.txt
--rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-02-20 16:19:14.000000 pyg2p-3.2.4/src/pyg2p.egg-info/zip-safe
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-02-15 12:18:09.000000 pyg2p-3.2.4/src/pyg2p.py
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/templates/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_cp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_lsp.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_rg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_rn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_ta.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_td.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_wu.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/AFFS_wv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_15d.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_15d_glob.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_inv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_nn.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_agg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_december.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/EUE_RainAnim_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/UKMO_t24_LA_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cin.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24_newmaps.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/cosmo_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_2.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_3.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_efas.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_gmi.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24_2nd.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwd_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/dwdl_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/efas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_e06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_e06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eud_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_e24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_e24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_g.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_noagg.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_15days_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_r24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/eue_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_sro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_sro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_ssro.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/glofas_ssro_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_global.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_global_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/octahedral_test_scipy_invdist.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/rn_false_mv.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_r06_scipy_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_rotated.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_scipy.json
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.4/templates/tigge_lam_t24_scipy_rotated.json
-drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-05-19 09:37:07.000000 pyg2p-3.2.4/tests/
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     4666 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_aggregator.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     8785 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_api.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      938 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_conversion.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2786 2023-04-26 09:56:42.000000 pyg2p-3.2.4/tests/test_correction.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     6597 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_interpolation.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     2246 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_oracle_data.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)     1997 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_readers.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)      669 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_strings.py
--rw-rw-r--   0 carlo     (1000) carlo     (1000)       76 2023-02-15 12:18:09.000000 pyg2p-3.2.4/tests/test_writers.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13760 2023-02-15 12:18:09.000000 pyg2p-3.2.5/LICENSE
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       84 2023-02-20 17:30:36.000000 pyg2p-3.2.5/MANIFEST.in
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    48250 2023-07-17 09:18:32.000000 pyg2p-3.2.5/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    47255 2023-07-17 09:08:12.000000 pyg2p-3.2.5/README.md
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/bin/
+-rwxrwxr-x   0 carlo     (1000) carlo     (1000)      191 2023-02-15 12:18:09.000000 pyg2p-3.2.5/bin/pyg2p
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/configuration/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/geopotentials.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/configuration/global/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      100 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/global/ftp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3225 2023-05-19 09:35:08.000000 pyg2p-3.2.5/configuration/global/geopotentials.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      149 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/global/global_conf.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    42231 2023-07-17 09:08:12.000000 pyg2p-3.2.5/configuration/global/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8250 2023-05-19 09:35:08.000000 pyg2p-3.2.5/configuration/global/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      155 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/global/test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        4 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/intertables.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        3 2023-02-15 12:18:09.000000 pyg2p-3.2.5/configuration/parameters.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      201 2023-07-17 09:08:12.000000 pyg2p-3.2.5/requirements.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       38 2023-07-17 09:18:32.000000 pyg2p-3.2.5/setup.cfg
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7115 2023-05-19 09:35:08.000000 pyg2p-3.2.5/setup.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        5 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/VERSION
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7644 2023-05-17 14:15:45.000000 pyg2p-3.2.5/src/pyg2p/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4261 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/exceptions.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/main/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2334 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    15783 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    14257 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/config.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    23102 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/context.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8033 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/controller.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/main/interpolation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    21232 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/interpolation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11019 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/interpolation/grib_interpolation_lib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2020 2023-04-26 09:56:42.000000 pyg2p-3.2.5/src/pyg2p/main/interpolation/latlong.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    62427 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/interpolation/scipy_interpolation_lib.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/main/manipulation/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/manipulation/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    13758 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/manipulation/aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1752 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/manipulation/conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4907 2023-04-26 09:56:42.000000 pyg2p-3.2.5/src/pyg2p/main/manipulation/correction.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/main/readers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       61 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/readers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    11805 2023-04-26 09:56:42.000000 pyg2p-3.2.5/src/pyg2p/main/readers/grib.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     3011 2023-07-17 09:08:12.000000 pyg2p-3.2.5/src/pyg2p/main/readers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1386 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/main/readers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/main/writers/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     6837 2023-04-26 09:56:42.000000 pyg2p-3.2.5/src/pyg2p/main/writers/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8513 2023-04-26 09:56:42.000000 pyg2p-3.2.5/src/pyg2p/main/writers/netcdf.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2012 2023-05-19 09:35:08.000000 pyg2p-3.2.5/src/pyg2p/main/writers/pcr.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/util/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2978 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/files.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      593 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/generics.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      940 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/numeric.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p/util/profiling/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        0 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/profiling/__init__.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    24815 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/profiling/profilehooks.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      970 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p/util/strings.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)    48250 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/PKG-INFO
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4419 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/SOURCES.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/dependency_links.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      162 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/requires.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        6 2023-07-17 09:18:32.000000 pyg2p-3.2.5/src/pyg2p.egg-info/top_level.txt
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)        1 2023-02-20 16:19:14.000000 pyg2p-3.2.5/src/pyg2p.egg-info/zip-safe
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      112 2023-02-15 12:18:09.000000 pyg2p-3.2.5/src/pyg2p.py
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/templates/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      655 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_cp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      658 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_lsp.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_rg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_rn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      915 2023-07-17 06:26:27.000000 pyg2p-3.2.5/templates/AFFS_ta.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_td.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_wu.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      610 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/AFFS_wv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_15d.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_15d_glob.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_CV.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      527 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_CV_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      520 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy_inv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      522 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy_nn.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      650 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_agg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      592 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_december.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      570 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      565 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/EUE_RainAnim_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/UKMO_t24_LA.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/UKMO_t24_LA_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      854 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/UKMO_t24_LA_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      536 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cin.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      665 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      739 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_e06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      617 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      677 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      751 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_r06_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      629 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      809 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      885 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_t24_newmaps.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      743 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/cosmo_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      694 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_e06_2.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_e06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      771 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_e06_3.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      646 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      737 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      642 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_r06_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      715 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_r06_efas.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      683 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_r06_gmi.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      614 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      863 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      881 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_t24_2nd.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      797 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwd_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      740 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/dwdl_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      615 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/efas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      709 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_e06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_e06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      710 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      705 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      821 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eud_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      654 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_e24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      649 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_e24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      656 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24_15days.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      747 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24_15days_g.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24_15days_noagg.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      742 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24_15days_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      651 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_r24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      773 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      816 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/eue_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      704 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/glofas_sro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      699 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/glofas_sro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/glofas_ssro.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      702 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/glofas_ssro_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      807 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      817 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      675 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      684 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      824 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      812 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_scipy_global.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      670 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_scipy_global_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      679 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/octahedral_test_scipy_invdist.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      631 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/rn_false_mv.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      647 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_r06.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      713 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_r06_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      648 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_r06_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      714 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_r06_scipy_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      789 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_t24.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      855 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_t24_rotated.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      790 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_t24_scipy.json
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      708 2023-02-15 12:18:09.000000 pyg2p-3.2.5/templates/tigge_lam_t24_scipy_rotated.json
+drwxrwxr-x   0 carlo     (1000) carlo     (1000)        0 2023-07-17 09:18:32.000000 pyg2p-3.2.5/tests/
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     4666 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_aggregator.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     8785 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_api.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      938 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_conversion.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2786 2023-04-26 09:56:42.000000 pyg2p-3.2.5/tests/test_correction.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     7610 2023-07-17 09:08:12.000000 pyg2p-3.2.5/tests/test_interpolation.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     2246 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_oracle_data.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)     1997 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_readers.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)      669 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_strings.py
+-rw-rw-r--   0 carlo     (1000) carlo     (1000)       76 2023-02-15 12:18:09.000000 pyg2p-3.2.5/tests/test_writers.py
```

### Comparing `pyg2p-3.2.4/LICENSE` & `pyg2p-3.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/PKG-INFO` & `pyg2p-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.4
+Version: 3.2.5
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -48,15 +48,15 @@
   ```
 
 >IMPORTANT: Before to launch setup, you need the following steps:
 
 >Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes gdal
+$ conda install -c conda-forge gdal eccodes
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -431,15 +431,15 @@
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>type</b></td><td>Type of aggregation (it was Manipulation in
 grib2pcraster). It can be average or accumulation.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to True and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
+        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to true and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td>forceZeroArray</td><td>Optional. In case of “accumulation”, and only
 then, if this attribute is set to”y” (or any value different from “false”, “False”, “FALSE”, “no”,
 “NO”, “No”, “0”), the program will use a zero array as message at step 0 to compute the first
 map, even if the GRIB file has a step 0 message.</td>
         </tr>
@@ -690,14 +690,28 @@
 
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
+#### ADW
+It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
+If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "adw",
+  "@adw_broadcasting": false}
+}
+```
+
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
@@ -755,15 +769,15 @@
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
 {
 "Aggregation": {
   "@type": "average",
-  "@halfweights": False}
+  "@halfweights": false}
 }
 ```
 
 To better understand what these two types of aggregations do, the DEBUG output of execution is presented later in same paragraph.
 
 ### Average
 Temperatures are often extracted as averages on 24 hours or 6 hours. Here's a typical execution configuration and the output of interest:
@@ -773,15 +787,15 @@
 ```json
 {
 "Execution": {
 "@name": "cosmo_T24",
 "Aggregation": {
 "@step": 24,
 "@type": "average",
-"@halfweights": False
+"@halfweights": false
 },
 "OutMaps": {
 "@cloneMap": "/dataset/maps/europe/dem.map",
 "@ext": 4,
 "@fmap": 1,
 "@namePrefix": "T24",
 "@unitTime": 24,
@@ -819,33 +833,33 @@
 
 This is needed because we performed 24 hours average over 6 hourly steps.
 
 **Details about average parameters:**
 
 The to evaluate the average, the following steps are executed:
 
-- when "halfweights" is False, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
+- when "halfweights" is false, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 48 every 6 hours: 0,6,12,18,24,30,....
 
   Day 1: Aggregation starts from 24-24+1=1, so it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 six times. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24+1=25...
 
-- when "halfweights" is True, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
+- when "halfweights" is true, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 72 every 6 hours: 0,6,12,18,24,30,36,....
 
   Day 1: Aggregation starts from 24-24=0, and will consider the step 0 value multiplied but 3, that is half of the number of steps between two step keys in the grib file. Then it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 again multiplied by 3. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24=24: the step 24 will have a weight of 3, while steps 30,36 and 42 will be counted 6 times, and finally the step 48 will have a weight of 3. 
 
-- if start_step is zero or is not specified, the aggregation will start from 1
+- if start_step is zero or is not specified, the aggregation will start from 0
 
 ### Accumulation
 For precipitation values, accumulation over 6 or 24 hours is often performed. Here's an example of configuration and execution output in DEBUG mode.
 
 **dwd_r06.json**
 
 ```json
```

### Comparing `pyg2p-3.2.4/README.md` & `pyg2p-3.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   ```
 
 >IMPORTANT: Before to launch setup, you need the following steps:
 
 >Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes gdal
+$ conda install -c conda-forge gdal eccodes
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -406,15 +406,15 @@
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>type</b></td><td>Type of aggregation (it was Manipulation in
 grib2pcraster). It can be average or accumulation.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to True and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
+        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to true and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td>forceZeroArray</td><td>Optional. In case of “accumulation”, and only
 then, if this attribute is set to”y” (or any value different from “false”, “False”, “FALSE”, “no”,
 “NO”, “No”, “0”), the program will use a zero array as message at step 0 to compute the first
 map, even if the GRIB file has a step 0 message.</td>
         </tr>
@@ -665,14 +665,28 @@
 
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
+#### ADW
+It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
+If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "adw",
+  "@adw_broadcasting": false}
+}
+```
+
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
@@ -730,15 +744,15 @@
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
 {
 "Aggregation": {
   "@type": "average",
-  "@halfweights": False}
+  "@halfweights": false}
 }
 ```
 
 To better understand what these two types of aggregations do, the DEBUG output of execution is presented later in same paragraph.
 
 ### Average
 Temperatures are often extracted as averages on 24 hours or 6 hours. Here's a typical execution configuration and the output of interest:
@@ -748,15 +762,15 @@
 ```json
 {
 "Execution": {
 "@name": "cosmo_T24",
 "Aggregation": {
 "@step": 24,
 "@type": "average",
-"@halfweights": False
+"@halfweights": false
 },
 "OutMaps": {
 "@cloneMap": "/dataset/maps/europe/dem.map",
 "@ext": 4,
 "@fmap": 1,
 "@namePrefix": "T24",
 "@unitTime": 24,
@@ -794,33 +808,33 @@
 
 This is needed because we performed 24 hours average over 6 hourly steps.
 
 **Details about average parameters:**
 
 The to evaluate the average, the following steps are executed:
 
-- when "halfweights" is False, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
+- when "halfweights" is false, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 48 every 6 hours: 0,6,12,18,24,30,....
 
   Day 1: Aggregation starts from 24-24+1=1, so it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 six times. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24+1=25...
 
-- when "halfweights" is True, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
+- when "halfweights" is true, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 72 every 6 hours: 0,6,12,18,24,30,36,....
 
   Day 1: Aggregation starts from 24-24=0, and will consider the step 0 value multiplied but 3, that is half of the number of steps between two step keys in the grib file. Then it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 again multiplied by 3. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24=24: the step 24 will have a weight of 3, while steps 30,36 and 42 will be counted 6 times, and finally the step 48 will have a weight of 3. 
 
-- if start_step is zero or is not specified, the aggregation will start from 1
+- if start_step is zero or is not specified, the aggregation will start from 0
 
 ### Accumulation
 For precipitation values, accumulation over 6 or 24 hours is often performed. Here's an example of configuration and execution output in DEBUG mode.
 
 **dwd_r06.json**
 
 ```json
```

### Comparing `pyg2p-3.2.4/configuration/global/geopotentials.json` & `pyg2p-3.2.5/configuration/global/geopotentials.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/configuration/global/intertables.json` & `pyg2p-3.2.5/configuration/global/intertables.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9914529914529915%*

 * *Differences: {"'I-15.75_16.125_511_415_212065_rotated_ll_-1700000_2700000_5000_-5000_34.97_71.07_-1700000_2700000_5000_-5000_-24.35_51.35scipy_adw'": "OrderedDict([('filename', "*

 * *                                                                                                                                         "'tbl_pf10tp_550800_scipy_adw.npy'), "*

 * *                                                                                                                                         "('method', "*

 * *                    […]*

```diff
@@ -72,14 +72,25 @@
             212065
         ],
         "target_shape": [
             810,
             680
         ]
     },
+    "I-15.75_16.125_511_415_212065_rotated_ll_-1700000_2700000_5000_-5000_34.97_71.07_-1700000_2700000_5000_-5000_-24.35_51.35scipy_adw": {
+        "filename": "tbl_pf10tp_550800_scipy_adw.npy",
+        "method": "adw",
+        "source_shape": [
+            212065
+        ],
+        "target_shape": [
+            810,
+            680
+        ]
+    },
     "I-15.75_16.125_511_415_212065_rotated_ll_-1700000_2700000_5000_-5000_34.97_71.07_-1700000_2700000_5000_-5000_-24.35_51.35scipy_invdist": {
         "filename": "tbl_pf10tp_550800_scipy_invdist.npy",
         "method": "invdist",
         "source_shape": [
             212065
         ],
         "target_shape": [
```

### Comparing `pyg2p-3.2.4/configuration/global/parameters.json` & `pyg2p-3.2.5/configuration/global/parameters.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/setup.py` & `pyg2p-3.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/__init__.py` & `pyg2p-3.2.5/src/pyg2p/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/exceptions.py` & `pyg2p-3.2.5/src/pyg2p/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/__init__.py` & `pyg2p-3.2.5/src/pyg2p/main/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/api.py` & `pyg2p-3.2.5/src/pyg2p/main/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,15 @@
             self._vars['correction.demMap'] = self.api_conf['Parameter']['demMap']
             if not self._vars['geopotential.dir'] and self.api_conf.get('geopotentialDir'):
                 self._vars['geopotential.dirs']['user'] = self.api_conf['geopotentialDir']
 
         self._vars['outMaps.clone'] = self.api_conf['OutMaps']['cloneMap']
         interpolation_conf = self.api_conf['OutMaps']['Interpolation']
         self._vars['interpolation.mode'] = interpolation_conf.get('mode', self.default_values['interpolation.mode'])
+        self._vars['interpolation.use_broadcasting'] = interpolation_conf.get('use_broadcasting', False)
         self._vars['interpolation.rotated_target'] = interpolation_conf.get('rotated_target', False)
         if not self._vars['interpolation.dir'] and self.api_conf.get('intertableDir'):
             self._vars['interpolation.dirs']['user'] = self.api_conf['intertableDir']
 
         self._vars['interpolation.latMap'] = interpolation_conf['latMap']
         self._vars['interpolation.lonMap'] = interpolation_conf['lonMap']
         self._vars['outMaps.unitTime'] = self.api_conf['OutMaps'].get('unitTime')
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/config.py` & `pyg2p-3.2.5/src/pyg2p/main/config.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/context.py` & `pyg2p-3.2.5/src/pyg2p/main/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from ..util import files, strings
 from .manipulation.aggregator import ACCUMULATION
 from ..exceptions import (ApplicationException, INVALID_INTERPOL_METHOD,
                           WRONG_ARGS, NOT_A_NUMBER, NOT_EXISTING_MAPS, MISSING_INPUT_GRIB, NOT_EXISTING_INPUT_GRIB)
 
 
 class Context:
-    allowed_interp_methods = ('grib_nearest', 'grib_invdist', 'nearest', 'invdist', 'bilinear', 'triangulation', 'bilinear_delaunay')
+    allowed_interp_methods = ('grib_nearest', 'grib_invdist', 'nearest', 'invdist', 'adw', 'cdd', 'bilinear', 'triangulation', 'bilinear_delaunay')
     default_values = {'interpolation.mode': 'grib_nearest', 'outMaps.unitTime': '24'}
 
     def __getitem__(self, param):
         return self._vars[param]
 
     def __setitem__(self, param, value):
         self._vars[param] = value
@@ -356,14 +356,15 @@
             self._vars['correction.formula'] = exec_conf['Parameter']['@correctionFormula']
             self._vars['correction.gemFormula'] = exec_conf['Parameter']['@gem']
             self._vars['correction.demMap'] = exec_conf['Parameter']['@demMap']
 
         self._vars['outMaps.clone'] = exec_conf['OutMaps']['@cloneMap']
         interpolation_conf = exec_conf['OutMaps']['Interpolation']
         self._vars['interpolation.mode'] = interpolation_conf.get('@mode', self.default_values['interpolation.mode'])
+        self._vars['interpolation.adw_broadcasting'] = interpolation_conf.get('@adw_broadcasting', False)
         self._vars['interpolation.rotated_target'] = interpolation_conf.get('@rotated_target', False)
         if not self._vars['interpolation.dir'] and interpolation_conf.get('@intertableDir'):
             # get from JSON
             self._vars['interpolation.dirs']['user'] = interpolation_conf['@intertableDir']
         if not self._vars['geopotential.dir'] and interpolation_conf.get('@geopotentialDir'):
             # get from JSON
             self._vars['geopotential.dirs']['user'] = interpolation_conf['@geopotentialDir']
@@ -408,14 +409,15 @@
             self._vars['parameter.dataDate'] = int(exec_conf['Parameter']['@dataDate'])  # date
 
         self._vars['parameter.level'] = exec_conf['Parameter'].get('@level')  # number
 
         if exec_conf.get('Aggregation'):
             self._vars['aggregation.step'] = exec_conf['Aggregation'].get('@step')
             self._vars['aggregation.type'] = exec_conf['Aggregation'].get('@type')
+            self._vars['aggregation.halfweights'] = bool(exec_conf['Aggregation'].get('@halfweights'))
 
             self._vars['execution.doAggregation'] = bool(self._vars.get('aggregation.step')) \
                 and bool(self._vars.get('aggregation.type'))
             self._vars['aggregation.forceZeroArray'] = self._vars.get('aggregation.type') == ACCUMULATION \
                 and exec_conf['Aggregation'].get('@forceZeroArray', 'False').lower() not in strings.FALSE_STRINGS
 
         # string interpolation for custom user configurations (i.e. dataset folders)
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/controller.py` & `pyg2p-3.2.5/src/pyg2p/main/controller.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/interpolation/__init__.py` & `pyg2p-3.2.5/src/pyg2p/main/interpolation/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,36 +5,37 @@
 
 import numpy as np
 import numpy.ma as ma
 from pyg2p import Loggable
 
 from . import grib_interpolation_lib
 from .latlong import LatLong
-from .scipy_interpolation_lib import ScipyInterpolation, DEBUG_BILINEAR_INTERPOLATION, \
+from .scipy_interpolation_lib import ScipyInterpolation, DEBUG_BILINEAR_INTERPOLATION, DEBUG_ADW_INTERPOLATION, \
                                         DEBUG_MIN_LAT, DEBUG_MIN_LON, DEBUG_MAX_LAT, DEBUG_MAX_LON
                                         
 from ...exceptions import ApplicationException, NO_INTERTABLE_CREATED
 import pyg2p.util.files
 import pyg2p.util.numeric
 
 
 class Interpolator(Loggable):
     _LOADED_INTERTABLES = {}
     _prefix = 'I'
-    scipy_modes_nnear = {'nearest': 1, 'invdist': 4, 'bilinear': 4, 'triangulation': 3, 'bilinear_delaunay': 4}
+    scipy_modes_nnear = {'nearest': 1, 'invdist': 4, 'adw': 4, 'cdd': 4, 'bilinear': 4, 'triangulation': 3, 'bilinear_delaunay': 4}
     suffixes = {'grib_nearest': 'grib_nearest', 'grib_invdist': 'grib_invdist',
-                'nearest': 'scipy_nearest', 'invdist': 'scipy_invdist',
+                'nearest': 'scipy_nearest', 'invdist': 'scipy_invdist', 'adw': 'scipy_adw', 'cdd': 'scipy_cdd',
                 'bilinear': 'scipy_bilinear', 'triangulation': 'scipy_triangulation', 'bilinear_delaunay': 'scipy_bilinear_delaunay'}
     _format_intertable = 'tbl{prognum}_{source_file}_{target_size}_{suffix}.npy.gz'.format
 
     def __init__(self, exec_ctx, mv_input):
         super().__init__()
         self._mv_grib = mv_input
         self.interpolate_with_grib = exec_ctx.is_with_grib_interpolation
         self._mode = exec_ctx.get('interpolation.mode')
+        self._adw_broadcasting = exec_ctx.get('interpolation.adw_broadcasting')
         self._source_filename = pyg2p.util.files.filename(exec_ctx.get('input.file'))
         self._suffix = self.suffixes[self._mode]
         self._intertable_dirs = exec_ctx.get('interpolation.dirs')
         self._rotated_target_grid = exec_ctx.get('interpolation.rotated_target')
         self._target_coords = LatLong(exec_ctx.get('interpolation.latMap'), exec_ctx.get('interpolation.lonMap'))
         self.mv_out = self._target_coords.mv
         self.parallel = exec_ctx.get('interpolation.parallel')
@@ -123,15 +124,15 @@
             return intertable[0], intertable[1], intertable[2]
         elif self._mode == 'grib_invdist':
             # grib inverse distance table is a "recorded numpy array" with keys 'indexes' and 'coeffs'
             indexes = intertable['indexes']  # first two arrays of this group are target xs and ys indexes
             coeffs = intertable['coeffs']
             return indexes[0], indexes[1], indexes[2], indexes[3], indexes[4], indexes[5], coeffs[0], coeffs[1], coeffs[2], coeffs[3]
         else:
-            # self._mode in ('invdist', 'nearest', 'bilinear', 'triangulation', 'bilinear_delaunay'):
+            # self._mode in ('invdist', 'adw', 'cdd', 'nearest', 'bilinear', 'triangulation', 'bilinear_delaunay'):
             # return indexes and weighted distances (only used with nnear > 1)
             indexes = intertable['indexes']
             coeffs = intertable['coeffs']
             return indexes, coeffs
 
     # ####### SCIPY INTERPOLATION ###################################
     def _interpolate_scipy_append_mv(self, v, weights, indexes, nnear):
@@ -173,30 +174,52 @@
                 latefas=self._target_coords.lats[selection_lats,:][:,selection_lons]
                 lonefas=self._target_coords.lons[selection_lats,:][:,selection_lons]
 
             intertable_id, intertable_name = 'DEBUG','DEBUG.npy'
         else:
             intertable_id, intertable_name = self._intertable_filename(grid_id)
 
+        if DEBUG_ADW_INTERPOLATION:
+            # to debug create a limited controlled set of input values 
+            #
+            # np.random.seed(0)
+            # latgrib = np.random.uniform(low=3, high=11, size=10)
+            # longrib = np.random.uniform(low=46, high=50, size=10)
+            # v = np.random.uniform(low=100, high=200, size=10)
+            # latgrib = np.array([ 7.39050803,  8.72151493,  7.82210701,  7.35906546,  6.38923839,
+            #     8.1671529,  6.50069769, 10.13418401, 10.70930208,  6.06753215])
+            # longrib = np.array([49.16690015, 48.11557968, 48.27217824, 49.70238655, 46.28414423,
+            #     46.3485172, 46.08087359, 49.33047938, 49.112627, 49.48004859])
+            # v = np.array([197.86183422, 179.91585642, 146.14793623, 178.05291763, 111.82744259, 
+            #     163.99210213, 114.33532874, 194.4668917, 152.18483218, 141.466194  ])
+            # latgrib = np.array([ 7.39050803,  8.72151493,  7.82210701,  7.35906546])
+            # longrib = np.array([49.16690015, 48.11557968, 48.27217824, 49.70238655])
+            # v = np.array([100, 133, 166, 200  ])
+            latgrib = np.array([ 8,  8,  8,  8])
+            longrib = np.array([45, 48.5, 49, 50])
+            v = np.array([200, 100, 100, 100  ])
+            intertable_id, intertable_name = 'DEBUG_ADW','DEBUG_ADW.npy'
+
         nnear = self.scipy_modes_nnear[self._mode]
 
-        if pyg2p.util.files.exists(intertable_name) or pyg2p.util.files.exists(intertable_name + '.gz'):
-            indexes, weights = self._read_intertable(intertable_name)
-            result = self._interpolate_scipy_append_mv(v, weights, indexes, nnear)
+        if (not DEBUG_ADW_INTERPOLATION) and \
+            (pyg2p.util.files.exists(intertable_name) or pyg2p.util.files.exists(intertable_name + '.gz')):
+                indexes, weights = self._read_intertable(intertable_name)
+                result = self._interpolate_scipy_append_mv(v, weights, indexes, nnear)
 
         elif self.create_if_missing:
             self.intertables_config.check_write()
             if latgrib is None:
                 self._log('Trying to interpolate without grib lat/lons. Probably a malformed grib!', 'ERROR')
                 raise ApplicationException.get_exc(5000)
 
             self._log('\nInterpolating table not found\n Id: {}\nWill create file: {}'.format(intertable_id, intertable_name), 'WARN')
             scipy_interpolation = ScipyInterpolation(longrib, latgrib, grid_details, v.ravel(), nnear, self.mv_out,
                                           self._mv_grib, target_is_rotated=self._rotated_target_grid,
-                                          parallel=self.parallel, mode=self._mode)
+                                          parallel=self.parallel, mode=self._mode, use_broadcasting=self._adw_broadcasting)
             _, weights, indexes = scipy_interpolation.interpolate(lonefas, latefas)
             result = self._interpolate_scipy_append_mv(v, weights, indexes, nnear)
 
             # saving interpolation lookup table
             intertable = np.rec.fromarrays((indexes, weights), names=('indexes', 'coeffs'))
             if intertable_name.endswith('.gz'):
                 f = gzip.GzipFile(intertable_name, 'w')
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/interpolation/grib_interpolation_lib.py` & `pyg2p-3.2.5/src/pyg2p/main/interpolation/grib_interpolation_lib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/interpolation/latlong.py` & `pyg2p-3.2.5/src/pyg2p/main/interpolation/latlong.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/interpolation/scipy_interpolation_lib.py` & `pyg2p-3.2.5/src/pyg2p/main/interpolation/scipy_interpolation_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,30 +15,35 @@
 from pyg2p.util.strings import now_string
 
 #from matplotlib import pyplot as plt
 from scipy.integrate import quad
 
 
 DEBUG_BILINEAR_INTERPOLATION = False
+DEBUG_ADW_INTERPOLATION = False
 # DEBUG_MIN_LAT = 88
 # DEBUG_MIN_LON = -180
 # DEBUG_MAX_LAT = 90
 # DEBUG_MAX_LON = 180
 # DEBUG_MIN_LAT = 40
 # DEBUG_MIN_LON = 5
 # DEBUG_MAX_LAT = 50
 # DEBUG_MAX_LON = 10
 # DEBUG_MIN_LAT = 68
 # DEBUG_MIN_LON = -24
 # DEBUG_MAX_LAT = 70
 # DEBUG_MAX_LON = -22
-DEBUG_MIN_LAT = -10
-DEBUG_MIN_LON = -100
-DEBUG_MAX_LAT = 25
-DEBUG_MAX_LON = -50
+# DEBUG_MIN_LAT = -10
+# DEBUG_MIN_LON = -100
+# DEBUG_MAX_LAT = 25
+# DEBUG_MAX_LON = -50
+DEBUG_MIN_LAT = 7
+DEBUG_MIN_LON = 45
+DEBUG_MAX_LAT = 9
+DEBUG_MAX_LON = 50
 #DEBUG_NN = 15410182
 
 
 ###########################################################################################
 ###### functions used to get correct quadrilateral points for the bilinear interpolation ####
 ###########################################################################################
 
@@ -279,25 +284,26 @@
     http://docs.scipy.org/doc/scipy/reference/spatial.html
     """
     gribapi_version = list(map(int, eccodes.codes_get_api_version().split('.')))
     rotated_bugfix_gribapi = gribapi_version[0] > 1 or (gribapi_version[0] == 1 and gribapi_version[1] > 14) or (gribapi_version[0] == 1 and gribapi_version[1] == 14 and gribapi_version[2] >= 3)
 
     def __init__(self, longrib, latgrib, grid_details, source_values, nnear, 
                     mv_target, mv_source, target_is_rotated=False, parallel=False,
-                    mode='nearest'):
+                    mode='nearest', use_broadcasting = False):
         stdout.write('Start scipy interpolation: {}\n'.format(now_string()))
         self.geodetic_info = grid_details
         self.source_grid_is_rotated = 'rotated' in grid_details.get('gridType')
         self.target_grid_is_rotated = target_is_rotated
         self.njobs = 1 if not parallel else -1
         
         self.longrib = longrib
         self.latgrib = latgrib
         self.nnear = nnear
         self.mode = mode
+        self.use_broadcasting = use_broadcasting
         self._mv_target = mv_target
         self._mv_source = mv_source
         self.z = source_values
         
         # we receive rotated coords from GRIB_API iterator before 1.14.3
         x, y, zz = self.to_3d(longrib, latgrib, to_regular=not self.rotated_bugfix_gribapi)
         source_locations = np.vstack((x.ravel(), y.ravel(), zz.ravel())).T
@@ -333,30 +339,31 @@
         if self.mode == 'nearest' and self.nnear == 1:
             # return results, indexes
             result, indexes = self._build_nn(distances, indexes)
             weights = distances
         else:
             if self.mode == 'invdist': 
                 # return results, distances, indexes
-                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear) 
-            else:  
-                if self.mode == 'bilinear' and self.nnear == 4: # bilinear interpolation only supported with nnear = 4
-                    # BILINEAR INTERPOLATION
-                    result, weights, indexes = self._build_weights_bilinear(distances, indexes, efas_locations, self.nnear) 
-                else:
-                    if self.mode == 'triangulation':
-                        # linear barycentric interpolation on Delaunay triangulation
-                        result, weights, indexes = self._build_weights_triangulation(use_bilinear=False) 
-                    else:
-                        if self.mode == 'bilinear_delaunay':
-                            # bilinear interpolation on Delaunay triangulation
-                            result, weights, indexes = self._build_weights_triangulation(use_bilinear=True) 
-                        else:
-                            raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
-                                        f"interpolation method not supported (mode = {self.mode}, nnear = {self.nnear})")
+                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear)
+            elif self.mode == 'adw':
+                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='Shepard', use_broadcasting=self.use_broadcasting)             
+            elif self.mode == 'cdd':
+                result, weights, indexes = self._build_weights_invdist(distances, indexes, self.nnear, adw_type='CDD', use_broadcasting=self.use_broadcasting)
+            elif self.mode == 'bilinear' and self.nnear == 4: # bilinear interpolation only supported with nnear = 4
+                # BILINEAR INTERPOLATION
+                result, weights, indexes = self._build_weights_bilinear(distances, indexes, efas_locations, self.nnear) 
+            elif self.mode == 'triangulation':
+                # linear barycentric interpolation on Delaunay triangulation
+                result, weights, indexes = self._build_weights_triangulation(use_bilinear=False) 
+            elif self.mode == 'bilinear_delaunay':
+                    # bilinear interpolation on Delaunay triangulation
+                    result, weights, indexes = self._build_weights_triangulation(use_bilinear=True) 
+            else:
+                raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
+                            f"interpolation method not supported (mode = {self.mode}, nnear = {self.nnear})")
                     
                
         stdout.write('End scipy interpolation: {}\n'.format(now_string()))
         end = time.time()
         stdout.write('Interpolation time (sec): {}\n'.format(end - start))
 
         return result, weights, indexes
@@ -415,16 +422,66 @@
             result[jinterpol] = wz
             jinterpol += 1
         stdout.write('{}{:>100}'.format(back_char, ' '))
         stdout.write('{}Building coeffs: {}/{} [outs: {}] (100%)\n'.format(back_char, jinterpol, num_cells, outs))
         stdout.flush()
         return result, idxs
 
-    # Invdist Optimized version (using broadcast)
-    def _build_weights_invdist(self, distances, indexes, nnear):
+    # # Invdist Optimized version (using broadcast)
+    # def _build_weights_invdist(self, distances, indexes, nnear):
+    #     z = self.z
+    #     result = mask_it(np.empty((len(distances),) + np.shape(z[0])), self._mv_target, 1)
+    #     weights = empty((len(distances),) + (nnear,))
+    #     idxs = empty((len(indexes),) + (nnear,), fill_value=z.size, dtype=int)
+    #     num_cells = result.size
+    #     back_char, _ = progress_step_and_backchar(num_cells)
+
+    #     stdout.write('Skipping neighbors at distance > {}\n'.format(self.min_upper_bound))
+    #     stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 0, 5, 0, 0))
+    #     stdout.flush()
+
+    #     dist_leq_1e_10 = distances[:, 0] <= 1e-10
+    #     dist_leq_min_upper_bound = np.logical_and(~dist_leq_1e_10, distances[:, 0] <= self.min_upper_bound)
+        
+    #     # distances <= 1e-10 : take exactly the point, weight = 1
+    #     onlyfirst_array = np.zeros(nnear)
+    #     onlyfirst_array[0] = 1
+    #     weights[dist_leq_1e_10] = onlyfirst_array
+    #     idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
+    #     result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
+
+    #     w = np.zeros_like(distances)
+    #     w[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound] ** 2
+    #     stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 1, 5, 100/5))
+    #     stdout.flush()
+    #     sums = np.sum(w[dist_leq_min_upper_bound], axis=1, keepdims=True)
+    #     stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 2, 5, 2*100/5))
+    #     stdout.flush()
+    #     weights[dist_leq_min_upper_bound] = w[dist_leq_min_upper_bound] / sums
+    #     stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 3, 5, 3*100/5))
+    #     stdout.flush()
+    #     wz = np.einsum('ij,ij->i', weights, z[indexes])
+    #     stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 4, 5, 4*100/5))
+    #     stdout.flush()
+    #     idxs[dist_leq_min_upper_bound] = indexes[dist_leq_min_upper_bound]
+    #     result[dist_leq_min_upper_bound] = wz[dist_leq_min_upper_bound]
+    #     stdout.write('{}Building coeffs: {}/{} (100%)\n'.format(back_char, 5, 5))
+    #     stdout.flush()
+    #     return result, weights, idxs
+
+    # Inverse distance weights (IDW) interpolation, with optional Angular distance weighting (ADW) factor
+    # if adw_type == None -> simple IDW 
+    # if adw_type == Shepard -> Shepard 1968 original formulation
+    def _build_weights_invdist(self, distances, indexes, nnear, adw_type = None, use_broadcasting = False):
+        if DEBUG_ADW_INTERPOLATION:
+            self.min_upper_bound = 1000000000
+            if DEBUG_BILINEAR_INTERPOLATION:
+                n_debug=1940
+            else:
+                n_debug=11805340
         z = self.z
         result = mask_it(np.empty((len(distances),) + np.shape(z[0])), self._mv_target, 1)
         weights = empty((len(distances),) + (nnear,))
         idxs = empty((len(indexes),) + (nnear,), fill_value=z.size, dtype=int)
         num_cells = result.size
         back_char, _ = progress_step_and_backchar(num_cells)
 
@@ -432,35 +489,168 @@
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 0, 5, 0, 0))
         stdout.flush()
 
         dist_leq_1e_10 = distances[:, 0] <= 1e-10
         dist_leq_min_upper_bound = np.logical_and(~dist_leq_1e_10, distances[:, 0] <= self.min_upper_bound)
         
         # distances <= 1e-10 : take exactly the point, weight = 1
-        weights[dist_leq_1e_10] = np.array([1., 0., 0., 0.])
+        onlyfirst_array = np.zeros(nnear)
+        onlyfirst_array[0] = 1
+        weights[dist_leq_1e_10] = onlyfirst_array
         idxs[dist_leq_1e_10] = indexes[dist_leq_1e_10]
         result[dist_leq_1e_10] = z[indexes[dist_leq_1e_10][:, 0]]
 
         w = np.zeros_like(distances)
         w[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound] ** 2
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 1, 5, 100/5))
         stdout.flush()
+
+        if (adw_type=='Shepard'):
+            # initialize weights
+            weight_directional = np.zeros_like(distances)
+
+            # get "s" vector as the inverse distance with power = 1 (in "w" we have the invdist power 2)
+            # actually s(d) should be 
+            #   1/d                     when 0 < d < r'/3
+            #   (27/4r')*(d/r'-1)       when r'/3 < d < r'
+            #   0                       when r' < d
+            # The orginal method consider a range of 4 to 10 data points e removes distant point using the rule:
+            # pi*r= 7(N/A)  where N id the number of points and A is the area of the largest poligon enclosed by data points
+            # r'(C^n) = di(n+1) where di is the Point having the minimum distance major than the first n Points
+            # so that
+            #   r' = r' C^4 = di(5)     when n(C) <= 4
+            #   r' = r                  when 4 < n(C) <= 10
+            #   r' = r' C^10 = di(11)   when 10 < n(C)
+            #
+            # TODO: check if the implementation needs to be updated accordingly
+            # here we take only the inverse of the distance in "s"
+            s = np.zeros_like(distances)       
+            s[dist_leq_min_upper_bound] = 1. / distances[dist_leq_min_upper_bound]
+
+            self.lat_inALL = self.target_latsOR.ravel()
+            self.lon_inALL = self.target_lonsOR.ravel()
+
+            # start_time = time.time()
+            if not use_broadcasting:
+                for i in range(nnear):
+                    xj_diff = self.lat_inALL[:, np.newaxis] - self.latgrib[indexes]
+                    yj_diff = self.lon_inALL[:, np.newaxis] - self.longrib[indexes]
+                    
+                    Dj = np.sqrt(xj_diff**2 + yj_diff**2)
+                    # TODO: check here: we could use "distances", but we are actually evaluating the cos funcion on lat and lon values, that 
+                    # approximates the real angle... to use "distances" we need to operate in 3d version of the points
+                    # in theory it should be OK to use the solution above, otherwise we can change it to 
+                    # Di = distances[i]
+                    # Dj = distances
+                    # and formula cos_theta = [(x-xi)*(x-xj) + (y-yi)*(y-yj) + (z-zi)*(z-zj)] / di*dj
+                    
+                    # cos_theta = [(x-xi)*(x-xj) + (y-yi)*(y-yj)] / di*dj. 
+                    #cos_theta = (xi_diff[:,np.newaxis] * xj_diff + yi_diff[:,np.newaxis] * yj_diff) / (Di[:,np.newaxis] * Dj)
+                    # cos_theta = (xj_diff[:,i,np.newaxis] * xj_diff + yj_diff[:,i,np.newaxis] * yj_diff) / (Dj[:,i,np.newaxis] * Dj)
+                    # numerator = np.sum((1 - cos_theta) * s, axis=1)
+                    # denominator = np.sum(s, axis=1)
+                    
+                    cos_theta = (xj_diff[:,i,np.newaxis] * xj_diff + yj_diff[:,i,np.newaxis] * yj_diff) / (Dj[:,i,np.newaxis] * Dj)
+                    # skip when i==j, so that directional weight of i is evaluated on all points j where j!=i 
+                    # TODO: tip: since cos_theta = 1 for i==j, to speed up we can skip this passage and apply i!=j only on denominator
+                    cos_theta = cos_theta[:,np.concatenate([np.arange(i), np.arange(i+1, cos_theta.shape[1])])]
+                    sj = s[:,np.concatenate([np.arange(i), np.arange(i+1, s.shape[1])])]            
+                    numerator = np.sum((1 - cos_theta) * sj, axis=1)
+                    denominator = np.sum(sj, axis=1)
+                                        
+                    weight_directional[dist_leq_min_upper_bound, i] = numerator[dist_leq_min_upper_bound] / denominator[dist_leq_min_upper_bound]
+
+                    # DEBUG: test the point at n_debug 11805340=lat 8.025 lon 47.0249999
+                    if DEBUG_ADW_INTERPOLATION:
+                        print("i: {}".format(i))
+                        print("cos_theta: {}".format(cos_theta[n_debug]))
+                        print("s: {}".format(s[n_debug]))
+                        print("numerator: {}".format(numerator[n_debug]))
+                        print("denominator: {}".format(denominator[n_debug]))
+            else:
+                # All in broadcasting:            
+                # this algorithm uses huge amount of memory and deas not speed up much on standard Virtual Machine
+                # TODO: check if it is worth to use it on HPC 
+                # Compute xi and yi for all elements
+                xi = self.latgrib[indexes]
+                yi = self.longrib[indexes]
+                # Compute xi_diff and yi_diff for all elements
+                xi_diff = self.lat_inALL[:, np.newaxis] - xi
+                yi_diff = self.lon_inALL[:, np.newaxis] - yi
+                # Compute Di for all elements
+                Di = np.sqrt(xi_diff**2 + yi_diff**2)
+                # Compute cos_theta for all elements
+                cos_theta = (xi_diff[:, :, np.newaxis] * xi_diff[:, np.newaxis, :] + yi_diff[:, :, np.newaxis] * yi_diff[:, np.newaxis, :]) / (Di[:, :, np.newaxis] * Di[:, np.newaxis, :])
+                # skip when i==j, so that directional weight of i is evaluated on all points j where j!=i 
+                # TODO: tip: since cos_theta = 1 for i==j, to speed up we can skip this passage and apply i!=j only on denominator
+                # Delete the diagonal elements from cos_theta
+                # Reshape cos_theta to (n, nnear, nnear-1)
+                n = cos_theta.shape[0]
+                m = cos_theta.shape[1]
+                strided = np.lib.stride_tricks.as_strided
+                s0,s1,s2 = cos_theta[:].strides
+                cos_theta = strided(cos_theta.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).reshape(n,m,-1)
+                sj = np.tile(s[:, np.newaxis, :], (1, 4, 1))
+                s0,s1,s2 = sj[:].strides
+                sj = strided(sj.ravel()[1:], shape=(n,m-1,m), strides=(s0,s1+s2,s2)).reshape(n,m,-1)
+
+                numerator = np.sum((1 - cos_theta) * sj, axis=2)
+                denominator = np.sum(sj, axis=2)
+                # Compute weight_directional for all elements
+                weight_directional[dist_leq_min_upper_bound, :] = numerator[dist_leq_min_upper_bound, :] / denominator[dist_leq_min_upper_bound, :]
+    
+            # end_time = time.time()
+            # elapsed_time = end_time - start_time
+            # print(f"Elapsed time for computation: {elapsed_time:.6f} seconds")
+    
+            # update weights with directional ones
+            if DEBUG_ADW_INTERPOLATION:
+                print("weight_directional: {}".format(weight_directional[n_debug]))
+                print("w (before adding angular weights): {}".format(w[n_debug]))
+            w = np.multiply(w,1+weight_directional)
+            if DEBUG_ADW_INTERPOLATION:
+                print("w (after adding angular weights): {}".format(w[n_debug]))
+        elif (adw_type=='CDD'):
+            raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
+                        f"interpolation method not implemented yet (mode = {self.mode}, nnear = {self.nnear}, adw_type = {adw_type})")
+        elif (adw_type!=None):
+            raise ApplicationException.get_exc(INVALID_INTERPOL_METHOD, 
+                        f"interpolation method not supported (mode = {self.mode}, nnear = {self.nnear}, adw_type = {adw_type})")
+
+        #normalize weights
         sums = np.sum(w[dist_leq_min_upper_bound], axis=1, keepdims=True)
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 2, 5, 2*100/5))
         stdout.flush()
         weights[dist_leq_min_upper_bound] = w[dist_leq_min_upper_bound] / sums
+        if DEBUG_ADW_INTERPOLATION:
+            dist_smalltest = distances[:, 0] <= 10000
+            onlyfirst_array_test = np.zeros(nnear)
+            onlyfirst_array_test[0] = 1000
+            weights[dist_smalltest]=onlyfirst_array_test
+            print("weights (after normalization): {}".format(weights[n_debug]))
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 3, 5, 3*100/5))
         stdout.flush()
+
         wz = np.einsum('ij,ij->i', weights, z[indexes])
         stdout.write('{}Building coeffs: {}/{} ({:.2f}%)\n'.format(back_char, 4, 5, 4*100/5))
         stdout.flush()
         idxs[dist_leq_min_upper_bound] = indexes[dist_leq_min_upper_bound]
         result[dist_leq_min_upper_bound] = wz[dist_leq_min_upper_bound]
+        if DEBUG_ADW_INTERPOLATION:
+            print("result: {}".format(result[n_debug]))
+            print("lat: {}".format(self.lat_inALL[n_debug]))
+            print("lon: {}".format(self.lon_inALL[n_debug]))
+            print("idxs: {}".format(idxs[n_debug]))
+            print("distances: {}".format(distances[n_debug]))
+            print("latgrib: {}".format(self.latgrib[idxs[n_debug]]))
+            print("longrib: {}".format(self.longrib[idxs[n_debug]]))
+            print("value: {}".format(self.z[idxs[n_debug]]))
         stdout.write('{}Building coeffs: {}/{} (100%)\n'.format(back_char, 5, 5))
         stdout.flush()
+
         return result, weights, idxs
 
     # take additional points from the KDTree close to the current point and replace the wrong ones with a new ones
     def replaceIndex(self, indexes_to_replace, indexes, nn, additional_points):
         additional_points += len(indexes_to_replace)
         # replace the unwanted index with next one:
         _, replacement_indexes = self.tree.query(self.target_location, k=self.nnear+additional_points, n_jobs=self.njobs) 
@@ -738,15 +928,15 @@
         normalized_latgrib=self.latgrib.copy()
         normalized_longrib=self.longrib.copy()
         normalized_longrib[normalized_longrib>180]-=360
         z=self.z.copy()
 
         longrib_max = normalized_longrib.max()
         longrib_min = normalized_longrib.min()
-        # evaluate an approx_grib_resolution by using 10 times the first longidure values 
+        # evaluate an approx_grib_resolution by using 10 times the first longitude values 
         # to check if the whole globe is covered
         approx_grib_resolution = abs(normalized_longrib[0]-normalized_longrib[1])*1.5
         is_global_map = (360-(longrib_max-longrib_min))<approx_grib_resolution
         if is_global_map:
             #additional points map
             original_indexes=[]
             original_indexes = np.append(original_indexes,np.where(normalized_longrib>longrib_max-approx_grib_resolution*2)).astype(int)
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/manipulation/aggregator.py` & `pyg2p-3.2.5/src/pyg2p/main/manipulation/aggregator.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,35 +161,28 @@
             out_values = {}
             first_key = list(values.keys())[0]
             resolution_1 = first_key.resolution
             level = first_key.level
             shape_iter = values[first_key].shape
 
             v_ord = collections.OrderedDict(sorted(dict((k.end_step, v_) for (k, v_) in values.items()).items(), key=lambda k: k))
-            iter_end = self._end - self._aggregation_step + 2
-            if self._start > 0 and not self._second_t_res:
-                if self._aggregation_halfweights:
-                    iter_start = self._start - self._aggregation_step
-                    iter_end = self._end - self._aggregation_step + 1
-                else:
-                    iter_start = self._start - self._aggregation_step + 1
-            elif self._second_t_res:
+            if self._start == 0 or self._second_t_res:
                 iter_start = self._start
+                iter_end = self._end - self._aggregation_step + 2
             else:
-                iter_start = 0
+                iter_start = self._start - self._aggregation_step
+                iter_end = self._end - self._aggregation_step + 1
 
             for iter_ in range(iter_start, iter_end, self._aggregation_step):
-                if self._aggregation_halfweights == False and self._start == 0:
-                    iter_from = iter_ + 1
+                if self._aggregation_halfweights or self._start == 0:
+                    iter_from = iter_ 
                     iter_to = iter_ + self._aggregation_step + 1
                 else:
-                    iter_from = iter_
-                    iter_to = iter_ + self._aggregation_step
-                if self._aggregation_halfweights:
-                    iter_to += 1
+                    iter_from = iter_ + 1
+                    iter_to = iter_ + self._aggregation_step + 1
                 temp_sum = np.zeros(shape_iter)
                 v_ord_keys = list(v_ord.keys())
 
                 if self._aggregation_halfweights:
                     count_steps=-1
                     for iterator_avg in range(iter_from, iter_to, 1):
                         if iterator_avg in v_ord_keys:
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/manipulation/conversion.py` & `pyg2p-3.2.5/src/pyg2p/main/manipulation/conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/manipulation/correction.py` & `pyg2p-3.2.5/src/pyg2p/main/manipulation/correction.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/readers/grib.py` & `pyg2p-3.2.5/src/pyg2p/main/readers/grib.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/readers/netcdf.py` & `pyg2p-3.2.5/src/pyg2p/main/readers/netcdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,28 @@
 class NetCDFReader(Loggable):
 
     def __init__(self, nc_map):
         super().__init__()
         self._log(f'Reading {nc_map}')
         nc_map = nc_map.as_posix() if isinstance(nc_map, Path) else nc_map
         self._dataset = Dataset(nc_map)
-        self._var_name = list(self._dataset.variables.items())[-1][0]  # get the last variable name
-        self._rows, self._cols = self._dataset.variables[self._var_name].shape  # just use shape to know rows and cols...
+        self.var_name = self.find_main_var(nc_map)
+
+        self._rows, self._cols = self._dataset.variables[self.var_name].shape  # just use shape to know rows and cols...
         if ('lon' in list(self._dataset.variables)):
             self.label_lat = 'lat'
             self.label_lon = 'lon'
         else:
             self.label_lat = 'y'
             self.label_lon = 'x'
 
         self._origX = self._dataset.variables[self.label_lon][:].min()
         self._origY = self._dataset.variables[self.label_lat][:].min()
         self._pxlW = self._dataset.variables[self.label_lon][1]-self._dataset.variables[self.label_lon][0]
-        self._pxlH = self._dataset.variables[self.label_lat][1]-self._dataset.variables[self.label_lat][0]
-
-        self.var_name = self.find_main_var(nc_map)
-        
+        self._pxlH = self._dataset.variables[self.label_lat][1]-self._dataset.variables[self.label_lat][0]       
         self.lat_min = self._dataset.variables[self.label_lat][:].min()
         self.lon_min = self._dataset.variables[self.label_lon][:].min()
         self.lat_max = self._dataset.variables[self.label_lat][:].max()
         self.lon_max = self._dataset.variables[self.label_lon][:].max()
         self.mv = self._dataset.variables[self.var_name].missing_value
 
     def find_main_var(self, path):
@@ -48,16 +46,16 @@
 
     @property
     def values(self):
         data = self._dataset.variables[self.var_name][:].data
         return data
     
     def get_lat_lon_values(self):
-        lats = np.reshape(self._dataset.variables[self.label_lat][:],(-1,1))*np.ones(self._dataset.variables[self._var_name].shape)
-        lons = self._dataset.variables[self.label_lon][:]*np.ones(self._dataset.variables[self._var_name].shape)
+        lats = np.reshape(self._dataset.variables[self.label_lat][:],(-1,1))*np.ones(self._dataset.variables[self.var_name].shape)
+        lons = self._dataset.variables[self.label_lon][:]*np.ones(self._dataset.variables[self.var_name].shape)
         return lats.data, lons.data
 
     def get_lat_values(self):
         return self._dataset.variables[self.label_lat][:].data
 
     def get_lon_values(self):
         return self._dataset.variables[self.label_lon][:].data
```

### Comparing `pyg2p-3.2.4/src/pyg2p/main/readers/pcr.py` & `pyg2p-3.2.5/src/pyg2p/main/readers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/writers/__init__.py` & `pyg2p-3.2.5/src/pyg2p/main/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/writers/netcdf.py` & `pyg2p-3.2.5/src/pyg2p/main/writers/netcdf.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/main/writers/pcr.py` & `pyg2p-3.2.5/src/pyg2p/main/writers/pcr.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/util/files.py` & `pyg2p-3.2.5/src/pyg2p/util/files.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/util/generics.py` & `pyg2p-3.2.5/src/pyg2p/util/generics.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/util/numeric.py` & `pyg2p-3.2.5/src/pyg2p/util/numeric.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/util/profiling/profilehooks.py` & `pyg2p-3.2.5/src/pyg2p/util/profiling/profilehooks.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p/util/strings.py` & `pyg2p-3.2.5/src/pyg2p/util/strings.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/src/pyg2p.egg-info/PKG-INFO` & `pyg2p-3.2.5/src/pyg2p.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyg2p
-Version: 3.2.4
+Version: 3.2.5
 Summary: Convert GRIB files to netCDF or PCRaster
 Author: Domenico Nappo
 Author-email: domenico.nappo@gmail.com
 License: EUPL 1.2
 Keywords: NetCDF GRIB PCRaster Lisflood EFAS GLOFAS
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -48,15 +48,15 @@
   ```
 
 >IMPORTANT: Before to launch setup, you need the following steps:
 
 >Install eccodes (and GDAL): this can be done compiling from source code or using the available conda virtual environment package by running 
 
 ```bash
-$ conda install -c conda-forge eccodes gdal
+$ conda install -c conda-forge gdal eccodes
 ```
 
 >Configure geopotentials and intertables paths in
 configuration/global/global_conf.json. These paths are used by pyg2p to read
 geopotentials and intertables already configured. You may need to download files from FTP (launch `pyg2p -W` for this). 
 Users running pyg2p installed by a different user (ie. root) will configure similar paths for their own intertables 
 and geopotentials under his home folder. These paths will need write permissions.
@@ -431,15 +431,15 @@
         <td><b>Aggregation</b></td><td><b>step</b></td><td>Step of aggregation in hours.</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td><b>type</b></td><td>Type of aggregation (it was Manipulation in
 grib2pcraster). It can be average or accumulation.</td>
         </tr>
         <tr>
-        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to True and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
+        <td>&nbsp;</td><td><b>halfweights</b></td><td>If set to true and type is "average", it will avaluate the average by using half weights for the first and the last step</td>
         </tr>
         <tr>
         <td>&nbsp;</td><td>forceZeroArray</td><td>Optional. In case of “accumulation”, and only
 then, if this attribute is set to”y” (or any value different from “false”, “False”, “FALSE”, “no”,
 “NO”, “No”, “0”), the program will use a zero array as message at step 0 to compute the first
 map, even if the GRIB file has a step 0 message.</td>
         </tr>
@@ -690,14 +690,28 @@
 
 | Attribute | Details              |
 |-----------|----------------------|
 | p         | 2 (Euclidean metric) |
 | eps       | 0                    |
 | leafsize  | 10                   |
 
+#### ADW
+It's the Angular Distance Weighted (ADW) algorithm with scipy.kd_tree, using 4 neighbours.
+If @adw_broadcasting is set to true, computations will run in full broadcasting mode but requires more memory
+
+```json
+{
+"Interpolation": {
+  "@latMap": "/dataset/maps/europe5km/lat.map",
+  "@lonMap": "/dataset/maps/europe5km/long.map",
+  "@mode": "adw",
+  "@adw_broadcasting": false}
+}
+```
+
 #### bilinear
 It's the bilinear interpolation algorithm applyied on regular and irregular grids. On irregular grids, it tries to get the best quatrilateral around each target point, but at the same time tries to use the best stable and grid-like shape from starting points. To do so, evaluates interpolation looking at point on similar latitude, thus on projected grib files may show some irregular results. 
 
 ```json
 {
 "Interpolation": {
   "@latMap": "/dataset/maps/europe5km/lat.map",
@@ -755,15 +769,15 @@
 Values from grib files can be aggregated before to write the final PCRaster maps. There are two kinds of aggregation available: average and accumulation. 
 The JSON configuration in the execution file will look like:
 
 ```json
 {
 "Aggregation": {
   "@type": "average",
-  "@halfweights": False}
+  "@halfweights": false}
 }
 ```
 
 To better understand what these two types of aggregations do, the DEBUG output of execution is presented later in same paragraph.
 
 ### Average
 Temperatures are often extracted as averages on 24 hours or 6 hours. Here's a typical execution configuration and the output of interest:
@@ -773,15 +787,15 @@
 ```json
 {
 "Execution": {
 "@name": "cosmo_T24",
 "Aggregation": {
 "@step": 24,
 "@type": "average",
-"@halfweights": False
+"@halfweights": false
 },
 "OutMaps": {
 "@cloneMap": "/dataset/maps/europe/dem.map",
 "@ext": 4,
 "@fmap": 1,
 "@namePrefix": "T24",
 "@unitTime": 24,
@@ -819,33 +833,33 @@
 
 This is needed because we performed 24 hours average over 6 hourly steps.
 
 **Details about average parameters:**
 
 The to evaluate the average, the following steps are executed:
 
-- when "halfweights" is False, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
+- when "halfweights" is false, the results of the function is the sum of all the values from "start_step-aggregation_step+1" to end_step, taking for each step the value corresponding to the next available value in the grib file. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 48 every 6 hours: 0,6,12,18,24,30,....
 
   Day 1: Aggregation starts from 24-24+1=1, so it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 six times. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24+1=25...
 
-- when "halfweights" is True, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
+- when "halfweights" is true, the results of the function is the sum of all the values from "start_step-aggregation_step" to end_step, taking for each step the value corresponding to the next available value in the grib file but using half of the weights for the first and the last step in each aggregation_step cicle. E.g:
 
   INPUT: start_step=24, end_step=<not specified, will take the end of file>, aggregation_step=24
 GRIB File: contains data starting from step 0 to 72 every 6 hours: 0,6,12,18,24,30,36,....
 
   Day 1: Aggregation starts from 24-24=0, and will consider the step 0 value multiplied but 3, that is half of the number of steps between two step keys in the grib file. Then it will sum up the step 6 six times, then the step 12 six times, step 18 six times, and finally the step 24 again multiplied by 3. The sum will be divided by the aggretation_step (24) to get the average.
 
   Day 2: same as Day 1 starting from (24+24)-24=24: the step 24 will have a weight of 3, while steps 30,36 and 42 will be counted 6 times, and finally the step 48 will have a weight of 3. 
 
-- if start_step is zero or is not specified, the aggregation will start from 1
+- if start_step is zero or is not specified, the aggregation will start from 0
 
 ### Accumulation
 For precipitation values, accumulation over 6 or 24 hours is often performed. Here's an example of configuration and execution output in DEBUG mode.
 
 **dwd_r06.json**
 
 ```json
```

### Comparing `pyg2p-3.2.4/src/pyg2p.egg-info/SOURCES.txt` & `pyg2p-3.2.5/src/pyg2p.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_cp.json` & `pyg2p-3.2.5/templates/AFFS_cp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_lsp.json` & `pyg2p-3.2.5/templates/AFFS_lsp.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_rg.json` & `pyg2p-3.2.5/templates/AFFS_rg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_rn.json` & `pyg2p-3.2.5/templates/AFFS_rn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_ta.json` & `pyg2p-3.2.5/templates/eud_t24.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9138888888888889%*

 * *Differences: {"'Execution'": "{'@name': 'eud_t24', 'OutMaps': {'@cloneMap': '/dataset/maps/europe5km/dem.map', "*

 * *                "'@ext': 4, '@namePrefix': 'pT24', 'Interpolation': {'@latMap': "*

 * *                "'/dataset/maps/europe5km/lat.map', '@lonMap': "*

 * *                "'/dataset/maps/europe5km/long.map'}}, 'Parameter': {'@demMap': "*

 * *                "'/dataset/maps/dem05.map'}}"}*

```diff
@@ -1,28 +1,28 @@
 {
     "Execution": {
-        "@name": "AFFS_T24",
+        "@name": "eud_t24",
         "Aggregation": {
             "@step": 24,
             "@type": "average"
         },
         "OutMaps": {
-            "@cloneMap": "/dataset/vera/dem_mean.map",
-            "@ext": 1,
+            "@cloneMap": "/dataset/maps/europe5km/dem.map",
+            "@ext": 4,
             "@fmap": 1,
-            "@namePrefix": "ta",
+            "@namePrefix": "pT24",
             "@unitTime": 24,
             "Interpolation": {
-                "@latMap": "/dataset/vera/lat.map",
-                "@lonMap": "/dataset/vera/lon.map",
+                "@latMap": "/dataset/maps/europe5km/lat.map",
+                "@lonMap": "/dataset/maps/europe5km/long.map",
                 "@mode": "grib_nearest"
             }
         },
         "Parameter": {
             "@applyConversion": "k2c",
             "@correctionFormula": "p+gem-dem*0.0065",
-            "@demMap": "/dataset/vera/dem_mean.map",
+            "@demMap": "/dataset/maps/dem05.map",
             "@gem": "(z/9.81)*0.0065",
             "@shortName": "2t"
         }
     }
 }
```

### Comparing `pyg2p-3.2.4/templates/AFFS_td.json` & `pyg2p-3.2.5/templates/AFFS_td.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_wu.json` & `pyg2p-3.2.5/templates/AFFS_wu.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/AFFS_wv.json` & `pyg2p-3.2.5/templates/AFFS_wv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_15d.json` & `pyg2p-3.2.5/templates/EUE_15d.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_15d_glob.json` & `pyg2p-3.2.5/templates/EUE_15d_glob.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim.json` & `pyg2p-3.2.5/templates/EUE_RainAnim.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_CV.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_CV.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_CV_g.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_CV_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_inv.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy_inv.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_CV_scipy_nn.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_CV_scipy_nn.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_agg.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_agg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_december.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_december.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_g.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/EUE_RainAnim_scipy.json` & `pyg2p-3.2.5/templates/EUE_RainAnim_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/UKMO_t24_LA.json` & `pyg2p-3.2.5/templates/UKMO_t24_LA.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/UKMO_t24_LA_g.json` & `pyg2p-3.2.5/templates/UKMO_t24_LA_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/UKMO_t24_LA_scipy.json` & `pyg2p-3.2.5/templates/UKMO_t24_LA_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cin.json` & `pyg2p-3.2.5/templates/cin.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_e06.json` & `pyg2p-3.2.5/templates/cosmo_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_e06_newmaps.json` & `pyg2p-3.2.5/templates/cosmo_e06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_e06_scipy.json` & `pyg2p-3.2.5/templates/cosmo_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_r06.json` & `pyg2p-3.2.5/templates/cosmo_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_r06_newmaps.json` & `pyg2p-3.2.5/templates/cosmo_r06_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_r06_scipy.json` & `pyg2p-3.2.5/templates/cosmo_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_t24.json` & `pyg2p-3.2.5/templates/cosmo_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_t24_newmaps.json` & `pyg2p-3.2.5/templates/cosmo_t24_newmaps.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/cosmo_t24_scipy.json` & `pyg2p-3.2.5/templates/cosmo_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_e06.json` & `pyg2p-3.2.5/templates/dwd_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_e06_2.json` & `pyg2p-3.2.5/templates/dwd_e06_2.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_e06_2nd.json` & `pyg2p-3.2.5/templates/dwd_e06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_e06_3.json` & `pyg2p-3.2.5/templates/dwd_e06_3.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_e06_scipy.json` & `pyg2p-3.2.5/templates/dwd_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_r06.json` & `pyg2p-3.2.5/templates/dwd_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_r06_2nd.json` & `pyg2p-3.2.5/templates/dwd_r06_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_r06_efas.json` & `pyg2p-3.2.5/templates/dwd_r06_efas.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_r06_gmi.json` & `pyg2p-3.2.5/templates/dwd_r06_gmi.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_r06_scipy.json` & `pyg2p-3.2.5/templates/dwd_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_t24.json` & `pyg2p-3.2.5/templates/dwd_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_t24_2nd.json` & `pyg2p-3.2.5/templates/dwd_t24_2nd.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwd_t24_scipy.json` & `pyg2p-3.2.5/templates/dwd_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/dwdl_r06.json` & `pyg2p-3.2.5/templates/dwdl_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/efas_sro.json` & `pyg2p-3.2.5/templates/efas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_e06.json` & `pyg2p-3.2.5/templates/eud_e06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_e06_scipy.json` & `pyg2p-3.2.5/templates/eud_e06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_r06.json` & `pyg2p-3.2.5/templates/eud_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_r06_scipy.json` & `pyg2p-3.2.5/templates/eud_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_r24.json` & `pyg2p-3.2.5/templates/eud_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_r24_scipy.json` & `pyg2p-3.2.5/templates/eud_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eud_t24.json` & `pyg2p-3.2.5/templates/eue_e24_scipy.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8553819444444444%*

 * *Differences: {"'Execution'": "{'@name': 'eue_e', 'Aggregation': {'@type': 'accumulation'}, 'OutMaps': "*

 * *                "{'@namePrefix': 'pE24', 'Interpolation': {'@mode': 'nearest'}, delete: ['@ext']}, "*

 * *                "'Parameter': {'@applyConversion': 'tomm', '@shortName': 'e', delete: "*

 * *                "['@correctionFormula', '@demMap', '@gem']}}"}*

```diff
@@ -1,28 +1,24 @@
 {
     "Execution": {
-        "@name": "eud_t24",
+        "@name": "eue_e",
         "Aggregation": {
             "@step": 24,
-            "@type": "average"
+            "@type": "accumulation"
         },
         "OutMaps": {
             "@cloneMap": "/dataset/maps/europe5km/dem.map",
-            "@ext": 4,
             "@fmap": 1,
-            "@namePrefix": "pT24",
+            "@namePrefix": "pE24",
             "@unitTime": 24,
             "Interpolation": {
                 "@latMap": "/dataset/maps/europe5km/lat.map",
                 "@lonMap": "/dataset/maps/europe5km/long.map",
-                "@mode": "grib_nearest"
+                "@mode": "nearest"
             }
         },
         "Parameter": {
-            "@applyConversion": "k2c",
-            "@correctionFormula": "p+gem-dem*0.0065",
-            "@demMap": "/dataset/maps/dem05.map",
-            "@gem": "(z/9.81)*0.0065",
-            "@shortName": "2t"
+            "@applyConversion": "tomm",
+            "@shortName": "e"
         }
     }
 }
```

### Comparing `pyg2p-3.2.4/templates/eud_t24_scipy.json` & `pyg2p-3.2.5/templates/eud_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_e24.json` & `pyg2p-3.2.5/templates/eue_e24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_e24_scipy.json` & `pyg2p-3.2.5/templates/octahedral_test_scipy_invdist.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9053819444444444%*

 * *Differences: {"'Execution'": "{'@name': 'Octahedral test 1', 'OutMaps': {'@namePrefix': 'tp', 'Interpolation': "*

 * *                "{'@mode': 'invdist'}, '@ext': 1}, 'Parameter': {'@shortName': 'tp'}}"}*

```diff
@@ -1,24 +1,25 @@
 {
     "Execution": {
-        "@name": "eue_e",
+        "@name": "Octahedral test 1",
         "Aggregation": {
             "@step": 24,
             "@type": "accumulation"
         },
         "OutMaps": {
             "@cloneMap": "/dataset/maps/europe5km/dem.map",
+            "@ext": 1,
             "@fmap": 1,
-            "@namePrefix": "pE24",
+            "@namePrefix": "tp",
             "@unitTime": 24,
             "Interpolation": {
                 "@latMap": "/dataset/maps/europe5km/lat.map",
                 "@lonMap": "/dataset/maps/europe5km/long.map",
-                "@mode": "nearest"
+                "@mode": "invdist"
             }
         },
         "Parameter": {
             "@applyConversion": "tomm",
-            "@shortName": "e"
+            "@shortName": "tp"
         }
     }
 }
```

### Comparing `pyg2p-3.2.4/templates/eue_r24.json` & `pyg2p-3.2.5/templates/eue_r24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_r24_15days.json` & `pyg2p-3.2.5/templates/eue_r24_15days.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_r24_15days_g.json` & `pyg2p-3.2.5/templates/eue_r24_15days_g.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_r24_15days_noagg.json` & `pyg2p-3.2.5/templates/eue_r24_15days_noagg.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_r24_15days_scipy.json` & `pyg2p-3.2.5/templates/eue_r24_15days_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_r24_scipy.json` & `pyg2p-3.2.5/templates/eue_r24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_t24.json` & `pyg2p-3.2.5/templates/eue_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/eue_t24_scipy.json` & `pyg2p-3.2.5/templates/eue_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/glofas_sro.json` & `pyg2p-3.2.5/templates/glofas_sro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/glofas_sro_scipy.json` & `pyg2p-3.2.5/templates/glofas_sro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/glofas_ssro.json` & `pyg2p-3.2.5/templates/glofas_ssro.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/glofas_ssro_scipy.json` & `pyg2p-3.2.5/templates/glofas_ssro_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test.json` & `pyg2p-3.2.5/templates/octahedral_test.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_global.json` & `pyg2p-3.2.5/templates/octahedral_test_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_global_invdist.json` & `pyg2p-3.2.5/templates/octahedral_test_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_invdist.json` & `pyg2p-3.2.5/templates/octahedral_test_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_scipy.json` & `pyg2p-3.2.5/templates/octahedral_test_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_scipy_global.json` & `pyg2p-3.2.5/templates/octahedral_test_scipy_global.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_scipy_global_invdist.json` & `pyg2p-3.2.5/templates/octahedral_test_scipy_global_invdist.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/octahedral_test_scipy_invdist.json` & `pyg2p-3.2.5/templates/rn_false_mv.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8784722222222222%*

 * *Differences: {"'Execution'": "{'@name': 'rn false missing values', 'OutMaps': {'@cloneMap': "*

 * *                "'/dataset/maps/global/dem.map', '@namePrefix': 'rnx', 'Interpolation': "*

 * *                "{'@latMap': '/dataset/maps/global/lat.map', '@lonMap': "*

 * *                "'/dataset/maps/global/lon.map'}}, 'Parameter': {'@shortName': 'str', delete: "*

 * *                "['@applyConversion']}}"}*

```diff
@@ -1,25 +1,24 @@
 {
     "Execution": {
-        "@name": "Octahedral test 1",
+        "@name": "rn false missing values",
         "Aggregation": {
             "@step": 24,
             "@type": "accumulation"
         },
         "OutMaps": {
-            "@cloneMap": "/dataset/maps/europe5km/dem.map",
+            "@cloneMap": "/dataset/maps/global/dem.map",
             "@ext": 1,
             "@fmap": 1,
-            "@namePrefix": "tp",
+            "@namePrefix": "rnx",
             "@unitTime": 24,
             "Interpolation": {
-                "@latMap": "/dataset/maps/europe5km/lat.map",
-                "@lonMap": "/dataset/maps/europe5km/long.map",
+                "@latMap": "/dataset/maps/global/lat.map",
+                "@lonMap": "/dataset/maps/global/lon.map",
                 "@mode": "invdist"
             }
         },
         "Parameter": {
-            "@applyConversion": "tomm",
-            "@shortName": "tp"
+            "@shortName": "str"
         }
     }
 }
```

### Comparing `pyg2p-3.2.4/templates/rn_false_mv.json` & `pyg2p-3.2.5/templates/tigge_lam_t24_scipy_rotated.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8509114583333334%*

 * *Differences: {"'Execution'": "{'@name': 'tigge_lam_scipy_t24', 'Aggregation': {'@type': 'average'}, 'OutMaps': "*

 * *                "{'@cloneMap': '/dataset/maps/cosmo/dem05.map', '@namePrefix': 'T24', "*

 * *                "'Interpolation': {'@latMap': '/dataset/maps/cosmo/lat_cosmo5km_new.map', "*

 * *                "'@lonMap': '/dataset/maps/cosmo/lon_cosmo5km_new.map', '@mode': 'nearest', "*

 * *                "'@rotated_target': True}, delete: ['@ext']}, 'Parameter': {'@shortName': '2t', "*

 * *                "'@applyConversion': 'k2 […]*

```diff
@@ -1,24 +1,25 @@
 {
     "Execution": {
-        "@name": "rn false missing values",
+        "@name": "tigge_lam_scipy_t24",
         "Aggregation": {
             "@step": 24,
-            "@type": "accumulation"
+            "@type": "average"
         },
         "OutMaps": {
-            "@cloneMap": "/dataset/maps/global/dem.map",
-            "@ext": 1,
+            "@cloneMap": "/dataset/maps/cosmo/dem05.map",
             "@fmap": 1,
-            "@namePrefix": "rnx",
+            "@namePrefix": "T24",
             "@unitTime": 24,
             "Interpolation": {
-                "@latMap": "/dataset/maps/global/lat.map",
-                "@lonMap": "/dataset/maps/global/lon.map",
-                "@mode": "invdist"
+                "@latMap": "/dataset/maps/cosmo/lat_cosmo5km_new.map",
+                "@lonMap": "/dataset/maps/cosmo/lon_cosmo5km_new.map",
+                "@mode": "nearest",
+                "@rotated_target": true
             }
         },
         "Parameter": {
-            "@shortName": "str"
+            "@applyConversion": "k2c",
+            "@shortName": "2t"
         }
     }
 }
```

### Comparing `pyg2p-3.2.4/templates/tigge_lam_r06.json` & `pyg2p-3.2.5/templates/tigge_lam_r06.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_r06_rotated.json` & `pyg2p-3.2.5/templates/tigge_lam_r06_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_r06_scipy.json` & `pyg2p-3.2.5/templates/tigge_lam_r06_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_r06_scipy_rotated.json` & `pyg2p-3.2.5/templates/tigge_lam_r06_scipy_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_t24.json` & `pyg2p-3.2.5/templates/tigge_lam_t24.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_t24_rotated.json` & `pyg2p-3.2.5/templates/tigge_lam_t24_rotated.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/templates/tigge_lam_t24_scipy.json` & `pyg2p-3.2.5/templates/tigge_lam_t24_scipy.json`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_aggregator.py` & `pyg2p-3.2.5/tests/test_aggregator.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_api.py` & `pyg2p-3.2.5/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_conversion.py` & `pyg2p-3.2.5/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_correction.py` & `pyg2p-3.2.5/tests/test_correction.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_interpolation.py` & `pyg2p-3.2.5/tests/test_interpolation.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,35 @@
         lats, lons = messages.latlons
         values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
         shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
         assert shape_target == values_resampled.shape
         os.unlink('tests/data/tbl_pf10tp_550800_scipy_invdist.npy.gz')
 
     @pytest.mark.slow
+    def test_interpolation_create_scipy_adw(self):
+        d = deepcopy(config_dict)
+        d['interpolation.create'] = True
+        d['interpolation.parallel'] = True
+        d['interpolation.mode'] = 'adw'
+        d['interpolation.adw_broadcasting'] = True
+        file = d['input.file']
+        reader = GRIBReader(file)
+        messages = reader.select_messages(shortName='2t')
+        grid_id = messages.grid_id
+        missing = messages.missing_value
+        ctx = MockedExecutionContext(d, False)
+        interpolator = Interpolator(ctx, missing)
+        values_in = messages.values_first_or_single_res[messages.first_step_range]
+        lats, lons = messages.latlons
+        values_resampled = interpolator.interpolate_scipy(lats, lons, values_in, grid_id, messages.grid_details)
+        shape_target = PCRasterReader(d['interpolation.latMap']).values.shape
+        assert shape_target == values_resampled.shape
+        os.unlink('tests/data/tbl_pf10tp_550800_scipy_adw.npy.gz')
+
+    @pytest.mark.slow
     def test_interpolation_create_scipy_bilinear(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
         d['interpolation.parallel'] = True
         d['interpolation.mode'] = 'bilinear'
         # # Test on era5 grib map in NetCDF format
         d['interpolation.lonMap'] = 'tests/data/template_test.nc'
@@ -120,15 +141,15 @@
         assert shape_target == values_resampled.shape
         os.unlink('tests/data/tbl_era5t2avg_441_scipy_bilinear_delaunay.npy.gz')
 
     @pytest.mark.slow
     def test_interpolation_create_eccodes_nearest(self):
         d = deepcopy(config_dict)
         d['interpolation.create'] = True
-        d['interpolation.parallel'] = True
+        d['interpolation.parallel'] = False
         d['interpolation.mode'] = 'grib_nearest'
         file = d['input.file']
         reader = GRIBReader(file)
         messages = reader.select_messages(shortName='2t')
         grid_id = messages.grid_id
         missing = messages.missing_value
         ctx = MockedExecutionContext(d, True)
```

### Comparing `pyg2p-3.2.4/tests/test_oracle_data.py` & `pyg2p-3.2.5/tests/test_oracle_data.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_readers.py` & `pyg2p-3.2.5/tests/test_readers.py`

 * *Files identical despite different names*

### Comparing `pyg2p-3.2.4/tests/test_strings.py` & `pyg2p-3.2.5/tests/test_strings.py`

 * *Files identical despite different names*

