# Comparing `tmp/Finance-Seleya-1.1.4.tar.gz` & `tmp/Finance-Seleya-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Finance-Seleya-1.1.4.tar", last modified: Wed Jul  5 08:01:19 2023, max compression
+gzip compressed data, was "dist/Finance-Seleya-1.1.5.tar", last modified: Mon Jul 17 00:57:20 2023, max compression
```

## Comparing `Finance-Seleya-1.1.4.tar` & `Finance-Seleya-1.1.5.tar`

### file list

```diff
@@ -1,124 +1,116 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3312 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      213 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/Finance_Seleya.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      145 2023-07-05 06:31:30.000000 Finance-Seleya-1.1.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      211 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/requirements/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/requirements/py2.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/requirements/py3.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/
--rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/audit/esg_metrics.py
--rw-r--r--   0 root         (0) root         (0)   306958 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/blob_service.c
--rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/blob_service.pyx
--rw-r--r--   0 root         (0) root         (0)   425791 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/calendar.c
--rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/calendar.pyx
--rw-r--r--   0 root         (0) root         (0)   538976 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/file_util.c
--rw-r--r--   0 root         (0) root         (0)     7223 2023-07-05 03:01:47.000000 Finance-Seleya-1.1.4/seleya/Toolset/file_util.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/Toolset/portfolio/esg_metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/
--rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/runner.py
--rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/tests/suite.py
--rw-r--r--   0 root         (0) root         (0)   331551 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/Toolset/translator.c
--rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/Toolset/translator.pyx
--rw-r--r--   0 root         (0) root         (0)     2074 2023-07-05 03:10:06.000000 Finance-Seleya-1.1.4/seleya/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/config/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/config/__init__.py
--rw-r--r--   0 root         (0) root         (0)      489 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/config/default_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/core/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/env.pyx
--rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/fixes.pyx
--rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/helper.pyx
--rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.4/seleya/core/parallel.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/
--rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/
--rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/ESG.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/GD.py
--rw-r--r--   0 root         (0) root         (0)     4296 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/SEARCH.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/USER.py
--rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/__init__.py
--rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/http/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/fetch_engine.py
--rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/mongodb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)    36127 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/db_factory.py
--rw-r--r--   0 root         (0) root         (0)     7397 2023-04-17 00:03:09.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/fetch_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/DataAPI/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/
--rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/
--rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/basic.py
--rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/engine.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
--rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
--rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/
--rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/__init__.py
--rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/basic.py
--rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
--rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
--rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/engine.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
--rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
--rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
--rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/industry.py
--rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/metrics.py
--rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
--rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sector.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/mfc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/
--rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505167 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.c
--rw-r--r--   0 root         (0) root         (0)     7687 2023-06-24 10:01:03.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/__init__.py
--rw-r--r--   0 root         (0) root         (0)   886071 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.c
--rw-r--r--   0 root         (0) root         (0)    22737 2023-04-02 13:21:46.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/__init__.py
--rw-r--r--   0 root         (0) root         (0)   469404 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.c
--rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.pyx
--rw-r--r--   0 root         (0) root         (0)   501218 2023-07-05 03:10:53.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.c
--rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/mfc/micro/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.4/seleya/mfc/micro/__init__.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/seleya.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/seleya/utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3293 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/api_base.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.4/seleya/utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.4/seleya/utilities/kd_logger.py
--rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/singleton.py
--rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.4/seleya/utilities/warning.py
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-05 08:00:55.000000 Finance-Seleya-1.1.4/seleya/version.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 08:01:19.000000 Finance-Seleya-1.1.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3762 2023-07-05 06:18:11.000000 Finance-Seleya-1.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3059 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      213 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/Finance_Seleya.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      145 2023-07-05 06:31:30.000000 Finance-Seleya-1.1.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      211 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        9 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/requirements/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/requirements/py2.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.5/requirements/py3.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/Toolset/
+-rw-r--r--   0 root         (0) root         (0)      107 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/Toolset/audit/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/audit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/Toolset/audit/esg_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     3486 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/Toolset/blob_service.py
+-rw-r--r--   0 root         (0) root         (0)     4827 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/calendar.py
+-rw-r--r--   0 root         (0) root         (0)     7223 2023-07-05 03:01:47.000000 Finance-Seleya-1.1.5/seleya/Toolset/file_util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/Toolset/portfolio/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/portfolio/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6676 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/Toolset/portfolio/esg_metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/Toolset/tests/
+-rw-r--r--   0 root         (0) root         (0)       24 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      632 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/tests/runner.py
+-rw-r--r--   0 root         (0) root         (0)      244 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/tests/suite.py
+-rw-r--r--   0 root         (0) root         (0)     5733 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/Toolset/translator.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2023-07-05 03:10:06.000000 Finance-Seleya-1.1.5/seleya/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/config/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/config/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      489 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/config/default_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.5/seleya/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3121 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.5/seleya/core/env.pyx
+-rw-r--r--   0 root         (0) root         (0)     9714 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.5/seleya/core/fixes.pyx
+-rw-r--r--   0 root         (0) root         (0)     7809 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.5/seleya/core/helper.pyx
+-rw-r--r--   0 root         (0) root         (0)     1921 2022-11-11 11:55:10.000000 Finance-Seleya-1.1.5/seleya/core/parallel.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/
+-rw-r--r--   0 root         (0) root         (0)       94 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/ESG.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/GD.py
+-rw-r--r--   0 root         (0) root         (0)     4296 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/SEARCH.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/USER.py
+-rw-r--r--   0 root         (0) root         (0)      382 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      599 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/http/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)       62 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/mongo/fetch_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2408 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/mongo/mongodb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)      117 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    36297 2023-07-17 00:37:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/db_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7428 2023-07-17 00:04:32.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/fetch_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/sly/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/sly/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55584 2023-07-04 06:39:24.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/sly/sly_engine.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/DataAPI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/
+-rw-r--r--   0 root         (0) root         (0)      383 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      633 2023-02-28 12:53:15.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/basic.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-03-03 01:31:51.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/engine.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-02-28 10:24:23.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py
+-rw-r--r--   0 root         (0) root         (0)     1168 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py
+-rw-r--r--   0 root         (0) root         (0)      877 2023-02-28 12:26:53.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-03-28 11:57:26.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-03-02 23:18:44.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/basic.py
+-rw-r--r--   0 root         (0) root         (0)      626 2023-03-01 14:55:21.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-03-02 23:18:57.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/company.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-03-02 01:54:52.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py
+-rw-r--r--   0 root         (0) root         (0)      525 2023-03-02 02:20:33.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2023-03-30 06:02:56.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/engine.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/feature_importance.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/gd_overview.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py
+-rw-r--r--   0 root         (0) root         (0)      624 2023-03-28 12:22:57.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-03-28 12:11:51.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/industry.py
+-rw-r--r--   0 root         (0) root         (0)     2475 2023-03-16 08:51:54.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/metrics.py
+-rw-r--r--   0 root         (0) root         (0)      700 2023-02-24 05:29:06.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
+-rw-r--r--   0 root         (0) root         (0)      836 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/sector.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/mfc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/
+-rw-r--r--   0 root         (0) root         (0)      284 2023-03-16 07:14:16.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/qrank/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/qrank/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7687 2023-06-24 10:01:03.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/qrank/glassdoor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/sbti/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-03-01 14:22:17.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/sbti/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22737 2023-07-12 05:50:32.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/sbti/emission.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-28 01:50:45.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7878 2023-03-17 00:13:38.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/aerosol.py
+-rw-r--r--   0 root         (0) root         (0)    11460 2023-03-10 06:20:30.000000 Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/s2f.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/mfc/micro/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-06 13:27:54.000000 Finance-Seleya-1.1.5/seleya/mfc/micro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/seleya.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/seleya/utilities/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/utilities/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/utilities/api_base.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-03-03 01:22:19.000000 Finance-Seleya-1.1.5/seleya/utilities/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     5108 2023-02-20 15:07:28.000000 Finance-Seleya-1.1.5/seleya/utilities/kd_logger.py
+-rw-r--r--   0 root         (0) root         (0)      490 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/utilities/singleton.py
+-rw-r--r--   0 root         (0) root         (0)      399 2022-11-07 11:29:19.000000 Finance-Seleya-1.1.5/seleya/utilities/warning.py
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-17 00:54:57.000000 Finance-Seleya-1.1.5/seleya/version.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-17 00:57:20.000000 Finance-Seleya-1.1.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3457 2023-07-17 00:55:03.000000 Finance-Seleya-1.1.5/setup.py
```

### Comparing `Finance-Seleya-1.1.4/Finance_Seleya.egg-info/SOURCES.txt` & `Finance-Seleya-1.1.5/Finance_Seleya.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,22 +9,18 @@
 Finance_Seleya.egg-info/top_level.txt
 requirements/py2.txt
 requirements/py3.txt
 seleya/__init__.py
 seleya/seleya.py
 seleya/version.py
 seleya/Toolset/__init__.py
