# Comparing `tmp/dragonk8s-1.0.2.tar.gz` & `tmp/dragonk8s-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonk8s-1.0.2.tar", last modified: Mon Jul 17 12:21:38 2023, max compression
+gzip compressed data, was "dragonk8s-1.0.3.tar", last modified: Mon Jul 17 13:05:02 2023, max compression
```

## Comparing `dragonk8s-1.0.2.tar` & `dragonk8s-1.0.3.tar`

### file list

```diff
@@ -1,293 +1,293 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.462954 dragonk8s-1.0.2/
--rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-17 12:21:38.463072 dragonk8s-1.0.2/PKG-INFO
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.259984 dragonk8s-1.0.2/dragonk8s/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 01:14:53.000000 dragonk8s-1.0.2/dragonk8s/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.262565 dragonk8s-1.0.2/dragonk8s/cmd/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/cmd/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2300 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/cmd/replicaset_controller.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.268540 dragonk8s-1.0.2/dragonk8s/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)    20327 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.269306 dragonk8s-1.0.2/dragonk8s/dragon/api/
--rw-r--r--   0 bytedance   (501) staff       (20)       87 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/dragon/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    25570 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/api_client.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/dragon/configuration.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/dragon/exceptions.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.388051 dragonk8s-1.0.2/dragonk8s/dragon/models/
--rw-r--r--   0 bytedance   (501) staff       (20)    19839 2023-07-08 07:31:36.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7340 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7160 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11281 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5424 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6311 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4536 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py
--rw-r--r--   0 bytedance   (501) staff       (20)    56389 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5932 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8080 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5669 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7051 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5771 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4948 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6305 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9118 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8852 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6036 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6084 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5914 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9472 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9206 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8504 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9422 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6151 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9338 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7400 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8561 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6613 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4830 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)    33173 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8609 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3990 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6588 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4367 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5772 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5101 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7896 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6144 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5807 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6430 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5684 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4014 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py
--rw-r--r--   0 bytedance   (501) staff       (20)    35072 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5208 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py
--rw-r--r--   0 bytedance   (501) staff       (20)    12563 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6531 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6579 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5787 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5952 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7957 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8074 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3958 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5003 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8566 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6126 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6411 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4531 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5007 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15402 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3918 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5628 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4679 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4691 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5749 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4520 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8264 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5030 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5036 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5717 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15919 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5173 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4976 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6182 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4372 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5354 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5162 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8175 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6203 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5636 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6869 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3894 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6813 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7305 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6992 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9041 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11636 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3902 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4117 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5403 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5415 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13690 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8578 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4788 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18343 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18391 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py
--rw-r--r--   0 bytedance   (501) staff       (20)    18069 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6689 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6024 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4890 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9521 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4599 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6669 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6012 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9501 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py
--rw-r--r--   0 bytedance   (501) staff       (20)    15875 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8948 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3950 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9007 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py
--rw-r--r--   0 bytedance   (501) staff       (20)    22109 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7066 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5968 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5077 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6112 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6010 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5079 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9982 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py
--rw-r--r--   0 bytedance   (501) staff       (20)    30790 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7634 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9920 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8637 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4659 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7550 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7335 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6125 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8587 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py
--rw-r--r--   0 bytedance   (501) staff       (20)     7781 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py
--rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/dragon/rest.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.389019 dragonk8s-1.0.2/dragonk8s/lib/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.389467 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.391070 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.393638 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/api/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5346 2023-07-17 06:22:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/api/errors.py
--rw-r--r--   0 bytedance   (501) staff       (20)       50 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/api/meta.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.395924 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/apis/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/apis/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      228 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/apis/meta_internal_version.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3992 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py
--rw-r--r--   0 bytedance   (501) staff       (20)     9011 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/labels.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.397310 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/runtime/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/runtime/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2082 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/runtime/schema.py
--rw-r--r--   0 bytedance   (501) staff       (20)      210 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/selection.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.398911 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/types/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/types/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      253 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/types/patch.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.400182 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.402134 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/validation/
--rw-r--r--   0 bytedance   (501) staff       (20)       89 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/validation/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3534 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/validation/field.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1464 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/wait.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.404629 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/watch/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/watch/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4802 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/watch/mux.py
--rw-r--r--   0 bytedance   (501) staff       (20)      436 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/watch/watch.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.406817 dragonk8s-1.0.2/dragonk8s/lib/apimeta/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/apimeta/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1607 2023-07-08 07:54:43.000000 dragonk8s-1.0.2/dragonk8s/lib/apimeta/apigvk.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.411660 dragonk8s-1.0.2/dragonk8s/lib/client/
--rw-r--r--   0 bytedance   (501) staff       (20)    12934 2023-07-08 07:45:28.000000 dragonk8s-1.0.2/dragonk8s/lib/client/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    26010 2023-07-08 07:39:40.000000 dragonk8s-1.0.2/dragonk8s/lib/client/api_client.py
--rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/configuration.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/exceptions.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.414031 dragonk8s-1.0.2/dragonk8s/lib/client/informers/
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/informers/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.415218 dragonk8s-1.0.2/dragonk8s/lib/client/informers/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/informers/dragon/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1823 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/informers/dragon/replicaset.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4242 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/client/informers/factory.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1043 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/informers/informer.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.416031 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.416460 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.416897 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.417801 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      761 2023-07-08 01:05:12.000000 dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.418580 dragonk8s-1.0.2/dragonk8s/lib/client/lister/
--rw-r--r--   0 bytedance   (501) staff       (20)     2982 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/lister/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/rest.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.425981 dragonk8s-1.0.2/dragonk8s/lib/client/tools/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11820 2023-07-17 12:17:45.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/cache.py
--rw-r--r--   0 bytedance   (501) staff       (20)    11329 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/delta.py
--rw-r--r--   0 bytedance   (501) staff       (20)    14093 2023-07-17 12:21:10.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/events.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5330 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/fifo.py
--rw-r--r--   0 bytedance   (501) staff       (20)    30330 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/informer.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2200 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/pager.py
--rw-r--r--   0 bytedance   (501) staff       (20)    19026 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/record.py
--rw-r--r--   0 bytedance   (501) staff       (20)      908 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/tools/reference.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.430173 dragonk8s-1.0.2/dragonk8s/lib/client/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/util/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1182 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/lib/client/util/flow_control.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3604 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/client/util/trans.py
--rw-r--r--   0 bytedance   (501) staff       (20)     8618 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/dragonk8s/lib/client/util/workqueue.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.431528 dragonk8s-1.0.2/dragonk8s/lib/models/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/models/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      165 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/models/corev1.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.432803 dragonk8s-1.0.2/dragonk8s/lib/pool/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/pool/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1609 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/pool/thread_manager.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.434123 dragonk8s-1.0.2/dragonk8s/lib/util/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.435360 dragonk8s-1.0.2/dragonk8s/lib/util/cache/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/cache/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1738 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/cache/lru.py
--rw-r--r--   0 bytedance   (501) staff       (20)      238 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/string.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.436649 dragonk8s-1.0.2/dragonk8s/lib/util/timeutil/
--rw-r--r--   0 bytedance   (501) staff       (20)     1008 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/timeutil/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     6557 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/lib/util/timeutil/rate.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.437698 dragonk8s-1.0.2/dragonk8s/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.438569 dragonk8s-1.0.2/dragonk8s/pkg/api/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/api/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/api/types.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.439729 dragonk8s-1.0.2/dragonk8s/pkg/api/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/api/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1770 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/pkg/api/v1/pod_util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.440767 dragonk8s-1.0.2/dragonk8s/pkg/controller/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/controller/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    19819 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/pkg/controller/controller_utils.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.443400 dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)    21656 2023-07-09 10:27:36.000000 dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/replica_set.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5025 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/replica_set_utils.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.261706 dragonk8s-1.0.2/dragonk8s.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-17 12:21:38.000000 dragonk8s-1.0.2/dragonk8s.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)    15788 2023-07-17 12:21:38.000000 dragonk8s-1.0.2/dragonk8s.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-17 12:21:38.000000 dragonk8s-1.0.2/dragonk8s.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       16 2023-07-17 12:21:38.000000 dragonk8s-1.0.2/dragonk8s.egg-info/top_level.txt
--rw-r--r--   0 bytedance   (501) staff       (20)     1098 2023-07-17 12:21:38.463757 dragonk8s-1.0.2/setup.cfg
--rw-r--r--   0 bytedance   (501) staff       (20)      285 2023-07-17 12:21:29.000000 dragonk8s-1.0.2/setup.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.444030 dragonk8s-1.0.2/tests/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.445376 dragonk8s-1.0.2/tests/dragon/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/dragon/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5940 2023-07-08 07:53:20.000000 dragonk8s-1.0.2/tests/dragon/test_client.py
--rw-r--r--   0 bytedance   (501) staff       (20)     4575 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/tests/dragon/test_infromer.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.446060 dragonk8s-1.0.2/tests/lib/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.454640 dragonk8s-1.0.2/tests/lib/client/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.455422 dragonk8s-1.0.2/tests/lib/client/kubernetes/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/kubernetes/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.455741 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.456245 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.457555 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/v1/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/v1/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     5071 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.460288 dragonk8s-1.0.2/tests/lib/client/tools/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/client/tools/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      433 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/tests/lib/client/tools/test_cache.py
--rw-r--r--   0 bytedance   (501) staff       (20)     2133 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/tests/lib/client/tools/test_events.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1296 2023-07-08 01:05:11.000000 dragonk8s-1.0.2/tests/lib/client/tools/test_record.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1704 2023-07-06 13:41:18.000000 dragonk8s-1.0.2/tests/lib/client/util_test.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.461270 dragonk8s-1.0.2/tests/lib/until/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/lib/until/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      450 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/tests/lib/until/test_util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.461825 dragonk8s-1.0.2/tests/pkg/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/pkg/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 12:21:38.462368 dragonk8s-1.0.2/tests/pkg/controller/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.2/tests/pkg/controller/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     3840 2023-07-08 01:05:10.000000 dragonk8s-1.0.2/tests/pkg/controller/test_controller_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.117298 dragonk8s-1.0.3/
+-rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-17 13:05:02.117629 dragonk8s-1.0.3/PKG-INFO
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:01.836795 dragonk8s-1.0.3/dragonk8s/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 01:14:53.000000 dragonk8s-1.0.3/dragonk8s/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:01.839879 dragonk8s-1.0.3/dragonk8s/cmd/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/cmd/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2300 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/cmd/replicaset_controller.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:01.844618 dragonk8s-1.0.3/dragonk8s/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)    20327 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:01.845566 dragonk8s-1.0.3/dragonk8s/dragon/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)       87 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/dragon/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    25570 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/api_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/dragon/configuration.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/dragon/exceptions.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.042058 dragonk8s-1.0.3/dragonk8s/dragon/models/
+-rw-r--r--   0 bytedance   (501) staff       (20)    19839 2023-07-08 07:31:36.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7340 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7160 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11281 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5424 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6311 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4536 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    56389 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5932 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8080 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5669 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7051 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5771 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4948 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6305 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9118 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8852 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6036 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6084 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5914 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9472 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9206 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8504 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9422 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6151 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9338 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7400 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3926 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8561 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6613 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4830 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    33173 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8609 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3990 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6588 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4367 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5772 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5101 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7896 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6144 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5807 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6430 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5684 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4014 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    35072 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5208 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12563 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6531 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6579 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5787 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5952 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7957 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8074 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3958 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5003 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8566 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6126 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6411 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4531 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5007 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15402 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3918 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5628 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4679 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4691 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5749 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4520 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8264 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5030 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5036 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5717 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15919 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5173 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4976 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6182 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4372 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5354 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5162 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8175 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6203 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5636 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6869 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3894 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6813 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7305 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6992 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9041 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11636 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3902 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4117 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15963 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5403 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5415 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13690 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3934 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8578 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4788 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18343 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18391 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    18069 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6689 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6024 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4890 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9521 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4599 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6669 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6012 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9501 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    15875 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8948 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3950 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9007 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    22109 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7066 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5968 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5077 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6112 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6010 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5079 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9982 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    30790 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7634 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9920 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8637 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4659 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7550 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7335 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6125 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8587 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     7781 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/dragon/rest.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.042786 dragonk8s-1.0.3/dragonk8s/lib/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.043169 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.044709 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.049880 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5346 2023-07-17 06:22:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/api/errors.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       50 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/api/meta.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.052407 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/apis/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/apis/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      228 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/apis/meta_internal_version.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3992 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     9011 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/labels.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.053729 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/runtime/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/runtime/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2082 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/runtime/schema.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      210 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/selection.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.055645 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/types/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/types/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      253 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/types/patch.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.057219 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.059081 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/validation/
+-rw-r--r--   0 bytedance   (501) staff       (20)       89 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/validation/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3534 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/validation/field.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1464 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/wait.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.061048 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/watch/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/watch/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4802 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/watch/mux.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      436 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/watch/watch.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.062050 dragonk8s-1.0.3/dragonk8s/lib/apimeta/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/apimeta/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1607 2023-07-08 07:54:43.000000 dragonk8s-1.0.3/dragonk8s/lib/apimeta/apigvk.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.066745 dragonk8s-1.0.3/dragonk8s/lib/client/
+-rw-r--r--   0 bytedance   (501) staff       (20)    12934 2023-07-08 07:45:28.000000 dragonk8s-1.0.3/dragonk8s/lib/client/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    26010 2023-07-08 07:39:40.000000 dragonk8s-1.0.3/dragonk8s/lib/client/api_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    13219 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/configuration.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3789 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/exceptions.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.069157 dragonk8s-1.0.3/dragonk8s/lib/client/informers/
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/informers/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.070321 dragonk8s-1.0.3/dragonk8s/lib/client/informers/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/informers/dragon/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1823 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/informers/dragon/replicaset.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4242 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/client/informers/factory.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1043 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/informers/informer.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.071149 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.071520 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.071901 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.072592 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      761 2023-07-08 01:05:12.000000 dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.073364 dragonk8s-1.0.3/dragonk8s/lib/client/lister/
+-rw-r--r--   0 bytedance   (501) staff       (20)     2982 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/lister/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    12500 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/rest.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.080713 dragonk8s-1.0.3/dragonk8s/lib/client/tools/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11820 2023-07-17 12:17:45.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/cache.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    11329 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/delta.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    14076 2023-07-17 13:03:29.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/events.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5330 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/fifo.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    30330 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/informer.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2200 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/pager.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    19026 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/record.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      908 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/tools/reference.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.084611 dragonk8s-1.0.3/dragonk8s/lib/client/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/util/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1182 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/lib/client/util/flow_control.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3604 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/client/util/trans.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     8618 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/dragonk8s/lib/client/util/workqueue.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.086246 dragonk8s-1.0.3/dragonk8s/lib/models/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/models/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      165 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/models/corev1.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.087852 dragonk8s-1.0.3/dragonk8s/lib/pool/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/pool/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1609 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/pool/thread_manager.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.089533 dragonk8s-1.0.3/dragonk8s/lib/util/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.090558 dragonk8s-1.0.3/dragonk8s/lib/util/cache/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/cache/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1738 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/cache/lru.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      238 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/string.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.091668 dragonk8s-1.0.3/dragonk8s/lib/util/timeutil/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1008 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/timeutil/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     6557 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/lib/util/timeutil/rate.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.092387 dragonk8s-1.0.3/dragonk8s/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.093142 dragonk8s-1.0.3/dragonk8s/pkg/api/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/api/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)       78 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/api/types.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.094352 dragonk8s-1.0.3/dragonk8s/pkg/api/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/api/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1770 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/pkg/api/v1/pod_util.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.096955 dragonk8s-1.0.3/dragonk8s/pkg/controller/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/controller/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    19819 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/pkg/controller/controller_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.100278 dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-07-08 00:12:50.000000 dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)    21656 2023-07-09 10:27:36.000000 dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/replica_set.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5025 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/replica_set_utils.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:01.838974 dragonk8s-1.0.3/dragonk8s.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)      526 2023-07-17 13:05:01.000000 dragonk8s-1.0.3/dragonk8s.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)    15788 2023-07-17 13:05:01.000000 dragonk8s-1.0.3/dragonk8s.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2023-07-17 13:05:01.000000 dragonk8s-1.0.3/dragonk8s.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       16 2023-07-17 13:05:01.000000 dragonk8s-1.0.3/dragonk8s.egg-info/top_level.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)     1098 2023-07-17 13:05:02.118588 dragonk8s-1.0.3/setup.cfg
+-rw-r--r--   0 bytedance   (501) staff       (20)      285 2023-07-17 13:04:51.000000 dragonk8s-1.0.3/setup.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.101112 dragonk8s-1.0.3/tests/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.103501 dragonk8s-1.0.3/tests/dragon/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/dragon/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5940 2023-07-08 07:53:20.000000 dragonk8s-1.0.3/tests/dragon/test_client.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     4575 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/tests/dragon/test_infromer.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.104427 dragonk8s-1.0.3/tests/lib/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.105608 dragonk8s-1.0.3/tests/lib/client/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.107211 dragonk8s-1.0.3/tests/lib/client/kubernetes/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/kubernetes/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.107820 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.108645 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.109861 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/v1/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/v1/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     5071 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.112866 dragonk8s-1.0.3/tests/lib/client/tools/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/client/tools/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      433 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/tests/lib/client/tools/test_cache.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     2133 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/tests/lib/client/tools/test_events.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1296 2023-07-08 01:05:11.000000 dragonk8s-1.0.3/tests/lib/client/tools/test_record.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1704 2023-07-06 13:41:18.000000 dragonk8s-1.0.3/tests/lib/client/util_test.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.114227 dragonk8s-1.0.3/tests/lib/until/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/lib/until/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      450 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/tests/lib/until/test_util.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.115196 dragonk8s-1.0.3/tests/pkg/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/pkg/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2023-07-17 13:05:02.116390 dragonk8s-1.0.3/tests/pkg/controller/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2023-03-27 07:36:27.000000 dragonk8s-1.0.3/tests/pkg/controller/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     3840 2023-07-08 01:05:10.000000 dragonk8s-1.0.3/tests/pkg/controller/test_controller_utils.py
```

### Comparing `dragonk8s-1.0.2/PKG-INFO` & `dragonk8s-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonk8s
-Version: 1.0.2
+Version: 1.0.3
 Summary: A k8s implement of Python3
 Home-page: https://dragonk8s.com
 Author: ma
 Author-email: 591867837@qq.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dragonk8s-1.0.2/dragonk8s/cmd/replicaset_controller.py` & `dragonk8s-1.0.3/dragonk8s/cmd/replicaset_controller.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/__init__.py` & `dragonk8s-1.0.3/dragonk8s/dragon/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/api_client.py` & `dragonk8s-1.0.3/dragonk8s/dragon/api_client.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/configuration.py` & `dragonk8s-1.0.3/dragonk8s/dragon/configuration.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/exceptions.py` & `dragonk8s-1.0.3/dragonk8s/dragon/exceptions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/__init__.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_list.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_selector_match_expressions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preference_match_expressions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_preferred_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_node_affinity_required_during_scheduling_ignored_during_execution_node_selector_terms.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_label_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_pod_affinity_term_namespace_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_preferred_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_affinity_required_during_scheduling_ignored_during_execution.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_affinity_pod_anti_affinity.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_aws_elastic_block_store.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_azure_file.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cephfs_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_cinder_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_items.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_config_map_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_containers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_csi_node_publish_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_dns_config_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_items.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_downward_api_resource_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_empty_dir.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_env_from.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_containers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_data_source_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_resources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ephemeral_volume_claim_template_spec_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_fc.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flex_volume_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_flocker.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_gce_persistent_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_git_repo.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_glusterfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_aliases.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_host_path.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_image_pull_secrets.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_iscsi_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_label_selector.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_exec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_http_get_http_headers.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_post_start_tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_lifecycle_pre_stop.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_grpc.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_liveness_probe_tcp_socket.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_nfs.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_os.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_photon_persistent_disk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_ports.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_portworx_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_config_map.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_downward_api.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_secret.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_service_account_token.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_projected_sources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_quobyte.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_rbd_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_gates.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_readiness_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_resources1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_scale_io_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_sysctls.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context2_windows_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_capabilities.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_se_linux_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_seccomp_profile.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_security_context_windows_options.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_startup_probe.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_storageos_secret_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_tolerations.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_topology_spread_constraints.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_config_map_key_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_resource_field_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_value_from_secret_key_ref.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_devices.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volume_mounts.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_volumes.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_spec_template_spec_vsphere_volume.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_conditions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_job_status_uncounted_terminated_pods.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_list.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_spec.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py` & `dragonk8s-1.0.3/dragonk8s/dragon/models/io_dragon_apps_v1_replica_set_status_conditions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/dragon/rest.py` & `dragonk8s-1.0.3/dragonk8s/dragon/rest.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/api/errors.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/api/errors.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/apis/meta_v1.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/labels.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/labels.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/runtime/schema.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/runtime/schema.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/validation/field.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/validation/field.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/util/wait.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/util/wait.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimachinery/pkg/watch/mux.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimachinery/pkg/watch/mux.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/apimeta/apigvk.py` & `dragonk8s-1.0.3/dragonk8s/lib/apimeta/apigvk.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/__init__.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/api_client.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/api_client.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/configuration.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/configuration.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/exceptions.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/informers/dragon/replicaset.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/informers/dragon/replicaset.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/informers/factory.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/informers/factory.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/informers/informer.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/informers/informer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/kubernetes/typed/core/v1/event_expansion.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/lister/__init__.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/lister/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/rest.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/rest.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/cache.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/cache.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/delta.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/delta.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/events.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/events.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         if event.metadata is None or event.metadata.namespace == "":
             raise Exception("can't update an event with empty namespace")
         return self.client.replace(body=event, name=event.metadata.name, namespace=event.metadata.namespace)
 
     def patch(self, event: EventsV1Event, data) -> EventsV1Event:
         if event.metadata is None or event.metadata.namespace == "":
             raise Exception("can't patch an event with empty namespace")
