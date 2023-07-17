# Comparing `tmp/spai-2023.7.17.post2.tar.gz` & `tmp/spai-2023.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spai-2023.7.17.post2.tar", max compression
+gzip compressed data, was "spai-2023.7.4.tar", max compression
```

## Comparing `spai-2023.7.17.post2.tar` & `spai-2023.7.4.tar`

### file list

```diff
@@ -1,73 +1,64 @@
--rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.7.17.post2/README.md
--rw-r--r--   0        0        0      508 2023-07-17 09:43:09.343154 spai-2023.7.17.post2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.7.17.post2/spai/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.7.17.post2/spai/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.7.17.post2/spai/cli/commands/__init__.py
--rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.7.17.post2/spai/cli/commands/auth.py
--rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.7.17.post2/spai/cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.7.17.post2/spai/cli/src/errors/auth.py
--rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.7.17.post2/spai/cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.7.17.post2/spai/cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.7.17.post2/spai/cli/src/repos/__init__.py
--rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.7.17.post2/spai/cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      364 2023-07-17 09:42:53.879109 spai-2023.7.17.post2/spai/cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.7.17.post2/spai/cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.7.17.post2/spai/cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.7.17.post2/spai/cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.7.17.post2/spai/cli/src/usecases/project/GetLogs.py
--rw-r--r--   0        0        0      669 2023-07-04 12:57:35.512652 spai-2023.7.17.post2/spai/cli/src/usecases/project/GetServices.py
--rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.7.17.post2/spai/cli/src/usecases/project/RunService.py
--rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.7.17.post2/spai/cli/src/usecases/project/ScheduleService.py
--rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.7.17.post2/spai/cli/src/usecases/project/StopService.py
--rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.7.17.post2/spai/cli/src/usecases/project/__init__.py
--rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.7.17.post2/spai/cli/src/usecases/project/init_project.py
--rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.7.17.post2/spai/cli/src/usecases/project/main.py
--rw-r--r--   0        0        0     5617 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/README.md
--rw-r--r--   0        0        0      860 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
--rw-r--r--   0        0        0       20 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/apis/analytics/requirements.txt
--rw-r--r--   0        0        0     1798 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
--rw-r--r--   0        0        0       72 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/apis/xyz/requirements.txt
--rw-r--r--   0        0        0   780104 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
--rw-r--r--   0        0        0   479926 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
--rw-r--r--   0        0        0       31 2023-07-17 09:12:37.333760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/requirements.txt
--rw-r--r--   0        0        0       54 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
--rw-r--r--   0        0        0     1083 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
--rw-r--r--   0        0        0       64 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/requirements.txt
--rw-r--r--   0        0        0      524 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
--rw-r--r--   0        0        0       30 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/ndvi/requirements.txt
--rw-r--r--   0        0        0      941 2023-07-17 09:12:37.329759 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/spai.config.yml
--rw-r--r--   0        0        0     1689 2023-07-17 09:12:37.373760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/uis/map/main.py
--rw-r--r--   0        0        0       23 2023-07-17 09:12:37.373760 spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/uis/map/requirements.txt
--rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.7.17.post2/spai/cli/src/usecases/run/__init__.py
--rw-r--r--   0        0        0     3646 2023-07-12 08:58:37.693605 spai-2023.7.17.post2/spai/cli/src/usecases/run/cloud.py
--rw-r--r--   0        0        0     3458 2023-07-12 07:21:02.211592 spai-2023.7.17.post2/spai/cli/src/usecases/run/local.py
--rw-r--r--   0        0        0     3780 2023-07-12 06:51:07.529211 spai-2023.7.17.post2/spai/cli/src/usecases/run/validate.py
--rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.7.17.post2/spai/data/__init__.py
--rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.7.17.post2/spai/data/satellite/__init__.py
--rw-r--r--   0        0        0     1188 2023-07-12 12:20:02.332533 spai-2023.7.17.post2/spai/data/satellite/download.py
--rw-r--r--   0        0        0      647 2023-07-12 09:55:19.447608 spai-2023.7.17.post2/spai/data/satellite/explore.py
--rw-r--r--   0        0        0     3448 2023-07-12 12:20:01.620532 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHDownloader.py
--rw-r--r--   0        0        0     2538 2023-07-12 08:22:59.982605 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHExplorer.py
--rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py
--rw-r--r--   0        0        0     1264 2023-07-12 12:20:00.660531 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py
--rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
--rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
--rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.7.17.post2/spai/data/satellite/sentinelhub/__init__.py
--rw-r--r--   0        0        0     7130 2023-07-12 08:37:23.561984 spai-2023.7.17.post2/spai/data/satellite/utils.py
--rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.7.17.post2/spai/image/__init__.py
--rw-r--r--   0        0        0     1350 2023-07-12 13:13:58.227261 spai-2023.7.17.post2/spai/image/utils.py
--rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.7.17.post2/spai/image/xyz/__init__.py
--rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.7.17.post2/spai/image/xyz/cache.py
--rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.7.17.post2/spai/image/xyz/errors.py
--rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.7.17.post2/spai/image/xyz/get_image_tile.py
--rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.7.17.post2/spai/image/xyz/image_utils.py
--rw-r--r--   0        0        0     2298 2023-07-04 14:28:43.830331 spai-2023.7.17.post2/spai/main.py
--rw-r--r--   0        0        0        0 2023-07-10 11:09:54.127903 spai-2023.7.17.post2/spai/pulses/__init__.py
--rw-r--r--   0        0        0       41 2023-07-10 11:10:22.811986 spai-2023.7.17.post2/spai/pulses/forest-monitoring.py
--rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.7.17.post2/spai/storage/BaseStorage.py
--rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.7.17.post2/spai/storage/CloudStorage.py
--rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.7.17.post2/spai/storage/Storage.py
--rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.7.17.post2/spai/storage/__init__.py
--rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.7.17.post2/spai/storage/minio.py
--rw-r--r--   0        0        0     1723 1970-01-01 00:00:00.000000 spai-2023.7.17.post2/setup.py
--rw-r--r--   0        0        0      798 1970-01-01 00:00:00.000000 spai-2023.7.17.post2/PKG-INFO
+-rw-r--r--   0        0        0       57 2023-06-09 06:48:31.112024 spai-2023.7.4/README.md
+-rw-r--r--   0        0        0      378 2023-07-04 15:45:54.547735 spai-2023.7.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-25 05:56:52.038729 spai-2023.7.4/spai/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-09 10:26:06.805927 spai-2023.7.4/spai/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 05:53:50.146413 spai-2023.7.4/spai/cli/commands/__init__.py
+-rw-r--r--   0        0        0      950 2023-06-09 08:58:19.195513 spai-2023.7.4/spai/cli/commands/auth.py
+-rw-r--r--   0        0        0        0 2023-06-09 08:55:40.482622 spai-2023.7.4/spai/cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-06-09 08:55:40.490621 spai-2023.7.4/spai/cli/src/errors/auth.py
+-rw-r--r--   0        0        0     2479 2023-06-12 10:28:14.981273 spai-2023.7.4/spai/cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      985 2023-06-09 08:57:32.155257 spai-2023.7.4/spai/cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       60 2023-06-09 08:57:23.015206 spai-2023.7.4/spai/cli/src/repos/__init__.py
+-rw-r--r--   0        0        0     1587 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-06-09 08:55:33.898583 spai-2023.7.4/spai/cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      716 2023-06-09 08:57:34.415269 spai-2023.7.4/spai/cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      466 2023-06-09 11:53:22.345855 spai-2023.7.4/spai/cli/src/usecases/project/GetLogs.py
+-rw-r--r--   0        0        0      669 2023-07-04 12:57:35.512652 spai-2023.7.4/spai/cli/src/usecases/project/GetServices.py
+-rw-r--r--   0        0        0      482 2023-06-09 11:33:56.178515 spai-2023.7.4/spai/cli/src/usecases/project/RunService.py
+-rw-r--r--   0        0        0      492 2023-06-09 11:53:19.529847 spai-2023.7.4/spai/cli/src/usecases/project/ScheduleService.py
+-rw-r--r--   0        0        0      510 2023-06-09 11:19:01.311705 spai-2023.7.4/spai/cli/src/usecases/project/StopService.py
+-rw-r--r--   0        0        0      125 2023-06-09 11:48:45.469043 spai-2023.7.4/spai/cli/src/usecases/project/__init__.py
+-rw-r--r--   0        0        0      391 2023-06-09 11:06:06.948997 spai-2023.7.4/spai/cli/src/usecases/project/init_project.py
+-rw-r--r--   0        0        0     1350 2023-06-09 11:53:23.257858 spai-2023.7.4/spai/cli/src/usecases/project/main.py
+-rw-r--r--   0        0        0     5617 2023-05-26 12:00:02.150333 spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md
+-rw-r--r--   0        0        0      648 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/analytics/main.py
+-rw-r--r--   0        0        0     1570 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py
+-rw-r--r--   0        0        0   780104 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb
+-rw-r--r--   0        0        0   783403 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/output.ipynb
+-rw-r--r--   0        0        0       54 2023-05-26 11:59:24.882199 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/.env.example
+-rw-r--r--   0        0        0     1198 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py
+-rw-r--r--   0        0        0      524 2023-05-26 11:56:34.213566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py
+-rw-r--r--   0        0        0      529 2023-05-26 12:01:08.490568 spai-2023.7.4/spai/cli/src/usecases/project/project-template/spai.config.yml
+-rw-r--r--   0        0        0     1421 2023-05-26 11:56:34.225566 spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py
+-rw-r--r--   0        0        0      108 2023-06-09 10:28:57.166050 spai-2023.7.4/spai/cli/src/usecases/run/__init__.py
+-rw-r--r--   0        0        0     3591 2023-06-09 12:16:07.390164 spai-2023.7.4/spai/cli/src/usecases/run/cloud.py
+-rw-r--r--   0        0        0     3143 2023-06-09 10:29:07.730004 spai-2023.7.4/spai/cli/src/usecases/run/local.py
+-rw-r--r--   0        0        0     3698 2023-07-04 10:07:01.300284 spai-2023.7.4/spai/cli/src/usecases/run/validate.py
+-rw-r--r--   0        0        0        0 2023-05-19 06:35:36.838003 spai-2023.7.4/spai/data/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-25 06:12:52.855484 spai-2023.7.4/spai/data/satellite/__init__.py
+-rw-r--r--   0        0        0     1694 2023-05-25 08:13:53.594295 spai-2023.7.4/spai/data/satellite/download.py
+-rw-r--r--   0        0        0     1194 2023-05-25 06:52:32.506705 spai-2023.7.4/spai/data/satellite/explore.py
+-rw-r--r--   0        0        0     3400 2023-05-25 06:20:08.928458 spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py
+-rw-r--r--   0        0        0     2528 2023-05-25 06:53:39.046996 spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py
+-rw-r--r--   0        0        0      854 2023-05-25 06:56:10.755647 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py
+-rw-r--r--   0        0        0     1209 2023-05-25 06:16:32.727955 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py
+-rw-r--r--   0        0        0      275 2023-05-25 06:56:56.219839 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L1CDownloader.py
+-rw-r--r--   0        0        0      276 2023-05-25 05:49:51.650010 spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2L2ADownloader.py
+-rw-r--r--   0        0        0      176 2023-05-25 06:57:02.707866 spai-2023.7.4/spai/data/satellite/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       29 2023-05-25 13:36:54.194947 spai-2023.7.4/spai/image/__init__.py
+-rw-r--r--   0        0        0     1293 2023-05-25 09:01:28.729625 spai-2023.7.4/spai/image/utils.py
+-rw-r--r--   0        0        0       95 2023-05-25 13:32:15.318266 spai-2023.7.4/spai/image/xyz/__init__.py
+-rw-r--r--   0        0        0     2026 2023-05-25 13:32:39.966326 spai-2023.7.4/spai/image/xyz/cache.py
+-rw-r--r--   0        0        0      575 2023-05-25 13:32:27.546296 spai-2023.7.4/spai/image/xyz/errors.py
+-rw-r--r--   0        0        0     6924 2023-05-25 13:31:09.006104 spai-2023.7.4/spai/image/xyz/get_image_tile.py
+-rw-r--r--   0        0        0     1828 2023-05-25 13:32:00.366229 spai-2023.7.4/spai/image/xyz/image_utils.py
+-rw-r--r--   0        0        0     2298 2023-07-04 14:28:43.830331 spai-2023.7.4/spai/main.py
+-rw-r--r--   0        0        0     1915 2023-05-26 08:51:56.602852 spai-2023.7.4/spai/storage/BaseStorage.py
+-rw-r--r--   0        0        0     3605 2023-05-26 08:52:19.331037 spai-2023.7.4/spai/storage/CloudStorage.py
+-rw-r--r--   0        0        0     2537 2023-05-30 10:26:02.759827 spai-2023.7.4/spai/storage/Storage.py
+-rw-r--r--   0        0        0       68 2023-05-25 09:01:59.821768 spai-2023.7.4/spai/storage/__init__.py
+-rw-r--r--   0        0        0      535 2023-05-25 07:41:40.204202 spai-2023.7.4/spai/storage/minio.py
+-rw-r--r--   0        0        0     1522 1970-01-01 00:00:00.000000 spai-2023.7.4/setup.py
+-rw-r--r--   0        0        0      516 1970-01-01 00:00:00.000000 spai-2023.7.4/PKG-INFO
```

### Comparing `spai-2023.7.17.post2/spai/cli/commands/auth.py` & `spai-2023.7.4/spai/cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/repos/APIRepo.py` & `spai-2023.7.4/spai/cli/src/repos/APIRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/repos/AuthRepo.py` & `spai-2023.7.4/spai/cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/auth/Auth.py` & `spai-2023.7.4/spai/cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/auth/main.py` & `spai-2023.7.4/spai/cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/GetServices.py` & `spai-2023.7.4/spai/cli/src/usecases/project/GetServices.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/README.md` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/README.md`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/apis/xyz/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/apis/xyz/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from fastapi.middleware.cors import CORSMiddleware
 from fastapi import FastAPI
 from starlette.responses import StreamingResponse
 from fastapi import HTTPException, status
 import uvicorn