-seleya/Toolset/blob_service.c
-seleya/Toolset/blob_service.pyx
-seleya/Toolset/calendar.c
-seleya/Toolset/calendar.pyx
-seleya/Toolset/file_util.c
-seleya/Toolset/file_util.pyx
-seleya/Toolset/translator.c
-seleya/Toolset/translator.pyx
+seleya/Toolset/blob_service.py
+seleya/Toolset/calendar.py
+seleya/Toolset/file_util.py
+seleya/Toolset/translator.py
 seleya/Toolset/audit/__init__.py
 seleya/Toolset/audit/esg_metrics.py
 seleya/Toolset/portfolio/__init__.py
 seleya/Toolset/portfolio/esg_metrics.py
 seleya/Toolset/tests/__init__.py
 seleya/Toolset/tests/runner.py
 seleya/Toolset/tests/suite.py
@@ -74,24 +70,20 @@
 seleya/data/SurfaceAPI/sqlatom/industry.py
 seleya/data/SurfaceAPI/sqlatom/metrics.py
 seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py
 seleya/data/SurfaceAPI/sqlatom/sector.py
 seleya/mfc/__init__.py
 seleya/mfc/alchemy/__init__.py
 seleya/mfc/alchemy/qrank/__init__.py
-seleya/mfc/alchemy/qrank/glassdoor.c
-seleya/mfc/alchemy/qrank/glassdoor.pyx
+seleya/mfc/alchemy/qrank/glassdoor.py
 seleya/mfc/alchemy/sbti/__init__.py
