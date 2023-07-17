# Comparing `tmp/MetaCerberus-1.0.tar.gz` & `tmp/MetaCerberus-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MetaCerberus-1.0.tar", last modified: Wed May 25 23:06:36 2022, max compression
+gzip compressed data, was "/home/jlfiguer/raw-lab/MetaCerberus/dist/.tmp-c27lq3r4/MetaCerberus-1.1.tar", last modified: Mon Jul 17 20:27:56 2023, max compression
```

## Comparing `MetaCerberus-1.0.tar` & `MetaCerberus-1.1.tar`

### file list

```diff
@@ -1,61 +1,83 @@
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.521424 MetaCerberus-1.0/
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1507 2022-05-25 21:57:42.000000 MetaCerberus-1.0/LICENSE.txt
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.349424 MetaCerberus-1.0/MetaCerberus.egg-info/
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    13644 2022-05-25 23:06:35.000000 MetaCerberus-1.0/MetaCerberus.egg-info/PKG-INFO
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1684 2022-05-25 23:06:36.000000 MetaCerberus-1.0/MetaCerberus.egg-info/SOURCES.txt
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)        1 2022-05-25 23:06:35.000000 MetaCerberus-1.0/MetaCerberus.egg-info/dependency_links.txt
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)      104 2022-05-25 23:06:35.000000 MetaCerberus-1.0/MetaCerberus.egg-info/requires.txt
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)       14 2022-05-25 23:06:35.000000 MetaCerberus-1.0/MetaCerberus.egg-info/top_level.txt
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    13644 2022-05-25 23:06:36.520424 MetaCerberus-1.0/PKG-INFO
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    10824 2022-05-25 21:57:42.000000 MetaCerberus-1.0/README.md
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.355424 MetaCerberus-1.0/bin/
--rwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)    28788 2022-05-25 01:53:24.000000 MetaCerberus-1.0/bin/metacerberus.py
--rwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)    11470 2022-05-24 21:51:37.000000 MetaCerberus-1.0/bin/pathview-metacerberus.R
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)      879 2022-04-09 22:09:25.000000 MetaCerberus-1.0/bin/ray-slurm-metacerberus.sh
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.417424 MetaCerberus-1.0/lib/
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     5129 2022-02-25 21:12:54.000000 MetaCerberus-1.0/lib/Chunker.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-02-25 21:12:54.000000 MetaCerberus-1.0/lib/__init__.py
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.427424 MetaCerberus-1.0/lib/dependency_files/
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     4127 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/dependency_files/PacBio_quality-control.fna
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    25304 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/dependency_files/adapters.fna
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    49167 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/dependency_files/lambda-phage.fna
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     5527 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/dependency_files/phix174_ill.ref.fna
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)      121 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/dependency_files/readme.md
-drwxr-xr-x   0 jlfiguer  (3042) jlfiguer  (3042)        0 2022-05-25 23:06:36.511424 MetaCerberus-1.0/lib/fraggenescanplus_dependences/
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1314 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_10
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1314 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_30
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1314 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_5
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1197 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/complete
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)   121095 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/gene
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1302 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_1
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1294 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_10
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1298 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_5
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     5175 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/noncoding
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     8670 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/pwm
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)       63 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/readme.md
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)   121095 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/rgene
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1294 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/sanger_10
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1298 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/sanger_5
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)  1584045 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/start
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)  1584045 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/start1
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)  1584045 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/stop
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)  1584045 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/fraggenescanplus_dependences/stop1
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1596 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus.config
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1086 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_decon.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     2690 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_formatFasta.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     2447 2022-05-25 02:02:52.000000 MetaCerberus-1.0/lib/metacerberus_genecall.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     3026 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/metacerberus_hmm.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)   163125 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/metacerberus_logo.jpg
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)      939 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_merge.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)      904 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_metastats.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     5861 2022-05-23 16:28:55.000000 MetaCerberus-1.0/lib/metacerberus_parser.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     2299 2022-05-23 16:08:00.000000 MetaCerberus-1.0/lib/metacerberus_prostats.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1497 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_qc.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)    16367 2022-05-11 21:55:31.000000 MetaCerberus-1.0/lib/metacerberus_report.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     1332 2022-05-05 20:46:31.000000 MetaCerberus-1.0/lib/metacerberus_setup.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     2206 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/metacerberus_trim.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     8408 2022-05-11 22:09:09.000000 MetaCerberus-1.0/lib/metacerberus_visual.py
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)  3512600 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/plotly-2.0.0.min.js
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     7661 2022-04-09 22:09:26.000000 MetaCerberus-1.0/lib/style.css
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)       38 2022-05-25 23:06:36.521424 MetaCerberus-1.0/setup.cfg
--rw-r--r--   0 jlfiguer  (3042) jlfiguer  (3042)     2306 2022-05-23 19:47:59.000000 MetaCerberus-1.0/setup.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.299601 MetaCerberus-1.1/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1507 2022-05-26 03:57:57.000000 MetaCerberus-1.1/LICENSE.txt
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.271596 MetaCerberus-1.1/MetaCerberus.egg-info/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    11594 2023-07-17 20:27:56.000000 MetaCerberus-1.1/MetaCerberus.egg-info/PKG-INFO
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2557 2023-07-17 20:27:56.000000 MetaCerberus-1.1/MetaCerberus.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)        1 2023-07-17 20:27:56.000000 MetaCerberus-1.1/MetaCerberus.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      111 2023-07-17 20:27:56.000000 MetaCerberus-1.1/MetaCerberus.egg-info/requires.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       14 2023-07-17 20:27:56.000000 MetaCerberus-1.1/MetaCerberus.egg-info/top_level.txt
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    11594 2023-07-17 20:27:56.299601 MetaCerberus-1.1/PKG-INFO
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    10791 2023-07-17 20:24:51.000000 MetaCerberus-1.1/README.md
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.271596 MetaCerberus-1.1/bin/
+-rwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)    32692 2023-07-17 20:24:51.000000 MetaCerberus-1.1/bin/metacerberus.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    11085 2023-07-17 20:24:51.000000 MetaCerberus-1.1/bin/pathview-metacerberus.R
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      879 2022-04-15 16:33:42.000000 MetaCerberus-1.1/bin/ray-slurm-metacerberus.sh
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.279597 MetaCerberus-1.1/lib/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5129 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/Chunker.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.279597 MetaCerberus-1.1/lib/FGS/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  2219806 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/FGS/FragGeneScanRS-Darwin.tar.gz
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)  3102361 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/FGS/FragGeneScanRS-Linux.tar.gz
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)        0 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/__init__.py
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.287599 MetaCerberus-1.1/lib/__pycache__/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      142 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1224 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_decon.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2295 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_formatFasta.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2211 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_genecall.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2046 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_hmm.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1070 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_merge.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      992 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_metastats.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4355 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_parser.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1855 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_prostats.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1665 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_qc.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    12803 2022-04-16 18:27:02.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_report.cpython-39.pyc
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      604 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_setup.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     2168 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_trim.cpython-39.pyc
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5568 2022-04-16 18:27:01.000000 MetaCerberus-1.1/lib/__pycache__/metacerberus_visual.cpython-39.pyc
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.287599 MetaCerberus-1.1/lib/cerberusDB/
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)   551484 2023-04-26 16:19:58.000000 MetaCerberus-1.1/lib/cerberusDB/COG-onto_rel1.tsv
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.287599 MetaCerberus-1.1/lib/dependency_files/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     4127 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/dependency_files/PacBio_quality-control.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    25304 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/dependency_files/adapters.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)    49167 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/dependency_files/lambda-phage.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5527 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/dependency_files/phix174_ill.ref.fna
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)      121 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/dependency_files/readme.md
+drwxrwxr-x   0 jlfiguer  (1004) jlfiguer  (1004)        0 2023-07-17 20:27:56.299601 MetaCerberus-1.1/lib/fraggenescanplus_dependences/
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:41.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_30
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1314 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1197 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/complete
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/gene
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1302 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     5175 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/noncoding
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     8670 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/pwm
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)       63 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/readme.md
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   121095 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/rgene
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1294 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/sanger_10
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1298 2022-04-15 16:46:42.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/sanger_5
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:43.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/start
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/start1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:44.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/stop
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  1584045 2022-04-15 16:46:45.000000 MetaCerberus-1.1/lib/fraggenescanplus_dependences/stop1
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     1596 2022-04-15 16:46:45.000000 MetaCerberus-1.1/lib/metacerberus.config
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1231 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_decon.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     3052 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_formatFasta.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2425 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_genecall.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4478 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_hmm.py
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)   163125 2022-04-16 18:29:53.000000 MetaCerberus-1.1/lib/metacerberus_logo.jpg
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1102 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_merge.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)      827 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_metastats.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7924 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_parser.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4867 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_prostats.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     1502 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_qc.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)    16640 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_report.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     4886 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_setup.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2580 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_trim.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     7833 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacerberus_visual.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     5986 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacereberus_parser_wPl.py
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     9394 2023-07-17 20:24:51.000000 MetaCerberus-1.1/lib/metacereberus_visual_wPL.py
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)  3512600 2022-04-15 16:46:47.000000 MetaCerberus-1.1/lib/plotly-2.0.0.min.js
+-rw-r--r--   0 jlfiguer  (1004) jlfiguer  (1004)     7661 2022-04-15 16:46:48.000000 MetaCerberus-1.1/lib/style.css
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)       38 2023-07-17 20:27:56.299601 MetaCerberus-1.1/setup.cfg
+-rw-rw-r--   0 jlfiguer  (1004) jlfiguer  (1004)     2331 2023-07-17 20:24:56.000000 MetaCerberus-1.1/setup.py
```

### Comparing `MetaCerberus-1.0/LICENSE.txt` & `MetaCerberus-1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/MetaCerberus.egg-info/PKG-INFO` & `MetaCerberus-1.1/MetaCerberus.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,276 @@
 Metadata-Version: 2.1
 Name: MetaCerberus
-Version: 1.0
+Version: 1.1
 Summary: Versatile Functional Ontology Assignments for Metagenomes via Hidden Markov Model (HMM) searching with environmental focus of shotgun meta'omics data
 Home-page: https://github.com/raw-lab/metacerberus
 Author: Jose L. Figueroa III, Richard A. White III
 Author-email: jlfiguer@uncc.edu
 License: BSD License