-        return self.client.patch_namespaced_event(body=data, name=event.metadata.name,
+        return self.client.patch(body=data, name=event.metadata.name,
                                                   namespace=event.metadata.namespace,
                                                   content_type=patch.PatchType.StrategicMergePatchType)
 
 
 def _create_patch_for_series(event: EventsV1Event) -> dict:
     if event.series is None:
         return dict()
@@ -194,15 +194,15 @@
         namespace = ref_regarding.namespace
         if namespace is None or namespace == "":
             namespace = meta_v1.NamespaceDefault
         return EventsV1Event(
             api_version="events.k8s.io/v1",
             kind="Event",
             metadata=V1ObjectMeta(
-                name="%s.%d" % (ref_regarding.name, timestamp),
+                name="%s.%f" % (ref_regarding.name, timestamp),
                 namespace=namespace,
             ),
             event_time=timeutil.to_time_str_with_ns(timestamp),
             series=None,
             reporting_controller=reporting_controller,
             reporting_instance=reporting_instance,
             action=action,
```

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/fifo.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/fifo.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/informer.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/informer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/pager.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/pager.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/record.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/record.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/tools/reference.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/tools/reference.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/util/flow_control.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/util/flow_control.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/util/trans.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/util/trans.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/client/util/workqueue.py` & `dragonk8s-1.0.3/dragonk8s/lib/client/util/workqueue.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/pool/thread_manager.py` & `dragonk8s-1.0.3/dragonk8s/lib/pool/thread_manager.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/util/cache/lru.py` & `dragonk8s-1.0.3/dragonk8s/lib/util/cache/lru.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/util/timeutil/__init__.py` & `dragonk8s-1.0.3/dragonk8s/lib/util/timeutil/__init__.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/lib/util/timeutil/rate.py` & `dragonk8s-1.0.3/dragonk8s/lib/util/timeutil/rate.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/pkg/api/v1/pod_util.py` & `dragonk8s-1.0.3/dragonk8s/pkg/api/v1/pod_util.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/pkg/controller/controller_utils.py` & `dragonk8s-1.0.3/dragonk8s/pkg/controller/controller_utils.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/replica_set.py` & `dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/replica_set.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s/pkg/controller/replicaset/replica_set_utils.py` & `dragonk8s-1.0.3/dragonk8s/pkg/controller/replicaset/replica_set_utils.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/dragonk8s.egg-info/PKG-INFO` & `dragonk8s-1.0.3/dragonk8s.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dragonk8s
-Version: 1.0.2
+Version: 1.0.3
 Summary: A k8s implement of Python3
 Home-page: https://dragonk8s.com
 Author: ma
 Author-email: 591867837@qq.com
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `dragonk8s-1.0.2/dragonk8s.egg-info/SOURCES.txt` & `dragonk8s-1.0.3/dragonk8s.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/setup.cfg` & `dragonk8s-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/dragon/test_client.py` & `dragonk8s-1.0.3/tests/dragon/test_client.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/dragon/test_infromer.py` & `dragonk8s-1.0.3/tests/dragon/test_infromer.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py` & `dragonk8s-1.0.3/tests/lib/client/kubernetes/typed/core/v1/test_event_expansion.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/lib/client/tools/test_events.py` & `dragonk8s-1.0.3/tests/lib/client/tools/test_events.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/lib/client/tools/test_record.py` & `dragonk8s-1.0.3/tests/lib/client/tools/test_record.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/lib/client/util_test.py` & `dragonk8s-1.0.3/tests/lib/client/util_test.py`

 * *Files identical despite different names*

### Comparing `dragonk8s-1.0.2/tests/pkg/controller/test_controller_utils.py` & `dragonk8s-1.0.3/tests/pkg/controller/test_controller_utils.py`

 * *Files identical despite different names*

