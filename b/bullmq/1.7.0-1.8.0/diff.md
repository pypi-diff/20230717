# Comparing `tmp/bullmq-1.7.0.tar.gz` & `tmp/bullmq-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-1.7.0.tar", last modified: Fri Jul 14 17:30:11 2023, max compression
+gzip compressed data, was "bullmq-1.8.0.tar", last modified: Mon Jul 17 20:35:26 2023, max compression
```

## Comparing `bullmq-1.7.0.tar` & `bullmq-1.8.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 17:30:11.935833 bullmq-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-14 17:28:40.000000 bullmq-1.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.931832 bullmq-1.7.0/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-14 17:30:08.000000 bullmq-1.7.0/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8794 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/addJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/changePriority-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getState-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/getStateV2-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToActive-10.lua
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToFinished-13.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/pause-5.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/promote-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/retryJob-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-14 17:29:34.000000 bullmq-1.7.0/bullmq/commands/updateProgress-2.lua
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/custom_errors/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/custom_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/custom_errors/waiting_children_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19430 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.935833 bullmq-1.7.0/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-07-14 17:28:40.000000 bullmq-1.7.0/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 17:30:11.931832 bullmq-1.7.0/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 17:30:11.000000 bullmq-1.7.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-14 17:30:08.000000 bullmq-1.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 17:30:11.935833 bullmq-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-14 17:28:40.000000 bullmq-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 20:35:26.152906 bullmq-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-17 20:34:17.000000 bullmq-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.148906 bullmq-1.8.0/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-17 20:35:23.000000 bullmq-1.8.0/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/addJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/changePriority-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getState-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/getStateV2-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToActive-10.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    24195 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToFinished-13.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/pause-5.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/promote-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/retryJob-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-07-17 20:34:59.000000 bullmq-1.8.0/bullmq/commands/updateProgress-2.lua
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/custom_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/custom_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/custom_errors/waiting_children_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8266 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19424 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.152906 bullmq-1.8.0/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-17 20:34:17.000000 bullmq-1.8.0/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:35:26.148906 bullmq-1.8.0/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 20:35:26.000000 bullmq-1.8.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-07-17 20:35:23.000000 bullmq-1.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:35:26.152906 bullmq-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 20:34:17.000000 bullmq-1.8.0/setup.py
```

### Comparing `bullmq-1.7.0/PKG-INFO` & `bullmq-1.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.7.0
+Version: 1.8.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.7.0/README.md` & `bullmq-1.8.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/backoffs.py` & `bullmq-1.8.0/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/addJob-9.lua` & `bullmq-1.8.0/bullmq/commands/addJob-9.lua`

 * *Files 3% similar despite different names*

```diff
@@ -119,20 +119,21 @@
     rcall("XTRIM", eventStreamKey, "MAXLEN", "~", 10000)
   end
 end
 --[[
   Validate and move or add dependencies to parent.
 ]]
 -- Includes
-local function updateParentDepsIfNeeded(parentKey, parentQueueKey, parentDependenciesKey,
-  parentId, jobIdKey, returnvalue, timestamp )
-  local processedSet = parentKey .. ":processed"
-  rcall("HSET", processedSet, jobIdKey, returnvalue)
-  local activeParent = rcall("ZSCORE", parentQueueKey .. ":waiting-children", parentId)
-  if rcall("SCARD", parentDependenciesKey) == 0 and activeParent then 
+--[[
+  Validate and move parent to active if needed.
+]]
+-- Includes
+local function moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey, parentKey, parentId, timestamp)
+  local isParentActive = rcall("ZSCORE", parentQueueKey .. ":waiting-children", parentId)
+  if rcall("SCARD", parentDependenciesKey) == 0 and isParentActive then 
     rcall("ZREM", parentQueueKey .. ":waiting-children", parentId)
     local parentWaitKey = parentQueueKey .. ":wait"
     local parentTarget, paused = getTargetQueueList(parentQueueKey .. ":meta", parentWaitKey,
       parentQueueKey .. ":paused")
     local jobAttributes = rcall("HMGET", parentKey, "priority", "delay")
     local priority = tonumber(jobAttributes[1]) or 0
     local delay = tonumber(jobAttributes[2]) or 0