-Description: # Welcome to MetaCerberus
-        
-        ## About 
-        MetaCerberus transforms raw shotgun metaomics sequencing (i.e. metagenomics/metatranscriptomic) data into knowledge. It is a start to finish python code for versatile analysis of the Functional Ontology Assignments for Metagenomes (FOAM) database and KEGG via Hidden Markov Models (HMM) for whole ecosystem metabolomic analysis.
-        
-        ![GitHub Logo](metacerberus_logo.jpg)
-        
-        ## Installing MetaCerberus
-        
-        ### Option 1) Anaconda
-        
-        - Anaconda install from bioconda with all dependencies:
-        
-        ```
-        conda create -n metacerberus -c conda-forge -c bioconda metacerberus -y
-        conda activate metacerberus
-        metacerberus.py --setup
-        ```
-        
-        ### Option 2) Manual Install
-        
-        1. Clone github Repo
-        
-        ```
-        git clone https://github.com/raw-lab/metacerberus.git
-        ```
-        
-        2. Run Setup File
-        
-        ```
-        cd metacerberus
-        bash install_metacerberus.sh
-        conda activate metacerberus
-        metacerberus.py --setup
-        ```
-        
-        This creates an anaconda environment called "metacerberus" with all dependencies installed.
-        
-        ## Input formats
-        
-        - From any NextGen sequencing technology (from Illumina, PacBio, Oxford Nanopore)
-        - type 1 raw reads (.fastq format)
-        - type 2 nucleotide fasta (.fasta, .fa, .fna, .ffn format), assembled raw reads into contigs
-        - type 3 protein fasta (.faa format), assembled contigs which genes are converted to amino acid sequence
-        
-        ## Output Files
-        
-        - If an output directory is given, that folder will be created where all files are stored.
-        - If no output directory is specified, the 'pipeline' subfolder will be created in the current directory.
-        - Gage/Pathview R analysis provided as separate scripts within R. 
-        
-        ## Visualization of Outputs
-        
-        - We use Plotly to visualize the data
-        - Once the program is executed the html reports with the visuals will be saved to the last step of the pipeline.
-        - The HTML files require plotly.js to be present. One has been provided in the package and is saved to the report folder.
-        
-        ## Quick start examples
-        
-        ### Illumina data 
-        
-        #### Bacterial, Archaea and Bacteriophage 
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder] --illumina --meta --dir_out [out_folder] 
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder] --illumina --meta --dir_out [out_folder] 
-        ```
-        
-        ### Nanopore data 
-        
-        #### Bacterial, Archaea and Bacteriophage
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder]  --nanopore --meta --dir_out [out_folder]
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder] --nanopore --meta --dir_out [out_folder] 
-        ```
-        
-        ### PacBio data
-        
-        #### Microbial, Archaea and Bacteriophage
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder]  --pacbio --meta --dir_out [out_folder]
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder]  --pacbio --meta --dir_out [out_folder]
-        ```
-        
-        ### SUPER (both methods)
-        ```
-        conda activate metacerberus
-        metacerberus.py --super [input_folder]  --pacbio/--nanopore/--illumina --meta --dir_out [out_folder]
-        ```
-        
-        - Note: Fraggenescan will work for prokaryotes and viruses/bacteriophage but prodigal will not work for eukaryotes. 
-        
-        
-        ## Prerequisites and dependencies
-        
-        - python >= 3.7
-        - MetaCerberus currently runs best with Python version 3.7, 3.8, 3.9 due to compatibility with dependencies.
-        - MetaCerberus currently doesn't support Python 3.10 due to the "Ray" dependency. 
-        - Python 3.10 is not currently supported.
-        
-        ### Available from Bioconda
-        
-        - fastqc - <https://github.com/s-andrews/FastQC>
-        - fastp - <https://github.com/OpenGene/fastp>
-        - porechop - <https://github.com/rrwick/Porechop>
-        - bbmap - <https://sourceforge.net/projects/bbmap/> or <https://github.com/BioInfoTools/BBMap>
-        - prodigal - <https://github.com/hyattpd/Prodigal>
-        - hmmer - <https://github.com/EddyRivasLab/hmmer>
-        
-        - NOTE: The KEGG database contains KOs related to Human disease. It is possible that these will show up in the results, even when analyzing microbes.
-        
-        ## MetaCerberus Options
-        
-        - If the metacerberus environment is not used, make sure the dependencies are in PATH or specified in the config file.
-        - Run metacerberus.py with the options required for your project.
-        
-        ```
-        usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--meta META] [--super SUPER] [--protein PROTEIN]
-                               [--illumina | --nanopore | --pacbio] [--setup] [--uninstall] [--dir_out DIR_OUT] [--scaffolds] [--minscore MINSCORE] [--cpus CPUS]
-                               [--chunker CHUNKER] [--replace] [--keep] [--hmm HMM] [--class CLASS] [--slurm_nodes SLURM_NODES] [--tmpdir TMPDIR] [--version] [-h]
-                               [--adapters ADAPTERS] [--control_seq CONTROL_SEQ]
-        
-        optional arguments:
-          --illumina            Specifies that the given FASTQ files are from Illumina
-          --nanopore            Specifies that the given FASTQ files are from Nanopore
-          --pacbio              Specifies that the given FASTQ files are from PacBio
-        
-        Required arguments
-        At least one sequence is required.
-        <accepted formats {.fastq .fasta .faa .fna .ffn .rollup}>
-        Example:
-        > metaerberus.py --prodigal file1.fasta
-        > metacerberus.py --config file.config
-        *Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.:
-          -c CONFIG, --config CONFIG
-                                Path to config file, command line takes priority
-          --prodigal PRODIGAL   Prokaryote nucleotide sequence (includes microbes, bacteriophage)
-          --fraggenescan FRAGGENESCAN
-                                Eukaryote nucleotide sequence (includes other viruses, works all around for everything)
-          --meta META           Metagenomic nucleotide sequences (Uses prodigal)
-          --super SUPER         Run sequence in both --prodigal and --fraggenescan modes
-          --protein PROTEIN, --amino PROTEIN
-                                Protein Amino Acid sequence
-        
-        optional arguments:
-          --setup               Set this flag to ensure dependencies are setup [False]
-          --uninstall           Set this flag to remove downloaded databases and FragGeneScan+ [False]
-          --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./meta_cerberus]
-          --scaffolds           Sequences are treated as scaffolds [False]
-          --minscore MINSCORE   Filter for parsing HMMER results [25]
-          --cpus CPUS           Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]
-          --chunker CHUNKER     Split files into smaller chunks, in Megabytes [Disabled by default]
-          --replace             Flag to replace existing files. [False]
-          --keep                Flag to keep temporary files. [False]
-          --hmm HMM             Specify a custom HMM file for HMMER. Default uses downloaded FOAM HMM Database
-          --class CLASS         path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R
-          --slurm_nodes SLURM_NODES
-                                list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST
-          --tmpdir TMPDIR       temp directory for RAY [system tmp dir]
-          --version, -v         show the version number and exit
-          -h, --help            show this help message and exit
-        
-          --adapters ADAPTERS   FASTA File containing adapter sequences for trimming
-          --control_seq CONTROL_SEQ
-                                FASTA File containing control sequences for decontamination
-        
-        Args that start with '--' (eg. --prodigal) can also be set in a config file (specified via -c). Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
-        details, see syntax at https://goo.gl/R74nmi). If an arg is specified in more than one place, then commandline values override config file values which override defaults.
-        ```
-        
-        ### GAGE / PathView
-        
-        After processing the HMM files MetaCerberus calculates a KO (KEGG Orthology) counts table from KEGG/FOAM for processing through GAGE and PathView.
-        GAGE is recommended for pathway enrichment followed by PathView for visualize the metabolic pathways. A "class" file is required through the --class option to run this analysis. The output is saved under the step_10-visualizeData/combined/pathview folder. Also, at least 4 samples need to be used for this type of analysis.  
-          
-        GAGE and PathView also require internet access to be able to download information from a database. MetaCerberus will save a bash script 'run_pathview.sh' in the step_10-visualizeData/combined/pathview directory along with the KO Counts tsv files and the class file for running manualy in case MetaCerberus was run on a cluster without access to the internet.
-        
-        ### Multiprocessing / Multi-Computing with RAY
-        
-        MetaCerberus uses Ray for distributed processing. This is compatible with both multiprocessing on a single node (computer) or multiple nodes in a cluster.  
-        MetaCerberus has been tested on a cluster using Slurm <https://github.com/SchedMD/slurm>.  
-          
-        A script has been included to facilitate running MetaCerberus on Slurm. To use MetaCerberus on a Slurm cluster, setup your slurm script and run it using sbatch.  
-        
-        ```bash
-        sbatch example_script.sh
-        ```
-        
-        example script:  
-        
-        ```bash
-        #!/usr/bin/env bash
-        
-        #SBATCH --job-name=test-job
-        #SBATCH --nodes=3
-        #SBATCH --tasks-per-node=1
-        #SBATCH --cpus-per-task=16
-        #SBATCH --mem=128MB
-        #SBATCH -e slurm-%j.err
-        #SBATCH -o slurm-%j.out
-        #SBATCH --mail-type=END,FAIL,REQUEUE
-        
-        echo "====================================================="
-        echo "Start Time  : $(date)"
-        echo "Submit Dir  : $SLURM_SUBMIT_DIR"
-        echo "Job ID/Name : $SLURM_JOBID / $SLURM_JOB_NAME"
-        echo "Node List   : $SLURM_JOB_NODELIST"
-        echo "Num Tasks   : $SLURM_NTASKS total [$SLURM_NNODES nodes @ $SLURM_CPUS_ON_NODE CPUs/node]"
-        echo "======================================================"
-        echo ""
-        
-        # Load any modules or resources here
-        conda activate metacerberus
-        # source the slurm script to initialize the Ray worker nodes
-        source ray-slurm-metacerberus.sh
-        # run MetaCerberus
-        metacerberus.py --prodigal [input_folder] --illumina --dir_out [out_folder]
-        
-        echo ""
-        echo "======================================================"
-        echo "End Time   : $(date)"
-        echo "======================================================"
-        echo ""
-        ```
-        
-        ## Citing MetaCerberus
-        
-        MetaCerberus: python code for versatile Functional Ontology Assignments for Metagenomes (FOAM) database searching via Hidden Markov Models (HMM) with environmental focus of shotgun metaomics data. Preprints.
-        
-        ## CONTACT
-        
-        The informatics point-of-contact for this project is [Dr. Richard Allen White III](https://github.com/raw-lab).  
-        If you have any questions or feedback, please feel free to get in touch by email.  
-        Dr. Richard Allen White III - rwhit101@uncc.edu or raw937@gmail.com.  
-        Jose L. Figueroa III - jlfiguer@uncc.edu  
-        Or [open an issue](https://github.com/raw-lab/metacerberus/issues).  
-        
 Platform: Unix
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
-Requires-Python: <3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Welcome to MetaCerberus
+
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/metacerberus/README.html)
+
+## About
+
+MetaCerberus transforms raw shotgun metaomics sequencing (i.e. metagenomics/metatranscriptomic) data into knowledge. It is a start to finish python code for versatile analysis of the Functional Ontology Assignments for Metagenomes (FOAM) database and KEGG via Hidden Markov Models (HMM) for whole ecosystem metabolomic analysis.
+
+![GitHub Logo](https://raw.githubusercontent.com/raw-lab/MetaCerberus/main/metacerberus_logo.jpg)
+
+## Installing MetaCerberus
+
+### Option 1) Anaconda
+
+- Anaconda install from bioconda with all dependencies:
+
+```bash
+conda create -n metacerberus -c conda-forge -c bioconda metacerberus -y
+conda activate metacerberus
+metacerberus.py --setup
+```
+
+### Option 2) Manual Install
+
+1. Clone github Repo
+
+```bash
+git clone https://github.com/raw-lab/metacerberus.git
+```
+
+2. Run Setup File
+
+```bash
+cd metacerberus
+bash install_metacerberus.sh
+conda activate metacerberus
+metacerberus.py --setup
+```
+
+This creates an anaconda environment called "metacerberus" with all dependencies installed.
+
+## Input formats
+
+- From any NextGen sequencing technology (from Illumina, PacBio, Oxford Nanopore)
+- type 1 raw reads (.fastq format)
+- type 2 nucleotide fasta (.fasta, .fa, .fna, .ffn format), assembled raw reads into contigs
+- type 3 protein fasta (.faa format), assembled contigs which genes are converted to amino acid sequence
+
+## Output Files
+
+- If an output directory is given, that folder will be created where all files are stored.
+- If no output directory is specified, the 'pipeline' subfolder will be created in the current directory.
+- Gage/Pathview R analysis provided as separate scripts within R. 
+
+## Visualization of Outputs
+
+- We use Plotly to visualize the data
+- Once the program is executed the html reports with the visuals will be saved to the last step of the pipeline.
+- The HTML files require plotly.js to be present. One has been provided in the package and is saved to the report folder.
+
+## Quick start examples
+
+### Illumina data
+
+#### Bacterial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder] --illumina --meta --dir_out [out_folder] 
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder] --illumina --meta --dir_out [out_folder] 
+```
+
+### Nanopore data
+
+#### Bacterial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder]  --nanopore --meta --dir_out [out_folder]
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder] --nanopore --meta --dir_out [out_folder] 
+```
+
+### PacBio data
+
+#### Microbial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder]  --pacbio --meta --dir_out [out_folder]
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder]  --pacbio --meta --dir_out [out_folder]
+```
+
+### SUPER (both methods)
+
+```bash
+conda activate metacerberus
+metacerberus.py --super [input_folder]  --pacbio/--nanopore/--illumina --meta --dir_out [out_folder]
+```
+
+- Note: Fraggenescan will work for prokaryotes and viruses/bacteriophage but prodigal will not work for eukaryotes. 
+
+## Prerequisites and dependencies
+
+- python >= 3.8
+
+### Available from Bioconda
+
+- fastqc - <https://github.com/s-andrews/FastQC>
+- fastp - <https://github.com/OpenGene/fastp>
+- porechop - <https://github.com/rrwick/Porechop>
+- bbmap - <https://sourceforge.net/projects/bbmap/> or <https://github.com/BioInfoTools/BBMap>
+- prodigal - <https://github.com/hyattpd/Prodigal>
+- hmmer - <https://github.com/EddyRivasLab/hmmer>
+
+- NOTE: The KEGG database contains KOs related to Human disease. It is possible that these will show up in the results, even when analyzing microbes.
+
+## MetaCerberus Options
+
+- If the metacerberus environment is not used, make sure the dependencies are in PATH or specified in the config file.
+- Run metacerberus.py with the options required for your project.
+
+```
+usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--super SUPER] [--protein PROTEIN] [--illumina | --nanopore | --pacbio] [--setup]
+                       [--uninstall] [--dir_out DIR_OUT] [--meta] [--scaffolds] [--minscore MINSCORE] [--evalue EVALUE] [--cpus CPUS] [--chunker CHUNKER] [--replace]
+                       [--keep] [--hmm HMM] [--class CLASS] [--tmpdir TMPDIR] [--version] [-h] [--adapters ADAPTERS] [--qc_seq QC_SEQ]
+
+options:
+  --illumina            Specifies that the given FASTQ files are from Illumina
+  --nanopore            Specifies that the given FASTQ files are from Nanopore
+  --pacbio              Specifies that the given FASTQ files are from PacBio
+
+Required arguments
+At least one sequence is required.
+<accepted formats {.fastq .fasta .faa .fna .ffn .rollup}>
+Example:
+> metaerberus.py --prodigal file1.fasta
+> metacerberus.py --config file.config
+*Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.:
+  -c CONFIG, --config CONFIG
+                        Path to config file, command line takes priority
+  --prodigal PRODIGAL   Prokaryote nucleotide sequence (includes microbes, bacteriophage)
+  --fraggenescan FRAGGENESCAN
+                        Eukaryote nucleotide sequence (includes other viruses, works all around for everything)
+  --super SUPER         Run sequence in both --prodigal and --fraggenescan modes
+  --protein PROTEIN, --amino PROTEIN
+                        Protein Amino Acid sequence
+
+optional arguments:
+  --setup               Set this flag to ensure dependencies are setup [False]
+  --uninstall           Set this flag to remove downloaded databases and FragGeneScan+ [False]
+  --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./results-metacerberus]
+  --meta                Metagenomic nucleotide sequences (for prodigal) [False]
+  --scaffolds           Sequences are treated as scaffolds [False]
+  --minscore MINSCORE   Score cutoff for parsing HMMER results [25]
+  --evalue EVALUE       E-value cutoff for parsing HMMER results [1e-09]
+  --cpus CPUS           Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]
+  --chunker CHUNKER     Split files into smaller chunks, in Megabytes [Disabled by default]
+  --replace             Flag to replace existing files. [False]
+  --keep                Flag to keep temporary files. [False]
+  --hmm HMM             Specify the database for HMMER. (KOFam_all, KOFam_eukariote, KOFam_prokaryote, COG, CAZy, PHROG, COG) [KOFam_all]
+  --class CLASS         path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R
+  --tmpdir TMPDIR       temp directory for RAY [system tmp dir]
+  --version, -v         show the version number and exit
+  -h, --help            show this help message and exit
+
+  --adapters ADAPTERS   FASTA File containing adapter sequences for trimming
+  --qc_seq QC_SEQ       FASTA File containing control sequences for decontamination
+
+Args that start with '--' (eg. --prodigal) can also be set in a config file (specified via -c). Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
+details, see syntax at https://goo.gl/R74nmi). If an arg is specified in more than one place, then commandline values override config file values which override defaults.
+```
+
+### GAGE / PathView
+
+After processing the HMM files MetaCerberus calculates a KO (KEGG Orthology) counts table from KEGG/FOAM for processing through GAGE and PathView.
+GAGE is recommended for pathway enrichment followed by PathView for visualize the metabolic pathways. A "class" file is required through the --class option to run this analysis. The output is saved under the step_10-visualizeData/combined/pathview folder. Also, at least 4 samples need to be used for this type of analysis.  
+  
+GAGE and PathView also require internet access to be able to download information from a database. MetaCerberus will save a bash script 'run_pathview.sh' in the step_10-visualizeData/combined/pathview directory along with the KO Counts tsv files and the class file for running manualy in case MetaCerberus was run on a cluster without access to the internet.
+
+### Multiprocessing / Multi-Computing with RAY
+
+MetaCerberus uses Ray for distributed processing. This is compatible with both multiprocessing on a single node (computer) or multiple nodes in a cluster.  
+MetaCerberus has been tested on a cluster using Slurm <https://github.com/SchedMD/slurm>.  
+  
+A script has been included to facilitate running MetaCerberus on Slurm. To use MetaCerberus on a Slurm cluster, setup your slurm script and run it using sbatch.  
+
+```bash
+sbatch example_script.sh
+```
+
+example script:  
+
+```bash
+#!/usr/bin/env bash
+
+#SBATCH --job-name=test-job
+#SBATCH --nodes=3
+#SBATCH --tasks-per-node=1
+#SBATCH --cpus-per-task=16
+#SBATCH --mem=128MB
+#SBATCH -e slurm-%j.err
+#SBATCH -o slurm-%j.out
+#SBATCH --mail-type=END,FAIL,REQUEUE
+
+echo "====================================================="
+echo "Start Time  : $(date)"
+echo "Submit Dir  : $SLURM_SUBMIT_DIR"
+echo "Job ID/Name : $SLURM_JOBID / $SLURM_JOB_NAME"
+echo "Node List   : $SLURM_JOB_NODELIST"
+echo "Num Tasks   : $SLURM_NTASKS total [$SLURM_NNODES nodes @ $SLURM_CPUS_ON_NODE CPUs/node]"
+echo "======================================================"
+echo ""
+
+# Load any modules or resources here
+conda activate metacerberus
+# source the slurm script to initialize the Ray worker nodes
+source ray-slurm-metacerberus.sh
+# run MetaCerberus
+metacerberus.py --prodigal [input_folder] --illumina --dir_out [out_folder]
+
+echo ""
+echo "======================================================"
+echo "End Time   : $(date)"
+echo "======================================================"
+echo ""
+```
+
+## Citing MetaCerberus
+
+MetaCerberus: python code for versatile Functional Ontology Assignments for Metagenomes (FOAM) database searching via Hidden Markov Models (HMM) with environmental focus of shotgun metaomics data. Preprints.
+
+## CONTACT
+
+The informatics point-of-contact for this project is [Dr. Richard Allen White III](https://github.com/raw-lab).  
+If you have any questions or feedback, please feel free to get in touch by email.  
+Dr. Richard Allen White III - rwhit101@uncc.edu or raw937@gmail.com.  
+Jose L. Figueroa III - jlfiguer@uncc.edu  
+Or [open an issue](https://github.com/raw-lab/metacerberus/issues).
```

### Comparing `MetaCerberus-1.0/PKG-INFO` & `MetaCerberus-1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,272 +1,276 @@
 Metadata-Version: 2.1
 Name: MetaCerberus
-Version: 1.0
+Version: 1.1
 Summary: Versatile Functional Ontology Assignments for Metagenomes via Hidden Markov Model (HMM) searching with environmental focus of shotgun meta'omics data
 Home-page: https://github.com/raw-lab/metacerberus
 Author: Jose L. Figueroa III, Richard A. White III
 Author-email: jlfiguer@uncc.edu
 License: BSD License
-Description: # Welcome to MetaCerberus
-        
-        ## About 
-        MetaCerberus transforms raw shotgun metaomics sequencing (i.e. metagenomics/metatranscriptomic) data into knowledge. It is a start to finish python code for versatile analysis of the Functional Ontology Assignments for Metagenomes (FOAM) database and KEGG via Hidden Markov Models (HMM) for whole ecosystem metabolomic analysis.
-        
-        ![GitHub Logo](metacerberus_logo.jpg)
-        
-        ## Installing MetaCerberus
-        
-        ### Option 1) Anaconda
-        
-        - Anaconda install from bioconda with all dependencies:
-        
-        ```
-        conda create -n metacerberus -c conda-forge -c bioconda metacerberus -y
-        conda activate metacerberus
-        metacerberus.py --setup
-        ```
-        
-        ### Option 2) Manual Install
-        
-        1. Clone github Repo
-        
-        ```
-        git clone https://github.com/raw-lab/metacerberus.git
-        ```
-        
-        2. Run Setup File
-        
-        ```
-        cd metacerberus
-        bash install_metacerberus.sh
-        conda activate metacerberus
-        metacerberus.py --setup
-        ```
-        
-        This creates an anaconda environment called "metacerberus" with all dependencies installed.
-        
-        ## Input formats
-        
-        - From any NextGen sequencing technology (from Illumina, PacBio, Oxford Nanopore)
-        - type 1 raw reads (.fastq format)
-        - type 2 nucleotide fasta (.fasta, .fa, .fna, .ffn format), assembled raw reads into contigs
-        - type 3 protein fasta (.faa format), assembled contigs which genes are converted to amino acid sequence
-        
-        ## Output Files
-        
-        - If an output directory is given, that folder will be created where all files are stored.
-        - If no output directory is specified, the 'pipeline' subfolder will be created in the current directory.
-        - Gage/Pathview R analysis provided as separate scripts within R. 
-        
-        ## Visualization of Outputs
-        
-        - We use Plotly to visualize the data
-        - Once the program is executed the html reports with the visuals will be saved to the last step of the pipeline.
-        - The HTML files require plotly.js to be present. One has been provided in the package and is saved to the report folder.
-        
-        ## Quick start examples
-        
-        ### Illumina data 
-        
-        #### Bacterial, Archaea and Bacteriophage 
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder] --illumina --meta --dir_out [out_folder] 
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder] --illumina --meta --dir_out [out_folder] 
-        ```
-        
-        ### Nanopore data 
-        
-        #### Bacterial, Archaea and Bacteriophage
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder]  --nanopore --meta --dir_out [out_folder]
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder] --nanopore --meta --dir_out [out_folder] 
-        ```
-        
-        ### PacBio data
-        
-        #### Microbial, Archaea and Bacteriophage
-        ```
-        conda activate metacerberus
-        metacerberus.py --prodigal [input_folder]  --pacbio --meta --dir_out [out_folder]
-        ```
-        
-        #### Eukaryotes and Viruses
-        ```
-        conda activate metacerberus
-        metacerberus.py --fraggenescan [input_folder]  --pacbio --meta --dir_out [out_folder]
-        ```
-        
-        ### SUPER (both methods)
-        ```
-        conda activate metacerberus
-        metacerberus.py --super [input_folder]  --pacbio/--nanopore/--illumina --meta --dir_out [out_folder]
-        ```
-        
-        - Note: Fraggenescan will work for prokaryotes and viruses/bacteriophage but prodigal will not work for eukaryotes. 
-        
-        
-        ## Prerequisites and dependencies
-        
-        - python >= 3.7
-        - MetaCerberus currently runs best with Python version 3.7, 3.8, 3.9 due to compatibility with dependencies.
-        - MetaCerberus currently doesn't support Python 3.10 due to the "Ray" dependency. 
-        - Python 3.10 is not currently supported.
-        
-        ### Available from Bioconda
-        
-        - fastqc - <https://github.com/s-andrews/FastQC>
-        - fastp - <https://github.com/OpenGene/fastp>
-        - porechop - <https://github.com/rrwick/Porechop>
-        - bbmap - <https://sourceforge.net/projects/bbmap/> or <https://github.com/BioInfoTools/BBMap>
-        - prodigal - <https://github.com/hyattpd/Prodigal>
-        - hmmer - <https://github.com/EddyRivasLab/hmmer>
-        
-        - NOTE: The KEGG database contains KOs related to Human disease. It is possible that these will show up in the results, even when analyzing microbes.
-        
-        ## MetaCerberus Options
-        
-        - If the metacerberus environment is not used, make sure the dependencies are in PATH or specified in the config file.
-        - Run metacerberus.py with the options required for your project.
-        
-        ```
-        usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--meta META] [--super SUPER] [--protein PROTEIN]
-                               [--illumina | --nanopore | --pacbio] [--setup] [--uninstall] [--dir_out DIR_OUT] [--scaffolds] [--minscore MINSCORE] [--cpus CPUS]
-                               [--chunker CHUNKER] [--replace] [--keep] [--hmm HMM] [--class CLASS] [--slurm_nodes SLURM_NODES] [--tmpdir TMPDIR] [--version] [-h]
-                               [--adapters ADAPTERS] [--control_seq CONTROL_SEQ]
-        
-        optional arguments:
-          --illumina            Specifies that the given FASTQ files are from Illumina
-          --nanopore            Specifies that the given FASTQ files are from Nanopore
-          --pacbio              Specifies that the given FASTQ files are from PacBio
-        
-        Required arguments
-        At least one sequence is required.
-        <accepted formats {.fastq .fasta .faa .fna .ffn .rollup}>
-        Example:
-        > metaerberus.py --prodigal file1.fasta
-        > metacerberus.py --config file.config
-        *Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.:
-          -c CONFIG, --config CONFIG
-                                Path to config file, command line takes priority
-          --prodigal PRODIGAL   Prokaryote nucleotide sequence (includes microbes, bacteriophage)
-          --fraggenescan FRAGGENESCAN
-                                Eukaryote nucleotide sequence (includes other viruses, works all around for everything)
-          --meta META           Metagenomic nucleotide sequences (Uses prodigal)
-          --super SUPER         Run sequence in both --prodigal and --fraggenescan modes
-          --protein PROTEIN, --amino PROTEIN
-                                Protein Amino Acid sequence
-        
-        optional arguments:
-          --setup               Set this flag to ensure dependencies are setup [False]
-          --uninstall           Set this flag to remove downloaded databases and FragGeneScan+ [False]
-          --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./meta_cerberus]
-          --scaffolds           Sequences are treated as scaffolds [False]
-          --minscore MINSCORE   Filter for parsing HMMER results [25]
-          --cpus CPUS           Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]
-          --chunker CHUNKER     Split files into smaller chunks, in Megabytes [Disabled by default]
-          --replace             Flag to replace existing files. [False]
-          --keep                Flag to keep temporary files. [False]
-          --hmm HMM             Specify a custom HMM file for HMMER. Default uses downloaded FOAM HMM Database
-          --class CLASS         path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R
-          --slurm_nodes SLURM_NODES
-                                list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST
-          --tmpdir TMPDIR       temp directory for RAY [system tmp dir]
-          --version, -v         show the version number and exit
-          -h, --help            show this help message and exit
-        
-          --adapters ADAPTERS   FASTA File containing adapter sequences for trimming
-          --control_seq CONTROL_SEQ
-                                FASTA File containing control sequences for decontamination
-        
-        Args that start with '--' (eg. --prodigal) can also be set in a config file (specified via -c). Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
-        details, see syntax at https://goo.gl/R74nmi). If an arg is specified in more than one place, then commandline values override config file values which override defaults.
-        ```
-        
-        ### GAGE / PathView
-        
-        After processing the HMM files MetaCerberus calculates a KO (KEGG Orthology) counts table from KEGG/FOAM for processing through GAGE and PathView.
-        GAGE is recommended for pathway enrichment followed by PathView for visualize the metabolic pathways. A "class" file is required through the --class option to run this analysis. The output is saved under the step_10-visualizeData/combined/pathview folder. Also, at least 4 samples need to be used for this type of analysis.  
-          
-        GAGE and PathView also require internet access to be able to download information from a database. MetaCerberus will save a bash script 'run_pathview.sh' in the step_10-visualizeData/combined/pathview directory along with the KO Counts tsv files and the class file for running manualy in case MetaCerberus was run on a cluster without access to the internet.
-        
-        ### Multiprocessing / Multi-Computing with RAY
-        
-        MetaCerberus uses Ray for distributed processing. This is compatible with both multiprocessing on a single node (computer) or multiple nodes in a cluster.  
-        MetaCerberus has been tested on a cluster using Slurm <https://github.com/SchedMD/slurm>.  
-          
-        A script has been included to facilitate running MetaCerberus on Slurm. To use MetaCerberus on a Slurm cluster, setup your slurm script and run it using sbatch.  
-        
-        ```bash
-        sbatch example_script.sh
-        ```
-        
-        example script:  
-        
-        ```bash
-        #!/usr/bin/env bash
-        
-        #SBATCH --job-name=test-job
-        #SBATCH --nodes=3
-        #SBATCH --tasks-per-node=1
-        #SBATCH --cpus-per-task=16
-        #SBATCH --mem=128MB
-        #SBATCH -e slurm-%j.err
-        #SBATCH -o slurm-%j.out
-        #SBATCH --mail-type=END,FAIL,REQUEUE
-        
-        echo "====================================================="
-        echo "Start Time  : $(date)"
-        echo "Submit Dir  : $SLURM_SUBMIT_DIR"
-        echo "Job ID/Name : $SLURM_JOBID / $SLURM_JOB_NAME"
-        echo "Node List   : $SLURM_JOB_NODELIST"
-        echo "Num Tasks   : $SLURM_NTASKS total [$SLURM_NNODES nodes @ $SLURM_CPUS_ON_NODE CPUs/node]"
-        echo "======================================================"
-        echo ""
-        
-        # Load any modules or resources here
-        conda activate metacerberus
-        # source the slurm script to initialize the Ray worker nodes
-        source ray-slurm-metacerberus.sh
-        # run MetaCerberus
-        metacerberus.py --prodigal [input_folder] --illumina --dir_out [out_folder]
-        
-        echo ""
-        echo "======================================================"
-        echo "End Time   : $(date)"
-        echo "======================================================"
-        echo ""
-        ```
-        
-        ## Citing MetaCerberus
-        
-        MetaCerberus: python code for versatile Functional Ontology Assignments for Metagenomes (FOAM) database searching via Hidden Markov Models (HMM) with environmental focus of shotgun metaomics data. Preprints.
-        
-        ## CONTACT
-        
-        The informatics point-of-contact for this project is [Dr. Richard Allen White III](https://github.com/raw-lab).  
-        If you have any questions or feedback, please feel free to get in touch by email.  
-        Dr. Richard Allen White III - rwhit101@uncc.edu or raw937@gmail.com.  
-        Jose L. Figueroa III - jlfiguer@uncc.edu  
-        Or [open an issue](https://github.com/raw-lab/metacerberus/issues).  
-        
 Platform: Unix
+Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: Unix
-Requires-Python: <3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Welcome to MetaCerberus
+
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/metacerberus/README.html)
+
+## About
+
+MetaCerberus transforms raw shotgun metaomics sequencing (i.e. metagenomics/metatranscriptomic) data into knowledge. It is a start to finish python code for versatile analysis of the Functional Ontology Assignments for Metagenomes (FOAM) database and KEGG via Hidden Markov Models (HMM) for whole ecosystem metabolomic analysis.
+
+![GitHub Logo](https://raw.githubusercontent.com/raw-lab/MetaCerberus/main/metacerberus_logo.jpg)
+
+## Installing MetaCerberus
+
+### Option 1) Anaconda
+
+- Anaconda install from bioconda with all dependencies:
+
+```bash
+conda create -n metacerberus -c conda-forge -c bioconda metacerberus -y
+conda activate metacerberus
+metacerberus.py --setup
+```
+
+### Option 2) Manual Install
+
+1. Clone github Repo
+
+```bash
+git clone https://github.com/raw-lab/metacerberus.git
+```
+
+2. Run Setup File
+
+```bash
+cd metacerberus
+bash install_metacerberus.sh
+conda activate metacerberus
+metacerberus.py --setup
+```
+
+This creates an anaconda environment called "metacerberus" with all dependencies installed.
+
+## Input formats
+
+- From any NextGen sequencing technology (from Illumina, PacBio, Oxford Nanopore)
+- type 1 raw reads (.fastq format)
+- type 2 nucleotide fasta (.fasta, .fa, .fna, .ffn format), assembled raw reads into contigs
+- type 3 protein fasta (.faa format), assembled contigs which genes are converted to amino acid sequence
+
+## Output Files
+
+- If an output directory is given, that folder will be created where all files are stored.
+- If no output directory is specified, the 'pipeline' subfolder will be created in the current directory.
+- Gage/Pathview R analysis provided as separate scripts within R. 
+
+## Visualization of Outputs
+
+- We use Plotly to visualize the data
+- Once the program is executed the html reports with the visuals will be saved to the last step of the pipeline.
+- The HTML files require plotly.js to be present. One has been provided in the package and is saved to the report folder.
+
+## Quick start examples
+
+### Illumina data
+
+#### Bacterial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder] --illumina --meta --dir_out [out_folder] 
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder] --illumina --meta --dir_out [out_folder] 
+```
+
+### Nanopore data
+
+#### Bacterial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder]  --nanopore --meta --dir_out [out_folder]
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder] --nanopore --meta --dir_out [out_folder] 
+```
+
+### PacBio data
+
+#### Microbial, Archaea and Bacteriophage
+
+```bash
+conda activate metacerberus
+metacerberus.py --prodigal [input_folder]  --pacbio --meta --dir_out [out_folder]
+```
+
+#### Eukaryotes and Viruses
+
+```bash
+conda activate metacerberus
+metacerberus.py --fraggenescan [input_folder]  --pacbio --meta --dir_out [out_folder]
+```
+
+### SUPER (both methods)
+
+```bash
+conda activate metacerberus
+metacerberus.py --super [input_folder]  --pacbio/--nanopore/--illumina --meta --dir_out [out_folder]
+```
+
+- Note: Fraggenescan will work for prokaryotes and viruses/bacteriophage but prodigal will not work for eukaryotes. 
+
+## Prerequisites and dependencies
+
+- python >= 3.8
+
+### Available from Bioconda
+
+- fastqc - <https://github.com/s-andrews/FastQC>
+- fastp - <https://github.com/OpenGene/fastp>
+- porechop - <https://github.com/rrwick/Porechop>
+- bbmap - <https://sourceforge.net/projects/bbmap/> or <https://github.com/BioInfoTools/BBMap>
+- prodigal - <https://github.com/hyattpd/Prodigal>
+- hmmer - <https://github.com/EddyRivasLab/hmmer>
+
+- NOTE: The KEGG database contains KOs related to Human disease. It is possible that these will show up in the results, even when analyzing microbes.
+
+## MetaCerberus Options
+
+- If the metacerberus environment is not used, make sure the dependencies are in PATH or specified in the config file.
+- Run metacerberus.py with the options required for your project.
+
+```
+usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--super SUPER] [--protein PROTEIN] [--illumina | --nanopore | --pacbio] [--setup]
+                       [--uninstall] [--dir_out DIR_OUT] [--meta] [--scaffolds] [--minscore MINSCORE] [--evalue EVALUE] [--cpus CPUS] [--chunker CHUNKER] [--replace]
+                       [--keep] [--hmm HMM] [--class CLASS] [--tmpdir TMPDIR] [--version] [-h] [--adapters ADAPTERS] [--qc_seq QC_SEQ]
+
+options:
+  --illumina            Specifies that the given FASTQ files are from Illumina
+  --nanopore            Specifies that the given FASTQ files are from Nanopore
+  --pacbio              Specifies that the given FASTQ files are from PacBio
+
+Required arguments
+At least one sequence is required.
+<accepted formats {.fastq .fasta .faa .fna .ffn .rollup}>
+Example:
+> metaerberus.py --prodigal file1.fasta
+> metacerberus.py --config file.config
+*Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.:
+  -c CONFIG, --config CONFIG
+                        Path to config file, command line takes priority
+  --prodigal PRODIGAL   Prokaryote nucleotide sequence (includes microbes, bacteriophage)
+  --fraggenescan FRAGGENESCAN
+                        Eukaryote nucleotide sequence (includes other viruses, works all around for everything)
+  --super SUPER         Run sequence in both --prodigal and --fraggenescan modes
+  --protein PROTEIN, --amino PROTEIN
+                        Protein Amino Acid sequence
+
+optional arguments:
+  --setup               Set this flag to ensure dependencies are setup [False]
+  --uninstall           Set this flag to remove downloaded databases and FragGeneScan+ [False]
+  --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./results-metacerberus]
+  --meta                Metagenomic nucleotide sequences (for prodigal) [False]
+  --scaffolds           Sequences are treated as scaffolds [False]
+  --minscore MINSCORE   Score cutoff for parsing HMMER results [25]
+  --evalue EVALUE       E-value cutoff for parsing HMMER results [1e-09]
+  --cpus CPUS           Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]
+  --chunker CHUNKER     Split files into smaller chunks, in Megabytes [Disabled by default]
+  --replace             Flag to replace existing files. [False]
+  --keep                Flag to keep temporary files. [False]
+  --hmm HMM             Specify the database for HMMER. (KOFam_all, KOFam_eukariote, KOFam_prokaryote, COG, CAZy, PHROG, COG) [KOFam_all]
+  --class CLASS         path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R
+  --tmpdir TMPDIR       temp directory for RAY [system tmp dir]
+  --version, -v         show the version number and exit
+  -h, --help            show this help message and exit
+
+  --adapters ADAPTERS   FASTA File containing adapter sequences for trimming
+  --qc_seq QC_SEQ       FASTA File containing control sequences for decontamination
+
+Args that start with '--' (eg. --prodigal) can also be set in a config file (specified via -c). Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
+details, see syntax at https://goo.gl/R74nmi). If an arg is specified in more than one place, then commandline values override config file values which override defaults.
+```
+
+### GAGE / PathView
+
+After processing the HMM files MetaCerberus calculates a KO (KEGG Orthology) counts table from KEGG/FOAM for processing through GAGE and PathView.
+GAGE is recommended for pathway enrichment followed by PathView for visualize the metabolic pathways. A "class" file is required through the --class option to run this analysis. The output is saved under the step_10-visualizeData/combined/pathview folder. Also, at least 4 samples need to be used for this type of analysis.  
+  
+GAGE and PathView also require internet access to be able to download information from a database. MetaCerberus will save a bash script 'run_pathview.sh' in the step_10-visualizeData/combined/pathview directory along with the KO Counts tsv files and the class file for running manualy in case MetaCerberus was run on a cluster without access to the internet.
+
+### Multiprocessing / Multi-Computing with RAY
+
+MetaCerberus uses Ray for distributed processing. This is compatible with both multiprocessing on a single node (computer) or multiple nodes in a cluster.  
+MetaCerberus has been tested on a cluster using Slurm <https://github.com/SchedMD/slurm>.  
+  
+A script has been included to facilitate running MetaCerberus on Slurm. To use MetaCerberus on a Slurm cluster, setup your slurm script and run it using sbatch.  
+
+```bash
+sbatch example_script.sh
+```
+
+example script:  
+
+```bash
+#!/usr/bin/env bash
+
+#SBATCH --job-name=test-job
+#SBATCH --nodes=3
+#SBATCH --tasks-per-node=1
+#SBATCH --cpus-per-task=16
+#SBATCH --mem=128MB
+#SBATCH -e slurm-%j.err
+#SBATCH -o slurm-%j.out
+#SBATCH --mail-type=END,FAIL,REQUEUE
+
+echo "====================================================="
+echo "Start Time  : $(date)"
+echo "Submit Dir  : $SLURM_SUBMIT_DIR"
+echo "Job ID/Name : $SLURM_JOBID / $SLURM_JOB_NAME"
+echo "Node List   : $SLURM_JOB_NODELIST"
+echo "Num Tasks   : $SLURM_NTASKS total [$SLURM_NNODES nodes @ $SLURM_CPUS_ON_NODE CPUs/node]"
+echo "======================================================"
+echo ""
+
+# Load any modules or resources here
+conda activate metacerberus
+# source the slurm script to initialize the Ray worker nodes
+source ray-slurm-metacerberus.sh
+# run MetaCerberus
+metacerberus.py --prodigal [input_folder] --illumina --dir_out [out_folder]
+
+echo ""
+echo "======================================================"
+echo "End Time   : $(date)"
+echo "======================================================"
+echo ""
+```
+
+## Citing MetaCerberus
+
+MetaCerberus: python code for versatile Functional Ontology Assignments for Metagenomes (FOAM) database searching via Hidden Markov Models (HMM) with environmental focus of shotgun metaomics data. Preprints.
+
+## CONTACT
+
+The informatics point-of-contact for this project is [Dr. Richard Allen White III](https://github.com/raw-lab).  
+If you have any questions or feedback, please feel free to get in touch by email.  
+Dr. Richard Allen White III - rwhit101@uncc.edu or raw937@gmail.com.  
+Jose L. Figueroa III - jlfiguer@uncc.edu  
+Or [open an issue](https://github.com/raw-lab/metacerberus/issues).
```

### Comparing `MetaCerberus-1.0/README.md` & `MetaCerberus-1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # Welcome to MetaCerberus
 
-## About 
+[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg?style=flat)](http://bioconda.github.io/recipes/metacerberus/README.html)
+
+## About
+
 MetaCerberus transforms raw shotgun metaomics sequencing (i.e. metagenomics/metatranscriptomic) data into knowledge. It is a start to finish python code for versatile analysis of the Functional Ontology Assignments for Metagenomes (FOAM) database and KEGG via Hidden Markov Models (HMM) for whole ecosystem metabolomic analysis.
 
-![GitHub Logo](metacerberus_logo.jpg)
+![GitHub Logo](https://raw.githubusercontent.com/raw-lab/MetaCerberus/main/metacerberus_logo.jpg)
 
 ## Installing MetaCerberus
 
 ### Option 1) Anaconda
 
 - Anaconda install from bioconda with all dependencies:
 
-```
+```bash
 conda create -n metacerberus -c conda-forge -c bioconda metacerberus -y
 conda activate metacerberus
 metacerberus.py --setup
 ```
 
 ### Option 2) Manual Install
 
 1. Clone github Repo
 
-```
+```bash
 git clone https://github.com/raw-lab/metacerberus.git
 ```
 
 2. Run Setup File
 
-```
+```bash
 cd metacerberus
 bash install_metacerberus.sh
 conda activate metacerberus
 metacerberus.py --setup
 ```
 
 This creates an anaconda environment called "metacerberus" with all dependencies installed.
@@ -53,71 +56,74 @@
 
 - We use Plotly to visualize the data
 - Once the program is executed the html reports with the visuals will be saved to the last step of the pipeline.
 - The HTML files require plotly.js to be present. One has been provided in the package and is saved to the report folder.
 
 ## Quick start examples
 
-### Illumina data 
+### Illumina data
 
-#### Bacterial, Archaea and Bacteriophage 
-```
+#### Bacterial, Archaea and Bacteriophage
+
+```bash
 conda activate metacerberus
 metacerberus.py --prodigal [input_folder] --illumina --meta --dir_out [out_folder] 
 ```
 
 #### Eukaryotes and Viruses
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --fraggenescan [input_folder] --illumina --meta --dir_out [out_folder] 
 ```
 
-### Nanopore data 
+### Nanopore data
 
 #### Bacterial, Archaea and Bacteriophage
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --prodigal [input_folder]  --nanopore --meta --dir_out [out_folder]
 ```
 
 #### Eukaryotes and Viruses
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --fraggenescan [input_folder] --nanopore --meta --dir_out [out_folder] 
 ```
 
 ### PacBio data
 
 #### Microbial, Archaea and Bacteriophage
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --prodigal [input_folder]  --pacbio --meta --dir_out [out_folder]
 ```
 
 #### Eukaryotes and Viruses
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --fraggenescan [input_folder]  --pacbio --meta --dir_out [out_folder]
 ```
 
 ### SUPER (both methods)
-```
+
+```bash
 conda activate metacerberus
 metacerberus.py --super [input_folder]  --pacbio/--nanopore/--illumina --meta --dir_out [out_folder]
 ```
 
 - Note: Fraggenescan will work for prokaryotes and viruses/bacteriophage but prodigal will not work for eukaryotes. 
 
-
 ## Prerequisites and dependencies
 
-- python >= 3.7
-- MetaCerberus currently runs best with Python version 3.7, 3.8, 3.9 due to compatibility with dependencies.
-- MetaCerberus currently doesn't support Python 3.10 due to the "Ray" dependency. 
-- Python 3.10 is not currently supported.
+- python >= 3.8
 
 ### Available from Bioconda
 
 - fastqc - <https://github.com/s-andrews/FastQC>
 - fastp - <https://github.com/OpenGene/fastp>
 - porechop - <https://github.com/rrwick/Porechop>
 - bbmap - <https://sourceforge.net/projects/bbmap/> or <https://github.com/BioInfoTools/BBMap>
@@ -128,20 +134,19 @@
 
 ## MetaCerberus Options
 
 - If the metacerberus environment is not used, make sure the dependencies are in PATH or specified in the config file.
 - Run metacerberus.py with the options required for your project.
 
 ```
-usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--meta META] [--super SUPER] [--protein PROTEIN]
-                       [--illumina | --nanopore | --pacbio] [--setup] [--uninstall] [--dir_out DIR_OUT] [--scaffolds] [--minscore MINSCORE] [--cpus CPUS]
-                       [--chunker CHUNKER] [--replace] [--keep] [--hmm HMM] [--class CLASS] [--slurm_nodes SLURM_NODES] [--tmpdir TMPDIR] [--version] [-h]
-                       [--adapters ADAPTERS] [--control_seq CONTROL_SEQ]
+usage: metacerberus.py [-c CONFIG] [--prodigal PRODIGAL] [--fraggenescan FRAGGENESCAN] [--super SUPER] [--protein PROTEIN] [--illumina | --nanopore | --pacbio] [--setup]
+                       [--uninstall] [--dir_out DIR_OUT] [--meta] [--scaffolds] [--minscore MINSCORE] [--evalue EVALUE] [--cpus CPUS] [--chunker CHUNKER] [--replace]
+                       [--keep] [--hmm HMM] [--class CLASS] [--tmpdir TMPDIR] [--version] [-h] [--adapters ADAPTERS] [--qc_seq QC_SEQ]
 
-optional arguments:
+options:
   --illumina            Specifies that the given FASTQ files are from Illumina
   --nanopore            Specifies that the given FASTQ files are from Nanopore
   --pacbio              Specifies that the given FASTQ files are from PacBio
 
 Required arguments
 At least one sequence is required.
 <accepted formats {.fastq .fasta .faa .fna .ffn .rollup}>
@@ -150,40 +155,38 @@
 > metacerberus.py --config file.config
 *Note: If a sequence is given in .fastq format, one of --nanopore, --illumina, or --pacbio is required.:
   -c CONFIG, --config CONFIG
                         Path to config file, command line takes priority
   --prodigal PRODIGAL   Prokaryote nucleotide sequence (includes microbes, bacteriophage)
   --fraggenescan FRAGGENESCAN
                         Eukaryote nucleotide sequence (includes other viruses, works all around for everything)
-  --meta META           Metagenomic nucleotide sequences (Uses prodigal)
   --super SUPER         Run sequence in both --prodigal and --fraggenescan modes
   --protein PROTEIN, --amino PROTEIN
                         Protein Amino Acid sequence
 
 optional arguments:
   --setup               Set this flag to ensure dependencies are setup [False]
   --uninstall           Set this flag to remove downloaded databases and FragGeneScan+ [False]
-  --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./meta_cerberus]
+  --dir_out DIR_OUT     path to output directory, creates "pipeline" folder. Defaults to current directory. [./results-metacerberus]
+  --meta                Metagenomic nucleotide sequences (for prodigal) [False]
   --scaffolds           Sequences are treated as scaffolds [False]
-  --minscore MINSCORE   Filter for parsing HMMER results [25]
+  --minscore MINSCORE   Score cutoff for parsing HMMER results [25]
+  --evalue EVALUE       E-value cutoff for parsing HMMER results [1e-09]
   --cpus CPUS           Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]
   --chunker CHUNKER     Split files into smaller chunks, in Megabytes [Disabled by default]
   --replace             Flag to replace existing files. [False]
   --keep                Flag to keep temporary files. [False]
-  --hmm HMM             Specify a custom HMM file for HMMER. Default uses downloaded FOAM HMM Database
+  --hmm HMM             Specify the database for HMMER. (KOFam_all, KOFam_eukariote, KOFam_prokaryote, COG, CAZy, PHROG, COG) [KOFam_all]
   --class CLASS         path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R
-  --slurm_nodes SLURM_NODES
-                        list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST
   --tmpdir TMPDIR       temp directory for RAY [system tmp dir]
   --version, -v         show the version number and exit
   -h, --help            show this help message and exit
 
   --adapters ADAPTERS   FASTA File containing adapter sequences for trimming
-  --control_seq CONTROL_SEQ
-                        FASTA File containing control sequences for decontamination
+  --qc_seq QC_SEQ       FASTA File containing control sequences for decontamination
 
 Args that start with '--' (eg. --prodigal) can also be set in a config file (specified via -c). Config file syntax allows: key=value, flag=true, stuff=[a,b,c] (for
 details, see syntax at https://goo.gl/R74nmi). If an arg is specified in more than one place, then commandline values override config file values which override defaults.
 ```
 
 ### GAGE / PathView
```

### Comparing `MetaCerberus-1.0/bin/metacerberus.py` & `MetaCerberus-1.1/bin/metacerberus.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 
 """metacerberus.py: Versatile Functional Ontology Assignments for Metagenomes
 
 Uses Hidden Markov Model (HMM) searching with environmental focus of shotgun metaomics data.
 """
 
 
-__version__     = "1.0"
+__version__     = "1.1"
 __author__      = "Jose L. Figueroa III, Richard A. White III"
-__copyright__   = "Copyright 2022"
-
+__copyright__   = "Copyright 2023"
+__date__        = "July 2023"
 
 def warn(*args, **kwargs):
-    #print("args", str(args))
     pass
 import warnings
 warnings.warn = warn
 
 import sys
 import os
+import re
+from pathlib import Path
 import psutil
 import shutil
 import subprocess
 import configargparse as argparse #replace argparse with: https://pypi.org/project/ConfigArgParse/
 import pkg_resources as pkg #to import package data files
 import time
 import datetime
+from urllib import request
 import socket
 import ray #parallel-processing
 import pandas as pd
 
 
 # our package import
 from meta_cerberus import (
@@ -44,112 +46,85 @@
 ##### Global Variables #####
 
 # known file extensions
 FILES_FASTQ = ['.fastq', '.fastq.gz']
 FILES_FASTA = [".fasta", ".fa", ".fna", ".ffn"]
 FILES_AMINO = [".faa"]
 
-# External file downloads
-pathDB = pkg.resource_filename("meta_cerberus", "cerberusDB")
-pathFGS = pkg.resource_filename("meta_cerberus", "FGS+")
+# External file paths
+pathDB = pkg.resource_filename("meta_cerberus", "DB")
+pathFGS = pkg.resource_filename("meta_cerberus", "FGS")
 
-# refseq default locations (for decontamination)
-REFSEQ = {
+# qc sequence default locations (for decontamination)
+QC_SEQ = {
     "adapters": pkg.resource_filename("meta_cerberus", "dependency_files/adapters.fna"),
     "illumina": pkg.resource_filename("meta_cerberus", "dependency_files/phix174_ill.ref.fna"),
     "lambda": pkg.resource_filename("meta_cerberus", "dependency_files/lambda-phage.fna"),
     "pacbio": pkg.resource_filename("meta_cerberus", "dependency_files/PacBio_quality-control.fna")
 }
 
 # external dependencies
 DEPENDENCIES = {
     'EXE_FASTQC': 'fastqc',
     'EXE_FLASH' : 'flash2',
     'EXE_FASTP': 'fastp',
     'EXE_PORECHOP': 'porechop',
     'EXE_BBDUK': 'bbduk.sh',
-    'EXE_FGS+': 'FGS+',
+    'EXE_FGS': 'FragGeneScanRs',
     'EXE_PRODIGAL': 'prodigal',
     'EXE_HMMSEARCH': 'hmmsearch',
     'EXE_COUNT_ASSEMBLY': 'countAssembly.py'
     }
 
+# Databases
+DB_HMM = dict(
+    KOFam_all=Path(pathDB, 'KOFam_all.hmm.gz'),
+    KOFam_prokaryote=Path(pathDB, 'KOFam_prokaryote.hmm.gz'),
+    KOFam_eukaryote=Path(pathDB, 'KOFam_eukaryote.hmm.gz'),
+    COG=Path(pathDB, 'COG-noIter.hmm.gz'),
+    CAZy=Path(pathDB, 'CAZy.hmm.gz'),
+    PHROG=Path(pathDB, 'PHROG.hmm.gz'),
+    VOG=Path(pathDB, 'VOG.hmm.gz'),
+    )
+
 # step names
 STEP = {
     1:"step_01-loadFiles",
     2:"step_02-QC",
     3:"step_03-trim",
     4:"step_04-decontaminate",    
     5:"step_05-format",
     6:"step_06-metaomeQC",
     7:"step_07-geneCall",
     8:"step_08-hmmer",
     9:"step_09-parse",
     10:"step_10-visualizeData"}
 
 
-## PRINT to stderr ##
-def eprint(*args, **kwargs):
-    print(*args, file=sys.stderr, **kwargs)
-    return
+def set_add(to_set:set, item, msg:str):
+    if item not in to_set:
+        to_set.add(item)
+        print('\n', msg, '\n', sep='')
+    return to_set
 
 def logTime(dirout, host, funcName, path, time):
     with open(f'{dirout}/time.tsv', 'a+') as outTime:
         print(host, funcName, time, path, file=outTime, sep='\t')
     return
 
-# Setup SLURM
-def slurm(SLURM_JOB_NODELIST):
-    """Sets up RAY on a SLURM cluster
-    Not Yet Fully Implemented"""
-
-    proc = subprocess.run(['scontrol', 'show', 'hostnames', SLURM_JOB_NODELIST],
-        stdout=subprocess.PIPE, text=True)
-    if proc.returncode == 0:
-        nodes = proc.stdout.split()
-    else:
-        print(f"ERROR executing 'scontrol show hostnames {SLURM_JOB_NODELIST}'")
-        return None
-    print("NODES:", nodes)
-
-    head_node = nodes[0]
-    proc = subprocess.run(['srun', '--nodes=1', '--ntasks=1', '-w', head_node, 'hostname', '--ip-address'],
-        stdout=subprocess.PIPE, text=True)
-    if proc.returncode == 0:
-        head_node_ip = proc.stdout.strip()
-    else:
-        print(f"ERROR getting head node IP")
-        return None
 
-    port = 6379
-    ip_head = f"{head_node_ip}:{port}"
-    print("IP Head:", ip_head)
-
-    print("Starting HEAD at", head_node)
-    cmd = ["srun", "--nodes=1", "--ntasks=1", "-w", head_node, "ray", "start", "--head", f"--node-ip-address={head_node_ip}", f"--port={port}", "--num-cpus", "1", "--block"]
-    subprocess.Popen(cmd)
-    time.sleep(5)
-
-    # Start Worker Nodes
-    for i in range(1, len(nodes)):
-        print(f"Starting WORKER {i} at {nodes[i]}")
-        cmd = ["srun", "--nodes=1", "--ntasks=1", "-w", nodes[i], "ray", "start", "--address", ip_head, "--num-cpus", "1", "--block"]
-        subprocess.Popen(cmd)
-        time.sleep(5)
-    return
-
-
-## RAY WORKER THREADS ##
+## Ray Worker Threads ##
 @ray.remote
-def rayWorker(func, key, value, config, path):
+def rayWorkerThread(func, key, dir_log, params:list):
     start = time.time()
-    ret = func(value, config, path)
+    ret = func(*params)
     end = str(datetime.timedelta(seconds=time.time()-start))
-    logTime(config["DIR_OUT"], socket.gethostname(), func.__name__, path, end)
-    return key, ret
+    logTime(dir_log, socket.gethostname(), func.__name__, key, end)
+    return key, ret, func.__name__
+
 
 ## MAIN
 def main():
     ## Parse the command line
     parser = argparse.ArgumentParser(add_help=False)
     parser.set_defaults()
     # At least one of these options are required
@@ -170,49 +145,66 @@
     readtype.add_argument('--illumina', action="store_true", help="Specifies that the given FASTQ files are from Illumina")
     readtype.add_argument('--nanopore', action="store_true", help="Specifies that the given FASTQ files are from Nanopore")
     readtype.add_argument('--pacbio', action="store_true", help="Specifies that the given FASTQ files are from PacBio")
     # optional flags
     optional = parser.add_argument_group('optional arguments')
     optional.add_argument('--setup', action="store_true", help="Set this flag to ensure dependencies are setup [False]")
     optional.add_argument('--uninstall', action="store_true", help="Set this flag to remove downloaded databases and FragGeneScan+ [False]")
-    optional.add_argument('--dir_out', type=str, default='./meta_cerberus', help='path to output directory, creates "pipeline" folder. Defaults to current directory. [./meta_cerberus]')
+    optional.add_argument('--dir_out', type=str, default='./results-metacerberus', help='path to output directory, creates "pipeline" folder. Defaults to current directory. [./results-metacerberus]')
     optional.add_argument('--meta', action="store_true", help="Metagenomic nucleotide sequences (for prodigal) [False]")
     optional.add_argument('--scaffolds', action="store_true", help="Sequences are treated as scaffolds [False]")
-    optional.add_argument('--minscore', type=float, default=25, help="Filter for parsing HMMER results [25]")
+    optional.add_argument('--minscore', type=float, default=25, help="Score cutoff for parsing HMMER results [25]")
+    optional.add_argument('--evalue', type=float, default=1e-09, help="E-value cutoff for parsing HMMER results [1e-09]")
     optional.add_argument('--cpus', type=int, help="Number of CPUs to use per task. System will try to detect available CPUs if not specified [Auto Detect]")
     optional.add_argument('--chunker', type=int, default=0, help="Split files into smaller chunks, in Megabytes [Disabled by default]")
     optional.add_argument('--replace', action="store_true", help="Flag to replace existing files. [False]")
     optional.add_argument('--keep', action="store_true", help="Flag to keep temporary files. [False]")
-    optional.add_argument('--hmm', type=str, default='', help="Specify a custom HMM file for HMMER. Default uses downloaded FOAM HMM Database")
+    optional.add_argument('--hmm', type=str, default='KOFam_all', help="Specify the database for HMMER. (KOFam_all, KOFam_eukariote, KOFam_prokaryote, COG, CAZy, PHROG, COG) [KOFam_all]")
     optional.add_argument('--class', type=str, default='', help='path to a tsv file which has class information for the samples. If this file is included scripts will be included to run Pathview in R')
-    optional.add_argument('--slurm_nodes', type=str, default="", help='list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST')
+    optional.add_argument('--slurm_nodes', type=str, default="", help=argparse.SUPPRESS)# help='list of node hostnames from SLURM, i.e. $SLURM_JOB_NODELIST.')
     optional.add_argument('--tmpdir', type=str, default="", help='temp directory for RAY [system tmp dir]')
     optional.add_argument('--version', '-v', action='version',
-                        version=f'MetaCerberus: \n version: {__version__} June 24th 2021',
+                        version=f'MetaCerberus: \n version: {__version__} {__date__}',
                         help='show the version number and exit')
     optional.add_argument("-h", "--help", action="help", help="show this help message and exit")
     # Hidden from help, expected to load from config file
     dependencies = parser.add_argument_group()
     for key in DEPENDENCIES:
         dependencies.add_argument(f"--{key}", help=argparse.SUPPRESS)
-    dependencies.add_argument('--adapters', type=str, default=REFSEQ['adapters'], help="FASTA File containing adapter sequences for trimming")
-    dependencies.add_argument('--control_seq', type=str, default="default", help="FASTA File containing control sequences for decontamination")
+    dependencies.add_argument('--adapters', type=str, default=QC_SEQ['adapters'], help="FASTA File containing adapter sequences for trimming")
+    dependencies.add_argument('--qc_seq', type=str, default="default", help="FASTA File containing control sequences for decontamination")
 
     args = parser.parse_args()
 
     if args.uninstall:
         metacerberus_setup.Remove(pathDB, pathFGS)
 
     if args.setup:
-        metacerberus_setup.Download(pathDB)
         metacerberus_setup.FGS(pathFGS)
+        metacerberus_setup.Download(pathDB)
 
     if args.setup or args.uninstall:
         return 0
 
+
+    # TODO: Add Custom HMM DB
+    dbHMM = dict()
+    for i,hmm in enumerate([x.strip() for x in args.hmm.split(',')], 1):
+        print(f"HMM: '{hmm}'")
+        if hmm in DB_HMM:
+            if DB_HMM[hmm].exists():
+                dbHMM[hmm] = DB_HMM[hmm]
+            else:
+                print(f"ERROR: Cannot use '{hmm}', please download it using 'metacerberus.py --setup")
+        else:
+            print(f"ERROR: Cannot use '{hmm}', custom databases not supported yet. Please use one of:", *list(DB_HMM.keys()))
+    if not len(dbHMM):
+        print("ERROR: No HMM DB Loaded")
+        return 1
+
     print("\nStarting MetaCerberus Pipeline\n")
 
     # Merge related arguments
     if args.super:
         args.prodigal += args.super
         args.fraggenescan += args.super
 
@@ -220,39 +212,38 @@
     if not any([args.prodigal, args.fraggenescan, args.protein]):
         parser.error('At least one sequence must be declared either in the command line or through the config file')
     # Check sequence type
     for file in args.prodigal + args.fraggenescan:
         if '.fastq' in file:
             if not any([args.illumina, args.nanopore, args.pacbio]):
                 parser.error('A .fastq file was given, but no flag specified as to the type.\nPlease use one of --illumina, --nanopore, or --pacbio')
-            elif args.control_seq =="default":
+            elif args.qc_seq =="default":
                 if args.illumina:
-                    args.control_seq = REFSEQ["illumina"]
+                    args.qc_seq = QC_SEQ["illumina"]
                 if args.nanopore:
-                    args.control_seq = REFSEQ["lambda"]
+                    args.qc_seq = QC_SEQ["lambda"]
                 if args.pacbio:
-                    args.control_seq = REFSEQ["pacbio"]
+                    args.qc_seq = QC_SEQ["pacbio"]
 
     # Initialize Config Dictionary
     config = {}
-    #config['PATH'] = os.path.dirname(os.path.abspath(__file__))
     config['STEP'] = STEP
     config['PATHDB'] = pathDB
 
     # Get FGS+ Folder from Library Path
-    config['EXE_FGS+'] = os.path.join(pathFGS, 'FGS+')
+    config['EXE_FGS'] = os.path.join(pathFGS, DEPENDENCIES["EXE_FGS"])
 
     # load all args into config
     for arg,value in args.__dict__.items():
         if value is not None:
-            if arg == "control_seq": arg = "refseq"
             arg = arg.upper()
             if type(value) is str and os.path.isfile(value):
                 value = os.path.abspath(os.path.expanduser(value))
             config[arg] = value
+    config['HMM'] = dbHMM
     
 
     # Create output directory
     config['DIR_OUT'] = os.path.abspath(os.path.expanduser(args.dir_out))
     os.makedirs(config['DIR_OUT'], exist_ok=True)
 
     # Sequence File extensions
@@ -283,29 +274,31 @@
     for key,value in config.items():
         if key.startswith("EXE_") and not os.path.isfile(value):
             parser.error(f"Unable to find file: {value}")
 
 
     # Initialize RAY for Multithreading
     print("Initializing RAY")
-    if config['TMPDIR']:
-        tmpdir = os.path.abspath(os.path.expanduser(config['TMPDIR']))
-        os.environ['RAY_TMPDIR'] = tmpdir
-        os.makedirs(tmpdir, exist_ok=True)
+
     # First try if ray is setup for a cluster
+    #TODO: Fix this, does not set up slurm script
     if config['SLURM_NODES']:
-        slurm(config['SLURM_NODES'])
+        metacerberus_setup.slurm(config['SLURM_NODES'])
     
-    try:
-        ray.init(address='auto', log_to_driver=False)
-    except:
-        ray.init(log_to_driver=False)
     # Get CPU Count
     if 'CPUS' not in config:
         config['CPUS'] = psutil.cpu_count()
+    try:
+        ray.init(address='auto')#, log_to_driver=False)
+        print("Started RAY on cluster")
+        config['CLUSTER'] = True
+    except:
+        ray.init(num_cpus=config['CPUS'])#log_to_driver=False)
+        print("Started RAY single node")
+        config['CLUSTER'] = False
     print(f"Running RAY on {len(ray.nodes())} node(s)")
     print(f"Using {config['CPUS']} CPUs per node")
 
 
     startTime = time.time()
     # Step 1 - Load Input Files
     print("\nSTEP 1: Loading sequence files:")
@@ -363,331 +356,337 @@
         else:
             print(f'{item} is not a valid sequence')
     
     print(f"Processing {len(fastq)} fastq sequences")
     print(f"Processing {len(fasta)} fasta sequences")
     print(f"Processing {len(amino)} protein Sequences")
 
-    # Step 2 (check quality of fastq files)
-    jobsQC = []
+    # Main Pipeline
+    pipeline = list()
+    step_curr = set()
+    
+    # Entry Point: Fastq
     if fastq:
+        # Step 2 (check quality of fastq files)
         print("\nSTEP 2: Checking quality of fastq files")
         for key,value in fastq.items():
-            jobsQC.append(rayWorker.remote(metacerberus_qc.checkQuality, key, value, config, f"{STEP[2]}/{key}"))
-
-
-    # Step 3 (trim fastq files)
-    jobTrim = []
-    if fastq:
+            pipeline.append(rayWorkerThread.remote(metacerberus_qc.checkQuality, key, config['DIR_OUT'], [value, config, f"{STEP[2]}/{key}"]))
         print("\nSTEP 3: Trimming fastq files")
         # Merge Paired End Reads
         fastqPaired = {k:v for k,v in fastq.items() if "R1.fastq" in v and v.replace("R1.fastq", "R2.fastq") in fastq.values() }
         for key,value in fastqPaired.items():
             reverse = fastq.pop(key.replace("R1", "R2"))
             fastq[key] = metacerberus_merge.mergePairedEnd([value,reverse], config, f"{STEP[3]}/{key}/merged")
         del fastqPaired # memory cleanup
         # Trim
         for key,value in fastq.items():
-            jobTrim.append(rayWorker.remote(metacerberus_trim.trimSingleRead, key, [key, value], config, f"{STEP[3]}/{key}"))
-
-    # Wait for Trimmed Reads
-    while jobTrim:
-        ready,jobTrim = ray.wait(jobTrim)
-        key,value = ray.get(ready[0])
-        fastq[key] = value
-        jobsQC.append(rayWorker.remote(metacerberus_qc.checkQuality, key+'_trim', value, config, f"{STEP[3]}/{key}/quality"))
-
+            pipeline.append(rayWorkerThread.remote(metacerberus_trim.trimSingleRead, key, config['DIR_OUT'], [[key, value], config, Path(STEP[3], key)]))
 
-    # step 4 Decontaminate (adapter free read to clean quality read + removal of junk)
-    jobDecon = []
-    if fastq and config['ILLUMINA']:
-        print("\nSTEP 4: Decontaminating trimmed files")
-        for key,value in fastq.items():
-            jobDecon.append(rayWorker.remote(metacerberus_decon.deconSingleReads, key, [key, value], config, f"{STEP[4]}/{key}"))
-
-    # Wait for Decontaminating Reads
-    while jobDecon:
-        ready,jobDecon = ray.wait(jobDecon)
-        key,value = ray.get(ready[0])
-        fastq[key] = value
-        jobsQC.append(rayWorker.remote(metacerberus_qc.checkQuality, key+'_decon', value, config, f"{STEP[4]}/{key}/quality"))
-
-
-    # step 5a for cleaning contigs
-    jobContigs = [] #TODO: Add config flag for contigs/scaffolds/raw reads
+    # Step 5 Contig Entry Point
     # Only do this if a fasta file was given, not if fastq
     if fasta:# and "scaffold" in config:
         print("\nSTEP 5a: Removing N's from contig files")
         for key,value in fasta.items():
-            jobContigs.append(rayWorker.remote(metacerberus_formatFasta.removeN, key, value, config, f"{STEP[5]}/{key}"))
+            pipeline.append(rayWorkerThread.remote(metacerberus_formatFasta.removeN, key, config['DIR_OUT'], [value, config, Path(STEP[5], key)]))
 
-    NStats = {}
-    for job in jobContigs:
-        key,value = ray.get(job)
-        fasta[key] = value[0]
-        if value[1]:
-            NStats[key] = value[1]
 
-    # step 5b Format (convert fq to fna. Remove quality scores and N's)
-    jobFormat = []
-    if fastq:
-        print("\nSTEP 5b: Reformating FASTQ files to FASTA format")
-        for key,value in fastq.items():
-            jobFormat.append(rayWorker.remote(metacerberus_formatFasta.reformat, key, value, config, f"{STEP[5]}/{key}"))
+    # Step 8 Protein Entry Point
+    jobsORF = 0
+    if amino:
+        set_add(step_curr, 8, "STEP 8: HMMER Search")
+        for key,value in amino.items():
+            pipeline += [ray.put([key, value, 'findORF_'])]
+            jobsORF += 1
+    
+    NStats = dict()
+    readStats = dict()
+    report_path = os.path.join(config['DIR_OUT'], STEP[10])
 
-    for job in jobFormat:
-        key, value = ray.get(job)
-        fasta[key] = value
-
-    # step 6 Metaome Stats
-    readStats = {}
-    if fasta:
-        print("\nSTEP 6: Metaome Stats\n")
-        for key,value in fasta.items():
-                readStats[key] = metacerberus_metastats.getReadStats(value, config, os.path.join(STEP[6], key))
+    amino_queue = dict()
+    jobs_per_node = int(-(config["CPUS"] // -4))
+    dictChunks = dict()
+    dictHMM = dict()
+    hmm_tsv = dict()
+    hmmRollup = {}
+    hmmCounts = {}
+    while pipeline:
+        ready,pipeline = ray.wait(pipeline, timeout=1)
+        if not ready:
+            continue
+        key,value,func = ray.get(ready[0])
 
-    # step 7 (ORF Finder)
-    jobGenecall = []
-    if fasta:
-        print("\nSTEP 7: ORF Finder")
-        for key,value in fasta.items():
+        if func == "checkQuality":
+            name = key
+            key = key.rstrip('_decon').rstrip('_trim')
+            os.makedirs(os.path.join(report_path, key), exist_ok=True)
+            shutil.copy(value, os.path.join(report_path, key, f"qc_{name}.html"))
+        if func == "trimSingleRead":
+            # Wait for Trimmed Reads
+            fastq[key] = value
+            pipeline.append(rayWorkerThread.remote(metacerberus_qc.checkQuality, key+'_trim', config['DIR_OUT'], [value, config, f"{STEP[3]}/{key}/quality"]))
+            if fastq and config['ILLUMINA']:
+                set_add(step_curr, 4, "STEP 4: Decontaminating trimmed files")
+                pipeline.append(rayWorkerThread.remote(metacerberus_decon.deconSingleReads, config['DIR_OUT'], key, [[key, value], config, f"{STEP[4]}/{key}"]))
+            else:
+                set_add(step_curr, 5.2, "STEP 5b: Reformating FASTQ files to FASTA format")
+                pipeline.append(rayWorkerThread.remote(metacerberus_formatFasta.reformat, config['DIR_OUT'], key, [value, config, f"{STEP[5]}/{key}"]))
+        if func == "deconSingleReads":
+            fastq[key] = value
+            pipeline.append(rayWorkerThread.remote(metacerberus_qc.checkQuality, key+'_decon', config['DIR_OUT'], [value, config, f"{STEP[4]}/{key}/quality"]))
+        if func == "removeN":
+            fasta[key] = value[0]
+            if value[1]:
+                NStats[key] = value[1]
+            set_add(step_curr, 6, "STEP 6: Metaome Stats")
+            readStats[key] = metacerberus_metastats.getReadStats(value[0], config, os.path.join(STEP[6], key))
+            set_add(step_curr, 7, "STEP 7: ORF Finder")
             if key.startswith("FragGeneScan_"):
-                jobGenecall.append(rayWorker.remote(metacerberus_genecall.findORF_fgs, key, value, config, f"{STEP[7]}/{key}"))
+                pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_fgs, key, config['DIR_OUT'], [value[0], config, f"{STEP[7]}/{key}"]))
             else:
                 if config['META']:
-                    jobGenecall.append(rayWorker.remote(metacerberus_genecall.findORF_meta, key, value, config, f"{STEP[7]}/{key}"))
+                    pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_meta, key, config['DIR_OUT'], [value[0], config, f"{STEP[7]}/{key}"]))
                 else:
-                    jobGenecall.append(rayWorker.remote(metacerberus_genecall.findORF_prod, key, value, config, f"{STEP[7]}/{key}"))
-
-    # Waiting for GeneCall
-    for job in jobGenecall:
-        key,value = ray.get(job)
-        if value:
-            amino[key] = value
-
-
-    # step 8 (HMMER)
-    print("\nSTEP 8: HMMER Search")
-
-    jobHMM = []
-    chunker = {}
-    hmm_tsv = {}
-    limit = int(config["CPUS"]/4)
-    iter_amino = iter(amino)
-    for key in iter_amino:
-        tsv_file = os.path.join(config['DIR_OUT'], STEP[8], key, f"{key}.tsv")
-        if not config['REPLACE'] and os.path.exists(tsv_file):
-            hmm_tsv[key] = tsv_file
-            continue
-        # Split files into chunks
-        if config['CHUNKER'] > 0:
-            chunker[key] = Chunker.Chunker(amino[key], os.path.join(config['DIR_OUT'], 'chunks', key), f"{config['CHUNKER']}M", '>')
-            c = 0
-            for i in range(0, len(chunker[key].files), limit):
-                files = chunker[key].files[i:i+limit]
-                aminoAcids = {}
-                for chunk in files:
-                    aminoAcids[f'chunk_{c}'] = chunk
-                    c += 1
-                jobHMM.append(rayWorker.remote(metacerberus_hmm.searchHMM, key, aminoAcids, config, f"{STEP[8]}/{key}"))
-        else:
-            aminoAcids = {}
-            aminoAcids[key] = amino[key]
-            for i in range(0, limit-1):
-                try:
-                    key = next(iter_amino)
-                except:
-                    break
-                aminoAcids[key] = amino[key]
-            jobHMM.append(rayWorker.remote(metacerberus_hmm.searchHMM, list(aminoAcids.keys()), aminoAcids, config, f"{STEP[8]}"))
-    print("Waiting for HMMER")
-    dictChunks = dict()
-    while(jobHMM):
-        readyHMM, jobHMM = ray.wait(jobHMM)
-        keys,values = ray.get(readyHMM[0])
-        if type(keys) is str:
-            # files in list belongs to same key
-            for value in values:
-                if keys not in dictChunks:
-                    dictChunks[keys] = []
-                dictChunks[keys].append(value)
-        else:
-            # files in list belongs to different keys
-            for i in range(0,len(keys)):
-                key = keys[i]
-                value = values[i]
-                if key not in dictChunks:
-                    dictChunks[key] = []
-                dictChunks[key].append(value)
-
-    # Merge chunked results
-    print("Merging HMMER Results")
-    for key,value in dictChunks.items():
-        tsv_file = os.path.join(config['DIR_OUT'], STEP[8], key, f"{key}.tsv")
-        with open(tsv_file, 'w') as writer:
-            #print("target", "score", "e-value", "query", sep='\t', file=writer)
-            for item in sorted(value):
-                writer.write(open(item).read())
-                os.remove(item)
-        hmm_tsv[key] = tsv_file
-    del dictChunks
-    # Delete chunked files
-    for key,value in chunker.items():
-        for item in value.files:
-            os.remove(item)
-
-    # step 9 (Parser)
-    print("\nSTEP 9: Parse HMMER results")
-    jobParse = []
-    for key,value in hmm_tsv.items():
-        jobParse.append(rayWorker.options(num_cpus=1).remote(metacerberus_parser.parseHmmer, key, value, config, f"{STEP[9]}/{key}"))
-
-    hmmRollup = {}
-    hmmCounts = {}
-    jobCounts = []
-    while(jobParse + jobCounts):
-        ready,jobParse = ray.wait(jobParse, timeout=0)
-        if ready:
-            key,value = ray.get(ready[0])
+                    pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_prod, key, config['DIR_OUT'], [value[0], config, f"{STEP[7]}/{key}"]))
+            jobsORF += 1
+        if func == "reformat":
+            fasta[key] = value
+            set_add(step_curr, 7, "STEP 7: ORF Finder")
+            if key.startswith("FragGeneScan_"):
+                pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_fgs, key, config['DIR_OUT'], [value, config, f"{STEP[7]}/{key}"]))
+            else:
+                if config['META']:
+                    pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_meta, key, config['DIR_OUT'], [value, config, f"{STEP[7]}/{key}"]))
+                else:
+                    pipeline.append(rayWorkerThread.remote(metacerberus_genecall.findORF_prod, key, config['DIR_OUT'], [value, config, f"{STEP[7]}/{key}"]))
+            jobsORF += 1
+        if func.startswith("findORF_"):
+            set_add(step_curr, 8, "STEP 8: HMMER Search")
+            if value:
+                amino[key] = value
+                if not config['CLUSTER']:
+                    if config['CHUNKER'] > 0:
+                        chunks = Chunker.Chunker(amino[key], os.path.join(config['DIR_OUT'], 'chunks', key), f"{config['CHUNKER']}M", '>')
+                        chunkCount = 1
+                        for chunk in chunks.files:
+                            key_chunk = f'chunk{chunkCount}-{len(chunks.files)}_{key}'
+                            chunkCount += 1
+                            val_chunk = chunk
+                            for hmm in dbHMM.items(): #TODO: Fix long line syntax
+                                pipeline.append(rayWorkerThread.options(num_cpus=4).remote(metacerberus_hmm.searchHMM, [key_chunk], config['DIR_OUT'],
+                                                                                        [{key_chunk:val_chunk}, config, Path(STEP[8], key), hmm, 4]))
+                    else:
+                        for hmm in dbHMM.items():
+                            pipeline.append(rayWorkerThread.options(num_cpus=4).remote(metacerberus_hmm.searchHMM, [key], config['DIR_OUT'],
+                                                                    [{key:value}, config, Path(STEP[8]), hmm, 4]))
+                    continue
+                if config['CHUNKER'] > 0:
+                    chunks = Chunker.Chunker(amino[key], os.path.join(config['DIR_OUT'], 'chunks', key), f"{config['CHUNKER']}M", '>')
+                    chunkCount = 1
+                    for chunk in chunks.files:
+                        amino_queue[f'chunk{chunkCount}-{len(chunks.files)}_{key}'] = chunk
+                        chunkCount += 1
+                        jobsORF -= 1
+                        # submit searchHMM jobs
+                        if len(amino_queue) >= jobs_per_node:
+                            for hmm in dbHMM.items():
+                                pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, list(amino_queue.keys()), config['DIR_OUT'],
+                                                                    [amino_queue, config, Path(STEP[8]), hmm]))
+                            amino_queue = dict()
+                else:
+                    amino_queue[key] = value
+                    jobsORF -= 1
+                # submit searchHMM jobs
+                if len(amino_queue) >= jobs_per_node or jobsORF == 0:
+                    for hmm in dbHMM.items():
+                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.searchHMM, list(amino_queue.keys()), config['DIR_OUT'],
+                                                               [amino_queue, config, Path(STEP[8]), hmm]))
+                    amino_queue = dict()
+        if func.startswith('searchHMM'):
+            keys = key
+            for key,tsv_file in zip(keys,value):
+                match = re.search(r"^chunk(\d+)-(\d+)_(.+)", key)
+                if match: # Matches if the keys are part of chunks
+                    i,l,key = match.groups()
+                    if key not in dictChunks:
+                        dictChunks[key] = list()
+                    dictChunks[key].append(tsv_file)
+                    if len(dictChunks[key]) >= int(l):
+                        # All chunks of a file have returned
+                        tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{key}.tsv")
+                        tsv_out.parent.mkdir(parents=True, exist_ok=True)
+                        if key not in dictHMM:
+                            dictHMM[key] = 1
+                            with tsv_out.open('w') as writer:
+                                print("target", "query", "e-value", "score", "length", "start", "end", sep='\t', file=writer)
+                                for item in sorted(dictChunks[key]):
+                                    writer.write(open(item).read())
+                                    dictChunks[key].remove(item)
+                                    os.remove(item)
+                        else:
+                            dictHMM[key] += 1
+                            with tsv_out.open('a') as writer:
+                                for item in sorted(dictChunks[key]):
+                                    writer.write(open(item).read())
+                                    dictChunks[key].remove(item)
+                                    os.remove(item)
+                        if dictHMM[key] == len(dbHMM):
+                            tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
+                            set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
+                            pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
+                else: # Not chunked file
+                    tsv_out = Path(config['DIR_OUT'], STEP[8], key, f"{key}.tsv")
+                    if key not in dictHMM:
+                        dictHMM[key] = 1
+                        with tsv_out.open('w') as writer:
+                            print("target", "query", "e-value", "score", "length", "start", "end", sep='\t', file=writer)
+                            writer.write(open(tsv_file).read())
+                            os.remove(tsv_file)
+                    else:
+                        dictHMM[key] += 1
+                        with tsv_out.open('a') as writer:
+                            writer.write(open(tsv_file).read())
+                            os.remove(tsv_file)
+                    if dictHMM[key] == len(dbHMM):
+                        tsv_filtered = Path(config['DIR_OUT'], STEP[8], key, "filtered.tsv")
+                        set_add(step_curr, 8.1, "STEP 8: Filtering HMMER results")
+                        pipeline.append(rayWorkerThread.remote(metacerberus_hmm.filterHMM, key, config['DIR_OUT'], [tsv_out, tsv_filtered, config['PATHDB']]))
+        if func.startswith('filterHMM'):
+            hmm_tsv[key] = value
+            set_add(step_curr, 9, "STEP 9: Parse HMMER results")
+            pipeline.append(rayWorkerThread.remote(metacerberus_parser.parseHmmer, key, config['DIR_OUT'], [value, config, f"{STEP[9]}/{key}"]))
+        if func.startswith('parseHmmer'):
             hmmRollup[key] = value
