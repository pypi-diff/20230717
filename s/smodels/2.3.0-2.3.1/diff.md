# Comparing `tmp/smodels-2.3.0.tar.gz` & `tmp/smodels-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smodels-2.3.0.tar", last modified: Tue May 23 18:30:00 2023, max compression
+gzip compressed data, was "smodels-2.3.1.tar", last modified: Mon Jul 17 12:33:30 2023, max compression
```

## Comparing `smodels-2.3.0.tar` & `smodels-2.3.1.tar`

### file list

```diff
@@ -1,222 +1,281 @@
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.665647 smodels-2.3.0/
--rw-r--r--   0 walten    (1000) walten    (1000)      248 2023-05-06 11:20:28.000000 smodels-2.3.0/MANIFEST.in
--rw-r--r--   0 walten    (1000) walten    (1000)     2686 2023-05-06 11:20:28.000000 smodels-2.3.0/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)     4548 2023-05-23 18:30:00.665647 smodels-2.3.0/PKG-INFO
--rw-r--r--   0 walten    (1000) walten    (1000)     3567 2023-05-06 11:20:28.000000 smodels-2.3.0/README.rst
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.641647 smodels-2.3.0/inputFiles/
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.642647 smodels-2.3.0/inputFiles/lhe/
--rw-r--r--   0 walten    (1000) walten    (1000)    28882 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/lhe/gluino_squarks.lhe
--rw-r--r--   0 walten    (1000) walten    (1000)     7317 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/lhe/simplyGluino.lhe
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.643647 smodels-2.3.0/inputFiles/scanExample/
--rw-r--r--   0 walten    (1000) walten    (1000)  1046891 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/scanExample/slhas.tar.gz
--rw-r--r--   0 walten    (1000) walten    (1000)   400983 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/scanExample/smodels-output.tar.gz
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.644647 smodels-2.3.0/inputFiles/scanExampleIDM/
--rw-r--r--   0 walten    (1000) walten    (1000)    31786 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/scanExampleIDM/slhas.tar.gz
--rw-r--r--   0 walten    (1000) walten    (1000)    13168 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/scanExampleIDM/smodels-output.tar.gz
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.645647 smodels-2.3.0/inputFiles/slha/
--rw-r--r--   0 walten    (1000) walten    (1000)   105311 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/complicated.slha
--rw-r--r--   0 walten    (1000) walten    (1000)     9815 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/gluinoToTops.slha
--rw-r--r--   0 walten    (1000) walten    (1000)   105959 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/gluino_squarks.slha
--rw-r--r--   0 walten    (1000) walten    (1000)    47731 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/higgsinoStop.slha
--rw-r--r--   0 walten    (1000) walten    (1000)     7475 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/idm_example.slha
--rw-r--r--   0 walten    (1000) walten    (1000)    50317 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/lightEWinos.slha
--rw-r--r--   0 walten    (1000) walten    (1000)    99924 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/longLived.slha
--rw-r--r--   0 walten    (1000) walten    (1000)    12261 2023-05-06 11:20:28.000000 smodels-2.3.0/inputFiles/slha/simplyGluino.slha
--rw-r--r--   0 walten    (1000) walten    (1000)       80 2023-05-23 18:30:00.666647 smodels-2.3.0/setup.cfg
--rwxr-xr-x   0 walten    (1000) walten    (1000)     5297 2023-05-06 11:20:28.000000 smodels-2.3.0/setup.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.645647 smodels-2.3.0/smodels/
--rw-r--r--   0 walten    (1000) walten    (1000)      801 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/COPYING
--rw-r--r--   0 walten    (1000) walten    (1000)      326 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/INSTALLATION.rst
--rw-r--r--   0 walten    (1000) walten    (1000)     3567 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/README.rst
--rw-r--r--   0 walten    (1000) walten    (1000)       59 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/__init__.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.646647 smodels-2.3.0/smodels/etc/
--rw-r--r--   0 walten    (1000) walten    (1000)      636 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/logging.conf
--rw-r--r--   0 walten    (1000) walten    (1000)      374 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/logging_consoleonly.conf
--rw-r--r--   0 walten    (1000) walten    (1000)      636 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/logging_file.conf
--rw-r--r--   0 walten    (1000) walten    (1000)      735 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/parameters_default.ini
--rw-r--r--   0 walten    (1000) walten    (1000)      613 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/pythia.card
--rw-r--r--   0 walten    (1000) walten    (1000)     2613 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/etc/pythia8.cfg
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.647647 smodels-2.3.0/smodels/experiment/
--rw-r--r--   0 walten    (1000) walten    (1000)      163 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/__init__.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    52484 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/databaseObj.py
--rw-r--r--   0 walten    (1000) walten    (1000)    19004 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/datasetObj.py
--rw-r--r--   0 walten    (1000) walten    (1000)     7934 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/defaultFinalStates.py
--rw-r--r--   0 walten    (1000) walten    (1000)      767 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/exceptions.py
--rw-r--r--   0 walten    (1000) walten    (1000)    11905 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/expResultObj.py
--rw-r--r--   0 walten    (1000) walten    (1000)     4195 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/infoObj.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     7667 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/metaObj.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    45349 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/experiment/txnameObj.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     9275 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/installation.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.647647 smodels-2.3.0/smodels/lib/
--rw-r--r--   0 walten    (1000) walten    (1000)      723 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/Makefile
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.647647 smodels-2.3.0/smodels/lib/nllfast/
--rw-r--r--   0 walten    (1000) walten    (1000)      338 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/Makefile
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.649647 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/
--rw-r--r--   0 walten    (1000) walten    (1000)      248 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)    14381 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    14014 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    48613 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    53903 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    55237 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    56001 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    28310 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/nllfast-1.2.f
--rwxr-xr-x   0 walten    (1000) walten    (1000)    46736 2023-05-06 11:23:14.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/nllfast_7TeV
--rw-r--r--   0 walten    (1000) walten    (1000)    48612 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    55581 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     5588 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     5548 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    48612 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    31981 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    32933 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    55488 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    48611 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    55945 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3567 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3181 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    48973 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    56209 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_mstw2008.grid
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.651647 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/
--rw-r--r--   0 walten    (1000) walten    (1000)      248 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)     3527 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3527 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    63818 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    63820 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    28021 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/nllfast-2.1.f
--rwxr-xr-x   0 walten    (1000) walten    (1000)    46736 2023-05-06 11:23:14.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/nllfast_8TeV
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3359 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3359 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    63818 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    63818 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    76410 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_mstw2008.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     5439 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_cteq6.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     5438 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_mstw2008.grid
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.655647 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/
--rw-r--r--   0 walten    (1000) walten    (1000)      249 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)     4110 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     4110 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3589 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    77779 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    77158 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    66718 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    96447 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    36172 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/nllfast-3.1-13TeV.f
--rwxr-xr-x   0 walten    (1000) walten    (1000)    63160 2023-05-06 11:23:14.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/nllfast_13TeV
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    96447 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     4165 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     4165 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     3645 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    77779 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    77779 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    66718 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    96447 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)   111585 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)    96447 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_nnpdf30_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     6153 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_cteq66_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     6153 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_mstw2008_13TeV.grid
--rw-r--r--   0 walten    (1000) walten    (1000)     5710 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_nnpdf30_13TeV.grid
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.660647 smodels-2.3.0/smodels/lib/pythia6/
--rw-r--r--   0 walten    (1000) walten    (1000)      338 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia6/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)  2877981 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia6/pythia-6.4.27.f
--rwxr-xr-x   0 walten    (1000) walten    (1000)  3928432 2023-05-06 11:21:34.000000 smodels-2.3.0/smodels/lib/pythia6/pythia_lhe
--rw-r--r--   0 walten    (1000) walten    (1000)     1884 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia6/pythia_lhe.f
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.660647 smodels-2.3.0/smodels/lib/pythia8/
--rw-r--r--   0 walten    (1000) walten    (1000)     1266 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia8/Makefile
--rwxr-xr-x   0 walten    (1000) walten    (1000)     5930 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia8/installer.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     3143 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia8/parseXml.py
--rw-r--r--   0 walten    (1000) walten    (1000)     3983 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia8/pythia8.cc
--rwxr-xr-x   0 walten    (1000) walten    (1000)   133192 2023-05-17 16:33:40.000000 smodels-2.3.0/smodels/lib/pythia8/pythia8.exe
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.660647 smodels-2.3.0/smodels/lib/pythia8/pythia8308/
--rw-r--r--   0 walten    (1000) walten    (1000)     5459 2022-11-18 15:51:04.000000 smodels-2.3.0/smodels/lib/pythia8/pythia8308/Makefile
--rw-r--r--   0 walten    (1000) walten    (1000)        5 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/lib/pythia8/pythiaversion
--rwxr-xr-x   0 walten    (1000) walten    (1000)       33 2023-05-17 16:33:36.000000 smodels-2.3.0/smodels/lib/pythia8/xml.doc
--rw-r--r--   0 walten    (1000) walten    (1000)     5665 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/particlesLoader.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.660647 smodels-2.3.0/smodels/share/
--rw-r--r--   0 walten    (1000) walten    (1000)      897 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/BANNER
--rw-r--r--   0 walten    (1000) walten    (1000)      105 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/__init__.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.661647 smodels-2.3.0/smodels/share/models/
--rw-r--r--   0 walten    (1000) walten    (1000)     4828 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/SMparticles.py
--rw-r--r--   0 walten    (1000) walten    (1000)        0 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/__init__.py
--rw-r--r--   0 walten    (1000) walten    (1000)     5249 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/dgmssm.py
--rw-r--r--   0 walten    (1000) walten    (1000)      861 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/idm.py
--rw-r--r--   0 walten    (1000) walten    (1000)     4019 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/mssm.py
--rw-r--r--   0 walten    (1000) walten    (1000)    10429 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/mssmQNumbers.slha
--rw-r--r--   0 walten    (1000) walten    (1000)     4309 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/models/nmssm.py
--rw-r--r--   0 walten    (1000) walten    (1000)     2594 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/pythia_test.card
--rw-r--r--   0 walten    (1000) walten    (1000)      138 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/share/requirements.txt
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.662647 smodels-2.3.0/smodels/theory/
--rw-r--r--   0 walten    (1000) walten    (1000)      297 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/__init__.py
--rw-r--r--   0 walten    (1000) walten    (1000)    17717 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/auxiliaryFunctions.py
--rw-r--r--   0 walten    (1000) walten    (1000)    20140 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/branch.py
--rw-r--r--   0 walten    (1000) walten    (1000)    19578 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/clusterTools.py
--rw-r--r--   0 walten    (1000) walten    (1000)    23064 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/crossSection.py
--rw-r--r--   0 walten    (1000) walten    (1000)     5464 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/decomposer.py
--rw-r--r--   0 walten    (1000) walten    (1000)    22973 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/element.py
--rw-r--r--   0 walten    (1000) walten    (1000)      414 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/exceptions.py
--rw-r--r--   0 walten    (1000) walten    (1000)    11628 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/lheReader.py
--rw-r--r--   0 walten    (1000) walten    (1000)    18087 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/model.py
--rw-r--r--   0 walten    (1000) walten    (1000)    23761 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/particle.py
--rw-r--r--   0 walten    (1000) walten    (1000)    39837 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/theory/theoryPrediction.py
--rw-r--r--   0 walten    (1000) walten    (1000)    11625 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/theory/topology.py
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.665647 smodels-2.3.0/smodels/tools/
--rw-r--r--   0 walten    (1000) walten    (1000)      144 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/__init__.py
--rw-r--r--   0 walten    (1000) walten    (1000)    12991 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/tools/analysesCombinations.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     3861 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/asciiGraph.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     5847 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/tools/basicStats.py
--rw-r--r--   0 walten    (1000) walten    (1000)     2583 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/caching.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     1420 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/colors.py
--rw-r--r--   0 walten    (1000) walten    (1000)    19783 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/coverage.py
--rw-r--r--   0 walten    (1000) walten    (1000)     5604 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/crashReport.py
--rw-r--r--   0 walten    (1000) walten    (1000)    10841 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/databaseBrowser.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    11259 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/databaseClient.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     9646 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/databaseServer.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     2984 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/externalPythonTools.py
--rw-r--r--   0 walten    (1000) walten    (1000)     1375 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/inclusiveObjects.py
--rw-r--r--   0 walten    (1000) walten    (1000)    20468 2023-05-07 13:26:20.000000 smodels-2.3.0/smodels/tools/interactivePlots.py
--rw-r--r--   0 walten    (1000) walten    (1000)    41552 2023-05-07 13:03:13.000000 smodels-2.3.0/smodels/tools/interactivePlotsHelpers.py
--rw-r--r--   0 walten    (1000) walten    (1000)    12373 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/ioObjects.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)      317 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/lheChecks.py
--rw-r--r--   0 walten    (1000) walten    (1000)    23437 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/modelTester.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    13536 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/nllFastWrapper.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     1502 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/physicsUnits.py
--rw-r--r--   0 walten    (1000) walten    (1000)    69079 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/printer.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     4492 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/proxyDBCreator.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    46842 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/tools/pyhfInterface.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    10581 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/pythia6Wrapper.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     8883 2023-05-09 15:42:10.000000 smodels-2.3.0/smodels/tools/pythia8Wrapper.py
--rw-r--r--   0 walten    (1000) walten    (1000)    16770 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/pythia8particles.py
--rw-r--r--   0 walten    (1000) walten    (1000)     8082 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/reweighting.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     5229 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/runSModelS.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     2351 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/runtime.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    43989 2023-05-23 18:22:30.000000 smodels-2.3.0/smodels/tools/simplifiedLikelihoods.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)      604 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/slhaChecks.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     3179 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/smodelsLogging.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     9054 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/smodelsTools.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    19114 2023-05-08 18:53:14.000000 smodels-2.3.0/smodels/tools/statsTools.py
--rw-r--r--   0 walten    (1000) walten    (1000)     1378 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/stringTools.py
--rw-r--r--   0 walten    (1000) walten    (1000)     1174 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/timeOut.py
--rw-r--r--   0 walten    (1000) walten    (1000)     4373 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/toolBox.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)     9675 2023-05-08 18:53:14.000000 smodels-2.3.0/smodels/tools/truncatedGaussians.py
--rw-r--r--   0 walten    (1000) walten    (1000)     5098 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/wrapperBase.py
--rwxr-xr-x   0 walten    (1000) walten    (1000)    26772 2023-05-06 11:20:28.000000 smodels-2.3.0/smodels/tools/xsecComputer.py
--rw-r--r--   0 walten    (1000) walten    (1000)        6 2023-05-09 15:55:44.000000 smodels-2.3.0/smodels/version
-drwxr-xr-x   0 walten    (1000) walten    (1000)        0 2023-05-23 18:30:00.646647 smodels-2.3.0/smodels.egg-info/
--rw-r--r--   0 walten    (1000) walten    (1000)     4548 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/PKG-INFO
--rw-r--r--   0 walten    (1000) walten    (1000)     7928 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/SOURCES.txt
--rw-r--r--   0 walten    (1000) walten    (1000)        1 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/dependency_links.txt
--rw-r--r--   0 walten    (1000) walten    (1000)      157 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/entry_points.txt
--rw-r--r--   0 walten    (1000) walten    (1000)      138 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/requires.txt
--rw-r--r--   0 walten    (1000) walten    (1000)        8 2023-05-23 18:30:00.000000 smodels-2.3.0/smodels.egg-info/top_level.txt
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.598593 smodels-2.3.1/
+-rw-r--r--   0 walten    (1001) walten    (1001)      248 2022-10-18 14:32:06.000000 smodels-2.3.1/MANIFEST.in
+-rw-r--r--   0 walten    (1001) walten    (1001)     2686 2022-10-18 14:32:06.000000 smodels-2.3.1/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)     4548 2023-07-17 12:33:30.598593 smodels-2.3.1/PKG-INFO
+-rw-r--r--   0 walten    (1001) walten    (1001)     3567 2023-05-10 12:04:45.000000 smodels-2.3.1/README.rst
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.542592 smodels-2.3.1/inputFiles/
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.546592 smodels-2.3.1/inputFiles/lhe/
+-rw-r--r--   0 walten    (1001) walten    (1001)    28882 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/lhe/gluino_squarks.lhe
+-rw-r--r--   0 walten    (1001) walten    (1001)     7317 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/lhe/simplyGluino.lhe
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.546592 smodels-2.3.1/inputFiles/scanExample/
+-rw-r--r--   0 walten    (1001) walten    (1001)  1046891 2023-01-19 16:20:50.000000 smodels-2.3.1/inputFiles/scanExample/slhas.tar.gz
+-rw-r--r--   0 walten    (1001) walten    (1001)   400983 2023-01-19 16:20:50.000000 smodels-2.3.1/inputFiles/scanExample/smodels-output.tar.gz
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.546592 smodels-2.3.1/inputFiles/scanExampleIDM/
+-rw-r--r--   0 walten    (1001) walten    (1001)    31786 2023-01-19 16:20:50.000000 smodels-2.3.1/inputFiles/scanExampleIDM/slhas.tar.gz
+-rw-r--r--   0 walten    (1001) walten    (1001)    13168 2023-01-19 16:20:50.000000 smodels-2.3.1/inputFiles/scanExampleIDM/smodels-output.tar.gz
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.550592 smodels-2.3.1/inputFiles/slha/
+-rw-r--r--   0 walten    (1001) walten    (1001)   105311 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/complicated.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)    31467 2023-07-17 09:00:32.000000 smodels-2.3.1/inputFiles/slha/ew_ymi2l51r.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)     9815 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/gluinoToTops.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)   105959 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/gluino_squarks.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)    47731 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/higgsinoStop.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)     7475 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/idm_example.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)    50317 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/lightEWinos.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)    99924 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/longLived.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)    12261 2022-10-18 14:32:06.000000 smodels-2.3.1/inputFiles/slha/simplyGluino.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)       80 2023-07-17 12:33:30.598593 smodels-2.3.1/setup.cfg
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5297 2023-01-19 16:20:50.000000 smodels-2.3.1/setup.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.550592 smodels-2.3.1/smodels/
+-rw-r--r--   0 walten    (1001) walten    (1001)      801 2023-05-23 12:39:50.000000 smodels-2.3.1/smodels/COPYING
+-rw-r--r--   0 walten    (1001) walten    (1001)      326 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/INSTALLATION.rst
+-rw-r--r--   0 walten    (1001) walten    (1001)     3567 2023-05-10 12:04:45.000000 smodels-2.3.1/smodels/README.rst
+-rw-r--r--   0 walten    (1001) walten    (1001)       59 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/__init__.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.550592 smodels-2.3.1/smodels/etc/
+-rw-r--r--   0 walten    (1001) walten    (1001)      636 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/logging.conf
+-rw-r--r--   0 walten    (1001) walten    (1001)      374 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/logging_consoleonly.conf
+-rw-r--r--   0 walten    (1001) walten    (1001)      636 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/logging_file.conf
+-rw-r--r--   0 walten    (1001) walten    (1001)      735 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/parameters_default.ini
+-rw-r--r--   0 walten    (1001) walten    (1001)      613 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/pythia.card
+-rw-r--r--   0 walten    (1001) walten    (1001)     2613 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/etc/pythia8.cfg
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.554592 smodels-2.3.1/smodels/experiment/
+-rw-r--r--   0 walten    (1001) walten    (1001)      163 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/experiment/__init__.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    52484 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/experiment/databaseObj.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    19968 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/experiment/datasetObj.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     7934 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/experiment/defaultFinalStates.py
+-rw-r--r--   0 walten    (1001) walten    (1001)      767 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/experiment/exceptions.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    11905 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/experiment/expResultObj.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     4195 2023-02-13 11:16:24.000000 smodels-2.3.1/smodels/experiment/infoObj.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     7691 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/experiment/metaObj.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    45349 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/experiment/txnameObj.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9275 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/installation.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.554592 smodels-2.3.1/smodels/lib/
+-rw-r--r--   0 walten    (1001) walten    (1001)      723 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/Makefile
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.554592 smodels-2.3.1/smodels/lib/nllfast/
+-rw-r--r--   0 walten    (1001) walten    (1001)      338 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/Makefile
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.558592 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/
+-rw-r--r--   0 walten    (1001) walten    (1001)      248 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)    14381 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    14014 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    48613 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    53903 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    55237 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    56001 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    28310 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/nllfast-1.2.f
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    46736 2022-11-15 13:14:36.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/nllfast_7TeV
+-rw-r--r--   0 walten    (1001) walten    (1001)    48612 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    55581 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     5588 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     5548 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    48612 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    31981 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    32933 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    55488 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    48611 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    55945 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3567 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3181 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    48973 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    56209 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_mstw2008.grid
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.562593 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/
+-rw-r--r--   0 walten    (1001) walten    (1001)      248 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)     3527 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3527 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    63818 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    63820 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    28021 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/nllfast-2.1.f
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    46736 2022-11-15 13:14:37.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/nllfast_8TeV
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3359 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3359 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    63818 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    63818 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    76410 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_mstw2008.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     5439 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_cteq6.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     5438 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_mstw2008.grid
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.570593 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/
+-rw-r--r--   0 walten    (1001) walten    (1001)      249 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)     4110 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     4110 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3589 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    77779 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    77158 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    66718 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    96447 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    36172 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/nllfast-3.1-13TeV.f
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    63160 2022-11-15 13:14:37.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/nllfast_13TeV
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    96447 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     4165 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     4165 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     3645 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    77779 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    77779 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    66718 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    96447 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)   111585 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)    96447 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_nnpdf30_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     6153 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_cteq66_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     6153 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_mstw2008_13TeV.grid
+-rw-r--r--   0 walten    (1001) walten    (1001)     5710 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_nnpdf30_13TeV.grid
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.578593 smodels-2.3.1/smodels/lib/pythia6/
+-rw-r--r--   0 walten    (1001) walten    (1001)      452 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/lib/pythia6/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)  2877981 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/pythia6/pythia-6.4.27.f
+-rwxr-xr-x   0 walten    (1001) walten    (1001)  3928432 2022-11-15 13:09:27.000000 smodels-2.3.1/smodels/lib/pythia6/pythia_lhe
+-rw-r--r--   0 walten    (1001) walten    (1001)     1884 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/lib/pythia6/pythia_lhe.f
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.578593 smodels-2.3.1/smodels/lib/pythia8/
+-rw-r--r--   0 walten    (1001) walten    (1001)     1266 2023-05-03 14:18:09.000000 smodels-2.3.1/smodels/lib/pythia8/Makefile
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5930 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/lib/pythia8/installer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3143 2023-05-03 14:18:09.000000 smodels-2.3.1/smodels/lib/pythia8/parseXml.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     3983 2023-05-03 14:18:09.000000 smodels-2.3.1/smodels/lib/pythia8/pythia8.cc
+-rwxr-xr-x   0 walten    (1001) walten    (1001)   133192 2023-05-10 12:18:03.000000 smodels-2.3.1/smodels/lib/pythia8/pythia8.exe
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.578593 smodels-2.3.1/smodels/lib/pythia8/pythia8308/
+-rw-r--r--   0 walten    (1001) walten    (1001)     5459 2022-11-18 15:51:04.000000 smodels-2.3.1/smodels/lib/pythia8/pythia8308/Makefile
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.578593 smodels-2.3.1/smodels/lib/pythia8/pythia8309/
+-rw-r--r--   0 walten    (1001) walten    (1001)     5575 2023-02-16 17:12:45.000000 smodels-2.3.1/smodels/lib/pythia8/pythia8309/Makefile
+-rw-r--r--   0 walten    (1001) walten    (1001)        5 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/lib/pythia8/pythiaversion
+-rwxr-xr-x   0 walten    (1001) walten    (1001)       33 2023-05-10 12:17:57.000000 smodels-2.3.1/smodels/lib/pythia8/xml.doc
+-rw-r--r--   0 walten    (1001) walten    (1001)     6459 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/particlesLoader.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.578593 smodels-2.3.1/smodels/share/
+-rw-r--r--   0 walten    (1001) walten    (1001)      897 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/share/BANNER
+-rw-r--r--   0 walten    (1001) walten    (1001)   770744 2023-06-27 12:28:11.000000 smodels-2.3.1/smodels/share/LHAPDF-6.3.0.tar.gz
+-rw-r--r--   0 walten    (1001) walten    (1001)      105 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/share/__init__.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.582593 smodels-2.3.1/smodels/share/models/
+-rw-r--r--   0 walten    (1001) walten    (1001)     4828 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/share/models/SMparticles.py
+-rw-r--r--   0 walten    (1001) walten    (1001)        0 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/share/models/__init__.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     5249 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/share/models/dgmssm.py
+-rw-r--r--   0 walten    (1001) walten    (1001)      861 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/share/models/idm.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     4019 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/share/models/mssm.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    10429 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/share/models/mssmQNumbers.slha
+-rw-r--r--   0 walten    (1001) walten    (1001)     4309 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/share/models/nmssm.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     2594 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/share/pythia_test.card
+-rw-r--r--   0 walten    (1001) walten    (1001)      138 2023-02-13 15:32:46.000000 smodels-2.3.1/smodels/share/requirements.txt
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.582593 smodels-2.3.1/smodels/theory/
+-rw-r--r--   0 walten    (1001) walten    (1001)      297 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/__init__.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    17717 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/auxiliaryFunctions.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    20140 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/branch.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    19578 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/theory/clusterTools.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    23064 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/crossSection.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     5464 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/decomposer.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    22973 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/element.py
+-rw-r--r--   0 walten    (1001) walten    (1001)      414 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/exceptions.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    11628 2023-05-10 12:04:45.000000 smodels-2.3.1/smodels/theory/lheReader.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    18148 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/theory/model.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    23761 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/theory/particle.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    40415 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/theory/theoryPrediction.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    11625 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/theory/topology.py
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.590593 smodels-2.3.1/smodels/tools/
+-rw-r--r--   0 walten    (1001) walten    (1001)      144 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/tools/__init__.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    13077 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/analysesCombinations.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3861 2023-05-08 10:25:26.000000 smodels-2.3.1/smodels/tools/asciiGraph.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5907 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/basicStats.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     2583 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/caching.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1420 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/colors.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    19783 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/coverage.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     5604 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/crashReport.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    10841 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/databaseBrowser.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    11259 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/databaseClient.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9646 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/databaseServer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2984 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/externalPythonTools.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     1375 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/inclusiveObjects.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    20468 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/tools/interactivePlots.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    41552 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/tools/interactivePlotsHelpers.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    12373 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/ioObjects.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      317 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/tools/lheChecks.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    23437 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/tools/modelTester.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    13536 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/nllFastWrapper.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1502 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/physicsUnits.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    69079 2023-05-10 12:04:57.000000 smodels-2.3.1/smodels/tools/printer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4492 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/tools/proxyDBCreator.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    47243 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/pyhfInterface.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    10575 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/pythia6Wrapper.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9240 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/pythia8Wrapper.py
+-rw-r--r--   0 walten    (1001) walten    (1001)    16770 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/tools/pythia8particles.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     8082 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/reweighting.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5235 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/runSModelS.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2899 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/runtime.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    43989 2023-07-10 09:09:45.000000 smodels-2.3.1/smodels/tools/simplifiedLikelihoods.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      604 2022-10-18 14:32:06.000000 smodels-2.3.1/smodels/tools/slhaChecks.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3179 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/smodelsLogging.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9190 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/smodelsTools.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    19495 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/statsTools.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     1378 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/stringTools.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     1174 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/timeOut.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     4373 2023-01-19 16:20:50.000000 smodels-2.3.1/smodels/tools/toolBox.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    10540 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/truncatedGaussians.py
+-rw-r--r--   0 walten    (1001) walten    (1001)     5118 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/wrapperBase.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    27143 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/tools/xsecComputer.py
+-rw-r--r--   0 walten    (1001) walten    (1001)        6 2023-07-17 09:00:32.000000 smodels-2.3.1/smodels/version
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.550592 smodels-2.3.1/smodels.egg-info/
+-rw-r--r--   0 walten    (1001) walten    (1001)     4548 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/PKG-INFO
+-rw-r--r--   0 walten    (1001) walten    (1001)     9259 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/SOURCES.txt
+-rw-r--r--   0 walten    (1001) walten    (1001)        1 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/dependency_links.txt
+-rw-r--r--   0 walten    (1001) walten    (1001)      157 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/entry_points.txt
+-rw-r--r--   0 walten    (1001) walten    (1001)      138 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/requires.txt
+-rw-r--r--   0 walten    (1001) walten    (1001)        8 2023-07-17 12:33:30.000000 smodels-2.3.1/smodels.egg-info/top_level.txt
+drwxr-xr-x   0 walten    (1001) walten    (1001)        0 2023-07-17 12:33:30.598593 smodels-2.3.1/test/
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2402 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testAdditiveDB.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1237 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testAsciiGraph.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5359 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testBranch.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1248 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCaching.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    13619 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testClusterer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2581 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCombined.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3257 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCompression.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1272 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testConditions.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4756 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCorrelations.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     8832 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCoverage.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4208 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testCpp.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2235 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testDatabase.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9857 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testDecomposer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4979 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testDetectorSize.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9218 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testElement.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1680 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testElementID.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      704 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testElementsInStr.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2356 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testExtrapolation.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1115 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testFinalStates.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     7156 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testInclusiveObjects.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2870 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testInteractivePlots.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4286 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testIntermediateState.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     8331 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testInterpolation.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2337 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testInterpolation1D.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4938 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testLHEReader.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1016 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testLoadDBParticles.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1872 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testModelQNumbers.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     7783 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testModels.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4702 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testMoreSL.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1403 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testNllFast.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     5296 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testParticle.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      777 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testPhysicsUnits.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    10063 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testPrinter.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    13189 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testPyhf.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3211 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testPythia.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1541 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testReportAll.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2127 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testReweighting.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    11924 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testRunSModelS.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      864 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testRuntime.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     7676 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testSL.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1937 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testScanSummary.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3646 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testServer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      603 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testSlhaChecks.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)    25107 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testStatistics.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     9385 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTheoryPredCombinations.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     4298 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTheoryPrediction.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)      596 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testToolBox.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     6851 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTopoComb.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     3210 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTopology.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1251 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTx.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     8656 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testTxname.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     1551 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testUpperLimit.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     8943 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testXSecComputer.py
+-rwxr-xr-x   0 walten    (1001) walten    (1001)     2033 2023-07-17 12:27:35.000000 smodels-2.3.1/test/testZRecipes.py
```

### Comparing `smodels-2.3.0/Makefile` & `smodels-2.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/PKG-INFO` & `smodels-2.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smodels
-Version: 2.3.0
+Version: 2.3.1
 Summary: A tool for interpreting simplified-model results from the LHC
 Home-page: https://smodels.github.io/
 Author: The SModelS collaboration, smodels-users@lists.oeaw.ac.at Current members: Mohammad Mahdi Altakach, Sabine Kraml, Andre Lessa, Sahana Narashima, Timothee Pascal, Humberto Reyes-Gonzalez, Wolfgang Waltenberger  Previously involved in SModelS: Gael Alguero, Federico Ambrogi, Juhi Dutta, Jan Heisig, Charanjit K. Khosa, Suchita Kulkarni, Ursula Laa, Veronika Magerl, Wolfgang Magerl, Philipp Neuhuber, Doris Proschofsky, Jory Sonneveld, Michael Traub, Matthias Wolf, Alicia Wongel
 Author-email: smodels-developers@lists.oeaw.ac.at 
 License: GPLv3
 Keywords: simplified models LHC BSM theories interpretation supersymmetry UEDs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `smodels-2.3.0/README.rst` & `smodels-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/lhe/gluino_squarks.lhe` & `smodels-2.3.1/inputFiles/lhe/gluino_squarks.lhe`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/lhe/simplyGluino.lhe` & `smodels-2.3.1/inputFiles/lhe/simplyGluino.lhe`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/scanExample/slhas.tar.gz` & `smodels-2.3.1/inputFiles/scanExample/slhas.tar.gz`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/scanExample/smodels-output.tar.gz` & `smodels-2.3.1/inputFiles/scanExample/smodels-output.tar.gz`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/scanExampleIDM/slhas.tar.gz` & `smodels-2.3.1/inputFiles/scanExampleIDM/slhas.tar.gz`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/scanExampleIDM/smodels-output.tar.gz` & `smodels-2.3.1/inputFiles/scanExampleIDM/smodels-output.tar.gz`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/complicated.slha` & `smodels-2.3.1/inputFiles/slha/complicated.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/gluinoToTops.slha` & `smodels-2.3.1/inputFiles/slha/gluinoToTops.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/gluino_squarks.slha` & `smodels-2.3.1/inputFiles/slha/gluino_squarks.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/higgsinoStop.slha` & `smodels-2.3.1/inputFiles/slha/higgsinoStop.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/idm_example.slha` & `smodels-2.3.1/inputFiles/slha/idm_example.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/lightEWinos.slha` & `smodels-2.3.1/inputFiles/slha/lightEWinos.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/longLived.slha` & `smodels-2.3.1/inputFiles/slha/longLived.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/inputFiles/slha/simplyGluino.slha` & `smodels-2.3.1/inputFiles/slha/simplyGluino.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/setup.py` & `smodels-2.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/COPYING` & `smodels-2.3.1/smodels/COPYING`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/README.rst` & `smodels-2.3.1/smodels/README.rst`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/etc/logging.conf` & `smodels-2.3.1/smodels/etc/logging.conf`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/etc/logging_file.conf` & `smodels-2.3.1/smodels/etc/logging_file.conf`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/etc/parameters_default.ini` & `smodels-2.3.1/smodels/etc/parameters_default.ini`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/etc/pythia.card` & `smodels-2.3.1/smodels/etc/pythia.card`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/etc/pythia8.cfg` & `smodels-2.3.1/smodels/etc/pythia8.cfg`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/databaseObj.py` & `smodels-2.3.1/smodels/experiment/databaseObj.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/datasetObj.py` & `smodels-2.3.1/smodels/experiment/datasetObj.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,22 @@
 
     def isCombinableWith(self, other):
         """
         Function that reports if two datasets are mutually uncorrelated = combinable.
 
         :param other: datasetObj to compare self with
         """