-import argparse
 
 from spai.image.xyz import get_image_data, get_tile_data, ready_image
 from spai.image.xyz.errors import ImageOutOfBounds
 from spai.storage import Storage
 
 # init api
 app = FastAPI(title="xyz")
@@ -55,14 +54,11 @@
         tile = get_image_data(tile, stretch, palette)
         image = ready_image(tile)
         return StreamingResponse(image, media_type="image/png")
     except ImageOutOfBounds as error:
         raise HTTPException(status_code=status.HTTP_404_NOT_FOUND, detail=error.message)
 
 
-# need this to run in background
+# put ui here !
+
 if __name__ == "__main__":
-    parser = argparse.ArgumentParser()
-    parser.add_argument("--host", type=str, default="0.0.0.0")
-    parser.add_argument("--port", type=int, default=8000)
-    args = parser.parse_args()
-    uvicorn.run(app, host=args.host, port=args.port)
+    uvicorn.run(app, host="0.0.0.0", port=8001)
```

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/notebooks/analytics/main.ipynb`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/downloader/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,18 +2,22 @@
 from dotenv import load_dotenv
 
 from spai.storage import Storage
 from spai.data.satellite import explore_satellite_images, download_satellite_image
 
 load_dotenv()
 
+# create time range (3 months)
+now = datetime.now()
+last_months = now - timedelta(days=30 * 3)
+time_interval = (last_months.strftime("%Y-%m-%d"), now.strftime("%Y-%m-%d"))
+
 # explore available images