-            jobCounts.append( rayWorker.options(num_cpus=1).remote(metacerberus_parser.createCountTables, key, value, config, f"{STEP[9]}/{key}") )
-
-        ready,jobCounts = ray.wait(jobCounts, timeout=0)
-        if ready:
-            key,value = ray.get(ready[0])
+            pipeline.append(rayWorkerThread.remote(metacerberus_parser.createCountTables, key, config['DIR_OUT'], [value, config, f"{STEP[9]}/{key}"]))
+        if func.startswith('createCountTables'):
             hmmCounts[key] = value
 
+    # End main pipeline
+
+    # Log time of main pipeline
+    time_pipeline = str(datetime.timedelta(seconds=time.time()-startTime))
+    logTime(config["DIR_OUT"], socket.gethostname(), "Pipeline_time", config["DIR_OUT"], time_pipeline)
+
     # step 10 (Report)
     print("\nSTEP 10: Creating Reports")
-    outpath = os.path.join(config['DIR_OUT'], STEP[10])
 
     # Copy report files from QC, Parser
-    print("Copying QC reports")
-    while(jobsQC):
-        ready, jobsQC = ray.wait(jobsQC)
-        key,value = ray.get(ready[0])
-        name = key
-        key = key.rstrip('_decon').rstrip('_trim')
-        os.makedirs(os.path.join(outpath, key), exist_ok=True)
-        shutil.copy(value, os.path.join(outpath, key, f"qc_{name}.html"))
     for key in hmmRollup.keys():