-seleya/mfc/alchemy/sbti/emission.c
-seleya/mfc/alchemy/sbti/emission.pyx
+seleya/mfc/alchemy/sbti/emission.py
 seleya/mfc/alchemy/tsi/__init__.py
-seleya/mfc/alchemy/tsi/aerosol.c
-seleya/mfc/alchemy/tsi/aerosol.pyx
-seleya/mfc/alchemy/tsi/s2f.c
-seleya/mfc/alchemy/tsi/s2f.pyx
+seleya/mfc/alchemy/tsi/aerosol.py
+seleya/mfc/alchemy/tsi/s2f.py
 seleya/mfc/micro/__init__.py
 seleya/utilities/__init__.py
 seleya/utilities/api_base.py
 seleya/utilities/exceptions.py
 seleya/utilities/kd_logger.py
 seleya/utilities/singleton.py
 seleya/utilities/warning.py
```

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/audit/esg_metrics.py` & `Finance-Seleya-1.1.5/seleya/Toolset/audit/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/blob_service.pyx` & `Finance-Seleya-1.1.5/seleya/Toolset/blob_service.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/calendar.pyx` & `Finance-Seleya-1.1.5/seleya/Toolset/calendar.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/file_util.pyx` & `Finance-Seleya-1.1.5/seleya/Toolset/file_util.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/portfolio/esg_metrics.py` & `Finance-Seleya-1.1.5/seleya/Toolset/portfolio/esg_metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/tests/runner.py` & `Finance-Seleya-1.1.5/seleya/Toolset/tests/runner.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/Toolset/translator.pyx` & `Finance-Seleya-1.1.5/seleya/Toolset/translator.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/__init__.py` & `Finance-Seleya-1.1.5/seleya/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/core/env.pyx` & `Finance-Seleya-1.1.5/seleya/core/env.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/core/fixes.pyx` & `Finance-Seleya-1.1.5/seleya/core/fixes.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/core/helper.pyx` & `Finance-Seleya-1.1.5/seleya/core/helper.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/core/parallel.pyx` & `Finance-Seleya-1.1.5/seleya/core/parallel.pyx`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/ESG.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/http/ESG.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/GD.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/http/GD.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/SEARCH.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/http/SEARCH.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/USER.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/http/USER.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/http/utils.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/http/utils.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/mongo/mongodb.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/mongo/mongodb.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/db_factory.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/db_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,30 +101,35 @@
                 kd_logger.warning("{0} not indices".format(clause.left.name))
                 raise ("{0} not indices".format(clause.left.name))
 
         return self._fetch_engine.join(big_table=big_table,
                                        clause_list=new_list,
                                        columns=columns)
 
