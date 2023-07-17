# Comparing `tmp/SLAMBUC-0.1.0.tar.gz` & `tmp/SLAMBUC-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SLAMBUC-0.1.0.tar", last modified: Thu Jul  6 12:27:39 2023, max compression
+gzip compressed data, was "SLAMBUC-0.2.0.tar", last modified: Mon Jul 17 15:27:22 2023, max compression
```

## Comparing `SLAMBUC-0.1.0.tar` & `SLAMBUC-0.2.0.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.986443 SLAMBUC-0.1.0/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    11357 2023-06-30 19:22:13.000000 SLAMBUC-0.1.0/LICENSE
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    16081 2023-07-06 12:27:39.986443 SLAMBUC-0.1.0/PKG-INFO
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    15115 2023-07-06 08:41:21.000000 SLAMBUC-0.1.0/README.md
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/SLAMBUC.egg-info/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    16081 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/PKG-INFO
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2316 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/SOURCES.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/dependency_links.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/not-zip-safe
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      197 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/requires.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)       13 2023-07-06 12:27:39.000000 SLAMBUC-0.1.0/SLAMBUC.egg-info/top_level.txt
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1669 2023-07-04 11:45:39.000000 SLAMBUC-0.1.0/pyproject.toml
--rw-rw-r--   0 czentye   (1000) czentye   (1000)       38 2023-07-06 12:27:39.986443 SLAMBUC-0.1.0/setup.cfg
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2414 2023-07-06 08:22:16.000000 SLAMBUC-0.1.0/setup.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/slambuc/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      596 2023-07-06 08:04:58.000000 SLAMBUC-0.1.0/slambuc/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/slambuc/alg/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      857 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/slambuc/alg/chain/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      611 2023-07-05 20:30:38.000000 SLAMBUC-0.1.0/slambuc/alg/chain/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/slambuc/alg/chain/dp/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      720 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/dp/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3107 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/dp/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     5658 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/dp/min.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    12747 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/dp/mtx.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.970443 SLAMBUC-0.1.0/slambuc/alg/chain/ser/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      688 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/ser/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3012 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/ser/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    11235 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/chain/ser/ilp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/ext/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      956 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/ext/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2444 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/ext/baseline.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    10444 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/ext/csp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     9075 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/ext/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     7605 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/ext/min_cut.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/service/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      646 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/service/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1476 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/service/common.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/tree/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      630 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/tree/dp/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      699 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     6436 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     9346 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/meta.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     7596 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/min.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     9566 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/seq.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1869 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/dp/seq_state.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/tree/layout/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      574 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/layout/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    14487 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/layout/ilp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.974443 SLAMBUC-0.1.0/slambuc/alg/tree/par/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      880 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/par/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3712 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/par/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    18830 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/par/ilp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    18727 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/par/pseudo.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    12721 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/par/pseudo_mp.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.978443 SLAMBUC-0.1.0/slambuc/alg/tree/ser/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1006 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    36174 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/bicriteria.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3583 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/greedy.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    18544 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/ilp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    12675 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/ilp_cplex.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    16024 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/pseudo.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    23179 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/tree/ser/pseudo_mp.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    26971 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/alg/util.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.978443 SLAMBUC-0.1.0/slambuc/gen/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      647 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.978443 SLAMBUC-0.1.0/slambuc/gen/cluster/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      642 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/__init__.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.978443 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2214 2023-03-09 09:23:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/cpl_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   255904 2023-03-09 12:08:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/instance_num_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     1419 2023-03-09 09:24:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/level_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      429 2023-03-09 09:28:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_cpu_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   212962 2023-03-09 09:27:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_duration_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2557 2023-03-09 09:30:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_mem_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     4077 2023-03-09 09:25:00.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_num_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     8253 2023-07-03 17:24:03.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/job_tree.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.978443 SLAMBUC-0.1.0/slambuc/gen/cluster/samples/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)   245994 2023-03-06 16:52:01.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/samples/batch_task.csv
--rw-rw-r--   0 czentye   (1000) czentye   (1000)  2397573 2023-03-01 10:28:19.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/samples/sample_tasks.csv
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3863 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/cluster/syn_job.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     4045 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/io.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.982443 SLAMBUC-0.1.0/slambuc/gen/microservice/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/microservice/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     4420 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/microservice/faas_tree.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.982443 SLAMBUC-0.1.0/slambuc/gen/microservice/hist/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      865 2023-03-16 12:15:00.000000 SLAMBUC-0.1.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      897 2023-03-16 12:26:00.000000 SLAMBUC-0.1.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3443 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/microservice/power_ba_graph.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.982443 SLAMBUC-0.1.0/slambuc/gen/random/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/random/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2402 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/random/random_tree.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     2904 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/gen/transform.py
-drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-06 12:27:39.982443 SLAMBUC-0.1.0/slambuc/misc/
--rw-rw-r--   0 czentye   (1000) czentye   (1000)      574 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/misc/__init__.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     3110 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/misc/generator.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)     6071 2023-07-03 16:04:48.000000 SLAMBUC-0.1.0/slambuc/misc/plot.py
--rw-rw-r--   0 czentye   (1000) czentye   (1000)    19429 2023-07-03 19:30:00.000000 SLAMBUC-0.1.0/slambuc/misc/util.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    11357 2023-06-30 19:22:13.000000 SLAMBUC-0.2.0/LICENSE
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13287 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/PKG-INFO
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    12301 2023-07-17 15:20:23.000000 SLAMBUC-0.2.0/README.md
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/SLAMBUC.egg-info/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13287 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/PKG-INFO
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2316 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/SOURCES.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/dependency_links.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)        1 2023-07-17 15:27:21.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/not-zip-safe
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      226 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/requires.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)       18 2023-07-17 15:27:22.000000 SLAMBUC-0.2.0/SLAMBUC.egg-info/top_level.txt
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1948 2023-07-10 20:36:21.000000 SLAMBUC-0.2.0/pyproject.toml
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)       38 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/setup.cfg
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2414 2023-07-17 15:22:22.000000 SLAMBUC-0.2.0/setup.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      596 2023-07-17 15:22:13.000000 SLAMBUC-0.2.0/slambuc/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1488 2023-07-17 14:17:13.000000 SLAMBUC-0.2.0/slambuc/alg/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      611 2023-07-05 20:30:38.000000 SLAMBUC-0.2.0/slambuc/alg/chain/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/dp/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      720 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3531 2023-07-14 09:45:49.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6082 2023-07-14 12:53:11.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/min.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13948 2023-07-14 12:26:08.000000 SLAMBUC-0.2.0/slambuc/alg/chain/dp/mtx.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/chain/ser/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      688 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3455 2023-07-14 09:45:49.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    12538 2023-07-14 09:55:33.000000 SLAMBUC-0.2.0/slambuc/alg/chain/ser/ilp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/ext/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      956 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/ext/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2432 2023-07-14 12:04:55.000000 SLAMBUC-0.2.0/slambuc/alg/ext/baseline.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    11000 2023-07-14 12:11:51.000000 SLAMBUC-0.2.0/slambuc/alg/ext/csp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     8901 2023-07-14 12:12:50.000000 SLAMBUC-0.2.0/slambuc/alg/ext/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     7569 2023-07-14 12:15:57.000000 SLAMBUC-0.2.0/slambuc/alg/ext/min_cut.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/service/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      646 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/service/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1581 2023-07-17 15:18:02.000000 SLAMBUC-0.2.0/slambuc/alg/service/common.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.126269 SLAMBUC-0.2.0/slambuc/alg/tree/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      652 2023-07-14 13:43:20.000000 SLAMBUC-0.2.0/slambuc/alg/tree/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/dp/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      738 2023-07-14 12:23:04.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6571 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    10080 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/meta.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     8311 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/min.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    10608 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3512 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq_state.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/layout/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      678 2023-07-14 13:31:02.000000 SLAMBUC-0.2.0/slambuc/alg/tree/layout/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    15230 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/layout/ilp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/par/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      880 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3964 2023-07-14 15:03:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    20165 2023-07-14 15:09:47.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/ilp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    19075 2023-07-14 15:19:54.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    14051 2023-07-14 15:28:59.000000 SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo_mp.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/alg/tree/ser/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1006 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    39042 2023-07-14 15:05:26.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/bicriteria.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3807 2023-07-14 15:05:26.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/greedy.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    20792 2023-07-14 15:12:10.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    13015 2023-07-14 15:17:56.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp_cplex.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    16298 2023-07-14 15:31:33.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    26917 2023-07-14 15:36:32.000000 SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo_mp.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    37129 2023-07-17 15:01:40.000000 SLAMBUC-0.2.0/slambuc/alg/util.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/gen/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      647 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.130269 SLAMBUC-0.2.0/slambuc/gen/cluster/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      642 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/__init__.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.134269 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2214 2023-03-09 09:23:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/cpl_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   255904 2023-03-09 12:08:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/instance_num_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     1419 2023-03-09 09:24:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/level_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      429 2023-03-09 09:28:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_cpu_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   212962 2023-03-09 09:27:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_duration_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2557 2023-03-09 09:30:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_mem_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     4077 2023-03-09 09:25:00.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_num_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     9982 2023-07-17 06:38:45.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/job_tree.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.134269 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)   245994 2023-03-06 16:52:01.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/batch_task.csv
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)  2397573 2023-03-01 10:28:19.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/samples/sample_tasks.csv
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     4094 2023-07-17 06:33:18.000000 SLAMBUC-0.2.0/slambuc/gen/cluster/syn_job.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     5021 2023-07-17 07:03:22.000000 SLAMBUC-0.2.0/slambuc/gen/io.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/microservice/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     5425 2023-07-17 06:38:45.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/faas_tree.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      865 2023-03-16 12:15:00.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      897 2023-03-16 12:26:00.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3489 2023-07-17 06:50:42.000000 SLAMBUC-0.2.0/slambuc/gen/microservice/power_ba_graph.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/gen/random/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      643 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/gen/random/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     2981 2023-07-17 06:54:00.000000 SLAMBUC-0.2.0/slambuc/gen/random/random_tree.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3202 2023-07-17 07:09:04.000000 SLAMBUC-0.2.0/slambuc/gen/transform.py
+drwxrwxr-x   0 czentye   (1000) czentye   (1000)        0 2023-07-17 15:27:22.138270 SLAMBUC-0.2.0/slambuc/misc/
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)      574 2023-07-03 16:04:48.000000 SLAMBUC-0.2.0/slambuc/misc/__init__.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     3963 2023-07-17 07:11:05.000000 SLAMBUC-0.2.0/slambuc/misc/generator.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)     6655 2023-07-17 07:18:15.000000 SLAMBUC-0.2.0/slambuc/misc/plot.py
+-rw-rw-r--   0 czentye   (1000) czentye   (1000)    28204 2023-07-17 14:17:13.000000 SLAMBUC-0.2.0/slambuc/misc/util.py
```

### Comparing `SLAMBUC-0.1.0/LICENSE` & `SLAMBUC-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/PKG-INFO` & `SLAMBUC-0.2.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,14 @@
-Metadata-Version: 2.1
-Name: SLAMBUC
-Version: 0.1.0
-Summary: Serverless Layout Adaptation with Memory-Bounds and User Constraints
-Author: Janos Czentye
-Author-email: Janos Czentye <czentye@tmit.bme.hu>
-License: Apache 2.0
-Project-URL: Repository, https://github.com/hsnlab/SLAMBUC
-Project-URL: Homepage, https://github.com/hsnlab/SLAMBUC/wiki
-Project-URL: Issue Tracker, https://github.com/hsnlab/SLAMBUC/issues
-Keywords: cloud,serverless,ilp,dp,tree
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: validation
-License-File: LICENSE
-
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
 ![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
 ![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
+![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
+
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -91,15 +69,15 @@
 python3.11 -m pip install pygraphviz
 ```
 
 External solvers can also be used in LP-based algorithms that require the given solver packages to be
 preinstalled and available for the [PuLP frontend](https://github.com/coin-or/pulp). Currently,
 the following solvers are tested.
 
-* CBC (default)
+* CBC (default, packaged with PuLP)
 * GLPK (see installation [here](https://coin-or.github.io/pulp/main/installing_pulp_at_home.html#linux-installation))
 * CPLEX ([installation](https://www.ibm.com/products/ilog-cplex-optimization-studio)
   and [setup](https://coin-or.github.io/pulp/guides/how_to_configure_solvers.html#cplex))
 
 It is worth noting that CPLEX's python wrapper [docplex](https://pypi.org/project/docplex/)
 (as a replacement for PuLP) is left behind the latest Python version. For using this API, requirements
 are prepared separately for **Python3.10**.
@@ -179,61 +157,38 @@
 Execution results:
 
 | Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
 |----------------------|-----------------------------------------------------|--------|-----------|------------|
 | GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
 | GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
 | GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| GREEDY_ILP_0         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0947832  |
-| GREEDY_ILP_1         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0947832  |
-| GREEDY_ILP_2         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0947832  |
-| GREEDY_PAR_0         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0405943  |
-| GREEDY_PAR_1         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0405943  |
-| GREEDY_PAR_2         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0405943  |
-| GREEDY_ILP_PAR_0     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.101437   |
-| GREEDY_ILP_PAR_1     | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.101437   |
-| GREEDY_ILP_PAR_2     | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.101437   |
 | ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_CFG_GREEDY       | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.017507   |
-| ILP_CFG_HYBRID_PAR   | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0126527  |
-| ILP_CFG_GREEDY_PAR   | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0145207  |
-| ILP_HYBRID_CPLEX_CMD | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0133516  |
 | ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| ILP_MTX_PAR          | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0200093  |
 | PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_B_MP          | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00764985 |
-| PSEUDO_B_PAR         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00122202 |
 | PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| PSEUDO_L_MP          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0073112  |
-| PSEUDO_L_PAR         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00087904 |
-| PSEUDO_L_PAR_MP      | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00585536 |
-| BIHEUR_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00065136 |
 | BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BIFPTAS_L_DUAL       | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00079769 |
-| CHAIN_DECOMP         | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.00010146 |
-| TREE_CLUSTER         | [[1, 2, 3], [4], [5], [6, 7, 8, 9, 10]]             |    888 |       455 | 0.00152091 |
-| MINW_UNBOUDED        | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00016116 |
-| MINW_HEUR            | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00030477 |
-| CSP                  | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.0173627  |
 | BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
 | BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
 
-Tests are conducted on Ubuntu 5.15.0-69-generic with AMD EPYC-Rome Processor @ 2.35GHz.
-
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
 python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
-# Remove editing-mode package outside of repo root
-python3.11 -m pip uninstall slambuc 
+# OR
+cd SLAMBUC && make install-req && make dev-install
+
+## Remove editing-mode package outside of repo root
+python3.11 -m pip uninstall slambuc
+# OR
+make uninstall
 ```
 
 ## Publications
 
 If you use one of our algorithms published in this package or our test harness, please consider citing 
 one of our related works.
 
@@ -297,8 +252,8 @@
     pages = {1--7},
     doi = {10.1109/GLOBECOM38437.2019.9013988}
 }
 ```
 
 ## License
 
-SLAMBUC is an open-source software licensed under [Apache 2.0](LICENSE).
+SLAMBUC is an open-source software licensed under [Apache 2.0](LICENSE).
```

### Comparing `SLAMBUC-0.1.0/README.md` & `SLAMBUC-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,39 @@
+Metadata-Version: 2.1
+Name: SLAMBUC
+Version: 0.2.0
+Summary: Serverless Layout Adaptation with Memory-Bounds and User Constraints
+Author: Janos Czentye
+Author-email: Janos Czentye <czentye@tmit.bme.hu>
+License: Apache 2.0
+Project-URL: Repository, https://github.com/hsnlab/SLAMBUC
+Project-URL: Homepage, https://github.com/hsnlab/SLAMBUC/wiki
+Project-URL: Issue Tracker, https://github.com/hsnlab/SLAMBUC/issues
+Keywords: cloud,serverless,ilp,dp,tree
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: tests
+Provides-Extra: validation
+Provides-Extra: doc
+License-File: LICENSE
+
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
 ![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
 ![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
+![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
+
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -67,15 +94,15 @@
 python3.11 -m pip install pygraphviz
 ```
 
 External solvers can also be used in LP-based algorithms that require the given solver packages to be
 preinstalled and available for the [PuLP frontend](https://github.com/coin-or/pulp). Currently,
 the following solvers are tested.
 
-* CBC (default)
+* CBC (default, packaged with PuLP)
 * GLPK (see installation [here](https://coin-or.github.io/pulp/main/installing_pulp_at_home.html#linux-installation))
 * CPLEX ([installation](https://www.ibm.com/products/ilog-cplex-optimization-studio)
   and [setup](https://coin-or.github.io/pulp/guides/how_to_configure_solvers.html#cplex))
 
 It is worth noting that CPLEX's python wrapper [docplex](https://pypi.org/project/docplex/)
 (as a replacement for PuLP) is left behind the latest Python version. For using this API, requirements
 are prepared separately for **Python3.10**.
@@ -155,61 +182,38 @@
 Execution results:
 
 | Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
 |----------------------|-----------------------------------------------------|--------|-----------|------------|
 | GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
 | GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
 | GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| GREEDY_ILP_0         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0947832  |
-| GREEDY_ILP_1         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0947832  |
-| GREEDY_ILP_2         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0947832  |
-| GREEDY_PAR_0         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0405943  |
-| GREEDY_PAR_1         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0405943  |
-| GREEDY_PAR_2         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0405943  |
-| GREEDY_ILP_PAR_0     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.101437   |
-| GREEDY_ILP_PAR_1     | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.101437   |
-| GREEDY_ILP_PAR_2     | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.101437   |
 | ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_CFG_GREEDY       | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.017507   |
-| ILP_CFG_HYBRID_PAR   | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0126527  |
-| ILP_CFG_GREEDY_PAR   | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0145207  |
-| ILP_HYBRID_CPLEX_CMD | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0133516  |
 | ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| ILP_MTX_PAR          | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0200093  |
 | PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_B_MP          | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00764985 |
-| PSEUDO_B_PAR         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00122202 |
 | PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| PSEUDO_L_MP          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0073112  |
-| PSEUDO_L_PAR         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00087904 |
-| PSEUDO_L_PAR_MP      | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00585536 |
-| BIHEUR_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00065136 |
 | BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BIFPTAS_L_DUAL       | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00079769 |
-| CHAIN_DECOMP         | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.00010146 |
-| TREE_CLUSTER         | [[1, 2, 3], [4], [5], [6, 7, 8, 9, 10]]             |    888 |       455 | 0.00152091 |
-| MINW_UNBOUDED        | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00016116 |
-| MINW_HEUR            | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00030477 |
-| CSP                  | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.0173627  |
 | BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
 | BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
 
-Tests are conducted on Ubuntu 5.15.0-69-generic with AMD EPYC-Rome Processor @ 2.35GHz.
-
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
 python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
-# Remove editing-mode package outside of repo root
-python3.11 -m pip uninstall slambuc 
+# OR
+cd SLAMBUC && make install-req && make dev-install
+
+## Remove editing-mode package outside of repo root
+python3.11 -m pip uninstall slambuc
+# OR
+make uninstall
 ```
 
 ## Publications
 
 If you use one of our algorithms published in this package or our test harness, please consider citing 
 one of our related works.
 
@@ -273,8 +277,8 @@
     pages = {1--7},
     doi = {10.1109/GLOBECOM38437.2019.9013988}
 }
 ```
 
 ## License
 
-SLAMBUC is an open-source software licensed under [Apache 2.0](LICENSE).
+SLAMBUC is an open-source software licensed under [Apache 2.0](LICENSE).
```

### Comparing `SLAMBUC-0.1.0/SLAMBUC.egg-info/PKG-INFO` & `SLAMBUC-0.2.0/SLAMBUC.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SLAMBUC
-Version: 0.1.0
+Version: 0.2.0
 Summary: Serverless Layout Adaptation with Memory-Bounds and User Constraints
 Author: Janos Czentye
 Author-email: Janos Czentye <czentye@tmit.bme.hu>
 License: Apache 2.0
 Project-URL: Repository, https://github.com/hsnlab/SLAMBUC
 Project-URL: Homepage, https://github.com/hsnlab/SLAMBUC/wiki
 Project-URL: Issue Tracker, https://github.com/hsnlab/SLAMBUC/issues
@@ -16,21 +16,24 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 Provides-Extra: validation
+Provides-Extra: doc
 License-File: LICENSE
 
 # Serverless Layout Adaptation with Memory-Bounds and User Constraints (SLAMBUC)
 
 ![PyPI](https://img.shields.io/pypi/v/SLAMBUC)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/SLAMBUC)
 ![PyPI - License](https://img.shields.io/pypi/l/SLAMBUC)
+![Algorithm tests](https://github.com/hsnlab/SLAMBUC/actions/workflows/python-alg-tests.yml/badge.svg?branch=main)
+
 
 Collection of graph partitioning algorithms implemented in Python for composing cloud-native
 applications from standalone serverless functions in a cost-efficient and latency-constrained manner.
 
 ## Overview
 
 In the context of serverless computing, function fusion is a novel, high-level approach to improve
@@ -91,15 +94,15 @@
 python3.11 -m pip install pygraphviz
 ```
 
 External solvers can also be used in LP-based algorithms that require the given solver packages to be
 preinstalled and available for the [PuLP frontend](https://github.com/coin-or/pulp). Currently,
 the following solvers are tested.
 
-* CBC (default)
+* CBC (default, packaged with PuLP)
 * GLPK (see installation [here](https://coin-or.github.io/pulp/main/installing_pulp_at_home.html#linux-installation))
 * CPLEX ([installation](https://www.ibm.com/products/ilog-cplex-optimization-studio)
   and [setup](https://coin-or.github.io/pulp/guides/how_to_configure_solvers.html#cplex))
 
 It is worth noting that CPLEX's python wrapper [docplex](https://pypi.org/project/docplex/)
 (as a replacement for PuLP) is left behind the latest Python version. For using this API, requirements
 are prepared separately for **Python3.10**.
@@ -179,61 +182,38 @@
 Execution results:
 
 | Algorithm            | Partitioning                                        |   Cost |   Latency |   Time (s) |
 |----------------------|-----------------------------------------------------|--------|-----------|------------|
 | GREEDY_0             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0235749  |
 | GREEDY_1             | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0235749  |
 | GREEDY_2             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0235749  |
-| GREEDY_ILP_0         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0947832  |
-| GREEDY_ILP_1         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0947832  |
-| GREEDY_ILP_2         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0947832  |
-| GREEDY_PAR_0         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0405943  |
-| GREEDY_PAR_1         | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0405943  |
-| GREEDY_PAR_2         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0405943  |
-| GREEDY_ILP_PAR_0     | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.101437   |
-| GREEDY_ILP_PAR_1     | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.101437   |
-| GREEDY_ILP_PAR_2     | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.101437   |
 | ILP_CFG_HYBRID       | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0167496  |
-| ILP_CFG_GREEDY       | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.017507   |
-| ILP_CFG_HYBRID_PAR   | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0126527  |
-| ILP_CFG_GREEDY_PAR   | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.0145207  |
-| ILP_HYBRID_CPLEX_CMD | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0133516  |
 | ILP_MTX              | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0197985  |
-| ILP_MTX_PAR          | [[1, 3, 4, 5], [2], [6, 8, 9, 10], [7]]             |    858 |       474 | 0.0200093  |
 | PSEUDO_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00047041 |
-| PSEUDO_B_MP          | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00764985 |
-| PSEUDO_B_PAR         | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00122202 |
 | PSEUDO_L             | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00083811 |
-| PSEUDO_L_MP          | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.0073112  |
-| PSEUDO_L_PAR         | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00087904 |
-| PSEUDO_L_PAR_MP      | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00585536 |
-| BIHEUR_B             | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00065136 |
 | BIFPTAS_L            | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00082326 |
-| BIFPTAS_L_DUAL       | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00079769 |
-| CHAIN_DECOMP         | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.00010146 |
-| TREE_CLUSTER         | [[1, 2, 3], [4], [5], [6, 7, 8, 9, 10]]             |    888 |       455 | 0.00152091 |
-| MINW_UNBOUDED        | [[1, 3, 4, 5], [2], [6, 7, 8, 9], [10]]             |    858 |       471 | 0.00016116 |
-| MINW_HEUR            | [[1, 2, 3], [4, 5, 6, 8, 9, 10], [7]]               |    858 |       443 | 0.00030477 |
-| CSP                  | [[1, 3, 4, 5], [2], [6, 9], [7], [8, 10]]           |    882 |       433 | 0.0173627  |
 | BASELINE_NO_PART     | [[1], [2], [3], [4], [5], [6], [7], [8], [9], [10]] |   1090 |       472 | 9.38e-05   |
 | BASELINE_SINGLE      | [[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]]                   |    822 |       686 | 6.718e-05  |
 
-Tests are conducted on Ubuntu 5.15.0-69-generic with AMD EPYC-Rome Processor @ 2.35GHz.
-
 ## Development and contribution
 
 If you would like to contribute, add a feature, or just play with the implementations, the development
 environment can be set up with the following commands.
 
 ```bash
 git clone https://github.com/hsnlab/SLAMBUC.git
 python3.11 -m pip install -U -r SLAMBUC/requirements.txt
 python3.11 -m pip install --ignore-requires-python --no-deps -e SLAMBUC/
-# Remove editing-mode package outside of repo root
-python3.11 -m pip uninstall slambuc 
+# OR
+cd SLAMBUC && make install-req && make dev-install
+
+## Remove editing-mode package outside of repo root
+python3.11 -m pip uninstall slambuc
+# OR
+make uninstall
 ```
 
 ## Publications
 
 If you use one of our algorithms published in this package or our test harness, please consider citing 
 one of our related works.
```

### Comparing `SLAMBUC-0.1.0/SLAMBUC.egg-info/SOURCES.txt` & `SLAMBUC-0.2.0/SLAMBUC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/pyproject.toml` & `SLAMBUC-0.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -44,16 +44,17 @@
     'tabulate~=0.9.0'
 ]
 validation = [
     'tabulate~=0.9.0',
     'Click~=8.1.3',
     'psutil~=5.9.4'
 ]
-
-
+doc = [
+    'pydoc-markdown~=4.8.2'
+]
 
 [tool.setuptools.packages.find]
 exclude = [
     "tests",
     "tests.*",
     "validation",
     "validation.*"
@@ -62,8 +63,20 @@
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.package-data]
 "*" = [
     '*.pkl',
     '*.csv'
-]
+]
+
+[[tool.pydoc-markdown.loaders]]
+type = "python"
+search_path = [ "slambuc" ]
+
+[tool.pydoc-markdown.renderer]
+type = "mkdocs"
+
+[[tool.pydoc-markdown.renderer.pages]]
+title = "SLAMBUC API Documentation"
+name = "index"
+contents = [ "slambuc.*" ]
```

### Comparing `SLAMBUC-0.1.0/setup.py` & `SLAMBUC-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/__init__.py` & `SLAMBUC-0.2.0/slambuc/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-__version__ = "0.1.0"
+__version__ = "0.2.0"
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/ser/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,17 +7,9 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# Constants for attribute indices in DP matrix
-import math
-
-BARR, COST, LAT = 0, 1, 2
-# Constant for block cache index
-MEM, CPU = 0, 3
-# Constant for ILP model names
-LP_LAT = 'C_LAT'
-# Values of infeasible solution [partitioning, opt_cost, opt_lat]
-INFEASIBLE = ([], math.inf, None)
+from .greedy import greedy_ser_chain_partitioning
+from .ilp import chain_cfg_partitioning, chain_mtx_partitioning
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/dp/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/dp/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/dp/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/dp/greedy.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,53 +9,63 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS, T_PART_GEN
 from slambuc.alg.util import ipowerset, split_chain, block_memory, block_cost, block_latency, block_cpu
 
 
-def ichain_blocks(memory: list[int], M: int, rate: list[int], N: int) -> list[list[list[int]]]:
+def ichain_blocks(memory: list[int], rate: list[int], N: int, M: int) -> T_PART_GEN:
     """
-    Calculates all combination of chain cuts with respect to the *memory* values and constraint *M*.
-    The calculation is improved compared to brute force to only start calculating cuts from c_min.
+    Calculates all combination of chain cuts with respect to *memory* and *rate* values and the constraint **M**.
+
+    The calculation is improved compared to brute force to only start calculating cuts from minimal cut size *c_min*.
+
+    :param memory:  list of node memory values
+    :param rate:    list of invocation rate values
+    :param N:       number of vCPU cores
+    :param M:       upper memory limit
+    :return:        Generator over M-feasible cuts.
     """
     n = len(memory)
     for cut in ipowerset(range(1, n), start=math.ceil(sum(memory) / M) - 1):
         barr = sorted({0}.union(cut))
         # Consider only block with appropriate size
         valid = [blk for blk in split_chain(barr, n)
                  if block_memory(memory, blk[0], blk[-1]) <= M and block_cpu(rate, blk[0], blk[-1]) <= N]
         if len(valid) == len(barr):
             yield valid
 
 
-def greedy_chain_partitioning(runtime: list, memory: list, rate: list, M: int = math.inf, N: int = math.inf,
-                              L: int = math.inf, start: int = 0, end: int = None, delay: int = 1,
-                              unit: int = 100) -> list[tuple[list[int], int, int]]:
+def greedy_chain_partitioning(runtime: list[int], memory: list[int], rate: list[int], M: int = math.inf,
+                              N: int = math.inf, L: int = math.inf, start: int = 0, end: int = None, 
+                              delay: int = 1, unit: int = 100) -> list[T_RESULTS]:
     """
-    Calculates the minimal-cost partitioning of a given chain by exhaustive search
+    Calculates all minimal-cost partitioning outcomes of a given chain by applying exhaustive search.
+
+    Parameters are the same as the partitioning algorithms in ``slambuc.alg.chain.dp.mtx``
+    and ``slambuc.alg.chain.dp.min``.
 
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
     :param delay:   invocation delay between blocks
     :param start:   head node of the latency-limited subchain
     :param end:     tail node of the latency-limited subchain
     :param unit:    rounding unit for the cost calculation (default: 100 ms)
     :return:        list if min-cost partitions, related optimal cost and latency
     """
     best_res, best_cost = [INFEASIBLE], math.inf
-    for partition in ichain_blocks(memory, M, rate, N):
+    for partition in ichain_blocks(memory, rate, N, M):
         if (sum_lat := sum(block_latency(runtime, blk[0], blk[-1], delay, start, end) for blk in partition)) > L:
             continue
         elif (sum_cost := sum(block_cost(runtime, rate, blk[0], blk[-1], unit) for blk in partition)) == best_cost:
             best_res.append((partition, sum_cost, sum_lat))
         elif sum_cost < best_cost:
             best_res, best_cost = [(partition, sum_cost, sum_lat)], sum_cost
     return best_res
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/dp/min.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/dp/min.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,27 +10,33 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import math
 
-from slambuc.alg import MEM, COST, LAT, CPU
+from slambuc.alg import MEM, COST, LAT, CPU, T_BARRS, T_BRESULTS
 from slambuc.alg.chain.dp.mtx import State
 
 
-def min_chain_partitioning(runtime: list, memory: list, rate: list, M: int = math.inf, N: int = math.inf,
-                           L: int = math.inf, start: int = 0, end: int = None, delay: int = 1,
-                           unit: int = 100) -> tuple[list, int, int]:
+def min_chain_partitioning(runtime: list[int], memory: list[int], rate: list[int], M: int = math.inf,
+                           N: int = math.inf, L: int = math.inf, start: int = 0, end: int = None,
+                           delay: int = 1, unit: int = 100) -> T_BRESULTS:
     """
     Calculates minimal-cost partitioning of a chain based on the node properties of *running time*, *memory usage* and
     *invocation rate* with respect to an upper bound **M** on the total memory of blocks and a latency constraint **L**
     defined on the subchain between *start* and *end* nodes.
 
-    It can be only used when the cost function regarding the chain attributes is sub-additive, that is k_opt = k_min.
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
+
+    It gives optimal result only in case the cost function regarding the chain attributes is sub-additive,
+    that is k_opt = k_min is guaranteed for each case.
+
+    Instead of full partitioning it only returns the list of barrier nodes.
 
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
@@ -40,31 +46,31 @@
     :param unit:    rounding unit for the cost calculation (default: 100 ms)
     :return:        tuple of barrier nodes, sum cost of the partitioning, and the calculated latency on the subchain
     """
     n = len(runtime)
     end = end if end is not None else n - 1
 
     def block_memory(_v: int, cumsum: list = (0,)) -> int:
-        """Calculate memory of a block from the cached cumulative sum of block[v+1, w] or block[b, v-1]"""
+        """Calculate memory of a block from the cached cumulative sum of block[v+1, w] or block[b, v-1]."""
         cumsum[MEM] += memory[_v]
         return cumsum[MEM]
 
     def block_cpu(_b: int, cumsum: list = (0, 0, 0, (0, 1))) -> int:
-        """Calculate CPU need of a block from the cached cumulative sum of block[b+1, w]"""
+        """Calculate CPU need of a block from the cached cumulative sum of block[b+1, w]."""
         cumsum[CPU][0] = max(cumsum[CPU][0], rate[_b])
         cumsum[CPU][1] = max(cumsum[CPU][1], math.ceil(cumsum[CPU][0] / rate[_b]))
         return cumsum[CPU][1]
 
     def block_cost(_b: int, cumsum: list = (0, 0)) -> int:
-        """Calculate running time of block[b, w] from the cached cumulative sum of block[b+1, w]"""
+        """Calculate running time of block[b, w] from the cached cumulative sum of block[b+1, w]."""
         cumsum[COST] += runtime[_b]
         return rate[_b] * (math.ceil(cumsum[COST] / unit) * unit)
 
     def block_latency(_b: int, _w: int, cumsum: list = (0, 0, 0)) -> int:
-        """Calculate relevant latency for block[b, w] from the cached cumulative sum of block[b+1, w]"""
+        """Calculate relevant latency for block[b, w] from the cached cumulative sum of block[b+1, w]."""
         # Do not consider latency if no intersection
         if end < _b or _w < start:
             return 0
         if b < start:
             return cumsum[LAT]
         cumsum[LAT] += runtime[_b]
         # Ignore delay if latency path starts within the subchain
@@ -98,14 +104,19 @@
             if (lat := DP[b - 1].lat + block_latency(b, w, _cache)) <= L:
                 # Store and overwrite subcases with equal costs (<=) to consider larger blocks for lower latency
                 if (cost := DP[b - 1].cost + block_cost(b, _cache)) <= DP[w].cost:
                     DP[w] = State(b, cost, lat)
     return (extract_min_barr(DP), DP[n - 1].cost, DP[n - 1].lat) if DP[n - 1].cost < math.inf else DP[n - 1]
 
 
-def extract_min_barr(DP: list[State]) -> list[int]:
-    """Extract barrier nodes form DP matrix by iteratively backtracking the minimal cost subcases"""
+def extract_min_barr(DP: list[State]) -> T_BARRS:
+    """
+    Extract barrier nodes form DP list by iteratively backtracking minimal cost subcases.
+
+    :param DP:  dynamic programming structure storing intermediate *States*
+    :return:    list of barrier nodes
+    """
     barr = [DP[-2].barr]
     while barr[-1]:
         barr.append(DP[barr[-1] - 1].barr)
     barr.reverse()
     return barr
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/dp/mtx.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/dp/mtx.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,46 +14,53 @@
 import functools
 import itertools
 import math
 import typing
 
 import numpy as np
 
-from slambuc.alg import MEM, CPU, COST, LAT, BARR
+from slambuc.alg import INFEASIBLE, T_BARRS, MEM, CPU, COST, LAT, BARR
 
 
 class State(typing.NamedTuple):
-    """Store block attributes for a given subcase"""
+    """Store block attributes for a given DP subcase."""
     barr: int = None  # Barrier/heading node of the last block in the given subcase partitioning
     cost: int = math.inf  # Sum cost of the partitioning
     lat: int = math.inf  # Sum latency of the partitioning regarding the limited subchain[start, end]
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def chain_partitioning(runtime: list, memory: list, rate: list, M: int = math.inf, N: int = math.inf,
                        L: int = math.inf, start: int = 0, end: int = None, delay: int = 1,
-                       unit: int = 100, ret_dp: bool = False) -> tuple[list, int, int]:
+                       unit: int = 100, ret_dp: bool = False) -> tuple[T_BARRS | list[list[State]], int, int]:
     """
     Calculates minimal-cost partitioning of a chain based on the node properties of *running time*, *memory usage* and
     *invocation rate* with respect to an upper bound **M** on the total memory of blocks and a latency constraint **L**
     defined on the subchain between *start* and *end* nodes.
 
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
+
+    Details in: J. Czentye, I. Pelle and B. Sonkoly, "Cost-optimal Operation of Latency Constrained Serverless
+    Applications: From Theory to Practice," NOMS 2023-2023 IEEE/IFIP Network Operations and Management Symposium,
+    Miami, FL, USA, 2023, pp. 1-10, doi: 10.1109/NOMS56928.2023.10154412.
+
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
     :param delay:   invocation delay between blocks
     :param start:   head node of the latency-limited subchain
     :param end:     tail node of the latency-limited subchain
     :param unit:    rounding unit for the cost calculation (default: 100 ms)
-    :param ret_dp:  return the calculated DP matrix instead of the barrier nodes
+    :param ret_dp:  return the calculated DP matrix instead of barrier nodes
     :return:        tuple of barrier nodes, sum cost of the partitioning, and the calculated latency on the subchain
     """
     n = len(runtime)
     end = end if end is not None else n - 1
 
     @functools.lru_cache(maxsize=n - 1)
     def block_memory(_b: int, _w: int) -> int:
@@ -78,22 +85,22 @@
         if end < _b or _w < start:
             return 0
         blk_lat = sum(runtime[max(_b, start): min(_w, end) + 1])
         # Ignore delay if latency path starts within the subchain
         return delay + blk_lat if start < _b else blk_lat
 
     # Check lower bound for latency limit
-    if L < (lat_min := sum(runtime[start: end + 1])):
-        return None, None, lat_min
+    if L < sum(runtime[start: end + 1]):
+        return INFEASIBLE
     # Check if memory constraint allows feasible solutions for the given latency constraint
     k_min = max(math.ceil(sum(memory[start: end + 1]) / M),
                 sum(1 for i, j in itertools.pairwise(rate) if math.ceil(j / i) > N))
     k_max = math.floor(min((L - sum(runtime[start: end + 1])) / delay + 1, n))
     if k_max < k_min:
-        return None, None, None
+        return INFEASIBLE
     # Check single node partitioning
     if len(runtime) == 1:
         return [0], block_cost(0, 0), block_latency(0, 0)
     # Initialize left triangular part of DP matrix -> DP[i][j][COST, LAT, BARR]
     DP = [[State() for _ in range(i + 1)] for i in range(n)]
     # Initialize default values for grouping first w nodes into one group
     for w in range(0, n):
@@ -116,19 +123,25 @@
                 break
     # Index of optimal cost partition, the fist one if multiple min values exist
     k_opt = min(range(n), key=lambda x: DP[-1][x].cost)
     _, opt_cost, opt_lat = DP[-1][k_opt]
     if opt_cost < math.inf:
         return DP if ret_dp else extract_barr(DP, k_opt), opt_cost, opt_lat
     else:
-        return None, math.inf, None
+        return INFEASIBLE
 
 
-def extract_barr(DP: list[list[State]], k: int) -> list[int]:
-    """Extract barrier nodes form DP matrix by iteratively backtracking the minimal cost subcases from *k*"""
+def extract_barr(DP: list[list[State]], k: int) -> T_BARRS:
+    """
+    Extract barrier nodes form DP matrix by iteratively backtracking the minimal cost subcases started from *k*.
+
+    :param DP:  DP matrix containing subcase *States*
+    :param k:   number of optimal cuts
+    :return:    list of barrier nodes
+    """
     barr = []
     w = len(DP) - 1
     for k in reversed(range(0, k + 1)):
         # The cached b value marks the barrier node of the k. block and refers the subcase => C[b-1,k-1] + c[b,w]
         b = DP[w][k].barr
         w = b - 1
         barr.append(b)
@@ -137,20 +150,27 @@
 
 
 ########################################################################################################################
 
 
 def vec_chain_partitioning(runtime: list, memory: list, rate: list, M: int = np.inf, N: int = np.inf, L: int = np.inf,
                            start: int = 0, end: int = None, delay: int = 1, unit: int = 100,
-                           ret_dp: bool = False) -> tuple[list, int, int]:
+                           ret_dp: bool = False) -> tuple[T_BARRS | np.ndarray, int, int]:
     """
     Calculates minimal-cost partitioning of a chain based on the node properties of *runtime*, *memory* and *rate* with
     respect to an upper bound **M** on the total memory of blocks and a latency constraint **L** defined on the subchain
     between *start* and *end* nodes leveraging vectorized operations.
 
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
+
+    Details in: J. Czentye, I. Pelle and B. Sonkoly, "Cost-optimal Operation of Latency Constrained Serverless
+    Applications: From Theory to Practice," NOMS 2023-2023 IEEE/IFIP Network Operations and Management Symposium,
+    Miami, FL, USA, 2023, pp. 1-10, doi: 10.1109/NOMS56928.2023.10154412.
+
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
     :param delay:   invocation delay between blocks
@@ -196,22 +216,22 @@
             if b < start:
                 return cumsum[LAT]
             cumsum[LAT] += runtime[_b]
         # Ignore delay if latency path starts within the subchain
         return delay + cumsum[LAT] if start < _b else cumsum[LAT]
 
     # Check lower bound for latency limit
-    if L < (lat_min := sum(runtime[start: end + 1])):
-        return None, None, lat_min
+    if L < sum(runtime[start: end + 1]):
+        return INFEASIBLE
     # Check if memory constraint allows feasible solutions for the given latency constraint
     k_min = max(math.ceil(sum(memory[start: end + 1]) / M),
                 sum(1 for i, j in itertools.pairwise(rate) if math.ceil(j / i) > N))
     k_max = math.floor(min((L - sum(runtime[start: end + 1])) / delay + 1, n))
     if k_max < k_min:
-        return None, None, None
+        return INFEASIBLE
     # Check single node partitioning
     if len(runtime) == 1:
         return [0], block_cost(0), block_latency(0, 0)
     # Initialize DP matrix -> DP[i][j][BARR, COST, LAT]
     DP = np.full((n, n, 3), np.inf)
     # Define cache for cumulative block attribute calculations: [MEM, COST, LAT]
     __cache = [0, 0, 0, [0, 0]]
@@ -235,19 +255,25 @@
             DP[w, feasible_idx + 1] = subcases[feasible_idx]
     # Index of optimal cost partition, the fist one if multiple min values exist
     k_opt = np.argmin(DP[n - 1, :, COST])
     _, opt_cost, opt_lat = DP[n - 1, k_opt]
     if opt_cost < np.inf:
         return DP if ret_dp else extract_vec_barr(DP, k_opt), opt_cost, opt_lat
     else:
-        return None, np.inf, None
+        return INFEASIBLE
 
 
-def extract_vec_barr(DP: np.array, k: int) -> list[int]:
-    """Extract barrier nodes form DP matrix by iteratively backtracking the minimal cost subcases from *k*"""
+def extract_vec_barr(DP: np.ndarray, k: int) -> T_BARRS:
+    """
+    Extract barrier nodes from vectorized DP matrix by iteratively backtracking the minimal cost subcases from *k*.
+
+    :param DP:  DP matrix containing subcase *States*
+    :param k:   number of optimal cuts
+    :return:    list of barrier nodes
+    """
     barr = []
     B = DP[..., BARR]
     w = len(B) - 1
     for k in reversed(range(0, k + 1)):
         # The cached b value marks the barrier node of the k. block and refers the subcase => C[b-1,k-1] + c[b,w]
         b = int(B[w, k])
         w = b - 1
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/ser/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/layout/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,9 +7,8 @@
 # http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-from .greedy import greedy_ser_chain_partitioning
-from .ilp import chain_cfg_partitioning, chain_mtx_partitioning
+from .ilp import tree_gen_hybrid_partitioning, tree_gen_mtx_partitioning, all_gen_tree_mtx_partitioning
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/ser/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/ser/greedy.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,37 +9,48 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_PART_GEN, T_RESULTS
 from slambuc.alg.util import ipowerset, split_chain, ser_block_submemory, ser_block_sublatency, ser_block_subcost
 
 
-def ichain_blocks(memory: list[int], M: int) -> list[list[list[int]]]:
+def ichain_blocks(memory: list[int], M: int) -> T_PART_GEN:
     """
-    Calculates all combination of chain cuts with respect to the *memory* values and constraint *M*.
-    The calculation is improved compared to brute force to only start calculating cuts from c_min.
+    Calculates all combinations of chain cuts with respect to the *memory* values and constraint *M*.
+
+    Block memories are calculated assuming serialized platform execution model.
+
+    The calculation is improved compared to brute force to only start calculating cuts from minimal cut size *c_min*.
+
+    :param memory:  list of node memory values
+    :param M:       upper memory limit
+    :return:        Generator over M-feasible cuts.
     """
     n = len(memory)
     for cut in ipowerset(range(1, n), start=math.ceil(sum(memory) / M) - 1):
         barr = sorted({0}.union(cut))
         # Consider only block with appropriate size
         valid = [blk for blk in split_chain(barr, n) if ser_block_submemory(memory, blk[0], blk[-1]) <= M]
         if len(valid) == len(barr):
             yield valid
 
 
-def greedy_ser_chain_partitioning(runtime: list, memory: list, rate: list, data: list, M: int = math.inf,
-                                  L: int = math.inf, start: int = 0, end: int = None,
-                                  delay: int = 1) -> list[tuple[list[int], int, int]]:
+def greedy_ser_chain_partitioning(runtime: list[int], memory: list[int], rate: list[int], data: list[int],
+                                  M: int = math.inf, L: int = math.inf, start: int = 0, end: int = None,
+                                  delay: int = 1) -> T_RESULTS:
     """
-    Calculates the minimal-cost partitioning of a given chain by exhaustive search
+    Calculates all minimal-cost partitioning outcomes of a given chain by applying exhaustive search.
+
+    Parameters are the same as the partitioning algorithms in ``slambuc.alg.chain.ser.ilp``.
+
+    Block metrics are calculated assuming serialized platform execution model.
 
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param data:    input data fetching delay in ms
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/chain/ser/ilp.py` & `SLAMBUC-0.2.0/slambuc/alg/chain/ser/ilp.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,34 +12,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import math
 
 import pulp as lp
 
-from slambuc.alg import LP_LAT, INFEASIBLE
+from slambuc.alg import LP_LAT, INFEASIBLE, T_IBLOCK_GEN, T_RESULTS, T_PART
 from slambuc.alg.util import (ser_block_sublatency, split_chain, ser_block_subcost, ser_block_submemory,
                               iser_mul_factor)
 
 
-def ifeasible_greedy_blocks(memory: list[int], M: int) -> list[list[int]]:
+def ifeasible_greedy_blocks(memory: list[int], M: int) -> T_IBLOCK_GEN:
     """
-    Generate all feasible (connected) blocks that meet the memory constraint *M*.
+    Generate all feasible (connected) blocks that meet the memory constraint *M* in a greedy manner.
+
+    Block memories are calculated assuming serialized platform execution model.
 
     :param memory:  list of node memory values
     :param M:       upper block memory limit
     :return:        generator of blocks
     """
     n = len(memory)
     yield from ((i, j) for i in range(n) for j in range(i, n) if ser_block_submemory(memory, i, j) <= M)
 
 
-def ifeasible_blocks(memory: list[int], M: int) -> list[list[int]]:
+def ifeasible_blocks(memory: list[int], M: int) -> T_IBLOCK_GEN:
     """
-    Generate all feasible (connected) blocks that meet the memory constraint *M*.
+    Generate all feasible (connected) blocks that meet the memory constraint *M* assuming serialized executions.
 
     :param memory:  list of node memory values
     :param M:       upper block memory limit
     :return:        generator of blocks
     """
     n = len(memory)
     for i in range(n):
@@ -47,19 +49,23 @@
         for j in range(i, n):
             if (cumsum := cumsum + memory[j]) > M:
                 break
             else:
                 yield i, j
 
 
-def build_chain_cfg_model(runtime: list, memory: list, rate: list, data: list, M: int = math.inf, L: int = math.inf,
-                          start: int = 0, end: int = None, delay: int = 1) -> tuple[lp.LpProblem, dict[lp.LpVariable]]:
+def build_chain_cfg_model(runtime: list[int], memory: list[int], rate: list[int], data: list[int],
+                          M: int = math.inf, L: int = math.inf, start: int = 0, end: int = None,
+                          delay: int = 1) -> tuple[lp.LpProblem, dict[lp.LpVariable]]:
     """
-    Generate the ILP model.
-    :return: tuple of the created model and list of decision variables
+    Generate the configuration ILP model for chains.
+
+    Block metrics are calculated assuming serialized platform execution model.
+
+    :return: tuple of the created LP model and the dict of created decision variables
     """
     # Model
     model = lp.LpProblem(name="Chain_Partitioning", sense=lp.LpMinimize)
     # Decision variables
     X = {(b, w): lp.LpVariable(f'x_{b}_{w}', cat=lp.LpBinary) for b, w in ifeasible_blocks(memory, M)}
     # Objective
     model += lp.lpSum(ser_block_subcost(runtime, rate, data, b, w) * X[b, w] for b, w in X)
@@ -72,19 +78,21 @@
         model += sum_lat <= L, LP_LAT
     else:
         # Add redundant constraint to implicitly calculate the latency value
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
-def chain_cfg_partitioning(runtime: list, memory: list, rate: list, data: list, M: int = math.inf,
-                           L: int = math.inf, start: int = 0, end: int = None, delay: int = 1,
-                           solver: lp.LpSolver = None) -> tuple[list[list[int]], int, int]:
+def chain_cfg_partitioning(runtime: list[int], memory: list[int], rate: list[int], data: list[int],
+                           M: int = math.inf, L: int = math.inf, start: int = 0, end: int = None,
+                           delay: int = 1, solver: lp.LpSolver = None) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a chain based on configuration LP formulation.
+    Calculates minimal-cost partitioning of a chain based on the configuration ILP formalization.
+
+    Block metrics are calculated assuming serialized platform execution model.
 
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param data:    input data fetching delay in ms
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
@@ -99,32 +107,47 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = lp.value(model.objective), lp.value(model.constraints[LP_LAT])
         return extract_blocks_from_xvars(X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def recreate_blocks_from_xvars(X: dict[tuple[int, int], lp.LpVariable], n: int) -> list[list[int]]:
-    """Extract barrier nodes from variable dict and recreate partitioning blocks"""
+def recreate_blocks_from_xvars(X: dict[tuple[int, int], lp.LpVariable], n: int) -> T_PART:
+    """
+    Extract barrier nodes from variable dict and recreate partitioning blocks.
+
+    :param X:   dict of decision variables
+    :param n:   chain size
+    :return:    partition blocks
+    """
     return split_chain(barr=[b for (b, _), x in X.items() if x.varValue == 1], n=n)
 
 
-def extract_blocks_from_xvars(X: dict[tuple[int, int], lp.LpVariable]) -> list[list[int]]:
-    """Extract interval boundaries [b, w] from variable dict"""
+def extract_blocks_from_xvars(X: dict[tuple[int, int], lp.LpVariable]) -> T_PART:
+    """
+    Extract interval boundaries [b, w] relying on the decision variable's structure.
+
+    :param X:   dict of decision variables
+    :return:    partition blocks
+    """
     return [list(range(b, w + 1)) for (b, w), x in X.items() if x.varValue == 1]
 
 
 ########################################################################################################################
 
 
-def build_greedy_chain_mtx_model(runtime: list, memory: list, rate: list, data: list, M: int = math.inf,
-                                 L: int = math.inf, delay: int = 1) -> tuple[lp.LpProblem, list[list[lp.LpVariable]]]:
+def build_greedy_chain_mtx_model(runtime: list[int], memory: list[int], rate: list[int],
+                                 data: list[int], M: int = math.inf, L: int = math.inf,
+                                 delay: int = 1) -> tuple[lp.LpProblem, list[list[lp.LpVariable]]]:
     """
-    Generate the ILP model.
-    :return: tuple of the created model and list of decision variables
+    Generate the matrix ILP model for chains by calculating block metrics greedily using utility functions.
+
+    Block metrics are calculated assuming serialized platform execution model.
+
+    :return: tuple of the created LP model and the dict of created decision variables
     """
     # Model
     model = lp.LpProblem(name="Chain_Partitioning", sense=lp.LpMinimize)
     n = len(runtime)
     # Decision variable matrix
     X = [[lp.LpVariable(f"x_{i}_{j}", cat=lp.LpBinary) for j in range(i + 1)] for i in range(n)]
     # Objective
@@ -158,18 +181,22 @@
         model += sum_lat <= L, LP_LAT
     else:
         # Add redundant constraint to implicitly calculate the latency value
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
-def build_chain_mtx_model(runtime: list, memory: list, rate: list, data: list, M, L: int = math.inf,
+def build_chain_mtx_model(runtime: list[int], memory: list[int], rate: list[int],
+                          data: list[int], M: int = math.inf, L: int = math.inf,
                           delay: int = 1) -> tuple[lp.LpProblem, list[list[lp.LpVariable]]]:
     """
-    Generate the ILP model.
+    Generate the matrix ILP model for chains.
+
+    Block metrics are calculated assuming serialized platform execution model.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Chain_Partitioning", sense=lp.LpMinimize)
     n = len(runtime)
     # Decision variable matrix
     X = [[lp.LpVariable(f"x_{i}_{j}", cat=lp.LpBinary) for j in range(i + 1)] for i in range(n)]
@@ -213,18 +240,21 @@
         model += sum_lat <= L, LP_LAT
     else:
         # Add redundant constraint to implicitly calculate the latency value
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
-def chain_mtx_partitioning(runtime: list, memory: list, rate: list, data: list, M: int = math.inf, L: int = math.inf,
-                           delay: int = 1, solver: lp.LpSolver = None, **kwargs) -> tuple[list[list[int]], int, int]:
+def chain_mtx_partitioning(runtime: list[int], memory: list[int], rate: list[int], data: list[int],
+                           M: int = math.inf, L: int = math.inf, delay: int = 1, solver: lp.LpSolver = None,
+                           **kwargs) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a chain based on configuration LP formulation.
+    Calculates minimal-cost partitioning of a chain based on the matrix ILP formalization.
+
+    Block metrics are calculated assuming serialized platform execution model.
 
     :param runtime: running times in ms
     :param memory:  memory requirements in MB
     :param rate:    avg. rate of function invocations
     :param data:    input data fetching delay in ms
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path in the form of subchain[start -> end] (in ms)
@@ -237,16 +267,26 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = lp.value(model.objective), lp.value(model.constraints[LP_LAT])
         return recreate_blocks_from_xmatrix(X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def recreate_blocks_from_xmatrix(X: list[list[lp.LpVariable]]) -> list[list[int]]:
-    """Extract barrier nodes from variable matrix and recreate partitioning blocks"""
+def recreate_blocks_from_xmatrix(X: list[list[lp.LpVariable]]) -> T_PART:
+    """
+    Extract barrier nodes from decision variable matrix and recreate partitioning blocks.
+
+    :param X:   matrix of decision variables
+    :return:    partition blocks
+    """
     return split_chain(barr=list(filter(lambda i: X[i][i].value(), range(len(X)))), n=len(X))
 
 
-def extract_blocks_from_xmatrix(X: list[list[lp.LpVariable]]) -> list[list[int]]:
-    """Extract interval boundaries [b, w] from variable matrix"""
+def extract_blocks_from_xmatrix(X: list[list[lp.LpVariable]]) -> T_PART:
+    """
+    Extract interval boundaries [b, w] directly from decision variable matrix.
+
+    :param X:   matrix of decision variables
+    :return:    partition blocks
+    """
     return [list(itertools.takewhile(lambda i: X[i][j].value(), range(j, len(X))))
             for j in range(len(X)) if X[j][j].value()]
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/ext/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/ext/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/ext/baseline.py` & `SLAMBUC-0.2.0/slambuc/alg/ext/baseline.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import networkx as nx
 
+from slambuc.alg import T_RESULTS
 from slambuc.alg.service import PLATFORM
 from slambuc.alg.util import recalculate_partitioning
 
 
 def baseline_singleton_partitioning(tree: nx.DiGraph, root: int = 1, N: int = 1, cp_end: int = None,
-                                    delay: int = 1, **kwargs) -> tuple[list[list[int]], int, int]:
+                                    delay: int = 1, **kwargs) -> T_RESULTS:
     """
     Derive the trivial partitioning of grouping all nodes into one single block.
 
     :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate and data
     :param root:    root node of the graph
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
@@ -30,15 +31,15 @@
     :return:        tuple of partitioning, reached sum cost and latency on the critical path
     """
     partitioning = [sorted(filter(lambda v: v is not PLATFORM, tree))]
     return partitioning, *recalculate_partitioning(tree, partitioning, root, N, cp_end, delay)
 
 
 def baseline_no_partitioning(tree: nx.DiGraph, root: int = 1, N: int = 1, cp_end: int = None,
-                             delay: int = 1, **kwargs) -> tuple[list[list[int]], int, int]:
+                             delay: int = 1, **kwargs) -> T_RESULTS:
     """
     Derive the trivial solution of not merging any of the given tree nodes.
 
     :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate and data
     :param root:    root node of the graph
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/ext/csp.py` & `SLAMBUC-0.2.0/slambuc/alg/ext/csp.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,47 +11,60 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import collections
 import itertools
 import math
 import time
+from collections.abc import Generator, Callable
 
 import cspy
 import networkx as nx
 import numpy as np
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_BLOCK, T_RESULTS, T_PART
 from slambuc.alg.service.common import SEP, ASSIGN, Flavor
 from slambuc.alg.util import (leaf_label_nodes, ibacktrack_chain, iflattened_tree, gen_subtree_memory, gen_subtree_cost,
                               gen_subchain_latency, verify_limits)
 
 # Naming convention for state-space DAG required by *cspy* lib
 START, END = 'Source', 'Sink'
 COST, LAT = 'weight', 'res_cost'
 
 
-def encode_state(grp: list[int], flavor: Flavor) -> str:
-    """Encode DAG node name with flavor's memory as a unique str (hashable)"""
+def encode_state(grp: T_BLOCK, flavor: Flavor) -> str:
+    """
+    Encode DAG node name with flavor's memory as a unique str (hashable).
+
+    :param grp:     partition block
+    :param flavor:  assigned *flavor*
+    :return:        encoded partition block
+    """
     return f"{SEP.join(map(str, grp))}{ASSIGN}{SEP.join(map(str, flavor))}"
 
 
-def decode_state(name: str) -> list[list[int], int]:
-    """Decode DAG node name from encoded str into partition block (list of int) and flavor's memory (mem)"""
+def decode_state(name: str) -> list[T_BLOCK, str]:
+    """
+    Decode DAG node name from encoded str into partition block (list of int) and flavor's memory (mem).
+
+    :param name:    encoded partition block
+    :return:        decoded block and assigned flavor
+    """
     parts = name.rsplit(ASSIGN, maxsplit=1)
     return list(map(int, parts[0].split(SEP))), Flavor(*parts[1].split(SEP)).name
 
 
 def ibuild_gen_csp_dag(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
-                       exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
-                       cpath: set[int] = frozenset(), delay: int = 1) -> tuple[nx.DiGraph, list[list[int]]]:
+                       exec_calc: Callable[[int, int, int], int] = lambda i, t, n: t,
+                       cpath: set[int] = frozenset(), delay: int = 1) -> Generator[nx.DiGraph, list[list[int]]]:
     """
-    Calculate the state-space DAGs of the given *tree* based on the alternative chain decompositions.
-    The given flavors as list of (memory, CPU, cost_factor) tuple defines the available memory (and group upper limit),
-    available relative vCPU cores and
+    Calculate all state-space DAGs of the given *tree* based on the alternative chain decompositions.
+
+    The given flavors as list of (memory, CPU, cost_factor) tuples define the available memory (and group upper limit),
+    available relative vCPU cores and relative cost multiplier.
 
     :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
     :param root:        root node of the graph
     :param flavors:     list of flavors resources given by the tuple of available *(memory, relative CPU cores)*
     :param exec_calc:   function that calculates the effective runtimes from reference runtime and available CPU cores
     :param cpath:       critical path in the form of subchain[root -> cp_end]
     :param delay:       invocation delay between blocks
@@ -94,19 +107,20 @@
                 del _cache[p]
         # Add initial connections from START node
         for sc in _cache[root]:
             dag.add_edge(START, sc, **{COST: 0, LAT: np.array([1, 0])})
         yield dag, chains
 
 
-def csp_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
-                          cp_end: int = None, delay: int = 1, exhaustive: bool = True, solver=cspy.BiDirectional,
-                          timeout: int = None, **cspargs) -> tuple[list[list[int]], int, int]:
+def csp_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                          N: int = 1, cp_end: int = None, delay: int = 1, exhaustive: bool = True,
+                          solver=cspy.BiDirectional, timeout: int = None, **cspargs) -> T_RESULTS:
     """
-    Calculate minimal-cost partitioning of a *tree* based on constrained shortest path (CSP) formalization.
+    Calculate minimal-cost partitioning of a *tree* based on constrained shortest path (CSP) formalization
+    without considering flavor assignment.
 
     Details in: T. Elgamal at al.: “Costless: Optimizing Cost of Serverless Computing through Function Fusion
     and Placement,” in 2018 IEEE/ACM Symposium on Edge Computing (SEC), 2018, pp. 300–312. doi: 10.1109/SEC.2018.00029.
 
     :param tree:        service tree annotated with node runtime(ms), memory(MB) and edge rate
     :param root:        root node of the graph
     :param M:           upper memory bound of the partition blocks in MB
@@ -128,15 +142,16 @@
         # No feasible solution due to too strict limits
         return INFEASIBLE
     for dag, chains in ibuild_gen_csp_dag(tree, root, [Flavor(M, N, 1.0)], cpath=cpath, delay=delay):
         try:
             model = solver(dag, max_res=[len(dag.edges), L], min_res=[1, 0], time_limit=timeout, **cspargs)
             model.run()
             if model.path is not None and model.total_cost < best_res[1]:
-                best_res = extract_grp_from_path(model.path, flav=False), model.total_cost, model.consumed_resources[-1]
+                best_res = extract_grp_from_path(model.path, flavors=False), model.total_cost, model.consumed_resources[
+                    -1]
                 if not exhaustive:
                     # Stop at first feasible solution
                     break
         except Exception:
             # No feasible solution
             continue
         finally:
@@ -144,17 +159,18 @@
                 break
     return best_res
 
 
 def csp_gen_tree_partitioning(tree: nx.DiGraph, root: int = 1, flavors: list[tuple[int, int]] = ((math.inf, 1),),
                               exec_calc: collections.abc.Callable[[int, int], int] = lambda i, t, n: t,
                               L: int = math.inf, cp_end: int = None, delay: int = 1, solver=cspy.BiDirectional,
-                              timeout: int = None, **cspargs) -> tuple[list[list[int]], int, int]:
+                              timeout: int = None, **cspargs) -> T_RESULTS:
     """
-    Calculate minimal-cost partitioning of a *tree* based on constrained shortest path (CSP) formalization.
+    Calculate minimal-cost partitioning of a *tree* based on constrained shortest path (CSP) formalization with
+    incorporated flavor assignment.
 
     Details in: T. Elgamal at al.: “Costless: Optimizing Cost of Serverless Computing through Function Fusion
     and Placement,” in 2018 IEEE/ACM Symposium on Edge Computing (SEC), 2018, pp. 300–312. doi: 10.1109/SEC.2018.00029.
 
 
     :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
     :param root:        root node of the graph
@@ -183,10 +199,16 @@
                 best_res = extract_grp_from_path(model.path), model.total_cost, model.consumed_resources[-1]
         except Exception:
             # No feasible solution
             continue
     return best_res
 
 
-def extract_grp_from_path(path: list[str], flav: bool = True) -> list[list[int]]:
-    """Extract partitioning from *path* and recreate blocks"""
-    return sorted(decode_state(grp) if flav else decode_state(grp)[0] for grp in path[1:-1])
+def extract_grp_from_path(path: list[str], flavors: bool = True) -> T_PART:
+    """
+    Extract partitioning from *path* and recreate partition blocks.
+
+    :param path:    solution path of the CSP graph
+    :param flavors: whether return flavors or not
+    :return:        resulted partitioning blocks
+    """
+    return sorted(decode_state(grp) if flavors else decode_state(grp)[0] for grp in path[1:-1])
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/ext/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/ext/greedy.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,25 +14,26 @@
 import collections
 import heapq
 import itertools
 import math
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_BLOCK, T_RESULTS
 from slambuc.alg.service import MEMORY, RATE, DATA
 from slambuc.alg.util import ibacktrack_chain, recalculate_partitioning, par_subchain_latency, par_subtree_memory
 
 
 def get_bounded_greedy_block(tree: nx.DiGraph, root: int, M: int, N: int = 1, cp_end: int = None,
-                             cp_cuts: set[int] = frozenset()) -> tuple[set[int], list[int]]:
+                             cp_cuts: set[int] = frozenset()) -> tuple[T_BLOCK, list[int]]:
     """
-    Calculate partition block based on the memory limit *M* by iteratively merging edges with the largest weights
-    started from the given *root*. Filter out mandatory cuts of *cp_cuts* on the cpath form merging, while merges
-    other cpath edges.
+    Calculate a partition block based on the memory limit *M* by iteratively merging edges with the largest weights
+    started from the given *root*.
+
+    Filter out mandatory cuts of *cp_cuts* on the cpath form merging, while merges other cpath edges.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param M:       upper memory bound of the partition blocks in MB
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param cp_cuts: barrier nodes of mandatory cuts on the critical path
@@ -58,49 +59,47 @@
         # Stop extension of the current block due to memory limit
         if par_subtree_memory(tree, root, blk | {v}, N) > M:
             break
         blk.add(v)
         add_neighbours(v)
     # Collect root nodes of cut subtrees by the given block
     succ = [sn for n in blk for sn in tree[n] if sn not in blk]
-    return blk, succ
+    return sorted(blk), succ
 
 
-def min_weight_greedy_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
-                                   N: int = 1, cp_end: int = None, delay: int = 1,
-                                   metrics: bool = True, **kwargs) -> tuple[list[list[int]], int, int]:
+def min_weight_greedy_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = 1,
+                                   delay: int = 1, metrics: bool = True, **kwargs) -> T_RESULTS:
     """
-    Calculates memory-bounded tree partitioning in a greedy manner.
+    Calculates memory-bounded tree partitioning in a greedy manner without any latency limit.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param M:       upper memory bound of the partition blocks in MB
     :param N:       available CPU core count
-    :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:   invocation delay between blocks
     :param metrics: return calculated sum cost and critical path latency
     :return:        tuple of derived partitioning, sum cost, and the latency on the critical path (root, cp_end)
     """
     partition, succ = [], collections.deque((root,))
     # Iteratively grow partition blocks starting from root and restarting it at the neighbouring nodes
     while succ:
         blk, next_succ = get_bounded_greedy_block(tree, succ.popleft(), M, N)
         succ.extend(next_succ)
-        partition.append(sorted(blk))
-    sum_cost, sum_lat = recalculate_partitioning(tree, partition, root, N, cp_end, delay) if metrics else (None, None)
+        partition.append(blk)
+    sum_cost, sum_lat = recalculate_partitioning(tree, partition, root, N, None, delay) if metrics else (None, None)
     return partition, sum_cost, sum_lat
 
 
 ########################################################################################################################
 
 
 def get_feasible_cpath_split(tree: nx.DiGraph, root: int, cp_end: int, M: int, L: int, N: int = 1,
                              delay: int = 1) -> set[int]:
     """
-    Calculate feasible splitting of the critical path that meets given memory and latency limits.
+    Calculate feasible splitting of the critical path that meets given memory *M* and latency *L* limits.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param M:       upper memory bound of the partition blocks in MB
     :param L:       latency limit defined on the critical path in ms
     :param N:       available CPU core count
@@ -139,19 +138,18 @@
         else:
             # Greedily select the locally best cut (the largest reduce in lat possibly but not necessarily in opt cuts)
             cuts.add(best_cut)
     return {root, *(cpath[c] for c in cuts)}
 
 
 def min_weight_partition_heuristic(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
-                                   N: int = 1, cp_end: int = None, delay: int = 1,
-                                   metrics: bool = True) -> tuple[list[list[int]], int, int]:
+                                   N: int = 1, cp_end: int = None, delay: int = 1, metrics: bool = True) -> T_RESULTS:
     """
-    Heuristic algorithm to calculate partitioning of the given *tree* regarding the given memory *M* and latency *L*
-    limits.
+    Greedy heuristic algorithm to calculate partitioning of the given *tree* regarding the given memory *M* and
+    latency *L* limits.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param M:       upper memory bound of the partition blocks in MB
     :param L:       latency limit defined on the critical path in ms
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
@@ -166,10 +164,10 @@
         return INFEASIBLE
     partition, succ = [], collections.deque((root,))
     # Iteratively grow partition blocks starting from root and restarting it at the neighbouring nodes
     while succ:
         v = succ.popleft()
         blk, next_succ = get_bounded_greedy_block(tree, v, M, N, cp_end, cpath_cuts)
         succ.extend(next_succ)
-        partition.append(sorted(blk))
+        partition.append(blk)
     sum_cost, sum_lat = recalculate_partitioning(tree, partition, root, N, cp_end, delay) if metrics else (None, None)
     return partition, sum_cost, sum_lat
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/ext/min_cut.py` & `SLAMBUC-0.2.0/slambuc/alg/ext/min_cut.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,37 +14,39 @@
 import collections
 import itertools
 import math
 import operator
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import RATE, DATA, PLATFORM
 from slambuc.alg.util import recreate_subtree_blocks, recalculate_partitioning
 
 
 def min_weight_subchain_split(tree: nx.DiGraph, root: int) -> set[int]:
     """
     Return chain-based edge cuts with the minimal edge weight (amount of transferred data).
+
     The splitting marks the edge with the largest weight at each branching nodes to be a must-merge edge.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
-    :return:        barrier nodes
+    :return:        set of barrier nodes
     """
     return {root}.union(*(set(tree.successors(v)) -
                           {max(tree.successors(v), key=lambda s: tree[v][s][RATE] * tree[v][s][DATA])}
                           for v in tree if v is not PLATFORM and len(tree.succ[v]) > 1))
 
 
-def min_weight_chain_decomposition(tree: nx.DiGraph, root: int, N: int = 1, cp_end: int = None, delay: int = 1,
-                                   metrics: bool = True, **kwargs) -> tuple[list[list[int]], int, int]:
+def min_weight_chain_decomposition(tree: nx.DiGraph, root: int, N: int = 1, cp_end: int = None,
+                                   delay: int = 1, metrics: bool = True, **kwargs) -> T_RESULTS:
     """
     Minimal edge-weight chain-based tree partitioning (O(n)) without memory and latency constraints.
+
     Although latency is not considered on the critical path the algorithm reports it with the sum cost.
 
     :param tree:    service graph annotated with node runtime(ms) and edge rate
     :param root:    root node of the tree
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:   invocation delay between blocks
@@ -58,24 +60,25 @@
 
 ########################################################################################################################
 
 
 def min_weight_ksplit(tree: nx.DiGraph, root: int, k: int) -> set[int]:
     """
     Minimal data-transfer tree clustering into *k* clusters with k-1 cuts without memory and latency constraints.
+
     The clustering algorithm is based on the maximum split clustering algorithm(O(n^3)) which ranks the edges (paths)
     based on the amount of transferred data.
 
     Details in: M. Maravalle et al.: “Clustering on trees,” Computational Statistics & Data Analysis, vol. 24, no. 2,
     pp. 217–234, Apr. 1997, doi: 10.1016/S0167-9473(96)00062-X.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param k:       number of clusters
-    :return:        barrier nodes
+    :return:        set of barrier nodes
     """
     dist_tree = nx.to_undirected(tree)
     # Define distance of two nodes as the reciprocal of the sum transferred data between the nodes
     D = {(u, v): sum(1 / (attr[RATE] * attr[DATA]) if attr[RATE] and attr[DATA] else 0
                      for i, j, attr in tree.edges(next(nx.all_simple_paths(dist_tree, u, v)), data=True))
          for u, v in itertools.combinations(filter(lambda n: n is not PLATFORM, tree), 2)}
     edges, rank = set(tree.edges(filter(lambda n: n is not PLATFORM, tree))), 1
@@ -91,18 +94,19 @@
             if not edges:
                 break
             rank += 1
     return {root}.union(b for _, b in labeled)
 
 
 def min_weight_ksplit_clustering(tree: nx.DiGraph, root: int, k: int = None, N: int = 1, cp_end: int = None,
-                                 delay: int = 1, metrics: bool = True, **kwargs) -> tuple[list[list[int]], int, int]:
+                                 delay: int = 1, metrics: bool = True, **kwargs) -> T_RESULTS:
     """
     Minimal data-transfer tree clustering into *k* clusters (with k-1 cuts) without memory and latency constraints.
-    Although latency is not considered on the critical path the algorithm reports it with the sum cost.
+
+    Although latency is not considered on the critical path the algorithm reports it along with the sum cost.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param k:       number of clusters
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:   invocation delay between blocks
@@ -112,18 +116,20 @@
     k = k if k is not None else math.ceil(math.sqrt(len(tree) - 1))
     partition = recreate_subtree_blocks(tree, barr=min_weight_ksplit(tree, root, k))
     sum_cost, sum_lat = recalculate_partitioning(tree, partition, root, N, cp_end, delay) if metrics else (None, None)
     return partition, sum_cost, sum_lat
 
 
 def min_weight_tree_clustering(tree: nx.DiGraph, root: int, L: int = math.inf, N: int = 1, cp_end: int = None,
-                               delay: int = 1, metrics: bool = True, **kwargs) -> tuple[list[list[int]], int, int]:
+                               delay: int = 1, metrics: bool = True, **kwargs) -> T_RESULTS:
     """
-    Minimal data-transfer tree clustering into without memory  constraints.
-    Iteratively calculates k-1 different ksplit clustering in reverse order until a latency-feasible solution is found.
+    Minimal data-transfer tree clustering into without memory constraints.
+
+    Iteratively calculates *k-1* different ksplit clustering in reverse order until an L-feasible solution is found.
+
     Although latency is not considered on the critical path the algorithm reports it with the sum cost.
 
     :param tree:    service graph annotated with node runtime(ms), edge rate and edge data unit size
     :param root:    root node of the tree
     :param L:       latency limit defined on the critical path in ms
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/service/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/service/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/service/common.py` & `SLAMBUC-0.2.0/slambuc/alg/service/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,12 +41,14 @@
 class Flavor(typing.NamedTuple):
     """Store subtree partitioning attributes for a given subcase"""
     mem: int = math.inf  # Available memory
     ncore: int = 1  # Available relative vCPU cores
     cfactor: float = 1.0  # Relative cost factor
 
     def __repr__(self):
-        return repr(tuple(self))
+        # return repr(tuple(self))
+        return self.name
 
     @property
-    def name(self):
-        return f"F[{self.mem},{self.ncore}]"
+    def name(self) -> str:
+        """String representation of the given flavor"""
+        return f"F[{self.mem},{self.ncore},{self.cfactor}]"
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,9 +8,10 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .dp import *
+from .layout import *
 from .par import *
 from .ser import *
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/dp/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/dp/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,8 +9,9 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 from .greedy import greedy_tree_partitioning
 from .meta import meta_tree_partitioning
+from .min import min_tree_partitioning
 from .seq import seq_tree_partitioning
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/dp/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/dp/greedy.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import math
+from collections.abc import Generator
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.util import (isubtrees, ibacktrack_chain, ipowerset, path_blocks, block_cost, block_latency,
                               block_memory, block_cpu)
 
 
-def ichains_exhaustive(tree: nx.DiGraph, root: int, M: int, N: int) -> list[int]:
-    """Calculate all combination of edge cuts and returns only if it is feasible wrt. the chain connectivity, M, and N.
-    The calculation is improved compared to brute force to only start calculating cuts from c_min.
+def ichains_exhaustive(tree: nx.DiGraph, root: int, M: int, N: int) -> Generator[list[int]]:
+    """
+    Calculate all combination of edge cuts and returns only if it is feasible wrt. the chain connectivity, M, and N.
+
+    Calculation is improved compared to brute force to only start calculating cuts from c_min.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound in MB
     :param N:       upper CPU core bound
     :return:        generator of chain partitions
     """
     c_min = math.ceil(sum(nx.get_node_attributes(tree, MEMORY).values()) / M) - 1
     for cuts in ipowerset(tree.edges(range(1, len(tree))), start=c_min):