-        os.makedirs(os.path.join(outpath, key), exist_ok=True)
-        shutil.copy( os.path.join(config['DIR_OUT'], config['STEP'][9], key, "HMMER_top_5.tsv"), os.path.join(outpath, key) )
+        os.makedirs(os.path.join(report_path, key), exist_ok=True)
+        shutil.copy( os.path.join(config['DIR_OUT'], config['STEP'][9], key, "HMMER_top_5.tsv"), os.path.join(report_path, key) )
 
     # Write Stats
     print("Saving Statistics")
     protStats = {}
-    for key,value in hmm_tsv.items():
-        protStats[key] = metacerberus_prostats.getStats(amino[key], value, hmmCounts[key], config)
-    metacerberus_report.write_Stats(outpath, readStats, protStats, NStats, config)
+    for key in hmm_tsv.keys():
+        protStats[key] = metacerberus_prostats.getStats(amino[key], hmm_tsv[key], hmmCounts[key], config, Path(report_path, key, 'annotation_summary.tsv'))
+    metacerberus_report.write_Stats(report_path, readStats, protStats, NStats, config)
     del protStats
 
-
-    # write roll-up tables
-    print("Creating rollup tables")
+    # Write Roll-up Tables
+    print("Creating Rollup Tables")
     for sample,tables in hmmCounts.items():
