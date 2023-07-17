# Comparing `tmp/libmata-0.79.1.tar.gz` & `tmp/libmata-0.80.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libmata-0.79.1.tar", last modified: Fri Jul 14 13:55:51 2023, max compression
+gzip compressed data, was "libmata-0.80.0.tar", last modified: Mon Jul 17 12:44:43 2023, max compression
```

## Comparing `libmata-0.79.1.tar` & `libmata-0.80.0.tar`

### file list

```diff
@@ -1,430 +1,440 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.050115 libmata-0.79.1/
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-14 13:55:51.050115 libmata-0.79.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.022116 libmata-0.79.1/libmata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:42:38.405352 libmata-0.79.1/libmata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   327352 2023-07-14 13:43:29.053409 libmata-0.79.1/libmata/alphabets.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.022116 libmata-0.79.1/libmata/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 13:42:38.405352 libmata-0.79.1/libmata/nfa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1211272 2023-07-14 13:43:29.809406 libmata-0.79.1/libmata/nfa/nfa.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   296108 2023-07-14 13:43:30.213404 libmata-0.79.1/libmata/nfa/strings.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   160470 2023-07-14 13:43:30.545401 libmata-0.79.1/libmata/parser.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   571955 2023-07-14 13:43:31.009397 libmata-0.79.1/libmata/plotting.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   273140 2023-07-14 13:43:31.109397 libmata-0.79.1/libmata/utils.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.022116 libmata-0.79.1/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.022116 libmata-0.79.1/mata/3rdparty/
--rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-14 13:42:38.357353 libmata-0.79.1/mata/3rdparty/args.hxx
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/catch.hpp
--rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-14 13:42:38.361353 libmata-0.79.1/mata/3rdparty/catch.hpp.1.9.3
--rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/catch.hpp.2.0.1
--rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/catch.hpp.2.13.9
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.022116 libmata-0.79.1/mata/3rdparty/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd/Doxyfile.in
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd/README
--rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd/RELEASE.NOTES
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.026116 libmata-0.79.1/mata/3rdparty/cudd/cplusplus/
--rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cplusplus/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cplusplus/test_obj.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cplusplus/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cplusplus/testobj.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.030115 libmata-0.79.1/mata/3rdparty/cudd/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-14 13:42:38.385352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-14 13:42:38.389352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/r7x8.1.mat
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/test_cudd.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/cudd_config.h.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.030115 libmata-0.79.1/mata/3rdparty/cudd/dddmp/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/README.dddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/README.testdddmp
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
--rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpUtil.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.030115 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/commands.html
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/credit.html
--rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
--rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
--rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
--rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
--rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
--rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
--rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/packages.html
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/0.add
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/0.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/1.add
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-14 13:42:38.393352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/3.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.max1
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.max2
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/5.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/one.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/varnames.ord
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/zero.bdd
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/dddmp/testdddmp.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/doc/
--rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/doc/cudd.tex.in
--rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/doc/phase.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/epd/
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/epd/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/epd/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/epd/epdInt.h
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/groups.dox
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/cudd/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/cudd/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/mtr/
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/test.groups
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/test_mtr.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/mtr/testmtr.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/st/
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/st/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/st/st.h
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/st/test_st.test.in
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/st/testst.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/cudd/util/
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/cudd/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.026116 libmata-0.79.1/mata/3rdparty/cudd-min/
--rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/bnet.c
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/bnet.h
--rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/chkMterm.c
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/config.h
--rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cpu_stats.c
--rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cpu_time.c
--rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cstringstream.c
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cstringstream.h
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAPI.c
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddApply.c
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddFind.c
--rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-14 13:42:38.365352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddInv.c
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddNeg.c
--rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddWalsh.c
--rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAndAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddAnneal.c
--rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddApa.c
--rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddApprox.c
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddAbs.c
--rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddCorr.c
--rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddIte.c
--rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddBridge.c
--rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddCheck.c
--rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddClip.c
--rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddCompose.c
--rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddDecomp.c
--rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddEssent.c
--rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddExact.c
--rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddExport.c
--rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddGenCof.c
--rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddGenetic.c
--rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddHarwell.c
--rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddInit.c
--rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-07-14 13:42:38.369352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddInteract.c
--rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddLCache.c
--rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddLevelQ.c
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddLinear.c
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddLiteral.c
--rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddMatMult.c
--rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddObj.cc
--rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddPriority.c
--rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddRead.c
--rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddRef.c
--rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddReorder.c
--rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSat.c
--rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSign.c
--rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSolve.c
--rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSplit.c
--rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSubsetHB.c
--rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSubsetSP.c
--rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddSymmetry.c
--rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddTable.c
--rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddWindow.c
--rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-14 13:42:38.373352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddCount.c
--rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddFuncs.c
--rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddIsop.c
--rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddLin.c
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddPort.c
--rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddReord.c
--rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddSetop.c
--rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddSymm.c
--rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/datalimit.c
--rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmp.h
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpBinary.c
--rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpConvert.c
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpDbg.c
--rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpLoad.c
--rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpLoadCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreAdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreBdd.c
--rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreCnf.c
--rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreMisc.c
--rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/dddmpUtil.c
--rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/epd.c
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/epd.h
--rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/epdInt.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/cudd-min/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.026116 libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/cudd/
--rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
--rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
--rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/main.c
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-14 13:42:38.377352 libmata-0.79.1/mata/3rdparty/cudd-min/mtr.h
--rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/mtrBasic.c
--rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/mtrGroup.c
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/mtrInt.h
--rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntr.c
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntr.h
--rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntrBddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntrHeap.c
--rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntrMflow.c
--rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntrShort.c
--rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ntrZddTest.c
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/pathsearch.c
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/pipefork.c
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/prtime.c
--rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/safe_mem.c
--rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/st.c
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/st.h
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/strsav.c
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testcudd.c
--rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testdddmp.c
--rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testextra.c
--rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testmtr.c
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testmulti.cc
--rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testobj.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/testst.c
--rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/texpand.c
--rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/ucbqsort.c
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-14 13:42:38.381352 libmata-0.79.1/mata/3rdparty/cudd-min/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.034115 libmata-0.79.1/mata/3rdparty/re2/
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/re2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/re2/CONTRIBUTORS
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/re2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.038116 libmata-0.79.1/mata/3rdparty/re2/re2/
--rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-14 13:42:38.397352 libmata-0.79.1/mata/3rdparty/re2/re2/bitmap256.h
--rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/compile.cc
--rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/parse.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/perl_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/pod_array.h
--rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/prog.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/prog.h
--rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/re2.cc
--rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/re2.h
--rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/regexp.cc
--rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/regexp.h
--rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/simplify.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/sparse_array.h
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/sparse_set.h
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/stringpiece.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/stringpiece.h
--rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/tostring.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/unicode_casefold.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/unicode_casefold.h
--rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/unicode_groups.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/unicode_groups.h
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/re2/walker-inl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.038116 libmata-0.79.1/mata/3rdparty/re2/util/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/logging.h
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/mutex.h
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/rune.cc
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/strutil.cc
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/strutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/utf.h
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/re2/util/util.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/simlib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/simlib/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/3rdparty/simlib/include/mata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.038116 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.038116 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.038116 libmata-0.79.1/mata/3rdparty/simlib/src/
--rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-14 13:42:38.401352 libmata-0.79.1/mata/3rdparty/simlib/src/explicit_lts_sim.cc
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-14 13:55:50.914115 libmata-0.79.1/mata/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-14 13:55:50.914115 libmata-0.79.1/mata/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 13:55:50.914115 libmata-0.79.1/mata/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.018115 libmata-0.79.1/mata/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.042116 libmata-0.79.1/mata/include/mata/
--rw-r--r--   0 runner    (1001) docker     (123)    17314 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/afa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/alphabet.hh
--rw-r--r--   0 runner    (1001) docker     (123)    19025 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/closed-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    10509 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/inter-aut.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/mintermization.hh
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/nfa-algorithms.hh
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/nfa-plumbing.hh
--rw-r--r--   0 runner    (1001) docker     (123)    18622 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/nfa-strings.hh
--rw-r--r--   0 runner    (1001) docker     (123)    45972 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/nfa.hh
--rw-r--r--   0 runner    (1001) docker     (123)    16535 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/number-predicate.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/ord-vector.hh
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/re2parser.hh
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/sparse-set.hh
--rw-r--r--   0 runner    (1001) docker     (123)    12674 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/synchronized-iterator.hh
--rw-r--r--   0 runner    (1001) docker     (123)    15407 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/include/mata/util.hh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.042116 libmata-0.79.1/mata/src/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-14 13:42:38.409352 libmata-0.79.1/mata/src/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.042116 libmata-0.79.1/mata/src/afa/
--rw-r--r--   0 runner    (1001) docker     (123)    38796 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/afa/afa.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/alphabet.cc
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/config.cc.in
--rw-r--r--   0 runner    (1001) docker     (123)    26602 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/inter-aut.cc
--rw-r--r--   0 runner    (1001) docker     (123)    14526 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/mintermization.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.046115 libmata-0.79.1/mata/src/nfa/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa-complement.cc
--rw-r--r--   0 runner    (1001) docker     (123)     5331 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa-concatenation.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa-inclusion.cc
--rw-r--r--   0 runner    (1001) docker     (123)     9492 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa-intersection.cc
--rw-r--r--   0 runner    (1001) docker     (123)     4820 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa-universal.cc
--rw-r--r--   0 runner    (1001) docker     (123)    77739 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/nfa/nfa.cc
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/parser.cc
--rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/re2parser.cc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 13:55:51.050115 libmata-0.79.1/mata/src/strings/
--rw-r--r--   0 runner    (1001) docker     (123)    17847 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/strings/nfa-noodlification.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/strings/nfa-segmentation.cc
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-14 13:42:38.413352 libmata-0.79.1/mata/src/strings/nfa-strings.cc
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-14 13:42:38.405352 libmata-0.79.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-14 13:42:38.405352 libmata-0.79.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-07-17 12:44:43.374560 libmata-0.80.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.358559 libmata-0.80.0/libmata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:27:43.430636 libmata-0.80.0/libmata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   327567 2023-07-17 12:28:39.514053 libmata-0.80.0/libmata/alphabets.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.358559 libmata-0.80.0/libmata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 12:27:43.430636 libmata-0.80.0/libmata/nfa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1211581 2023-07-17 12:28:40.454110 libmata-0.80.0/libmata/nfa/nfa.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   296417 2023-07-17 12:28:40.966142 libmata-0.80.0/libmata/nfa/strings.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   160793 2023-07-17 12:28:41.390168 libmata-0.80.0/libmata/parser.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   572264 2023-07-17 12:28:41.970203 libmata-0.80.0/libmata/plotting.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   273343 2023-07-17 12:28:42.094211 libmata-0.80.0/libmata/utils.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.358559 libmata-0.80.0/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.358559 libmata-0.80.0/mata/3rdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)    79536 2023-07-17 12:27:43.374633 libmata-0.80.0/mata/3rdparty/args.hxx
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/catch.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)   417675 2023-07-17 12:27:43.378634 libmata-0.80.0/mata/3rdparty/catch.hpp.1.9.3
+-rw-r--r--   0 runner    (1001) docker     (123)   416932 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/catch.hpp.2.0.1
+-rw-r--r--   0 runner    (1001) docker     (123)   657276 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/catch.hpp.2.13.9
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.358559 libmata-0.80.0/mata/3rdparty/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   104287 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd/Doxyfile.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd/README
+-rw-r--r--   0 runner    (1001) docker     (123)    13840 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd/RELEASE.NOTES
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.366560 libmata-0.80.0/mata/3rdparty/cudd/cplusplus/
+-rw-r--r--   0 runner    (1001) docker     (123)   118858 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cplusplus/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23907 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cplusplus/testobj.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.366560 libmata-0.80.0/mata/3rdparty/cudd/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-17 12:27:43.406635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47195 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-17 12:27:43.410635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/r7x8.1.mat
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/test_cudd.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14038 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/cudd_config.h.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/dddmp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/README.dddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/README.testdddmp
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES
+-rw-r--r--   0 runner    (1001) docker     (123)    13047 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/cmdIndex.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/commands.html
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/credit.html
+-rw-r--r--   0 runner    (1001) docker     (123)    64661 2023-07-17 12:27:43.414635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    64648 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps
+-rw-r--r--   0 runner    (1001) docker     (123)    23413 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllByFunc.html
+-rw-r--r--   0 runner    (1001) docker     (123)   127869 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32197 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpExt.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4170 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)    27862 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpTitle.html
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/packages.html
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/pkgIndex.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/0.add
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/0.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2262 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/1.add
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/3.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.max1
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.max2
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/5.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/one.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/s27RP1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp1.bdd.bis
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/s27deltaDddmp2.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/varauxids.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/varnames.ord
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/zero.bdd
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/test_dddmp.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/dddmp/testdddmp.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)    97463 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/doc/cudd.tex.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17981 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/doc/phase.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/epd/
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/epd/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/epd/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4264 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/epd/epdInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-17 12:27:43.418635 libmata-0.80.0/mata/3rdparty/cudd/groups.dox
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/cudd/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/cudd/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29098 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/mtr/
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/test.groups
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/test_mtr.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/mtr/testmtr.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/st/
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/st/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/st/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/st/test_st.test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/st/testst.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/cudd/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/cudd/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.366560 libmata-0.80.0/mata/3rdparty/cudd-min/
+-rw-r--r--   0 runner    (1001) docker     (123)    57591 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/cudd-min/bnet.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/cudd-min/bnet.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7149 2023-07-17 12:27:43.382634 libmata-0.80.0/mata/3rdparty/cudd-min/chkMterm.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/config.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8594 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cpu_stats.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4338 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cpu_time.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5483 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cstringstream.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cstringstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)   105019 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAPI.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18658 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddApply.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddFind.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddInv.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddNeg.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddWalsh.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10360 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAndAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19718 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddAnneal.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26589 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddApa.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65063 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddApprox.c
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddAbs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12211 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddCorr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33952 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddIte.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23247 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddBridge.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23919 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24032 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddCheck.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14546 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddClip.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14050 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    44880 2023-07-17 12:27:43.386634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddCompose.c
+-rw-r--r--   0 runner    (1001) docker     (123)    59815 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddDecomp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40003 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddEssent.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24861 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddExact.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46041 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddExport.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57084 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddGenCof.c
+-rw-r--r--   0 runner    (1001) docker     (123)    26667 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddGenetic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    57030 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    15705 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddHarwell.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8575 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddInit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47179 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddInteract.c
+-rw-r--r--   0 runner    (1001) docker     (123)    34453 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddLCache.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14636 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddLevelQ.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddLinear.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddLiteral.c
+-rw-r--r--   0 runner    (1001) docker     (123)    18676 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddMatMult.c
+-rw-r--r--   0 runner    (1001) docker     (123)   118352 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddObj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    29046 2023-07-17 12:27:43.390634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    54937 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddPriority.c
+-rw-r--r--   0 runner    (1001) docker     (123)    16895 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddRead.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17072 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddRef.c
+-rw-r--r--   0 runner    (1001) docker     (123)    54629 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddReorder.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45218 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSat.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9094 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSign.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9722 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSolve.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17869 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSplit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40719 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSubsetHB.c
+-rw-r--r--   0 runner    (1001) docker     (123)    53495 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSubsetSP.c
+-rw-r--r--   0 runner    (1001) docker     (123)    46846 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddSymmetry.c
+-rw-r--r--   0 runner    (1001) docker     (123)    92286 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddTable.c
+-rw-r--r--   0 runner    (1001) docker     (123)   102122 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24532 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddWindow.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8209 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddCount.c
+-rw-r--r--   0 runner    (1001) docker     (123)    36242 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddFuncs.c
+-rw-r--r--   0 runner    (1001) docker     (123)    35725 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23996 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddIsop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25595 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddLin.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddPort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    40115 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddReord.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23818 2023-07-17 12:27:43.394634 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddSetop.c
+-rw-r--r--   0 runner    (1001) docker     (123)    43419 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddSymm.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/datalimit.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13036 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmp.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpBinary.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6332 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpConvert.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpDbg.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7986 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    45057 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpLoad.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30128 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12169 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    25140 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28404 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    47973 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45283 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10701 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/dddmpUtil.c
+-rw-r--r--   0 runner    (1001) docker     (123)    23011 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/epd.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/epd.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/epdInt.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/cudd-min/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.366560 libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/cudd/
+-rw-r--r--   0 runner    (1001) docker     (123)    47917 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h
+-rw-r--r--   0 runner    (1001) docker     (123)    29047 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    42502 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/main.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/mtr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9536 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/mtrBasic.c
+-rw-r--r--   0 runner    (1001) docker     (123)    24499 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/mtrGroup.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-17 12:27:43.398635 libmata-0.80.0/mata/3rdparty/cudd-min/mtrInt.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80087 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntr.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    60542 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntrBddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntrHeap.c
+-rw-r--r--   0 runner    (1001) docker     (123)    56481 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntrMflow.c
+-rw-r--r--   0 runner    (1001) docker     (123)    17013 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntrShort.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13086 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ntrZddTest.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/pathsearch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/pipefork.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/prtime.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3904 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/safe_mem.c
+-rw-r--r--   0 runner    (1001) docker     (123)    30078 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/st.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/st.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/strsav.c
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testcudd.c
+-rw-r--r--   0 runner    (1001) docker     (123)    66662 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testdddmp.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14048 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testextra.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8134 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testmtr.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testmulti.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    23917 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testobj.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8891 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/testst.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3877 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/texpand.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10751 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/ucbqsort.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-17 12:27:43.402635 libmata-0.80.0/mata/3rdparty/cudd-min/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.370560 libmata-0.80.0/mata/3rdparty/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/CONTRIBUTORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/3rdparty/re2/re2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2584 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/bitmap256.h
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/compile.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    76112 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/parse.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3087 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/perl_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/pod_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/prog.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/prog.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2136 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/re2.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    15388 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/re2.h
+-rw-r--r--   0 runner    (1001) docker     (123)    20816 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/regexp.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    21633 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/regexp.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19503 2023-07-17 12:27:43.422636 libmata-0.80.0/mata/3rdparty/re2/re2/simplify.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10857 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/sparse_array.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/sparse_set.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/stringpiece.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/stringpiece.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8701 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/tostring.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/unicode_casefold.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/unicode_casefold.h
+-rw-r--r--   0 runner    (1001) docker     (123)   124977 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/unicode_groups.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/unicode_groups.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/re2/walker-inl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/3rdparty/re2/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/logging.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/mutex.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/rune.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/strutil.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/strutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/utf.h
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/re2/util/util.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/simlib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/simlib/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.350559 libmata-0.80.0/mata/3rdparty/simlib/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    19405 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5566 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/3rdparty/simlib/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    18325 2023-07-17 12:27:43.426636 libmata-0.80.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-07-17 12:44:43.222550 libmata-0.80.0/mata/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8936 2023-07-17 12:44:43.222550 libmata-0.80.0/mata/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 12:44:43.222550 libmata-0.80.0/mata/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.354559 libmata-0.80.0/mata/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/include/mata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/include/mata/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    17343 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/afa/afa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/alphabet.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/include/mata/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6440 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/algorithms.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/builder.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     8866 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/delta.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    31904 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/nfa.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/plumbing.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    18036 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/strings.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/nfa/types.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/include/mata/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/parser/inter-aut.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/parser/mintermization.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     2676 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/parser/parser.hh
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/parser/re2parser.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/include/mata/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    19015 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/utils/closed-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    16531 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/utils/number-predicate.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15382 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/utils/ord-vector.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-07-17 12:27:43.434636 libmata-0.80.0/mata/include/mata/utils/sparse-set.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    12669 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/include/mata/utils/synchronized-iterator.hh
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/include/mata/utils/util.hh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/src/afa/
+-rw-r--r--   0 runner    (1001) docker     (123)    38800 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/afa/afa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/alphabet.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/config.cc.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26609 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/inter-aut.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/mintermization.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/src/nfa/
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/builder.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/complement.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/concatenation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10688 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/delta.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/inclusion.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     9496 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/intersection.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/nfa.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    32836 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/operations.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/nfa/universal.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    11753 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/parser.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    31773 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/re2parser.cc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 12:44:43.374560 libmata-0.80.0/mata/src/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)    17857 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/strings/nfa-noodlification.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/strings/nfa-segmentation.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-07-17 12:27:43.438636 libmata-0.80.0/mata/src/strings/nfa-strings.cc
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-17 12:27:43.430636 libmata-0.80.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-17 12:27:43.430636 libmata-0.80.0/setup.py
```

### Comparing `libmata-0.79.1/PKG-INFO` & `libmata-0.80.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libmata
-Version: 0.79.1
+Version: 0.80.0
 Summary: The automata library
 Home-page: https://github.com/verifit/mata
 Author: Lukáš Holík <holik@fit.vutbr.cz>, Ondřej Lengál <lengal@fit.vutbr.cz>, Martin Hruška <ihruskam@fit.vutbr.cz>, Tomáš Fiedor <ifiedortom@fit.vutbr.cz>, David Chocholatý <chocholaty.david@protonmail.com>, Juraj Síč <sicjuraj@fit.vutbr.cz>, Tomáš Vojnar <vojnar@fit.vutbr.cz>
 Author-email: lengal@fit.vutbr.cz
 License: UNKNOWN
 Keywords: automata,finite automata,alternating automata
 Platform: UNKNOWN