@@ -147,18 +148,25 @@
     else
       if priority == 0 then
         rcall("RPUSH", parentTarget, parentId)
       else
         addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
           parentId, parentQueueKey .. ":pc")
       end
-      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId,
+        "prev", "waiting-children")
     end
   end
 end
+local function updateParentDepsIfNeeded(parentKey, parentQueueKey, parentDependenciesKey,
+  parentId, jobIdKey, returnvalue, timestamp )
+  local processedSet = parentKey .. ":processed"
+  rcall("HSET", processedSet, jobIdKey, returnvalue)
+  moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey, parentKey, parentId, timestamp)
+end
 if parentKey ~= nil then
   if rcall("EXISTS", parentKey) ~= 1 then
     return -5
   end
   parentData = cjson.encode(parent)
 end
 local jobCounter = rcall("INCR", KEYS[4])
```

### Comparing `bullmq-1.7.0/bullmq/commands/changeDelay-3.lua` & `bullmq-1.8.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/changePriority-5.lua` & `bullmq-1.8.0/bullmq/commands/changePriority-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-1.8.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/drain-4.lua` & `bullmq-1.8.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/getCounts-1.lua` & `bullmq-1.8.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/getRanges-1.lua` & `bullmq-1.8.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/getState-8.lua` & `bullmq-1.8.0/bullmq/commands/getState-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/getStateV2-8.lua` & `bullmq-1.8.0/bullmq/commands/getStateV2-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/isFinished-3.lua` & `bullmq-1.8.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-1.8.0/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-1.8.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/moveToActive-10.lua` & `bullmq-1.8.0/bullmq/commands/moveToActive-10.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-1.8.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/moveToFinished-13.lua` & `bullmq-1.8.0/bullmq/commands/moveToFinished-13.lua`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
       opts - token - lock token
       opts - keepJobs
       opts - lockDuration - lock duration in milliseconds
       opts - attempts max attempts
       opts - attemptsMade
       opts - maxMetricsSize
       opts - fpof - fail parent on fail
+      opts - rdof - remove dependency on fail
     Output:
       0 OK
       -1 Missing key.
       -2 Missing lock.
       -3 Job not in active set
       -4 Job has pending dependencies
       -6 Lock is not owned by this client
@@ -188,14 +189,95 @@
   rcall("HSET", jobKey, "processedOn", processedOn)
   rcall("HINCRBY", jobKey, "attemptsMade", 1)
   return {rcall("HGETALL", jobKey), jobId, 0, 0} -- get job data
 end
 --[[
   Function to recursively move from waitingChildren to failed.
 ]]
+-- Includes
+--[[
+  Validate and move parent to active if needed.
+]]
+-- Includes
+--[[
+  Add delay marker if needed.
+]]
+-- Includes
+local function addDelayMarkerIfNeeded(targetKey, delayedKey)
+  if rcall("LLEN", targetKey) == 0 then
+    local nextTimestamp = getNextDelayedTimestamp(delayedKey)
+    if nextTimestamp ~= nil then
+      rcall("LPUSH", targetKey, "0:" .. nextTimestamp)
+    end
+  end
+end
+--[[
+  Function to add job considering priority.
+]]
+-- Includes
+--[[
+  Function priority marker to wait if needed
+  in order to wake up our workers and to respect priority
+  order as much as possible
+]]
+local function addPriorityMarkerIfNeeded(waitKey)
+  local waitLen = rcall("LLEN", waitKey)
+  if waitLen == 0 then
+    rcall("LPUSH", waitKey, "0:0")
+  end
+end
+local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
+  local prioCounter = rcall("INCR", priorityCounterKey)
+  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
+  rcall("ZADD", prioritizedKey, score, jobId)
+  if not paused then
+    addPriorityMarkerIfNeeded(waitKey)
+  end
+end
+--[[
+  Function to check for the meta.paused key to decide if we are paused or not
+  (since an empty list and !EXISTS are not really the same).
+]]
+local function getTargetQueueList(queueMetaKey, waitKey, pausedKey)
+  if rcall("HEXISTS", queueMetaKey, "paused") ~= 1 then
+    return waitKey, false
+  else
+    return pausedKey, true
+  end
+end
+local function moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey, parentKey, parentId, timestamp)
+  local isParentActive = rcall("ZSCORE", parentQueueKey .. ":waiting-children", parentId)
+  if rcall("SCARD", parentDependenciesKey) == 0 and isParentActive then 
+    rcall("ZREM", parentQueueKey .. ":waiting-children", parentId)
+    local parentWaitKey = parentQueueKey .. ":wait"
+    local parentTarget, paused = getTargetQueueList(parentQueueKey .. ":meta", parentWaitKey,
+      parentQueueKey .. ":paused")
+    local jobAttributes = rcall("HMGET", parentKey, "priority", "delay")
+    local priority = tonumber(jobAttributes[1]) or 0
+    local delay = tonumber(jobAttributes[2]) or 0
+    if delay > 0 then
+      local delayedTimestamp = tonumber(timestamp) + delay 
+      local score = delayedTimestamp * 0x1000
+      local parentDelayedKey = parentQueueKey .. ":delayed" 
+      rcall("ZADD", parentDelayedKey, score, parentId)
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "delayed", "jobId", parentId,
+        "delay", delayedTimestamp)
+      addDelayMarkerIfNeeded(parentTarget, parentDelayedKey)
+    else
+      if priority == 0 then
+        rcall("RPUSH", parentTarget, parentId)
+      else
+        addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
+          parentId, parentQueueKey .. ":pc")
+      end
+      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId,
+        "prev", "waiting-children")
+    end
+  end
+end
 local function moveParentFromWaitingChildrenToFailed( parentQueueKey, parentKey, parentId, jobIdKey, timestamp)
   if rcall("ZREM", parentQueueKey .. ":waiting-children", parentId) == 1 then
     rcall("ZADD", parentQueueKey .. ":failed", timestamp, parentId)
     local failedReason = "child " .. jobIdKey .. " failed"
     rcall("HMSET", parentKey, "failedReason", failedReason, "finishedOn", timestamp)
     rcall("XADD", parentQueueKey .. ":events", "*", "event", "failed", "jobId", parentId, "failedReason",
       failedReason, "prev", "waiting-children")
@@ -206,48 +288,32 @@
         moveParentFromWaitingChildrenToFailed(
           parentData['queueKey'],
           parentData['queueKey'] .. ':' .. parentData['id'],
           parentData['id'],
           parentKey,
           timestamp
         )
+      elseif parentData['rdof'] then
+        local grandParentKey = parentData['queueKey'] .. ':' .. parentData['id']
+        local grandParentDependenciesSet = grandParentKey .. ":dependencies"
+        if rcall("SREM", grandParentDependenciesSet, parentKey) == 1 then
+          moveParentToWaitIfNeeded(parentData['queueKey'], grandParentDependenciesSet,
+            grandParentKey, parentData['id'], timestamp)
+        end
       end
     end
   end
 end
 --[[
   Updates the delay set, by moving delayed jobs that should
   be processed now to "wait".
      Events:
       'waiting'
 ]]
 -- Includes
---[[
-  Function to add job considering priority.
-]]
--- Includes
---[[
-  Function priority marker to wait if needed
-  in order to wake up our workers and to respect priority
-  order as much as possible
-]]
-local function addPriorityMarkerIfNeeded(waitKey)
-  local waitLen = rcall("LLEN", waitKey)
-  if waitLen == 0 then
-    rcall("LPUSH", waitKey, "0:0")
-  end
-end
-local function addJobWithPriority(waitKey, prioritizedKey, priority, paused, jobId, priorityCounterKey)
-  local prioCounter = rcall("INCR", priorityCounterKey)
-  local score = priority * 0x100000000 + bit.band(prioCounter, 0xffffffffffff)
-  rcall("ZADD", prioritizedKey, score, jobId)
-  if not paused then
-    addPriorityMarkerIfNeeded(waitKey)
-  end
-end
 -- Try to get as much as 1000 jobs at once
 local function promoteDelayedJobs(delayedKey, waitKey, targetKey, prioritizedKey,
                                   eventStreamKey, prefix, timestamp, paused, priorityCounterKey)
     local jobs = rcall("ZRANGEBYSCORE", delayedKey, 0, (timestamp + 1) * 0x1000, "LIMIT", 0, 1000)
     if (#jobs > 0) then
         rcall("ZREM", delayedKey, unpack(jobs))
         for _, jobId in ipairs(jobs) do
@@ -287,25 +353,14 @@
 ]]
 local getJobIdFromKey = function (jobKey)
   return string.match(jobKey, ".*:(.*)")
 end
 local getJobKeyPrefix = function (jobKey, jobId)
   return string.sub(jobKey, 0, #jobKey - #jobId)
 end
---[[
-  Function to check for the meta.paused key to decide if we are paused or not
-  (since an empty list and !EXISTS are not really the same).
-]]
-local function getTargetQueueList(queueMetaKey, waitKey, pausedKey)
-  if rcall("HEXISTS", queueMetaKey, "paused") ~= 1 then
-    return waitKey, false
-  else
-    return pausedKey, true
-  end
-end
 local function moveParentToWait(parentPrefix, parentId, emitEvent)
   local parentTarget = getTargetQueueList(parentPrefix .. "meta", parentPrefix .. "wait", parentPrefix .. "paused")
   rcall("RPUSH", parentTarget, parentId)
   if emitEvent then
     local parentEventStream = parentPrefix .. "events"
     rcall("XADD", parentEventStream, "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
   end
@@ -401,57 +456,19 @@
     rcall("XTRIM", eventStreamKey, "MAXLEN", "~", 10000)
   end
 end
 --[[
   Validate and move or add dependencies to parent.
 ]]
 -- Includes
---[[
-  Add delay marker if needed.
-]]
--- Includes
-local function addDelayMarkerIfNeeded(targetKey, delayedKey)
-  if rcall("LLEN", targetKey) == 0 then
-    local nextTimestamp = getNextDelayedTimestamp(delayedKey)
-    if nextTimestamp ~= nil then
-      rcall("LPUSH", targetKey, "0:" .. nextTimestamp)
-    end
-  end
-end
 local function updateParentDepsIfNeeded(parentKey, parentQueueKey, parentDependenciesKey,
   parentId, jobIdKey, returnvalue, timestamp )
   local processedSet = parentKey .. ":processed"
   rcall("HSET", processedSet, jobIdKey, returnvalue)
-  local activeParent = rcall("ZSCORE", parentQueueKey .. ":waiting-children", parentId)
-  if rcall("SCARD", parentDependenciesKey) == 0 and activeParent then 
-    rcall("ZREM", parentQueueKey .. ":waiting-children", parentId)
-    local parentWaitKey = parentQueueKey .. ":wait"
-    local parentTarget, paused = getTargetQueueList(parentQueueKey .. ":meta", parentWaitKey,
-      parentQueueKey .. ":paused")
-    local jobAttributes = rcall("HMGET", parentKey, "priority", "delay")
-    local priority = tonumber(jobAttributes[1]) or 0
-    local delay = tonumber(jobAttributes[2]) or 0
-    if delay > 0 then
-      local delayedTimestamp = tonumber(timestamp) + delay 
-      local score = delayedTimestamp * 0x1000
-      local parentDelayedKey = parentQueueKey .. ":delayed" 
-      rcall("ZADD", parentDelayedKey, score, parentId)
-      rcall("XADD", parentQueueKey .. ":events", "*", "event", "delayed", "jobId", parentId,
-        "delay", delayedTimestamp)
-      addDelayMarkerIfNeeded(parentTarget, parentDelayedKey)
-    else
-      if priority == 0 then
-        rcall("RPUSH", parentTarget, parentId)
-      else
-        addJobWithPriority(parentWaitKey, parentQueueKey .. ":prioritized", priority, paused,
-          parentId, parentQueueKey .. ":pc")
-      end
-      rcall("XADD", parentQueueKey .. ":events", "*", "event", "waiting", "jobId", parentId, "prev", "waiting-children")
-    end
-  end
+  moveParentToWaitIfNeeded(parentQueueKey, parentDependenciesKey, parentKey, parentId, timestamp)
 end
 local function getRateLimitTTL(maxJobs, rateLimiterKey)
   if maxJobs then
     local pttl = rcall("PTTL", rateLimiterKey)
     if pttl == 0 then
       rcall("DEL", rateLimiterKey)
     end
@@ -521,17 +538,25 @@
         if ARGV[5] == "completed" then
             local dependenciesSet = parentKey .. ":dependencies"
             if rcall("SREM", dependenciesSet, jobIdKey) == 1 then
                 updateParentDepsIfNeeded(parentKey, parentQueueKey,
                                          dependenciesSet, parentId, jobIdKey,
                                          ARGV[4], timestamp)
             end
-        elseif opts['fpof'] then
-            moveParentFromWaitingChildrenToFailed(parentQueueKey, parentKey,
-                                                  parentId, jobIdKey, timestamp)
+        else
+            if opts['fpof'] then
+                moveParentFromWaitingChildrenToFailed(parentQueueKey, parentKey,
+                                            parentId, jobIdKey, timestamp)
+            elseif opts['rdof'] then
+                local dependenciesSet = parentKey .. ":dependencies"
+                if rcall("SREM", dependenciesSet, jobIdKey) == 1 then
+                    moveParentToWaitIfNeeded(parentQueueKey, dependenciesSet,
+                        parentKey, parentId, timestamp)
+                end 
+            end
         end
     end
     -- Remove job?
     if maxCount ~= 0 then
         local targetSet = KEYS[11]
         -- Add to complete/failed set
         rcall("ZADD", targetSet, timestamp, jobId)
```