-        os.makedirs(f"{outpath}/{sample}", exist_ok=True)
+        os.makedirs(f"{report_path}/{sample}", exist_ok=True)
         for name,table in tables.items():
-            metacerberus_report.writeTables(table, f"{outpath}/{sample}/{name}")
+            metacerberus_report.writeTables(table, f"{report_path}/{sample}/{name}")
     for sample,tables in hmmRollup.items():
-        os.makedirs(f"{outpath}/{sample}", exist_ok=True)
+        os.makedirs(f"{report_path}/{sample}", exist_ok=True)
         for name,table in tables.items():
-            shutil.copy(table, f"{outpath}/{sample}/{name}_rollup.tsv")
+            shutil.copy(table, Path(report_path, sample, f'{name}_rollup.tsv'))
 
+    # Counts Tables
+    print("Creating Count Tables")
+    dfCounts = dict()
+    for dbName in ['FOAM', 'KEGG', 'COG', 'CAZy', 'PHROG', 'VOG']:
+        tsv_list = dict()
+        for name in hmm_tsv.keys():
+            table_path = Path(config['DIR_OUT'], STEP[9], name, f'counts_{dbName}.tsv')
+            if table_path.exists():
+                name = re.sub(rf'^FragGeneScan_|prodigal_|Protein_', '', name)
+                tsv_list[name] = table_path
+        combined_path = Path(config['DIR_OUT'], STEP[10], 'combined', f'counts_{dbName}.tsv')
+        metacerberus_parser.merge_tsv(tsv_list, Path(combined_path))
+        if combined_path.exists():
+            dfCounts[dbName] = combined_path
+        del(combined_path)
 
-    # KO Counts Tables
-    print("Creating Count tables")
-    dfCounts = {}
-    for sample,tables in hmmCounts.items():
-        for name,table_path in tables.items():
-            table = pd.read_csv(table_path, sep='\t')
-            X = table[table.Level == 'Function']
-            row = dict(zip(X['Name'].tolist(), X['Count'].tolist()))
-            row = pd.Series(row, name=sample)
-            if name not in dfCounts:
-                dfCounts[name] = pd.DataFrame()
-            dfCounts[name] = pd.concat([dfCounts[name], pd.DataFrame(row).T])
-    table: pd.DataFrame
-    for name,table in dfCounts.items():
-        outfile = os.path.join(outpath, "combined", f"KO_Counts_{name}.tsv")
-        table = table.T.reset_index().rename(columns={'index':'KO'})
-        table.KO = table.KO.apply(lambda x : x[0:6])
-        table.to_csv(outfile, index=False, header=True, sep='\t')
-        dfCounts[name] = outfile
-
-    # HTML of PCA
+    # PCA output (HTML)
     pcaFigures = None
-    if len(hmmCounts) < 4:
-        print("NOTE: PCA Tables and Pathview created only when there are at least four samples.\n")
+    if len(hmm_tsv) < 4:
+        print("NOTE: PCA Tables created only when there are at least four sequence files.\n")
     else:
         print("PCA Analysis")
         pcaFigures = metacerberus_visual.graphPCA(dfCounts)
-        os.makedirs(os.path.join(outpath, "combined"), exist_ok=True)
-        metacerberus_report.write_PCA(os.path.join(outpath, "combined"), pcaFigures)
+        Path(report_path, 'combined').mkdir(parents=True, exist_ok=True)
+        metacerberus_report.write_PCA(os.path.join(report_path, "combined"), pcaFigures)
 
-        # run post processing analysis in R
+    # Run post processing analysis in R
+    if len(hmm_tsv) < 4:
+        print("NOTE: Pathview created only when there are at least four sequence files.\n")
+    else:
         if config['CLASS']:
-            print("\nSTEP 11: Post Analysis with GAGE and PathView")
-            outpathview = os.path.join(outpath, 'combined', 'pathview')
-            os.makedirs(os.path.join(outpathview), exist_ok=True)
-            rscript = os.path.join(outpathview, 'run_pathview.sh')
-            with open(rscript, 'w') as writer:
+            print("\nSTEP 11: Post Analysis with GAGE and Pathview")
+            outpathview = Path(report_path, 'pathview')
+            outpathview.mkdir(exist_ok=True, parents=True)
+            rscript = Path(outpathview, 'run_pathview.sh')
+
+            # Check for internet
+            try:#attempt to open Google
+                request.urlopen('216.58.195.142', timeout=1)
+                is_internet = True
+            except request.URLError as err: 
+                is_internet = False
+            
+            with rscript.open('w') as writer:
                 writer.write(f"#!/bin/bash\n\n")
-                for name,filepath in dfCounts.items():
-                    shutil.copy(filepath, os.path.join(outpathview, f"{name}_counts.tsv"))
-                    shutil.copy(config['CLASS'], os.path.join(outpathview, f"{name}_class.tsv"))
+                for name,countpath in dfCounts.items():
+                    if name not in ['FOAM', 'KEGG']:
+                        continue
+                    shutil.copy(countpath, Path(outpathview, f"{name}_counts.tsv"))
+                    shutil.copy(config['CLASS'], Path(outpathview, f"{name}_class.tsv"))
                     writer.write(f"mkdir -p {name}\n")
                     writer.write(f"cd {name}\n")
                     writer.write(f"pathview-metacerberus.R ../{name}_counts.tsv ../{name}_class.tsv\n")
                     writer.write(f"cd ..\n")
-            for name,filepath in dfCounts.items():
-                os.makedirs(os.path.join(outpathview, name), exist_ok=True)
-                subprocess.run(['pathview-metacerberus.R', filepath, config['CLASS']],
-                                cwd=os.path.join(outpathview, name),
-                                stdout=open(f'{outpathview}/stdout.txt', 'w'),
-                                stderr=open(f'{outpathview}/stderr.txt', 'w')
-                            )
-            print(f"GAGE and Pathview require internet access to run. Run the script '{rscript}'")
+                    outcmd = Path(outpathview, name)
+                    outcmd.mkdir(parents=True, exist_ok=True)
+                    if is_internet:
+                        subprocess.run(['pathview-metacerberus.R', countpath, config['CLASS']],
+                                        cwd=outcmd,
+                                        stdout=Path(outcmd, 'stdout.txt').open('w'),
+                                        stderr=Path(outcmd, 'stderr.txt').open('w')
+                                    )
+            if not is_internet:
+                print(f"GAGE and Pathview require internet access to run. Run the script '{rscript}'")
 
-    # HTML of Figures
-    print("Creating combined HTML Sunburst and Bar Graphs")
+    # Figure outputs (HTML)
+    print("Creating combined sunburst and bargraphs")
     figSunburst = {}
     for key,value in hmmCounts.items():
         figSunburst[key] = metacerberus_visual.graphSunburst(value)
     
     @ray.remote
     def graphCharts(key, rollup, counts):
         return key, metacerberus_visual.graphBarcharts(rollup, counts)
 
     jobCharts = []
     for key,value in hmmRollup.items():
-        jobCharts.append( graphCharts.options(num_cpus=1).remote(key, value, hmmCounts[key]) )
+        jobCharts.append( graphCharts.remote(key, value, hmmCounts[key]) )
     
     figCharts = {}
     while(jobCharts):
         ready,jobCharts = ray.wait(jobCharts)
         if ready:
             key,value = ray.get(ready[0])
             figCharts[key] = value
 
     metacerberus_report.createReport(figSunburst, figCharts, config, STEP[10])
 
-
-    # Wait for misc jobs
-    jobs = jobsQC
-    ready, jobs = ray.wait(jobs, num_returns=len(jobs), timeout=1) # clear buffer
-    while(jobs):
-        print(f"Waiting for {len(jobs)} jobs:", end=' ')
-        ready, jobs = ray.wait(jobs)
-        print(ray.get(ready[0]))
-
-
     # Finished!
     print("\nFinished Pipeline")
-    end = str(datetime.timedelta(seconds=time.time()-startTime)) #end = time.strftime("%H:%M:%S", time.gmtime(time.time()-startTime))
+    end = str(datetime.timedelta(seconds=time.time()-startTime))
     logTime(config["DIR_OUT"], socket.gethostname(), "Total_Time", config["DIR_OUT"], end)
 
     return 0
 
 
 ## Start main method
 if __name__ == "__main__":
```

### Comparing `MetaCerberus-1.0/bin/pathview-metacerberus.R` & `MetaCerberus-1.1/bin/pathview-metacerberus.R`

 * *Files 4% similar despite different names*

```diff
@@ -1,244 +1,249 @@
 #!/usr/bin/env Rscript
 
 # Load libraries
 is_quiet <- TRUE
 
 if (!require("BiocManager", quietly = TRUE)) {
-    install.packages("BiocManager", quiet = TRUE)
-    library(BiocManager)
+  install.packages("BiocManager", quiet = TRUE)
+  library(BiocManager)
 }
 
 if (!require("DESeq2", quietly = TRUE))
-    BiocManager::install("DESeq2", quiet = is_quiet)
+  BiocManager::install("DESeq2", quiet = is_quiet)
 
 if (!require("edgeR", quietly = TRUE))
-    BiocManager::install("edgeR", quiet = is_quiet)
+  BiocManager::install("edgeR", quiet = is_quiet)
 
 if (!require("limma", quietly = TRUE))
-    BiocManager::install("limma", quiet = is_quiet)
+  BiocManager::install("limma", quiet = is_quiet)
 
 if (!require("EnhancedVolcano", quietly = TRUE))
-    BiocManager::install("EnhancedVolcano", quiet = is_quiet)
+  BiocManager::install("EnhancedVolcano", quiet = is_quiet)
 
 if (!require("gage", quietly = TRUE))