+        if type(other)==CombinedDataSet:
+            # if other is a combined dataset, self is combinable if it is
+            # combinable with all datasets in other
+            other_ds = other._datasets
+            for ods in other_ds:
+                if not self.isCombinableWith ( ods ):
+                    return False
+            return True
         idSelf = self.globalInfo.id
         didSelf = self.dataInfo.dataId
         selflabel = f"{idSelf}:{didSelf}"
         idOther = other.globalInfo.id
         didOther = other.dataInfo.dataId
         otherlabel = f"{idOther}:{didOther}"
 
@@ -97,14 +105,16 @@
             return True
         if self.isLocalFieldCombinableWith_(other):
             return True
         if other.isLocalFieldCombinableWith_(self):
             return True
         if self.isCombMatrixCombinableWith_(other):
             return True
+        if other.isCombMatrixCombinableWith_(self):
+            return True
         return False
 
     def isCombMatrixCombinableWith_(self, other):
         """ check for combinability via the combinations matrix """
         if not hasattr(self.globalInfo, "_combinationsmatrix"):
             return False
         if self.globalInfo._combinationsmatrix is None:
@@ -206,15 +216,15 @@
             ret = "Dataset: %s" % (", ".join(map(str, self.txnameList)))
         return ret
 
     def __repr__(self):
         if self.dataInfo.dataId:
             return self.dataInfo.dataId
         else:
-            return 'Dataset'
+            return 'Dataset (UL)'
 
     def __eq__(self, other):
         if type(other) != type(self):
             return False
         if self.dataInfo != other.dataInfo:
             return False
         if len(self.txnameList) != len(other.txnameList):
@@ -406,24 +416,40 @@
         self.path = expResult.path
         self.globalInfo = expResult.globalInfo
         self._datasets = expResult.datasets[:]
         self.origdatasets = expResult.origdatasets[:]
         self.sortDataSets()
         self.findType()
 
+    def isCombinableWith ( self, other ):
+        """ 
+        Function that reports if two datasets are mutually uncorrelated = combinable.
+        A combined dataset is combinable with "other", if all consistituents are.
+
+        :param other: datasetObj to compare self with
+        """
+        for ds in self._datasets:
+            if not ds.isCombinableWith ( other ):
+                return False
+        return True
+
     def findType(self):
         """ find the type of the combined dataset """
         self.type = "bestSR"  # type of combined dataset, e.g. pyhf, or simplified
         if hasattr(self.globalInfo, "covariance"):
             self.type = "simplified"
         if hasattr(self.globalInfo, "jsonFiles"):
             self.type = "pyhf"
 
     def __str__(self):
-        ret = "Combined Dataset (%i datasets)" % len(self._datasets)
+        ret = f"Combined Dataset ({len(self._datasets)} datasets)"
+        return ret
+
+    def __repr__(self):
+        ret = f"Combined Dataset ({len(self._datasets)} datasets)"
         return ret
 
     def getIndex(self, dId, datasetOrder):
         """ get the index of dataset within the datasetOrder,
             but allow for abbreviated names
         :param dId: id of dataset to search for, may be abbreviated
         :param datasetOrder: the ordered list of datasetIds, long form
```

### Comparing `smodels-2.3.0/smodels/experiment/defaultFinalStates.py` & `smodels-2.3.1/smodels/experiment/defaultFinalStates.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/exceptions.py` & `smodels-2.3.1/smodels/experiment/exceptions.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/expResultObj.py` & `smodels-2.3.1/smodels/experiment/expResultObj.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/infoObj.py` & `smodels-2.3.1/smodels/experiment/infoObj.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/experiment/metaObj.py` & `smodels-2.3.1/smodels/experiment/metaObj.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         :param subdir: directory name that is checked
         :param lastm: the most recent timestamp so far, plus number of files
         :returns: the most recent timestamp, and the number of files
         """
         #ret = lastm
         #ctr=0
         for f in os.listdir ( subdir ):