-print("Looking for images in the last month")
-bbox = (2.0052191, 41.38238988, 2.17002873, 41.48530451)  # Collserola
-images = explore_satellite_images(bbox, cloud_cover=10)
+print("Looking for images in the range", time_interval)
+images = explore_satellite_images(time_interval, cloud_cover=10)
 if len(images) == 0:
     raise ValueError("No images found")
 
 # download images and save locally
 storage = Storage("data")
 sensor = "S2L2A"  # or 'S2L1C'
 existing_images = storage.list(f"{sensor}*.tif")
@@ -22,9 +26,9 @@
 for image in images:
     # check if image is already downloaded
     date = image["date"].split("T")[0]
     if date in dates:
         print("Image already downloaded:", date)
         continue
     print("Downloading new image:", date)
-    path = download_satellite_image(storage, bbox, date, sensor)
+    path = download_satellite_image(date, sensor, storage)
     print("Image saved at", path)
```

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/scripts/ndvi/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/project/project-template/uis/map/main.py` & `spai-2023.7.4/spai/cli/src/usecases/project/project-template/uis/map/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,18 @@
 import streamlit as st
 import pandas as pd
 import requests
 import pydeck as pdk
-import os
-
-# tengo que poder sacar la url de alguna manera
-
-# API_URL = "http://localhost"
-# # API_URL = "http://148.113.137.45"
-# ANALYTICS_URL = f"{API_URL}:8011"
-# XYZ_URL = f"{API_URL}:8012"
 
 st.set_page_config(page_title="SPAI Demo", page_icon="🌍")
 
 
 @st.cache_data(ttl=10)
-def get_data():  # in cloud fails because localhost is inside docker, need public url
-    api_url = os.getenv("ANALYTICS_URL")
+def get_data():
+    api_url = "http://localhost:8000/"
     analytics = requests.get(api_url).json()
     df = pd.DataFrame(analytics)
     return df
 
 
 df = get_data()
 
@@ -29,19 +21,18 @@
     "https://s3.amazonaws.com/elevation-tiles-prod/terrarium/{z}/{x}/{y}.png"
 )
 
 # Define how to parse elevation tiles
 ELEVATION_DECODER = {"rScaler": 256, "gScaler": 1, "bScaler": 1 / 256, "offset": -32768}
 
 st.sidebar.markdown("### Dates")
-
 selected_layers = [
     pdk.Layer(
         "TerrainLayer",
-        texture=f"{os.getenv('XYZ_URL')}/NDVI_{date}.tif/{{z}}/{{x}}/{{y}}.png",
+        texture=f"http://localhost:8001/NDVI_{date}.tif/{{z}}/{{x}}/{{y}}.png",
         elevation_decoder=ELEVATION_DECODER,
         elevation_data=TERRAIN_IMAGE,
     )
     for date in df.index
     if st.sidebar.checkbox(date, True)
 ]
 
@@ -57,12 +48,13 @@
             },
             layers=selected_layers,
         )
     )
 else:
     st.error("Please choose at least one layer above.")
 
+
 st.title("Vegetation Analytics")
 
 st.line_chart(df)
 if st.checkbox("Show data"):
     st.write(df)
```

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/run/cloud.py` & `spai-2023.7.4/spai/cli/src/usecases/run/cloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-import json
+import requests
 
 from ..project import get_services, stop_service, run_service, schedule_service
 
 
 def setup_files(item_type, dir):
     files = {
         item_type: open(
@@ -26,16 +26,14 @@
         "rebuild": rebuild,
         "command": item.command,
     }
     if item_type == "api" or item_type == "ui":
         data["port"] = item.port
     if item_type == "ui":
         data["command"] = item.command
-        if item.env:
-            data["env_vars"] = json.dumps(item.env)
     if item_type != "ui":
         data["storage"] = item.storage
     files = setup_files(item_type, item_dir)
     return run_service(user, item_type, files, data)
 
 
 def schedule_item(user, item, dir, typer, config, rebuild, item_type):
@@ -50,17 +48,17 @@
         "rebuild": rebuild,
     }
     return schedule_service(user, item_type, files, data)
 
 
 def run_script_or_notebook(user, item, dir, typer, config, rebuild, item_type):
     if item.run_on_start:
-        run_item(user, item, dir, typer, config, rebuild, item_type)
+        return run_item(user, item, dir, typer, config, rebuild, item_type)
     if item.run_every:
-        schedule_item(user, item, dir, typer, config, rebuild, item_type)
+        return schedule_item(user, item, dir, typer, config, rebuild, item_type)
 
 
 def check_item(user, item, project, services, typer, item_type):
     name = f"{item_type}.{item.name}"
     if name in services:
         typer.echo(f"Service '{name}' already deployed.")
         typer.echo(f"Stopping ...")  # confirm?
```

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/run/local.py` & `spai-2023.7.4/spai/cli/src/usecases/run/local.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,22 +31,17 @@
 
 
 def run_api(api, dir, port, host):
     os.chdir(dir)
     os.system(f"python apis/{api.name}/main.py --port {port} --host {host}")
 
 
-def run_ui(ui, dir, api_urls):
+def run_ui(ui, dir):
     os.chdir(dir)
-    cmd = ""
-    for name, value in ui.env.items():
-        if value in api_urls:
-            cmd += f"export {name}={api_urls[value]}; "
-    cmd += ui.command
-    os.system(cmd)
+    os.system(ui.command)
 
 
 def run_schdule():
     while True:
         schedule.run_pending()
         time.sleep(1)
 
@@ -74,33 +69,30 @@
             if notebook.run_on_start:
                 run_notebook((notebook, dir, typer))
             if notebook.run_every:
                 keep_alive = True
                 schedule.every(notebook.run_every).minutes.do(
                     run_notebook, (notebook, dir, typer)
                 )
-    api_urls = {}
     if config.apis:
         typer.echo(f"Deploying apis...")
         for api in config.apis:
             typer.echo(f"Running api '{api.name}'...")
             # TODO: reqs, env
             # load_dotenv(f"{dir}/apis/{api.name}/.env")
             p = Process(target=run_api, args=(api, dir, api.port, api.host))
             p.start()
             processes.append(p)
-            # save api_urls in case UIs need them
-            api_urls[f"api.{api.name}"] = f"http://{api.host}:{api.port}"
     if config.uis:
         typer.echo(f"Deploying uis...")
         for ui in config.uis:
             typer.echo(f"Running ui '{ui.name}'...")
             # TODO: reqs, env
             # load_dotenv(f"{dir}/apis/{api.name}/.env")
-            p = Process(target=run_ui, args=(ui, dir, api_urls))
+            p = Process(target=run_ui, args=(ui, dir))
             p.start()
             processes.append(p)
     typer.echo(f"Project '{config.project}' deployed.")
     if keep_alive:
         p = Process(target=run_schdule)
         p.start()
         processes.append(p)
```