@@ -43,19 +46,21 @@
                                  itertools.pairwise([next(tree.predecessors(b)), *nodes])])
             if block_memory(memory, 0, len(nodes) - 1) > M or block_cpu(rate, 0, len(nodes) - 1) > N:
                 break
         else:
             yield barr
 
 
-def ifeasible_chains(tree: nx.DiGraph, root: int, M: int, N: int) -> list[int]:
-    """Calculate only feasible chain partitions and returns the one which meets the limits M and N.
-    The calculation is improved compared to brute force to only calculate chain partitions based on the branching nodes.
+def ifeasible_chains(tree: nx.DiGraph, root: int, M: int, N: int) -> Generator[list[int]]:
+    """
+    Calculate only feasible chain partitions and returns the one which meets the limits M and N.
+
+    Calculation is improved compared to brute force to only calculate chain partitions based on the branching nodes.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound in MB
     :param N:       upper CPU core bound
     :return:        generator of chain partitions
     """
     branch_edges = [itertools.chain(itertools.combinations(tree.succ[b], len(tree.succ[b]) - 1),
                                     [tuple(tree.successors(b))]) for b in (v for v, d in tree.out_degree if d > 1)]
@@ -71,19 +76,19 @@
                 break
         else:
             yield barr
 
 
 def greedy_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = math.inf,
                              L: int = math.inf, cp_end: int = None, delay: int = 1, unit: int = 100,
-                             ichains=ifeasible_chains, only_cuts: bool = False) -> list[tuple[list, int, int]]:
+                             ichains=ifeasible_chains, only_cuts: bool = False) -> list[T_RESULTS]:
     """
     Calculates minimal-cost partitioning of a service graph(tree) by iterating over all possible cuttings.
 