-    BiocManager::install("gage", quiet = is_quiet)
+  BiocManager::install("gage", quiet = is_quiet)
 
 if (!require("gageData", quietly=TRUE))
-    BiocManager::install("gageData", quiet = is_quiet)
+  BiocManager::install("gageData", quiet = is_quiet)
 
 if (!require("pathview", quietly = TRUE))
-    BiocManager::install("pathview", quiet = is_quiet)
+  BiocManager::install("pathview", quiet = is_quiet)
 
 
 
 args <- commandArgs(trailingOnly = TRUE)
 
 if (length(args) < 2) {
-    print("Usage: pathview-metacerberus.R <counts.tsv> <class.tsv>")
-    quit()
+  print("Usage: pathview-metacerberus.R <counts.tsv> <class.tsv>")
+  quit()
 }
 
 #' This is the function to run pathway analysis
 #'
 run_path_analysis <- function(lf.c, gsets, ref = ref, samp = samp, compare) {
-    suppressMessages(library(gage, quietly = TRUE))
-    fc.kegg.p <- gage::gage(exprs = lf.c, gsets = gsets, ref = NULL, samp = NULL, compare = compare)
-    return(fc.kegg.p)
+  suppressMessages(library(gage, quietly = TRUE))
+  fc.kegg.p <- gage::gage(exprs = lf.c, gsets = gsets, ref = NULL, samp = NULL, compare = compare)
+  return(fc.kegg.p)
 }
 
 
 #' this is a function to run different diff expression analysis tools
 #'
 rundifftool <- function(diff.tool, gene.data, ref, samp, outname) {
-    grp.idx <- NULL
-    grp.idx[ref] <- "reference"
-    grp.idx[samp] <- "sample"
-
-    suppressMessages(library(EnhancedVolcano, quietly = TRUE))
-
-    if (diff.tool == "deseq2") {
-        suppressMessages(library(DESeq2, quietly = TRUE))
-        coldat <- DataFrame(grp = factor(grp.idx))
-
-        print("Deseq2 is running")
-        dds <- DESeq2::DESeqDataSetFromMatrix(gene.data, colData = coldat, design = ~grp)
-        dds <- DESeq2::DESeq(dds)
-        deseq2.res <- results(dds)
-        # direction of fc, depends on levels(coldat$grp), the first level
-        # taken as reference (or control) and the second one as experiment.
-        deseq2.fc <- deseq2.res$log2FoldChange
-        names(deseq2.fc) <- rownames(deseq2.res)
-        exp.fc <- deseq2.fc
-        #pdf("Volcano_deseq2.pdf", width = 14,height= 14)
-        jpeg("Volcano_deseq2.jpg", units = "in", width = 15, height = 15, res = 300)
-        plot(EnhancedVolcano::EnhancedVolcano(deseq2.res, x = "log2FoldChange", y = "pvalue",
-                lab = rownames(deseq2.res)))
-        #plot(x = 1:10, y = 1:10)
-        dev.off()
-    }
-    else if (diff.tool == "edgeR") {
-        suppressMessages(library(edgeR, quietly = TRUE))
-        dgel <- edgeR::DGEList(counts = gene.data, group = factor(grp.idx))
-        dgel <- edgeR::calcNormFactors(dgel)
-        dgel <- edgeR::estimateCommonDisp(dgel)
-        dgel <- edgeR::estimateTagwiseDisp(dgel)
-        et <- edgeR::exactTest(dgel)
-        edger.fc <- et$table$logFC
-        names(edger.fc) <- rownames(et$table)
-        exp.fc <- edger.fc
-        jpeg("Volcano_edgeR.jpg", units = "in", width = 15, height = 15, res = 300)
-        plot(EnhancedVolcano::EnhancedVolcano(et$table, x = "logFC", y = "PValue", lab = rownames(et$table)))
-        dev.off()
-    }
-    else if (diff.tool == "limma") {
-        suppressMessages(library(limma, quietly = TRUE))
-        dgel2 <- edgeR::DGEList(counts = gene.data, group = factor(grp.idx))
-        dgel2 <- edgeR::calcNormFactors(dgel2)
-        design <- limma::model.matrix(~grp.idx)
-        log2.cpm <- limma::voom(dgel2, design)
-        fit <- limma::lmFit(log2.cpm, design)
-        fit <- limma::eBayes(fit)
-        limma.res <- limma::topTable(fit, coef = 2, n = Inf, sort = "p")
-        limma.fc <- limma.res$logFC
-
-        names(limma.fc) <- limma.res$ID
-        exp.fc <- limma.fc
-    }
-    else {
-        print("The diff tool is not avaliable")
-    }
-    return(exp.fc)
+  grp.idx <- NULL
+  grp.idx[ref] <- "reference"
+  grp.idx[samp] <- "sample"
+  
+  suppressMessages(library(EnhancedVolcano, quietly = TRUE))
+  
+  if (diff.tool == "deseq2") {
+    suppressMessages(library(DESeq2, quietly = TRUE))
+    coldat <- DataFrame(grp = factor(grp.idx))
+    
+    print("Deseq2 is running")
+    dds <- DESeq2::DESeqDataSetFromMatrix(gene.data, colData = coldat, design = ~grp)
+    dds <- estimateSizeFactors(dds)
+    # dds <- estimateDispersions(dds)
+    
+    dds <- estimateDispersionsGeneEst(dds)
+    dispersions(dds) <- mcols(dds)$dispGeneEst
+    dds <-  nbinomWaldTest(dds)
+    #dds <- DESeq2::DESeq(dds)
+    deseq2.res <- results(dds)
+    # direction of fc, depends on levels(coldat$grp), the first level
+    # taken as reference (or control) and the second one as experiment.
+    deseq2.fc <- deseq2.res$log2FoldChange
+    names(deseq2.fc) <- rownames(deseq2.res)
+    exp.fc <- deseq2.fc
+    #pdf("Volcano_deseq2.pdf", width = 14,height= 14)
+    jpeg("Volcano_deseq2.jpg", units = "in", width = 15, height = 15, res = 300)
+    plot(EnhancedVolcano::EnhancedVolcano(deseq2.res, x = "log2FoldChange", y = "pvalue",
+                                          lab = rownames(deseq2.res)))
+    #plot(x = 1:10, y = 1:10)
+    dev.off()
+  }
+  else if (diff.tool == "edgeR") {
+    suppressMessages(library(edgeR, quietly = TRUE))
+    dgel <- edgeR::DGEList(counts = gene.data, group = factor(grp.idx))
+    dgel <- edgeR::calcNormFactors(dgel)
+    dgel <- edgeR::estimateCommonDisp(dgel)
+    dgel <- edgeR::estimateTagwiseDisp(dgel)
+    et <- edgeR::exactTest(dgel)
+    edger.fc <- et$table$logFC
+    names(edger.fc) <- rownames(et$table)
+    exp.fc <- edger.fc
+    jpeg("Volcano_edgeR.jpg", units = "in", width = 15, height = 15, res = 300)
+    plot(EnhancedVolcano::EnhancedVolcano(et$table, x = "logFC", y = "PValue", lab = rownames(et$table)))
+    dev.off()
+  }
+  else if (diff.tool == "limma") {
+    suppressMessages(library(limma, quietly = TRUE))
+    dgel2 <- edgeR::DGEList(counts = gene.data, group = factor(grp.idx))
+    dgel2 <- edgeR::calcNormFactors(dgel2)
+    design <- limma::model.matrix(~grp.idx)
+    log2.cpm <- limma::voom(dgel2, design)
+    fit <- limma::lmFit(log2.cpm, design)
+    fit <- limma::eBayes(fit)
+    limma.res <- limma::topTable(fit, coef = 2, n = Inf, sort = "p")
+    limma.fc <- limma.res$logFC
+    
+    names(limma.fc) <- limma.res$ID
+    exp.fc <- limma.fc
+  }
+  else {
+    print("The diff tool is not avaliable")
+  }
+  return(exp.fc)
 }
 
 
 #' this is a function to run pathview.2 function
 #'
 pathview.2 <- function(run, diff.tool, gene.data, ref, samp, outname, gsets, compare,
-                        both.dirs = list(gene = T, cpd = T), pathway.id = NULL, species, plot.gene.data = T) {
-
-    if (is.null(pathway.id) == FALSE) {
-        pathview::pathview(gene.data = gene.data, pathway.id = pathway.id, out.suffix = outname, plot.gene.data)
+                       both.dirs = list(gene = T, cpd = T), pathway.id = NULL, species, plot.gene.data = T) {
+  
+  if (is.null(pathway.id) == FALSE) {
+    pathview::pathview(gene.data = gene.data, pathway.id = pathway.id, out.suffix = outname, plot.gene.data)
+  }
+  else {
+    if (run == "complete") {
+      logfoldchange <- rundifftool(diff.tool, gene.data, ref, samp, outname)
+      print("diff tool run successful")
+      fc.kegg.p <- run_path_analysis(logfoldchange, gsets, ref = NULL, samp = NULL, compare = compare)
+      #, gene.data = gene.data, ref, samp, plot.gene.data = T )
+      print("gage run successful")
+      
+      print("now pathview")
+      path.ids.2 <- rownames(fc.kegg.p$greater)[fc.kegg.p$greater[, "q.val"] < 0.1 &
+                                                  + !is.na(fc.kegg.p$greater[, "q.val"])]
+      
+      if (length(fc.kegg.p) > 2) {
+        print(length(fc.kegg.p))
+        path.ids.l <- rownames(fc.kegg.p$less)[
+          fc.kegg.p$less[, "q.val"] < 0.1 & + !is.na(fc.kegg.p$less[, "q.val"])]
+        path.ids.2 <- c(path.ids.2[1:3], path.ids.l[1:3])
+        path.ids.2 <- gsub("[^0-9.-]", "", sapply(stringr::str_split(path.ids.2, " ", 2), "[[", 1))
+      }
+      print(c("Visualize Pathway", na.omit(path.ids.2[1:6])))
+      for (pid in na.omit(path.ids.2[1:6])) {
+        print(c("Processing", paste0('k', pid)))
+        tryCatch(
+          expr = {
+            pathview::pathview(
+              gene.data = logfoldchange,
+              pathway.id = pid,
+              species = species,
+              out.suffix = diff.tool,
+              plot.gene.data = T
+              #kegg.native = T,
+            )
+          },
+          error = function(e) {
+            print(c("ERROR: Pathview failed on", pid))
+          }
+        )
+      }
+      print("Finished Pathview")
     }
     else {
-        if (run == "complete") {
-            logfoldchange <- rundifftool(diff.tool, gene.data, ref, samp, outname)
-            print("diff tool run successful")
-            fc.kegg.p <- run_path_analysis(logfoldchange, gsets, ref = NULL, samp = NULL, compare = compare)
-                                            #, gene.data = gene.data, ref, samp, plot.gene.data = T )
-            print("gage run successful")
-
-            print("now pathview")
-            path.ids.2 <- rownames(fc.kegg.p$greater)[fc.kegg.p$greater[, "q.val"] < 0.1 &
-                                    + !is.na(fc.kegg.p$greater[, "q.val"])]
-
-            if (length(fc.kegg.p) > 2) {
-                print(length(fc.kegg.p))
-                path.ids.l <- rownames(fc.kegg.p$less)[
-                                            fc.kegg.p$less[, "q.val"] < 0.1 & + !is.na(fc.kegg.p$less[, "q.val"])]
-                path.ids.2 <- c(path.ids.2[1:3], path.ids.l[1:3])
-                path.ids.2 <- gsub("[^0-9.-]", "", sapply(stringr::str_split(path.ids.2, " ", 2), "[[", 1))
-            }
-            print(c("Visualize Pathway", na.omit(path.ids.2[1:6])))
-            for (pid in na.omit(path.ids.2[1:6])) {
-                print(c("Processing", paste0('k', pid)))
-                tryCatch(
-                    expr = {
-                        pathview::pathview(
-                            gene.data = logfoldchange,
-                            pathway.id = pid,
-                            species = species,
-                            out.suffix = diff.tool,
-                            plot.gene.data = T
-                            #kegg.native = T,
-                                    )
-                    },
-                    error = function(e) {
-                        print(c("ERROR: Pathview failed on", pid))
-                    }
-                )
-            }
-            print("Finished Pathview")
-        }
-        else {
-            fc.kegg.p <- run_path_analysis(gene.data, gsets, ref = ref, samp = samp, compare = compare)
-            #, gene.data = gene.data, ref, samp, plot.gene.data = T  )
-            print("now pathview")
-            path.ids.2 <- rownames(fc.kegg.p$greater)[fc.kegg.p$greater[, "q.val"] < 0.1 &
-                                + !is.na(fc.kegg.p$greater[, "q.val"])]
-
-            if (length(fc.kegg.p) > 2) {
-                path.ids.l <- rownames(fc.kegg.p$less)[fc.kegg.p$less[, "q.val"] < 0.1 &
-                                                        + !is.na(fc.kegg.p$less[, "q.val"])]
-                path.ids.2 <- c(path.ids.2[1:3], path.ids.l[1:3])
-                path.ids.2 <- gsub("[^0-9.-]", "", sapply(stringr::str_split(path.ids.2, " ", 2), "[[", 1))
-
-                #visualize pathway
-                pv.out.list <- sapply(na.omit(path.ids.2[1:6]), function(pid) pathview::pathview(gene.data =  gene.data,
-                                        pathway.id = pid, out.suffix = diff.tool, species, plot.gene.data = T))
-            }
-        }
+      fc.kegg.p <- run_path_analysis(gene.data, gsets, ref = ref, samp = samp, compare = compare)
+      #, gene.data = gene.data, ref, samp, plot.gene.data = T  )
+      print("now pathview")
+      path.ids.2 <- rownames(fc.kegg.p$greater)[fc.kegg.p$greater[, "q.val"] < 0.1 &
+                                                  + !is.na(fc.kegg.p$greater[, "q.val"])]
+      
+      if (length(fc.kegg.p) > 2) {
+        path.ids.l <- rownames(fc.kegg.p$less)[fc.kegg.p$less[, "q.val"] < 0.1 &
+                                                 + !is.na(fc.kegg.p$less[, "q.val"])]
+        path.ids.2 <- c(path.ids.2[1:3], path.ids.l[1:3])
+        path.ids.2 <- gsub("[^0-9.-]", "", sapply(stringr::str_split(path.ids.2, " ", 2), "[[", 1))
+        
+        #visualize pathway
+        pv.out.list <- sapply(na.omit(path.ids.2[1:6]), function(pid) pathview::pathview(gene.data =  gene.data,
+                                                                                         pathway.id = pid, out.suffix = diff.tool, species, plot.gene.data = T))
+      }
     }
-
-    suppressMessages(library(plotly, quietly = TRUE))
-
-    print("Plotting Pathview Data")
-    if (plot.gene.data == T) { #& is.null(pathway.id))  ) {
-        gs <- unique(unlist(gsets[rownames(fc.kegg.p$greater)[1:3]]))
-        essData <- gage::essGene(gs, gene.data, ref = ref, samp = samp, compare = compare)
-        for (gs in rownames(fc.kegg.p$greater)[1:3]) {
-            outname <- paste(gsub(" |:|/", "_", substr(gs, 9, 100)), "greater", sep="_")
-            gage::geneData(genes = gsets[[gs]], exprs = essData, ref = ref,
-                samp = samp, outname = outname, txt = T, heatmap = T,
-                Colv = F, Rowv = F, dendrogram = "none", limit = 3, scatterplot = T, pdf.size = c(7, 7))
-        }
-        #print("PLOTTING HEATMAPS PLOTLY")
-        #print(getwd())
-        #for (file_tsv in list.files(pattern = "\\.txt$", ignore.case = TRUE)) {
-        #    file_name = basename(file_tsv)
-        #    file_tsv <- read.csv(file_tsv, sep = '\t', stringsAsFactors = TRUE)
-        #    p <- ggplot(file_tsv,
-        #                x = "Samples",
-        #                y = "KO IDs",
-        #                fill = "KO Pathway\nRegulation")
-        #    pltHeatmap <- plotly::ggplotly(p)
-        #    print(paste0("SAVING: ", file_name, ".html"))
-        #    htmlwidgets::saveWidget(pltHeatmap, paste0(file_name, ".html"))
-        #}
-
-        if (length(fc.kegg.p) > 2) {
-            gs <- unique(unlist(gsets[rownames(fc.kegg.p$lesser)[1:3]]))
-            essData <- gage::essGene(gs, gene.data, ref = ref, samp = samp, compare = compare)
-            for (gs in rownames(fc.kegg.p$lesser)[1:3]) {
-                outname <- paste(gsub(" |:|/", "_", substr(gs, 10, 100)), "lesser", sep="_")
-                gage::geneData(genes = gsets[[gs]], exprs = essData, ref = ref,
-                    samp = samp, outname = outname, txt = T, heatmap = T,
-                    Colv = F, Rowv = F, dendrogram = "none", limit = 3, scatterplot = T, pdf.size = c(7, 7))
-            }
-        }
+  }
+  
+  suppressMessages(library(plotly, quietly = TRUE))
+  
+  print("Plotting Pathview Data")
+  if (plot.gene.data == T) { #& is.null(pathway.id))  ) {
+    gs <- unique(unlist(gsets[rownames(fc.kegg.p$greater)[1:3]]))
+    essData <- gage::essGene(gs, gene.data, ref = ref, samp = samp, compare = compare)
+    for (gs in rownames(fc.kegg.p$greater)[1:3]) {
+      outname <- paste(gsub(" |:|/", "_", substr(gs, 9, 100)), "greater", sep="_")
+      gage::geneData(genes = gsets[[gs]], exprs = essData, ref = ref,
+                     samp = samp, outname = outname, txt = T, heatmap = T,
+                     Colv = F, Rowv = F, dendrogram = "none", limit = 3, scatterplot = T, pdf.size = c(7, 7))
+    }
+    #print("PLOTTING HEATMAPS PLOTLY")
+    #print(getwd())
+    #for (file_tsv in list.files(pattern = "\\.txt$", ignore.case = TRUE)) {
+    #    file_name = basename(file_tsv)
+    #    file_tsv <- read.csv(file_tsv, sep = '\t', stringsAsFactors = TRUE)
+    #    p <- ggplot(file_tsv,
+    #                x = "Samples",
+    #                y = "KO IDs",
+    #                fill = "KO Pathway\nRegulation")
+    #    pltHeatmap <- plotly::ggplotly(p)
+    #    print(paste0("SAVING: ", file_name, ".html"))
+    #    htmlwidgets::saveWidget(pltHeatmap, paste0(file_name, ".html"))
+    #}
+    
+    if (length(fc.kegg.p) > 2) {
+      gs <- unique(unlist(gsets[rownames(fc.kegg.p$lesser)[1:3]]))
+      essData <- gage::essGene(gs, gene.data, ref = ref, samp = samp, compare = compare)
+      for (gs in rownames(fc.kegg.p$lesser)[1:3]) {
+        outname <- paste(gsub(" |:|/", "_", substr(gs, 10, 100)), "lesser", sep="_")
+        gage::geneData(genes = gsets[[gs]], exprs = essData, ref = ref,
+                       samp = samp, outname = outname, txt = T, heatmap = T,
+                       Colv = F, Rowv = F, dendrogram = "none", limit = 3, scatterplot = T, pdf.size = c(7, 7))
+      }
     }
+  }
 }
 
 
 library(stringr, quietly = TRUE)
 library(gage, quietly = TRUE)
 library(pathview, quietly = TRUE)
 #source("pathview.2.R")
 
 print("Loading Data")
 #options(stringsAsFactors = TRUE) #TODO: DEPRECATED
 
-gene_data <- read.table(file = args[1], sep = "\t", header  = T, quote = "", row.names = 1, stringsAsFactors = TRUE)
-colnames(gene_data) <- sapply(str_split(colnames(gene_data), "_", n = 2), "[[", 2)
+gene_data <- read.table(file =args[1], sep = "\t", header  = T, quote = "", row.names = 1, stringsAsFactors = TRUE)
 coldata <- read.table(args[2], sep = "\t", header = T, row.names = 1, stringsAsFactors = TRUE)
 
 print("Levels")
 levels(coldata[, 1])[1]
 print("Coldata")
-print(coldata)
+print(head(coldata))
 reference_indx <- which(coldata[, 1] ==  levels(coldata[, 1])[1])
 samp_indx <- which(coldata[, 1] ==  levels(coldata[, 1])[2])
 print("the treatment and reference are ")
 print("Sample Index")
 samp_indx
 print("Reference Index")
 reference_indx
@@ -258,35 +263,35 @@
 all(rownames(coldata) == colnames(gene.data))
 
 print("Running pathview")
 
 dir.create("deseq2", showWarnings = FALSE)
 setwd("deseq2")
 pathview.2(run = "complete",
-    both.dirs = list(gene = T, cpd = T),
-    diff.tool = "deseq2",
-    gene.data = gene.data,
-    ref = reference_indx,
-    samp = samp_indx,
-    pathway.id = NULL,
-    gsets = kegg.gs,
-    plot.gene.data = T,
-    outname = outname,
-    compare = "unpaired",
-    species = "ko")
+           both.dirs = list(gene = T, cpd = T),
+           diff.tool = "deseq2",
+           gene.data = gene.data,
+           ref = reference_indx,
+           samp = samp_indx,
+           pathway.id = NULL,
+           gsets = kegg.gs,
+           plot.gene.data = T,
+           outname = outname,
+           compare = "unpaired",
+           species = "ko")
 setwd("..")
 
 dir.create("edgeR", showWarnings = FALSE)
 setwd("edgeR")
 pathview.2(run = "complete",
-    both.dirs = list(gene = T, cpd = T),
-    diff.tool = "edgeR",
-    gene.data= gene.data,
-    ref = reference_indx,
-    samp=samp_indx,
-    pathway.id = NULL,
-    gsets = kegg.gs,
-    plot.gene.data = T,
-    outname = outname,
-    compare = "unpaired",
-    species = "ko")
+           both.dirs = list(gene = T, cpd = T),
+           diff.tool = "edgeR",
+           gene.data= gene.data,
+           ref = reference_indx,
+           samp=samp_indx,
+           pathway.id = NULL,
+           gsets = kegg.gs,
+           plot.gene.data = T,
+           outname = outname,
+           compare = "unpaired",
+           species = "ko")
 setwd("..")