### Comparing `spai-2023.7.17.post2/spai/cli/src/usecases/run/validate.py` & `spai-2023.7.4/spai/cli/src/usecases/run/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,14 @@
     storage: Union[str, None] = None  # folder to bind in cloud
 
 
 class UIConfig(BaseModel):
     name: str
     command: str  # steamlit, javascript, ...
     port: int = 3000
-    env: dict = {}  # can accept the name of another service as a url placeholder
 
 
 class Config(BaseModel):
     project: Union[str, None] = None
     scripts: Union[List[ScriptConfig], None] = None
     notebooks: Union[List[NotebookConfig], None] = None
     apis: Union[List[APIConfig], None] = None
```

### Comparing `spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHDownloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHDownloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,15 @@
         date_next_day = date_next_day.strftime("%Y-%m-%d")
         self.time_interval = (date_day_before, date_next_day)
 
     def download(self, gdf, date):
         self.prepare_time_interval(date)
         self.compute_image_size(gdf)
         if self.bbox_size[0] > 2500 or self.bbox_size[1] > 2500:
-            # return self.download_large_area(gdf)
-            raise Exception("Area too large")
+            return self.download_large_area(gdf)
         return self.download_small_area(self.bbox)
 
     def request_bands(self, bbox):
         return SentinelHubRequest(
             data_folder=self.download_folder,
             evalscript=self.script,
             input_data=[
```

### Comparing `spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHExplorer.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHExplorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 self.fields["include"].append("properties.eo:cloud_cover")
         elif sensor == "S5P":
             self.data_collection = DataCollection.SENTINEL5P
             # self.data_collection = DataCollection.SENTINEL3_OLCI
             self.config.sh_base_url = DataCollection.SENTINEL5P.service_url
             # self.config.sh_base_url = DataCollection.SENTINEL3_OLCI.service_url
         else:
-            raise Exception(f"Invalid sensor {sensor}")
+            raise Exception("Invalid sensor")
         self.time_interval = time_interval
         self.config.sh_client_id = os.environ["SH_CLIENT_ID"]
         self.config.sh_client_secret = os.environ["SH_CLIENT_SECRET"]
         self.config.save()
 
     def search(self, gdf):
         # generate the bbox containing the geometry
```

### Comparing `spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS1Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS1Downloader.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/data/satellite/sentinelhub/SHS2Downloader.py` & `spai-2023.7.4/spai/data/satellite/sentinelhub/SHS2Downloader.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from .SHDownloader import SHDownloader
-from sentinelhub import MosaickingOrder
 
 
 class SHS2Downloader(SHDownloader):
     def __init__(self, download_folder):
         super().__init__(download_folder)
         self.resolution = 10  # mpp
-        self.mosaicking_order = MosaickingOrder.LEAST_CC
+        self.mosaicking_order = "leastCC"
         self.script = """
             //VERSION=3
             function setup() {
                 return {
                     input: [{
                         bands: ["B01","B02","B03","B04","B05","B06","B07","B08","B8A","B09","B11","B12"],
                         units: "DN"
```

### Comparing `spai-2023.7.17.post2/spai/image/utils.py` & `spai-2023.7.4/spai/image/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import rasterio as rio
 import numpy as np
 from PIL import Image
 
 
 # TODO: should know the source in order to generate the rgb thumbnail
-def thumbnail(image, storage=None, sensor="S2L2A", size=None, factor=1):
-    ds = rio.open(image)
+def thumbnail(image, size=None, factor=1):
+    sensor = image.split("/")[-1].split("_")[0]
     if sensor == "S2L2A" or sensor == "S2L1C":
+        ds = rio.open(image)
         rgb = ds.read((4, 3, 2)) / 4000
         rgb = np.clip(rgb, 0, 1)
         rgb = np.moveaxis(rgb, 0, -1)
         rgb = (rgb * 255).astype(np.uint8)
         image = Image.fromarray(rgb)
     elif sensor == "S1":
         ds = rio.open(image)
@@ -27,11 +28,9 @@
         image = Image.fromarray(rgb)
     else:
         raise Exception(f"sensor {sensor} not supported")
     if size:
         image.thumbnail(size)
     elif factor != 1:
         assert factor > 0, "factor must be greater than 0"
-        image = image.resize((int(image.width // factor), int(image.height // factor)))
-    if storage is None:
-        return image
-    return storage.create(image, "thumbnail.png")
+        return image.resize((int(image.width // factor), int(image.height // factor)))
+    return image
```

### Comparing `spai-2023.7.17.post2/spai/image/xyz/cache.py` & `spai-2023.7.4/spai/image/xyz/cache.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/image/xyz/errors.py` & `spai-2023.7.4/spai/image/xyz/errors.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/image/xyz/get_image_tile.py` & `spai-2023.7.4/spai/image/xyz/get_image_tile.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/image/xyz/image_utils.py` & `spai-2023.7.4/spai/image/xyz/image_utils.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/main.py` & `spai-2023.7.4/spai/main.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/storage/BaseStorage.py` & `spai-2023.7.4/spai/storage/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/storage/CloudStorage.py` & `spai-2023.7.4/spai/storage/CloudStorage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/storage/Storage.py` & `spai-2023.7.4/spai/storage/Storage.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/spai/storage/minio.py` & `spai-2023.7.4/spai/storage/minio.py`

 * *Files identical despite different names*

### Comparing `spai-2023.7.17.post2/setup.py` & `spai-2023.7.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,39 +16,30 @@
  'spai.cli.src.usecases.project.project-template.uis.map',
  'spai.cli.src.usecases.run',
  'spai.data',
  'spai.data.satellite',
  'spai.data.satellite.sentinelhub',
  'spai.image',
  'spai.image.xyz',
- 'spai.pulses',
  'spai.storage']
 
 package_data = \
 {'': ['*'],
  'spai.cli.src.usecases.project': ['project-template/*',
                                    'project-template/notebooks/analytics/*']}
 
 install_requires = \
-['PyJWT>=2.7.0,<3.0.0',
- 'PyYAML>=6.0.0,<7.0.0',
- 'minio>=7.1.15,<8.0.0',
- 'overpy>=0.6,<0.7',
- 'pandas>=2.0.2,<3.0.0',
- 'pydantic>=2.0.3,<3.0.0',
- 'requests>=2.31.0,<3.0.0',
- 'schedule>=1.2.0,<2.0.0',
- 'typer>=0.9.0,<0.10.0']
+['minio>=7.1.15,<8.0.0', 'pandas>=2.0.2,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['spai = spai.main:app']}
 
 setup_kwargs = {
     'name': 'spai',
-    'version': '2023.7.17.post2',
+    'version': '2023.7.4',
     'description': '',
     'long_description': '# SPAI CLI\n\n## Create new project\n\n```bash\nspai init\n```\n',
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `spai-2023.7.17.post2/PKG-INFO` & `spai-2023.7.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,20 @@
 Metadata-Version: 2.1
 Name: spai
-Version: 2023.7.17.post2
+Version: 2023.7.4
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: PyJWT (>=2.7.0,<3.0.0)
-Requires-Dist: PyYAML (>=6.0.0,<7.0.0)
 Requires-Dist: minio (>=7.1.15,<8.0.0)
-Requires-Dist: overpy (>=0.6,<0.7)
 Requires-Dist: pandas (>=2.0.2,<3.0.0)
-Requires-Dist: pydantic (>=2.0.3,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
-Requires-Dist: schedule (>=1.2.0,<2.0.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # SPAI CLI
 
 ## Create new project
 
 ```bash
```