-    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:        root node of the graph
     :param M:           upper memory bound of the partition blocks (in MB)
     :param N:           upper CPU core bound of the partition blocks
     :param L:           latency limit defined on the critical path (in ms)
     :param cp_end:      tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:       invocation delay between blocks
     :param unit:        rounding unit for the cost calculation (default: 100 ms)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/dp/meta.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/dp/meta.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,39 +14,51 @@
 import collections
 import itertools
 import math
 import typing
 
 import networkx as nx
 
-from slambuc.alg import COST, INFEASIBLE
+from slambuc.alg import COST, INFEASIBLE, T_BRESULTS
 from slambuc.alg.chain.dp.mtx import chain_partitioning, extract_barr
 from slambuc.alg.service import *
 from slambuc.alg.service.common import LABEL
 from slambuc.alg.util import ipostorder_dfs, isubchains, ibacktrack_chain, leaf_label_nodes, recreate_subchain_blocks
 
 
 class TPart(typing.NamedTuple):
-    """Store subtree attributes for a given subcase"""
+    """Store subtree attributes for a given meta subcase."""
     barr: set = set()  # Barrier/heading nodes of the given subtree partitioning
     cost: int = math.inf  # Sum cost of the partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def meta_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = math.inf, L: int = math.inf,
                            cp_end: int = None, delay: int = 1, unit: int = 100, only_barr: bool = False,
