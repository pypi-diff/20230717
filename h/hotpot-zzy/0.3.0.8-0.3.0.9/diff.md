# Comparing `tmp/hotpot-zzy-0.3.0.8.tar.gz` & `tmp/hotpot-zzy-0.3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/zz1/hotpot/dist/.tmp-qskjt3wf/hotpot-zzy-0.3.0.8.tar", last modified: Tue Jul  4 06:24:40 2023, max compression
+gzip compressed data, was "hotpot-zzy-0.3.0.9.tar", last modified: Fri Jul  7 05:50:26 2023, max compression
```

## Comparing `hotpot-zzy-0.3.0.8.tar` & `hotpot-zzy-0.3.0.9.tar`

### file list

```diff
@@ -1,127 +1,127 @@
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/LICENSE
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       17 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/MANIFEST.in
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     6643 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/README.md
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.564325 hotpot-zzy-0.3.0.8/hotpot/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      419 2023-07-04 06:17:05.000000 hotpot-zzy-0.3.0.8/hotpot/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    36575 2023-07-04 06:09:00.000000 hotpot-zzy-0.3.0.8/hotpot/_io.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    25799 2023-07-04 06:05:29.000000 hotpot-zzy-0.3.0.8/hotpot/bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   113273 2023-07-04 04:34:02.000000 hotpot-zzy-0.3.0.8/hotpot/cheminfo.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/atom_single_point.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/deepmd_script.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/LJ.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.568325 hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/SiC.tersoff
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/force_field/contents.json
--rw-rw-r--   0 zz1       (1005) zz1       (1008)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/periodic_table.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.584325 hotpot-zzy-0.3.0.8/hotpot/data/solvents/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,2-trichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-diethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dimethoxymethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dimethoxyethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,4-dioxane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-pentanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2,2-dimethoxypropane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-ethoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methoxyethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyl-1-propanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/3-methyl-1-butanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DCM.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMSO.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/N,N-dimethylacetamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/N-methylpyrrolidone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/THF.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetonitrile.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/benzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/butylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/carbon_tetrachloride.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/chlorobenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/chloroform.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/cumene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/cyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/diethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/diisopropylamine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyl_formate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyleneglycol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/formamide.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/formic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/heptane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/hexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isobutyl_acetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isooctane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/meta-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methanol.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methoxybenzene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylbutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylcyclohexane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylethylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisobutylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisopropylketone.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/morpholine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/nitromethane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/ortho-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/para-xylene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/pentane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/propylacetate.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/pyridine.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/sulfolane.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/t-butylmethylether.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/tetralin.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/toluene.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/trichloroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/trifluoroacetic_acid.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/solvents/water.mol2
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/data/units.json
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.584325 hotpot-zzy-0.3.0.8/hotpot/tanks/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)    10245 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/cc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8070 2023-07-04 05:01:45.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/deepmd.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/features.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/base.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/gcmc.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     9158 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/materials.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     8896 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tanks/quantum.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tmo.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/tools.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot/utils/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/__init__.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.0.8/hotpot/utils/library.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/manage_machine.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/hotpot/utils/units_convert.py
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      382 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/PKG-INFO
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3941 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/SOURCES.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        1 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/dependency_links.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       44 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/requires.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)        7 2023-07-04 06:24:40.000000 hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/top_level.txt
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      656 2023-07-04 06:17:05.000000 hotpot-zzy-0.3.0.8/pyproject.toml
--rw-rw-r--   0 zz1       (1005) zz1       (1008)       38 2023-07-04 06:24:40.592325 hotpot-zzy-0.3.0.8/setup.cfg
-drwxrwxr-x   0 zz1       (1005) zz1       (1008)        0 2023-07-04 06:24:40.588325 hotpot-zzy-0.3.0.8/test/
--rw-rw-r--   0 zz1       (1005) zz1       (1008)      533 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_amorphous_maker.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     1812 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_bundle.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     3095 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_chemif.py
--rw-rw-r--   0 zz1       (1005) zz1       (1008)     6853 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.8/test/test_lmp.py
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.309484 hotpot-zzy-0.3.0.9/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1070 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/LICENSE
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)       17 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/MANIFEST.in
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      449 2023-07-07 05:50:26.308484 hotpot-zzy-0.3.0.9/PKG-INFO
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     6643 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/README.md
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.095516 hotpot-zzy-0.3.0.9/hotpot/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      419 2023-07-07 05:38:01.000000 hotpot-zzy-0.3.0.9/hotpot/__init__.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)    36575 2023-07-04 06:09:00.000000 hotpot-zzy-0.3.0.9/hotpot/_io.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)    25800 2023-07-04 07:52:05.000000 hotpot-zzy-0.3.0.9/hotpot/bundle.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)   112109 2023-07-06 06:16:21.000000 hotpot-zzy-0.3.0.9/hotpot/cheminfo.py
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.146257 hotpot-zzy-0.3.0.9/hotpot/data/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)       65 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/atom_single_point.json
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1874 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/deepmd_script.json
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.160364 hotpot-zzy-0.3.0.9/hotpot/data/force_field/
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.177362 hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     4606 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/LJ.json
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:25.195362 hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1701 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/SiC.tersoff
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)       82 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/force_field/contents.json
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)   231681 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/periodic_table.json
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.097163 hotpot-zzy-0.3.0.9/hotpot/data/solvents/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      946 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trichloroethane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1039 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trifluroethanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      760 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,2-trichloroethene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dichloroethene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2525 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-diethoxypropane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1410 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dimethoxymethane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      943 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      757 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1688 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dimethoxyethane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1518 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,4-dioxane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-butanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1865 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-pentanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1307 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-propanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2,2-dimethoxypropane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1585 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-butanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1684 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-ethoxyethanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1406 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methoxyethanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1595 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyl-1-propanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1716 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyltetrahydrofuran.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/3-methyl-1-butanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      649 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DCM.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1300 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMF.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1115 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMSO.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1597 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/N,N-dimethylacetamide.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1712 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/N-methylpyrrolidone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1417 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/THF.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      936 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetic_acid.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1118 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      751 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetonitrile.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1328 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/benzene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2053 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/butylacetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      666 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/carbon_tetrachloride.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1334 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/chlorobenzene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      656 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/chloroform.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2164 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/cumene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/cyclohexane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1588 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/diethylether.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2243 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/diisopropylamine.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1025 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyl_formate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1495 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethylacetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyleneglycol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      748 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/formamide.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      657 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/formic_acid.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2327 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/heptane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2047 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/hexane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2057 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isobutyl_acetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2608 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isooctane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1308 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1778 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylacetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2148 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylether.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/meta-xylene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      747 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methanol.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1707 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methoxybenzene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1217 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylacetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1965 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylbutylketone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2175 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylcyclohexane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1407 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylethylketone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1968 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisobutylketone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1690 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisopropylketone.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1610 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/morpholine.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      844 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/nitromethane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1891 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/ortho-xylene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1890 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/para-xylene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1769 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/pentane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1775 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/propylacetate.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1236 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/pyridine.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1609 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/sulfolane.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1873 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/t-butylmethylether.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2283 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/tetralin.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1607 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/toluene.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/trichloroacetic_acid.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      945 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/trifluoroacetic_acid.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      465 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/solvents/water.mol2
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      182 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/data/units.json
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.145492 hotpot-zzy-0.3.0.9/hotpot/tanks/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      205 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/__init__.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)    10283 2023-07-06 05:53:15.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/cc.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     8140 2023-07-06 01:38:16.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/deepmd.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      149 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/features.py
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.193897 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      269 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/__init__.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     7862 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/base.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     8553 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/gcmc.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     9158 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/materials.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)    16656 2023-07-06 09:21:59.000000 hotpot-zzy-0.3.0.9/hotpot/tanks/quantum.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2838 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tmo.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     2805 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/tools.py
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.232231 hotpot-zzy-0.3.0.9/hotpot/utils/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      125 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/__init__.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3979 2023-07-03 10:51:41.000000 hotpot-zzy-0.3.0.9/hotpot/utils/library.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1403 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/manage_machine.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      642 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/hotpot/utils/units_convert.py
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.269851 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      449 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/PKG-INFO
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3941 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)        1 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)       44 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/requires.txt
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)        7 2023-07-07 05:50:24.000000 hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/top_level.txt
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      731 2023-07-07 05:38:01.000000 hotpot-zzy-0.3.0.9/pyproject.toml
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)       38 2023-07-07 05:50:26.309484 hotpot-zzy-0.3.0.9/setup.cfg
+drwxrwxrwx   0 zzy       (1000) zzy       (1000)        0 2023-07-07 05:50:26.299484 hotpot-zzy-0.3.0.9/test/
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)      533 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_amorphous_maker.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     1812 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_bundle.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     3095 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_chemif.py
+-rwxrwxrwx   0 zzy       (1000) zzy       (1000)     6853 2023-07-03 02:49:38.000000 hotpot-zzy-0.3.0.9/test/test_lmp.py
```

### Comparing `hotpot-zzy-0.3.0.8/LICENSE` & `hotpot-zzy-0.3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/README.md` & `hotpot-zzy-0.3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/_io.py` & `hotpot-zzy-0.3.0.9/hotpot/_io.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/bundle.py` & `hotpot-zzy-0.3.0.9/hotpot/bundle.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,26 +577,25 @@
                 mol_save_root = \
                     save_root.joinpath(str(m.atom_counts)) if mode == 'att' else system_dir.joinpath(str(c))
                 if not mol_save_root.exists():
                     mol_save_root.mkdir()
 
                 m.to_dpmd_sys(mol_save_root, mode)
 