-    def customize(self, clause_list, columns=None, method='and'):
+    def customize(self,
+                  clause_list,
+                  columns=None,
+                  method='and',
+                  show_id=False):
         table = self._fetch_engine.name(self.__name__)
         new_list = and_(table.__dict__['flag'] == 1,
                         table.__dict__['flag'].isnot(None))
         indices = self._fetch_engine.show_indexs(self.__name__)
         for clause in clause_list:
             if clause.left.name in indices:
                 new_list.append(clause)
             else:
                 kd_logger.warning("{0} not indices".format(clause.left.name))
         if len(new_list) <= 2:
             kd_logger.error("unconditional query is not allowed")
             return pd.DataFrame()
         return self._fetch_engine.customize(table=table,
                                             clause_list=new_list,
-                                            columns=columns)
+                                            columns=columns,
+                                            show_id=show_id)
 
 
 class ShowColumnsFactory(EngineFactory):
 
     def result(self, name):
         return self._fetch_engine.show_cloumns(
             mapping_name[name]) if name in mapping_name else pd.DataFrame(
@@ -967,14 +972,15 @@
         return self._fetch_engine.ultron_gentic(rootid=rootid,
                                                 fitness=fitness,
                                                 classify=classify,
                                                 columns=columns)
 
 
 class UsersFactory(EngineFactory):
+    __name__ = 'user'
 
     def result(self, codes=None, key='id', columns=None):
         return self._fetch_engine.users(codes=codes, key=key, columns=columns)
 
 
 class CNMarketDaily(EngineFactory):
```

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/fetch_engine.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/fetch_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,29 +55,29 @@
     def show_indexs(self, name):
         indexs = [ins['column_names'] for ins in self._insp.get_indexes(name)]
         return list(set(itertools.chain.from_iterable(indexs)))
 
     def custom(self, query):
         return pd.read_sql(query, con=self._engine.sql_engine())
 
-    def customize(self, table, clause_list, columns):
+    def customize(self, table, clause_list, columns, show_id=False):
         condition = clause_list
         if columns is not None:
             cols = [
                 table.__dict__[col] for col in columns if col in table.__dict__
             ]
         else:
             cols = [table]
         query = select(cols).where(condition)
         result = pd.read_sql(query, self._engine.sql_engine())
         if 'flag' in result.columns:
             result = result.drop(['flag'], axis=1)
         if 'timestamp' in result.columns:
             result = result.drop(['timestamp'], axis=1)
-        if 'id' in result.columns:
+        if 'id' in result.columns and not show_id:
             result = result.drop(['id'], axis=1)
         return result
 
     def join(self, big_table, clause_list, columns):
         condition = clause_list
         cols = columns
         query = select(cols).select_from(big_table).where(condition)
```

### Comparing `Finance-Seleya-1.1.4/seleya/data/DataAPI/sqlatom/sly/sly_engine.py` & `Finance-Seleya-1.1.5/seleya/data/DataAPI/sqlatom/sly/sly_engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/basic.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/engine.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gd_qrank_dist.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gd_qrank_raw.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/mongo/non_gic_dist_level1.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/__init__.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/__init__.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/basic.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/basic.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/co2_emission_target.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/company.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/company_emission_temperature.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/emission_score_average.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/engine.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/engine.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/feature_importance.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/feature_importance.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/gd_reviews.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/gd_reviews_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/industry.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/industry.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/metrics.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/metrics.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/sasb_mapdom.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/data/SurfaceAPI/sqlatom/sector.py` & `Finance-Seleya-1.1.5/seleya/data/SurfaceAPI/sqlatom/sector.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/mfc/alchemy/qrank/glassdoor.pyx` & `Finance-Seleya-1.1.5/seleya/mfc/alchemy/qrank/glassdoor.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/mfc/alchemy/sbti/emission.pyx` & `Finance-Seleya-1.1.5/seleya/mfc/alchemy/sbti/emission.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/aerosol.pyx` & `Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/aerosol.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/mfc/alchemy/tsi/s2f.pyx` & `Finance-Seleya-1.1.5/seleya/mfc/alchemy/tsi/s2f.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/utilities/api_base.py` & `Finance-Seleya-1.1.5/seleya/utilities/api_base.py`

 * *Files identical despite different names*

### Comparing `Finance-Seleya-1.1.4/seleya/utilities/kd_logger.py` & `Finance-Seleya-1.1.5/seleya/utilities/kd_logger.py`

 * *Files identical despite different names*