### Comparing `bullmq-1.7.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-1.8.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/obliterate-2.lua` & `bullmq-1.8.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/pause-5.lua` & `bullmq-1.8.0/bullmq/commands/pause-5.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/promote-7.lua` & `bullmq-1.8.0/bullmq/commands/promote-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/removeJob-1.lua` & `bullmq-1.8.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-1.8.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/reprocessJob-6.lua` & `bullmq-1.8.0/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/retryJob-9.lua` & `bullmq-1.8.0/bullmq/commands/retryJob-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/commands/retryJobs-6.lua` & `bullmq-1.8.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/event_emitter.py` & `bullmq-1.8.0/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/job.py` & `bullmq-1.8.0/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/queue.py` & `bullmq-1.8.0/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/redis_connection.py` & `bullmq-1.8.0/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/scripts.py` & `bullmq-1.8.0/bullmq/scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -282,15 +282,15 @@
     async def reprocessJob(self, job: Job, state: str):
         keys = [self.toKey(job.id)]
         keys.append(self.keys['events'])
         keys.append(self.keys[state])
         keys.append(self.keys['wait'])
         keys.append(self.keys['meta'])
         keys.append(self.keys['paused'])
-        
+
         args = [
             job.id,
             ("R" if job.opts.get("lifo") else "L") + "PUSH",
             "failedReason" if state == "failed" else "returnvalue",
             state
             ]
 