-            if f in [ "orig", "sms.root", "validation", ".git" ]:
+            if f in [ "orig", "sms.root", "validation", ".git", "exclusion_lines.json" ]:
                 continue
             if f[-1:]=="~":
                 continue
             if f[0]==".":
                 continue
             if f[-3:]==".py":
                 continue
```

### Comparing `smodels-2.3.0/smodels/experiment/txnameObj.py` & `smodels-2.3.1/smodels/experiment/txnameObj.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/installation.py` & `smodels-2.3.1/smodels/installation.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/Makefile` & `smodels-2.3.1/smodels/lib/Makefile`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gdcpl_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_hm_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/gg_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/nllfast-1.2.f` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/nllfast-1.2.f`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/nllfast_7TeV` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/nllfast_7TeV`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -24,15 +24,15 @@
   [19] .eh_frame         PROGBITS        00000000000099f0 0099f0 00017c 00   A  0   0  8
   [20] .init_array       INIT_ARRAY      000000000000ad00 009d00 000008 08  WA  0   0  8
   [21] .fini_array       FINI_ARRAY      000000000000ad08 009d08 000008 08  WA  0   0  8
   [22] .dynamic          DYNAMIC         000000000000ad10 009d10 000210 10  WA  7   0  8
   [23] .got              PROGBITS        000000000000af20 009f20 0000e0 08  WA  0   0  8
   [24] .data             PROGBITS        000000000000b000 00a000 000010 00  WA  0   0  8
   [25] .bss              NOBITS          000000000000b020 00a010 1adb88 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 00a010 000026 01  MS  0   0  1
+  [26] .comment          PROGBITS        0000000000000000 00a010 000025 01  MS  0   0  1
   [27] .symtab           SYMTAB          0000000000000000 00a038 000858 18     28  42  8
   [28] .strtab           STRTAB          0000000000000000 00a890 00056f 00      0   0  1
   [29] .shstrtab         STRTAB          0000000000000000 00adff 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 55bcfea7fe6f1a99a6b0de1b6acad6bddb482225
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 408196cddaf1e3a14d11fdbbf06c527e7f77d26f
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -42,15 +42,15 @@
 # mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu+ [pb] d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # LHC @ 7 TeV, MSTW2008NLO(MSTW2008LO for LO) 
 # LHC @ 7 TeV, CTEQ6.6M (CTEQ6L1 for LO) 
 # mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu [pb] d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # ms[GeV]  mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu+[pb]  d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # ms[GeV]  mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[b]  d_mu+[pb]  d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLLsb_nllnlo_mstw2008.gridss_nllnlo_mstw2008.gridgg_nllnlo_mstw2008.gridgg_nllnlo_hm_mstw2008.gridsg_nllnlo_mstw2008.gridsg_nllnlo_hm_mstw2008.gridst_nllnlo_mstw2008.gridtot_nllnlo_mstw2008.gridsdcpl_nllnlo_mstw2008.gridgdcpl_nllnlo_mstw2008.gridsb_nllnlo_cteq6.gridss_nllnlo_cteq6.gridgg_nllnlo_cteq6.gridgg_nllnlo_hm_cteq6.gridsg_nllnlo_cteq6.gridsg_nllnlo_hm_cteq6.gridst_nllnlo_cteq6.gridtot_nllnlo_cteq6.gridsdcpl_nllnlo_cteq6.gridgdcpl_nllnlo_cteq6.grid
 (' ',1(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))(' ',1(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))(' ',2(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))D
-GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
 __abi_tag
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+  [     0]  GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
```

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sb_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sdcpl_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_hm_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/sg_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/ss_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/st_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-1.2/tot_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gdcpl_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_hm_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/gg_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/nllfast-2.1.f` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/nllfast-2.1.f`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/nllfast_8TeV` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/nllfast_8TeV`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -24,15 +24,15 @@
   [19] .eh_frame         PROGBITS        00000000000099f0 0099f0 00017c 00   A  0   0  8
   [20] .init_array       INIT_ARRAY      000000000000ad00 009d00 000008 08  WA  0   0  8
   [21] .fini_array       FINI_ARRAY      000000000000ad08 009d08 000008 08  WA  0   0  8
   [22] .dynamic          DYNAMIC         000000000000ad10 009d10 000210 10  WA  7   0  8
   [23] .got              PROGBITS        000000000000af20 009f20 0000e0 08  WA  0   0  8
   [24] .data             PROGBITS        000000000000b000 00a000 000010 00  WA  0   0  8
   [25] .bss              NOBITS          000000000000b020 00a010 1adb88 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 00a010 000026 01  MS  0   0  1