-
         if split_mode and split_mode not in ['inside', 'outside']:
             raise ValueError("the split_mode must be 'inside' or 'outside'")
 
         if not 0.0 < validate_ratio < 1.0:
             raise ValueError('the validate_ratio must be from 0.0 to 1.0')
 
         # Organize dirs
         if not isinstance(system_dir, Path):
             system_dir = Path(system_dir)
-        training_dir = system_dir.joinpath('training_dir')
-        validate_dir = system_dir.joinpath('validate_dir')
+        training_dir = system_dir.joinpath('training_data')
+        validate_dir = system_dir.joinpath('validate_data')
         if not training_dir.exists():
             training_dir.mkdir()
         if not validate_dir.exists():
             validate_dir.mkdir()
 
         if mode == 'att':
             bundle = self.merge_atoms_same_mols()
```

### Comparing `hotpot-zzy-0.3.0.8/hotpot/cheminfo.py` & `hotpot-zzy-0.3.0.9/hotpot/cheminfo.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-python v3.7.9
+python v3.9.0
 @Project: hotpot
 @File   : cheminfo.py
 @Author : Zhiyuan Zhang
 @Date   : 2023/3/14
 @Time   : 4:09
 """
 import copy
@@ -24,14 +24,15 @@
 from rdkit.Chem import Draw
 
 from hotpot import data_root
 from hotpot.tanks import lmp
 from hotpot.tanks.quantum import Gaussian, GaussianRunError
 from hotpot.utils.library import library as _lib  # The chemical library
 
+
 # Define Exceptions
 class OperateOBMolFail(BaseException):
     """ Raise for any fail that trys to operate the OBMol """
 
 
 class AddAtomFail(OperateOBMolFail):
     """ Raise when add an atom into Molecule fail """
@@ -196,15 +197,15 @@
         # the items are ranked by the number of values for each atom, for example:
         #   - the all_atom_charges and atom_spin_densities have 1 value for each atom, so they are placed in the second
         #     item (with the index 1)
         #   - the coordinates have 3 values for each atom, i.e., [x, y, z], so it is placed in the forth
         #     item (with the index 3）
         # For the molecular attributes, which have only one value for each conformer and represent the attribute
         # of whole molecule, they are place in the first item (with the index 0)
-        ('all_energy',),
+        ('all_energy', 'identifier_array'),
         ('all_atom_charges', 'all_atom_spin_densities'),
         (),
         ('all_coordinates', 'all_forces')
     )
 
     def __init__(self, ob_mol: ob.OBMol = None, _data: dict = None, **kwargs):
         if _data:
@@ -1359,52 +1360,51 @@
                     break
 
         # Make the input gjf script
         script = self.dump('gjf', *args, link0=link0, route=route, **kwargs)
 
         # Run Gaussian16
         with Gaussian(g16root) as gaussian:
-            stdout, stderr = gaussian.run(script)
 
-            # If got an error message, save the error
-            if stderr:
+            try:
+                stdout, stderr = gaussian.run(script)
+
+                # save the calculate result into the molecule data dict
+                self._data['gaussian_output'] = stdout
+                self._data['gaussian_parse_data'] = gaussian.parse_log(stdout)
+
+                # Inplace the self attribute according to the result from gaussian
+                if inplace_attrs:
+                    self._set_attrs(**gaussian.molecule_setter_dict(stdout))
+
+                # Save log file when the path_log_file has been specified
+                if path_log_file:
+                    with open(path_log_file, 'w') as writer:
+                        writer.write(stdout)
+
+                # return results and error info
+                return stdout, stderr
+
+            # If got an error message, save the error and stdout file, before raise the error
+            except GaussianRunError:
+                stdout, stderr = gaussian.stdout, gaussian.stderr
+
                 # Save error file
                 if not path_err_file:
                     path_err_file = Path(f'{self.formula}.err')
                 with open(path_err_file, 'w') as writer:
                     writer.write(stderr)
 
                 # Save log file
                 if not path_log_file:
                     path_log_file = Path(f'{self.formula}.log')
                 with open(path_log_file, 'w') as writer:
                     writer.write(stdout)
 
-                raise GaussianRunError(
-                    f'Encourage error when Gaussian is running!\n'
-                    f'Check the Error file in {str(path_err_file.absolute())}\n'
-                    f'Check the output.log file in {str(path_log_file.absolute())}\n'
-                    f'Error massage from gaussian:\n{stderr}'
-                )
-
-            # save the calculate result into the molecule data dict
-            self._data['gaussian_output'] = stdout
-            self._data['gaussian_parse_data'] = gaussian.data
-
-            # Inplace the self attribute according to the result from gaussian
-            if inplace_attrs:
-                self._set_attrs(**gaussian.molecule_setter_dict)
-
-        # Save log file
-        if path_log_file:
-            with open(path_log_file, 'w') as writer:
-                writer.write(stdout)
-
-        # return results and error info
-        return stdout, stderr
+                raise GaussianRunError(stderr)
 
     def gcmc(
             self, *guest: 'Molecule', force_field: Union[str, os.PathLike] = None,
             work_dir: Union[str, os.PathLike] = None, T: float = 298.15, P: float = 1.0, **kwargs
     ):
         """
         Run gcmc to determine the adsorption of guest,