```

### Comparing `MetaCerberus-1.0/bin/ray-slurm-metacerberus.sh` & `MetaCerberus-1.1/bin/ray-slurm-metacerberus.sh`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/Chunker.py` & `MetaCerberus-1.1/lib/Chunker.py`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/dependency_files/PacBio_quality-control.fna` & `MetaCerberus-1.1/lib/dependency_files/PacBio_quality-control.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/dependency_files/adapters.fna` & `MetaCerberus-1.1/lib/dependency_files/adapters.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/dependency_files/lambda-phage.fna` & `MetaCerberus-1.1/lib/dependency_files/lambda-phage.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/dependency_files/phix174_ill.ref.fna` & `MetaCerberus-1.1/lib/dependency_files/phix174_ill.ref.fna`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_10` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_30` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_30`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/454_5` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/454_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/complete` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/complete`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/gene` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/gene`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_1` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_10` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/illumina_5` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/illumina_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/noncoding` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/noncoding`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/pwm` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/pwm`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/rgene` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/rgene`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/sanger_10` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/sanger_10`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/sanger_5` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/sanger_5`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/start` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/start`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/start1` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/start1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/stop` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/stop`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/fraggenescanplus_dependences/stop1` & `MetaCerberus-1.1/lib/fraggenescanplus_dependences/stop1`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/metacerberus.config` & `MetaCerberus-1.1/lib/metacerberus.config`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/metacerberus_decon.py` & `MetaCerberus-1.1/lib/metacerberus_decon.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # -*- coding: utf-8 -*-
 """metacerberus_decon.py: Module to clean trimmed .fastq files
 Uses bbduk [https://sourceforge.net/projects/bbmap/]
 """
 
 import os
+from pathlib import Path
 import subprocess
 
 
-## deconSingleReads
-#
+# Decontaminate single end reads
 def deconSingleReads(key_value, config, subdir):
-    # TODO: Find good long read mapper
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)
+    path = Path(config['DIR_OUT'], subdir)
 
     key = key_value[0]
     value = key_value[1]
 
-    deconReads = os.path.join(path, f"decon-{key}.fastq")
-    matched = os.path.join(path, "matched_"+key)
-    stats = os.path.join(path, "stats.txt")
+    deconReads = path / f"decon-{key}.fastq"
+    matched = path / f"matched_{key}"
+    stats = path / "stats.txt"
+
+    done = path / "complete"
+    if not config['REPLACE'] and done.exists() and deconReads.exists():
+        return deconReads
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
-    refseq = "ref="+config['REFSEQ'] if config['REFSEQ'] else ""
+    qc_seq = "ref="+config['QC_SEQ'] if config['QC_SEQ'] else ""
 
-    command = f"{config['EXE_BBDUK']} -Xmx1g in={value} out={deconReads} qin=33 qtrim=r minlen=50 outm={matched} {refseq} k=31 stats={stats}"
+    command = f"{config['EXE_BBDUK']} -Xmx1g in={value} out={deconReads} qin=30 qtrim=r minlen=50 outm={matched} {qc_seq} k=31 stats={stats}"
     try:
         with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
         print("ERROR: Failed to execute:\n", command)
 
+    done.touch()
     return deconReads
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_formatFasta.py` & `MetaCerberus-1.1/lib/metacerberus_formatFasta.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 # -*- coding: utf-8 -*-
 """metacerberus_formatFasta.py: Module for reformating FASTQ files to FASTA files
 Also removes N's from scaffolds
 """
 
 import os
+from pathlib import Path
 import re
 import subprocess
 import textwrap
 
 
-## format_fastq
+# Remove quality from fastq
 def reformat(fastq, config, subdir):
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)    
+    path = Path(config['DIR_OUT'], subdir)
 
-    fasta, ext = os.path.splitext(fastq)
-    fasta = os.path.basename(fasta) + ".fna"
-    fasta = os.path.join(path, fasta)
+    fasta = path / Path(fastq).with_suffix(".fna")
+
+    done = Path(path, 'complete')
+    if not config['REPLACE'] and done.exists() and fasta.exists():
+        return fasta
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
     if not config['REPLACE'] and os.path.exists(fasta):
         return fasta
 
     command = "sed -n '1~4s/^@/>/p;2~4p' " +fastq+ " > " +fasta
     subprocess.call(command, shell=True)
+
+    done.touch()
     return fasta
 
 
+# Helper for removeN
 def split_sequenceN(name, sequence):
     N_lengths = []
     regex = re.compile(r"(N+)")
     for match in regex.finditer(sequence):
         N_lengths.append(len(match.group(1)))
     sequences = regex.sub('\n', sequence).split('\n')
     name = name.split()
@@ -42,27 +49,33 @@
         seqs += textwrap.wrap(seq, 80)
     
     return seqs, N_lengths
 
 
 # Remove N's
 def removeN(fasta:str, config:dict, subdir:os.PathLike):
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)    
+    path = Path(config['DIR_OUT'], subdir)
 
     outFasta, ext = os.path.splitext(fasta)
     outFasta = os.path.basename(outFasta) + "_clean"+ ext
-    outFasta = os.path.join(path, outFasta)
+    outFasta = Path(path, outFasta)
+
+    done = Path(path, 'complete')
+    if not config['REPLACE'] and done.exists() and outFasta.exists():
+        return outFasta, None
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
     proc = subprocess.run(['grep', '-cE', '^[^>].*N', fasta], stdout=subprocess.PIPE, text=True)
     res = int(proc.stdout.strip())
     if res == 0:
+        done.touch()
         return fasta, None
 
-    with open(fasta) as reader, open(outFasta, 'w') as writer:
+    with open(fasta) as reader, outFasta.open('w') as writer:
         NStats = dict()
         line = reader.readline()
         while line:
             line = line.strip()
             if line.startswith('>'):
                 name = line[1:]
                 sequence = ""
@@ -79,8 +92,9 @@
                     print('\n'.join(sequences), file=writer)
                 else:
                     print('>', name, sep='', file=writer)
                     print('\n'.join(textwrap.wrap(sequence, 80)), file=writer)
                 continue #already got next line, next item in loop
             line = reader.readline()
 
+    done.touch()
     return outFasta, NStats
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_logo.jpg` & `MetaCerberus-1.1/lib/metacerberus_logo.jpg`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/metacerberus_merge.py` & `MetaCerberus-1.1/lib/metacerberus_merge.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 # -*- coding: utf-8 -*-
 """metacerberus_merge.py: Module to merge paired end .fastq files
 Uses flash [https://github.com/dstreett/FLASH2]
 """
 
 import os
+from pathlib import Path
 import subprocess
 
 
-## mergePairedEnd
-#
+# Merge paired end reads
 def mergePairedEnd(pairedFastq, config, subdir):
-    # TODO: Find good long read mapper
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)
+    path = Path(config['DIR_OUT'], subdir)
 
     R1 = pairedFastq[0]
     R2 = pairedFastq[1]
-
     prefix = os.path.basename(R1)
+    merged = os.path.join(path, prefix.replace('_R1', '_merged'))
+    merged = path / prefix.replace('_R1', '_merged')
+
+    done = path / "complete"
+    if not config['REPLACE'] and done.exists() and merged.exists():
+        return merged
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
     command = f"{config['EXE_FLASH']} {R1} {R2} -d {path} -o {prefix} -M 150"
     with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
         subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
 
-    merged = os.path.join(path, prefix.replace('_R1', '_merged'))
-    if os.path.exists(merged):
-        os.remove(merged)
     command = f"cat {path}/*.fastq > {merged}"
     subprocess.run(command, shell=True, check=True)
 
+    done.touch()
     return merged
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_parser.py` & `MetaCerberus-1.1/lib/metacereberus_parser_wPl.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,65 +8,59 @@
 def warn(*args, **kwargs):
     #print("args", str(args))
     pass
 import warnings
 warnings.warn = warn
 
 import os
-import pandas as pd
-
+import polars as pl
+from pathlib import Path
 
 def parseHmmer(hmm_tsv, config, subdir):
     path = os.path.join(config['DIR_OUT'], subdir)
     os.makedirs(path, exist_ok=True)
 
     minscore = config["MINSCORE"]
 
     top5File = os.path.join(path, "HMMER_top_5.tsv")
-    rollupFileFOAM = os.path.join(path, "HMMER_BH_FOAM.rollup")
-    rollupFileKEGG = os.path.join(path, "HMMER_BH_KO.rollup")
 
     # Calculate Best Hit
     BH_dict = {}
     BH_top5 = {}
-    #"target", "query", "e-value", "score"
-    with open(hmm_tsv, "r") as reader:
-        for line in reader:
-            line = line.split('\t')
-            try:
-                query = line[1]
-                line[3] = float(line[3])
-                score = line[3]
-            except:
-                continue
-            if score < minscore:            # Skip scores less than minscore
-                print("DEBUG: MINSCORE DETECTED")
-                continue
 
-            # store top 5 per query
-            if query not in BH_top5:
-                BH_top5[query] = [line]
-            elif len(BH_top5[query]) < 5:
-                BH_top5[query].append(line)
-            else:
-                BH_top5[query].sort(key = lambda x: x[3], reverse=False)
-                if score > float(BH_top5[query][0][3]):
-                    BH_top5[query][0] = line
-
-            # Check for Best Score per query
-            if query not in BH_dict:
-                BH_dict[query] = line
-            elif score > float(BH_dict[query][3]):
-                BH_dict[query] = line
+    # read input file
+    df = pl.read_csv(hmm_tsv, delimiter='\t', header=None, columns=["target", "query", "e-value", "score"])
+
+    # skip scores less than minscore
+    df = df[df['score'] >= minscore]
+
+    # store top 5 per query
+    groups = df.groupby('query')
+    for group in groups:
+        query = group['query'][0]
+        group = group.sort('score', reverse=True)
+        if len(group) < 5:
+            BH_top5[query] = group.to_list()
+        else:
+            BH_top5[query] = group[:5].to_list()
+
+    # Check for Best Score per query
+    groups = df.groupby('query')
+    for group in groups:
+        query = group['query'][0]
+        group = group.sort('score', reverse=True)
+        if query not in BH_dict:
+            BH_dict[query] = group[0].to_list()
+        elif group['score'][0] > BH_dict[query][3]:
+            BH_dict[query] = group[0].to_list()
 
     # Save Top 5 hits tsv rollup
     with open(top5File, 'w') as writer:
         print("Target Name", "KO ID", "EC value", "E-Value (sequence)", "Score (domain)", file=writer, sep='\t')
         for query in sorted(BH_top5.keys()):
-            BH_top5[query].sort(key = lambda x: x[3], reverse=True)
             for line in BH_top5[query]:
                 ko = []
                 ec = []
                 for id in line[1].split(','):
                     if "KO:" in id:
                         id = id.split(':')[1].split('_')
                         ko += [id[0]]
@@ -80,62 +74,69 @@
         KO_IDs = [KO_ID.split(":")[1].split("_")[0] for KO_ID in line[1].split(",") if "KO:" in KO_ID]
         for KO_ID in KO_IDs:
             if KO_ID not in KO_ID_counts:
                 KO_ID_counts[KO_ID] = 0
             KO_ID_counts[KO_ID] += 1
 
     # Write rollup files to disk
-    dfRollup = dict()
-
-    dbPath = os.path.join(config['PATHDB'], "FOAM-onto_rel1.tsv")
-    dfRollup['FOAM'] = rollup(KO_ID_counts, dbPath, path)
-
-    dbPath = os.path.join(config['PATHDB'], "KEGG-onto_rel1.tsv")
-    dfRollup['KEGG'] = rollup(KO_ID_counts, dbPath, path)
-
-    for name,df in dfRollup.items():
-        outfile = os.path.join(path, "HMMER_BH_"+name+"_rollup.tsv")
-        df.to_csv(outfile, index=False, header=True, sep='\t')
-        dfRollup[name] = outfile
-
-    return dfRollup
+def write_rollup_files(KO_ID_counts, path, config):
+    rollup_file = dict()
+    dbPaths = [
+        os.path.join(config['PATHDB'], "FOAM-onto_rel1.tsv"),
+        os.path.join(config['PATHDB'], "KEGG-onto_rel1.tsv")]
+    for dbPath in dbPaths:
+        dfRollup = pl.read_csv(dbPath, sep='\t')
+        dfRollup = rollup(KO_ID_counts, dfRollup, path)
+        outfile = os.path.join(path, f"HMMER_BH_{os.path.basename(dbPath).split('-')[0]}_rollup.tsv")
+        dfRollup.to_csv(outfile, delimiter='\t', header=True, index=False)
+        rollup_file[os.path.basename(dbPath).split('-')[0]] = outfile
 
+    return rollup_file
 
 ######### Roll-Up #########
 def rollup(KO_COUNTS: dict, lookupFile: str, outpath: str):
-    dfLookup = pd.read_csv(lookupFile, sep='\t')
-    dfRollup = pd.DataFrame()
+    dfLookup = pl.read_csv(lookupFile, delimiter='\t')
+    dfRollup = pl.DataFrame()
 
-    errfile = os.path.join( outpath, os.path.basename(lookupFile)+'.err' )
+    errfile = os.path.join(outpath, os.path.basename(lookupFile) + '.err')
     with open(errfile, 'w') as errlog:
-        for KO_ID,count in KO_COUNTS.items():
-            rows = pd.DataFrame(dfLookup[dfLookup.KO==KO_ID]).fillna('')
-            if rows.empty:
+        for KO_ID, count in KO_COUNTS.items():
+            rows = dfLookup[dfLookup['KO'] == KO_ID].fillna('')
+            if rows.shape[0] == 0:
                 print("WARNING:'", KO_ID, "'not found in the Lookup File", file=errlog)
                 continue
-            rows.drop(rows[rows['Function']==''].index, inplace=True)
-            if rows.empty:
+            rows = rows.drop(rows[rows['Function'] == ''].index)
+            if rows.shape[0] == 0:
                 print("WARNING:'", KO_ID, "'Does not have a 'Function' in the Lookup File", file=errlog)
                 continue
             rows['Count'] = count
-            dfRollup = pd.concat([dfRollup,rows])
-    #dfRollup.reset_index(inplace=True)
+            dfRollup = pl.concat([dfRollup, rows])
 
+    dfRollup.to_csv(outpath, delimiter='\t', index=False)
     return dfRollup
 
-
 ########## Counts Table #########
-def createCountTables(rollup_files:dict, config:dict, subdir: str):
+def createCountTables(rollup_files: dict, config: dict, subdir: str):
+    done = os.path.join(config['DIR_OUT'], subdir, "complete")
     dfCounts = dict()
-    for dbName,filepath in rollup_files.items():
+    print("createCountTables:", subdir)
+    for dbName, filepath in rollup_files.items():
+        outpath = os.path.join(config['DIR_OUT'], subdir, f"{dbName}_counts.tsv")
+        if not config['REPLACE'] and os.path.exists(done):
+            dfCounts[dbName] = outpath
+            continue
+
         print("Loading Count Tables:", dbName, filepath)
-        df = pd.read_csv(filepath, sep='\t')
+        try:
+            df = pl.read_csv(filepath, delimiter='\t')
+        except:
+            continue
         dictCount = {}
-        for i,row in df.iterrows():
-            for colName,colData in row.iteritems():
+        for i, row in df.iterrows():
+            for colName, colData in row.items():
                 if not colName.startswith('L'):
                     continue
                 level = colName[1]
                 name = colData
                 if name:
                     name = f"lvl{level}: {name}"
                     if name not in dictCount:
@@ -145,19 +146,19 @@
             if not name:
                 continue
             name = f"{row.KO}: {name}"
             if name not in dictCount:
                 dictCount[name] = ['Function', 0, row.KO]
             dictCount[name][1] += row['Count']
         data = {
-        'KO Id':[x[2] for x in dictCount.values()],
-        'Name':list(dictCount.keys()),
-        'Level':[x[0] for x in dictCount.values()],
-        'Count':[x[1] for x in dictCount.values()]}
-
-        outpath = os.path.join(config['DIR_OUT'], subdir, f"{dbName}_counts.tsv")
-        df = pd.DataFrame(data=data)
-        df.fillna(0, inplace=True)
-        df.to_csv(outpath, index=False, header=True, sep='\t')
+            'KO Id': [x[2] for x in dictCount.values()],
+            'Name': list(dictCount.keys()),
+            'Level': [x[0] for x in dictCount.values()],
+            'Count': [x[1] for x in dictCount.values()]}
+
+        df = pl.DataFrame(data=data)
+        df.fill_null(0, inplace=True)
+        df.to_csv(outpath, index=False, header=True, delimiter='\t')
         dfCounts[dbName] = outpath
 
