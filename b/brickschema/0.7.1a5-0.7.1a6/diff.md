# Comparing `tmp/brickschema-0.7.1a5.tar.gz` & `tmp/brickschema-0.7.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brickschema-0.7.1a5.tar", max compression
+gzip compressed data, was "brickschema-0.7.1a6.tar", max compression
```

## Comparing `brickschema-0.7.1a5.tar` & `brickschema-0.7.1a6.tar`

### file list

```diff
@@ -1,88 +1,87 @@
--rw-r--r--   0        0        0     1945 2021-07-23 15:38:20.787312 brickschema-0.7.1a5/LICENSE
--rw-r--r--   0        0        0     9176 2023-04-28 16:26:09.527473 brickschema-0.7.1a5/README.md
--rw-r--r--   0        0        0      530 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/__init__.py
--rw-r--r--   0        0        0      608 2020-11-10 06:11:23.496242 brickschema-0.7.1a5/brickschema/abbrmap.py
--rw-r--r--   0        0        0     2548 2022-11-20 19:44:54.915817 brickschema-0.7.1a5/brickschema/bacnet.py
--rw-r--r--   0        0        0     3572 2020-08-13 17:55:40.988282 brickschema-0.7.1a5/brickschema/bin/brick_validate.py
--rw-r--r--   0        0        0      145 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/__init__.py
--rw-r--r--   0        0        0       49 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/__main__.py
--rw-r--r--   0        0        0     4572 2022-02-24 17:03:40.701252 brickschema-0.7.1a5/brickschema/brickify/main.py
--rw-r--r--   0        0        0       45 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/__init__.py
--rw-r--r--   0        0        0     5890 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/Handler.py
--rw-r--r--   0        0        0     3755 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/__init__.py
--rw-r--r--   0        0        0     2511 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl
--rw-r--r--   0        0        0     3952 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json
--rw-r--r--   0        0        0     1577 2022-11-26 22:16:16.811116 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/__init__.py
--rw-r--r--   0        0        0     4339 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/__init__.py
--rw-r--r--   0        0        0     7715 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml
--rw-r--r--   0        0        0     4557 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/TableHandler.py
--rw-r--r--   0        0        0       74 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/__init__.py
--rw-r--r--   0        0        0        0 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/src/handlers/__init__.py
--rw-r--r--   0        0        0     6458 2021-06-10 16:16:30.295261 brickschema-0.7.1a5/brickschema/brickify/util.py
--rw-r--r--   0        0        0    23674 2023-03-29 17:17:46.145912 brickschema-0.7.1a5/brickschema/graph.py
--rw-r--r--   0        0        0    29028 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/inference.py
--rw-r--r--   0        0        0    14793 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/merge.py
--rw-r--r--   0        0        0     1949 2022-11-28 02:31:26.511103 brickschema-0.7.1a5/brickschema/namespaces.py
--rw-r--r--   0        0        0    33869 2021-03-03 20:58:32.139966 brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   540042 2021-08-06 17:41:07.025117 brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick.ttl
--rw-r--r--   0        0        0     6480 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/BrickShape.ttl
--rw-r--r--   0        0        0    72272 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/taglookup.pickle
--rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.1/vbis-masterlist.csv
--rw-r--r--   0        0        0    40592 2021-03-03 20:58:32.143966 brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   777615 2022-11-20 19:44:54.919817 brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick.ttl
--rw-r--r--   0        0        0     5682 2021-03-03 20:58:32.151966 brickschema-0.7.1a5/brickschema/ontologies/1.2/BrickShape.ttl
--rw-r--r--   0        0        0     3799 2022-11-20 19:44:28.855622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl
--rw-r--r--   0        0        0     4235 2022-11-20 19:44:28.851622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl
--rw-r--r--   0        0        0    25987 2022-11-20 19:44:28.851622 brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0  1013502 2021-11-09 22:15:04.147911 brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl
--rw-r--r--   0        0        0   630955 2022-11-20 19:44:54.919817 brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl
--rw-r--r--   0        0        0    72063 2022-11-21 22:27:04.539761 brickschema-0.7.1a5/brickschema/ontologies/1.2/taglookup.pickle
--rw-r--r--   0        0        0   334070 2021-03-03 20:58:32.155966 brickschema-0.7.1a5/brickschema/ontologies/1.2/vbis-masterlist.csv
--rw-r--r--   0        0        0  1601690 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/Brick.ttl
--rw-r--r--   0        0        0     3799 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl
--rw-r--r--   0        0        0     4235 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl
--rw-r--r--   0        0        0    25987 2022-11-28 02:31:26.515103 brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl
--rw-r--r--   0        0        0   695375 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl
--rw-r--r--   0        0        0    97692 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/taglookup.pickle
--rw-r--r--   0        0        0   334070 2022-11-28 02:31:26.519103 brickschema-0.7.1a5/brickschema/ontologies/1.3/vbis-masterlist.csv
--rw-r--r--   0        0        0     8710 2022-02-24 17:03:40.705252 brickschema-0.7.1a5/brickschema/orm.py
--rw-r--r--   0        0        0    11032 2023-05-22 23:54:32.421304 brickschema-0.7.1a5/brickschema/persistent.py
--rw-r--r--   0        0        0     2852 2021-12-14 06:59:29.240496 brickschema-0.7.1a5/brickschema/tagmap.py
--rw-r--r--   0        0        0     2399 2021-08-13 03:43:10.682814 brickschema-0.7.1a5/brickschema/web/index.html
--rw-r--r--   0        0        0     2233 2022-02-24 17:03:40.705252 brickschema-0.7.1a5/brickschema/web.py
--rw-r--r--   0        0        0     2068 2023-05-22 23:54:11.077119 brickschema-0.7.1a5/pyproject.toml
--rw-r--r--   0        0        0     2807 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/badBuilding.ttl
--rw-r--r--   0        0        0      881 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/brick_inference_test.ttl
--rw-r--r--   0        0        0      318 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/RAC/README.md
--rw-r--r--   0        0        0    29696 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls
--rw-r--r--   0        0        0     2400 2023-05-22 23:39:52.025722 brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls.brick.ttl
--rw-r--r--   0        0        0      139 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/haystack-v4/README.md
--rw-r--r--   0        0        0    49817 2023-02-06 17:25:43.296070 brickschema-0.7.1a5/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl
--rw-r--r--   0        0        0      819 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/README.md
--rw-r--r--   0        0        0      277 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv
--rw-r--r--   0        0        0     1158 2023-05-22 23:39:51.989722 brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv.brick.ttl
--rw-r--r--   0        0        0      902 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/template.json
--rw-r--r--   0        0        0      846 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/jinja2/template.yml
--rw-r--r--   0        0        0      306 2021-08-13 03:43:10.686814 brickschema-0.7.1a5/tests/data/brickify/rdf/README.md
--rw-r--r--   0        0        0      339 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/input.ttl
--rw-r--r--   0        0        0      427 2023-05-22 23:39:51.921722 brickschema-0.7.1a5/tests/data/brickify/rdf/input.ttl.brick.ttl
--rw-r--r--   0        0        0      868 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/template.json
--rw-r--r--   0        0        0     1155 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/rdf/template.yml
--rw-r--r--   0        0        0      485 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/README.md
--rw-r--r--   0        0        0      103 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/sheet.tsv
--rw-r--r--   0        0        0      430 2023-05-22 23:39:51.849721 brickschema-0.7.1a5/tests/data/brickify/tsv/sheet.tsv.brick.ttl
--rw-r--r--   0        0        0      513 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/template.json
--rw-r--r--   0        0        0      527 2021-06-10 16:16:30.299261 brickschema-0.7.1a5/tests/data/brickify/tsv/template.yml
--rw-r--r--   0        0        0    23372 2019-12-11 19:58:37.625874 brickschema-0.7.1a5/tests/data/carytown.json
--rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraOntology1.ttl
--rw-r--r--   0        0        0      657 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraOntology2.ttl
--rw-r--r--   0        0        0     1766 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/extraShapes.ttl
--rw-r--r--   0        0        0     1202 2021-08-06 17:41:07.033117 brickschema-0.7.1a5/tests/data/extraShapesWithExtraOnt.ttl
--rw-r--r--   0        0        0     1156 2022-11-28 02:31:26.523104 brickschema-0.7.1a5/tests/data/goodBuilding.ttl
--rw-r--r--   0        0        0      626 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/tags.ttl
--rw-r--r--   0        0        0     1236 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/test.ttl
--rw-r--r--   0        0        0      129 2021-03-03 20:58:32.159966 brickschema-0.7.1a5/tests/data/vbis_inference_test.ttl
--rw-r--r--   0        0        0    11393 1970-01-01 00:00:00.000000 brickschema-0.7.1a5/PKG-INFO
+-rw-r--r--   0        0        0     1945 2022-02-24 06:27:04.502259 brickschema-0.7.1a6/LICENSE
+-rw-r--r--   0        0        0     9176 2023-05-23 04:10:54.188693 brickschema-0.7.1a6/README.md
+-rw-r--r--   0        0        0      530 2023-03-29 17:12:12.006813 brickschema-0.7.1a6/brickschema/__init__.py
+-rw-r--r--   0        0        0     2548 2023-03-29 17:12:12.006910 brickschema-0.7.1a6/brickschema/bacnet.py
+-rw-r--r--   0        0        0     3572 2022-02-24 06:27:04.503543 brickschema-0.7.1a6/brickschema/bin/brick_validate.py
+-rw-r--r--   0        0        0      145 2022-02-24 06:27:04.503749 brickschema-0.7.1a6/brickschema/brickify/__init__.py
+-rw-r--r--   0        0        0       49 2022-02-24 06:27:04.503967 brickschema-0.7.1a6/brickschema/brickify/__main__.py
+-rw-r--r--   0        0        0     4572 2022-02-24 06:27:04.504168 brickschema-0.7.1a6/brickschema/brickify/main.py
+-rw-r--r--   0        0        0       45 2022-02-24 06:27:04.504340 brickschema-0.7.1a6/brickschema/brickify/src/__init__.py
+-rw-r--r--   0        0        0     5890 2022-02-24 06:27:04.504596 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/Handler.py
+-rw-r--r--   0        0        0     3755 2023-07-06 20:25:55.807813 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py
+-rw-r--r--   0        0        0        0 2022-02-24 06:27:04.505024 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/__init__.py
+-rw-r--r--   0        0        0     2511 2022-02-24 06:27:04.505251 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl
+-rw-r--r--   0        0        0     3952 2022-02-24 06:27:04.505402 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json
+-rw-r--r--   0        0        0     1577 2022-02-24 06:27:04.505704 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py
+-rw-r--r--   0        0        0        0 2022-02-24 06:27:04.505780 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/__init__.py
+-rw-r--r--   0        0        0     4339 2022-02-24 06:27:04.505981 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py
+-rw-r--r--   0        0        0        0 2022-02-24 06:27:04.506040 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/RACHandler/__init__.py
+-rw-r--r--   0        0        0     7715 2022-02-24 06:27:04.506379 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml
+-rw-r--r--   0        0        0     4557 2022-02-24 06:27:04.506599 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/TableHandler.py
+-rw-r--r--   0        0        0       74 2022-02-24 06:27:04.506787 brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-24 06:27:04.506896 brickschema-0.7.1a6/brickschema/brickify/src/handlers/__init__.py
+-rw-r--r--   0        0        0     6458 2022-02-24 06:27:04.507096 brickschema-0.7.1a6/brickschema/brickify/util.py
+-rw-r--r--   0        0        0    23674 2023-05-23 04:10:54.189018 brickschema-0.7.1a6/brickschema/graph.py
+-rw-r--r--   0        0        0    29028 2023-03-29 17:12:12.007386 brickschema-0.7.1a6/brickschema/inference.py
+-rw-r--r--   0        0        0    14793 2023-03-29 17:12:12.007514 brickschema-0.7.1a6/brickschema/merge.py
+-rw-r--r--   0        0        0     1949 2023-03-29 17:12:12.007592 brickschema-0.7.1a6/brickschema/namespaces.py
+-rw-r--r--   0        0        0    33869 2022-02-24 06:27:04.508673 brickschema-0.7.1a6/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   540042 2022-02-24 06:27:04.511127 brickschema-0.7.1a6/brickschema/ontologies/1.1/Brick.ttl
+-rw-r--r--   0        0        0     6480 2022-02-24 06:27:04.511404 brickschema-0.7.1a6/brickschema/ontologies/1.1/BrickShape.ttl
+-rw-r--r--   0        0        0    72272 2022-02-24 06:27:04.512261 brickschema-0.7.1a6/brickschema/ontologies/1.1/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2022-02-24 06:27:04.513614 brickschema-0.7.1a6/brickschema/ontologies/1.1/vbis-masterlist.csv
+-rw-r--r--   0        0        0    40592 2022-02-24 06:27:04.514115 brickschema-0.7.1a6/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   777615 2022-02-24 06:27:04.517143 brickschema-0.7.1a6/brickschema/ontologies/1.2/Brick.ttl
+-rw-r--r--   0        0        0     5682 2022-02-24 06:27:04.517402 brickschema-0.7.1a6/brickschema/ontologies/1.2/BrickShape.ttl
+-rw-r--r--   0        0        0     3799 2022-02-24 06:27:04.517597 brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl
+-rw-r--r--   0        0        0     4235 2022-02-24 06:27:04.517842 brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl
+-rw-r--r--   0        0        0    25987 2022-02-24 06:27:04.518046 brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0  1013502 2022-02-24 06:27:04.521787 brickschema-0.7.1a6/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl
+-rw-r--r--   0        0        0   630955 2022-02-24 06:27:04.524313 brickschema-0.7.1a6/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl
+-rw-r--r--   0        0        0    72063 2022-02-24 06:27:04.524722 brickschema-0.7.1a6/brickschema/ontologies/1.2/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2022-02-24 06:27:04.526134 brickschema-0.7.1a6/brickschema/ontologies/1.2/vbis-masterlist.csv
+-rw-r--r--   0        0        0  1601690 2023-03-29 17:12:12.009838 brickschema-0.7.1a6/brickschema/ontologies/1.3/Brick.ttl
+-rw-r--r--   0        0        0     3799 2023-03-29 17:12:12.009979 brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl
+-rw-r--r--   0        0        0     4235 2023-03-29 17:12:12.010039 brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl
+-rw-r--r--   0        0        0    25987 2023-03-29 17:12:12.010428 brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl
+-rw-r--r--   0        0        0   695375 2023-03-29 17:12:12.011400 brickschema-0.7.1a6/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl
+-rw-r--r--   0        0        0    97692 2023-03-29 17:12:12.011648 brickschema-0.7.1a6/brickschema/ontologies/1.3/taglookup.pickle
+-rw-r--r--   0        0        0   334070 2023-03-29 17:12:12.013975 brickschema-0.7.1a6/brickschema/ontologies/1.3/vbis-masterlist.csv
+-rw-r--r--   0        0        0     8710 2022-02-24 06:27:04.526399 brickschema-0.7.1a6/brickschema/orm.py
+-rw-r--r--   0        0        0    11032 2023-05-23 04:10:54.189258 brickschema-0.7.1a6/brickschema/persistent.py
+-rw-r--r--   0        0        0     2852 2022-02-24 06:27:04.526606 brickschema-0.7.1a6/brickschema/tagmap.py
+-rw-r--r--   0        0        0     2399 2022-02-24 06:27:04.527278 brickschema-0.7.1a6/brickschema/web/index.html
+-rw-r--r--   0        0        0     2233 2022-02-24 06:27:04.527017 brickschema-0.7.1a6/brickschema/web.py
+-rw-r--r--   0        0        0     2153 2023-07-07 21:40:30.259312 brickschema-0.7.1a6/pyproject.toml
+-rw-r--r--   0        0        0     2807 2023-03-29 17:12:12.016853 brickschema-0.7.1a6/tests/data/badBuilding.ttl
+-rw-r--r--   0        0        0      881 2023-03-29 17:12:12.016943 brickschema-0.7.1a6/tests/data/brick_inference_test.ttl
+-rw-r--r--   0        0        0      318 2022-02-24 06:27:04.538169 brickschema-0.7.1a6/tests/data/brickify/RAC/README.md
+-rw-r--r--   0        0        0    29696 2022-02-24 06:27:04.538491 brickschema-0.7.1a6/tests/data/brickify/RAC/rac.xls
+-rw-r--r--   0        0        0     2400 2023-07-06 18:56:48.120957 brickschema-0.7.1a6/tests/data/brickify/RAC/rac.xls.brick.ttl
+-rw-r--r--   0        0        0      139 2022-02-24 06:27:04.538750 brickschema-0.7.1a6/tests/data/brickify/haystack-v4/README.md
+-rw-r--r--   0        0        0    49817 2023-07-06 20:26:17.170084 brickschema-0.7.1a6/tests/data/brickify/haystack-v4/charlie.ttl.brick.ttl
+-rw-r--r--   0        0        0      819 2022-02-24 06:27:04.538987 brickschema-0.7.1a6/tests/data/brickify/jinja2/README.md
+-rw-r--r--   0        0        0      277 2022-02-24 06:27:04.539226 brickschema-0.7.1a6/tests/data/brickify/jinja2/sheet.csv
+-rw-r--r--   0        0        0     1158 2023-07-06 18:56:48.085229 brickschema-0.7.1a6/tests/data/brickify/jinja2/sheet.csv.brick.ttl
+-rw-r--r--   0        0        0      902 2022-02-24 06:27:04.539407 brickschema-0.7.1a6/tests/data/brickify/jinja2/template.json
+-rw-r--r--   0        0        0      846 2022-02-24 06:27:04.539637 brickschema-0.7.1a6/tests/data/brickify/jinja2/template.yml
+-rw-r--r--   0        0        0      306 2022-02-24 06:27:04.539917 brickschema-0.7.1a6/tests/data/brickify/rdf/README.md
+-rw-r--r--   0        0        0      339 2022-02-24 06:27:04.540085 brickschema-0.7.1a6/tests/data/brickify/rdf/input.ttl
+-rw-r--r--   0        0        0      427 2023-07-06 18:56:48.077546 brickschema-0.7.1a6/tests/data/brickify/rdf/input.ttl.brick.ttl
+-rw-r--r--   0        0        0      868 2022-02-24 06:27:04.540247 brickschema-0.7.1a6/tests/data/brickify/rdf/template.json
+-rw-r--r--   0        0        0     1155 2022-02-24 06:27:04.540410 brickschema-0.7.1a6/tests/data/brickify/rdf/template.yml
+-rw-r--r--   0        0        0      485 2022-02-24 06:27:04.540665 brickschema-0.7.1a6/tests/data/brickify/tsv/README.md
+-rw-r--r--   0        0        0      103 2022-02-24 06:27:04.540834 brickschema-0.7.1a6/tests/data/brickify/tsv/sheet.tsv
+-rw-r--r--   0        0        0      430 2023-07-06 18:56:48.053813 brickschema-0.7.1a6/tests/data/brickify/tsv/sheet.tsv.brick.ttl
+-rw-r--r--   0        0        0      513 2022-02-24 06:27:04.540984 brickschema-0.7.1a6/tests/data/brickify/tsv/template.json
+-rw-r--r--   0        0        0      527 2022-02-24 06:27:04.541194 brickschema-0.7.1a6/tests/data/brickify/tsv/template.yml
+-rw-r--r--   0        0        0    23372 2022-02-24 06:27:04.541454 brickschema-0.7.1a6/tests/data/carytown.json
+-rw-r--r--   0        0        0      657 2023-03-29 17:12:12.017134 brickschema-0.7.1a6/tests/data/extraOntology1.ttl
+-rw-r--r--   0        0        0      657 2023-03-29 17:12:12.017212 brickschema-0.7.1a6/tests/data/extraOntology2.ttl
+-rw-r--r--   0        0        0     1766 2023-03-29 17:12:12.017292 brickschema-0.7.1a6/tests/data/extraShapes.ttl
+-rw-r--r--   0        0        0     1202 2022-02-24 06:27:04.542389 brickschema-0.7.1a6/tests/data/extraShapesWithExtraOnt.ttl
+-rw-r--r--   0        0        0     1156 2023-03-29 17:12:12.017371 brickschema-0.7.1a6/tests/data/goodBuilding.ttl
+-rw-r--r--   0        0        0      626 2022-02-24 06:27:04.542891 brickschema-0.7.1a6/tests/data/tags.ttl
+-rw-r--r--   0        0        0     1236 2022-02-24 06:27:04.543081 brickschema-0.7.1a6/tests/data/test.ttl
+-rw-r--r--   0        0        0      129 2022-02-24 06:27:04.543253 brickschema-0.7.1a6/tests/data/vbis_inference_test.ttl
+-rw-r--r--   0        0        0    11358 1970-01-01 00:00:00.000000 brickschema-0.7.1a6/PKG-INFO
```

### Comparing `brickschema-0.7.1a5/LICENSE` & `brickschema-0.7.1a6/LICENSE`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/README.md` & `brickschema-0.7.1a6/README.md`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/__init__.py` & `brickschema-0.7.1a6/brickschema/__init__.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/bacnet.py` & `brickschema-0.7.1a6/brickschema/bacnet.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/bin/brick_validate.py` & `brickschema-0.7.1a6/brickschema/bin/brick_validate.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/main.py` & `brickschema-0.7.1a6/brickschema/brickify/main.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/Handler.py` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/Handler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/HaystackHandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
             input_format=input_format,
             module_path=module_path,
             config_file=config_file,
         )
         self.hs_graph = rdflib.Graph()
         self.h2b_graph = rdflib.Graph()
         self.hs_graph.parse(
-            source="https://project-haystack.dev/download/defs.ttl", format="turtle"
+            source="https://project-haystack.org/download/defs.ttl", format="turtle"
         )
         with importlib_resources.path(module_path[0], "analogy.ttl") as data_file:
             with open(data_file, "r") as h2b:
                 self.h2b_graph.parse(h2b, format="turtle")
 
     def ingest_data(self):
         """
@@ -58,15 +58,15 @@
 
     def infer(self):
         """
         Uses HaystackRDFInferenceSession to extract tags from instance types (classes) and use a
         TagInferenceSession to provide inference of a Brick model from a Haystack model.
         """
         super().infer()
-        haysess = HaystackRDFInferenceSession("https://project-haystack.dev/example#")
+        haysess = HaystackRDFInferenceSession("https://project-haystack.org/example#")
         haysess.infer_model(self.graph)
 
     def clean_up(self):
         """
         Removes the analogy graph and the haystack definitions, haystack triples from the output graph.
         """
         self.graph -= self.hs_graph
```

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/analogy.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/conversions/haystack.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/HaystackHandler/utils/HaystackRDFInferenceSession.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/RACHandler/RACHandler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/RACHandler/conversions/rac.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/src/handlers/Handler/TableHandler.py` & `brickschema-0.7.1a6/brickschema/brickify/src/handlers/Handler/TableHandler.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/brickify/util.py` & `brickschema-0.7.1a6/brickschema/brickify/util.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/graph.py` & `brickschema-0.7.1a6/brickschema/graph.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/inference.py` & `brickschema-0.7.1a6/brickschema/inference.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/merge.py` & `brickschema-0.7.1a6/brickschema/merge.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/namespaces.py` & `brickschema-0.7.1a6/brickschema/namespaces.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.1/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.1/Brick.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.1/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.1/BrickShape.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.1/BrickShape.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.1/taglookup.pickle` & `brickschema-0.7.1a6/brickschema/ontologies/1.1/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.1/vbis-masterlist.csv` & `brickschema-0.7.1a6/brickschema/ontologies/1.1/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/Brick.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/BrickShape.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/BrickShape.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-BOT-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-REC-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/alignments/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/extensions/brick_extension_bacnet.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/extensions/brick_extension_shacl_tag_inference.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/taglookup.pickle` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.2/vbis-masterlist.csv` & `brickschema-0.7.1a6/brickschema/ontologies/1.2/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/Brick.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/Brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-BOT-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-REC-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/alignments/Brick-VBIS-alignment.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/extensions/brick_extension_shacl_tag_inference.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/taglookup.pickle` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/taglookup.pickle`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/ontologies/1.3/vbis-masterlist.csv` & `brickschema-0.7.1a6/brickschema/ontologies/1.3/vbis-masterlist.csv`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/orm.py` & `brickschema-0.7.1a6/brickschema/orm.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/persistent.py` & `brickschema-0.7.1a6/brickschema/persistent.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/tagmap.py` & `brickschema-0.7.1a6/brickschema/tagmap.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/web/index.html` & `brickschema-0.7.1a6/brickschema/web/index.html`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/brickschema/web.py` & `brickschema-0.7.1a6/brickschema/web.py`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/pyproject.toml` & `brickschema-0.7.1a6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "brickschema"
-version = "0.7.1a5"
+version = "0.7.1a6"
 description = "A library for working with the Brick ontology for buildings (brickschema.org)"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 include = ["brickschema/ontologies", "tests/data", "brickschema/web"]
 homepage = "https://brickschema.org"
 license = "BSD-3-Clause"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rdflib = "^6.2"
 owlrl = "^6.0"