-                           partition=chain_partitioning, barriers=extract_barr) -> tuple[list[int], int, int]:
+                           partition=chain_partitioning, barriers=extract_barr) -> T_BRESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
     memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes using
-    the *partition* function to partition subchains.
+    the *partition* function to partition subchains independently.
 
-    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
+
+    It gives optimal result only in case the cost function regarding the chain attributes is sub-additive,
+    that is k_opt = k_min is guaranteed for each case.
+
+    Instead of full partitioning it only returns the list of barrier nodes.
+
+    Details in: J. Czentye, I. Pelle and B. Sonkoly, "Cost-optimal Operation of Latency Constrained Serverless
+    Applications: From Theory to Practice," NOMS 2023-2023 IEEE/IFIP Network Operations and Management Symposium,
+    Miami, FL, USA, 2023, pp. 1-10, doi: 10.1109/NOMS56928.2023.10154412.
+
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:        root node of the graph
     :param M:           upper memory bound of the partition blocks (in MB)
     :param N:           upper CPU core bound of the partition blocks
     :param L:           latency limit defined on the critical path (in ms)
     :param cp_end:      tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:       invocation delay between blocks
     :param unit:        rounding unit for the cost calculation (default: 100 ms)
@@ -88,15 +100,15 @@
                     DP[n][0] = TPart({subchain[b] for b in barr} | sum_m_barr, sum_cost)
             # Subchain is the tail part of cpath -> all inner edges are allowed to be merged
             elif subchain[-1] == cp_end:
                 # If subchain is the cpath -> partitioning can be calculated directly applying L
                 if subchain[0] == root:
                     barr, opt_cost, opt_lat = partition(runtime, memory, rate, M, N, L, delay=delay, unit=unit)
                     if not barr:
-                        return [], opt_cost, opt_lat
+                        return barr, opt_cost, opt_lat
                     opt_barr_cost = TPart({subchain[b] for b in barr} | sum_m_barr, sum_cost := opt_cost + sum_m_cost)
                     for c in range(len(barr) - 1, c_max + 1):
                         if sum_cost < DP[n][c].cost:
                             DP[n][c] = opt_barr_cost
                 else:
                     # Without L, there should exist feasible solution wrt. M
                     CDP, *_ = partition(runtime, memory, rate, M, N, delay=delay, unit=unit, ret_dp=True)
@@ -132,15 +144,15 @@
                         if c_head in c_cache:
                             barr, opt_cost = c_cache[c_head]
                         else:
                             L_head = sum(tree.nodes[v][RUNTIME] for v in head_part) + c_head * delay
                             barr, opt_cost, _ = partition(runtime, memory, rate, M, N, L_head, 0, len(head_part) - 1,
                                                           delay, unit)
                             # If subchain cannot be partitioned with L_head -> stricter L_head is also infeasible
-                            if barr is None:
+                            if not barr:
                                 break
                             # Precalculate stricter solutions based on the distance between optimal cut and L_head cut
                             for _c in reversed(range(len(barr) - 1, c_head + 1)):
                                 c_cache[_c] = (barr, opt_cost)
                         c = k + c_head + 1
                         if (sum_cost := opt_cost + DP[m_cp][k].cost + sum_m_cost) < DP[n][c].cost:
                             DP[n][c] = TPart({subchain[b] for b in barr}.union(DP[m_cp][k].barr, sum_m_barr), sum_cost)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/dp/min.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/dp/min.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,43 +13,48 @@
 # limitations under the License.
 import collections
 import math
 import typing
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_BLOCK, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.util import ipostorder_dfs, ibacktrack_chain
 
 
 class MinTBlock(typing.NamedTuple):
-    """Store subtree attributes for a given subcase"""
+    """Store subtree attributes for a given min subcase."""
     w: int = None  # Tailing node of the first block of the subtree partitioning
     c: int = 0  # Number of cuts the given subtree partitioning introduce on the critical path
     sum_cost: int = math.inf  # Sum cost of the subtree partitioning
     cost: int = math.inf  # Cost of the first block (with tail node w) in the subtree partitioning
     mem: int = math.inf  # Sum memory of the first block
     max_rate: int = 0  # Maximum rate value of internal edge in the first block
     cpu: int = 1  # Sum CPU core need of the first block
 
     def __repr__(self):
         return repr(tuple(self))
 
 
-def min_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = math.inf,
-                          L: int = math.inf, cp_end: int = None, delay: int = 1, unit: int = 100,
-                          full: bool = True) -> tuple[list[int], int, int]:
+def min_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = math.inf, L: int = math.inf,
+                          cp_end: int = None, delay: int = 1, unit: int = 100, full: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
     memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
 
-    It can be only used when the cost function regarding the graph attributes is sub-additive.
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    It gives optimal result only in case the cost function regarding the chain attributes is sub-additive,
+    that is k_opt = k_min is guaranteed for each case.
+
+    Instead of full partitioning it only returns the list of barrier nodes.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:   invocation delay between blocks
     :param unit:    rounding unit for the cost calculation (default: 100 ms)
@@ -73,16 +78,18 @@
         if blk.sum_cost < math.inf and blk.mem <= M and blk.cpu <= N and blk.c <= c_max:
             if blk.sum_cost <= qmin(node).sum_cost:
                 DP[node].appendleft(blk)
             else:
                 DP[node].append(blk)
 
     def qmerge(pred: int, node: int, barr: int, m_cost: int, add_cut: bool = False):
-        """Copy DP entries from queue of node *barr* with *c_b* cuts into queue of node *node* with *c_n* cuts
-        while leaving the best subcase in the original queue."""
+        """
+        Copy DP entries from queue of node *barr* with *c_b* cuts into queue of node *node* with *c_n* cuts
+        while leaving the best subcase in the original queue.
+        """
         blk = None
         while len(DP[barr]):
             blk = DP[barr].pop()
             # Ignore infeasible subcases
             if blk.sum_cost < math.inf:
                 blk_cost = block_cost(pred, node, blk.w)
                 sum_blk_cost = blk.sum_cost + (blk_cost - blk.cost) + m_cost
@@ -91,15 +98,15 @@
                 blk_max_rate = max(blk.max_rate, tree[pred][node][RATE])
                 blk_cpu = max(blk.cpu, math.ceil(blk_max_rate / tree[pred][node][RATE]))
                 qinsert(node, MinTBlock(blk.w, sum_blk_cut, sum_blk_cost, blk_cost, blk_mem, blk_max_rate, blk_cpu))
         # Leave only the best/min subcase in the queue as the first element
         DP[barr].append(blk)
 
     def block_cost(pred: int, barr: int, w: int) -> int:
-        """Calculate running time of block: p -> [barr -> w]"""
+        """Calculate running time of block: p -> [barr -> w]."""
         sum_time = tree.nodes[w][RUNTIME]
         while w > barr:
             w = next(tree.predecessors(w))
             sum_time += tree.nodes[w][RUNTIME]
         return tree[pred][barr][RATE] * (math.ceil(sum_time / unit) * unit)
 
     for p, n in ipostorder_dfs(tree, root):
@@ -129,16 +136,25 @@
                 qmerge(p, n, b, sum_m_cost - qmin(b).sum_cost, add_cut=True if b != m_cp else False)
     if qmin(root).sum_cost < math.inf:
         return extract_min_blocks(tree, DP, root, full), qmin(root).sum_cost, qmin(root).c
     else:
         return INFEASIBLE
 
 
