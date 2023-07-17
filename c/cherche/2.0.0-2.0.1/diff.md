# Comparing `tmp/cherche-2.0.0.tar.gz` & `tmp/cherche-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherche-2.0.0.tar", last modified: Mon May  8 16:19:38 2023, max compression
+gzip compressed data, was "cherche-2.0.1.tar", last modified: Mon Jul 17 10:10:38 2023, max compression
```

## Comparing `cherche-2.0.0.tar` & `cherche-2.0.1.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.172320 cherche-2.0.0/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1071 2023-01-07 22:47:32.000000 cherche-2.0.0/LICENSE
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     8363 2023-05-08 16:19:38.172445 cherche-2.0.0/PKG-INFO
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     7726 2023-05-08 16:13:17.000000 cherche-2.0.0/README.md
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.140000 cherche-2.0.0/cherche/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      134 2023-05-06 16:03:36.000000 cherche-2.0.0/cherche/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       63 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/__version__.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.142793 cherche-2.0.0/cherche/compose/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      151 2023-05-01 21:17:44.000000 cherche-2.0.0/cherche/compose/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6368 2023-05-07 23:19:39.000000 cherche-2.0.0/cherche/compose/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     8798 2023-05-07 17:58:57.000000 cherche-2.0.0/cherche/compose/intersection_union_vote.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    18160 2023-05-07 17:57:07.000000 cherche-2.0.0/cherche/compose/pipeline.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4608 2023-05-02 22:18:05.000000 cherche-2.0.0/cherche/compose/test_compose.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6904 2023-05-02 22:22:08.000000 cherche-2.0.0/cherche/compose/test_union_inter.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1980 2023-05-02 22:24:13.000000 cherche-2.0.0/cherche/compose/test_vote.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.143996 cherche-2.0.0/cherche/data/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      104 2023-04-30 19:26:48.000000 cherche-2.0.0/cherche/data/__init__.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.152688 cherche-2.0.0/cherche/data/semanlink/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)   899186 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/arxiv.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)  8324401 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/docs.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)  4587473 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink/tags.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3013 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/semanlink.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    29097 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/towns.json
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1577 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/data/towns.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.161212 cherche-2.0.0/cherche/evaluate/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       59 2023-05-08 15:34:32.000000 cherche-2.0.0/cherche/evaluate/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4141 2023-05-08 15:34:21.000000 cherche-2.0.0/cherche/evaluate/evaluate.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.163622 cherche-2.0.0/cherche/index/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       52 2023-04-30 13:03:44.000000 cherche-2.0.0/cherche/index/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     5056 2023-05-06 22:32:07.000000 cherche-2.0.0/cherche/index/faiss_index.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.164490 cherche-2.0.0/cherche/qa/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       37 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/qa/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6442 2023-05-07 14:50:43.000000 cherche-2.0.0/cherche/qa/qa.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.165498 cherche-2.0.0/cherche/query/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      110 2023-01-07 22:47:32.000000 cherche-2.0.0/cherche/query/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1153 2023-05-06 21:29:37.000000 cherche-2.0.0/cherche/query/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4455 2023-05-06 22:43:31.000000 cherche-2.0.0/cherche/query/norvig.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     5074 2023-05-06 22:43:33.000000 cherche-2.0.0/cherche/query/prf.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.167411 cherche-2.0.0/cherche/rank/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      217 2023-05-02 22:07:38.000000 cherche-2.0.0/cherche/rank/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)    10310 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     6692 2023-05-07 21:46:45.000000 cherche-2.0.0/cherche/rank/cross_encoder.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4155 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/dpr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4767 2023-05-07 14:33:29.000000 cherche-2.0.0/cherche/rank/embedding.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3805 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/rank/encoder.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3867 2023-05-06 13:01:19.000000 cherche-2.0.0/cherche/rank/test_rank.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.170548 cherche-2.0.0/cherche/retrieve/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      332 2023-04-30 19:33:52.000000 cherche-2.0.0/cherche/retrieve/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     2438 2023-05-07 14:03:51.000000 cherche-2.0.0/cherche/retrieve/base.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4513 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/dpr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4597 2023-05-08 12:44:27.000000 cherche-2.0.0/cherche/retrieve/embedding.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4371 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/encoder.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4750 2023-05-07 14:04:15.000000 cherche-2.0.0/cherche/retrieve/flash.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4951 2023-05-07 14:04:03.000000 cherche-2.0.0/cherche/retrieve/fuzz.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     3380 2023-05-07 14:03:59.000000 cherche-2.0.0/cherche/retrieve/lunr.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     4139 2023-05-06 21:28:01.000000 cherche-2.0.0/cherche/retrieve/test_retrieve.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     5742 2023-05-08 16:13:17.000000 cherche-2.0.0/cherche/retrieve/tfidf.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.172075 cherche-2.0.0/cherche/utils/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      174 2023-05-07 22:35:18.000000 cherche-2.0.0/cherche/utils/__init__.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1180 2023-05-07 22:35:03.000000 cherche-2.0.0/cherche/utils/batch.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1754 2023-05-01 20:27:11.000000 cherche-2.0.0/cherche/utils/quantize.py
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1983 2023-05-06 22:14:34.000000 cherche-2.0.0/cherche/utils/topk.py
-drwxr-xr-x   0 raphaelsourty   (501) staff       (20)        0 2023-05-08 16:19:38.140852 cherche-2.0.0/cherche.egg-info/
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     8363 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1437 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)        1 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)      736 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/requires.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)        8 2023-05-08 16:19:38.000000 cherche-2.0.0/cherche.egg-info/top_level.txt
--rw-r--r--   0 raphaelsourty   (501) staff       (20)       79 2023-05-08 16:19:38.172747 cherche-2.0.0/setup.cfg
--rw-r--r--   0 raphaelsourty   (501) staff       (20)     1745 2023-05-08 16:13:17.000000 cherche-2.0.0/setup.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.923171 cherche-2.0.1/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1071 2023-07-17 09:48:58.000000 cherche-2.0.1/LICENSE
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     8369 2023-07-17 10:10:38.923267 cherche-2.0.1/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     7732 2023-07-17 09:48:58.000000 cherche-2.0.1/README.md
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.891294 cherche-2.0.1/cherche/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      134 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       63 2023-07-17 09:58:41.000000 cherche-2.0.1/cherche/__version__.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.893664 cherche-2.0.1/cherche/compose/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      151 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     6368 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/base.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     8798 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/intersection_union_vote.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)    18160 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/pipeline.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4608 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/test_compose.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     6904 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/test_union_inter.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1980 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/compose/test_vote.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.895270 cherche-2.0.1/cherche/data/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      104 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/__init__.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.906397 cherche-2.0.1/cherche/data/semanlink/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)   899186 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/semanlink/arxiv.json
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)  8324401 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/semanlink/docs.json
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)  4587473 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/semanlink/tags.json
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     3013 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/semanlink.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)    29097 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/towns.json
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1577 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/data/towns.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.916962 cherche-2.0.1/cherche/evaluate/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       59 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/evaluate/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4141 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/evaluate/evaluate.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.917349 cherche-2.0.1/cherche/index/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       52 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/index/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5056 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/index/faiss_index.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.917731 cherche-2.0.1/cherche/qa/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       37 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/qa/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     6442 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/qa/qa.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.919745 cherche-2.0.1/cherche/query/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      110 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/query/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1153 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/query/base.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4455 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/query/norvig.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5074 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/query/prf.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.920844 cherche-2.0.1/cherche/rank/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      217 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)    10310 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/base.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     6692 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/cross_encoder.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4155 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/dpr.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4767 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/embedding.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     3805 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/encoder.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     3867 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/rank/test_rank.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.922341 cherche-2.0.1/cherche/retrieve/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      332 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     2438 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/base.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4513 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/dpr.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4597 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/embedding.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4371 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/encoder.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4750 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/flash.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4951 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/fuzz.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     3380 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/lunr.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     4139 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/test_retrieve.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     5742 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.923010 cherche-2.0.1/cherche/utils/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      174 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/utils/__init__.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1180 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/utils/batch.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1754 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/utils/quantize.py
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1983 2023-07-17 09:48:58.000000 cherche-2.0.1/cherche/utils/topk.py
+drwxr-xr-x   0 raphael.sourty   (502) staff       (20)        0 2023-07-17 10:10:38.892426 cherche-2.0.1/cherche.egg-info/
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     8369 2023-07-17 10:10:38.000000 cherche-2.0.1/cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1437 2023-07-17 10:10:38.000000 cherche-2.0.1/cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)        1 2023-07-17 10:10:38.000000 cherche-2.0.1/cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)      736 2023-07-17 10:10:38.000000 cherche-2.0.1/cherche.egg-info/requires.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)        8 2023-07-17 10:10:38.000000 cherche-2.0.1/cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)       79 2023-07-17 10:10:38.923521 cherche-2.0.1/setup.cfg
+-rw-r--r--   0 raphael.sourty   (502) staff       (20)     1745 2023-07-17 09:58:49.000000 cherche-2.0.1/setup.py
```

### Comparing `cherche-2.0.0/LICENSE` & `cherche-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/PKG-INFO` & `cherche-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cherche
-Version: 2.0.0
+Version: 2.0.1
 Summary: Neural Search
 Home-page: https://github.com/raphaelsty/cherche
 Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,question answering,semantic search