+  [26] .comment          PROGBITS        0000000000000000 00a010 000025 01  MS  0   0  1
   [27] .symtab           SYMTAB          0000000000000000 00a038 000858 18     28  42  8
   [28] .strtab           STRTAB          0000000000000000 00a890 00056f 00      0   0  1
   [29] .shstrtab         STRTAB          0000000000000000 00adff 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 768da339cfa6f89b77823a5f30c246f91798cedc
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: abed91ffe5ec821383ac75c36a616a81ccd4d5a8
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -43,15 +43,15 @@
 # mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu+ [pb] d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # LHC @ 8 TeV, MSTW2008NLO(MSTW2008LO for LO) 
 # LHC @ 8 TeV, CTEQ6.6M (CTEQ6L1 for LO) 
 # mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu [pb] d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # ms[GeV]  mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[pb]  d_mu+[pb]  d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLL
 # ms[GeV]  mg[GeV]  LO[pb]     NLO[pb]    NLL+NLO[b]  d_mu+[pb]  d_mu-[pb]   d_pdf+[%]  d_pdf-[%]  d_as+[%] d_as-[%]  K_NLO   K_NLLsb_nllnlo_mstw2008.gridss_nllnlo_mstw2008.gridgg_nllnlo_mstw2008.gridgg_nllnlo_hm_mstw2008.gridsg_nllnlo_mstw2008.gridsg_nllnlo_hm_mstw2008.gridst_nllnlo_mstw2008.gridtot_nllnlo_mstw2008.gridsdcpl_nllnlo_mstw2008.gridgdcpl_nllnlo_mstw2008.gridsb_nllnlo_cteq6.gridss_nllnlo_cteq6.gridgg_nllnlo_cteq6.gridgg_nllnlo_hm_cteq6.gridsg_nllnlo_cteq6.gridsg_nllnlo_hm_cteq6.gridst_nllnlo_cteq6.gridtot_nllnlo_cteq6.gridsdcpl_nllnlo_cteq6.gridgdcpl_nllnlo_cteq6.grid
 (' ',1(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))(' ',1(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))(' ',2(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'  ',(f8.1),'  ',(f8.1),'',2(f8.2))
-GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
 __abi_tag
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+  [     0]  GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
```

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sb_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sdcpl_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_hm_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/sg_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/ss_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_cteq6.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_cteq6.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_mstw2008.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-2.1/st_nllnlo_mstw2008.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gdcpl_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_hm_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/gg_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/nllfast-3.1-13TeV.f` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/nllfast-3.1-13TeV.f`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/nllfast_13TeV` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/nllfast_13TeV`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -24,15 +24,15 @@
   [19] .eh_frame         PROGBITS        000000000000cdc0 00cdc0 00017c 00   A  0   0  8
   [20] .init_array       INIT_ARRAY      000000000000dd00 00dd00 000008 08  WA  0   0  8
   [21] .fini_array       FINI_ARRAY      000000000000dd08 00dd08 000008 08  WA  0   0  8
   [22] .dynamic          DYNAMIC         000000000000dd10 00dd10 000210 10  WA  7   0  8
   [23] .got              PROGBITS        000000000000df20 00df20 0000e0 08  WA  0   0  8
   [24] .data             PROGBITS        000000000000e000 00e000 000010 00  WA  0   0  8
   [25] .bss              NOBITS          000000000000e020 00e010 1adb98 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 00e010 000026 01  MS  0   0  1
+  [26] .comment          PROGBITS        0000000000000000 00e010 000025 01  MS  0   0  1
   [27] .symtab           SYMTAB          0000000000000000 00e038 000870 18     28  42  8
   [28] .strtab           STRTAB          0000000000000000 00e8a8 00057d 00      0   0  1
   [29] .shstrtab         STRTAB          0000000000000000 00ee25 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 8a4675eadc3a6cd551fd5118fb57ecc9ed52b7b8
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ea2ee47017833bd7b0301e0d8ff29393a830a7da
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -56,15 +56,15 @@
 (' ',1(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '     ',(f8.1),'   ',2(f8.2))
 (' ',1(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '     ',(f8.1),'   ',2(f8.2))
 (' ',2(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '     ',(f8.1),'    ',2(f8.2))
 (' ',2(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '     ',(f8.1),'    ',2(f8.2))
 (' ',1(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'   ',(f8.1),' ',(f8.1),' ',2(f8.2))
 (' ',1(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '   ',(f8.1),'   ',(f8.1),' ',(f8.1),' ',2(f8.2))
 (' ',2(F7.0,2x),3(E11.3),'  ',(E11.3),' ',(E11.3),(f8.1),       '   ',(f8.1),'  ',(f8.1),' ',(f8.1),' ',2(f8.2))(' ',2(F7.0,2x),3(E11.3),' ',(E11.3),' ',(E11.3),(f8.1),        '   ',(f8.1),'  ',(f8.1),' ',(f8.1),' ',2(f8.2))
-GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
 __abi_tag
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+  [     0]  GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
```

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sb_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sdcpl_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_hm_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/sg_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/ss_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_cteq66_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_cteq66_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_mstw2008_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_mstw2008_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_nnpdf30_13TeV.grid` & `smodels-2.3.1/smodels/lib/nllfast/nllfast-3.1/st_nllnlo_nnpdf30_13TeV.grid`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia6/pythia-6.4.27.f` & `smodels-2.3.1/smodels/lib/pythia6/pythia-6.4.27.f`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia6/pythia_lhe` & `smodels-2.3.1/smodels/lib/pythia6/pythia_lhe`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 0% similar despite different names*

#### readelf --wide --sections {}

```diff
@@ -24,15 +24,15 @@
   [19] .eh_frame         PROGBITS        0000000000305460 305460 002334 00   A  0   0  8
   [20] .init_array       INIT_ARRAY      0000000000308c18 307c18 000008 08  WA  0   0  8
   [21] .fini_array       FINI_ARRAY      0000000000308c20 307c20 000008 08  WA  0   0  8
   [22] .dynamic          DYNAMIC         0000000000308c28 307c28 000220 10  WA  7   0  8
   [23] .got              PROGBITS        0000000000308e48 307e48 0001b8 08  WA  0   0  8
   [24] .data             PROGBITS        0000000000309000 308000 0afea6 00  WA  0   0 32
   [25] .bss              NOBITS          00000000003b8ec0 3b7ea6 165ca8 00  WA  0   0 32
-  [26] .comment          PROGBITS        0000000000000000 3b7ea6 000026 01  MS  0   0  1
+  [26] .comment          PROGBITS        0000000000000000 3b7ea6 000025 01  MS  0   0  1
   [27] .symtab           SYMTAB          0000000000000000 3b7ed0 004b78 18     28 430  8
   [28] .strtab           STRTAB          0000000000000000 3bca48 001e97 00      0   0  1
   [29] .shstrtab         STRTAB          0000000000000000 3be8df 000111 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
```

#### readelf --wide --notes {}

```diff
@@ -1,12 +1,12 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 ISA needed: x86-64-baseline
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d36b3fe0bd75d379766dc062660723f14d3953fa
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: dd9b1646e72cad8753c15db2e974b024860da11d
 
 Displaying notes found in: .note.ABI-tag
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_ABI_TAG (ABI version tag)	    OS: Linux, ABI: 3.2.0
```

#### strings --all --bytes=8 {}

```diff
@@ -1462,15 +1462,15 @@
 Q@33333s[
 c=@33333
 G@33333CX@fffff
 abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ
             *......*                   *:::!!:::::::::::*           *::::::!!::::::::::::::*      *::::::::!!::::::::::::::::*   *:::::::::!!:::::::::::::::::*  *:::::::::!!:::::::::::::::::*   *::::::::!!::::::::::::::::*!     *::::::!!::::::::::::::* !!     !! *:::!!:::::::::::*    !!     !!     !* -><- *         !!     !!     !!                !!     !!     !!                !!     !!                       !!     !!        lh             !!     !!                       !!     !!                 hh    !!     !!    ll                 !!     !!                       !!     !!                          Welcome to the Lund Monte Carlo!                                PPP  Y   Y TTTTT H   H III   A  P  P  Y Y    T   H   H  I   A A PPP    Y     T   HHHHH  I  AAAAAP      Y     T   H   H  I  A   AP      Y     T   H   H III A   A                                This is PYTHIA version x.xxx    Last date of change: xx xxx 201x                                Now is xx xxx 201x at xx:xx:xx                                  Disclaimer: this program comes  without any guarantees. Beware  of errors and use common sense  when interpreting results.                                      Copyright T. Sjostrand (2011)   
 JanFebMarAprMayJunJulAugSepOctNovDec
 An archive of program versions and documentation is found on the web:   http://www.thep.lu.se/~torbjorn/Pythia.html                                                                                                     When you cite this program, the official reference is to the 6.4 manual:T. Sjostrand, S. Mrenna and P. Skands, JHEP05 (2006) 026                (LU TP 06-13, FERMILAB-PUB-06-052-CD-T) [hep-ph/0603175].                                                                                       Also remember that the program, to a large extent, represents original  physics research. Other publications of special relevance to your       studies may therefore deserve separate mention.                                                                                                 Main author: Torbjorn Sjostrand; Department of Theoretical Physics,       Lund University, Solvegatan 14A, S-223 62 Lund, Sweden;                 phone: + 46 - 46 - 222 48 16; e-mail: torbjorn@thep.lu.se             Author: Stephen Mrenna; Computing Division, GDS Group,                    Fermi National Accelerator Laboratory, MS 234, Batavia, IL 60510, USA;  phone: + 1 - 630 - 840 - 2556; e-mail: mrenna@fnal.gov                Author: Peter Skands; CERN/PH-TH, CH-1211 Geneva, Switzerland             phone: + 41 - 22 - 767 24 47; e-mail: peter.skands@cern.ch            
-KCHG(I,1)KCHG(I,2)KCHG(I,3)KCHG(I,4)PMAS(I,1)PMAS(I,2)PMAS(I,3)PMAS(I,4)MDCY(I,1)MDCY(I,2)MDCY(I,3)MDME(I,1)MDME(I,2)BRAT(I)  KFDP(I,1)KFDP(I,2)KFDP(I,3)KFDP(I,4)KFDP(I,5)CHAF(I,1)CHAF(I,2)MWID(I)  GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+KCHG(I,1)KCHG(I,2)KCHG(I,3)KCHG(I,4)PMAS(I,1)PMAS(I,2)PMAS(I,3)PMAS(I,4)MDCY(I,1)MDCY(I,2)MDCY(I,3)MDME(I,1)MDME(I,2)BRAT(I)  KFDP(I,1)KFDP(I,2)KFDP(I,3)KFDP(I,4)KFDP(I,5)CHAF(I,1)CHAF(I,2)MWID(I)  GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
 __abi_tag
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
```

#### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     0]  GCC: (Ubuntu 12.2.0-17ubuntu1) 12.2.0
+  [     0]  GCC: (Ubuntu 12.2.0-3ubuntu1) 12.2.0
```

### Comparing `smodels-2.3.0/smodels/lib/pythia6/pythia_lhe.f` & `smodels-2.3.1/smodels/lib/pythia6/pythia_lhe.f`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/Makefile` & `smodels-2.3.1/smodels/lib/pythia8/Makefile`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/installer.py` & `smodels-2.3.1/smodels/lib/pythia8/installer.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/parseXml.py` & `smodels-2.3.1/smodels/lib/pythia8/parseXml.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/pythia8.cc` & `smodels-2.3.1/smodels/lib/pythia8/pythia8.cc`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/pythia8.exe` & `smodels-2.3.1/smodels/lib/pythia8/pythia8.exe`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/lib/pythia8/pythia8308/Makefile` & `smodels-2.3.1/smodels/lib/pythia8/pythia8308/Makefile`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/particlesLoader.py` & `smodels-2.3.1/smodels/particlesLoader.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,32 +40,55 @@
 
     if not os.path.isfile(filename):
         logger.error("Model file %s not found." %slhafile)
         raise SModelSError()
 
     logger.debug("Trying to define BSM particles from SLHA input file %s" %filename)
 
-    #Read file and extract blocks:
+    #Read file and extract blocks 
+    # (can not use pyslha, since it only allows for a single block per block name):
     with open(filename,'r') as f:
         data = f.read()
     data = data.lower()
-    data = data[:data.find('\ndecay')]
-    data = data[:data.find('\nxsection')]
-    blocks = [b.splitlines() for b in data.split('\nblock')]
+    qnumberBlocks = []
+    qBlock = False
+    for l in data.splitlines():
+        l = l.strip()
+        # Ignore empty lines and comments
+        if not l or l.startswith('#'):
+            continue
+        # Beginning of QNUMBERS block
+        if l.startswith('block qnumbers'):
+            qBlock = True
+            qnumberBlocks.append([l])
+            continue
+        # If any other block is starting set qBlock to False
+        elif l.startswith('block'):
+            qBlock = False
+            continue
+        # If a cross-section or decay block is starting set qBlock to False
+        elif l.startswith('xsection') or l.startswith('decay'):
+            qBlock = False
+            continue                   
+        
+        # If current block is not a qnumbers block, skip
+        if not qBlock:
+            continue
+        # Add line to qnumbers block
+        qnumberBlocks[-1].append(l)
 
-    #Extract qnumber blocks
-    qnumberBlocks = [b for b in blocks if 'qnumbers' in b[0]]
     if not qnumberBlocks:
         logger.error("No QNUMBERS blocks were found in %s" %slhafile)
         raise SModelSError()
 
     #Build list of BSM particles:
     BSMList = []
     for b in qnumberBlocks:
-        headerInfo = [x for x in b[0].replace('qnumbers','').split() if x != '#']
+        headerInfo = [x for x in b[0].replace('block','').replace('qnumbers','').split() 
+                      if x != '#']
         if headerInfo[0].replace('-','').replace('+','').isdigit():
             pdg = eval(headerInfo[0])
         else:
             logger.error("Error obtaining PDG number from QNUMBERS block:\n %s \n" %b)
 
         if any(p.pdg == pdg for p in BSMList):
             logger.warning("Particle with pdg %i appears multiple times in QNUMBERS blocks")
```

### Comparing `smodels-2.3.0/smodels/share/BANNER` & `smodels-2.3.1/smodels/share/BANNER`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/SMparticles.py` & `smodels-2.3.1/smodels/share/models/SMparticles.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/dgmssm.py` & `smodels-2.3.1/smodels/share/models/dgmssm.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/idm.py` & `smodels-2.3.1/smodels/share/models/idm.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/mssm.py` & `smodels-2.3.1/smodels/share/models/mssm.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/mssmQNumbers.slha` & `smodels-2.3.1/smodels/share/models/mssmQNumbers.slha`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/models/nmssm.py` & `smodels-2.3.1/smodels/share/models/nmssm.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/share/pythia_test.card` & `smodels-2.3.1/smodels/share/pythia_test.card`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/auxiliaryFunctions.py` & `smodels-2.3.1/smodels/theory/auxiliaryFunctions.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/branch.py` & `smodels-2.3.1/smodels/theory/branch.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/clusterTools.py` & `smodels-2.3.1/smodels/theory/clusterTools.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/crossSection.py` & `smodels-2.3.1/smodels/theory/crossSection.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/decomposer.py` & `smodels-2.3.1/smodels/theory/decomposer.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/element.py` & `smodels-2.3.1/smodels/theory/element.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/lheReader.py` & `smodels-2.3.1/smodels/theory/lheReader.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/model.py` & `smodels-2.3.1/smodels/theory/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,16 @@
 
             if particle.totalwidth > promptWidth:
                 particle.totalwidth = float('inf')*GeV  #Treat particle as prompt
                 logger.debug("Particle %s has width above the threshold and will be assumed as prompt." %particle.pdg)
                 if erasePrompt and particle.Z2parity == -1:
                     logger.debug("Erasing quantum numbers of (prompt) particle %s." %particle.pdg)
                     for attr in erasePrompt:
-                        delattr(particle,attr)
+                        if hasattr ( particle, attr ):
+                            delattr(particle,attr)
             else:
                 particle.decays.append(None) #Include possibility for particle being long-lived (non-prompt)
 
             for decay in particleData.decays:
                 pids = decay.ids
                 missingIDs = set(pids).difference(set(allPDGs))
                 if missingIDs:
@@ -356,15 +357,15 @@
                         minMass=1.0*GeV):
         """
         Update mass, total width and branches of allParticles particles from input SLHA or LHE file.
 
         :param inputFile: input file (SLHA or LHE)
 
         :param promptWidth: Maximum width for considering particles as decaying prompt. If None, it
-                            will be set 1e-8 GeV.
+                            will be set 1e-11 GeV.
         :param stableWidth: Minimum width for considering particles as stable. If None, it
                             will be set 1e-25 GeV.
         :param roundMasses: If set, it will round the masses to this number of digits (int)
 
         :param erasePrompt: If set, all particles with prompt decays (totalwidth > promptWidth)
                                will have the corresponding properties (quantum numbers). So all particles with the same
                                mass and Z2parity will be considered as equal when combining elements.
@@ -372,15 +373,15 @@
         :param minMass: Minimal mass for BSM particles in the model. Any particle with mass below minMass will
                         have its mass set to minMass.
 
         """
 
         self.inputFile = inputFile
         if promptWidth is None:
-            promptWidth = 1e-8*GeV
+            promptWidth = 1e-11*GeV
         if stableWidth is None:
             stableWidth = 1e-25*GeV
 
         massDict,decaysDict,xsections = self.getModelDataFrom(self.inputFile)
         self.xsections = xsections
 
         #Restric BSM particles to the overlap between allBSMparticles and massDict:
```

### Comparing `smodels-2.3.0/smodels/theory/particle.py` & `smodels-2.3.1/smodels/theory/particle.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/theory/theoryPrediction.py` & `smodels-2.3.1/smodels/theory/theoryPrediction.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from smodels.theory import clusterTools, crossSection, element
 from smodels.theory.auxiliaryFunctions import cSim, cGtr, elementsInStr, average
 from smodels.tools.physicsUnits import TeV, fb
 from smodels.theory.exceptions import SModelSTheoryError as SModelSError
 from smodels.experiment.datasetObj import CombinedDataSet
 from smodels.tools.smodelsLogging import logger
 from smodels.tools.statsTools import StatsComputer
-from typing import Union
+from typing import Union, Text
 import itertools
 import numpy as np
 
 __all__ = [ "TheoryPrediction", "theoryPredictionsFor", "TheoryPredictionsCombiner" ]
 
 
 class TheoryPrediction(object):
@@ -257,14 +257,26 @@
 
         if not "nllmax" in self.cachedObjs[expected]:
             self.computeStatistics(expected)
         return self.nllToLikelihood ( self.cachedObjs[expected]["nllmax"],
                 return_nll )
 
     @whenDefined
+    def CLs(self, mu : float = 1., expected : Union[Text,bool] = False ) -> \
+                    Union[float,None]:
+        """ obtain the CLs value of the combination for a given poi value "mu" """
+        if not "CLs" in self.cachedObjs[expected]:
+            self.cachedObjs[expected]["CLs"] = {}
+        if mu in self.cachedObjs[expected]["CLs"]:
+            return self.cachedObjs[expected]["CLs"][mu]
+        cls = self.statsComputer.CLs ( poi_test = mu, expected = expected )
+        self.cachedObjs[expected]["CLs"][mu] = cls
+        return cls
+
+    @whenDefined
     def sigma_mu(self, expected=False):
         """sigma_mu of mu_hat"""
 
         if not "sigma_mu" in self.cachedObjs[expected]:
             self.computeStatistics(expected)
 
         return self.cachedObjs[expected]["sigma_mu"]
```

### Comparing `smodels-2.3.0/smodels/theory/topology.py` & `smodels-2.3.1/smodels/theory/topology.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/analysesCombinations.py` & `smodels-2.3.1/smodels/tools/analysesCombinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -250,27 +250,29 @@
             # and not used the cached value (which is constant for mu~=1 an mu~=0)
             nll = self.likelihood(mu, return_nll=True, expected=expected, useCached=False)
             nllA = self.likelihood(mu, expected="posteriori", return_nll=True, useCached=False)
             return CLsfromNLL(nllA, nll0A, nll, nll0, return_type=return_type) if nll is not None else None
 
         return mu_hat, sigma_mu, clsRoot
 
-    def computeCLs(self, expected: bool = False, return_type: Text = "1-CLs"):
+    def CLs( self, mu : float = 1., expected: Union[Text,bool] = False,
+             return_type: Text = "CLs" ):
         """
-        Compute the exclusion confidence level of the model (1-CLs)
+        Compute the exclusion confidence level of the model
+        :param mu: compute for the parameter of interest mu
         :param expected: if false, compute observed, true: compute a priori expected
         :param return_type: (Text) can be "CLs-alpha", "1-CLs", "CLs" \
                         CLs-alpha: returns CLs - 0.05 \
                         1-CLs: returns 1-CLs value \
                         CLs: returns CLs value
         """
         assert return_type in ["CLs-alpha", "1-CLs", "CLs"], f"Unknown return type: {return_type}."
         _, _, clsRoot = self.getCLsRootFunc(expected=expected)
 
-        return clsRoot(1.0, return_type=return_type)
+        return clsRoot(mu, return_type=return_type)
 
     def getLlhds(self,muvals,expected=False,normalize=True):
         """
         Compute the likelihoods for the individual analyses and the combined
         likelihood.
         Returns a dictionary with the analysis IDs as keys and the likelihood values as values.
```

### Comparing `smodels-2.3.0/smodels/tools/asciiGraph.py` & `smodels-2.3.1/smodels/tools/asciiGraph.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/basicStats.py` & `smodels-2.3.1/smodels/tools/basicStats.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,17 +107,17 @@
         i += 1
         b += (i**2.0) * sigma_mu
         rb = rootfinder(b)
         if rb is None: # if cls computation failed, try with a bigger b value
             continue
         closestr, closest = float("inf"), None
         if i > ntrials or ( b < 0 and not allowNegative ):
-            bvalues = [1.0, 0.0, 3.0, -1.0, 10.0, -3.0, 0.1, -0.1, -10.0, 100.0, -100.0, 1000.0, .01, -.01, .001, -.001 ]
+            bvalues = [1.0, 0.0, 3.0, -1.0, 10.0, -3.0, 0.1, -0.1, -10.0, 100.0, -100.0, 1000.0, .01, -.01, .001, -.001, 10000.0, 100000.0, 1000000.0 ]
             if not allowNegative:
-                bvalues = [1.0, 0.0, 3.0, 10.0, 0.1, 100.0, 1000.0, .01, .001 ]
+                bvalues = [1.0, 0.0, 3.0, 10.0, 0.1, 100.0, 1000.0, .01, .001, 10000.0, 100000.0, 1000000.0 ]
             for b in bvalues:
                 rb = rootfinder(b)
                 if rb is None: # if cls computation failed, try with next b value
                     continue
                 if rb < 0.0:
                     foundExtra = True
                     break
```

### Comparing `smodels-2.3.0/smodels/tools/caching.py` & `smodels-2.3.1/smodels/tools/caching.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/colors.py` & `smodels-2.3.1/smodels/tools/colors.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/coverage.py` & `smodels-2.3.1/smodels/tools/coverage.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/crashReport.py` & `smodels-2.3.1/smodels/tools/crashReport.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/databaseBrowser.py` & `smodels-2.3.1/smodels/tools/databaseBrowser.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/databaseClient.py` & `smodels-2.3.1/smodels/tools/databaseClient.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/databaseServer.py` & `smodels-2.3.1/smodels/tools/databaseServer.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/externalPythonTools.py` & `smodels-2.3.1/smodels/tools/externalPythonTools.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/inclusiveObjects.py` & `smodels-2.3.1/smodels/tools/inclusiveObjects.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/interactivePlots.py` & `smodels-2.3.1/smodels/tools/interactivePlots.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/interactivePlotsHelpers.py` & `smodels-2.3.1/smodels/tools/interactivePlotsHelpers.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/ioObjects.py` & `smodels-2.3.1/smodels/tools/ioObjects.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/modelTester.py` & `smodels-2.3.1/smodels/tools/modelTester.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/nllFastWrapper.py` & `smodels-2.3.1/smodels/tools/nllFastWrapper.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/physicsUnits.py` & `smodels-2.3.1/smodels/tools/physicsUnits.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/printer.py` & `smodels-2.3.1/smodels/tools/printer.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/proxyDBCreator.py` & `smodels-2.3.1/smodels/tools/proxyDBCreator.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/pyhfInterface.py` & `smodels-2.3.1/smodels/tools/pyhfInterface.py`

 * *Files 1% similar despite different names*

```diff
@@ -509,15 +509,15 @@
                 model = workspace.model(modifier_settings=msettings)
                 wsData = workspace.data(model)
 
                 _, nllh = pyhf.infer.mle.fixed_poi_fit(
                     1.0, wsData, model, return_fitted_val=True, maxiter=200
                 )
             except (pyhf.exceptions.FailedMinimization, ValueError) as e:
-                logger.error(f"pyhf fixed_poi_fit failed for mu={mu}: {e}")
+                logger.error(f"pyhf fixed_poi_fit failed for {list(self.data.jsonFiles)[workspace_index]} for mu={mu}: {e}")
                 # lets try with different initialisation
                 init, n_ = pyhf.infer.mle.fixed_poi_fit(
                     0.0, workspace.data(model), model, return_fitted_val=True, maxiter=200
                 )
                 initpars = init.tolist()
                 initpars[model.config.poi_index] = 1.
                 # Try to turn positive all the negative total yields (mu*signal + background) evaluated with the initial parameters
@@ -535,15 +535,15 @@
                         maxiter=2000,
                     )
                     # If a total yield is negative with the best profiled parameters, return None
                     if not all([True if yld >= 0 else False for yld in model.expected_actualdata(bestFitParam)]):
                         self.restore()
                         return self.exponentiateNLL(None, not return_nll)
                 except (pyhf.exceptions.FailedMinimization, ValueError) as e:
-                    logger.info(f"pyhf fixed_poi_fit failed twice for mu={mu}: {e}")
+                    logger.info(f"pyhf fixed_poi_fit failed twice for {list(self.data.jsonFiles)[workspace_index]} for mu={mu}: {e}")
 
                     self.restore()
                     return self.exponentiateNLL(None, not return_nll)
 
             ret = nllh.tolist()
             try:
                 ret = float(ret)
@@ -832,54 +832,56 @@
                 # If expected == posteriori, use unmodified (but patched) workspace
                 workspace = self.updateWorkspace(workspace_index, expected=expected)
                 # Same modifiers_settings as those use when running the 'pyhf cls' command line
                 msettings = {
                     "normsys": {"interpcode": "code4"},
                     "histosys": {"interpcode": "code4p"},
                 }
-                model = workspace.model(modifier_settings=msettings)
-                bounds = model.config.suggested_bounds()
-                bounds[model.config.poi_index] = (0, 10)
-                start = time.time()
-                args = {}
-                args["return_expected"] = expected == "posteriori"
-                args["par_bounds"] = bounds
-                # args["maxiter"]=100000
-                pver = float(pyhf.__version__[:3])
-                stat = "qtilde"
-                if pver < 0.6:
-                    args["qtilde"] = True
-                else:
-                    args["test_stat"] = stat
-                with np.testing.suppress_warnings() as sup:
-                    if pyhfinfo["backend"] == "numpy":
-                        sup.filter(RuntimeWarning, r"invalid value encountered in log")
-                    # print ("expected", expected, "return_expected", args["return_expected"], "mu", mu, "\nworkspace.data(model) :", workspace.data(model, include_auxdata = False), "\nworkspace.observations :", workspace.observations, "\nobs[data] :", workspace['observations'])
-                    try:
-                        result = pyhf.infer.hypotest(mu, workspace.data(model), model, **args)
-                    except Exception as e:
-                        logger.info(f"when testing hypothesis {mu}, caught exception: {e}")
-                        result = float("nan")
-                        if expected == "posteriori":
-                            result = [float("nan")] * 2
-                end = time.time()
-                logger.debug("Hypotest elapsed time : %1.4f secs" % (end - start))
-                logger.debug(f"result for {mu} {result}")
-                if expected == "posteriori":
-                    logger.debug("computing a-posteriori expected limit")
-                    logger.debug("expected = {}, mu = {}, result = {}".format(expected, mu, result))
-                    try:
-                        CLs = float(result[1].tolist())
-                    except TypeError:
-                        CLs = float(result[1][0])
-                else:
-                    logger.debug("expected = {}, mu = {}, result = {}".format(expected, mu, result))
-                    CLs = float(result)
-                # logger.debug("Call of root_func(%f) -> %f" % (mu, 1.0 - CLs))
-                return 1.0 - self.cl - CLs
+                with warnings.catch_warnings():
+                    warnings.simplefilter("ignore", category=(DeprecationWarning,UserWarning))
+                    model = workspace.model(modifier_settings=msettings)
+                    bounds = model.config.suggested_bounds()
+                    bounds[model.config.poi_index] = (0, 10)
+                    start = time.time()
+                    args = {}
+                    args["return_expected"] = expected == "posteriori"
+                    args["par_bounds"] = bounds
+                    # args["maxiter"]=100000
+                    pver = float(pyhf.__version__[:3])
+                    stat = "qtilde"
+                    if pver < 0.6:
+                        args["qtilde"] = True
+                    else:
+                        args["test_stat"] = stat
+                    with np.testing.suppress_warnings() as sup:
+                        if pyhfinfo["backend"] == "numpy":
+                            sup.filter(RuntimeWarning, r"invalid value encountered in log")
+                        # print ("expected", expected, "return_expected", args["return_expected"], "mu", mu, "\nworkspace.data(model) :", workspace.data(model, include_auxdata = False), "\nworkspace.observations :", workspace.observations, "\nobs[data] :", workspace['observations'])
+                        try:
+                            result = pyhf.infer.hypotest(mu, workspace.data(model), model, **args)
+                        except Exception as e:
+                            logger.info(f"when testing hypothesis {mu}, caught exception: {e}")
+                            result = float("nan")
+                            if expected == "posteriori":
+                                result = [float("nan")] * 2
+                    end = time.time()
+                    logger.debug("Hypotest elapsed time : %1.4f secs" % (end - start))
+                    logger.debug(f"result for {mu} {result}")
+                    if expected == "posteriori":
+                        logger.debug("computing a-posteriori expected limit")
+                        logger.debug("expected = {}, mu = {}, result = {}".format(expected, mu, result))
+                        try:
+                            CLs = float(result[1].tolist())
+                        except TypeError:
+                            CLs = float(result[1][0])
+                    else:
+                        logger.debug("expected = {}, mu = {}, result = {}".format(expected, mu, result))
+                        CLs = float(result)
+                    # logger.debug("Call of root_func(%f) -> %f" % (mu, 1.0 - CLs))
+                    return 1.0 - self.cl - CLs
 
             # Rescaling signals so that mu is in [0, 10]
             factor = 3.0
             wereBothLarge = False
             wereBothTiny = False
             nattempts = 0
             nNan = 0
```

### Comparing `smodels-2.3.0/smodels/tools/pythia6Wrapper.py` & `smodels-2.3.1/smodels/tools/pythia6Wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,23 +193,23 @@
         if r == False:
             logger.info ( "Installation check failed." )
             sys.exit()
         self.replaceInCfgFile({"NEVENTS": self.nevents, "SQRTS":1000 * self.sqrts})
         self.setParameter("MSTP(163)", "6")
         lhedata = self._run(slhafile, unlink=unlink )
         if not "<LesHouchesEvents" in lhedata:
-            pythiadir = "%s/log" % self.tempDirectory()
-            logger.error("No LHE events found in pythia output %s" % pythiadir )
+            pythiadir = f"{self.tempDirectory()}/log"
+            logger.error( f"No LHE events found in pythia output {pythiadir}" )
             if not os.path.exists ( pythiadir ):
-                logger.error ("Will dump pythia output to %s" % pythiadir )
+                logger.error ( f"Will dump pythia output to {pythiadir}" )
                 f=open ( pythiadir, "w" )
                 for line in lhedata:
                     f.write ( line )
                 f.close()
-            raise SModelSError( "No LHE events found in %s" % pythiadir )
+            raise SModelSError( f"No LHE events found in {pythiadir}" )
 
         #Reset pythia card to its default value
         if self.pythiacard:
             self.cfgfile = pythiacard_default
 
         #if not unlink:
         #    lhefile = self.tempdir + "/events.lhe"
```

### Comparing `smodels-2.3.0/smodels/tools/pythia8Wrapper.py` & `smodels-2.3.1/smodels/tools/pythia8Wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,23 +117,32 @@
             for inputFile in ["temp.cfg"]:
                 os.unlink(self.tempdir + "/" + inputFile)
             if os.path.exists(self.tempdir):
                 os.rmdir(self.tempdir)
                 self.tempdir = None
 
     def checkInstallation ( self, compile : bool = True ):
-        super().checkInstallation(compile)
+        # super().checkInstallation(compile)
         exists = os.path.exists ( self.includeFile )
         xmldoc = self.getXmldoc()
-        if not os.path.exists ( xmldoc ): # if this disappears, start from scratch
-            import shutil
-            p = xmldoc.find ( "share" )
-            rm = xmldoc[:p-1]
-            shutil.rmtree ( rm, ignore_errors = True )
-            exists = False
+        sleep = 0.
+        while not os.path.exists ( xmldoc ): # if this disappears, start from scratch
+            import time
+            sleep += .5
+            time.sleep ( sleep )
+            if sleep > .5 and not os.path.exists ( xmldoc ): 
+                if compile:
+                    # after a few seconds, delete, if compile is true
+                    import shutil
+                    p = xmldoc.find ( "share" )
+                    rm = xmldoc[:p-1]
+                    if False:
+                        shutil.rmtree ( rm, ignore_errors = True )
+                exists = False
+                break
 
         if xmldoc == None:
             exists = False
         if exists:
             return True
         if compile:
             self.compile()
```

### Comparing `smodels-2.3.0/smodels/tools/pythia8particles.py` & `smodels-2.3.1/smodels/tools/pythia8particles.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/reweighting.py` & `smodels-2.3.1/smodels/tools/reweighting.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/runSModelS.py` & `smodels-2.3.1/smodels/tools/runSModelS.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 from smodels.installation import installDirectory, version
 from smodels.tools import modelTester
 from smodels.tools import crashReport
 from smodels.tools import smodelsLogging
 from smodels.tools import runtime
 from smodels import particlesLoader
-from imp import reload
+from importlib import reload
 
 def main():
     import argparse
     """ Set default input and output files """
     parameterFile = "%s/smodels/etc/parameters_default.ini" % installDirectory()
     outputDir = "./results/"
```

### Comparing `smodels-2.3.0/smodels/tools/runtime.py` & `smodels-2.3.1/smodels/tools/runtime.py`

 * *Files 15% similar despite different names*

```diff
@@ -53,17 +53,29 @@
 def experimentalFeatures():
     """ a simple boolean flag to turn experimental features on/off,
     can be turned on and off via options:experimental in parameters.ini.
     """
     return _experimental
 
 def nCPUs():
-    """ obtain the number of CPU cores on the machine, for several
+    """ obtain the number of *available* CPU cores on the machine, for several
         platforms and python versions. """
     try:
+        # next few lines taken from
+        # https://stackoverflow.comhttps//stackoverflow.com/questions/1006289/how-to-find-out-the-number-of-cpus-using-python/questions/1006289/how-to-find-out-the-number-of-cpus-using-python
+        import re
+        with open('/proc/self/status') as f:
+            m = re.search(r'(?m)^Cpus_allowed:\s*(.*)$', f.read())
+        if m:
+            res = bin(int(m.group(1).replace(',', ''), 16)).count('1')
+            if res > 0:
+                return res
+    except IOError:
+        pass
+    try:
         import multiprocessing
         return multiprocessing.cpu_count()
     except ImportError:
         pass
     try:
         import psutil
         return psutil.NUM_CPUS
```

### Comparing `smodels-2.3.0/smodels/tools/simplifiedLikelihoods.py` & `smodels-2.3.1/smodels/tools/simplifiedLikelihoods.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/slhaChecks.py` & `smodels-2.3.1/smodels/tools/slhaChecks.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/smodelsLogging.py` & `smodels-2.3.1/smodels/tools/smodelsLogging.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/smodelsTools.py` & `smodels-2.3.1/smodels/tools/smodelsTools.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,16 @@
         help="write cross sections to file (only highest order)")
     xseccomputer.add_argument('-P', '--alltofile', action='store_true',
         help="write all cross sections to file, including lower orders")
     xseccomputer.add_argument('-q', '--query', action='store_true',
         help="only query if there are cross sections in the file")
     xseccomputer.add_argument('-C', '--colors', action='store_true',
         help="colored terminal output" )
+    xseccomputer.add_argument('--tempdir', type=str, default="/tmp/",
+        help="specify a temporary directory (default is /tmp/)" )
     xseccomputer.add_argument( '--noautocompile', action='store_true',
         help="turn off automatic compilation" )
     xseccomputer.add_argument('-k', '--keep', action='store_true',
         help="do not unlink temporary directory")
     xseccomputer.add_argument('-6', '--pythia6', action='store_true',
         help="use pythia6 for LO cross sections")
     xseccomputer.add_argument('-8', '--pythia8', action='store_true',
```

### Comparing `smodels-2.3.0/smodels/tools/statsTools.py` & `smodels-2.3.1/smodels/tools/statsTools.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from smodels.tools.smodelsLogging import logger
 from smodels.tools.physicsUnits import fb
 from smodels.tools.simplifiedLikelihoods import LikelihoodComputer, UpperLimitComputer, Data
 from smodels.tools.pyhfInterface import PyhfData, PyhfUpperLimitComputer
 from smodels.tools.truncatedGaussians import TruncatedGaussians
 from smodels.tools.analysesCombinations import AnaCombLikelihoodComputer
 from smodels.experiment.datasetObj import DataSet,CombinedDataSet
+from typing import Union, Text
 
 class StatsComputer:
     __slots__ = [ "nsig", "dataObject", "dataType", "likelihoodComputer", "data",
                   "upperLimitComputer", "deltas_sys", "allowNegativeSignals" ]
     
     def __init__ ( self, dataObject : Union['DataSet','CombinedDataSet', list], dataType : str,
                    nsig : Union[None,float,List] = None,
@@ -333,14 +334,21 @@
         elif self.dataType == "truncGaussian":
             kwargs["expected"]=expected
         elif self.dataType == "analysesComb":
             kwargs["expected"]=expected
         return self.likelihoodComputer.likelihood ( poi_test,
                                                 return_nll = return_nll, **kwargs)
 
+    def CLs ( self, poi_test : float = 1., expected : Union[bool,Text] = False ) -> Union[float,None]:
+        """ compute CLs value for a given value of the poi """
+        # self.transform ( expected )
+        if hasattr ( self.likelihoodComputer, "CLs" ):
+            return self.likelihoodComputer.CLs ( poi_test, expected )
+        return None
+
     def transform ( self, expected ):
         """ SL only. transform the data to expected or observed """
         if self.dataType in [ "pyhf", "truncGaussian", "analysesComb" ]:
             return
         self.likelihoodComputer.transform ( expected )
 
     def maximize_likelihood ( self, expected : Union[bool,Text],
```

### Comparing `smodels-2.3.0/smodels/tools/stringTools.py` & `smodels-2.3.1/smodels/tools/stringTools.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/timeOut.py` & `smodels-2.3.1/smodels/tools/timeOut.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/toolBox.py` & `smodels-2.3.1/smodels/tools/toolBox.py`

 * *Files identical despite different names*

### Comparing `smodels-2.3.0/smodels/tools/truncatedGaussians.py` & `smodels-2.3.1/smodels/tools/truncatedGaussians.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,37 +164,52 @@
         return sigma_mu
 
     def _root_func( self, mu : float ):
         """ the root of this one should determine muhat """
         numerator = erf((self.upperLimitOnMu - mu) / self.denominator) + \
                     erf( mu / self.denominator)
         denominator = 1.0 + erf(mu / self.denominator)
+        if denominator == 0. and np.isclose ( numerator, denominator ):
+            ## 0 / 0 = 1 (in this case)
+            return 1. - self.cl
         ret = numerator / denominator - self.cl
         return ret
 
     def _findMuhat( self, xa : float = 0., 
                         xb : Union[float,None] = None ):
         """ find muhat, in [xa,xb] 
         :param xa: lower limit of initial bracket
         :param xb: upper limit of initial bracket. if none, then max(ul,eul)
         """
         if xa == None:
             xa = 0.
         if xb == None:
             xb = max(self.upperLimitOnMu, self.expectedUpperLimitOnMu)
         c = 0
-        while self._root_func(xa) * self._root_func(xb) > 0:
-            xa = 2 * xa
+        ra, rb = self._root_func(xa), self._root_func(xb)
+        while ra * rb > 0:
             c += 1
             if c > 10:
-                logger.error(
-                    f"cannot find bracket for brent bracketing ul={self.upperLimitOnMu:.2f}, eul={self.expectedUpperLimitOnMu:.2f},r({xa:.2f})={self._root_func(xa):.2f}, r({xb:.2f})={self._root_func(xb):.2f}"
-                )
+                line = f"cannot find bracket for brent bracketing ul={self.upperLimitOnMu:.2f}, eul={self.expectedUpperLimitOnMu:.2f},r({xa:.2f})={self._root_func(xa):.2f}, r({xb:.2f})={self._root_func(xb):.2f}"
+                logger.error( line )
+                raise ValueError ( line )
+            while ra < 0.:
+                xa = xa - 1.5 * abs(xa)-.3
+                ra = self._root_func ( xa )
+            while rb > 0.:
+                xb = xb + 1.5 * abs(xb)+.3
+                rb = self._root_func ( xb )
 
-        muhat = optimize.toms748(self._root_func, xa, xb, rtol=1e-07, xtol=1e-07)
+        try:
+            muhat = optimize.toms748(self._root_func, xa, xb, rtol=1e-07, xtol=1e-07)
+        except ValueError as e:
+            logger.error ( f"truncated gaussian got ValueError {e}: rf({xa:.2f})={self._root_func(xa):.2f}, rf({xb:.2f})={self._root_func(xb):.2f}" )
+            logger.error ( f"ul={self.upperLimitOnMu:.2f}, eul={self.expectedUpperLimitOnMu:.2f}" )
+            muhat = optimize.toms748(self._root_func, xa, xb, rtol=1e-02, xtol=1e-02)
+            logger.error ( f"retry with tol=1e-2 seemed to have worked" )
         return muhat
 
     def _computeLlhd( self, mu, muhat, return_nll):
         if mu is None:
             mu = muhat
         sigma_mu = self.sigma_mu
         ## we could also correct here
```

### Comparing `smodels-2.3.0/smodels/tools/wrapperBase.py` & `smodels-2.3.1/smodels/tools/wrapperBase.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     def absPath(self, path):
         """
         Get the absolute path of <path>, replacing <install> with the
         installation directory.
 
         """
         if path == None:
-            return self.tempDirectory() + "/temp.cfg"
+            return os.path.abspath ( self.tempDirectory() + "/temp.cfg" )
         installdir = installation.installDirectory()
         path = path.replace("<install>", installdir)
         # path = path.replace(".egg/smodels", ".egg/")
         path = os.path.abspath(path)
         return path
 
     def tempDirectory(self):
```

### Comparing `smodels-2.3.0/smodels/tools/xsecComputer.py` & `smodels-2.3.1/smodels/tools/xsecComputer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,37 +23,40 @@
     import cStringIO as io
 except ImportError as e:
     import io
 import sys
 
 class XSecComputer:
     """ cross section computer class, what else? """
-    def __init__ ( self, maxOrder, nevents, pythiaVersion, maycompile=True ):
+    def __init__ ( self, maxOrder, nevents, pythiaVersion, maycompile=True,
+                   defaulttempdir : str = "/tmp/" ):
         """
         :param maxOrder: maximum order to compute the cross section, given as an integer
                     if maxOrder == LO, compute only LO pythia xsecs
                     if maxOrder == NLO, apply NLO K-factors from NLLfast (if available)
                     if maxOrder == NLL, apply NLO+NLL K-factors from NLLfast (if available)
         :param nevents: number of events for pythia run
         :param pythiaVersion: pythia6 or pythia8 (integer)
         :param maycompile: if True, then tools can get compiled on-the-fly
+        :param defaulttempdir: the default temp directory
         """
         self.maxOrder = self._checkMaxOrder ( maxOrder )
         self.countNoXSecs = 0
         self.countNoNLOXSecs = 0
         self.maycompile = maycompile
         if nevents < 1:
             logger.error ( "Supplied nevents < 1" )
             sys.exit()
         self.nevents = nevents
         if pythiaVersion not in [ 6, 8 ]:
             logger.error ( "Unknown pythia version %s. Allowed values: 6, 8" % \
                             ( pythiaVersion ) )
             sys.exit()
         self.pythiaVersion = pythiaVersion
+        self.defaulttempdir = defaulttempdir
 
     def _checkSLHA ( self, slhafile ):
         if not os.path.isfile(slhafile):
             logger.error("SLHA file %s not found.", slhafile)
             raise SModelSError()
         try:
             f=pyslha.readSLHAFile(slhafile)
@@ -202,14 +205,15 @@
                 newx.add(x)
         return newx
 
     def getPythia ( self ):
         """ returns the pythia tool that is configured to be used """
         ret= toolBox.ToolBox().get("pythia%d" % self.pythiaVersion )
         ret.maycompile = self.maycompile
+        ret.defaulttempdir = self.defaulttempdir
         return ret
 
     def compute ( self, sqrts, slhafile,  lhefile=None, unlink=True, loFromSlha=None,
                   pythiacard=None, ssmultipliers=None ):
         """
         Run pythia and compute SUSY cross sections for the input SLHA file.
 
@@ -566,14 +570,20 @@
         if args.alltofile:
             if toFile=="highest":
                 logger.warning ( "Specified both --tofile and --alltofile. Will use "\
                               "--alltofile" )
             toFile="all"
         return toFile
 
+    def tempDir ( self, args ):
+        ret = "/tmp/"
+        if hasattr ( args, "tempdir" ):
+            ret = args.tempdir
+        return ret
+
 def main(args):
     canonizer = ArgsStandardizer()
     setLogLevel ( args.verbosity )
     if not hasattr ( args, "noautocompile" ):
         args.noautocompile = False
     if args.query:
         return canonizer.queryCrossSections ( args.filename )
@@ -610,15 +620,15 @@
             logger.error ( "fork did not succeed! Pid=%d" % pid )
             sys.exit()
         if pid == 0:
             logger.debug ( "chunk #%d: pid %d (parent %d)." %
                        ( i, os.getpid(), os.getppid() ) )
             logger.debug ( " `-> %s" % " ".join ( chunk ) )
             computer = XSecComputer( order, args.nevents, pythiaVersion, \
-                                     not args.noautocompile )
+                                   not args.noautocompile, canonizer.tempDir(args) )
             toFile = canonizer.writeToFile ( args )
             computer.computeForBunch (  sqrtses, chunk, not args.keep,
                           args.LOfromSLHA, toFile, pythiacard=pythiacard, \
                         ssmultipliers = ssmultipliers )
             os._exit ( 0 )
         if pid > 0:
             children.append ( pid )
```

### Comparing `smodels-2.3.0/smodels.egg-info/PKG-INFO` & `smodels-2.3.1/smodels.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smodels
-Version: 2.3.0
+Version: 2.3.1
 Summary: A tool for interpreting simplified-model results from the LHC
 Home-page: https://smodels.github.io/
 Author: The SModelS collaboration, smodels-users@lists.oeaw.ac.at Current members: Mohammad Mahdi Altakach, Sabine Kraml, Andre Lessa, Sahana Narashima, Timothee Pascal, Humberto Reyes-Gonzalez, Wolfgang Waltenberger  Previously involved in SModelS: Gael Alguero, Federico Ambrogi, Juhi Dutta, Jan Heisig, Charanjit K. Khosa, Suchita Kulkarni, Ursula Laa, Veronika Magerl, Wolfgang Magerl, Philipp Neuhuber, Doris Proschofsky, Jory Sonneveld, Michael Traub, Matthias Wolf, Alicia Wongel
 Author-email: smodels-developers@lists.oeaw.ac.at 
 License: GPLv3
 Keywords: simplified models LHC BSM theories interpretation supersymmetry UEDs
 Classifier: Development Status :: 5 - Production/Stable
```