-def extract_min_blocks(tree: nx.DiGraph, DP: list[dict], root: int, full: bool = True) -> list[int]:
-    """Extract subtree roots of partitioning from the tailing nodes stored in the *DP* matrix"""
+def extract_min_blocks(tree: nx.DiGraph, DP: list[collections.deque[MinTBlock]],
+                       root: int, full: bool = True) -> T_BLOCK:
+    """
+    Extract subtree roots of partitioning from the tailing nodes stored in the *DP* matrix.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param DP:      dynamic programming structure storing intermediate *MinTBlock* subcases
+    :param root:    root node of the graph
+    :param full:    calculate full blocks
+    :return:        partitioning blocks
+    """
     n = set(filter(lambda v: v is not PLATFORM, tree))
     p = []
     barr = {root}
     while len(n):
         b = barr.pop()
         w = DP[b][0].w
         blk, prior = [], None
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/dp/seq.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/dp/seq.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,40 +14,48 @@
 import collections
 import functools
 import math
 import typing
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS, T_PART
 from slambuc.alg.service import *
 from slambuc.alg.util import ipostorder_dfs, ibacktrack_chain, verify_limits
 
 
 class TBlock(typing.NamedTuple):
-    """Store subtree attributes for a given subcase"""
+    """Store subtree attributes for a given seq subcase."""
     w: int = None  # Tailing node of the first block of the subtree partitioning
     sum_cost: int = math.inf  # Sum cost of the subtree partitioning
     cumsum: int = 0  # Sum (cumulative) runtime of the first block (with tail node w) in the partitioning
     mem: int = math.inf  # Sum memory of the first block
     max_rate: int = 0  # Maximum rate value of internal edge in the first block
     cpu: int = 1  # Sum CPU core need of the first block
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def seq_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, N: int = math.inf,
                           L: int = math.inf, cp_end: int = None, delay: int = 1, unit: int = 100,
-                          full: bool = True) -> tuple[list[int], int, int]:
+                          full: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes leveraging
+    a bottom-up tree traversal approach.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    Cost calculation relies on the rounding *unit* and number of vCPU cores *N*, whereas platform invocation *delay*
+    is used for latency calculations.
+
+    Details in: J. Czentye, I. Pelle and B. Sonkoly, "Cost-optimal Operation of Latency Constrained Serverless
+    Applications: From Theory to Practice," NOMS 2023-2023 IEEE/IFIP Network Operations and Management Symposium,
+    Miami, FL, USA, 2023, pp. 1-10, doi: 10.1109/NOMS56928.2023.10154412.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param N:       upper CPU core bound of the partition blocks
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:   invocation delay between blocks
     :param unit:    rounding unit for the cost calculation (default: 100 ms)
@@ -66,22 +74,22 @@
         return [], None, c_max
     DP = [collections.defaultdict(collections.deque) for _ in range(len(tree))]
     for i in range(len(DP)):
         DP[i][0].append(TBlock())
 
     @functools.lru_cache(maxsize=(len(tree) - 1))
     def block_cost(pred: int, barr: int, cumsum: int, expand: bool = True) -> tuple[int, int]:
-        """Calculate sum cost of subtree: T_barr and also return the cumulative sum runtime of the block[barr, w]"""
+        """Calculate sum cost of subtree: T_barr and also return the cumulative sum runtime of the block[barr, w]."""
         if expand:
             cumsum += tree.nodes[barr][RUNTIME]
         return tree[pred][barr][RATE] * (math.ceil(cumsum / unit) * unit), cumsum
 
     @functools.lru_cache(maxsize=(len(tree) - 1))
     def block_cpu(pred: int, node: int, max_rate: int, cpu: int) -> tuple[int, int]:
-        """Calculate the nex CPU core need of the block[barr, w] and also return the max internal rate"""
+        """Calculate the nex CPU core need of the block[barr, w] and also return the max internal rate."""
         blk_max_rate = max(max_rate, tree[pred][node][RATE])
         return max(cpu, math.ceil(blk_max_rate / tree[pred][node][RATE])), blk_max_rate
 
     def qmin(node: int, c_n: int) -> int:
         """Return the sum cost of best/min subcase for *node* with *c_n* cuts."""
         return DP[node][c_n][0].sum_cost
 
@@ -90,16 +98,18 @@
         if blk.sum_cost < math.inf and blk.mem <= M and blk.cpu <= N:
             if len(DP[node][c_n]) and blk.sum_cost <= qmin(node, c_n):
                 DP[node][c_n].appendleft(blk)
             else:
                 DP[node][c_n].append(blk)
 
     def qmerge(pred: int, node: int, c_n: int, barr: int, c_b: int, m_cost: int):
-        """Copy DP entries from queue of node *barr* with *c_b* cuts into queue of node *node* with *c_n* cuts
-        while leaving the best subcase in the original queue."""
+        """
+        Copy DP entries from queue of node *barr* with *c_b* cuts into queue of node *node* with *c_n* cuts
+        while leaving the best subcase in the original queue.
+        """
         for blk in DP[barr][c_b]:
             # Ignore infeasible subcases
             if blk.sum_cost < math.inf:
                 # Calculate the original cost of the block[barr, w]
                 b_blk_cost, _ = block_cost(node, barr, blk.cumsum, expand=False)
                 # Calculate the cost of the expanded block[node, w], n -> barr
                 n_blk_cost, n_blk_cumsum = block_cost(pred, node, blk.cumsum)
@@ -161,17 +171,27 @@
     c_opt = min(DP[root], key=lambda _c: qmin(root, _c))
     if qmin(root, c_opt) < math.inf:
         return extract_blocks(tree, DP, root, cp_end, c_opt, full), qmin(root, c_opt), c_opt
     else:
         return [], math.inf, c_opt
 
 
-def extract_blocks(tree: nx.DiGraph, DP: list[dict], root: int, cp_end: int, c_opt: int,
-                   full: bool = True) -> list[int]:
-    """Extract subtree roots of partitioning from the tailing nodes stored in the *DP* matrix"""
+def extract_blocks(tree: nx.DiGraph, DP: list[collections.defaultdict[collections.deque[TBlock]]],
+                   root: int, cp_end: int, c_opt: int, full: bool = True) -> T_PART:
+    """
+    Extract subtree roots of partitioning from the tailing nodes stored in the *DP* matrix.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param DP:      dynamic programming structure storing intermediate *TBlock* subcases
+    :param root:    root node of the graph
+    :param cp_end:  tail node of the critical path
+    :param c_opt:   calculated optimal cut size
+    :param full:    calculate full blocks
+    :return:        partitioning blocks
+    """
     n = set(filter(lambda v: v is not PLATFORM, tree))
     cpath = set(ibacktrack_chain(tree, root, cp_end))
     p = []
     barr = {(root, c_opt)}
     while len(n):
         b, c = barr.pop()
         w = DP[b][c][0].w
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/layout/__init__.py` & `SLAMBUC-0.2.0/slambuc/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/layout/ilp.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/layout/ilp.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,26 +9,35 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import collections
 import itertools
+from collections.abc import Generator
 
 import networkx as nx
 import pulp as lp
 
-from slambuc.alg import LP_LAT, INFEASIBLE
+from slambuc.alg import LP_LAT, INFEASIBLE, T_FRESULTS, T_FPART
 from slambuc.alg.service.common import *
 from slambuc.alg.util import (ipowerset, ipostorder_dfs, ibacktrack_chain, gen_subtree_memory, gen_subtree_cost,
                               gen_subchain_latency, recreate_subtree_blocks, x_eval)
 
 
-def ifeasible_gen_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> tuple[int, list[list[int]]]:
-    """Generate feasible(connected) subtrees and roots in bottom-up way, which meet the memory constraint *M*"""
+def ifeasible_gen_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> Generator[tuple[int, set[int]]]:
+    """
+    Generate M-feasible(connected) subtrees and roots in bottom-up way, which meet the memory constraint *M*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param M:       upper memory bound of the partition blocks (in MB)
+    :param N:       upper CPU core bound of the partition blocks
+    :return:        generator of subtree root and regarding subtree nodes
+    """
     subtrees = collections.defaultdict(list)
     for _, n in ipostorder_dfs(tree, root):
         for children in ipowerset(tuple(tree.successors(n))):
             for sts in itertools.product(*(subtrees[c] for c in children)):
                 st = {n}.union(*sts)
                 if gen_subtree_memory(tree, n, st, N) <= M:
                     subtrees[n].append(st)
@@ -38,15 +47,16 @@
 
 
 def build_gen_tree_cfg_model(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
                              exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
                              L: int = math.inf, cp_end: int = None,
                              delay: int = 1) -> tuple[lp.LpProblem, list[lp.LpVariable]]:
     """
-    Generate the ILP model.
+    Generate the configuration ILP model with the given *flavors*.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Critical path
     cpath = set(ibacktrack_chain(tree, root, cp_end))
     # Decision variables with precalculated coefficients
@@ -74,21 +84,20 @@
     # Latency constraint
     model += lp.lpSum(l_x) <= L if L < math.inf else lp.lpSum(l_x) >= 0, LP_LAT
     return model, X
 
 
 def tree_gen_hybrid_partitioning(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
                                  exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
-                                 L: int = math.inf, cp_end: int = None, delay: int = 1,
-                                 solver: lp.LpSolver = None, timeout: int = None,
-                                 **lpargs) -> tuple[list[tuple[list[list[int]], Flavor]], int, int]:
+                                 L: int = math.inf, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
+                                 timeout: int = None, **lpargs) -> T_FRESULTS:
     """
-    Calculate minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculate minimal-cost partitioning of a tree based on configuration LP formulation and given *flavors*.
 
-    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:        root node of the graph
     :param flavors:     list of flavors resources given by the tuple of available *(memory, relative CPU cores)*
     :param exec_calc:   function that calculates the effective runtimes from reference runtime and available CPU cores
     :param L:           latency limit defined on the critical path (in ms)
     :param cp_end:      tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:       invocation delay between blocks
     :param solver:      specific solver class (default: COIN-OR CBC)
@@ -101,31 +110,37 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = lp.value(model.objective), lp.value(model.constraints[LP_LAT])
         return recreate_st_from_gen_xdict(tree, X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def recreate_st_from_gen_xdict(tree: nx.DiGraph,
-                               X: dict[Flavor, dict[int, list[lp.LpVariable]]]) -> list[tuple[list[int], Flavor]]:
-    """Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks"""
+def recreate_st_from_gen_xdict(tree: nx.DiGraph, X: dict[Flavor, dict[int, list[lp.LpVariable]]]) -> T_FPART:
+    """
+    Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param X:       internal structure of decision variables
+    :return:        partition blocks
+    """
     dbarr = {int(x.name.rsplit('_', 2)[1]): f
              for f in X for v in X[f] for x in filter(lambda _x: _x.varValue == 1, X[f][v])}
     return [(p, dbarr[p[0]]) for p in recreate_subtree_blocks(tree=tree, barr=dbarr)]
 
 
 ########################################################################################################################
 
 
 def build_gen_tree_mtx_model(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
                              exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
                              L: int = math.inf, cp_end: int = None,
                              delay: int = 1) -> tuple[lp.LpProblem, dict[int, dict[int, dict[int, lp.LpVariable]]]]:
     """
-    Generate the ILP model.
+    Generate the matrix ILP model with the given *flavors*.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Empty decision variable matrix
     X = {f: {j: {} for j in tree if j is not PLATFORM} for f in flavors}
     # Objective
@@ -188,19 +203,19 @@
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
 def tree_gen_mtx_partitioning(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
                               exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
                               L: int = math.inf, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                              timeout: int = None, **lpargs) -> tuple[list[tuple[list[list[int]], Flavor]], int, int]:
+                              timeout: int = None, **lpargs) -> T_FRESULTS:
     """
-    Calculate minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculate minimal-cost partitioning of a tree based on matrix LP formulation and given *flavors*.
 
-    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:        root node of the graph
     :param flavors:     list of flavors resources given by the tuple of available *(memory, relative CPU cores)*
     :param exec_calc:   function that calculates the effective runtimes from reference runtime and available CPU cores
     :param L:           latency limit defined on the critical path (in ms)
     :param cp_end:      tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:       invocation delay between blocks
     :param solver:      specific solver class (default: COIN-OR CBC)
@@ -213,32 +228,37 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = round(lp.value(model.objective), 0), round(lp.value(model.constraints[LP_LAT]), 0)
         return extract_st_from_gen_xmatrix(X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def extract_st_from_gen_xmatrix(X: dict[Flavor, dict[int, dict[int, lp.LpVariable]]]) -> list[tuple[list, Flavor]]:
-    """Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks"""
+def extract_st_from_gen_xmatrix(X: dict[Flavor, dict[int, dict[int, lp.LpVariable]]]) -> T_FPART:
+    """
+    Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks.
+
+    :param X:       internal structure of decision variables
+    :return:        partition blocks
+    """
     return sorted(([i for i in sorted(X[f]) if j in X[f][i] and x_eval(X[f][i][j])], f)
                   for f in X for j in sorted(X[f]) if x_eval(X[f][j][j]))
 
 
 ########################################################################################################################
 
 
 def all_gen_tree_mtx_partitioning(tree: nx.DiGraph, root: int = 1, flavors: list[Flavor] = (Flavor(),),
                                   exec_calc: collections.abc.Callable[[int, int, int], int] = lambda i, t, n: t,
                                   L: int = math.inf, cp_end: int = None, delay: int = 1,
                                   solver: lp.LpSolver = None, timeout: int = None,
-                                  **lpargs) -> tuple[list[tuple[list[list[int]], Flavor]], int, int]:
+                                  **lpargs) -> list[T_FPART]:
     """
-    Calculate all minimal-cost partitioning variations of a tree based on matrix ILP formulation.
+    Calculate all minimal-cost partitioning variations of a tree based on matrix ILP formulation and *flavors*.
 
-    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:        root node of the graph
     :param flavors:     list of flavors resources given by the tuple of available *(memory, relative CPU cores)*
     :param exec_calc:   function that calculates the effective runtimes from reference runtime and available CPU cores
     :param L:           latency limit defined on the critical path (in ms)
     :param cp_end:      tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:       invocation delay between blocks
     :param solver:      specific solver class (default: COIN-OR CBC)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/par/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/par/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/par/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/par/greedy.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,42 +11,47 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS, T_BARRS_GEN
 from slambuc.alg.util import (ipowerset, isubtrees, par_subtree_memory, ibacktrack_chain, par_subtree_cost,
                               par_subchain_latency)
 
 
-def isubtrees_exhaustive(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> list[int]:
-    """Calculate all combination of edge cuts and returns only if it is feasible wrt. the memory limit M.
+def isubtrees_exhaustive(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> T_BARRS_GEN:
+    """
+    Calculate all combinations of edge cuts and returns only if it is feasible wrt. the memory limit *M*.
+
+    Block metrics are calculated based on parallelized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound in MB
     :param N:       available CPU core count
-    :return:        generator of chain partitions
+    :return:        generator of feasible subtrees' barrier nodes
     """
     for cuts in ipowerset(tree.edges(range(1, len(tree)))):
         barrs = {root}.union(v for _, v in cuts)
         # Check whether the subtrees meet the memory requirement M
         feasible_subtrees = [b for b, nodes in isubtrees(tree, barrs) if par_subtree_memory(tree, b, nodes, N) <= M]
         if len(feasible_subtrees) == len(barrs):
             yield feasible_subtrees
 
 
-def greedy_par_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
-                                 cp_end: int = None, delay: int = 1) -> list[tuple[list, int, int]]:
+def greedy_par_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                                 N: int = 1, cp_end: int = None, delay: int = 1) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a service graph(tree) by iterating over all possible cuttings.
+    Calculate minimal-cost partitioning of a service graph(tree) by greedily iterating over all possible cuttings.
+
+    Block metrics are calculated based on parallelized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param N:       available CPU core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :return:        tuple of list of best partitions, sum cost of the partitioning, and resulted latency
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/par/ilp.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/par/ilp.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,56 +10,75 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import collections
 import itertools
 import math
+from collections.abc import Generator
 
 import networkx as nx
 import pulp as lp
 
-from slambuc.alg import LP_LAT, INFEASIBLE
+from slambuc.alg import LP_LAT, INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.tree.ser.ilp import recreate_subtrees_from_xdict, extract_subtrees_from_xmatrix
 from slambuc.alg.util import (ipowerset, par_subtree_memory, ipostorder_dfs, ibacktrack_chain, par_subtree_cost,
                               par_subchain_latency, induced_subtrees, par_inst_count, verify_limits, x_eval)
 
 
-def ifeasible_par_greedy_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> list[list[int]]:
-    """Generate feasible subtrees in combinatorial way, which meet the connectivity and memory constraint *M*"""
+def ifeasible_par_greedy_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> Generator[tuple[int, set[int]]]:
+    """
+    Generate feasible subtrees in a combinatorial way, which meet the connectivity and memory constraint *M*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param M:       upper memory bound of the partition blocks (in MB)
+    :param N:       upper CPU core bound of the partition blocks
+    :return:        generator of subtree root and regarding subtree nodes
+    """
     for st in ipowerset(tuple(filter(lambda n: n is not PLATFORM, tree)), start=1):
         st = set(st)
         for v in itertools.islice(sorted(st, reverse=True), len(st) - 1):
             if next(tree.predecessors(v)) not in st:
                 break
         else:
             if par_subtree_memory(tree, min(st), st, N) <= M:
                 yield min(st), st
 
 
-def ifeasible_par_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> tuple[int, list[list[int]]]:
-    """Generate feasible(connected) subtrees and roots in bottom-up way, which meet the memory constraint *M*"""
+def ifeasible_par_subtrees(tree: nx.DiGraph, root: int, M: int, N: int = 1) -> Generator[tuple[int, set[int]]]:
+    """
+    Generate M-feasible(connected) subtrees and roots in a bottom-up way, which meet the memory constraint *M*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param M:       upper memory bound of the partition blocks (in MB)
+    :param N:       upper CPU core bound of the partition blocks
+    :return:        generator of subtree root and regarding subtree nodes
+    """
     subtrees = collections.defaultdict(list)
     for _, n in ipostorder_dfs(tree, root):
         for children in ipowerset(tuple(tree.successors(n))):
             for sts in itertools.product(*(subtrees[c] for c in children)):
                 st = {n}.union(*sts)
                 if par_subtree_memory(tree, n, st, N) <= M:
                     subtrees[n].append(st)
                     yield n, st
         for c in tree.succ[n]:
             del subtrees[c]
 
 
-def build_par_tree_cfg_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
-                             L: int = math.inf, N: int = 1, cpath: set[int] = frozenset(), delay: int = 1,
-                             isubtrees: iter = ifeasible_par_subtrees) -> tuple[lp.LpProblem, list[lp.LpVariable]]:
+def build_par_tree_cfg_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                             N: int = 1, cpath: set[int] = frozenset(), delay: int = 1,
+                             isubtrees: iter = ifeasible_par_subtrees) -> tuple[
+    lp.LpProblem, dict[int, list[lp.LpVariable]]]:
     """
-    Generate the ILP model.
+    Generate the configuration ILP model using parallel metric calculation.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Decision variables with precalculated coefficients
     c_x, l_x, X_n = [], [], collections.defaultdict(list)
     for i, (b, nodes) in enumerate(isubtrees(tree, root, M, N)):
@@ -84,19 +103,22 @@
     # Latency constraint
     model += lp.lpSum(l_x) <= L if L < math.inf else lp.lpSum(l_x) >= 0, LP_LAT
     return model, X_n
 
 
 def tree_par_cfg_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                               N: int = 1, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                              timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+                              timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculate minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculate minimal-cost partitioning of a tree based on configuration LP formulation and greedy subcase
+    generation.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    Block metrics are calculated based on parallelized execution platform model.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param N:       available CPU core count
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
@@ -117,19 +139,22 @@
         return recreate_subtrees_from_xdict(tree, X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
 def tree_par_hybrid_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                  N: int = 1, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                                 timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+                                 timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculate minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculate minimal-cost partitioning of a tree based on configuration LP formulation and hybrid subcase
+    generation.
+
+    Block metrics are calculated based on parallelized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param N:       available CPU core count
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
@@ -154,15 +179,16 @@
 
 ########################################################################################################################
 
 def build_greedy_par_tree_mtx_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                                     L: int = math.inf, N: int = 1, cpath: set[int] = frozenset(),
                                     delay: int = 1) -> tuple[lp.LpProblem, dict[int, dict[int, lp.LpVariable]]]:
     """
-    Generate the ILP model.
+    Generate the matrix ILP model using greedy subcase building and parallel metric calculation.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Empty decision variable matrix
     X = {j: {} for j in filter(lambda n: n is not PLATFORM, tree)}
     # Objective