@@ -1573,14 +1573,26 @@
     def identifier(self):
         return self.ob_mol.GetTitle()
 
     @identifier.setter
     def identifier(self, value):
         self.ob_mol.SetTitle(value)
 
+    @property
+    def identifier_array(self) -> np.ndarray:
+        """ numpy.array of identifiers has the same number of items with the number of conformers """
+        idt_array = self._data.get('identifier_array')
+        if not isinstance(idt_array, np.ndarray):
+            idt_array = []
+            for i, c in enumerate(self.all_coordinates):
+                idt_array.append(f'{self.identifier}_c{i}')
+            self._data['identifier_array'] = idt_array = np.array(idt_array)
+
+        return idt_array
+
     def iadd_accessible(self, other):
         if self.atomic_numbers == other.atomic_numbers:
             return True
         return False
 
     @property
     def inchi(self):
@@ -2081,58 +2093,17 @@
         Args:
             system_dir: the dir for all system data store, if the validate_dir has been given, this is the dir of
              training system
             mode: the system mode, choose from att or std
             validate_ratio(float): the ratio of validate data set.
             validate_dir(str|Path): if validate_ratio has been specified, this must be given
         """
-        # dpmd_sys_root = Path(dpmd_sys_root)
-        # if not dpmd_sys_root.exists():
-        #     dpmd_sys_root.mkdir()
-        #
-        # # the dir of set data
-        # set_root = dpmd_sys_root.joinpath('set.000')
-        # if not set_root.exists():
-        #     set_root.mkdir()
-
         system: DeepSystem = self.dump('dpmd_sys')
         system(system_dir, mode, validate_ratio, validate_dir)
 
-        # for name, value in data.items():
-        #
-        #     # if the value is None, go to next
-        #     if value is None:
-        #         continue
-        #
-        #     # Write the type raw
-        #     if name == 'type':
-        #         if mode == 'std':
-        #             type_raw = value[0]
-        #         elif mode == 'att':
-        #             type_raw = np.zeros(value[0].shape, dtype=int)
-        #             np.save(set_root.joinpath("real_atom_types.npy"), value)
-        #         else:
-        #             raise ValueError('the mode just allows to be "std" or "att"')
-        #
-        #         with open(dpmd_sys_root.joinpath('type.raw'), 'w') as writer:
-        #             writer.write('\n'.join([str(i) for i in type_raw]))
-        #
-        #     elif name == 'type_map':
-        #         with open(dpmd_sys_root.joinpath('type_map.raw'), 'w') as writer:
-        #             writer.write('\n'.join([str(i) for i in value]))
-        #
-        #     # Create an empty 'nopbc', when the system is not periodical
-        #     elif name == 'nopbc' and value is True:
-        #         with open(dpmd_sys_root.joinpath('nopbc'), 'w') as writer:
-        #             writer.write('')
-        #
-        #     # Save the numpy format data
-        #     elif isinstance(value, np.ndarray):
-        #         np.save(str(set_root.joinpath(f'{name}.npy')), value)
-
     def to_mix_mol(self):
         """ Convert this Molecule object to MixSaveAtomMol """
         return MixSameAtomMol(_data=self._data)
 
     def to_rdmol(self):
         """ convert hotpot Molecule object to RdKit mol object """
         return Chem.MolFromMol2Block(self.dump('mol2'))
@@ -2928,14 +2899,18 @@
 
     @property
     def degree(self):
         ob_atoms = [a.ob_atom for a in self.atoms]
         return self.molecule.ob_mol.GetAngle(*ob_atoms)
 
 
+class Torsion:
+    """"""
+
+
 class Crystal(Wrapper, ABC):
     """"""
     _lattice_type = (
         'Undefined', 'Triclinic', 'Monoclinic', 'Orthorhombic', 'Tetragonal', 'Rhombohedral', 'Hexagonal', 'Cubic'
     )
 
     def __init__(self, ob_unitcell: ob.OBUnitCell = None, **kwargs):
```

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/deepmd_script.json` & `hotpot-zzy-0.3.0.9/hotpot/data/deepmd_script.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/force_field/UFF/LJ.json` & `hotpot-zzy-0.3.0.9/hotpot/data/force_field/UFF/LJ.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/force_field/aMaterials/SiC.tersoff` & `hotpot-zzy-0.3.0.9/hotpot/data/force_field/aMaterials/SiC.tersoff`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/periodic_table.json` & `hotpot-zzy-0.3.0.9/hotpot/data/periodic_table.json`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trichloroethane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,1-trifluroethanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,1-trifluroethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1,2-trichloroethene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1,2-trichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dichloroethene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-diethoxypropane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-diethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,1-dimethoxymethane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,1-dimethoxymethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dichloroethene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dichloroethene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,2-dimethoxyethane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,2-dimethoxyethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1,4-dioxane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1,4-dioxane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-butanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-pentanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-pentanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/1-propanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2,2-dimethoxypropane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2,2-dimethoxypropane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-butanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-ethoxyethanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-ethoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methoxyethanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methoxyethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyl-1-propanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyl-1-propanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/2-methyltetrahydrofuran.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/2-methyltetrahydrofuran.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/3-methyl-1-butanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/3-methyl-1-butanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DCM.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DCM.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMF.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/DMSO.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/DMSO.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/N,N-dimethylacetamide.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/N,N-dimethylacetamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/N-methylpyrrolidone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/N-methylpyrrolidone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/THF.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/THF.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetic_acid.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/acetonitrile.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/acetonitrile.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/benzene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/benzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/butylacetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/butylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/carbon_tetrachloride.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/carbon_tetrachloride.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/chlorobenzene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/chlorobenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/chloroform.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/chloroform.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/cumene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/cumene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/cyclohexane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/cyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/diethylether.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/diethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/diisopropylamine.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/diisopropylamine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyl_formate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyl_formate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethylacetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ethyleneglycol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ethyleneglycol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/formamide.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/formamide.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/formic_acid.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/formic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/heptane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/heptane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/hexane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/hexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isobutyl_acetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isobutyl_acetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isooctane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isooctane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylacetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/isopropylether.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/isopropylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/meta-xylene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/meta-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methanol.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methanol.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methoxybenzene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methoxybenzene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylacetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylbutylketone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylbutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylcyclohexane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylcyclohexane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylethylketone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylethylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisobutylketone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisobutylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/methylisopropylketone.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/methylisopropylketone.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/morpholine.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/morpholine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/nitromethane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/nitromethane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/ortho-xylene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/ortho-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/para-xylene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/para-xylene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/pentane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/pentane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/propylacetate.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/propylacetate.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/pyridine.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/pyridine.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/sulfolane.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/sulfolane.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/t-butylmethylether.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/t-butylmethylether.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/tetralin.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/tetralin.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/toluene.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/toluene.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/trichloroacetic_acid.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/trichloroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/data/solvents/trifluoroacetic_acid.mol2` & `hotpot-zzy-0.3.0.9/hotpot/data/solvents/trifluoroacetic_acid.mol2`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tanks/cc.py` & `hotpot-zzy-0.3.0.9/hotpot/tanks/cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,16 @@
 
     @property
     def pairs(self):
         return self.mols
 
     def determine_metal_ligand_bind_energy(
             self, g16root: Union[str, os.PathLike], work_dir: Union[str, os.PathLike],
-            method: str = 'B3LYP', basis_set: str = '6-311', route: str = ''
+            method: str = 'B3LYP', basis_set: str = '6-311', route: str = '',
+            cpu_uti: float = 0.75
     ) -> pd.DataFrame:
         # Specify directories and make these dirs
         dirs_files = self._specify_dir_files(work_dir)
         dirs_files.make_dirs()
 
         # Energy sheet, bond dissociation energy (BDE) sheet
         e_sheet, bde_sheet = [], []
@@ -163,18 +164,18 @@
         # save the initialized ligand structure
         self.ligand.writefile('mol2', dirs_files.ligand_struct_path)
 
         # optimize the configure of ligand and calculate their total energy after optimization
         self.ligand.gaussian(
             g16root,
             link0=[
-                f'CPU=0-{machine.take_CPUs()-1}',
+                f'CPU=0-{machine.take_CPUs(cpu_uti)-1}',
                 f'Mem={machine.take_memory(0.25)}GB'
             ],
-            route=f'opt=recalc=5 {method}/{basis_set} ' + route,
+            route=f'opt {method}/{basis_set} ' + route,
             path_log_file=dirs_files.ligand_log_path,
             path_err_file=dirs_files.ligand_err_path,
             inplace_attrs=True
         )
 
         ligand_energy = self.ligand.energy  # Retrieve the energy after optimizing the conformer
         e_sheet.append(['ligand', self.ligand.smiles, ligand_energy])
@@ -185,15 +186,15 @@
         # Calculate the single point (sp) energy for metal
         try:
             metal_sp = _atom_single_point[self.metal.atoms[0].symbol][method][basis_set]
         except KeyError:
             self.metal.gaussian(
                 g16root,
                 link0=[
-                    f'CPU=0-{machine.take_CPUs()-1}',
+                    f'CPU=0-{machine.take_CPUs(cpu_uti)-1}',
                     f'Mem={machine.take_memory(0.25)}GB'
                 ],
                 route=f'{method}/{basis_set} ' + route,
                 path_log_file=dirs_files.metal_log_path,
                 path_err_file=dirs_files.ligand_err_path,
                 inplace_attrs=True
             )
@@ -216,18 +217,18 @@
             # Save initialized Metal-ligand pair struct
             pair.writefile('mol2', dirs_files.pair_struct_path(i))
 
             # Performing calculation
             pair.gaussian(
                 g16root,
                 link0=[
-                    f'CPU=0-{machine.take_CPUs()-1}',
+                    f'CPU=0-{machine.take_CPUs(cpu_uti)-1}',
                     f'Mem={machine.take_memory(0.25)}GB'
                 ],
-                route=f'opt=recalc=5 {method}/{basis_set} ' + route,
+                route=f'opt {method}/{basis_set} ' + route,
                 path_log_file=dirs_files.pair_log_path(i),
                 path_err_file=dirs_files.pair_err_path(i),
                 inplace_attrs=True
             )
 
             # Append the pairs energy values to energy sheet
             e_sheet.append([f'pair_{i}', pair.smiles, pair.energy])
```

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tanks/deepmd.py` & `hotpot-zzy-0.3.0.9/hotpot/tanks/deepmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     Args:
         mol(Molecule):
 
     """
 
     required_items = ('coord', 'type')
     check_atom_num = ('coord', 'force', 'charge')