@@ -215,15 +215,15 @@
 
 TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
-```
+```bibtex
 @inproceedings{Sourty2022sigir,
     author = {Raphael Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant},
     title = {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
     booktitle = {Proceedings of SIGIR 2022},
     year = {2022}
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cherche Version: 2.0.0 Summary: Neural Search Home-
+Metadata-Version: 2.1 Name: cherche Version: 2.0.1 Summary: Neural Search Home-
 page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
 user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
 raphael.sourty@gmail.com License: MIT Keywords: neural search,information
 retrieval,question answering,semantic search Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown Provides-Extra: cpu Provides-Extra: gpu Provides-Extra: dev
@@ -89,15 +89,15 @@
 sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
 wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
 retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
 flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
 use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
 docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
 use cherche to produce results for your scientific publication, please refer to
-our SIGIR paper: ``` @inproceedings{Sourty2022sigir, author = {Raphael Sourty
-and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
+our SIGIR paper: ```bibtex @inproceedings{Sourty2022sigir, author = {Raphael
+Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
 {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
 booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
 The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
 raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
 Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
 scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-2.0.0/README.md` & `cherche-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -195,15 +195,15 @@
 
 TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
-```
+```bibtex
 @inproceedings{Sourty2022sigir,
     author = {Raphael Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant},
     title = {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
     booktitle = {Proceedings of SIGIR 2022},
     year = {2022}
 }
 ```
```

#### html2text {}

```diff
@@ -80,15 +80,15 @@
 sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
 wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
 retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
 flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
 use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
 docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
 use cherche to produce results for your scientific publication, please refer to
-our SIGIR paper: ``` @inproceedings{Sourty2022sigir, author = {Raphael Sourty
-and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
+our SIGIR paper: ```bibtex @inproceedings{Sourty2022sigir, author = {Raphael
+Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
 {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
 booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
 The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
 raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
 Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
 scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-2.0.0/cherche/compose/base.py` & `cherche-2.0.1/cherche/compose/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/compose/intersection_union_vote.py` & `cherche-2.0.1/cherche/compose/intersection_union_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/compose/pipeline.py` & `cherche-2.0.1/cherche/compose/pipeline.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/compose/test_compose.py` & `cherche-2.0.1/cherche/compose/test_compose.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/compose/test_union_inter.py` & `cherche-2.0.1/cherche/compose/test_union_inter.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/compose/test_vote.py` & `cherche-2.0.1/cherche/compose/test_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/semanlink/arxiv.json` & `cherche-2.0.1/cherche/data/semanlink/arxiv.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/semanlink/docs.json` & `cherche-2.0.1/cherche/data/semanlink/docs.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/semanlink/tags.json` & `cherche-2.0.1/cherche/data/semanlink/tags.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/semanlink.py` & `cherche-2.0.1/cherche/data/semanlink.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/towns.json` & `cherche-2.0.1/cherche/data/towns.json`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/data/towns.py` & `cherche-2.0.1/cherche/data/towns.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/evaluate/evaluate.py` & `cherche-2.0.1/cherche/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/index/faiss_index.py` & `cherche-2.0.1/cherche/index/faiss_index.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/qa/qa.py` & `cherche-2.0.1/cherche/qa/qa.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/query/base.py` & `cherche-2.0.1/cherche/query/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/query/norvig.py` & `cherche-2.0.1/cherche/query/norvig.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/query/prf.py` & `cherche-2.0.1/cherche/query/prf.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/base.py` & `cherche-2.0.1/cherche/rank/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/cross_encoder.py` & `cherche-2.0.1/cherche/rank/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/dpr.py` & `cherche-2.0.1/cherche/rank/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/embedding.py` & `cherche-2.0.1/cherche/rank/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/encoder.py` & `cherche-2.0.1/cherche/rank/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/rank/test_rank.py` & `cherche-2.0.1/cherche/rank/test_rank.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/base.py` & `cherche-2.0.1/cherche/retrieve/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/dpr.py` & `cherche-2.0.1/cherche/retrieve/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/embedding.py` & `cherche-2.0.1/cherche/retrieve/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/encoder.py` & `cherche-2.0.1/cherche/retrieve/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/flash.py` & `cherche-2.0.1/cherche/retrieve/flash.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/fuzz.py` & `cherche-2.0.1/cherche/retrieve/fuzz.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/lunr.py` & `cherche-2.0.1/cherche/retrieve/lunr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/test_retrieve.py` & `cherche-2.0.1/cherche/retrieve/test_retrieve.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/retrieve/tfidf.py` & `cherche-2.0.1/cherche/retrieve/tfidf.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/utils/batch.py` & `cherche-2.0.1/cherche/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/utils/quantize.py` & `cherche-2.0.1/cherche/utils/quantize.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche/utils/topk.py` & `cherche-2.0.1/cherche/utils/topk.py`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche.egg-info/PKG-INFO` & `cherche-2.0.1/cherche.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cherche
-Version: 2.0.0
+Version: 2.0.1
 Summary: Neural Search
 Home-page: https://github.com/raphaelsty/cherche
 Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,question answering,semantic search
@@ -215,15 +215,15 @@
 
 TfIdf retriever is a wrapper around [scikit-learn's TfidfVectorizer](https://scikit-learn.org/stable/modules/generated/sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/docs/pretrained_models.html) in a neural search pipeline.
 
 ## Citations
 
 If you use cherche to produce results for your scientific publication, please refer to our SIGIR paper:
 
-```
+```bibtex
 @inproceedings{Sourty2022sigir,
     author = {Raphael Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant},
     title = {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
     booktitle = {Proceedings of SIGIR 2022},
     year = {2022}
 }
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cherche Version: 2.0.0 Summary: Neural Search Home-
+Metadata-Version: 2.1 Name: cherche Version: 2.0.1 Summary: Neural Search Home-
 page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
 user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
 raphael.sourty@gmail.com License: MIT Keywords: neural search,information
 retrieval,question answering,semantic search Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown Provides-Extra: cpu Provides-Extra: gpu Provides-Extra: dev
@@ -89,15 +89,15 @@
 sklearn.feature_extraction.text.TfidfVectorizer.html). Lunr retriever is a
 wrapper around [Lunr.py](https://github.com/yeraydiazdiaz/lunr.py). Flash
 retriever is a wrapper around [FlashText](https://github.com/vi3k6i5/
 flashtext). DPR, Encode and CrossEncoder rankers are wrappers dedicated to the
 use of the pre-trained models of [SentenceTransformers](https://www.sbert.net/
 docs/pretrained_models.html) in a neural search pipeline. ## Citations If you
 use cherche to produce results for your scientific publication, please refer to
-our SIGIR paper: ``` @inproceedings{Sourty2022sigir, author = {Raphael Sourty
-and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
+our SIGIR paper: ```bibtex @inproceedings{Sourty2022sigir, author = {Raphael
+Sourty and Jose G. Moreno and Lynda Tamine and Francois-Paul Servant}, title =
 {CHERCHE: A new tool to rapidly implement pipelines in information retrieval},
 booktitle = {Proceedings of SIGIR 2022}, year = {2022} } ``` ## Dev Team ð¾
 The Cherche dev team is made up of [RaphaÃ«l Sourty](https://github.com/
 raphaelsty), [FranÃ§ois-Paul Servant](https://github.com/fpservant), [Nicolas
 Bizzozzero](https://github.com/NicolasBizzozzero), [Jose G Moreno](https://
 scholar.google.com/citations?user=4BZFUw8AAAAJ&hl=fr). ð¥³
```

### Comparing `cherche-2.0.0/cherche.egg-info/SOURCES.txt` & `cherche-2.0.1/cherche.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cherche-2.0.0/cherche.egg-info/requires.txt` & `cherche-2.0.1/cherche.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-numpy>=1.24.3
-scikit-learn>=1.2.2
+numpy>=1.23.5
+scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
 
 [cpu]
-numpy>=1.24.3
-scikit-learn>=1.2.2
+numpy>=1.23.5
+scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
 sentence-transformers>=2.2.2
 faiss-cpu>=1.7.4
 
 [dev]
-numpy>=1.24.3
-scikit-learn>=1.2.2
+numpy>=1.23.5
+scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
 sentence-transformers>=2.2.2
 faiss-cpu>=1.7.4
@@ -33,16 +33,16 @@
 mkdocs-jupyter>=0.21.0
 pytest-cov>=4.0.0
 pytest>=7.3.1
 isort>=5.12.0
 ipywidgets>=8.0.6
 
 [gpu]
-numpy>=1.24.3
-scikit-learn>=1.2.2
+numpy>=1.23.5
+scikit-learn>=1.1.2
 lunr>=0.6.2
 rapidfuzz>=3.0.0
 flashtext>=2.7
 tqdm>=4.62.3
 scipy>=1.7.3
 sentence-transformers>=2.2.2
 faiss-gpu>=1.7.4
```

### Comparing `cherche-2.0.0/setup.py` & `cherche-2.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from cherche.__version__ import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 base_packages = [
-    "numpy >= 1.24.3",
-    "scikit-learn >= 1.2.2",
+    "numpy >= 1.23.5",
+    "scikit-learn >= 1.1.2",
     "lunr >= 0.6.2",
     "rapidfuzz >= 3.0.0",
     "flashtext >= 2.7",
     "tqdm >= 4.62.3",
     "scipy >= 1.7.3",
 ]
```