@@ -219,15 +245,16 @@
     return model, X
 
 
 def build_par_tree_mtx_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                              L: int = math.inf, N: int = 1, cpath: set[int] = frozenset(),
                              delay: int = 1) -> tuple[lp.LpProblem, dict[int, dict[int, lp.LpVariable]]]:
     """
-    Generate the ILP model.
+    Generate the matrix ILP model based on parallel metric calculations.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Decision variable matrix with trivial variables
     X = {j: {j: lp.LpVariable(f"x_{j:02d}_{j:02d}", cat=lp.LpBinary) if j != root else 1}
          for j in tree.nodes if j is not PLATFORM}
@@ -285,21 +312,23 @@
         model += sum_lat <= L, LP_LAT
     else:
         # Add redundant constraint to implicitly calculate the latency value
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
-def tree_par_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
-                              cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                              timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+def tree_par_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                              N: int = 1, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
+                              timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculate minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculate minimal-cost partitioning of a tree based on matrix LP formulation.
+
+    Block metrics are calculated based on parallelized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param N:       available CPU  core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
@@ -321,21 +350,21 @@
     else:
         return INFEASIBLE
 
 
 ########################################################################################################################
 
 
-def all_par_tree_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
-                                  cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                                  timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+def all_par_tree_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                                  N: int = 1, cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
+                                  timeout: int = None, **lpargs) -> list[T_RESULTS]:
     """
     Calculate all minimal-cost partitioning variations of a tree based on matrix ILP formulation.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param N:       available CPU  core count
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/par/pseudo.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,40 +16,45 @@
 import math
 import operator
 import typing
 import warnings
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.tree.ser.pseudo import SubLTreePart, OPT
 from slambuc.alg.util import (ipostorder_dfs, ileft_right_dfs, ibacktrack_chain, recreate_subtree_blocks,
                               par_inst_count, verify_limits)
 
 
 class SubParBTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given subcase"""
+    """Store subtree partitioning attributes for a given subcase."""
     cost: int = math.inf  # Optimal sum cost of the subtree partitioning (OPT)
     top_cost: int = math.inf  # Cost of the topmost subtree block
     top_blk: set[int] = set()  # Nodes of the topmost block
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
-def pseudo_par_btree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
-                                  L: int = math.inf, N: int = 1, cp_end: int = None, delay: int = 1,
-                                  bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+def pseudo_par_btree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
+                                  cp_end: int = None, delay: int = 1, bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying bottom-up tree traversal approach.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Block metrics are calculated based on parallelized execution platform model.
+
+    Provide suboptimal partitioning due to the inaccurate latency calculation that directly comes from the bottom-up
+    tree traversal approach.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param N:               available CPU core count
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
@@ -162,22 +167,24 @@
         # No feasible solution
         return INFEASIBLE
 
 
 ########################################################################################################################
 
 
-def pseudo_par_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
-                                  L: int = math.inf, N: int = 1, cp_end: int = None, delay: int = 1,
-                                  bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+def pseudo_par_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, N: int = 1,
+                                  cp_end: int = None, delay: int = 1, bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying left-right tree traversal approach.
+
+    Block metrics are calculated based on parallelized execution platform model.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param N:               available CPU core count
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/par/pseudo_mp.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/par/pseudo_mp.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,28 +14,44 @@
 import collections
 import math
 import multiprocessing
 import operator
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.tree.ser.pseudo import SubBTreePart, SubLTreePart, OPT
 from slambuc.alg.tree.ser.pseudo_mp import isubtree_splits
 from slambuc.alg.util import (ipostorder_dfs, ibacktrack_chain, recreate_subtree_blocks, ileft_right_dfs,
                               par_inst_count, verify_limits)
 
 
 def _par_ltree_partitioning(ready: multiprocessing.SimpleQueue, sync: dict[int, multiprocessing.SimpleQueue],
                             tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                             N: int = 1, cpath: set[int] = frozenset(), delay: int = 1,
                             bidirectional: bool = True) -> None | dict[int, SubBTreePart]:
     """
-    Calculates minimal-cost partitioning of a subgraph with *root* while waits for subcases at sync edges.
+    Calculates minimal-cost partitioning of a subgraph with *root* node using the left-right tree traversal approach
+    while waits for subcases at *sync* edges.
+
+    This function is designed for running in a separate detached subprocess and synchronizing subresults via
+    *SimpleQueue* objects as an IPC method.
+
+    :param ready:           object for signaling the end of partitioning
+    :param sync:            object regarding subtrees which results need to be waited for
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:            root node of the graph
+    :param M:               upper memory bound of the partition blocks in MB
+    :param L:               latency limit defined on the critical path in ms
+    :param N:               available CPU core count
+    :param cpath:           critical path nodes
+    :param delay:           invocation delay between blocks
+    :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
+    :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
     """
     # Allocate empty dict for local subcases combined with prior subcase results
     TDP = {}
     # Process subtrees of T in a bottom-up traversal order
     for p, n in ipostorder_dfs(tree, root):
         # Init empty data structure for optimal subcases T_n[v,b]
         DP = collections.defaultdict(lambda: collections.defaultdict(dict))
@@ -144,20 +160,26 @@
         TDP[n] = {lat_n: min(dp.values(), key=operator.itemgetter(OPT)) for lat_n, dp in DP[n, n_w].items()}
     # Notify waiting process and push optimal subcases or return TDP locally for the main thread
     return ready.put(TDP) if ready else TDP
 
 
 def pseudo_par_mp_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                      N: int = 1, cp_end: int = None, delay: int = 1,
-                                     bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                     bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
     memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Partitioning is calculated using the left-right tree traversal approach.
+
+    Arbitrary disjoint subtrees are partitioned in separate subprocesses.
+
+    Block metrics are calculated based on parallelized execution platform model.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param N:               available CPU core count
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/__init__.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/bicriteria.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/bicriteria.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,41 +15,52 @@
 import itertools
 import math
 import operator
 import typing
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.service.common import WEIGHT
 from slambuc.alg.util import (ipostorder_dfs, ileft_right_dfs, ibacktrack_chain, recreate_subtree_blocks,
                               recalculate_ser_partitioning, ipostorder_edges, verify_limits)
 
 # Constants for attribute index
 OPT = 0
 
 
 class WeightedSubBTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given edge-weighted subcase"""
+    """Store subtree partitioning attributes for a given edge-weighted subcase."""
     weight: int = 0  # Cumulative weights of covered edges in the subtree partitioning
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def biheuristic_btree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                    cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                                   bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                   bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying the bottom-up tree traversal approach.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Cost approximation ratio *Epsilon* controls the maximum deviation from the cost-optimal partitioning
+    (Epsilon=0.0 enforces the algorithm to calculate exact solution) in exchange for reduces subcase calculations.
+
+    Latency approximation ratio (*Lambda*) controls the maximum deviation with respect to the latency limit $L$
+    (Lambda=0.0 enforces no rounding) in exchange for reduces subcase calculations.
+    
+    Block metrics are calculated based on serialized execution platform model.
+
+    Provide suboptimal partitioning due to the simplified and inaccurate latency rounding.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
@@ -170,20 +181,25 @@
     else:
         # No feasible solution
         return INFEASIBLE
 
 
 def biheuristic_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                   cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                                  bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                  bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying the bottom-up tree traversal approach.
+
+    Provide suboptimal partitioning due to the simplified and inaccurate latency rounding.
+
+    Recalculates original sum cost and latency metrics.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
@@ -198,32 +214,41 @@
         return INFEASIBLE
 
 
 ########################################################################################################################
 
 
 class WeightedSubLTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given edge-weighted subcase"""
+    """Store subtree partitioning attributes for a given edge-weighted subcase."""
     weight: int = 0  # Cumulative weights of covered edges in the subtree partitioning
     top_lat: int = 0  # Calculated latency for the topmost partition block
     mul: int = 1  # Last serialization multiplier of the top/first block of the subtree partitioning
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def bifptas_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                               bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                               bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying the left-right tree traversal approach.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Cost approximation ratio *Epsilon* controls the maximum deviation from the cost-optimal partitioning
+    (Epsilon=0.0 enforces the algorithm to calculate exact solution) in exchange for reduces subcase calculations.
+
+    Latency violation ratio (*Lambda*) controls the maximum violating deviation from the latency limit $L$
+    (Lambda=0.0 enforces no violation)  in exchange for reduces subcase calculations.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
@@ -365,20 +390,23 @@
     else:
         # No feasible solution
         return INFEASIBLE
 
 
 def bifptas_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                               cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                              bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                              bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying the left-right tree traversal approach.
+
+    Recalculates original sum cost and latency metrics.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
@@ -393,32 +421,44 @@
         return INFEASIBLE
 
 
 ########################################################################################################################
 
 
 class WeightedDualSubLTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given edge-weighted subcase"""
+    """Store subtree partitioning attributes for a given edge-weighted subcase."""
     mem: int = 0  # Memory demand of the topmost block in the subtree partitioning
     top_lat: int = 0  # Calculated latency for the topmost partition block
     mul: int = 1  # Last serialization multiplier of the top/first block of the subtree partitioning
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def bifptas_dual_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                     cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                                    bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                    bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying the left-right tree traversal approach.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Cost approximation ratio *Epsilon* controls the maximum deviation from the cost-optimal partitioning
+    (Epsilon=0.0 enforces the algorithm to calculate exact solution) in exchange for reduces subcase calculations.
+
+    Latency violation ratio (*Lambda*) controls the maximum violating deviation from the latency limit $L$
+    (Lambda=0.0 enforces no violation)  in exchange for reduces subcase calculations.
+
+    Instead of direct cost calculations, the cumulative overheads of externalized states are subject to minimization
+    as a different formalization of the same optimization problem.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
@@ -539,20 +579,31 @@
     else:
         # No feasible solution
         return INFEASIBLE
 
 
 def bifptas_dual_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                                    cp_end: int = None, delay: int = 1, Epsilon: float = 0.0, Lambda: float = 0.0,
-                                   bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                   bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying a different formalization of the optimal partitioning problem.
+
+    Cost approximation ratio *Epsilon* controls the maximum deviation from the cost-optimal partitioning
+    (Epsilon=0.0 enforces the algorithm to calculate exact solution) in exchange for reduces subcase calculations.
+
+    Latency violation ratio (*Lambda*) controls the maximum violating deviation from the latency limit $L$
+    (Lambda=0.0 enforces no violation)  in exchange for reduces subcase calculations.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    Recalculates original sum cost and latency metrics.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param Epsilon:         weight factor for state space trimming (0 <= Eps < 1, Eps = 0 falls back to exact calc.)
     :param Lambda:          latency factor for state space trimming (0 <= Lambda, Lambda = 0 falls back to exact calc.)
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/greedy.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/greedy.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,41 +11,46 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import math
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_BARRS_GEN, T_RESULTS
 from slambuc.alg.util import (isubtrees, ipowerset, ibacktrack_chain, ser_subtree_memory, ser_subtree_cost,
                               ser_subchain_latency)
 
 
-def isubtrees_exhaustive(tree: nx.DiGraph, root: int, M: int) -> list[int]:
-    """Calculate all combination of edge cuts and returns only if it is feasible wrt. the memory limit M.
+def isubtrees_exhaustive(tree: nx.DiGraph, root: int, M: int) -> T_BARRS_GEN:
+    """
+    Calculate all combinations of edge cuts and returns only if it is feasible wrt. the memory limit *M*.
+
+    Block metrics are calculated based on serialized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound in MB
     :return:        generator of chain partitions
     """
     for cuts in ipowerset(tree.edges(range(1, len(tree)))):
         barrs = {root}.union(v for _, v in cuts)
         # Check whether the subtrees meet the memory requirement M
         feasible_subtrees = [b for b, nodes in isubtrees(tree, barrs) if ser_subtree_memory(tree, nodes) <= M]
         if len(feasible_subtrees) == len(barrs):
             yield feasible_subtrees
 
 
 def greedy_ser_tree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
-                                 cp_end: int = None, delay: int = 1) -> list[tuple[list, int, int]]:
+                                 cp_end: int = None, delay: int = 1) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) by iterating over all possible cuttings.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :return:        tuple of list of best partitions, sum cost of the partitioning, and resulted latency
     """
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/ilp.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,55 +10,76 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import collections
 import itertools
 import math
+from collections.abc import Generator
 
 import networkx as nx
 import pulp as lp
 
-from slambuc.alg import LP_LAT, INFEASIBLE
+from slambuc.alg import LP_LAT, INFEASIBLE, T_RESULTS, T_PART
 from slambuc.alg.service import *
 from slambuc.alg.util import (ipowerset, ipostorder_dfs, ibacktrack_chain, recreate_subtree_blocks, induced_subtrees,
                               ser_subtree_cost, ser_subchain_latency, ser_subtree_memory, verify_limits, x_eval)
 
 
-def ifeasible_greedy_subtrees(tree: nx.DiGraph, root: int, M: int) -> list[list[int]]:
-    """Generate feasible subtrees in combinatorial way, which meet the connectivity and memory constraint *M*"""
+def ifeasible_greedy_subtrees(tree: nx.DiGraph, root: int, M: int) -> Generator[tuple[int, set[int]]]:
+    """
+    Generate feasible subtrees in a combinatorial way, which meet the connectivity and memory constraint *M*.
+    
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param M:       upper memory bound of the partition blocks (in MB)
+    :return:        generator of subtree root and regarding subtree nodes
+    """
     for st in ipowerset(tuple(filter(lambda n: n is not PLATFORM, tree)), start=1):
         st = set(st)
         for v in itertools.islice(sorted(st, reverse=True), len(st) - 1):
             if next(tree.predecessors(v)) not in st:
                 break
         else:
             if ser_subtree_memory(tree, st) <= M:
                 yield min(st), st
 
 
-def ifeasible_subtrees(tree: nx.DiGraph, root: int, M: int, filtered: bool = True) -> tuple[int, list[list[int]]]:
-    """Generate feasible(connected) subtrees and roots in bottom-up way, which meet the memory constraint *M*"""
+def ifeasible_subtrees(tree: nx.DiGraph, root: int, M: int, filtered: bool = True) -> Generator[tuple[int, set[int]]]:
+    """
+    Generate M-feasible(connected) subtrees and roots in a bottom-up way, which meet the memory constraint *M*.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:        service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:        root node of the graph
+    :param M:           upper memory bound of the partition blocks (in MB)
+    :param filtered:    filter our infeasible subtrees
+    :return:            generator of subtree root and regarding subtree nodes
+    """
     subtrees = collections.defaultdict(list)
     for _, n in ipostorder_dfs(tree, root):
         for children in ipowerset(tuple(tree.successors(n))):
             for sts in itertools.product(*(subtrees[c] for c in children)):
                 st = {n}.union(*sts)
                 if not filtered or ser_subtree_memory(tree, st) <= M:
                     subtrees[n].append(st)
                     yield n, st
         for c in tree.succ[n]:
             del subtrees[c]
 
 
-def build_tree_cfg_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
-                         L: int = math.inf, cpath: set[int] = frozenset(), delay: int = 1,
+def build_tree_cfg_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                         cpath: set[int] = frozenset(), delay: int = 1,
                          isubtrees: iter = ifeasible_subtrees) -> tuple[lp.LpProblem, dict[int, list[lp.LpVariable]]]:
     """
-    Generate the ILP model.
+    Generate the configuration ILP model using serialized metric calculation.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Decision variables with precalculated coefficients
     c_x, l_x, X_n = [], [], collections.defaultdict(list)
     for i, (b, nodes) in enumerate(isubtrees(tree, root, M)):
@@ -83,19 +104,22 @@
     # Latency constraint
     model += lp.lpSum(l_x) <= L if L < math.inf else lp.lpSum(l_x) >= 0, LP_LAT
     return model, X_n
 
 
 def tree_cfg_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                           cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                          timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+                          timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculates minimal-cost partitioning of a tree based on configuration LP formulation and greedy subcase
+    generation.
+    
+    Block metrics are calculated based on serialized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
     :param timeout: time limit in sec
@@ -115,19 +139,22 @@
         return recreate_subtrees_from_xdict(tree, X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
 def tree_hybrid_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                              cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                             timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+                             timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a tree based on configuration LP formulation.
+    Calculates minimal-cost partitioning of a tree based on configuration LP formulation and hybrid subcase
+    generation.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
     :param timeout: time limit in sec
@@ -145,33 +172,47 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = lp.value(model.objective), lp.value(model.constraints[LP_LAT])
         return recreate_subtrees_from_xdict(tree, X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def extract_subtrees_from_xdict(model: lp.LpProblem) -> list[list[int]]:
-    """Recreate partitioning blocks from metadata cached in variables objects"""
+def extract_subtrees_from_xdict(model: lp.LpProblem) -> T_PART:
+    """
+    Recreate partitioning blocks from metadata cached in variables objects.
+
+    :param model:   LP problem model
+    :return:        calculated partitioning
+    """
     return sorted(x.blk for x in filter(lambda x: round(x.varValue) == 1, model.variables()))
 
 
-def recreate_subtrees_from_xdict(tree: nx.DiGraph, Xn: dict[int, list[lp.LpVariable]]) -> list[list[int]]:
-    """Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks"""
+def recreate_subtrees_from_xdict(tree: nx.DiGraph, Xn: dict[int, list[lp.LpVariable]]) -> T_PART:
+    """
+    Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param Xn:      specific structure of decision variables
+    :return:        calculated partitioning
+    """
     barr = set(int(next(filter(lambda x: round(x.varValue) == 1, x_n)).name.split('_', 2)[1]) for x_n in Xn.values())
     return recreate_subtree_blocks(tree=tree, barr=barr)
 
 
 ########################################################################################################################
 
 
 def build_greedy_tree_mtx_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                                 L: int = math.inf, cpath: set[int] = frozenset(),
                                 delay: int = 1) -> tuple[lp.LpProblem, dict[int, dict[int, lp.LpVariable]]]:
     """
-    Generate the matrix ILP model.
+    Generate the matrix ILP model in a greedy manner.
+
+    Block metrics are calculated based on serialized execution platform model.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Empty decision variable matrix
     X = {j: {} for j in filter(lambda n: n is not PLATFORM, tree)}
     # Objective
@@ -220,15 +261,18 @@
     return model, X
 
 
 def build_tree_mtx_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                          L: int = math.inf, cpath: set[int] = frozenset(),
                          delay: int = 1) -> tuple[lp.LpProblem, dict[int, dict[int, lp.LpVariable]]]:
     """
-    Generate the matrix ILP model.
+    Generate the matrix ILP model directly from formulas.
+    
+    Block metrics are calculated based on serialized execution platform model.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = lp.LpProblem(name="Tree_Partitioning", sense=lp.LpMinimize)
     # Decision variable matrix with trivial variables
     X = {j: {j: lp.LpVariable(f"x_{j:02d}_{j:02d}", cat=lp.LpBinary) if j != root else 1}
          for j in tree.nodes if j is not PLATFORM}
@@ -279,17 +323,19 @@
         # Add redundant constraint to implicitly calculate the latency value
         model += sum_lat >= 0, LP_LAT
     return model, X
 
 
 def tree_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                           cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
-                          timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
+                          timeout: int = None, **lpargs) -> T_RESULTS:
     """
-    Calculates minimal-cost partitioning of a tree based on matrix ILP formulation.
+    Calculates minimal-cost partitioning of a tree based on the matrix ILP formulation.
+
+    Block metrics are calculated based on serialized execution platform model.
 
     :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
@@ -309,34 +355,47 @@
     if status == lp.LpStatusOptimal:
         opt_cost, opt_lat = round(lp.value(model.objective), 0), round(lp.value(model.constraints[LP_LAT]), 0)
         return extract_subtrees_from_xmatrix(X), opt_cost, L + opt_lat if L < math.inf else opt_lat
     else:
         return INFEASIBLE
 
 
-def recreate_subtrees_from_xmatrix(tree: nx.DiGraph, X: dict[int, dict[int, lp.LpVariable]]) -> list[list[int]]:
-    """Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks"""
+def recreate_subtrees_from_xmatrix(tree: nx.DiGraph, X: dict[int, dict[int, lp.LpVariable]]) -> T_PART:
+    """
+    Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param X:       specific structure of decision variables
+    :return:        calculated partitioning
+    """
     return recreate_subtree_blocks(tree, barr=set(i for i in X if x_eval(X[i][i])))
 
 
-def extract_subtrees_from_xmatrix(X: dict[int, dict[int, lp.LpVariable]]) -> list[list[int]]:
-    """Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks"""
+def extract_subtrees_from_xmatrix(X: dict[int, dict[int, lp.LpVariable]]) -> T_PART:
+    """
+    Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks.
+    
+    :param X:   specific structure of decision variables
+    :return:    calculated partitioning
+    """
     return [[i for i in sorted(X) if j in X[i] and x_eval(X[i][j])] for j in sorted(X) if x_eval(X[j][j])]
 
 
 ########################################################################################################################
 
 
 def all_tree_mtx_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                               cp_end: int = None, delay: int = 1, solver: lp.LpSolver = None,
                               timeout: int = None, **lpargs) -> tuple[list[list[int]], int, int]:
     """
     Calculates all minimal-cost partitioning variations of a tree based on matrix ILP formulation.
+    
+    Block metrics are calculated based on serialized execution platform model.
 
-    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rate
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
     :param cp_end:  tail node of the critical path in the form of subchain[root -> c_pend]
     :param delay:   invocation delay between blocks
     :param solver:  specific solver class (default: COIN-OR CBC)
     :param timeout: time limit in sec
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/ilp_cplex.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/ilp_cplex.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,36 +14,36 @@
 import collections
 import math
 import sys
 import warnings
 
 import docplex
 import docplex.cp.model as cpo
-import docplex.mp.dvar as var
 import docplex.mp.model as cpx
 import networkx as nx
 
 if sys.version_info.minor > 10 and docplex.docplex_version_minor <= 25:
     warnings.warn(f"docplex[{docplex.version.docplex_version_string}] package does not support Python version >3.10!")
 
-from slambuc.alg import LP_LAT, INFEASIBLE
+from slambuc.alg import LP_LAT, INFEASIBLE, T_RESULTS, T_PART
 from slambuc.alg.service import *
 from slambuc.alg.tree.ser.ilp import ifeasible_subtrees
 from slambuc.alg.util import (ibacktrack_chain, induced_subtrees, ser_subchain_latency, ser_subtree_cost,
                               recreate_subtree_blocks, verify_limits)
 from slambuc.misc.util import get_cpo_path
 
 CPO_PATH = get_cpo_path()
 
 
 def build_tree_cfg_cpo_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                              L: int = math.inf, cpath: set[int] = frozenset(), delay: int = 1,
                              isubtrees: iter = ifeasible_subtrees) -> tuple[cpo.CpoModel, list[cpo.CpoIntVar]]:
     """
     Generate the configuration CP model.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = cpo.CpoModel(name="Tree_Partitioning")
     # Decision variables with precalculated coefficients
     c_x, l_x, X_n = [], [], collections.defaultdict(list)
     for i, (b, nodes) in enumerate(isubtrees(tree, root, M)):
@@ -81,15 +81,15 @@
     context.model.sort_names = None
     context.solver.trace_cpo = False
     context.solver.trace_log = False
     context.solver.add_log_to_solution = False
 
 
 def tree_cpo_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, cp_end: int = None,