-pytest = "^7.2"
+
 pyshacl = "^0.22"
 requests = "^2.25.0"
 importlib-resources = "^3.3.0"
 click-spinner = {optional = true, version="^0.1.10"}
 tabulate = {optional = true, version="^0.8.7"}
 Jinja2 = {optional = true, version="^3.1"}
 xlrd = {optional = true, version="^1.2.0"}
@@ -27,14 +27,27 @@
 dedupe = {optional = true, version = "^2.0"}
 reasonable = {optional = true, version="^0.2.2a4"}
 sqlalchemy = {optional = true, version="^1.4"}
 rdflib_sqlalchemy = {optional = true, version = "^0.5"}
 BAC0 = {optional = true, version = "^22.9"}
 networkx = {optional = true, version="^2.6"}
 
+[tool.poetry.group.dev.dependencies]
+flake8 = "^3.7"
+pre-commit = "^2.1"
+tqdm = "^4.56.0"
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2"
+pytest-xdist = {extras = ["psutil"], version = "^2.3.0"}
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^4.2"
+sphinx-rtd-theme = "^1.0.0"
+
 [tool.poetry.scripts]
 brick_validate = "brickschema.bin.brick_validate:main"
 brickify = "brickschema.brickify.main:app"
 
 [tool.poetry.extras]
 allegro = ["docker"]
 brickify = ["click-spinner", "tabulate", "Jinja2", "xlrd", "PyYAML", "typer"]