@@ -329,15 +329,15 @@
         """
         current_state = state or 'failed'
         keys = self.getKeys(
             ['', 'events', current_state, 'wait', 'paused', 'meta'])
         result = await self.commands["retryJobs"](keys=keys, args=[count or 1000, timestamp or round(time.time()*1000), current_state])
         return result
 
-    async def moveToActive(self, token: str, opts: dict, jobId: str = "") -> list[Any]:
+    async def moveToActive(self, token: str, opts: dict, jobId: str = None) -> list[Any]:
         """
         Add an item to the queue
         """
         timestamp = round(time.time() * 1000)
         lockDuration = opts.get("lockDuration", 0)
         limiter = opts.get("limiter", None)
```

### Comparing `bullmq-1.7.0/bullmq/timer.py` & `bullmq-1.8.0/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/types/job_options.py` & `bullmq-1.8.0/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/types/worker_options.py` & `bullmq-1.8.0/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/utils.py` & `bullmq-1.8.0/bullmq/utils.py`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/bullmq/worker.py` & `bullmq-1.8.0/bullmq/worker.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,18 @@
         self.closing = False
         self.forceClosing = False
         self.closed = False
         self.running = False
         self.processing = set()
         self.jobs = set()
         self.id = uuid4().hex
+        self.waiting = None
+        self.blockUntil = 0
+        self.limitUntil = 0
+        self.drained = False
 
         if opts.get("autorun", True):
             asyncio.ensure_future(self.run())
 
     async def run(self):
         if self.running:
             raise Exception("Worker is already running")
@@ -55,29 +59,27 @@
             "stalledInterval") / 1000, self.runStalledJobsCheck)
         self.running = True
         jobs = []
 
         token_postfix = 0
 
         while not self.closed:
-            if len(jobs) == 0 and len(self.processing) < self.opts.get("concurrency") and not self.closing:
+            while not self.waiting and len(self.processing) < self.opts.get("concurrency") and not self.closing:
                 token_postfix+=1
                 token = f'{self.id}:{token_postfix}'
                 waiting_job = asyncio.ensure_future(self.getNextJob(token))
                 self.processing.add(waiting_job)
 
-            if len(jobs) > 0:
-                jobs_to_process = [self.processJob(job, job.token) for job in jobs]
-                processing_jobs = [asyncio.ensure_future(
-                    j) for j in jobs_to_process]
-                self.processing.update(processing_jobs)
-
             try:
                 jobs, pending = await getCompleted(self.processing)
 
+                jobs_to_process = [self.processJob(job, job.token) for job in jobs]
+                processing_jobs = [asyncio.ensure_future(
+                    j) for j in jobs_to_process]
+                pending.update(processing_jobs)
                 self.processing = pending
 
                 if (len(jobs) == 0 or len(self.processing) == 0) and self.closing:
                     # We are done processing so we can close the queue
                     break
 
             except Exception as e:
@@ -92,42 +94,73 @@
 
     async def getNextJob(self, token: str):
         """
         Returns a promise that resolves to the next job in queue.
         @param token: worker token to be assigned to retrieved job
         @returns a Job or undefined if no job was available in the queue.
         """
-        # First try to move a job from the waiting list to the active list
-        result = await self.scripts.moveToActive(token, self.opts)
-        job = None
-        job_id = None
+
+        if not self.waiting:
+            self.waiting = self.waitForJob()
+
+            try:
+                job_id = await self.waiting
+                job_instance = await self.moveToActive(token, job_id)
+                return job_instance
+            finally:
+                self.waiting = None
+        else:
+            job_instance = await self.moveToActive(token)
+            return job_instance
+
+    async def moveToActive(self, token: str, job_id: str = None):
+        if job_id and job_id.startswith('0:'):
+            self.blockUntil = int(job_id.split(':')[1]) or 0
+
+        result = await self.scripts.moveToActive(token, self.opts, job_id)
+        job_data = None
+        id = None
         limit_until = None
         delay_until = None
 
         if result:
-            job, job_id, limit_until, delay_until = result
+            job_data, id, limit_until, delay_until = result
+
+        return self.nextJobFromJobData(job_data, id, limit_until, delay_until, token)
+
+    def nextJobFromJobData(self, job_data = None, job_id: str = None, limit_until: int = 0,
+        delay_until: int = 0, token: str = None):
+        self.limitUntil = max(limit_until, 0) or 0
 
-        # If there are no jobs in the waiting list we keep waiting with BRPOPLPUSH
-        if job is None:
-            timeout = min(delay_until - int(time.time() * 1000)
-                          if delay_until else 5000, 5000) / 1000
-            
-            redis_version = await self.blockingRedisConnection.getRedisVersion()
-            # Only Redis v6.0.0 and above supports doubles as block time
-            timeout = int(math.ceil(timeout)) if isRedisVersionLowerThan(redis_version, '6.0.0') else timeout
-
-            job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
-            if job_id:
-                job, job_id, limit_until, delay_until = await self.scripts.moveToActive(token, self.opts, job_id)
+        if not job_data:
+            if not self.drained:
+                self.drained = True
+                self.blockUntil = 0
 
-        if job and job_id:
-            job_instance = Job.fromJSON(self, job, job_id)
+        if delay_until:
+            self.blockUntil = max(delay_until, 0) or 0
+
+        if job_data:
+            self.drained = False
+            job_instance = Job.fromJSON(self, job_data, job_id)
             job_instance.token = token
             return job_instance
 
+    async def waitForJob(self):
+        timeout = max(min(self.blockUntil - int(time.time() * 1000)
+                        if self.blockUntil else 5000, 5000) / 1000, 0.00001)
+
+        redis_version = await self.blockingRedisConnection.getRedisVersion()
+        # Only Redis v6.0.0 and above supports doubles as block time
+        timeout = int(math.ceil(timeout)) if isRedisVersionLowerThan(redis_version, '6.0.0') else timeout
+
+        job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
+
+        return job_id
+
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
                 await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", False), token, self.opts, fetchNext=not self.closing)
                 job.returnvalue = result
@@ -177,30 +210,29 @@
             print("Error checking stalled jobs", e)
             self.emit('error', e)
 
     async def close(self, force: bool = False):
         """
         Close the worker
         """
+        self.closing = True
         if force:
             self.forceClosing = True
             self.cancelProcessing()
 
-        self.closing = True
-
         await self.blockingRedisConnection.close()
         await self.redisConnection.close()
 
     def cancelProcessing(self):
         for job in self.processing:
             if not job.done():
                 job.cancel()
 
 
-async def getCompleted(task_set: set) -> tuple[list[Job], list]:
+async def getCompleted(task_set: set) -> tuple[list[Job], set]:
     job_set, pending = await asyncio.wait(task_set, return_when=asyncio.FIRST_COMPLETED)
     jobs = [extract_result(job_task) for job_task in job_set]
     # we filter `None` out to remove:
     # a) an empty 'completed jobs' list; and
     # b) a failed extract_result
     jobs = list(filter(lambda j: j is not None, jobs))
     return jobs, pending
```

### Comparing `bullmq-1.7.0/bullmq.egg-info/PKG-INFO` & `bullmq-1.8.0/bullmq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 1.7.0
+Version: 1.8.0
 Summary: BullMQ for Python
 Author-email: "Taskforce.sh Inc." <manast@taskforce.sh>
 Project-URL: Homepage, https://bullmq.io
 Project-URL: Bug Tracker, https://github.com/taskforcesh/bullmq/issues
 Keywords: python,bullmq,queues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-1.7.0/bullmq.egg-info/SOURCES.txt` & `bullmq-1.8.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-1.7.0/pyproject.toml` & `bullmq-1.8.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bullmq"
-version = "1.7.0"
+version = "1.8.0"
 description='BullMQ for Python'
 readme="README.md"
 authors = [
     {name = "Taskforce.sh Inc.", email = "manast@taskforce.sh"},
 ]
 requires-python = ">=3.10.0"
 classifiers=[
@@ -23,15 +23,15 @@
     "redis >= 4.5.0, < 5",
     "msgpack >= 1.0.0, < 2",
     "semver >= 2.13.0, < 3"
 ]
 
 [project.optional-dependencies]
 dev = [
-    "setuptools==63.4.3",
+    "setuptools==68.0.0",
     "pre-commit==3.3.3",
     "build==0.8.0",
     "python-semantic-release==7.28.1",
     "types-redis==4.6.0.2"
 ]
 
 [project.urls]
```