-                          delay: int = 1, **kwargs) -> tuple[list[list[int]], int, int]:
+                          delay: int = 1, **kwargs) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a tree based on configuration CP formulation.
 
     :param tree:      service graph annotated with node runtime(ms), memory(MB) and edge rate
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
@@ -109,28 +109,36 @@
         opt_cost, opt_lat = result.get_objective_values()[0], result.solution.get_kpis()[LP_LAT]
         return recreate_subtrees_from_cpo_xdict(tree, result, Xn), round(opt_cost, ndigits=6), round(opt_lat, ndigits=6)
     else:
         return INFEASIBLE
 
 
 def recreate_subtrees_from_cpo_xdict(tree: nx.DiGraph, result: cpo.CpoSolveResult,
-                                     Xn: dict[int, list[cpo.CpoIntVar]]) -> list[list[int]]:
-    """Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks"""
+                                     Xn: dict[int, list[cpo.CpoIntVar]]) -> T_PART:
+    """
+    Extract barrier nodes from variable names (x_{b}_{w}) and recreate partitioning blocks.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param result:  result object
+    :param Xn:      specific structure of decision variables
+    :return:        calculated partitioning
+    """
     barr = set(int(next(filter(lambda x: result[x], x_n)).name.split('_', 2)[1]) for x_n in Xn.values())
     return recreate_subtree_blocks(tree=tree, barr=barr)
 
 
 ########################################################################################################################
 
 
 def build_greedy_tree_cplex_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                                   L: int = math.inf, cpath: set[int] = frozenset(),
-                                  delay: int = 1) -> tuple[cpx.Model, dict[int, dict[int, var]]]:
+                                  delay: int = 1) -> tuple[cpx.Model, dict[int, dict[int, docplex.mp.dvar]]]:
     """
     Generate the matrix ILP model using CPLEX Python binding.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = cpx.Model(name="Tree_Partitioning")
     # Empty decision variable matrix
     X = {j: {} for j in filter(lambda n: n is not PLATFORM, tree)}
     # Objective
@@ -177,17 +185,18 @@
     # Add calculated sum latency as KPI for tracking
     model.add_kpi(sum_lat, LP_LAT)
     return model, X
 
 
 def build_tree_cplex_model(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                            L: int = math.inf, cpath: set[int] = frozenset(),
-                           delay: int = 1) -> tuple[cpx.Model, dict[int, dict[int, var]]]:
+                           delay: int = 1) -> tuple[cpx.Model, dict[int, dict[int, docplex.mp.dvar]]]:
     """
     Generate the matrix ILP model using CPLEX Python binding.
+
     :return: tuple of the created model and list of decision variables
     """
     # Model
     model = cpx.Model(name="Tree_Partitioning")
     # Decision variable matrix with trivial variables
     X = {j: {j: model.binary_var(f"x_{j:02d}_{j:02d}")} for j in tree.nodes if j is not PLATFORM}
     # Empty objective
@@ -234,16 +243,16 @@
     if L < math.inf:
         model.add_constraint(sum_lat <= L, ctname=LP_LAT)
     # Add calculated sum latency as KPI for tracking
     model.add_kpi(sum_lat, LP_LAT)
     return model, X
 
 
-def tree_cplex_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, cp_end: int = None,
-                            delay: int = 1, **kwargs) -> tuple[list[list[int]], int, int]:
+def tree_cplex_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
+                            cp_end: int = None, delay: int = 1, **kwargs) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a tree based on matrix CPLEX ILP formulation.
 
     :param tree:      service graph annotated with node runtime(ms), memory(MB) and edge rate
     :param root:    root node of the graph
     :param M:       upper memory bound of the partition blocks (in MB)
     :param L:       latency limit defined on the critical path (in ms)
@@ -262,11 +271,16 @@
     if solution is not None:
         opt_cost, opt_lat = solution.get_objective_value(), model.kpi_value_by_name(LP_LAT)
         return extract_subtrees_from_cplex_xmatrix(X), round(opt_cost, ndigits=6), round(opt_lat, ndigits=6)
     else:
         return INFEASIBLE
 
 
-def extract_subtrees_from_cplex_xmatrix(X: dict[int, dict[int, var]]) -> list[list[int]]:
-    """Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks"""
+def extract_subtrees_from_cplex_xmatrix(X: dict[int, dict[int, docplex.mp.dvar]]) -> T_PART:
+    """
+    Extract barrier nodes from variable matrix(dict-of-dict) and recreate partitioning blocks.
+
+    :param X:   specific structure of decision variables
+    :return:    calculated partitioning
+    """
     return [[i for i in sorted(X) if j in X[i] and round(X[i][j].solution_value, ndigits=6) == 1]
             for j in sorted(X) if round(X[j][j].solution_value, ndigits=6) == 1]
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/pseudo.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,38 +15,41 @@
 import itertools
 import math
 import operator
 import typing
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.util import ipostorder_dfs, ileft_right_dfs, ibacktrack_chain, recreate_subtree_blocks, verify_limits
 
 # Constants for attribute index
 OPT = 0
 
 
 class SubBTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given subcase"""
+    """Store subtree partitioning attributes for a given subcase."""
     cost: int = math.inf  # Sum cost of the subtree partitioning
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def pseudo_btree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, cp_end: int = None,
-                              delay: int = 1, bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                              delay: int = 1, bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying bottom-up tree traversal approach.
+    
+    Block metrics are calculated based on serialized execution platform model.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
     :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
@@ -137,30 +140,33 @@
         return INFEASIBLE
 
 
 ########################################################################################################################
 
 
 class SubLTreePart(typing.NamedTuple):
-    """Store subtree partitioning attributes for a given subcase"""
+    """Store subtree partitioning attributes for a given subcase."""
     cost: int = math.inf  # Sum cost of the subtree partitioning
     mul: int = 1  # Last serialization multiplier of the top/first block of the subtree partitioning
     barr: set[int] = set()  # Barrier/heading nodes of the given subtree partitioning
 
     def __repr__(self):
         return repr(tuple(self))
 
 
 def pseudo_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf, cp_end: int = None,
-                              delay: int = 1, bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                              delay: int = 1, bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
-    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
+    memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes, while
+    applying left-right tree traversal approach.
+    
+    Block metrics are calculated based on serialized execution platform model.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
     :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
```

### Comparing `SLAMBUC-0.1.0/slambuc/alg/tree/ser/pseudo_mp.py` & `SLAMBUC-0.2.0/slambuc/alg/tree/ser/pseudo_mp.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,48 +13,72 @@
 # limitations under the License.
 import collections
 import heapq
 import itertools
 import math
 import multiprocessing
 import operator
+from collections.abc import Generator
 
 import networkx as nx
 
-from slambuc.alg import INFEASIBLE
+from slambuc.alg import INFEASIBLE, T_RESULTS
 from slambuc.alg.service import *
 from slambuc.alg.tree.ser.pseudo import SubBTreePart, SubLTreePart, OPT
 from slambuc.alg.util import (ipostorder_dfs, ibacktrack_chain, recreate_subtree_blocks, ipostorder_tabu_dfs,
                               ileft_right_dfs, verify_limits)
 
 
 def isubtree_cutoffs(tree: nx.DiGraph, root: int = 1, lb: int = 1, ub: int = math.inf) -> tuple[tuple[int, int], int]:
-    """Recursively return edges that cut off non-trivial subtrees from *tree* with size between *lb* and *ub*"""
+    """
+    Recursively return edges that cut off non-trivial subtrees from *tree* with size between *lb* and *ub*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param lb:      lower size bound
+    :param ub:      upper size bound
+    :return:        cut barrier node, branches and subtree root
+    """
     _tmp = {}
     for _, v in ipostorder_dfs(tree, root, inclusive=True):
         # Sum the size of descendant subtrees
         if len(brs := _tmp.setdefault(v, {s: sum(_tmp.pop(s).values(), start=1) for s in tree.successors(v)})) > 1:
             # Only consider subtrees with proper size
             for br, st in brs.items():
                 if lb <= st:
                     if ub <= st:
                         _tmp[v][br] = 0
                     yield (v, br), st
 
 
 def get_cpu_splits(tree: nx.DiGraph, root: int = 1, workers: int = None) -> tuple[tuple[int, int]]:
-    """Calculate the cuts for parallelization based on *workers* count and subtree size heuristics"""
+    """
+    Calculate the cuts for parallelization based on *workers* count and subtree size heuristics.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param workers: workers count
+    :return:        cut edges
+    """
     ub = math.sqrt(len(tree) - 1)
     lb = ub if not workers else 1
     n = workers if workers else ub
     return [e for e, _ in heapq.nlargest(n, list(isubtree_cutoffs(tree, root, lb, ub)), key=operator.itemgetter(1))]
 
 
-def isubtree_sync_cutoffs(tree: nx.DiGraph, root: int = 1, size: int = math.inf) -> tuple[tuple[int], int, set[int]]:
-    """Recursively return edges that cut off non-trivial subtrees from *tree* with given *size*"""
+def isubtree_sync_cutoffs(tree: nx.DiGraph, root: int = 1,
+                          size: int = math.inf) -> Generator[tuple[tuple[int], int, set[int]]]:
+    """
+    Recursively return edges that cut off non-trivial subtrees from *tree* with given *size*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :param size:    subtree min size
+    :return:        generator of cut edge, subtree root, and related branches
+    """
     _tmp, sync = {}, collections.defaultdict(set)
     for _, v in ipostorder_dfs(tree, root, inclusive=True):
         # Sum the size of descendant subtrees
         brs = _tmp.setdefault(v, {s: sum(_tmp.pop(s).values(), start=0 if s in sync else 1)
                                   for s in tree.successors(v)}).items()
         for br, st in brs:
             # Only consider subtrees with proper size
@@ -68,28 +92,50 @@
             elif br in sync:
                 # Mark as a dependent node and propagate sync points
                 sync[v].update(sync[br])
         if v == root:
             yield (PLATFORM, root), None, sync[root]
 
 
-def isubtree_splits(tree: nx.DiGraph, root: int = 1) -> tuple[tuple[int, int], set[int]]:
-    """Return the heuristic cutoff edges of given *tree* along with the mandatory synchronization points"""
+def isubtree_splits(tree: nx.DiGraph, root: int = 1) -> Generator[tuple[tuple[int], int, set[int]]]:
+    """
+    Return the heuristic cutoff edges of given *tree* along with the mandatory synchronization points by assuming
+    the subtree size equals *sqrt(n)*.
+
+    :param tree:    service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:    root node of the graph
+    :return:        generator of cut edge, subtree root, and related branches
+    """
     yield from ((c, sync) for c, _, sync in isubtree_sync_cutoffs(tree, root, math.ceil(math.sqrt(len(tree) - 1))))
 
 
 ########################################################################################################################
 
 
 def _btree_partitioning(ready: multiprocessing.SimpleQueue, sync: dict[int, multiprocessing.SimpleQueue],
                         tree: nx.DiGraph, root: int = 1, M: int = math.inf, L: int = math.inf,
                         cpath: set[int] = frozenset(), delay: int = 1,
                         bidirectional: bool = True) -> None | dict[tuple[int, int], dict[int, SubBTreePart]]:
     """
-    Calculates minimal-cost partitioning of a subgraph with *root* while waits for subcases at sync edges.
+    Calculates minimal-cost partitioning of a subgraph with *root* using the bottom-up tree traversal approach
+    while waits for subcases at sync edges.
+
+    This function is designed for running in a separate detached subprocess and synchronizing subresults via
+    *SimpleQueue* objects as an IPC method.
+
+    :param ready:           object for signaling the end of partitioning
+    :param sync:            object regarding subtrees which results need to be waited for
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:            root node of the graph
+    :param M:               upper memory bound of the partition blocks in MB
+    :param L:               latency limit defined on the critical path in ms
+    :param cpath:           critical path nodes
+    :param delay:           invocation delay between blocks
+    :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
+    :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
     """
     # Allocate empty dict for local subcases combined with prior subcase results
     DP = {}
     # Iterate nodes in a bottom-up traversal order except the subtrees of the sync points
     for p, v in ipostorder_tabu_dfs(tree, root, tabu=sync):
         r_v, d_v, t_v, m_v = tree[p][v][RATE], tree[p][v][DATA], tree.nodes[v][RUNTIME], tree.nodes[v][MEMORY]
         # SINGLETON: calculate the default subcase of singleton partition of node v
@@ -167,20 +213,26 @@
             sub_v[OPT] = min(sub_v.values(), key=operator.itemgetter(0))
     # Notify waiting process and push optimal subcases or return TDP locally for the main thread
     return ready.put(DP[root]) if ready else DP
 
 
 def pseudo_mp_btree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                                  L: int = math.inf, cp_end: int = None, delay: int = 1,
-                                 bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                 bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
     memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Partitioning is calculated using the bottom-up tree traversal approach.
+
+    Arbitrary disjoint subtrees are partitioned in separate subprocesses.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
     :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
@@ -233,15 +285,30 @@
 
 
 def _ltree_partitioning(ready: multiprocessing.SimpleQueue, sync: dict[int, multiprocessing.SimpleQueue],
                         tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                         L: int = math.inf, cpath: set[int] = frozenset(), delay: int = 1,
                         bidirectional: bool = True) -> None | dict[int, dict[int, SubBTreePart]]:
     """
-    Calculates minimal-cost partitioning of a subgraph with *root* while waits for subcases at sync edges.
+    Calculates minimal-cost partitioning of a subgraph with *root* using the left-right tree traversal approach
+    while waits for subcases at sync edges.
+
+    This function is designed for running in a separate detached subprocess and synchronizing subresults via
+    *SimpleQueue* objects as an IPC method.
+
+    :param ready:           object for signaling the end of partitioning
+    :param sync:            object regarding subtrees which results need to be waited for
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
+    :param root:            root node of the graph
+    :param M:               upper memory bound of the partition blocks in MB
+    :param L:               latency limit defined on the critical path in ms
+    :param cpath:           critical path nodes
+    :param delay:           invocation delay between blocks
+    :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
+    :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
     """
     # Allocate empty dict for local subcases combined with prior subcase results
     TDP = {}
     # Process subtrees of T in a bottom-up traversal order
     for p, n in ipostorder_tabu_dfs(tree, root, tabu=sync):
         # Init empty data structure for optimal subcases T_n[v,b]
         DP = collections.defaultdict(lambda: collections.defaultdict(dict))