@@ -43,18 +56,10 @@
 orm = ["sqlalchemy"]
 reasonable = ["reasonable"]
 persistence = ["rdflib_sqlalchemy", "sqlalchemy"]
 bacnet = ["BAC0"]
 networkx = ["networkx"]
 all = ["docker","click-spinner", "tabulate", "Jinja2", "xlrd", "PyYAML", "typer", "Flask", "dedupe", "colorama", "reasonable", "sqlalchemy", "rdflib_sqlalchemy", "BAC0", "networkx"]
 
-[tool.poetry.dev-dependencies]
-pre-commit = "^2.1"
-flake8 = "^3.7"
-tqdm = "^4.56.0"
-pytest-xdist = {extras = ["psutil"], version = "^2.3.0"}
-Sphinx = "^4.2"
-sphinx-rtd-theme = "^1.0.0"
-
 [build-system]
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `brickschema-0.7.1a5/tests/data/badBuilding.ttl` & `brickschema-0.7.1a6/tests/data/badBuilding.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brick_inference_test.ttl` & `brickschema-0.7.1a6/tests/data/brick_inference_test.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls` & `brickschema-0.7.1a6/tests/data/brickify/RAC/rac.xls`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/RAC/rac.xls.brick.ttl` & `brickschema-0.7.1a6/tests/data/brickify/RAC/rac.xls.brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/jinja2/README.md` & `brickschema-0.7.1a6/tests/data/brickify/jinja2/README.md`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/jinja2/sheet.csv.brick.ttl` & `brickschema-0.7.1a6/tests/data/brickify/jinja2/sheet.csv.brick.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/jinja2/template.json` & `brickschema-0.7.1a6/tests/data/brickify/jinja2/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/jinja2/template.yml` & `brickschema-0.7.1a6/tests/data/brickify/jinja2/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/rdf/template.json` & `brickschema-0.7.1a6/tests/data/brickify/rdf/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/rdf/template.yml` & `brickschema-0.7.1a6/tests/data/brickify/rdf/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/tsv/template.json` & `brickschema-0.7.1a6/tests/data/brickify/tsv/template.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/brickify/tsv/template.yml` & `brickschema-0.7.1a6/tests/data/brickify/tsv/template.yml`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/carytown.json` & `brickschema-0.7.1a6/tests/data/carytown.json`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/extraOntology1.ttl` & `brickschema-0.7.1a6/tests/data/extraOntology1.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/extraOntology2.ttl` & `brickschema-0.7.1a6/tests/data/extraOntology2.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/extraShapes.ttl` & `brickschema-0.7.1a6/tests/data/extraShapes.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/extraShapesWithExtraOnt.ttl` & `brickschema-0.7.1a6/tests/data/extraShapesWithExtraOnt.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/goodBuilding.ttl` & `brickschema-0.7.1a6/tests/data/goodBuilding.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/tags.ttl` & `brickschema-0.7.1a6/tests/data/tags.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/tests/data/test.ttl` & `brickschema-0.7.1a6/tests/data/test.ttl`

 * *Files identical despite different names*

