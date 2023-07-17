# Comparing `tmp/kfp-tekton-server-api-1.8.0rc5.tar.gz` & `tmp/kfp-tekton-server-api-1.8.0rc6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfp-tekton-server-api-1.8.0rc5.tar", last modified: Fri Jul 14 23:10:33 2023, max compression
+gzip compressed data, was "kfp-tekton-server-api-1.8.0rc6.tar", last modified: Mon Jul 17 19:06:14 2023, max compression
```

## Comparing `kfp-tekton-server-api-1.8.0rc5.tar` & `kfp-tekton-server-api-1.8.0rc6.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.105477 kfp-tekton-server-api-1.8.0rc5/
--rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/LICENSE
--rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-14 23:10:33.105771 kfp-tekton-server-api-1.8.0rc5/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:54:41.000000 kfp-tekton-server-api-1.8.0rc5/README.md
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.029482 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/
--rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-14 23:07:44.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/__init__.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.035134 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/
--rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-14 23:07:49.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api_client.py
--rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-14 23:07:57.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/configuration.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/exceptions.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.065858 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/
--rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/__init__.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)    10871 2023-07-14 23:01:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:54:18.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)     9912 2023-07-14 23:05:47.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3567 2023-07-14 23:02:29.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_value.py
--rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/rest.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.031389 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/
--rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-14 23:10:32.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/PKG-INFO
--rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-14 23:10:32.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/SOURCES.txt
--rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-14 23:10:32.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/dependency_links.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-14 23:10:32.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/requires.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-14 23:10:32.000000 kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/top_level.txt
--rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-14 23:10:33.106865 kfp-tekton-server-api-1.8.0rc5/setup.cfg
--rw-r--r--   0 tommyli    (501) staff       (20)     1247 2023-07-14 23:06:53.000000 kfp-tekton-server-api-1.8.0rc5/setup.py
-drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-14 23:10:33.103836 kfp-tekton-server-api-1.8.0rc5/test/
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_experiment_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_googlerpc_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_healthz_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_inline_object.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_job_mode.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_job_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_spec_runtime_config.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_upload_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_protobuf_any.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_report_run_metrics_response_report_run_metric_result.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_report_run_metrics_response_report_run_metric_result_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_run_metric_format.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_run_service_api.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_cron_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_experiment.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_experiment_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_get_healthz_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_get_template_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_job.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_experiments_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_jobs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_pipeline_versions_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_pipelines_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_runs_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_parameter.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_periodic_schedule.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_runtime.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_spec.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_version.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_read_artifact_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_relationship.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_report_run_metrics_response.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_key.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_reference.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_type.py
--rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_run.py
--rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_detail.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_metric.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_storage_state.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_status.py
--rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_trigger.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_url.py
--rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc5/test/test_v1_value.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.687806 kfp-tekton-server-api-1.8.0rc6/
+-rw-r--r--   0 tommyli    (501) staff       (20)    11357 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/LICENSE
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-17 19:06:14.688012 kfp-tekton-server-api-1.8.0rc6/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)    13066 2023-07-13 21:54:41.000000 kfp-tekton-server-api-1.8.0rc6/README.md
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.625437 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/
+-rw-r--r--   0 tommyli    (501) staff       (20)     4398 2023-07-17 19:05:22.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/__init__.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.632904 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/
+-rw-r--r--   0 tommyli    (501) staff       (20)      550 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    36823 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5448 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    35425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    69047 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13674 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    59741 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    26288 2023-07-17 19:05:28.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api_client.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    13322 2023-07-17 19:05:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/configuration.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3795 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/exceptions.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.654093 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/
+-rw-r--r--   0 tommyli    (501) staff       (20)     3447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/__init__.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4658 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2873 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4643 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10425 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6709 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2896 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4712 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     7846 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2983 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3470 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3762 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14740 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5594 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5272 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5542 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5398 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5178 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3869 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5006 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10909 2023-07-17 19:04:24.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5052 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     8397 2023-07-13 21:54:18.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    10094 2023-07-17 19:04:20.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3868 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2916 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3597 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3989 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4894 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3057 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    14091 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4126 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     6333 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2897 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4504 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4362 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3609 2023-07-17 19:05:04.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4806 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_value.py
+-rw-r--r--   0 tommyli    (501) staff       (20)    12334 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/rest.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.627891 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/
+-rw-r--r--   0 tommyli    (501) staff       (20)      504 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/PKG-INFO
+-rw-r--r--   0 tommyli    (501) staff       (20)     4343 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/SOURCES.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)        1 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/dependency_links.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       48 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/requires.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       22 2023-07-17 19:06:14.000000 kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/top_level.txt
+-rw-r--r--   0 tommyli    (501) staff       (20)       69 2023-07-17 19:06:14.688735 kfp-tekton-server-api-1.8.0rc6/setup.cfg
+-rw-r--r--   0 tommyli    (501) staff       (20)     1247 2023-07-17 19:05:39.000000 kfp-tekton-server-api-1.8.0rc6/setup.py
+drwxr-xr-x   0 tommyli    (501) staff       (20)        0 2023-07-17 19:06:14.687068 kfp-tekton-server-api-1.8.0rc6/test/
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_experiment_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1622 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_googlerpc_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)      971 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_healthz_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1694 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_inline_object.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1339 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_job_mode.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1848 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_job_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3721 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1842 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_spec_runtime_config.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1071 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_upload_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1476 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_protobuf_any.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1915 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1837 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1429 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_run_metric_format.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2682 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_run_service_api.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1659 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_cron_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2104 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1530 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1520 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_healthz_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1528 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_template_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4344 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_job.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2563 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_experiments_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     5054 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_jobs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3607 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipeline_versions_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4513 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipelines_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4306 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_runs_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1440 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_parameter.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1714 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_periodic_schedule.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4295 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1533 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_runtime.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2232 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_spec.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3261 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_version.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1538 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_read_artifact_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1416 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_relationship.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1934 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_report_run_metrics_response.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1481 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_key.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1725 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_reference.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1418 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_type.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     3628 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     4134 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_detail.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1524 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_metric.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1453 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_storage_state.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1543 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_status.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     2286 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_trigger.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1389 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_url.py
+-rw-r--r--   0 tommyli    (501) staff       (20)     1447 2023-07-13 21:36:54.000000 kfp-tekton-server-api-1.8.0rc6/test/test_v1_value.py
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/LICENSE` & `kfp-tekton-server-api-1.8.0rc6/LICENSE`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/README.md` & `kfp-tekton-server-api-1.8.0rc6/README.md`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/__init__.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Contact: kubeflow-pipelines@google.com
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
-__version__ = "1.8.0rc5"
+__version__ = "1.8.0rc6"
 
 # import apis into sdk package
 from kfp_tekton_server_api.api.experiment_service_api import ExperimentServiceApi
 from kfp_tekton_server_api.api.healthz_service_api import HealthzServiceApi
 from kfp_tekton_server_api.api.job_service_api import JobServiceApi
 from kfp_tekton_server_api.api.pipeline_service_api import PipelineServiceApi
 from kfp_tekton_server_api.api.pipeline_upload_service_api import PipelineUploadServiceApi
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/__init__.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/job_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api/run_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api/run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/api_client.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/1.8.0rc5/python'
+        self.user_agent = 'OpenAPI-Generator/1.8.0rc6/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/configuration.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,16 +347,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 1.8.0rc5\n"\
-               "SDK Package Version: 1.8.0rc5".\
+               "Version of the API: 1.8.0rc6\n"\
+               "SDK Package Version: 1.8.0rc6".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/exceptions.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/__init__.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/inline_object.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/job_mode.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_job.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,22 +42,23 @@
         'error': 'str',
         'default_version': 'V1PipelineVersion',
         'resource_references': 'list[V1ResourceReference]'
     }
 
     attribute_map = {
         'id': 'id',
-        'created_at': 'createdAt',
+        # 'created_at': 'createdAt',
         'name': 'name',
         'description': 'description',
         'parameters': 'parameters',
         'url': 'url',
         'error': 'error',
         'default_version': 'defaultVersion',
-        'resource_references': 'resourceReferences'
+        'resource_references': 'resourceReferences',
+        'created_at': 'created_at'
     }
 
     def __init__(self, id=None, created_at=None, name=None, description=None, parameters=None, url=None, error=None, default_version=None, resource_references=None, local_vars_configuration=None):  # noqa: E501
         """V1Pipeline - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_pipeline_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,20 +42,24 @@
         'resource_references': 'list[V1ResourceReference]',
         'description': 'str'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        'created_at': 'createdAt',
+        # 'created_at': 'createdAt',
         'parameters': 'parameters',
-        'code_source_url': 'codeSourceUrl',
-        'package_url': 'packageUrl',
-        'resource_references': 'resourceReferences',
-        'description': 'description'
+        # 'code_source_url': 'codeSourceUrl',
+        # 'package_url': 'packageUrl',
+        # 'resource_references': 'resourceReferences',
+        'description': 'description',
+        'created_at': 'created_at',
+        'code_source_url': 'code_source_url',
+        'package_url': 'package_url',
+        'resource_references': 'resource_references'
     }
 
     def __init__(self, id=None, name=None, created_at=None, parameters=None, code_source_url=None, package_url=None, resource_references=None, description=None, local_vars_configuration=None):  # noqa: E501
         """V1PipelineVersion - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_status.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_url.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_url.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'pipeline_url': 'str'
     }
 
     attribute_map = {
-        'pipeline_url': 'pipelineUrl'
+        # 'pipeline_url': 'pipelineUrl',
+        'pipeline_url': 'pipeline_url'
     }
 
     def __init__(self, pipeline_url=None, local_vars_configuration=None):  # noqa: E501
         """V1Url - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration()
         self.local_vars_configuration = local_vars_configuration
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/models/v1_value.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/models/v1_value.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api/rest.py` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api/rest.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/kfp_tekton_server_api.egg-info/SOURCES.txt` & `kfp-tekton-server-api-1.8.0rc6/kfp_tekton_server_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/setup.py` & `kfp-tekton-server-api-1.8.0rc6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "kfp-tekton-server-api"
-VERSION = "1.8.0rc5"
+VERSION = "1.8.0rc6"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_experiment_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_experiment_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_googlerpc_status.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_googlerpc_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_healthz_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_healthz_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_inline_object.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_inline_object.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_job_mode.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_job_mode.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_job_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_job_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_spec_runtime_config.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_spec_runtime_config.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_pipeline_upload_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_pipeline_upload_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_protobuf_any.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_protobuf_any.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_report_run_metrics_response_report_run_metric_result.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_report_run_metrics_response_report_run_metric_result_status.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_report_run_metrics_response_report_run_metric_result_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_run_metric_format.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_run_metric_format.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_run_service_api.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_run_service_api.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_cron_schedule.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_cron_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_experiment.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_experiment_storage_state.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_experiment_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_get_healthz_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_healthz_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_get_template_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_get_template_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_job.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_job.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_experiments_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_experiments_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_jobs_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_jobs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_pipeline_versions_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipeline_versions_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_pipelines_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_pipelines_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_list_runs_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_list_runs_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_parameter.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_parameter.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_periodic_schedule.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_periodic_schedule.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_runtime.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_runtime.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_spec.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_spec.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_pipeline_version.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_pipeline_version.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_read_artifact_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_read_artifact_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_relationship.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_relationship.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_report_run_metrics_response.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_report_run_metrics_response.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_key.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_key.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_reference.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_reference.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_resource_type.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_resource_type.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_run.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_detail.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_detail.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_metric.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_metric.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_run_storage_state.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_run_storage_state.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_status.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_status.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_trigger.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_trigger.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_url.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_url.py`

 * *Files identical despite different names*

### Comparing `kfp-tekton-server-api-1.8.0rc5/test/test_v1_value.py` & `kfp-tekton-server-api-1.8.0rc6/test/test_v1_value.py`

 * *Files identical despite different names*