@@ -331,20 +398,26 @@
         TDP[n] = {lat_n: min(dp.values(), key=operator.itemgetter(OPT)) for lat_n, dp in DP[n, n_w].items()}
     # Notify waiting process and push optimal subcases or return TDP locally for the main thread
     return ready.put(TDP) if ready else TDP
 
 
 def pseudo_mp_ltree_partitioning(tree: nx.DiGraph, root: int = 1, M: int = math.inf,
                                  L: int = math.inf, cp_end: int = None, delay: int = 1,
-                                 bidirectional: bool = True) -> tuple[list[list[int]], int, int]:
+                                 bidirectional: bool = True) -> T_RESULTS:
     """
     Calculates minimal-cost partitioning of a service graph(tree) with respect to an upper bound **M** on the total
     memory of blocks and a latency constraint **L** defined on the subchain between *root* and *cp_end* nodes.
 
-    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rate and data
+    Partitioning is calculated using the left-right tree traversal approach.
+
+    Arbitrary disjoint subtrees are partitioned in separate subprocesses.
+
+    Block metrics are calculated based on serialized execution platform model.
+
+    :param tree:            service graph annotated with node runtime(ms), memory(MB) and edge rates and data overheads(ms)
     :param root:            root node of the graph
     :param M:               upper memory bound of the partition blocks in MB
     :param L:               latency limit defined on the critical path in ms
     :param cp_end:          tail node of the critical path in the form of subchain[root -> cp_end]
     :param delay:           invocation delay between blocks
     :param bidirectional:   use bidirectional subcase elimination (may introduce quadratic increase in the worst case)
     :return:                tuple of optimal partitioning, reached sum cost and latency on the critical path
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/__init__.py` & `SLAMBUC-0.2.0/slambuc/gen/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/__init__.py` & `SLAMBUC-0.2.0/slambuc/gen/cluster/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/cpl_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/cpl_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/instance_num_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/instance_num_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/level_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/level_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_duration_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_duration_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_mem_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_mem_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/hist/task_num_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/cluster/hist/task_num_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/job_tree.py` & `SLAMBUC-0.2.0/slambuc/gen/cluster/job_tree.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import pathlib
 import random
+from collections.abc import Generator
 
 import networkx as nx
 import numpy as np
 import pandas as pd
 import scipy
 
 from slambuc.alg.service.common import *
@@ -39,15 +40,23 @@
 DEF_DATA_FACTOR = 0.2
 
 DEF_JOB_TREE_PREFIX = "job_tree"
 
 
 def convert_tasks_to_dag(job_name: str, tasks: pd.DataFrame, mem_max: int = DEF_MEM_MAX,
                          data_mean: int = None) -> tuple[nx.DiGraph, int]:
-    """Convert the task lines of given job *job_name* into a DAG and return it with the generated front-end root node"""
+    """
+    Convert the task lines of given job *job_name* into a DAG and return it with the generated front-end root node.
+
+    :param job_name:    job name in the dataset
+    :param tasks:       tasks imported from the dataset
+    :param mem_max:     maximum memory to convert memory usage into MB
+    :param data_mean:   dataset overhead mean value for generating artificial values
+    :return:            generated DAG and dispatcher node
+    """
     dag = nx.DiGraph(**{NAME: job_name})
     # Build task DAG
     for _, task in tasks.iterrows():
         # Extract dependencies
         v, *pred = task.task.split('_')
         try:
             v = int(v[1:])
@@ -67,26 +76,39 @@
     data_mean = data_mean if data_mean else DEF_DATA_FACTOR * tasks["duration"].mean()
     # Draw data overhead from exponential distribution with lambda = 1 / avg(runtimes) rounded to integer (min 1)
     data_values = dict(zip(dag.edges, np.ceil(scipy.stats.expon(scale=data_mean).rvs(size=len(dag.edges))).astype(int)))
     nx.set_edge_attributes(dag, values=data_values, name=DATA)
     return dag, DISP_NODE
 
 
-def igenerate_job_tree(job_df: pd.DataFrame, min_size: int = 0) -> nx.DiGraph:
-    """Generate job service trees one-by-one from *min_size*"""
+def igenerate_job_tree(job_df: pd.DataFrame, min_size: int = 0) -> Generator[nx.DiGraph]:
+    """
+    Generate job service trees one-by-one from *min_size*.
+
+    :param job_df:      imported job dataset
+    :param min_size:    minimum tree size
+    :return:            generator of job DAGs
+    """
     jobs = job_df.groupby("job")["task"].count()
     viable_jobs = jobs[min_size <= jobs]
     for job in viable_jobs.index:
         dag, root = convert_tasks_to_dag(job, job_df[job_df["job"] == job])
         if dag is not None:
             yield faasify_dag_by_duplication(dag, root)
 
 
-def igenerate_syn_tree(n: int | tuple[int, int], iteration: int = 1, job_lb: int = 10) -> nx.DiGraph:
-    """Generate job service tree based on empirical distributions"""
+def igenerate_syn_tree(n: int | tuple[int, int], iteration: int = 1, job_lb: int = 10) -> Generator[nx.DiGraph]:
+    """
+    Generate random job service trees based on empirical distributions.
+
+    :param n:           tree size interval
+    :param iteration:   number of trees
+    :param job_lb:      minimum tree size
+    :return:            generator of tree DAGs
+    """
     tree_cntr = i = 0
     while tree_cntr < iteration:
         size = random.randint(job_lb, n[1]) if isinstance(n, tuple) else n
         job_df = random_job(task_num=size)
         dag, root = convert_tasks_to_dag(f"syn_job_{i}", job_df)
         tree = faasify_dag_by_duplication(dag, root)
         if ((isinstance(n, int) and len(tree) - 1 == size) or
@@ -99,15 +121,24 @@
 
 
 ########################################################################################################################
 
 
 def generate_all_job_trees(data_dir: str, task_file: str = DEF_TASK_CSV, start: int = 10, end: int = None,
                            step: int = 10, tree_name: str = DEF_JOB_TREE_PREFIX):
-    """Generate all job service trees with size interval between *start* and *end* and save to separate files"""
+    """
+    Generate all job service trees with size interval between *start* and *end* and save them into separate files.
+
+    :param data_dir:    data directory
+    :param task_file:   task file name
+    :param start:       lower bound of size intervals
+    :param end:         upper bound of size intervals
+    :param step:        step size of intervals
+    :param tree_name:   prefix name of tree files
+    """
     print(f"Load data from {task_file}...")
     job_df = pd.read_csv(task_file, usecols=DEF_TASK_CSV_COLS, names=DEF_TASK_CSV_HEADER)
     trees = [tree for tree in igenerate_job_tree(job_df, min_size=start)]
     max_size = max(map(len, trees)) - 1
     end = end if end is not None else max_size
     print(f"Generated {len(trees)} job trees with {start} <= size <= {max_size}")
     for min_size, max_size in itertools.pairwise(range(start, end + step, step)):
@@ -118,27 +149,47 @@
             print(f"Saving trees into {file_name}...")
             save_trees_to_file(filtered_trees, file_name=file_name, padding=max_size)
     print("Finished")
 
 
 def generate_syn_job_trees(data_dir: str, iteration: int = 100, start: int = 10, end: int = 100, step: int = 10,
                            tree_name: str = DEF_JOB_TREE_PREFIX):
-    """Generate synthetic job service trees with size interval between *start* and *end* and save to separate files"""
+    """
+    Generate synthetic job service trees with size interval between *start* and *end* and save to separate files
+    using extracted empirical distributions.
+
+    :param data_dir:    data directory
+    :param iteration:   number of generated trees
+    :param start:       lower bound of size intervals
+    :param end:         upper bound of size intervals
+    :param step:        step size of intervals
+    :param tree_name:   prefix name of tree files
+    """
     for n in range(start, end + 1, step):
         print(f"Generating synthetic task service trees for {n=} by exhaustive iteration...")
         file_name = pathlib.Path(data_dir, f"syn_{tree_name}_n{n}.npy").resolve()
         output_trees = list(igenerate_syn_tree(n, iteration, job_lb=int(n * 0.5)))
         print(f"Saving trees into {file_name}...")
         save_trees_to_file(output_trees, file_name, padding=n)
     print("Finished")
 
 
 def generate_mixed_job_trees(data_dir: str, task_file: str = DEF_TASK_CSV, iteration: int = 100, start: int = 10,
                              end: int = 100, step: int = 10, tree_name: str = DEF_JOB_TREE_PREFIX):
-    """Generate job trees from sample data and extend it with synthetic trees"""
+    """
+    Generate job trees from sample data and extend it with synthetic trees if necessary.
+
+    :param data_dir:    data directory
+    :param task_file:   task file name
+    :param iteration:   number of generated trees
+    :param start:       minimum of size intervals
+    :param end:         maximum of size intervals
+    :param step:        step size of intervals
+    :param tree_name:   prefix name of tree files
+    """
     print(f"Load data from {task_file}...")
     job_df = pd.read_csv(task_file, usecols=DEF_TASK_CSV_COLS, names=DEF_TASK_CSV_HEADER)
     trees = [tree for tree in igenerate_job_tree(job_df, min_size=start)]
     max_size = max(map(len, trees)) - 1
     end = end if end is not None else max_size
     print(f"Generated {len(trees)} job trees with {start} <= size <= {max_size}...")
     for min_size, max_size in itertools.pairwise(range(start, end + step, step)):
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/samples/batch_task.csv` & `SLAMBUC-0.2.0/slambuc/gen/cluster/samples/batch_task.csv`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/samples/sample_tasks.csv` & `SLAMBUC-0.2.0/slambuc/gen/cluster/samples/sample_tasks.csv`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/cluster/syn_job.py` & `SLAMBUC-0.2.0/slambuc/gen/cluster/syn_job.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 
 HIST_DATA_DIR = pathlib.Path(__file__).parent / "hist"
 DIST_CACHE = {}
 
 
 def draw(hist_name: str, num: int = 1, path: list = tuple(), ndigits: int = 2, positive: bool = True,
          output_integer: bool = False, seed: int = None) -> list[int | float]:
-    """Draw random samples from a given distribution."""
+    """
+    Draw random samples from a given distribution.
+
+    Random job generation source code is moved from package *spar* with adaptations to newer versions of Python3.11
+    and Scipy 1.10.  See also: https://github.com/All-less/trace-generator/blob/master/spar/generate.py
+    """
     if hist_name not in DIST_CACHE:
         with (HIST_DATA_DIR / f"{hist_name}.pkl").open('rb') as f:
             hist = pickle.load(f)
             if isinstance(hist, dict):
                 DIST_CACHE[hist_name] = {num: scipy.stats.rv_histogram(h, density=False, seed=seed)
                                          for num, h in hist.items()}
             else:
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/io.py` & `SLAMBUC-0.2.0/slambuc/gen/io.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,71 +12,111 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import operator
 import pathlib
 import pickle
 import warnings
+from collections.abc import Generator
 
 import networkx as nx
 import numpy as np
 
 from slambuc.alg.service.common import *
 
 
 def encode_service_tree(tree: nx.DiGraph, root: int = 0, pad_size: int = 0) -> np.ndarray[np.int64]:
-    """Encode the given service *tree* into an array with size of **5*n** where n is the size of the tree.
+    """
+    Encode the given service *tree* into an array with size of **5*n** where n is the size of the tree.
+
     The tree must have the tree structure where the root is PLATFORM and the node IDs are increasing integers from *1*
     to *n*. The array's structure is *[r, S_(n-1), R_n, D_n, T_n, M_n]*, where
         - *r* is the root node of the tree (default is PLATFORM that is converted to node *0*),
         - *S_(n-1) is the Prufer sequence of the tree extended with root node PLATFORM,
         - *D_n, R_n* are the ingress edge attributes (DATA, RATE) and
-        - *T_n, M_n* are the node attributes (RUNTIME, MEMORY) of the tree nodes in increasing order from *1* to *n*."""
+        - *T_n, M_n* are the node attributes (RUNTIME, MEMORY) of the tree nodes in increasing order from *1* to *n*.
+
+    :param tree:        service tree
+    :param root:        root node
+    :param pad_size:    padding size for uniform length
+    :return:            encoded tree as value arrays
+    """
     data_seq = np.fromiter(
         itertools.chain(
             [root, *nx.to_prufer_sequence(nx.relabel_nodes(tree.to_undirected(as_view=True), {PLATFORM: root}))],
             (tree[u][v][DATA] for u, v in sorted(tree.edges, key=operator.itemgetter(1))),
             (tree[u][v][RATE] for u, v in sorted(tree.edges, key=operator.itemgetter(1))),
             (tree.nodes[v][RUNTIME] for _, v in sorted(tree.edges, key=operator.itemgetter(1))),
             (tree.nodes[v][MEMORY] for _, v in sorted(tree.edges, key=operator.itemgetter(1)))),
         dtype=np.int64)
     # Padding each vector to have a uniform length for saving
     pad_width = max(0, pad_size - len(tree) + 1)
     return np.pad(data_seq.reshape((5, -1)), ((0, 0), (0, pad_width)))
 
 
 def decode_service_tree(tdata: np.ndarray[np.int64]) -> nx.DiGraph:
-    """Inverse method of :func:`encode_service_tree`"""
+    """
+    Decode and rebuild service tree from value arrays.
+
+    Inverse method of :func:`encode_service_tree`.
+
+    :param tdata:   array values
+    :return:        service tree
+    """
     if tdata.shape[0] % 5:
         warnings.warn(f"Given data with shape {tdata.shape} is not a valid encoded tree!")
     root, *prufer_seq = np.trim_zeros(tdata[0, :], 'b')
     tree = nx.bfs_tree(nx.from_prufer_sequence(prufer_seq), source=root, sort_neighbors=sorted)
     for u, v in tree.edges:
         tree[u][v][DATA], tree[u][v][RATE], tree.nodes[v][RUNTIME], tree.nodes[v][MEMORY] = tdata[1:, v - 1]
     nx.relabel_nodes(tree, {0: PLATFORM}, copy=False)
     tree.graph[NAME] = "tree_" + "".join(map(str, tdata[0]))
     return tree
 
 
 def save_trees_to_file(trees: list[nx.DiGraph], file_name: str = "test_trees.npy", padding: int = 0):
-    """Convert trees into a compact formant and save them in a single file"""
+    """
+    Convert trees into a compact format and save them in a single file.
+
+    :param trees:       list of trees
+    :param file_name:   output file name
+    :param padding:     padding size
+    """
     enc_trees = list(encode_service_tree(t, pad_size=padding) for t in trees)
     if enc_trees:
         np.save(file_name, np.stack(enc_trees))
 
 
 def get_tree_from_file(file_name: str, tree_num: int) -> nx.DiGraph:
+    """
+    Load and decode a service tree from the given *file_name* with specific ID *tree_num*.
+
+    :param file_name:   file name
+    :param tree_num:    tree ID
+    :return:            loaded tree
+    """
     np_trees = np.load(file_name, mmap_mode="r", allow_pickle=False)
     return decode_service_tree(np_trees[tree_num - 1, :])
 
 
-def iload_trees_from_file(file_name: str) -> nx.DiGraph:
-    """Generator of service trees loaded from given file"""
+def iload_trees_from_file(file_name: str) -> Generator[nx.DiGraph]:
+    """
+    Generator of service trees loaded from given *file_name*.
+
+    :param file_name:   tree file
+    :return:            generator of trees
+    """
     np_trees = np.load(file_name, mmap_mode="r", allow_pickle=False)
     for idx in range(np_trees.shape[0]):
         yield decode_service_tree(np_trees[idx, :])
 
 
 def load_hist_params(hist_dir: str | pathlib.Path, hist_name: str) -> tuple[list[int | float], list[int | float]]:
-    """Load pickled attributes from given file"""
+    """
+    Load pickled attributes from given file.
+
+    :param hist_dir:    directory of histogram attributes
+    :param hist_name:   name of the histogram
+    :return:            loaded histogram attributes
+    """
     with open((pathlib.Path(hist_dir, hist_name).with_suffix('.pkl')).resolve(), 'rb') as f:
         return pickle.load(f, fix_imports=True)
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/microservice/__init__.py` & `SLAMBUC-0.2.0/slambuc/gen/microservice/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/microservice/faas_tree.py` & `SLAMBUC-0.2.0/slambuc/gen/microservice/faas_tree.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import itertools
 import pathlib
 import random
+from collections.abc import Generator
 
 import networkx as nx
 import numpy as np
 import scipy
 
 from slambuc.alg.service import *
 from slambuc.gen.io import load_hist_params, save_trees_to_file
@@ -52,43 +53,72 @@
 # Tree structure parameters of preferential attachment (Alpha) and attractiveness of leafs (a)
 PREF_ATT_LOW, PREF_ATT_HIGH = 0.05, 0.9
 LEAF_ATTR_LOW, LEAF_ATTR_HIGH = 0.1, 3.25
 
 DEF_FAAS_TREE_PREFIX = f"faas_tree"
 
 
-def ifunc_attributes(n: int, dist: scipy.stats.rv_continuous, transform=np.round) -> int:
-    """Generate attribute values of the given size *n* base on the given distribution *dist*"""
+def ifunc_attributes(n: int, dist: scipy.stats.rv_continuous, transform=np.round) -> Generator[int]:
+    """
+    Generate attribute values of the given size *n* base on the given distribution *dist*.
+
+    :param n:           number of attributes
+    :param dist:        build distribution object
+    :param transform:   transform function applied on every attribute value
+    :return:            generator of attributes
+    """
     yield from transform(dist.rvs(size=n)).astype(int)
 
 
 def get_faas_tree(n: int, Alpha: float, a: float) -> nx.DiGraph:
-    """Generate service tree with attributes drawn from the predefined distributions"""
+    """
+    Generate service tree with attributes drawn from the predefined distributions.
+
+    :param n:       number of nodes
+    :param Alpha:   power of preferential attachment (default: 1.0)
+    :param a:       attractiveness of vertices with no edges (default: 0.0)
+    :return:        generated tree
+    """
     tree = nx.bfs_tree(generate_power_ba_graph(n=n, m=1, Alpha=Alpha, a=a, root=1), source=1, sort_neighbors=sorted)
     runtimes, memories = ifunc_attributes(n, RT_DIST), ifunc_attributes(n, MEM_DIST)
     rates, data = ifunc_attributes(n, RATE_DIST, transform=np.floor), ifunc_attributes(n, DATA_DIST)
     tree.add_edge(PLATFORM, 1)
     for u, v in nx.dfs_edges(tree, source=PLATFORM):
         tree.nodes[v][RUNTIME], tree.nodes[v][MEMORY] = next(runtimes), next(memories)
         tree[u][v][RATE], tree[u][v][DATA] = next(rates), next(data)
     tree[PLATFORM][1][RATE] = 1
     tree.graph[NAME] = f"faas_tree_n{n}A{Alpha}a{a}"
     return tree
 
 
 def verify_faas_tree(n: int = 10):
-    """Plot random generated serverless tree"""
+    """
+    Plot random generated serverless tree.
+
+    :param n:   tree size
+    """
     t = get_faas_tree(n)
     draw_tree(t, draw_weights=True)
 
 
 def generate_all_faas_trees(data_dir: str, Alpha: float = PREF_ATT_HIGH, a: float = LEAF_ATTR_HIGH,
                             iteration: int = 100, start: int = 10, end: int = 100, step: int = 10,
                             tree_name: str = DEF_FAAS_TREE_PREFIX):
-    """Generate Serverless/Faas service trees with attributes from predefined and extracted distributions"""
+    """
+    Generate Serverless/Faas service trees with attributes from predefined and extracted distributions.
+
+    :param data_dir:    directory of saved trees
+    :param Alpha:       power of preferential attachment (default: 1.0)
+    :param a:           attractiveness of vertices with no edges (default: 0.0)
+    :param iteration:   number of generated trees
+    :param start:       minimum of size intervals
+    :param end:         maximum of size intervals
+    :param step:        step size of intervals
+    :param tree_name:   prefix name of tree files
+    """
     for min_size, max_size in itertools.pairwise(range(start, end + step, step)):
         print(f"Generating Serverless/FaaS trees with {min_size} <= size <= {max_size}...")
         trees = [get_faas_tree(n=random.randint(min_size, max_size), Alpha=Alpha, a=a)
                  for _ in range(iteration)]
         file_name = pathlib.Path(data_dir, f"{tree_name}_n{min_size}-{max_size}.npy").resolve()
         print(f"Saving trees into {file_name}...")
         save_trees_to_file(trees, file_name, padding=max_size)
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/microservice/hist/func_inv_rate_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl` & `SLAMBUC-0.2.0/slambuc/gen/microservice/hist/rw_overhead_hist.pkl`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/microservice/power_ba_graph.py` & `SLAMBUC-0.2.0/slambuc/gen/microservice/power_ba_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 import networkx as nx
 
 
 def wrand_sample(population: list[int | float], weights: list[int], k: int = 1) -> list[int | float]:
     """
     Provide an *k*-size weighted random sample from *population* without replacement according to the given *weights*.
+
     See more: https://stackoverflow.com/questions/43549515/weighted-random-sample-without-replacement-in-python
 
     :param population:  list of items
     :param weights:     list of item weights
     :param k:           sample size (default: 1)
     :return:            sample list
     """
@@ -42,17 +43,21 @@
     return list(population[idx] for idx in opted)
 
 
 def generate_power_ba_graph(n: int, m: int, Alpha: float = 1.0, a: float = 0.0, root: int = 0,
                             create_using: nx.Graph = None) -> nx.Graph:
     """
     Generate Barabasi-Albert (BA) graph where the probability of choosing a vertex *v* for connecting to another node
-    follows a Power law distribution as *P(v) = deg(v)^Alpha + a*. Thus, choosing *Alpha = 1.0* and *a = 0.0* falls
-    back to standard BA graph generation. Choosing *m = 1* ensures the output to be a tree by default. See also:
-    https://networkx.org/documentation/stable/_modules/networkx/generators/random_graphs.html#barabasi_albert_graph
+    follows a Power law distribution as *P(v) = deg(v)^Alpha + a*.
+
+    Thus, choosing *Alpha = 1.0* and *a = 0.0* falls back to standard BA graph generation.
+
+    Choosing *m = 1* ensures the output to be a tree by default.
+
+    See also: https://networkx.org/documentation/stable/_modules/networkx/generators/random_graphs.html#barabasi_albert_graph
     and the related paper: https://dl.acm.org/doi/abs/10.5555/3432601.3432616.
 
     :param n:               number of nodes
     :param m:               number of existing nodes (or new edges) attached to the new node in each step
     :param Alpha:           power of preferential attachment (default: 1.0)
     :param a:               attractiveness of vertices with no edges (default: 0.0)
     :param root:            initial node ID that is increased in each attachment step (default: 0)
@@ -63,8 +68,8 @@
     node_max, node_miss = max(graph), n - len(graph)
     for source in range(node_max + 1, node_max + node_miss + 1):
         nodes, deg_weights = zip(*((v, d ** Alpha + a) for v, d in graph.degree))
         graph.add_edges_from(zip(itertools.repeat(source), wrand_sample(nodes, deg_weights, m)))
     return graph
 
 
-generate_power_ba_tree = functools.partial(generate_power_ba_graph, m=1)
+generate_power_ba_tree = functools.partial(generate_power_ba_graph, m=1)  # Generate power BA trees using m=1.
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/random/__init__.py` & `SLAMBUC-0.2.0/slambuc/gen/random/__init__.py`

 * *Files identical despite different names*

### Comparing `SLAMBUC-0.1.0/slambuc/gen/random/random_tree.py` & `SLAMBUC-0.2.0/slambuc/gen/random/random_tree.py`

 * *Files 18% similar despite different names*

```diff
@@ -24,24 +24,41 @@
 DATA = (10, 100)  # Read/write overhead in ms
 RATE = (1, 10)  # Invocations rate in 1/s
 
 DEF_RAND_TREE_PREFIX = "random_tree"
 
 
 def generate_random_trees(n: int, data_dir: str, iteration: int = 1000, file_prefix: str = DEF_RAND_TREE_PREFIX):
+    """
+    Generate random trees with attributes uniformly drawn form intervals.
+
+    :param n:           tree size
+    :param data_dir:    directory of saved trees
+    :param iteration:   number of generated trees
+    :param file_prefix: prefix name of tree files
+    """
     print(f"Generating random trees with size {n}...")
     trees = [get_random_tree(nodes=n, runtime=RUNTIME, memory=MEMORY, rate=RATE, data=DATA) for _ in range(iteration)]
     file_name = pathlib.Path(data_dir, f"{file_prefix}_n{n}.npy").resolve()
     print(f"Saving trees into {file_name}...")
     save_trees_to_file(trees, file_name)
 
 
 def generate_all_random_trees(data_dir: str, iteration: int = 100, start: int = 10, end: int = 100, step: int = 10,
                               file_prefix: str = DEF_RAND_TREE_PREFIX):
-    """Generate random service trees with attributes from uniform distribution"""
+    """
+    Generate random service trees with random sizes from given intervals.
+
+    :param data_dir:    directory of saved trees
+    :param iteration:   number of generated trees
+    :param start:       minimum of size intervals
+    :param end:         maximum of size intervals
+    :param step:        step size of intervals
+    :param file_prefix: prefix name of tree files
+    """
     for min_size, max_size in itertools.pairwise(range(start, end + step, step)):
         print(f"Generating random trees with {min_size} <= size <= {max_size}...")
         trees = [get_random_tree(nodes=random.randint(min_size, max_size), runtime=RUNTIME, memory=MEMORY,
                                  rate=RATE, data=DATA, name=DEF_RAND_TREE_PREFIX + f"_{i}") for i in range(iteration)]
         file_name = pathlib.Path(data_dir, f"{file_prefix}_n{min_size}-{max_size}.npy").resolve()
         print(f"Saving trees into {file_name}...")
         save_trees_to_file(trees, file_name, padding=max_size)
```

### Comparing `SLAMBUC-0.1.0/slambuc/gen/transform.py` & `SLAMBUC-0.2.0/slambuc/gen/transform.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,17 +16,24 @@
 import networkx as nx
 
 from slambuc.alg.service import PLATFORM, RUNTIME, DATA
 from slambuc.alg.util import ipostorder_dfs
 
 
 def faasify_dag_by_duplication(dag: nx.DiGraph, root: int) -> nx.DiGraph:
-    """One-way transformation of a DAG of modules/components into a tree by iteratively duplicating sub-graphs
+    """
+    One-way transformation of a DAG of modules/components into a tree by iteratively duplicating sub-graphs
     related to nodes with multiple predecessors.
-    The algorithm requires that the input DAG must have only one source node."""
+
+    The algorithm requires that the input DAG must have only one source node.
+
+    :param dag:     input DAG
+    :param root:    root node
+    :return:        generated tree
+    """
     if dag is None:
         return
     while not nx.is_tree(dag):
         new_id = itertools.count(max(filter(lambda _v: _v is not PLATFORM, dag.nodes)) + 1)
         for v in list(dag.nodes):
             if len(dag.pred[v]) > 1:
                 while len(ingress := list(dag.pred[v])) > 1:
@@ -51,13 +58,20 @@
 
 def faasify_dag_by_cutting(dag: nx.DiGraph, root: int) -> nx.DiGraph:
     ...
     # TODO
 
 
 def transform_autonomous_caching(tree: nx.DiGraph, root: int, copy: bool = False) -> nx.DiGraph:
-    """Transform given **tree** by adding fetching and out-caching overheads to function execution times"""
+    """
+    Transform given *tree* by adding fetching and out-caching overheads to function execution times.
+
+    :param tree:    input tree
+    :param root:    root node
+    :param copy:    use a deep copy of the input instead of modifying the original
+    :return:        transformed tree
+    """
     tf_tree = tree.copy() if copy else tree
     for p, n in ipostorder_dfs(tree, root):
         # Add data fetching and state caching overheads to the function execution time
         tf_tree.nodes[n][RUNTIME] += tree[p][n][DATA] + sum(tree[n][s][DATA] for s in tree.successors(n))
     return tf_tree
```

### Comparing `SLAMBUC-0.1.0/slambuc/misc/plot.py` & `SLAMBUC-0.2.0/slambuc/misc/plot.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,25 @@
 from slambuc.alg.util import path_blocks
 
 PART_COLORS = ('red', 'orange', "brown", 'green', "purple", "blue", "black", "magenta")
 
 
 def draw_tree(tree: nx.DiGraph, partition: list = None, cuts: list = None, draw_weights=False, draw_blocks=False,
               figsize=None, ax=None, **kwargs):
-    """Draw tree and given partitioning in a top-down topological structure"""
+    """
+    Draw tree with given partitioning in a top-down topological structure.
+
+    :param tree:            service tree
+    :param partition:       calculated partitioning (optional)
+    :param cuts:            calculated cuts (optional)
+    :param draw_weights:    draw node/edge weights instead of IDs
+    :param draw_blocks:     draw surrounding blocks
+    :param figsize:         figure dimensions (optional)
+    :param ax:              matplotlib axis (optional)
+    """
     if figsize is None:
         d = nx.dag_longest_path_length(tree)
         figsize = (d, d)
     if ax is None:
         plt.figure(figsize=figsize, dpi=300)
         ax = plt.gca()
     colors = itertools.cycle(PART_COLORS)
@@ -103,15 +113,21 @@
     plt.title(tree.graph[NAME])
     plt.tight_layout()
     plt.show()
     plt.close()
 
 
 def draw_state_dag(dag: nx.DiGraph, chains: list[list[int]], draw_weights: bool = False):
-    """Draw state-space DAG in a vertically-ordered multipartite layout"""
+    """
+    Draw state-space DAG in a vertically-ordered multipartite layout.
+
+    :param dag:             input DAG
+    :param chains:          chain decomposition of the given tree
+    :param draw_weights:    draw node/edge weights instead of IDs
+    """
     h = max(len(c) for c in chains) * 1.5
     plt.figure(figsize=(2 * h, h), dpi=300)
     layers = [START, *itertools.chain.from_iterable(chains), END]
     for v in dag.nodes:
         dag.nodes[v]['layer'] = layers.index(decode_state(v)[0][0] if v not in (START, END) else v)
     node_color = ["tab:green" if n is START else "tab:red" if n is END else "tab:blue" for n in dag.nodes]
     pos = nx.multipartite_layout(dag, subset_key='layer', scale=1)
```

