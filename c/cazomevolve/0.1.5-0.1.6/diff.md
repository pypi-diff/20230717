# Comparing `tmp/cazomevolve-0.1.5.tar.gz` & `tmp/cazomevolve-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.1.5.tar", last modified: Fri Jul  7 15:57:59 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.6.tar", last modified: Mon Jul 17 13:10:08 2023, max compression
```

## Comparing `cazomevolve-0.1.5.tar` & `cazomevolve-0.1.6.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1067 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/LICENSE
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    38355 2023-07-07 10:26:14.000000 cazomevolve-0.1.5/README.md
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2094 2023-07-07 15:57:06.000000 cazomevolve-0.1.5/cazomevolve/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/cazy/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     7022 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1548 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6148 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4889 2023-07-06 19:20:47.000000 cazomevolve-0.1.5/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.450540 cazomevolve-0.1.5/cazomevolve/cazome/explore/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1527 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17139 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6409 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_classes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    16877 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    19882 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/cooccurring_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     8670 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/identify_families.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3750 2023-05-18 10:26:39.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/ie_cazymes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11913 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    17620 2023-07-07 13:58:46.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/pca.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3181 2023-02-21 11:07:12.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/plot.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6041 2023-02-21 11:07:12.000000 cazomevolve-0.1.5/cazomevolve/cazome/explore/taxonomies.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.450540 cazomevolve-0.1.5/cazomevolve/genomes/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1540 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/genomes/__init__.py
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)    11300 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1492 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/bash/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1568 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/bash/build_cazy_db.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2401 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/bash/download_acc_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2078 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/build_cazy_db.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2462 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/cazomevolve_script.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3135 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/scripts/download_acc_genomes.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3063 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/get_fam_seqs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2064 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/run_fam_blast.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1969 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/run_fam_diamond.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.442540 cazomevolve-0.1.5/cazomevolve/scripts/tree/
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.454540 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2123 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/build_anim_tree.R
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1123 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/run_anim.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1863 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/align_scos.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1928 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1927 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/backtranslate.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6330 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/concatenate_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     5189 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/extract_cds.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1718 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/find_orthologues.sh
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2073 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/seq_diversity/
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1790 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/get_fam_seqs.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     1724 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/run_blastp.sh
--rwxrwxr-x   0 emmah     (1009) emmah     (1010)     2036 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/taxs/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1513 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/taxs/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    11322 2023-07-07 15:56:51.000000 cazomevolve-0.1.5/cazomevolve/taxs/add_taxs.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6982 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/taxs/ncbi.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.458540 cazomevolve-0.1.5/cazomevolve/utilities/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1517 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/__init__.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.462540 cazomevolve-0.1.5/cazomevolve/utilities/parsers/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     1529 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/__init__.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4914 2023-07-07 09:52:22.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/add_taxs_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2260 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/build_cazy_db_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3133 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/common_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6316 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     6780 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/download_genomes_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3477 2023-02-07 13:59:17.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/extract_prot_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4021 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_cazy_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3480 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_dbcan_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2899 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     3724 2023-07-06 15:09:54.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4343 2023-07-07 09:49:30.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/parse_cmd.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2257 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_blast_parser.py
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2372 2023-06-06 17:06:20.000000 cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_diamond_parser.py
-drwxrwxr-x   0 emmah     (1009) emmah     (1010)        0 2023-07-07 15:57:59.446540 cazomevolve-0.1.5/cazomevolve.egg-info/
--rw-rw-r--   0 emmah     (1009) emmah     (1010)    39120 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     2767 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)        1 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       76 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)      154 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       12 2023-07-07 15:57:59.000000 cazomevolve-0.1.5/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 emmah     (1009) emmah     (1010)       38 2023-07-07 15:57:59.466540 cazomevolve-0.1.5/setup.cfg
--rw-rw-r--   0 emmah     (1009) emmah     (1010)     4138 2023-07-07 15:57:02.000000 cazomevolve-0.1.5/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/
+-rw-rw-r--   0 em        (1000) em        (1000)     1067 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)    42471 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)    41706 2023-07-17 12:58:11.000000 cazomevolve-0.1.6/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.606311 cazomevolve-0.1.6/cazomevolve/
+-rw-rw-r--   0 em        (1000) em        (1000)     2094 2023-07-17 11:25:18.000000 cazomevolve-0.1.6/cazomevolve/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/
+-rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     7022 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6148 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4889 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.626311 cazomevolve-0.1.6/cazomevolve/cazome/explore/
+-rw-rw-r--   0 em        (1000) em        (1000)     1527 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)    17139 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6409 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 em        (1000) em        (1000)    16877 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)    19882 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)    20664 2023-07-17 11:37:31.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/explore_cazomes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     8670 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/identify_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11913 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 em        (1000) em        (1000)    17627 2023-07-17 11:18:55.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/pca.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3181 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/plot.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6041 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/taxonomies.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.630311 cazomevolve-0.1.6/cazomevolve/genomes/
+-rw-rw-r--   0 em        (1000) em        (1000)     1540 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11300 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.642311 cazomevolve-0.1.6/cazomevolve/scripts/
+-rw-rw-r--   0 em        (1000) em        (1000)     1492 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.646311 cazomevolve-0.1.6/cazomevolve/scripts/bash/
+-rw-rw-r--   0 em        (1000) em        (1000)     1568 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/bash/build_cazy_db.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     2401 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/bash/download_acc_genomes.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     2078 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2462 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3135 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3063 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2064 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1969 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.582310 cazomevolve-0.1.6/cazomevolve/scripts/tree/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.650311 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 em        (1000) em        (1000)     2123 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 em        (1000) em        (1000)     1123 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.662311 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 em        (1000) em        (1000)     1863 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     1928 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     1927 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     6330 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5189 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1718 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     2073 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.666312 cazomevolve-0.1.6/cazomevolve/seq_diversity/
+-rwxrwxr-x   0 em        (1000) em        (1000)     1790 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     1724 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     2036 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.670312 cazomevolve-0.1.6/cazomevolve/taxs/
+-rw-rw-r--   0 em        (1000) em        (1000)     1513 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11322 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6982 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.674312 cazomevolve-0.1.6/cazomevolve/utilities/
+-rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/cazomevolve/utilities/parsers/
+-rw-rw-r--   0 em        (1000) em        (1000)     1529 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4914 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/add_taxs_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2260 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/build_cazy_db_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3133 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/common_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6316 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6780 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/download_genomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6493 2023-07-17 11:40:52.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/explore_cazomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3477 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/extract_prot_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4021 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_cazy_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3480 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_dbcan_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2899 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3724 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4446 2023-07-17 11:38:28.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/parse_cmd.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2257 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_blast_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2372 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_diamond_parser.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)    42471 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     2828 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       76 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)      157 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       12 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)     4141 2023-07-17 11:39:25.000000 cazomevolve-0.1.6/setup.py
```

### Comparing `cazomevolve-0.1.5/LICENSE` & `cazomevolve-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/PKG-INFO` & `cazomevolve-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: cazomevolve
-Version: 0.1.5
-Summary: A bioinforamtic package for investigating the evolution of CAZomes
-Author: Emma E. M. Hobbs
-Author-email: eemh1@st-andrews.ac.uk
-License: MIT
-Keywords: bioinforamtics protein
-Platform: Posix
-Platform: MacOS X
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
@@ -622,14 +600,76 @@
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-l`, `--log` - path to write out log file
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 * `--retries` - number of times to retry connection to NCBI if connection fails
 
 # Explore the CAZome composition
 
+The `cazomevolve` subcommand provides a method for exploring CAZome compositions, calculating:
+* The number of CAZymes per genome, and mean and SD calculated per user defined group (e.g. genus)
+* Number of CAZy families per genome, and mean and SD calculated per user defined group
+* Total number of proteins in each genome, per genome, and mean and SD calculated per user defined group
+* Percentage of the proteome that encapsulates or consistutes the CAZomes per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy class, per genome, and mean and SD calculated per user defined group
+* Percentage of the CAZome represented by each CAZy class, per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy family in each genome
+* Analyse CAZy family frequencies using heirarchical clustering and generate a clustermap
+* Identify the core CAZome - CAZy families present in all genomes and per user defined group
+* Identify CAZy families that always co-occur in the genome together, although each group of co-occurring CAZy families may not be present in all genomes
+* Run Principal Component Analysis identify associations between user defined groups of genomes (e.g. genera), and CAZome compositions
+  * Plots scatters plots projecting genomes onto all pairs of PCs from PC1-4, genomes are colour coded by user defined group (e.g. genus)
+  * Plots a corresponding loadings plot for each PCA scatter plot
+
+## Command line arguments
+
+### Required
+
+1. Path to tab delimited FGP file, listing CAZy families, genomic accessions, and protein IDs
+2. Path CSV file listing taxonomic data, containing a column called 'Genome', listing genomic accessions, and one column per taxonomic rank retrieved from NCBI and/or GTDB.
+3. Directory to write out all outputs
+
+Each of the taxonomic ranks included in the CSV file of taxonomic data must also be specified, by adding each of the relevant flags to command:
+* `--kingdom`
+* `--phylum`
+* `--tax_class`
+* `--tax_order`
+* `--tax_family`
+* `--genus`
+* `--species`
+
+For example, if genus and species inforamtion was listed in the CSV of taxonomy data:
+```bash
+cazomevolve explore_cazomes\
+  data/cazomes/gfp_file.txt \
+  data/taxs/tax.csv \
+  results/ \
+  --genus \
+  --species
+```
+
+### Optional
+
+* `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
+* `-f`, `--force` - Force file over writting (default: False)
+* `-l`, `--log` log file name - Defines log file name and/or path (default: None)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+
+## Full customisation of CAZome exploration
+
+For full customisation of the exploration import the `cazomevolve.cazome.explore` into a jupyter notebook. 
+
+**Full customisation includes:**
+  * Adhock define groups of interest
+  * Exclude specific groups of interest from specific analyses
+  * Alter figure sizes
+  * Add additional and custom annotations (e.g. colour code by genomes by plant host)
+
+You can find an example notebook presented as a [website here](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pectobact_cazomes.html) and the [raw notebook here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/tree/master/notebooks).
+
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
 # loading and parsing data
 from cazomevolve.cazome.explore.parse_data import (
     load_fgp_data,
     load_tax_data,
```

### Comparing `cazomevolve-0.1.5/README.md` & `cazomevolve-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: cazomevolve
+Version: 0.1.6
+Summary: A bioinforamtic package for investigating the evolution of CAZomes
+Author: Emma E. M. Hobbs
+Author-email: eemh1@st-andrews.ac.uk
+License: MIT
+Keywords: bioinforamtics protein
+Platform: Posix
+Platform: MacOS X
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
@@ -600,14 +622,76 @@
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-l`, `--log` - path to write out log file
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 * `--retries` - number of times to retry connection to NCBI if connection fails
 
 # Explore the CAZome composition
 
+The `cazomevolve` subcommand provides a method for exploring CAZome compositions, calculating:
+* The number of CAZymes per genome, and mean and SD calculated per user defined group (e.g. genus)
+* Number of CAZy families per genome, and mean and SD calculated per user defined group
+* Total number of proteins in each genome, per genome, and mean and SD calculated per user defined group
+* Percentage of the proteome that encapsulates or consistutes the CAZomes per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy class, per genome, and mean and SD calculated per user defined group
+* Percentage of the CAZome represented by each CAZy class, per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy family in each genome
+* Analyse CAZy family frequencies using heirarchical clustering and generate a clustermap
+* Identify the core CAZome - CAZy families present in all genomes and per user defined group
+* Identify CAZy families that always co-occur in the genome together, although each group of co-occurring CAZy families may not be present in all genomes
+* Run Principal Component Analysis identify associations between user defined groups of genomes (e.g. genera), and CAZome compositions
+  * Plots scatters plots projecting genomes onto all pairs of PCs from PC1-4, genomes are colour coded by user defined group (e.g. genus)
+  * Plots a corresponding loadings plot for each PCA scatter plot
+
+## Command line arguments
+
+### Required
+
+1. Path to tab delimited FGP file, listing CAZy families, genomic accessions, and protein IDs
+2. Path CSV file listing taxonomic data, containing a column called 'Genome', listing genomic accessions, and one column per taxonomic rank retrieved from NCBI and/or GTDB.
+3. Directory to write out all outputs
+
+Each of the taxonomic ranks included in the CSV file of taxonomic data must also be specified, by adding each of the relevant flags to command:
+* `--kingdom`
+* `--phylum`
+* `--tax_class`
+* `--tax_order`
+* `--tax_family`
+* `--genus`
+* `--species`
+
+For example, if genus and species inforamtion was listed in the CSV of taxonomy data:
+```bash
+cazomevolve explore_cazomes\
+  data/cazomes/gfp_file.txt \
+  data/taxs/tax.csv \
+  results/ \
+  --genus \
+  --species
+```
+
+### Optional
+
+* `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
+* `-f`, `--force` - Force file over writting (default: False)
+* `-l`, `--log` log file name - Defines log file name and/or path (default: None)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+
+## Full customisation of CAZome exploration
+
+For full customisation of the exploration import the `cazomevolve.cazome.explore` into a jupyter notebook. 
+
+**Full customisation includes:**
+  * Adhock define groups of interest
+  * Exclude specific groups of interest from specific analyses
+  * Alter figure sizes
+  * Add additional and custom annotations (e.g. colour code by genomes by plant host)
+
+You can find an example notebook presented as a [website here](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pectobact_cazomes.html) and the [raw notebook here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/tree/master/notebooks).
+
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
 # loading and parsing data
 from cazomevolve.cazome.explore.parse_data import (
     load_fgp_data,
     load_tax_data,
```

### Comparing `cazomevolve-0.1.5/cazomevolve/__init__.py` & `cazomevolve-0.1.6/cazomevolve/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.1.5"
+__version__ = "0.1.6"
 
 __citation__ = "???"
 
 
 def closing_message(job, args):
     """Write closing messsage to terminal
```

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.6/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.6/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.6/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazome_sizes.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazome_sizes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_classes.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/cazy_families.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/cooccurring_families.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/cooccurring_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/identify_families.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/identify_families.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/parse_data.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/parse_data.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/pca.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/pca.py`

 * *Files 1% similar despite different names*

```diff
@@ -151,14 +151,15 @@
     pca,
     X_scaled,
     fam_df,
     first_pc,
     second_pc,
     group_by,
     file_path=None,
+    file_format='png',
     style=None,
     style_order=None,
     hue_order=None,
     font_scale=1.15,
     figsize=None, 
     xlim=None,
     ylim=None,
@@ -317,14 +318,15 @@
     sns.move_legend(g, "lower center", bbox_to_anchor=(.5, 1), ncol=3, title=None, frameon=False);
     
     if file_path is not None:
         plt.savefig(
             file_path,
             bbox_inches='tight',
             dpi=dpi,
+            format=file_format,
         )
     plt.show();
     
     return plt
 
 
 def plot_loadings(
@@ -335,16 +337,16 @@
     style=False,
     threshold=0.7,
     font_scale=1.15,
     font_size=12,
     dpi=300,
     fig_size=(16,16),
     file_path=None,
+    file_format='png',
     marker_size=100,
-    legend_cols=3,
     ax=None,
 ):
     """Build loadings plot
     
     :param pca: sklearn pca object
     :param fam_df: cazy family frequncy df
     :param first_pc: int, number of the first PC, e.g. PC1 == 1
@@ -354,15 +356,14 @@
         Only families with a value greater than the threshold
         will be annotated
     :param font_scale: scale font
     :param font_size: font size of family labels
     :param fig_size: tuple (width, height) of final plot
     :param file_path: str, path to write out a figure.
         If None, no figure is saved
-    :param legend_cols: int, number of columns to include in the legend
     :param ax: axis, used to define axis in multiple plot to place figure
     
     Return nothing"""
     sns.set(font_scale=font_scale)
 
     # calculate loading = variables x loadings, returns an array
     loadings = pca.components_.T * np.sqrt(pca.explained_variance_)
@@ -440,15 +441,15 @@
         ) if abs(xval) > threshold or abs(yval) > threshold
     ]
     adjustText.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='black'));
 
     sns.move_legend(g, "lower center", bbox_to_anchor=(.5, 1), ncol=3, title=None, frameon=False);
     
     if file_path is not None:
-        plt.savefig(file_path, dpi=dpi, bbox_inches='tight')
+        plt.savefig(file_path, dpi=dpi, bbox_inches='tight', format=file_format)
 
 
 def plot_ie_loadings(
     pca,
     fam_df,
     first_pc,
     second_pc,
```

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/plot.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/plot.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/cazome/explore/taxonomies.py` & `cazomevolve-0.1.6/cazomevolve/cazome/explore/taxonomies.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.6/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.6/cazomevolve/genomes/download_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/__init__.py` & `cazomevolve-0.1.6/cazomevolve/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/bash/build_cazy_db.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/bash/build_cazy_db.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/bash/download_acc_genomes.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/bash/download_acc_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/build_cazy_db.py` & `cazomevolve-0.1.6/cazomevolve/scripts/build_cazy_db.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/cazomevolve_script.py` & `cazomevolve-0.1.6/cazomevolve/scripts/cazomevolve_script.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/download_acc_genomes.py` & `cazomevolve-0.1.6/cazomevolve/scripts/download_acc_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/get_fam_seqs.py` & `cazomevolve-0.1.6/cazomevolve/scripts/get_fam_seqs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/run_fam_blast.py` & `cazomevolve-0.1.6/cazomevolve/scripts/run_fam_blast.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/run_fam_diamond.py` & `cazomevolve-0.1.6/cazomevolve/scripts/run_fam_diamond.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/build_anim_tree.R` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/build_anim_tree.R`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/ani/run_anim.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/run_anim.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/align_scos.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/align_scos.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/annotate_genomes.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/annotate_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/backtranslate.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/backtranslate.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/concatenate_cds.py` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/concatenate_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/extract_cds.py` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/extract_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/find_orthologues.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/find_orthologues.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh` & `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.6/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.6/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.6/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/taxs/__init__.py` & `cazomevolve-0.1.6/cazomevolve/taxs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/taxs/add_taxs.py` & `cazomevolve-0.1.6/cazomevolve/taxs/add_taxs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/taxs/ncbi.py` & `cazomevolve-0.1.6/cazomevolve/taxs/ncbi.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/__init__.py` & `cazomevolve-0.1.6/cazomevolve/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/__init__.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/add_taxs_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/add_taxs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/build_cazy_db_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/build_cazy_db_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/common_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/common_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/download_genomes_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/download_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/extract_prot_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/extract_prot_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_cazy_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_cazy_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_dbcan_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/get_fam_seqs_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_fam_seqs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/invoke_dbcan_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/invoke_dbcan_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/parse_cmd.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/parse_cmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     download_genomes_parser,
     build_cazy_db_parser,
     get_cazy_parser,
     invoke_dbcan_parser,
     get_dbcan_parser,
     common_parser,
     add_taxs_parser,
+    explore_cazomes_parser,
 )
 
 
 def build_parser(argv: Optional[List] = None) -> Namespace:
     """Parse command-line arguments for script.
 
     :param argv: Namesapce, command-line arguments
@@ -131,14 +132,17 @@
     # annotate cazome
     build_cazy_db_parser.build_parser(subparsers)
     get_cazy_parser.build_parser(subparsers)
     invoke_dbcan_parser.build_parser(subparsers)
     get_dbcan_parser.build_parser(subparsers)
     add_taxs_parser.build_parser(subparsers)
 
+    # explroe cazomes
+    explore_cazomes_parser.build_parser(subparsers)
+
     # Parse arguments
     # The list comprehension is to allow PosixPaths to be defined and passed in testing
     if argv is None:
         if len(sys.argv) == 1:
             argv = ["-h"]
         else:
             argv = sys.argv[1:]
```

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_blast_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_blast_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve/utilities/parsers/run_diamond_parser.py` & `cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_diamond_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.5/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.6/cazomevolve.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.5
+Version: 0.1.6
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
@@ -622,14 +622,76 @@
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-l`, `--log` - path to write out log file
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 * `--retries` - number of times to retry connection to NCBI if connection fails
 
 # Explore the CAZome composition
 
+The `cazomevolve` subcommand provides a method for exploring CAZome compositions, calculating:
+* The number of CAZymes per genome, and mean and SD calculated per user defined group (e.g. genus)
+* Number of CAZy families per genome, and mean and SD calculated per user defined group
+* Total number of proteins in each genome, per genome, and mean and SD calculated per user defined group
+* Percentage of the proteome that encapsulates or consistutes the CAZomes per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy class, per genome, and mean and SD calculated per user defined group
+* Percentage of the CAZome represented by each CAZy class, per genome, and mean and SD calculated per user defined group
+* Number of CAZymes per CAZy family in each genome
+* Analyse CAZy family frequencies using heirarchical clustering and generate a clustermap
+* Identify the core CAZome - CAZy families present in all genomes and per user defined group
+* Identify CAZy families that always co-occur in the genome together, although each group of co-occurring CAZy families may not be present in all genomes
+* Run Principal Component Analysis identify associations between user defined groups of genomes (e.g. genera), and CAZome compositions
+  * Plots scatters plots projecting genomes onto all pairs of PCs from PC1-4, genomes are colour coded by user defined group (e.g. genus)
+  * Plots a corresponding loadings plot for each PCA scatter plot
+
+## Command line arguments
+
+### Required
+
+1. Path to tab delimited FGP file, listing CAZy families, genomic accessions, and protein IDs
+2. Path CSV file listing taxonomic data, containing a column called 'Genome', listing genomic accessions, and one column per taxonomic rank retrieved from NCBI and/or GTDB.
+3. Directory to write out all outputs
+
+Each of the taxonomic ranks included in the CSV file of taxonomic data must also be specified, by adding each of the relevant flags to command:
+* `--kingdom`
+* `--phylum`
+* `--tax_class`
+* `--tax_order`
+* `--tax_family`
+* `--genus`
+* `--species`
+
+For example, if genus and species inforamtion was listed in the CSV of taxonomy data:
+```bash
+cazomevolve explore_cazomes\
+  data/cazomes/gfp_file.txt \
+  data/taxs/tax.csv \
+  results/ \
+  --genus \
+  --species
+```
+
+### Optional
+
+* `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
+* `-f`, `--force` - Force file over writting (default: False)
+* `-l`, `--log` log file name - Defines log file name and/or path (default: None)
+* `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
+* `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
+
+## Full customisation of CAZome exploration
+
+For full customisation of the exploration import the `cazomevolve.cazome.explore` into a jupyter notebook. 
+
+**Full customisation includes:**
+  * Adhock define groups of interest
+  * Exclude specific groups of interest from specific analyses
+  * Alter figure sizes
+  * Add additional and custom annotations (e.g. colour code by genomes by plant host)
+
+You can find an example notebook presented as a [website here](https://hobnobmancer.github.io/SI_Hobbs_et_al_2023_Pecto/notebooks/explore_pectobact_cazomes.html) and the [raw notebook here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto/tree/master/notebooks).
+
 The module `cazomevolve.cazome.explore` contains functions for exploring the CAZome annotated by `cazomevolve`. These are:
 
 ```python
 # loading and parsing data
 from cazomevolve.cazome.explore.parse_data import (
     load_fgp_data,
     load_tax_data,
```

### Comparing `cazomevolve-0.1.5/cazomevolve.egg-info/SOURCES.txt` & `cazomevolve-0.1.6/cazomevolve.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
 cazomevolve/cazome/dbcan/invoke_dbcan.py
 cazomevolve/cazome/explore/__init__.py
 cazomevolve/cazome/explore/cazome_sizes.py
 cazomevolve/cazome/explore/cazy_classes.py
 cazomevolve/cazome/explore/cazy_families.py
 cazomevolve/cazome/explore/cooccurring_families.py
+cazomevolve/cazome/explore/explore_cazomes.py
 cazomevolve/cazome/explore/identify_families.py
-cazomevolve/cazome/explore/ie_cazymes.py
 cazomevolve/cazome/explore/parse_data.py
 cazomevolve/cazome/explore/pca.py
 cazomevolve/cazome/explore/plot.py
 cazomevolve/cazome/explore/taxonomies.py
 cazomevolve/genomes/__init__.py
 cazomevolve/genomes/download_genomes.py
 cazomevolve/scripts/__init__.py
@@ -54,14 +54,15 @@
 cazomevolve/utilities/__init__.py
 cazomevolve/utilities/parsers/__init__.py
 cazomevolve/utilities/parsers/add_taxs_parser.py
 cazomevolve/utilities/parsers/build_cazy_db_parser.py
 cazomevolve/utilities/parsers/common_parser.py
 cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
 cazomevolve/utilities/parsers/download_genomes_parser.py
+cazomevolve/utilities/parsers/explore_cazomes_parser.py
 cazomevolve/utilities/parsers/extract_prot_parser.py
 cazomevolve/utilities/parsers/get_cazy_parser.py
 cazomevolve/utilities/parsers/get_dbcan_parser.py
 cazomevolve/utilities/parsers/get_fam_seqs_parser.py
 cazomevolve/utilities/parsers/invoke_dbcan_parser.py
 cazomevolve/utilities/parsers/parse_cmd.py
 cazomevolve/utilities/parsers/run_blast_parser.py
```

### Comparing `cazomevolve-0.1.5/setup.py` & `cazomevolve-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazomevolve",
-    version="0.1.5",
+    version="0.1.6",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A bioinforamtic package for investigating the evolution of CAZomes"
@@ -87,28 +87,28 @@
         'cazomevolve/scripts/tree/phylo/find_orthologues.sh',
         'cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh',
         'cazomevolve/scripts/tree/ani/run_anim.sh',
         'cazomevolve/scripts/tree/ani/build_anim_tree.R',
     ],
     install_requires=[
         "adjustText",
-        "cazy_webscraper",
         "biopython",
+        "cazy_webscraper",
+        "matplotlib",
+        "ncbi-genome-download",
+        "numpy",
         "pandas",
-        "tqdm",
-        "sklearn",
-        "scikit-learn",
         "saintbioutils",
-        "numpy",
+        "scikit-learn",
+        "scipy",
         "seaborn",
+        "sklearn",
         "sqlalchemy",
+        "tqdm",
         "upsetplot",
-        "scipy",
-        "jupyter",
-        "ncbi-genome-download",
     ],
     packages=setuptools.find_packages(),
     package_data={
     },
     include_package_data=True,
     classifiers=[
         "Development Status :: 3 - Alpha",
```