### Comparing `brickschema-0.7.1a5/PKG-INFO` & `brickschema-0.7.1a6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brickschema
-Version: 0.7.1a5
+Version: 0.7.1a6
 Summary: A library for working with the Brick ontology for buildings (brickschema.org)
 Home-page: https://brickschema.org
 License: BSD-3-Clause
 Author: Gabe Fierro
 Author-email: gtfierro@mines.edu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -30,15 +30,14 @@
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: colorama (>=0.4.4,<0.5.0) ; extra == "merge" or extra == "all"
 Requires-Dist: dedupe (>=2.0,<3.0) ; extra == "merge" or extra == "all"
 Requires-Dist: importlib-resources (>=3.3.0,<4.0.0)
 Requires-Dist: networkx (>=2.6,<3.0) ; extra == "networkx" or extra == "all"
 Requires-Dist: owlrl (>=6.0,<7.0)
 Requires-Dist: pyshacl (>=0.22,<0.23)
-Requires-Dist: pytest (>=7.2,<8.0)
 Requires-Dist: rdflib (>=6.2,<7.0)
 Requires-Dist: rdflib_sqlalchemy (>=0.5,<0.6) ; extra == "persistence" or extra == "all"
 Requires-Dist: reasonable (>=0.2.2a4,<0.3.0) ; extra == "reasonable" or extra == "all"
 Requires-Dist: requests (>=2.25.0,<3.0.0)
 Requires-Dist: sqlalchemy (>=1.4,<2.0) ; extra == "orm" or extra == "persistence" or extra == "all"
 Requires-Dist: tabulate (>=0.8.7,<0.9.0) ; extra == "brickify" or extra == "all"
 Requires-Dist: typer (>=0.4.1,<0.5.0) ; extra == "brickify" or extra == "all"
```