-    share_same_conformers = ('type', 'coord', 'energy', 'force', 'charge', 'virial')
+    share_same_conformers = ('type', 'coord', 'energy', 'force', 'charge', 'virial', 'box', 'identifiers')
     need_reshape = ('coord', 'force')
 
     def __init__(self, mol: Molecule = None, data: dict = None):
         if mol:
             self.data = self._organize_data(mol)
             # check numpy.ndarray shape
             self._check_shape()
@@ -102,15 +102,15 @@
 
     def __getattr__(self, item: str):
         if item not in self.__dir__():
             raise AttributeError(f'the {self.__class__.__name__} not have attribute {item}')
         return self.data.get(item, None)
 
     def __dir__(self) -> Iterable[str]:
-        return  [
+        return [
             'type', 'type_map', 'nopbc', 'coord', 'box', 'energy', 'force', 'charge',
             'atom_counts','virial', 'atom_ener', 'atom_pref', 'dipole', 'atom_dipole',
             'polarizability', 'atomic_polarizability'
         ]
 
     def __len__(self):
         return len(self.data['coord'])
@@ -163,14 +163,15 @@
             'nopbc': not is_periodic,
             'coord': mol.all_coordinates,  # angstrom,
             'box': box,
             'energy': mol.all_energy,  # eV
             'force': mol.all_forces,  # Hartree/Bohr,
             'charge': mol.all_atom_charges,  # q
             'atom_counts': mol.atom_counts,
+            'identifiers': mol.identifier_array,
             'virial': None,
             'atom_ener': None,
             'atom_pref': None,
             'dipole': None,
             'atom_dipole': None,
             'polarizability': None,
             'atomic_polarizability': None
```

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/base.py` & `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/base.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/gcmc.py` & `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/gcmc.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tanks/lmp/materials.py` & `hotpot-zzy-0.3.0.9/hotpot/tanks/lmp/materials.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tmo.py` & `hotpot-zzy-0.3.0.9/hotpot/tmo.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/tools.py` & `hotpot-zzy-0.3.0.9/hotpot/tools.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/utils/library.py` & `hotpot-zzy-0.3.0.9/hotpot/utils/library.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/utils/manage_machine.py` & `hotpot-zzy-0.3.0.9/hotpot/utils/manage_machine.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot/utils/units_convert.py` & `hotpot-zzy-0.3.0.9/hotpot/utils/units_convert.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/hotpot_zzy.egg-info/SOURCES.txt` & `hotpot-zzy-0.3.0.9/hotpot_zzy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/pyproject.toml` & `hotpot-zzy-0.3.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hotpot-zzy"
-version = "0.3.0.8"
+version = "0.3.0.9"
 readme = "RAEDME.md"
 authors = [
     { name = "Zhiyuan Zhang", email = "ZhiyuanZhang_scu@163.com" },
     { name = "Yue Dong", email = "1320801310@qq.com" },
     { name = "Yuqing Qiu", email = "2022223070045@stu.scu.edu.cn" },
 ]
 classifiers = [
@@ -23,8 +23,11 @@
     "cclib",
     "tqdm",
     'rdkit',
     'psutil'
 ]
 
 [tool.setuptools]
-include-package-data = true
+include-package-data = true
+
+[project.urls]
+"Homepage" = "https://github.com/Zhang-Zhiyuan-zzy/hotpot"
```

### Comparing `hotpot-zzy-0.3.0.8/test/test_amorphous_maker.py` & `hotpot-zzy-0.3.0.9/test/test_amorphous_maker.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/test/test_bundle.py` & `hotpot-zzy-0.3.0.9/test/test_bundle.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/test/test_chemif.py` & `hotpot-zzy-0.3.0.9/test/test_chemif.py`

 * *Files identical despite different names*

### Comparing `hotpot-zzy-0.3.0.8/test/test_lmp.py` & `hotpot-zzy-0.3.0.9/test/test_lmp.py`

 * *Files identical despite different names*