```

### Comparing `libmata-0.79.1/libmata/alphabets.cpp` & `libmata-0.80.0/libmata/alphabets.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/nfa/types.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -26,20 +26,23 @@
         "name": "libmata.alphabets",
         "sources": [
             "libmata/alphabets.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -939,19 +942,19 @@
     template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
     template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
     }
 
     #endif
     
 #include <unordered_map>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
-#include "mata/nfa.hh"
+#include "mata/nfa/types.hh"
 #include "mata/alphabet.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
```

### Comparing `libmata-0.79.1/libmata/nfa/nfa.cpp` & `libmata-0.80.0/libmata/nfa/nfa.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-algorithms.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-plumbing.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/nfa/algorithms.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/nfa.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/plumbing.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/types.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -28,20 +29,23 @@
         "name": "libmata.nfa.nfa",
         "sources": [
             "libmata/nfa/nfa.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -945,25 +949,26 @@
 #include <unordered_map>
 #include <vector>
 #include <memory>
 #include <string.h>
 #include <string>
 #include <list>
 #include <stdint.h>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
-#include "mata/nfa.hh"
+#include "mata/nfa/types.hh"
 #include "mata/alphabet.hh"
 #include <iostream>
 #include <fstream>
 #include <sstream>
-#include "mata/nfa-algorithms.hh"
-#include "mata/nfa-plumbing.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/nfa/plumbing.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
```

### Comparing `libmata-0.79.1/libmata/nfa/strings.cpp` & `libmata-0.80.0/libmata/nfa/strings.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-algorithms.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-plumbing.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-strings.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/nfa/algorithms.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/nfa.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/plumbing.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/strings.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/types.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -29,20 +30,23 @@
         "name": "libmata.nfa.strings",
         "sources": [
             "libmata/nfa/strings.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -946,26 +950,27 @@
 #include <set>
 #include <string.h>
 #include <string>
 #include <unordered_map>
 #include <vector>
 #include <unordered_set>
 #include <list>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
-#include "mata/nfa.hh"
+#include "mata/nfa/types.hh"
 #include "mata/alphabet.hh"
 #include <iostream>
 #include <fstream>
 #include <sstream>
-#include "mata/nfa-algorithms.hh"
-#include "mata/nfa-plumbing.hh"
-#include "mata/nfa-strings.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/nfa/plumbing.hh"
+#include "mata/nfa/strings.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
```

### Comparing `libmata-0.79.1/libmata/parser.cpp` & `libmata-0.80.0/libmata/parser.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -2,21 +2,22 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-algorithms.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-plumbing.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/re2parser.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/nfa/algorithms.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/nfa.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/plumbing.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/types.hh",
+            "/home/runner/work/mata/mata/include/mata/parser/re2parser.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -29,20 +30,23 @@
         "name": "libmata.parser",
         "sources": [
             "libmata/parser.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -946,26 +950,27 @@
 #include <set>
 #include <unordered_set>
 #include <unordered_map>
 #include <vector>
 #include <memory>
 #include <list>
 #include <stdint.h>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
-#include "mata/nfa.hh"
+#include "mata/nfa/types.hh"
 #include "mata/alphabet.hh"
 #include <iostream>
 #include <fstream>
 #include <sstream>
-#include "mata/nfa-algorithms.hh"
-#include "mata/nfa-plumbing.hh"
-#include "mata/re2parser.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/nfa/plumbing.hh"
+#include "mata/parser/re2parser.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
```

### Comparing `libmata-0.79.1/libmata/plotting.cpp` & `libmata-0.80.0/libmata/plotting.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
             "/home/runner/work/mata/mata/include/mata/alphabet.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-algorithms.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa-plumbing.hh",
-            "/home/runner/work/mata/mata/include/mata/nfa.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/nfa/algorithms.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/nfa.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/plumbing.hh",
+            "/home/runner/work/mata/mata/include/mata/nfa/types.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -28,20 +29,23 @@
         "name": "libmata.plotting",
         "sources": [
             "libmata/plotting.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -941,29 +945,30 @@
     template <typename T> typename std::remove_reference<T>::type&& move(T& t) noexcept { return std::move(t); }
     template <typename T> typename std::remove_reference<T>::type&& move(T&& t) noexcept { return std::move(t); }
     }
 
     #endif
     
 #include <unordered_map>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
-#include "mata/nfa.hh"
+#include "mata/nfa/types.hh"
 #include "mata/alphabet.hh"
 #include <set>
 #include <unordered_set>
 #include <memory>
 #include <list>
 #include <iostream>
 #include <fstream>
 #include <sstream>
-#include "mata/nfa-algorithms.hh"
-#include "mata/nfa-plumbing.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/nfa/plumbing.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
 #endif
```

### Comparing `libmata-0.79.1/libmata/utils.cpp` & `libmata-0.80.0/libmata/utils.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
             "/home/runner/work/mata/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh",
-            "/home/runner/work/mata/mata/include/mata/ord-vector.hh",
-            "/home/runner/work/mata/mata/include/mata/sparse-set.hh",
-            "/home/runner/work/mata/mata/include/mata/util.hh"
+            "/home/runner/work/mata/mata/include/mata/utils/ord-vector.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/sparse-set.hh",
+            "/home/runner/work/mata/mata/include/mata/utils/util.hh"
         ],
         "extra_compile_args": [
             "-std=c++20",
             "-DNO_THROW_DISPATCHER"
         ],
         "include_dirs": [
             "/home/runner/work/mata/mata/include",
@@ -24,20 +24,23 @@
         "name": "libmata.utils",
         "sources": [
             "libmata/utils.pyx",
             "/home/runner/work/mata/mata/src/afa/afa.cc",
             "/home/runner/work/mata/mata/src/alphabet.cc",
             "/home/runner/work/mata/mata/src/inter-aut.cc",
             "/home/runner/work/mata/mata/src/mintermization.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-complement.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-concatenation.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-inclusion.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-intersection.cc",
-            "/home/runner/work/mata/mata/src/nfa/nfa-universal.cc",
+            "/home/runner/work/mata/mata/src/nfa/builder.cc",
+            "/home/runner/work/mata/mata/src/nfa/complement.cc",
+            "/home/runner/work/mata/mata/src/nfa/concatenation.cc",
+            "/home/runner/work/mata/mata/src/nfa/delta.cc",
+            "/home/runner/work/mata/mata/src/nfa/inclusion.cc",
+            "/home/runner/work/mata/mata/src/nfa/intersection.cc",
             "/home/runner/work/mata/mata/src/nfa/nfa.cc",
+            "/home/runner/work/mata/mata/src/nfa/operations.cc",
+            "/home/runner/work/mata/mata/src/nfa/universal.cc",
             "/home/runner/work/mata/mata/src/parser.cc",
             "/home/runner/work/mata/mata/src/re2parser.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-noodlification.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-segmentation.cc",
             "/home/runner/work/mata/mata/src/strings/nfa-strings.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/compile.cc",
             "/home/runner/work/mata/mata/3rdparty/re2/re2/parse.cc",
@@ -921,17 +924,17 @@
 /* Early includes */
 #include <stdint.h>
 #include "ios"
 #include "new"
 #include "stdexcept"
 #include "typeinfo"
 #include <vector>
-#include "mata/sparse-set.hh"
-#include "mata/ord-vector.hh"
-#include "mata/util.hh"
+#include "mata/utils/sparse-set.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/util.hh"
 #include "mata/simlib/util/binary_relation.hh"
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
```

### Comparing `libmata-0.79.1/mata/3rdparty/args.hxx` & `libmata-0.80.0/mata/3rdparty/args.hxx`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/catch.hpp` & `libmata-0.80.0/mata/3rdparty/catch.hpp`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/catch.hpp.1.9.3` & `libmata-0.80.0/mata/3rdparty/catch.hpp.1.9.3`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/catch.hpp.2.0.1` & `libmata-0.80.0/mata/3rdparty/catch.hpp.2.0.1`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/catch.hpp.2.13.9` & `libmata-0.80.0/mata/3rdparty/catch.hpp.2.13.9`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/Doxyfile.in` & `libmata-0.80.0/mata/3rdparty/cudd/Doxyfile.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/LICENSE` & `libmata-0.80.0/mata/3rdparty/cudd/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/README` & `libmata-0.80.0/mata/3rdparty/cudd/README`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/RELEASE.NOTES` & `libmata-0.80.0/mata/3rdparty/cudd/RELEASE.NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cplusplus/cuddObj.cc` & `libmata-0.80.0/mata/3rdparty/cudd/cplusplus/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cplusplus/test_obj.test.in` & `libmata-0.80.0/mata/3rdparty/cudd/cplusplus/test_obj.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cplusplus/testmulti.cc` & `libmata-0.80.0/mata/3rdparty/cudd/cplusplus/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cplusplus/testobj.cc` & `libmata-0.80.0/mata/3rdparty/cudd/cplusplus/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAPI.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddApply.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddFind.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddInv.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddIte.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddNeg.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAddWalsh.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAndAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddAnneal.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddApa.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddApprox.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddCorr.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBddIte.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddBridge.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCache.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCheck.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddClip.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCof.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddCompose.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddDecomp.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddEssent.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddExact.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddExport.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGenCof.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGenetic.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddHarwell.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInit.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInt.h` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddInteract.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLCache.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLevelQ.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLinear.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddLiteral.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddMatMult.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddPriority.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddRead.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddRef.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddReorder.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSat.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSign.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSolve.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSplit.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSubsetHB.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSubsetSP.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddSymmetry.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddTable.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddWindow.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddCount.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddFuncs.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddIsop.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddLin.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddMisc.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddPort.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddReord.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddSetop.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddSymm.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/cuddZddUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/test_cudd.test.in` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/test_cudd.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/testcudd.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd/testextra.c` & `libmata-0.80.0/mata/3rdparty/cudd/cudd/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/cudd_config.h.in` & `libmata-0.80.0/mata/3rdparty/cudd/cudd_config.h.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/README.dddmp` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/README.dddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/README.testdddmp` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/README.testdddmp`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/RELEASE_NOTES` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/RELEASE_NOTES`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmp.h` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpBinary.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpConvert.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpDbg.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpInt.h` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpLoad.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/dddmpUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-A4.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmp-2.0-Letter.ps`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpAllFile.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpDesc.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtAbs.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/doc/dddmpExtDet.html`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/0or1.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/0or1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/1.add` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/1.add`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/1.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/1.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/2.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/2.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/2and3.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/2and3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/3.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/3.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis1`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis2`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis3`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.bdd.bis4`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.cnf` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.cnf`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.cnf.bis`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.max1` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.max1`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4.max2` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4.max2`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4bis.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4bis.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/exp/4xor5.bdd`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/dddmp/testdddmp.c` & `libmata-0.80.0/mata/3rdparty/cudd/dddmp/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/doc/cudd.tex.in` & `libmata-0.80.0/mata/3rdparty/cudd/doc/cudd.tex.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/doc/phase.pdf` & `libmata-0.80.0/mata/3rdparty/cudd/doc/phase.pdf`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/epd/epd.c` & `libmata-0.80.0/mata/3rdparty/cudd/epd/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/epd/epd.h` & `libmata-0.80.0/mata/3rdparty/cudd/epd/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/epd/epdInt.h` & `libmata-0.80.0/mata/3rdparty/cudd/epd/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/groups.dox` & `libmata-0.80.0/mata/3rdparty/cudd/groups.dox`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/include/mata/cudd/cudd.h` & `libmata-0.80.0/mata/3rdparty/cudd/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh` & `libmata-0.80.0/mata/3rdparty/cudd/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/mtr.h` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrBasic.c` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/mtrInt.h` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/test_mtr.test.in` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/test_mtr.test.in`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/mtr/testmtr.c` & `libmata-0.80.0/mata/3rdparty/cudd/mtr/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/st/st.c` & `libmata-0.80.0/mata/3rdparty/cudd/st/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/st/st.h` & `libmata-0.80.0/mata/3rdparty/cudd/st/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/st/testst.c` & `libmata-0.80.0/mata/3rdparty/cudd/st/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/cpu_stats.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/cpu_time.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/cstringstream.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/cstringstream.h` & `libmata-0.80.0/mata/3rdparty/cudd/util/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/datalimit.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/pathsearch.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/pipefork.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/prtime.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/safe_mem.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/strsav.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/texpand.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/ucbqsort.c` & `libmata-0.80.0/mata/3rdparty/cudd/util/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd/util/util.h` & `libmata-0.80.0/mata/3rdparty/cudd/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/bnet.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/bnet.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/bnet.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/bnet.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/chkMterm.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/chkMterm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/config.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/config.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cpu_stats.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cpu_stats.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cpu_time.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cpu_time.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cstringstream.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cstringstream.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cstringstream.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/cstringstream.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cudd.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAPI.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAPI.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddApply.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddApply.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddFind.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddFind.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddInv.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddInv.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddIte.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddNeg.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddNeg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAddWalsh.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAddWalsh.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAndAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAndAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddAnneal.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddAnneal.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddApa.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddApa.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddApprox.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddApprox.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddAbs.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddAbs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddCorr.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddCorr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddBddIte.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddBddIte.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddBridge.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddBridge.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddCache.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddCheck.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddCheck.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddClip.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddClip.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddCof.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddCompose.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddCompose.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddDecomp.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddDecomp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddEssent.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddEssent.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddExact.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddExact.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddExport.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddExport.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddGenCof.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddGenCof.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddGenetic.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddGenetic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddHarwell.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddHarwell.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddInit.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddInit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddInt.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddInteract.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddInteract.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddLCache.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddLCache.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddLevelQ.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddLevelQ.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddLinear.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddLinear.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddLiteral.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddLiteral.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddMatMult.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddMatMult.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddObj.cc` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddObj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddObj.hh` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddPriority.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddPriority.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddRead.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddRead.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddRef.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddRef.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddReorder.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddReorder.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSat.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSat.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSign.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSign.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSolve.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSolve.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSplit.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSplit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSubsetHB.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSubsetHB.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSubsetSP.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSubsetSP.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddSymmetry.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddSymmetry.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddTable.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddTable.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddWindow.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddWindow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddCount.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddCount.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddFuncs.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddFuncs.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddIsop.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddIsop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddLin.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddLin.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddMisc.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddPort.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddPort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddReord.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddReord.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddSetop.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddSetop.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddSymm.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddSymm.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/cuddZddUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/cuddZddUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/datalimit.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/datalimit.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmp.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpBinary.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpBinary.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpConvert.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpConvert.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpDbg.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpDbg.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpInt.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpLoad.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpLoad.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpLoadCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpLoadCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeAdd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeBdd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpNodeCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpNodeCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreAdd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreAdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreBdd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreBdd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreCnf.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreCnf.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpStoreMisc.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpStoreMisc.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/dddmpUtil.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/dddmpUtil.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/epd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/epd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/epd.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/epd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/epdInt.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/epdInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/cudd/cudd.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh` & `libmata-0.80.0/mata/3rdparty/cudd-min/include/mata/cudd/cuddObj.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/main.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/main.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/mtr.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/mtr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/mtrBasic.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/mtrBasic.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/mtrGroup.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/mtrGroup.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/mtrInt.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/mtrInt.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntr.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntr.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntr.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntrBddTest.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntrBddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntrHeap.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntrHeap.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntrMflow.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntrMflow.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntrShort.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntrShort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ntrZddTest.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ntrZddTest.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/pathsearch.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/pathsearch.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/pipefork.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/pipefork.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/prtime.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/prtime.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/safe_mem.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/safe_mem.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/st.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/st.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/st.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/st.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/strsav.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/strsav.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testcudd.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/testcudd.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testdddmp.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/testdddmp.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testextra.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/testextra.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testmtr.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/testmtr.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testmulti.cc` & `libmata-0.80.0/mata/3rdparty/cudd-min/testmulti.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testobj.cc` & `libmata-0.80.0/mata/3rdparty/cudd-min/testobj.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/testst.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/testst.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/texpand.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/texpand.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/ucbqsort.c` & `libmata-0.80.0/mata/3rdparty/cudd-min/ucbqsort.c`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/cudd-min/util.h` & `libmata-0.80.0/mata/3rdparty/cudd-min/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/CONTRIBUTORS` & `libmata-0.80.0/mata/3rdparty/re2/CONTRIBUTORS`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/LICENSE` & `libmata-0.80.0/mata/3rdparty/re2/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/bitmap256.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/bitmap256.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/compile.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/compile.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/parse.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/parse.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/perl_groups.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/perl_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/pod_array.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/pod_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/prog.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/prog.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/prog.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/prog.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/re2.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/re2.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/re2.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/re2.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/regexp.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/regexp.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/regexp.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/regexp.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/simplify.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/simplify.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/sparse_array.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/sparse_array.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/sparse_set.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/sparse_set.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/stringpiece.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/stringpiece.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/stringpiece.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/stringpiece.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/tostring.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/tostring.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/unicode_casefold.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/unicode_casefold.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/unicode_casefold.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/unicode_casefold.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/unicode_groups.cc` & `libmata-0.80.0/mata/3rdparty/re2/re2/unicode_groups.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/unicode_groups.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/unicode_groups.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/re2/walker-inl.h` & `libmata-0.80.0/mata/3rdparty/re2/re2/walker-inl.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/logging.h` & `libmata-0.80.0/mata/3rdparty/re2/util/logging.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/mutex.h` & `libmata-0.80.0/mata/3rdparty/re2/util/mutex.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/rune.cc` & `libmata-0.80.0/mata/3rdparty/re2/util/rune.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/strutil.cc` & `libmata-0.80.0/mata/3rdparty/re2/util/strutil.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/utf.h` & `libmata-0.80.0/mata/3rdparty/re2/util/utf.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/re2/util/util.h` & `libmata-0.80.0/mata/3rdparty/re2/util/util.h`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/explicit_lts.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/abstract_transl.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/binary_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/caching_allocator.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/convert.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_counter.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/shared_list.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/simlib.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/smart_set.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/splitting_relation.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/transl_weak.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh` & `libmata-0.80.0/mata/3rdparty/simlib/include/mata/simlib/util/two_way_dict.hh`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/3rdparty/simlib/src/explicit_lts_sim.cc` & `libmata-0.80.0/mata/3rdparty/simlib/src/explicit_lts_sim.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/LICENSE` & `libmata-0.80.0/mata/LICENSE`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/README.md` & `libmata-0.80.0/mata/README.md`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/include/mata/afa.hh` & `libmata-0.80.0/mata/include/mata/afa/afa.hh`

 * *Files 1% similar despite different names*

```diff
@@ -25,19 +25,19 @@
 #include <unordered_map>
 #include <unordered_set>
 #include <utility>
 #include <vector>
 #include <memory>
 
 #include "mata/alphabet.hh"
-#include "mata/nfa.hh"
-#include "mata/parser.hh"
-#include "mata/util.hh"
-#include "mata/ord-vector.hh"
-#include "mata/closed-set.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/parser/parser.hh"
+#include "mata/utils/util.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/utils/closed-set.hh"
 
 /**
  * Alternating Finite Automata including structures, transitions and algorithms.
  *
  * In particular, this includes:
  *   1. Structures (Automaton, Transitions, Results),
  *   2. Algorithms (operations, checks, tests),
```

### Comparing `libmata-0.79.1/mata/include/mata/alphabet.hh` & `libmata-0.80.0/mata/include/mata/alphabet.hh`

 * *Files 1% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 #ifndef MATA_ALPHABET_HH
 #define MATA_ALPHABET_HH
 
 #include <forward_list>
 #include <string>
 #include <utility>
 
-#include "mata/util.hh"
-#include "mata/ord-vector.hh"
+#include "utils/util.hh"
+#include "utils/ord-vector.hh"
 
 namespace Mata {
 
 using Symbol = unsigned;
 using StringToSymbolMap = std::unordered_map<std::string, Symbol>;
 
  /**
```

### Comparing `libmata-0.79.1/mata/include/mata/closed-set.hh` & `libmata-0.80.0/mata/include/mata/utils/closed-set.hh`

 * *Files 0% similar despite different names*

```diff
@@ -62,16 +62,16 @@
  */
 
 #ifndef MATA_CLOSED_SET_HH_
 #define MATA_CLOSED_SET_HH_
 
 #include <cassert>
 
-#include "mata/util.hh"
-#include "mata/ord-vector.hh"
+#include "util.hh"
+#include "ord-vector.hh"
 
 namespace Mata {
 
 // Ordered vector.
 template<typename T> using OrdVec = Mata::Util::OrdVector<T>;
 
 // A closed set could be upward-closed or downward-closed.
```

### Comparing `libmata-0.79.1/mata/include/mata/inter-aut.hh` & `libmata-0.80.0/mata/include/mata/parser/inter-aut.hh`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 #include <unordered_map>
 #include <unordered_set>
 #include <string>
 #include <utility>
 #include <vector>
 
-#include "mata/parser.hh"
+#include "parser.hh"
 
 namespace Mata {
 
 /**
  * A node of graph representing transition formula. A node could be operator (!,&,|) or operand (symbol, state, node).
  * Each node has a name (in case of marking naming, an initial character defining type of node is removed and stored in
  * name), raw (name including potential type marker), and information about its type.
```

### Comparing `libmata-0.79.1/mata/include/mata/mintermization.hh` & `libmata-0.80.0/mata/include/mata/parser/mintermization.hh`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_MINTERM_HH
 #define MATA_MINTERM_HH
 
-#include <mata/cudd/cuddObj.hh>
+#include "mata/cudd/cuddObj.hh"
 
-#include "mata/inter-aut.hh"
+#include "inter-aut.hh"
 
 namespace Mata {
 
 class Mintermization {
 private: // data types
     struct OptionalBdd {
         enum class TYPE {NOTHING_E, BDD_E};
```

### Comparing `libmata-0.79.1/mata/include/mata/nfa-algorithms.hh` & `libmata-0.80.0/mata/include/mata/nfa/algorithms.hh`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_NFA_INTERNALS_HH_
 #define MATA_NFA_INTERNALS_HH_
 
-#include <mata/nfa.hh>
-#include <mata/simlib/util/binary_relation.hh>
+#include "nfa.hh"
+#include "mata/simlib/util/binary_relation.hh"
 
 /**
  * Concrete NFA implementations of algorithms, such as complement, inclusion, or universality checking.
  *
  * This is a separation of the implementation from the interface defined in Mata::Nfa.
  * Note, that in Mata::Nfa interface, there are particular dispatch functions calling
  * these function according to parameters provided by a user.
```

### Comparing `libmata-0.79.1/mata/include/mata/nfa-plumbing.hh` & `libmata-0.80.0/mata/include/mata/nfa/plumbing.hh`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_NFA_PLUMBING_HH_
 #define MATA_NFA_PLUMBING_HH_
 
-#include <mata/nfa.hh>
+#include "nfa.hh"
+#include "builder.hh"
 
 /**
  * Simplified NFA API, used in binding to call NFA algorithms.
  *
  * In particular, this mostly includes operations and checks, that do not return Automaton,
  * but instead take resulting automaton as pointer (e.g. `void f(Nfa* result, const Nfa& lhs, const Nfa& rhs)`).
  */
@@ -63,15 +64,15 @@
 /** Loads an automaton from Parsed object */
 template <class ParsedObject>
 void construct(
         Nfa*                                 result,
         const ParsedObject&                  parsed,
         StringToSymbolMap*                   symbol_map = nullptr,
         StringToStateMap*                    state_map = nullptr) {
-    *result = Mata::Nfa::construct(parsed, symbol_map, state_map);
+    *result = Builder::construct(parsed, symbol_map, state_map);
 }
 
 inline void uni(Nfa *unionAutomaton, const Nfa &lhs, const Nfa &rhs) { *unionAutomaton = uni(lhs, rhs); }
 
 /**
  * @brief Compute intersection of two NFAs.
  *
```

### Comparing `libmata-0.79.1/mata/include/mata/nfa-strings.hh` & `libmata-0.80.0/mata/include/mata/nfa/strings.hh`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 #ifndef MATA_NFA_STRING_SOLVING_HH_
 #define MATA_NFA_STRING_SOLVING_HH_
 
 #include <memory>
 #include <optional>
 
-#include "mata/nfa.hh"
+#include "nfa.hh"
 
 namespace {
     using namespace Mata::Nfa;
 }
 
 /**
  * NFA Algorithms usable for solving string constraints.
@@ -125,29 +125,14 @@
  *
  * @param nfa Input automaton
  * @return true iff L(nfa) = {\eps}
  */
 bool is_lang_eps(const Nfa::Nfa& nfa);
 
 /**
- * Create an automaton accepting only a single @p word.
- */
-Nfa::Nfa create_single_word_nfa(const std::vector<Symbol>& word);
-
-/**
- * Create an automaton accepting only a single @p word.
- *
- * @param word Word to accept.
- * @param alphabet Alphabet to use in NFA for translating word into symbols. If specified, the alphabet has to contain
- *  translations for all of the word symbols. If left empty, a new alphabet with only the symbols of the word will be
- *  created.
- */
-Nfa::Nfa create_single_word_nfa(const std::vector<std::string>& word, Alphabet* alphabet = nullptr);
-
-/**
  * Segment Automata including structs and algorithms.
  *
  * These are automata whose state space can be split into several segments connected by ε-transitions in a chain.
  * No other ε-transitions are allowed. As a consequence, no ε-transitions can appear in a cycle.
  * Segment automaton can have initial states only in the first segment and final states only in the last segment.
  */
 namespace SegNfa {
```

### Comparing `libmata-0.79.1/mata/include/mata/nfa.hh` & `libmata-0.80.0/mata/include/mata/nfa/nfa.hh`

 * *Files 18% similar despite different names*

```diff
@@ -28,357 +28,35 @@
 #include <set>
 #include <unordered_map>
 #include <unordered_set>
 #include <utility>
 #include <vector>
 
 #include "mata/alphabet.hh"
-#include "mata/parser.hh"
-#include "mata/util.hh"
-#include "mata/ord-vector.hh"
-#include "mata/inter-aut.hh"
-#include "mata/synchronized-iterator.hh"
-#include "mata/sparse-set.hh"
+#include "mata/parser/parser.hh"
+#include "mata/utils/util.hh"
+#include "mata/utils/ord-vector.hh"
+#include "mata/parser/inter-aut.hh"
+#include "mata/utils/synchronized-iterator.hh"
+#include "mata/utils/sparse-set.hh"
+#include "types.hh"
+#include "delta.hh"
 
 /**
  * Nondeterministic Finite Automata including structures, transitions and algorithms.
  *
  * In particular, this includes:
  *   1. Structures (Automaton, Transitions, Results, Delta),
  *   2. Algorithms (operations, checks, tests),
  *   3. Constructions.
  *
  * Other algorithms are included in Mata::Nfa::Plumbing (simplified API for, e.g., binding)
  * and Mata::Nfa::Algorithms (concrete implementations of algorithms, such as for complement).
  */
 namespace Mata::Nfa {
-extern const std::string TYPE_NFA;
-
-using State = unsigned long;
-using StateSet = Mata::Util::OrdVector<State>;
-
-template<typename T> using Set = Mata::Util::OrdVector<T>;
-
-using WordSet = std::set<std::vector<Symbol>>;
-struct Run {
-    std::vector<Symbol> word{}; ///< A finite-length word.
-    std::vector<State> path{}; ///< A finite-length path through automaton.
-};
-
-using StringToStateMap = std::unordered_map<std::string, State>;
-
-using StateToStringMap = std::unordered_map<State, std::string>;
-// using StateToPostMap = StateMap<PostSymb>; ///< Transitions.
-/// Mapping of states to states, used, for example, to map original states to reindexed states of new automaton, etc.
-using StateToStateMap = std::unordered_map<State, State>;
-
-using SymbolToStringMap = std::unordered_map<Symbol, std::string>;
-/*TODO: this should become a part of the automaton somehow.
- * It should be a vector indexed by states.
- * */
-
-using StringMap = std::unordered_map<std::string, std::string>;
-
-/*TODO: What about to
- * have names Set, UMap/OMap, State, Symbol, Sequence... and name by Set<State>, UMap<State>, ...
- * maybe something else is needed for the more complex maps*/
-
-struct Limits {
-public:
-    static const State min_state = std::numeric_limits<State>::min();
-    static const State max_state = std::numeric_limits<State>::max();
-    static const Symbol min_symbol = std::numeric_limits<Symbol>::min();
-    static const Symbol max_symbol = std::numeric_limits<Symbol>::max();
-};
-
-/*TODO: Ideally remove functions using this struct as a parameter.
- * unpack the trans. relation to transitions is inefficient, goes against the hairs of the library.
- * Do we want to support it?
- */
-/// A single transition.
-struct Trans {
-	State src;
-	Symbol symb;
-	State tgt;
-
-	Trans() : src(), symb(), tgt() { }
-	Trans(State src, Symbol symb, State tgt) : src(src), symb(symb), tgt(tgt) { }
-
-	bool operator==(const Trans& rhs) const
-	{ // {{{
-		return src == rhs.src && symb == rhs.symb && tgt == rhs.tgt;
-	} // operator== }}}
-	bool operator!=(const Trans& rhs) const { return !this->operator==(rhs); }
-};
-
-using TransSequence = std::vector<Trans>; ///< Set of transitions.
-
-struct Nfa; ///< A non-deterministic finite automaton.
-
-//TODO: Kill these types names? Some of them?
-template<typename T> using Sequence = std::vector<T>; ///< A sequence of elements.
-using AutSequence = Sequence<Nfa>; ///< A sequence of non-deterministic finite automata.
-
-template<typename T> using RefSequence = Sequence<std::reference_wrapper<T>>; ///< A sequence of references to elements.
-using AutRefSequence = RefSequence<Nfa>; ///< A sequence of references to non-deterministic finite automata.
-using ConstAutRefSequence = RefSequence<const Nfa>; ///< A sequence of const references to non-deterministic finite automata.
-
-template<typename T> using PtrSequence = Sequence<T*>; ///< A sequence of pointers to elements.
-using AutPtrSequence = PtrSequence<Nfa>; ///< A sequence of pointers to non-deterministic finite automata.
-using ConstAutPtrSequence = PtrSequence<const Nfa>; ///< A sequence of pointers to const non-deterministic finite automata.
-
-template<typename T> using ConstPtrSequence = Sequence<T* const>; ///< A sequence of const pointers to elements.
-using AutConstPtrSequence = ConstPtrSequence<Nfa>; ///< A sequence of const pointers to non-deterministic finite automata.
-using ConstAutConstPtrSequence = ConstPtrSequence<const Nfa>; ///< A sequence of const pointers to const non-deterministic finite automata.
-
-// TODO: why introduce this type name?
-using SharedPtrAut = std::shared_ptr<Nfa>; ///< A shared pointer to NFA.
-
-/// serializes Nfa into a ParsedSection
-Mata::Parser::ParsedSection serialize(
-	const Nfa&                aut,
-	const SymbolToStringMap*  symbol_map = nullptr,
-	const StateToStringMap*   state_map = nullptr);
-
-/**
- * Structure represents a move which is a symbol and a set of target states of transitions.
- */
-struct Move {
-public:
-    Symbol symbol{};
-    StateSet targets{};
-
-    Move() = default;
-    explicit Move(Symbol symbol) : symbol{ symbol }, targets{} {}
-    Move(Symbol symbol, State state_to) : symbol{ symbol }, targets{ state_to } {}
-    Move(Symbol symbol, StateSet states_to) : symbol{ symbol }, targets{ std::move(states_to) } {}
-
-    Move(Move&& rhs) noexcept : symbol{ rhs.symbol }, targets{ std::move(rhs.targets) } {}
-    Move(const Move& rhs) = default;
-    Move& operator=(Move&& rhs) noexcept;
-    Move& operator=(const Move& rhs) = default;
-
-    inline bool operator<(const Move& rhs) const { return symbol < rhs.symbol; }
-    inline bool operator<=(const Move& rhs) const { return symbol <= rhs.symbol; }
-    inline bool operator==(const Move& rhs) const { return symbol == rhs.symbol; }
-    inline bool operator!=(const Move& rhs) const { return symbol != rhs.symbol; }
-    inline bool operator>(const Move& rhs) const { return symbol > rhs.symbol; }
-    inline bool operator>=(const Move& rhs) const { return symbol >= rhs.symbol; }
-
-    StateSet::iterator begin() { return targets.begin(); }
-    StateSet::iterator end() { return targets.end(); }
-
-    StateSet::const_iterator cbegin() const  { return targets.cbegin(); }
-    StateSet::const_iterator cend() const { return targets.cend(); }
-
-    size_t count(State s) const { return targets.count(s); }
-    bool empty() const { return targets.empty(); }
-    size_t size() const { return targets.size(); }
-
-    void insert(State s);
-    void insert(const StateSet& states);
-
-    // THIS BREAKS THE SORTEDNESS INVARIANT,
-    // dangerous,
-    // but useful for adding states in a random order to sort later (supposedly more efficient than inserting in a random order)
-    void inline push_back(const State s) { targets.push_back(s); }
-
-    void remove(State s) { targets.remove(s); }
-
-    std::vector<State>::const_iterator find(State s) const { return targets.find(s); }
-    std::vector<State>::iterator find(State s) { return targets.find(s); }
-};
-
-/**
- * Post is a data structure representing possible transitions over different symbols.
- * It is an ordered vector containing possible Moves (i.e., pair of symbol and target states.
- * Vector is ordered by symbols which are numbers.
- */
-struct Post : private Util::OrdVector<Move> {
-private:
-    using super = Util::OrdVector<Move>;
-public:
-    using super::iterator, super::const_iterator;
-    using super::begin, super::end, super::cbegin, super::cend;
-    using super::OrdVector;
-    using super::operator=;
-    Post(const Post&) = default;
-    Post(Post&&) = default;
-    Post& operator=(const Post&) = default;
-    Post& operator=(Post&&) = default;
-    using super::insert;
-    using super::reserve;
-    using super::remove;
-    using super::empty, super::size;
-    using super::ToVector;
-    using super::erase;
-    // dangerous, breaks the sortedness invariant
-    using super::push_back;
-    // is adding non-const version as well ok?
-    using super::back;
-    using super::filter;
-
-    using super::find;
-    iterator find(const Symbol symbol) { return super::find({ symbol, {} }); }
-    const_iterator find(const Symbol symbol) const { return super::find({ symbol, {} }); }
-}; // struct Post.
-
-/**
- * Delta is a data structure for representing transition relation.
- * Its underlying data structure is vector of Post structures.
- * Each index of vector corresponds to one state, that is a number of
- * state is an index to the vector of Posts.
- */
-struct Delta {
-private:
-    std::vector<Post> posts;
-
-public:
-    inline static const Post empty_post; // When posts[q] is not allocated, then delta[q] returns this.
-
-    Delta() : posts() {}
-    explicit Delta(size_t n) : posts(n) {}
-
-    void reserve(size_t n) {
-        posts.reserve(n);
-    };
-
-    /**
-     * Size of delta is number of all transitions, i.e. triples of form (state, symbol, state)
-     */
-    size_t size() const;
-
-    // Get a non const reference to post of a state, which allows modifying the post.
-    //
-    // BEWARE, IT HAS A SIDE EFFECT.
-    //
-    // Namely, it allocates the post of the state if it was not allocated yet. This in turn may cause that
-    // the entire post data structure is re-allocated, iterators to it get invalidated ...
-    // Use the constant [] operator below if possible.
-    // Or, to prevent the side effect from happening, one might want to make sure that posts of all states in the automaton
-    // are allocated, e.g., write an NFA method that allocate delta for all states of the NFA.
-    // But it feels fragile, before doing something like that, better think and talk to people.
-    Post& get_mutable_post(State q);
-
-    void defragment(const BoolVector& is_staying, const std::vector<State>& renaming);
-
-    // Get a constant reference to the post of a state. No side effects.
-    const Post & operator[] (State q) const;
-
-    void emplace_back() { posts.emplace_back(); }
-
-    void clear() { posts.clear(); }
-
-    void increase_size(size_t n) {
-        assert(n >= posts.size());
-        posts.resize(n);
-    }
-
-    /**
-     * @return Number of states in the whole Delta, including both source and target states.
-     */
-    size_t num_of_states() const { return posts.size(); }
-
-    void add(State state_from, Symbol symbol, State state_to);
-    void add(const Trans& trans) { add(trans.src, trans.symb, trans.tgt); }
-    void remove(State src, Symbol symb, State tgt);
-    void remove(const Trans& trans) { remove(trans.src, trans.symb, trans.tgt); }
-
-    bool contains(State src, Symbol symb, State tgt) const;
-
-    /**
-     * Check whether automaton contains no transitions.
-     * @return True if there are no transitions in the automaton, false otherwise.
-     */
-    bool empty() const;
-
-    /**
-     * @brief Append post vector to the delta.
-     * 
-     * @param post_vector Vector of posts to be appended.
-     */
-    void append(const std::vector<Post>& post_vector) {
-        for(const Post& pst : post_vector) {
-            this->posts.push_back(pst);
-        }
-    }
-
-    /**
-     * @brief Copy posts of delta and apply a lambda update function on each state from 
-     * targets. 
-     * 
-     * IMPORTANT: In order to work properly, the lambda function needs to be 
-     * monotonic. 
-     * 
-     * @param lambda Monotonic lambda function mapping states to different states
-     * @return std::vector<Post> Copied posts.
-     */
-    std::vector<Post> transform(const std::function<State(State)>& lambda) const;
-
-    /**
-     * @brief Add transitions to multiple destinations
-     * 
-     * @param state_from From
-     * @param symbol Symbol
-     * @param states Set of states to
-     */
-    void add(const State state_from, const Symbol symbol, const StateSet& states);
-
-    /**
-     * Iterator over transitions. It iterates over triples (lhs, symbol, rhs) where lhs and rhs are states.
-     */
-    struct const_iterator {
-    private:
-        const std::vector<Post>& post;
-        size_t current_state;
-        Post::const_iterator post_iterator{};
-        StateSet::const_iterator targets_position{};
-        bool is_end;
-
-    public:
-        using iterator_category = std::bidirectional_iterator_tag;
-        using value_type = int;
-        using difference_type = int;
-        using pointer = int*;
-        using reference = int&;
-
-        explicit const_iterator(const std::vector<Post>& post_p, bool ise = false);
-
-        const_iterator(const std::vector<Post>& post_p, size_t as,
-                       Post::const_iterator pi, StateSet::const_iterator ti, bool ise = false) :
-                post(post_p), current_state(as), post_iterator(pi), targets_position(ti), is_end(ise) {};
-
-        const_iterator(const const_iterator& other) = default;
-
-        Trans operator*() const { return Trans{current_state, (*post_iterator).symbol, *targets_position}; }
-
-        // Prefix increment
-        const_iterator& operator++();
-        // Postfix increment
-        const const_iterator operator++(int);
-
-        const_iterator& operator=(const const_iterator& x);
-
-        friend bool operator==(const const_iterator& a, const const_iterator& b);
-        friend bool operator!=(const const_iterator& a, const const_iterator& b) { return !(a == b); };
-    };
-
-    const_iterator cbegin() const { return const_iterator(posts); }
-    const_iterator cend() const { return const_iterator(posts, true); }
-    const_iterator begin() const { return cbegin(); }
-    const_iterator end() const { return cend(); }
-
-private:
-    State find_max_state();
-}; // struct Delta.
-
-bool operator==(const Delta::const_iterator& a, const Delta::const_iterator& b);
-
-/// An epsilon symbol which is now defined as the maximal value of data type used for symbols.
-constexpr Symbol EPSILON = Limits::max_symbol;
 
 /**
  * A struct representing an NFA.
  */
 struct Nfa {
 public:
     /**
@@ -712,27 +390,14 @@
      *
      * The value of the already existing symbols will NOT be overwritten.
      */
     void add_symbols_to(OnTheFlyAlphabet& target_alphabet) const;
 }; // struct Nfa.
 
 /**
- * Create automaton accepting only epsilon string.
- */
-Nfa create_empty_string_nfa();
-
-/**
- * Create automaton accepting sigma star over the passed alphabet.
- *
- * @param[in] alphabet Alphabet to construct sigma star automaton with. When alphabet is left empty, the default empty
- *  alphabet is used, creating an automaton accepting only the empty string.
- */
-Nfa create_sigma_star_nfa(Alphabet* alphabet = new OnTheFlyAlphabet{});
-
-/**
   * Fill @p alphabet with symbols from @p nfa.
   * @param[in] nfa NFA with symbols to fill @p alphabet with.
   * @param[out] alphabet Alphabet to be filled with symbols from @p nfa.
   */
 void fill_alphabet(const Mata::Nfa::Nfa& nfa, Mata::OnTheFlyAlphabet& alphabet);
 
 // Adapted from: https://www.fluentcpp.com/2019/01/25/variadic-number-function-parameters-type/.
@@ -1069,45 +734,14 @@
  *  @c Word instance
  */
  // TODO: rename to something, but no idea to what.
  // Maybe we need some terminology - Symbols and Words are made of numbers.
  // What are the symbol names and their sequences?
 Run encode_word(const StringToSymbolMap& symbol_map, const std::vector<std::string>& input);
 
-/** Loads an automaton from Parsed object */
-Nfa construct(
-        const Mata::Parser::ParsedSection&   parsec,
-        Alphabet*                            alphabet,
-        StringToStateMap*                    state_map = nullptr);
-
-/** Loads an automaton from Parsed object */
-Nfa construct(
-        const Mata::IntermediateAut&         inter_aut,
-        Alphabet*                            alphabet,
-        StringToStateMap*                    state_map = nullptr);
-
-template <class ParsedObject>
-Nfa construct(
-        const ParsedObject&                  parsed,
-        StringToSymbolMap*                   symbol_map = nullptr,
-        StringToStateMap*                    state_map = nullptr) {
-    StringToSymbolMap tmp_symbol_map;
-    if (symbol_map) {
-        tmp_symbol_map = *symbol_map;
-    }
-    Mata::OnTheFlyAlphabet alphabet(tmp_symbol_map);
-
-    Nfa aut = construct(parsed, &alphabet, state_map);
-
-    if (symbol_map) {
-        *symbol_map = alphabet.get_symbol_map();
-    }
-    return aut;
-} // construct().
-
 } // namespace Mata::Nfa.
 
 namespace std {
 template <>
 struct hash<Mata::Nfa::Trans> {
 	inline size_t operator()(const Mata::Nfa::Trans& trans) const {
 		size_t accum = std::hash<Mata::Nfa::State>{}(trans.src);
```

### Comparing `libmata-0.79.1/mata/include/mata/number-predicate.hh` & `libmata-0.80.0/mata/include/mata/utils/number-predicate.hh`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 // Created by Lukáš Holík on 06.12.2022.
 //
 
 #ifndef LIBMATA_NUMBER_PREDICATE_HH
 #define LIBMATA_NUMBER_PREDICATE_HH
 
 #include <vector>
-#include <mata/ord-vector.hh>
+
+#include "ord-vector.hh"
 
 namespace Mata::Util {
 
 template <class Number> class OrdVector;
 
 /**
  * @brief An enhanced boolean array, implementing a set of numbers, aka a unary predicate over numbers, that provides a
```

### Comparing `libmata-0.79.1/mata/include/mata/ord-vector.hh` & `libmata-0.80.0/mata/include/mata/utils/ord-vector.hh`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #ifndef MATA_ORD_VECTOR_HH_
 #define MATA_ORD_VECTOR_HH_
 
 #include <vector>
 #include <algorithm>
 #include <cassert>
 
-#include "mata/util.hh"
+#include "util.hh"
 
 namespace {
 /**
  * @brief  Converts an object to string
  *
  * Static method for conversion of an object of any class with the << output
  * operator into a string
```

### Comparing `libmata-0.79.1/mata/include/mata/parser.hh` & `libmata-0.80.0/mata/include/mata/parser/parser.hh`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #include <cassert>
 #include <list>
 #include <map>
 #include <ostream>
 #include <string>
 #include <vector>
 
-#include "mata/util.hh"
+#include "mata/utils/util.hh"
 
 /**
  * Parser from `.mata` format to automata (currently `Nfa` and `Afa` are supported).
  *
  * This includes parsing either from files or from other streams (strings, etc.).
  */
 namespace Mata::Parser {
```

### Comparing `libmata-0.79.1/mata/include/mata/re2parser.hh` & `libmata-0.80.0/mata/include/mata/parser/re2parser.hh`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  */
 
 #ifndef MATA_RE2PARSER_HH
 #define MATA_RE2PARSER_HH
 
 #include <string>
 
-#include "mata/nfa.hh"
+#include "mata/nfa/nfa.hh"
 
 /**
  * @brief Parser from regular expression to automata.
  *
  * Currently supported automata types are NFA and AFA.
  */
 namespace Mata::Parser {
```

### Comparing `libmata-0.79.1/mata/include/mata/sparse-set.hh` & `libmata-0.80.0/mata/include/mata/utils/sparse-set.hh`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 #include <concepts>
 #include <iterator>
 #include <cassert>
 #include <vector>
 #include <type_traits>
 
-#include "mata/ord-vector.hh"
+#include "ord-vector.hh"
 
 namespace Mata::Util {
 
 template <typename T>
 concept Iterable = requires(T t) {
     typename std::iterator_traits<decltype(begin(t))>::value_type;
     { begin(t) } -> std::same_as<decltype(end(t))>;
```

### Comparing `libmata-0.79.1/mata/include/mata/synchronized-iterator.hh` & `libmata-0.80.0/mata/include/mata/utils/synchronized-iterator.hh`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #ifndef MATA_SYNCHRONIZED_ITERATOR_HH
 #define MATA_SYNCHRONIZED_ITERATOR_HH
 
-#include "mata/ord-vector.hh"
+#include "ord-vector.hh"
 
 namespace Mata::Util {
 
 /**
  * Two classes that provide "synchronized" iterators through a vector of ordered vectors,
  * (or of some ordered OrdContainer that have a similar iterator),
  * needed in computation of post
```

### Comparing `libmata-0.79.1/mata/include/mata/util.hh` & `libmata-0.80.0/mata/include/mata/utils/util.hh`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#ifndef _MATA_UTIL_HH_
-#define _MATA_UTIL_HH_
+#ifndef MATA_UTIL_HH_
+#define MATA_UTIL_HH_
 
 #include <algorithm>
 #include <functional>
 #include <iostream>
 #include <list>
 #include <map>
 #include <set>
@@ -580,8 +580,8 @@
 
         // remove duplicates
         auto it = std::unique(vec.begin(), vec.end());
         vec.reserve(static_cast<size_t>(it - vec.begin()));
     }
 }
 }
-#endif /* _MATA_UTIL_HH_ */
+#endif /* MATA_UTIL_HH_ */
```

### Comparing `libmata-0.79.1/mata/src/afa/afa.cc` & `libmata-0.80.0/mata/src/afa/afa.cc`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 #include <algorithm>
 #include <list>
 #include <unordered_set>
 #include <memory>
 #include <queue>
 
 // MATA headers
-#include <mata/afa.hh>
+#include "mata/afa/afa.hh"
 
 using std::tie;
 
 using namespace Mata::Util;
 using namespace Mata::Afa;
 
 const std::string Mata::Afa::TYPE_AFA = "AFA";
```

### Comparing `libmata-0.79.1/mata/src/alphabet.cc` & `libmata-0.80.0/mata/src/alphabet.cc`

 * *Files identical despite different names*

### Comparing `libmata-0.79.1/mata/src/inter-aut.cc` & `libmata-0.80.0/mata/src/inter-aut.cc`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include "mata/inter-aut.hh"
+#include "mata/parser/inter-aut.hh"
 
 namespace {
     bool has_atmost_one_auto_naming(const Mata::IntermediateAut& aut)
     {
         return !(!(aut.node_naming == Mata::IntermediateAut::Naming::AUTO &&
               aut.symbol_naming == Mata::IntermediateAut::Naming::AUTO) &&
                  (aut.state_naming == Mata::IntermediateAut::Naming::AUTO));
```

### Comparing `libmata-0.79.1/mata/src/mintermization.cc` & `libmata-0.80.0/mata/src/mintermization.cc`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include "mata/mintermization.hh"
+#include "mata/parser/mintermization.hh"
 
 namespace {
     const Mata::FormulaGraph* detect_state_part(const Mata::FormulaGraph* node)
     {
         if (node->node.is_state())
             return node;
```

### Comparing `libmata-0.79.1/mata/src/nfa/nfa-complement.cc` & `libmata-0.80.0/mata/src/nfa/complement.cc`

 * *Files 2% similar despite different names*

```diff
@@ -12,16 +12,16 @@
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 // MATA headers
-#include <mata/nfa.hh>
-#include <mata/nfa-algorithms.hh>
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Util;
 
 Nfa Mata::Nfa::Algorithms::complement_classical(const Nfa& aut, const OrdVector<Symbol>& symbols,
                                                 bool minimize_during_determinization) {
     Nfa result;
```

### Comparing `libmata-0.79.1/mata/src/nfa/nfa-concatenation.cc` & `libmata-0.80.0/mata/src/nfa/concatenation.cc`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,16 @@
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 // MATA headers
-#include <mata/nfa.hh>
-#include <mata/nfa-algorithms.hh>
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
 
 using namespace Mata::Nfa;
 
 namespace Mata::Nfa {
 
 Nfa concatenate(const Nfa& lhs, const Nfa& rhs, bool use_epsilon,
                 StateToStateMap* lhs_result_states_map, StateToStateMap* rhs_result_states_map) {
```

### Comparing `libmata-0.79.1/mata/src/nfa/nfa-inclusion.cc` & `libmata-0.80.0/mata/src/nfa/inclusion.cc`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 // MATA headers
-#include <mata/nfa.hh>
-#include <mata/nfa-algorithms.hh>
-#include <mata/sparse-set.hh>
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/utils/sparse-set.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Util;
 
 /// naive language inclusion check (complementation + intersection + emptiness)
 bool Mata::Nfa::Algorithms::is_included_naive(
         const Nfa &smaller,
```

### Comparing `libmata-0.79.1/mata/src/nfa/nfa-intersection.cc` & `libmata-0.80.0/mata/src/nfa/intersection.cc`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 // MATA headers
-#include <mata/nfa.hh>
-#include <mata/nfa-algorithms.hh>
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
 
 using namespace Mata::Nfa;
 
 namespace {
 
 /**
  * Add transition to the product.
```

### Comparing `libmata-0.79.1/mata/src/nfa/nfa-universal.cc` & `libmata-0.80.0/mata/src/nfa/universal.cc`

 * *Files 2% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 // MATA headers
-#include <mata/nfa.hh>
-#include <mata/nfa-algorithms.hh>
-#include <mata/sparse-set.hh>
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/algorithms.hh"
+#include "mata/utils/sparse-set.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Util;
 
 //TODO: this could be merged with inclusion, or even removed, universality could be implemented using inclusion,
 // it is not something needed in practice, so some little overhead is ok
```

### Comparing `libmata-0.79.1/mata/src/parser.cc` & `libmata-0.80.0/mata/src/parser.cc`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,16 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include <mata/parser.hh>
-#include <mata/util.hh>
+#include "mata/parser/parser.hh"
+#include "mata/utils/util.hh"
 
 #include <algorithm>
 #include <cstring>
 #include <sstream>
 
 using std::tie;
```

### Comparing `libmata-0.79.1/mata/src/re2parser.cc` & `libmata-0.80.0/mata/src/re2parser.cc`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
 #include <iostream>
 
 #include "mata/alphabet.hh"
-#include "mata/nfa.hh"
-#include "mata/re2parser.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/parser/re2parser.hh"
 #include "re2/re2/regexp.h"
 #include "re2/re2/prog.h"
 
 namespace {
     class RegexParser {
     private:
         /**
```

### Comparing `libmata-0.79.1/mata/src/strings/nfa-noodlification.cc` & `libmata-0.80.0/mata/src/strings/nfa-noodlification.cc`

 * *Files 0% similar despite different names*

```diff
@@ -11,18 +11,18 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
  * GNU General Public License for more details.
  */
 
-#include "mata/nfa.hh"
-#include "mata/nfa-strings.hh"
-#include "mata/util.hh"
-#include <mata/nfa-algorithms.hh>
+#include "mata/utils/util.hh"
+#include "mata/nfa/nfa.hh"
+#include "mata/nfa/strings.hh"
+#include "mata/nfa/algorithms.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Strings;
 using namespace Mata::Nfa::Algorithms;
 
 namespace {
```

### Comparing `libmata-0.79.1/mata/src/strings/nfa-segmentation.cc` & `libmata-0.80.0/mata/src/strings/nfa-segmentation.cc`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include "mata/nfa-strings.hh"
+#include "mata/nfa/strings.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Strings;
 
 void SegNfa::Segmentation::process_state_depth_pair(const StateDepthTuple& state_depth_pair,
                                                     std::deque<StateDepthTuple>& worklist) {
     auto outgoing_post{ automaton.delta[state_depth_pair.state] };
```

### Comparing `libmata-0.79.1/mata/src/strings/nfa-strings.cc` & `libmata-0.80.0/mata/src/strings/nfa-strings.cc`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
  *
  * This program is distributed in the hope that it will be useful,
  * but WITHOUT ANY WARRANTY; without even the implied warranty of
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  */
 
-#include "mata/nfa-strings.hh"
+#include "mata/nfa/strings.hh"
+#include "mata/nfa/builder.hh"
 
 using namespace Mata::Nfa;
 using namespace Mata::Strings;
 
 WordSet Mata::Strings::get_shortest_words(const Nfa::Nfa& nfa) {
     // Map mapping states to a set of the shortest words accepted by the automaton from the mapped state.
     // Get the shortest words for all initial states accepted by the whole automaton (not just a part of the automaton).
@@ -207,30 +208,7 @@
         if(!tr_aut.final[ini])
             return false;
         if(tr_aut.delta[ini].size() > 0)
             return false;
     }
     return true;
 }
-
-Nfa Mata::Strings::create_single_word_nfa(const std::vector<Mata::Symbol>& word) {
-    const size_t word_size{ word.size() };
-    Nfa::Nfa nfa{ word_size + 1, { 0 }, { word_size } };
-
-    for (State state{ 0 }; state < word_size; ++state) {
-        nfa.delta.add(state, word[state], state + 1);
-    }
-    return nfa;
-}
-
-Nfa Mata::Strings::create_single_word_nfa(const std::vector<std::string>& word, Mata::Alphabet *alphabet) {
-    if (!alphabet) {
-        alphabet = new OnTheFlyAlphabet{ word };
-    }
-    const size_t word_size{ word.size() };
-    Nfa::Nfa nfa{ word_size + 1, { 0 }, { word_size }, alphabet };
-
-    for (State state{ 0 }; state < word_size; ++state) {
-        nfa.delta.add(state, alphabet->translate_symb(word[state]), state + 1);
-    }
-    return nfa;
-}
```

### Comparing `libmata-0.79.1/setup.py` & `libmata-0.80.0/setup.py`

 * *Files identical despite different names*