+    pl.Path(done).touch()
     return dfCounts
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_qc.py` & `MetaCerberus-1.1/lib/metacerberus_qc.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 Uses FastQC [https://www.bioinformatics.babraham.ac.uk/projects/fastqc/]
 """
 
 import os
 import subprocess
 
 
-## checkQuality
-#
+## Check quality
 def checkQuality(rawRead, config, subdir):
     if type(rawRead) is str:
         return checkSingleRead(rawRead, config, subdir)
     else:
         return checkPairedRead(rawRead, config, subdir)
 
 
-## checkSingleQuality
-#
+# Check single end quality
 def checkSingleRead(singleRead, config, subdir):
     path = f"{config['DIR_OUT']}/{subdir}"
     os.makedirs(path, exist_ok=True)
     
     command = f"{config['EXE_FASTQC']} -o {path} {singleRead}"
     try:
         with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
@@ -29,16 +27,15 @@
         return os.path.join(path, os.path.splitext(os.path.basename(singleRead))[0]+'_fastqc.html')
     except Exception as e:
         print(e)
 
     return None
 
 
-## checkPairedQuality
-#
+# Check paired end quality
 def checkPairedRead(pairedRead, config, subdir):
     path = f"{config['DIR_OUT']}/{subdir}"
     os.makedirs(path, exist_ok=True)
     
     command = f"{config['EXE_FASTQC']} -o {path} {pairedRead[0]} {pairedRead[1]}"
     try:
         with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_report.py` & `MetaCerberus-1.1/lib/metacerberus_report.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # -*- coding: utf-8 -*-
 """metacerberus_report.py: Module to create the final HTML reports and tsv files
 """
 
 def warn(*args, **kwargs):
-    #print("args", str(args))
     pass
 import warnings
 warnings.warn = warn
 
 from collections import OrderedDict
 import os
+from pathlib import Path
 import time
 import shutil
 import base64
 import re
 from dominate.util import raw
 import pandas as pd
 import pkg_resources as pkg
@@ -80,29 +80,35 @@
     deconLabels = ['contaminants', 'QTrimmed', 'Total Removed', 'Results']
     reNstats = re.compile(r"N25[\w\s:%()]*>= ([0-9]*)[\w\s:%()]*>= ([0-9]*)[\w\s:%()]*>= ([0-9]*)[\w\s:%()]*>= ([0-9]*)")
     reMinMax = re.compile(r"Max.*:.([0-9]*)\nMin.*:.([0-9]*)")
     reGC = re.compile(r"GC count:\s*([0-9]*)[\w\s]*%:\s*([.0-9]*)")
     reTrim = re.compile(r"Filtering result:[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)[\w\s]*: ([0-9]*)")
     reDecon = re.compile(r"([0-9]*) reads \([0-9%.]*\)[\s]*([0-9]*)[\w\s(0-9-.%)]*:[\s]*([0-9]*) reads \([0-9%.]*\)[\s]*([0-9]*)[\w\s(0-9-.%)]*:[\s]*([0-9]*) reads \([0-9%.]*\)[\s]*([0-9]*)[\w\s(0-9-.%)]*:[\s]*([0-9]*) reads \([0-9%.]*\)[\s]*([0-9]*)")
     for key,value in readStats.items():
-        # GC Count
-        gcCount = reGC.search(value, re.MULTILINE)
-        if gcCount: dictStats[key]['GC count'] = gcCount.group(1)
-        if gcCount: dictStats[key]['GC %'] = gcCount.group(2)
-        # N25-N90
-        Nstats = reNstats.search(value, re.MULTILINE)
-        if Nstats:
-            for i,label in enumerate(nstatLabels, 1):
-                dictStats[key][label] = Nstats.group(i)
-        # Min-Max fasta
-        min_max = reMinMax.search(value, re.MULTILINE)
-        if min_max: dictStats[key]['Contig Min Length'] = min_max.group(2)
-        if min_max: dictStats[key]['Contig Max Length'] = min_max.group(1)
-        # Trimmed stats
         try:
+            # GC Count
+            gcCount = reGC.search(value, re.MULTILINE)
+            if gcCount: dictStats[key]['GC count'] = gcCount.group(1)
+            if gcCount: dictStats[key]['GC %'] = gcCount.group(2)
+        except: pass
+        try:
+            # N25-N90
+            Nstats = reNstats.search(value, re.MULTILINE)
+            if Nstats:
+                for i,label in enumerate(nstatLabels, 1):
+                    dictStats[key][label] = Nstats.group(i)
+        except: pass
+        try:
+            # Min-Max fasta
+            min_max = reMinMax.search(value, re.MULTILINE)
+            if min_max: dictStats[key]['Contig Min Length'] = min_max.group(2)
+            if min_max: dictStats[key]['Contig Max Length'] = min_max.group(1)
+        except: pass
+        try:
+            # Trimmed stats
             infile = os.path.join(config['DIR_OUT'], config['STEP'][3], key, "stderr.txt")
             trimStats = '\n'.join(open(infile).readlines())
             trim = reTrim.search(trimStats, re.MULTILINE)
             if trim:
                 for i,label in enumerate(trimLabels, 1):
                     dictStats[key]['trim: '+label] = trim.group(i)
         except: pass
@@ -127,27 +133,27 @@
         repeats = [y for x in value.values() for y in x]
         dictStats[key]["Contigs w/ N-repeats:"] = len(value)
         dictStats[key]["N-repeat Count"] = len(repeats)
         dictStats[key]["N-repeat Total Length"] = sum(repeats)
         dictStats[key]["N-repeat Average "] = round(sum(repeats)/len(repeats), 2)
 
 
-    #Write Combined Stats to File
+    # Write Combined Stats to File
     outfile = os.path.join(outpath, "combined", "stats.tsv")
     os.makedirs(os.path.join(outpath, "combined"), exist_ok=True)
     dfStats = pd.DataFrame(dictStats)
     dfStats.to_csv(outfile, sep='\t')
 
-    # HTML Plots of Stats
+    # Statistical plotting (HTML)
     outfile = os.path.join(outpath, "combined", "stats.html")
 
     tsv_stats = base64.b64encode(dfStats.to_csv(sep='\t').encode('utf-8')).decode('utf-8')
     dfStats = dfStats.apply(pd.to_numeric).T.rename_axis('Sample').reset_index()
     regex = re.compile(r"^([a-zA-Z]*_)")
-    prefixes = {regex.search(x).group(1):i for i,x in dfStats['Sample'].iteritems()}.keys()
+    prefixes = {regex.search(x).group(1):i for i,x in dfStats['Sample'].items()}.keys()
 
     figPlots = OrderedDict()
     for prefix in prefixes:
         dfPre = dfStats[dfStats['Sample'].str.startswith(prefix)]
         dfPre['Sample'] = dfPre['Sample'].apply(lambda x: regex.sub('', x))
         # ORF Calling Results
         try:
@@ -161,17 +167,22 @@
         # Average Protein Length
         try:
             fig = px.bar(dfPre, x='Sample', y='Average Protein Length',
                 labels={'Average Protein Length':"Peptide Length"})
             figPlots[f'Average Protein Length ({prefix[:-1]})'] = fig
         except: pass
         # Annotations
-        try:
-            df = dfPre[['Sample', 'FOAM KO Count', 'KEGG KO Count']]
-            df.rename(columns={'FOAM KO Count': 'FOAM KO', 'KEGG KO Count':'KEGG KO'}, inplace=True)
+        try: #TODO: Add COG, CAZy...
+            columns = ['Sample']
+            for column in dfPre.columns:
+                if re.search(r'[A-Za-z] ID Count', column):
+                    columns.append(column)
+            df = dfPre[columns]
+            columns = {col:col.replace(" Count", "") for col in columns}
+            df.rename(columns=columns, inplace=True)
             df = df.melt(id_vars=['Sample'], var_name='group', value_name='value')
             fig = px.bar(df, x='Sample', y='value', color='group', barmode='group',
                 labels={'value': 'count', 'group':''})
             figPlots[f'Annotations ({prefix[:-1]})'] = fig
         except: pass
         # GC %
         try:
@@ -215,18 +226,18 @@
     # Create HTML with Figures
     with dominate.document(title='Stats Report') as doc:
         with doc.head:
             meta(charset="utf-8")
             script(type="text/javascript", src="plotly-2.0.0.min.js")
             with style(type="text/css"):
                 raw('\n'+STYLESHEET)
-        with div(cls="document", id="cerberus-summary"):
+        with div(cls="document", id="metacerberus-summary"):
             with h1(cls="title"):
                 img(src=f"data:image/png;base64,{ICON}", height="40")
-                a("CERBERUS", cls="reference external", href="https://github.com/raw-lab/cerberus")
+                a("METACERBERUS", cls="reference external", href="https://github.com/raw-lab/metacerberus")
                 raw(" - Statistical Summary")
             with div(cls="contents topic", id="contents"):
                 with ul(cls="simple"):
                     li(a("Summary", cls="reference internal", href="#summary"))
                     with ul():
                         for key in figPlots.keys():
                             li(a(f"{key}", cls="reference internal", href=f"#{key}"))
@@ -252,66 +263,65 @@
     return dfStats
 
 
 ########## Write PCA Report ##########
 def write_PCA(outpath, pcaFigures):
     # PCA Files
     os.makedirs(os.path.join(outpath), exist_ok=True)
-#    countpathlist = []
     for database,figures in pcaFigures.items():
         prefix = f"{outpath}/{database}"
-        with open(prefix+"_PCA.htm", 'w') as htmlOut:
+        with open(prefix+"_PCA.html", 'w') as htmlOut:
             htmlOut.write("\n".join(htmlHeader))
             htmlOut.write(f"<h1>PCA Report for {database}<h1>\n")
             for graph,fig in figures.items():
                 if type(fig) is pd.DataFrame:
                     fig.to_csv(f"{prefix}_{graph}.tsv", index=False, header=True, sep='\t')
-#                    if "Counts" in graph:
-#                        countpathlist.append(f"{prefix}_{graph}.tsv")
                 else:
                     htmlFig = fig.to_html(full_html=False, include_plotlyjs=PLOTLY_SOURCE)
                     htmlOut.write(htmlFig + '\n')
                     fig.write_image(os.path.join(outpath, "img", f"{database}_{graph}.svg"))
             htmlOut.write('\n</body>\n</html>\n')
-    return# countpathlist
+    return
 
 
 ########## Write Tables ##########
 def writeTables(table_path: os.PathLike, filePrefix: os.PathLike):
+    if not Path(table_path).exists():
+        return
     table = pd.read_csv(table_path, sep='\t')
 
     regex = re.compile(r"^lvl[0-9]: ")
     table['Name'] = table['Name'].apply(lambda x : regex.sub('',x))
     try:
         levels = int(max(table[table.Level != 'Function'].Level))
         for i in range(1,levels+1):
             filter = table['Level']==str(i)
             table[filter][['Name','Count']].to_csv(f"{filePrefix}_level-{i}.tsv", index = False, header=True, sep='\t')
         regex = re.compile(r"^K[0-9]*: ")
         table['Name'] = table['Name'].apply(lambda x : regex.sub('',x))
     except:
         return
-    table[table['Level']=='Function'][['KO Id','Name','Count']].to_csv(f"{filePrefix}_level-ko.tsv", index = False, header=True, sep='\t')
+    table[table['Level']=='Function'][['Id','Name','Count']].to_csv(f"{filePrefix}_level-id.tsv", index = False, header=True, sep='\t')
     return
 
 
 ########## Write HTML Files ##########
 def write_HTML_files(outfile, figure, sample, name):
     sample = re.sub(r'^[a-zA-Z]*_', '', sample)
-    with dominate.document(title=f'Cerberus: {name} - {sample}') as doc:
+    with dominate.document(title=f'MetaCerberus: {name} - {sample}') as doc:
         with doc.head:
             meta(charset="utf-8")
             script(type="text/javascript", src="plotly-2.0.0.min.js")
             with style(type="text/css"):
                 raw('\n'+STYLESHEET)
-        with div(cls="document", id="cerberus-report"):
+        with div(cls="document", id="metacerberus-report"):
             # Header
             with h1(cls="title"):
                 img(src=f"data:image/png;base64,{ICON}", height="40")
-                a("CERBERUS", cls="reference external", href="https://github.com/raw-lab/cerberus")
+                a("METACERBERUS", cls="reference external", href="https://github.com/raw-lab/metacerberus")
                 raw(f" - {name} Bar Graphs for '{sample}'")
             # Side Panel
             with div(cls="contents topic", id="contents"):
                 with ul(cls="simple"):
                     li("(Bargraphs might take a few minutes to load)", cls="reference internal")
                     li("*Clicking on a bar in the graph displays the next level.")
                     li("The graph will cycle back to the first level after reaching the last level.")
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_trim.py` & `MetaCerberus-1.1/lib/metacerberus_trim.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,64 +1,72 @@
 # -*- coding: utf-8 -*-
 """metacerberus_trim.py: Module for trimming .fastq files
 Uses fastp [https://github.com/OpenGene/fastp#quality-filter]
 Uses porechop
 """
 
 import os
+from pathlib import Path
 import subprocess
 
 
-## trimSingleRead
-#
+# Trim single end reads
 def trimSingleRead(key_value, config, subdir):
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)
+    path = Path(config['DIR_OUT'], subdir)
 
     key = key_value[0]
     value = key_value[1]
 
-    trimmedRead = f'{path}/trimmed_{key}.fastq'
+    trimmedRead = path / f'trimmed_{key}.fastq'
+
+    done = path / "complete"
+    if not config['REPLACE'] and done.exists() and trimmedRead.exists():
+        return trimmedRead
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
     adapters = "" if not config['ADAPTERS'] else f"--adapter_fasta {config['ADAPTERS']}"
 
     if config['NANOPORE']:
         command = f"{config['EXE_PORECHOP']} -i {value} -o {trimmedRead} --threads {config['CPUS']}"
     else:
         command = f"{config['EXE_FASTP']} -i {value} -o {trimmedRead} -p 20 -M 30 -q 30 --low_complexity_filter {adapters} -h {path}/fastp.{key}.html -j {path}/fastp.{key}.json"
     try:
         with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
             subprocess.run(command, shell=True, check=True, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
         print("Error: Failed to execute trimSingleRead: " + command)
 
+    done.touch()
     return trimmedRead
 
 
-## trimPairedRead
-#
+# Trim paired end reads
 def trimPairedRead(key_value, config, subdir):
-    path = f"{config['DIR_OUT']}/{subdir}"
-    os.makedirs(path, exist_ok=True)
+    path = Path(config['DIR_OUT'], subdir)
 
     key = key_value[0]
     value = key_value[1]
     outR1 = f"trimmed_{os.path.basename(value[0])}"
     outR2 = f"trimmed_{os.path.basename(value[1])}"
 
-    trimmedReads = (os.path.join(path, outR1), os.path.join(path, outR2))
+    trimmedReads = (Path(path, outR1), Path(path, outR2))
+
+    done = path / "complete"
+    if not config['REPLACE'] and done.exists() and trimmedReads.exists():
+        return trimmedReads
+    done.unlink(missing_ok=True)
+    path.mkdir(exist_ok=True, parents=True)
 
     adapters = "" if not config['ADAPTERS'] else f"--adapter_fasta {config['ADAPTERS']}"
 
     command = f"{config['EXE_FASTP']} -i {value[0]} -I {value[1]} -o {trimmedReads[0]} -O {trimmedReads[1]} -p 20 -M 30 -q 30 --low_complexity_filter {adapters} -h {path}/fastp.{key}.html -j {path}/fastp.{key}.json"
     try:
         with open(f"{path}/stdout.txt", 'w') as fout, open(f"{path}/stderr.txt", 'w') as ferr:
             subprocess.run(command, shell=True, check=False, stdout=fout, stderr=ferr)
     except Exception as e:
         print(e)
         print("Error: Failed to execute trimPairedRead: " + key_value)
 
+    done.touch()
     return trimmedReads
-
-
-## End of script
```

### Comparing `MetaCerberus-1.0/lib/metacerberus_visual.py` & `MetaCerberus-1.1/lib/metacerberus_visual.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,31 +4,33 @@
 
 def warn(*args, **kwargs):
     #print("args", str(args))
     pass
 import warnings
 warnings.warn = warn
 
+from pathlib import Path
 import numpy as np
 import pandas as pd
-from pandas.core.frame import DataFrame
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler
 import plotly.express as px
 import plotly.graph_objects as go
 
 # global vars
 BAR_LIMIT = 10
 SUN_LIMIT = 15
 
 
 ########## Create Sunburst Figures ##########
 def graphSunburst(tables):
     figs = {}
     for dbName,table in tables.items():
+        if not Path(table).exists():
+            continue
         df: pd.DataFrame = pd.read_csv(table, sep='\t')
 
         # Filter top MAX_DEPTH
         try:
             levels = int(max(df[df.Level != 'Function'].Level))
             dfLevels = []
             for i in range(1,levels+1):
@@ -58,48 +60,45 @@
 
 ######### Create PCA Graph ##########
 def graphPCA(dfTables:dict):
 
     # Run PCA and add to Plots
     figs = {}
     for name,file in dfTables.items():
-        df = pd.read_csv(file, sep='\t').set_index('KO', drop=True).T
+        df = pd.read_csv(file, sep='\t').set_index('ID', drop=True).T
         if df.empty:
             continue
         df = df.fillna(0).astype(int)
         figs[name] = {}
 
         # Do PCA
         X = df.copy()
+
+        X.sort_index(inplace=True)
+
         scaler = StandardScaler()
         scaler.fit(X)
         X_scaled = scaler.transform(X)
 
         pca = PCA()
         X_pca = pca.fit_transform(X_scaled)
 
         # Loadings table
         loadings = pd.DataFrame(
             pca.components_.T,
             columns=[f"PC{pc}" for pc in range(1, pca.n_components_+1)], index=df.columns)
         loadings.reset_index(inplace=True) # Move index to column and re-index
         dfLoadings = pd.DataFrame()
-#        dfLoadings[['KO-ID','Name']] = loadings['KO'].str.split(':', n=1, expand=True)
-#        dfLoadings = pd.merge(dfLoadings, loadings, left_index=True, right_index=True)
-#        dfLoadings.drop(labels=['KO'], axis=1, inplace=True)
         
         # Loading Matrix
         loadings_matrix = pd.DataFrame(
             pca.components_.T * np.sqrt(pca.explained_variance_),
             columns=[f"PC{pc}" for pc in range(1, pca.n_components_+1)], index=df.columns)
         loadings_matrix.reset_index(inplace=True) # Move index to column and re-index
         dfLoadings_matrix = pd.DataFrame()
-#        dfLoadings_matrix[['KO-ID','Name']] = loadings_matrix['KO'].str.split(':', n=1, expand=True)
-#        dfLoadings_matrix = pd.merge(dfLoadings_matrix, loadings_matrix, left_index=True, right_index=True)
-#        dfLoadings_matrix.drop(labels=['KO'], axis=1, inplace=True)
 
         # Create Scree Plot
         figScree = px.bar(
             x=range(1, pca.n_components_+1),
             y=np.round(pca.explained_variance_ratio_*100, decimals=2),
             labels={'x':'Principal Component', 'y':'Percent Variance Explained'},
             title="Scree Plot"
@@ -129,18 +128,14 @@
                         ),
                     zaxis = dict(
                         backgroundcolor="White",
                         gridcolor="LightGray",
                         showbackground=False,
                         zerolinecolor="LightGray"
                         ),
-                    #width=700,
-                    #margin=dict(
-                    #r=10, l=10,
-                    #b=10, t=10
                   ))
         else:
             print("WARNING: Insufficient data in", name, "results for 3D PCA Plot")
             fig3d = None
 
 
         # Add Figures to Dictionary
@@ -152,74 +147,75 @@
         figs[name]["Loading_Matrix"] = loadings_matrix
 #        figs[name]["Counts_Table"] = df.T.reset_index().rename(columns={'index':'KO'})
         continue
 
     return figs
 
 
-########## Create Bar Chart Figures ##########
+########## Create Barchart Figures ##########
 def graphBarcharts(rollup_files:dict, dfCounts):
     dfCounts = dfCounts.copy()
 
     # Set index for our dataframes
     for dbName,table in dfCounts.items():
+        if not Path(table).exists():
+            continue
         df = pd.read_csv(table, sep='\t')
         dfCounts[dbName] = df.set_index('Name', inplace=False)
     
     # Recursively add branches to tree    
     def buildTree(branch, cols, dbName):
         if cols:
             name = cols.pop(0)
             while not name:
                  name = cols.pop(0)
             if name not in branch[0]:
                 branch[0][name] = ({}, 0) if not name else ({}, dfCounts[dbName].loc[name,'Count'])
-            #else:
-                #print("WARNING: duplicate line in rollup: ", dbName, name, cols) #TODO: Remove when bugs not found
             buildTree(branch[0][name], cols, dbName)
 
     # Add rows to tree
     dbTrees = dict()
     for dbName,filepath in rollup_files.items():
-        df = pd.read_csv(filepath, sep='\t')
-        tree = [dict(), 0]
-        for _,row in df.iterrows():
-            cols = list()
-            for colName,colData in row.iteritems():
-                if colName.startswith('L'):
-                    level = colName[1]
-                    if colData:
-                        cols.append(f"lvl{level}: {colData}")
-            if row.Function:
-                cols.append(f"{row.KO}: {row.Function}")
-                buildTree(tree, cols, dbName)
-        dbTrees[dbName] = tree[0]
+        try:
+            df = pd.read_csv(filepath, sep='\t')
+            tree = [dict(), 0]
+            for _,row in df.iterrows():
+                cols = list()
+                for colName,colData in row.items():
+                    if colName.startswith('L'):
+                        level = colName[1]
+                        if colData:
+                            cols.append(f"lvl{level}: {colData}")
+                if row.Function:
+                    cols.append(f"{row.KO}: {row.Function}")
+                    buildTree(tree, cols, dbName)
+            dbTrees[dbName] = tree[0]
+        except: pass
 
     # Create Figures
     figs = dict()
     for dbName,tree in dbTrees.items():
         figs[dbName] = createBarFigs(tree)
 
     return figs, dbTrees
 
 
 ##### Create Barchart Figures #####
 def createBarFigs(tree, level=1, name=""):
     chart = {}
     data = {}
     for k,v in tree.items():
-        #print("\t"*level, k, ' ', v[1], sep='')
         data[k] = v[1]
         chart.update(createBarFigs(v[0], level+1, k)) # updating from empty dict does nothing
     if len(data): #if no data at this level, just return the empty chart{}
         title = f"Level {level}: {name}".strip().strip(':')
         data = dict(sorted(data.items(), key=lambda item: item[1], reverse=True)[:BAR_LIMIT])
         fig = go.Figure( # Create the figure of this level's data
             layout={'title':title,
-                'yaxis_title':"KO Count"},
+                'yaxis_title':"KO Count"}, # TODO: Remove KO References from code
             data=[go.Bar(x=list(data.keys()), y=list(data.values()))]
             )
         if max(data.values()) < 20: # to remove decimals from graph with low counts, let plotly decide tick marks otherwise
             fig.update_yaxes(dtick=1)
         fig.update_layout(dict(plot_bgcolor='White', paper_bgcolor='White'))
         fig.update_xaxes(showline=True, linewidth=2, linecolor='black')
         fig.update_yaxes( showline=True, linewidth=2, linecolor='black',
```

### Comparing `MetaCerberus-1.0/lib/plotly-2.0.0.min.js` & `MetaCerberus-1.1/lib/plotly-2.0.0.min.js`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/lib/style.css` & `MetaCerberus-1.1/lib/style.css`

 * *Files identical despite different names*

### Comparing `MetaCerberus-1.0/setup.py` & `MetaCerberus-1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 
 # read long description
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="MetaCerberus",
-    version="1.0",
+    version="1.1",
     author="Jose L. Figueroa III, Richard A. White III",
     author_email="jlfiguer@uncc.edu",
     description="Versatile Functional Ontology Assignments for Metagenomes via Hidden Markov Model (HMM) searching with environmental focus of shotgun meta'omics data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/raw-lab/metacerberus",
-    scripts=['bin/metacerberus.py',
+    scripts=['bin/metacerberus.py',                                     # scripts to copy to 'bin' path
              'bin/ray-slurm-metacerberus.sh',
-             'bin/pathview-metacerberus.R'],                            # scripts to copy to 'bin' path
+             'bin/pathview-metacerberus.R'],
     packages=['meta_cerberus'],                                         # list of packages, installed to site-packages folder
     package_dir=dict(meta_cerberus='lib'),                              # dict with 'package'='relative dir'
     package_data=dict(meta_cerberus=package_files('lib/')),             # add non-python data to package, relative paths
     license="BSD License",  # metadata
     platforms=['Unix'],     # metadata
     classifiers=[           # This is the new updated way for metadata, but old way seems to still be used in some of the output
+        "Development Status :: 4 - Beta",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "License :: OSI Approved :: BSD License",
         "Operating System :: Unix",
     ],
-    python_requires='<3.10',
+    python_requires='>=3.8',
     install_requires=[
             'setuptools',
             'ray',
+            'grpcio',
             'metaomestats',
             'configargparse',
             'kaleido',
             'scikit-learn',
             'pandas',
             'plotly',
             'psutil',
```

