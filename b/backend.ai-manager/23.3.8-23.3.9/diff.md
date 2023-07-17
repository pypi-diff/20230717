# Comparing `tmp/backend.ai-manager-23.3.8.tar.gz` & `tmp/backend.ai-manager-23.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-manager-23.3.8.tar", last modified: Thu Jul  6 04:38:16 2023, max compression
+gzip compressed data, was "backend.ai-manager-23.3.9.tar", last modified: Mon Jul 17 14:36:00 2023, max compression
```

## Comparing `backend.ai-manager-23.3.8.tar` & `backend.ai-manager-23.3.9.tar`

### file list

```diff
@@ -1,251 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.800408 backend.ai-manager-23.3.8/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.800408 backend.ai-manager-23.3.8/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.804407 backend.ai-manager-23.3.8/ai/backend/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.804407 backend.ai-manager-23.3.8/ai/backend/manager/api/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/cluster_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/domainconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/groupconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/ratelimit.py
--rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    22820 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    76777 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/userconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   121225 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/api/wsproxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/dbschema.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/etcd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/fixture.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/cli/image_impl.py
--rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/harbor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/container_registry/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/idle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.808408 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.820408 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
--rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
--rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
--rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d643752544de_.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
--rw-r--r--   0 runner    (1001) docker     (123)    34759 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/dotfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/error_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    54934 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    51383 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/keypair.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/ordering.py
--rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/queryfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/resource_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/resource_preset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/scaling_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    57492 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/session.py
--rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/session_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    43458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/models/vfolder.py
--rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/pglock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/error_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/plugin/webapp.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   159742 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    62224 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/drf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/fifo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/mof.py
--rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/predicates.py
--rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/scheduler/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    30221 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/ai/backend/manager/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14740 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend.ai_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 04:38:16.824408 backend.ai-manager-23.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-06 04:38:16.000000 backend.ai-manager-23.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.208613 backend.ai-manager-23.3.9/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.208613 backend.ai-manager-23.3.9/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.212613 backend.ai-manager-23.3.9/ai/backend/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.216613 backend.ai-manager-23.3.9/ai/backend/manager/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41187 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/cluster_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7895 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/domainconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15209 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11774 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/groupconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21704 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9907 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/ratelimit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36500 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76825 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32921 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/userconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12387 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   121225 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9419 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/api/wsproxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.216613 backend.ai-manager-23.3.9/ai/backend/manager/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/dbschema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/cli/image_impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.216613 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13492 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10671 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/harbor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3808 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/container_registry/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39934 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/idle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.220613 backend.ai-manager-23.3.9/ai/backend/manager/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22229 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.220613 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.240613 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/06184d82a211_add_session_creation_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0e558d06e0e3_add_service_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3166 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0f7a4b643940_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1e673659b283_add_clusterized_column_to_agents_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/213a04e90ecf_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/360af8f33d4e_merge_f83d_and_1f55.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/36b69ddee76e_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3cf19d906e71_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3f1dafab60b2_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6458 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/51dddd79aa21_add_logs_column_on_kernel_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4948 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/57e717103287_rename_clone_allowed_to_cloneable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8446 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5e88398bc340_add_unmanaged_path_column_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/65c4a109bbc7_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1400 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2426 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5829 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/95f51fc6ffdb_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/97f6c80c8aa5_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/a7ca9f175d5f_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29414 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3029 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/bf4bae8f942e_add_kernel_host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c1409ad0e8da_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c3e74dcf1808_add_environ_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5209 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d643752544de_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3491 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3214 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3222 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ff4bfca66bf8_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34759 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13327 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/dotfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13044 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/error_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54934 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/gql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25170 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31776 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51745 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22869 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/keypair.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.240613 backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2828 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7477 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/queryfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24594 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/resource_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5606 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/resource_preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23805 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/scaling_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58306 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10949 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/session_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43815 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55151 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/models/vfolder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11475 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/pglock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/ai/backend/manager/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/plugin/error_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/plugin/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/plugin/webapp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)   160102 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62298 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/drf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4886 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/fifo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/mof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8627 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/predicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13801 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/scheduler/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30221 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7064 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/ai/backend/manager/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14825 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-17 14:36:00.000000 backend.ai-manager-23.3.9/backend.ai_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:36:00.244613 backend.ai-manager-23.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    11857 2023-07-17 14:35:59.000000 backend.ai-manager-23.3.9/setup.py
```

### Comparing `backend.ai-manager-23.3.8/PKG-INFO` & `backend.ai-manager-23.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/acl.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/admin.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/auth.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/auth.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/cluster_template.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/cluster_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/context.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/domainconfig.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/domainconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/etcd.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/events.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/events.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/exceptions.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/groupconfig.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/groupconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/image.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/logs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/manager.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/ratelimit.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/ratelimit.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/resource.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/resource.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/scaling_group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/service.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/service.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 
 
 @auth_required
 @server_status_required(ALL_ALLOWED)
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["name", "clientSessionToken"])
+            tx.AliasedKey(["name", "service_name", "clientSessionToken"])
             >> "service_name": t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
             tx.AliasedKey(["desired_session_count", "desiredSessionCount"]): t.Int,
             tx.AliasedKey(["image", "lang"]): t.String,
             tx.AliasedKey(["arch", "architecture"], default=DEFAULT_IMAGE_ARCH)
             >> "architecture": t.String,
             tx.AliasedKey(["group", "groupName", "group_name"], default="default"): t.String,
             tx.AliasedKey(["domain", "domainName", "domain_name"], default="default"): t.String,
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/session.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
             tx.AliasedKey(["template_id", "templateId"]): t.Null | tx.UUID,
-            tx.AliasedKey(["name", "clientSessionToken"], default=undefined)
+            tx.AliasedKey(["name", "session_name", "clientSessionToken"], default=undefined)
             >> "session_name": UndefChecker | t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
             tx.AliasedKey(["image", "lang"], default=undefined): UndefChecker | t.Null | t.String,
             tx.AliasedKey(["arch", "architecture"], default=DEFAULT_IMAGE_ARCH)
             >> "architecture": t.String,
             tx.AliasedKey(["type", "sessionType"], default="interactive")
             >> "session_type": tx.Enum(SessionTypes),
             tx.AliasedKey(["group", "groupName", "group_name"], default=undefined): (
@@ -560,15 +560,15 @@
 
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["name", "clientSessionToken"])
+            tx.AliasedKey(["name", "session_name", "clientSessionToken"])
             >> "session_name": t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
             tx.AliasedKey(["image", "lang"]): t.String,
             tx.AliasedKey(["arch", "architecture"], default=DEFAULT_IMAGE_ARCH)
             >> "architecture": t.String,
             tx.AliasedKey(["type", "sessionType"], default="interactive")
             >> "session_type": tx.Enum(SessionTypes),
             tx.AliasedKey(["group", "groupName", "group_name"], default="default"): t.String,
@@ -1058,15 +1058,15 @@
 
 
 @server_status_required(ALL_ALLOWED)
 @auth_required
 @check_api_params(
     t.Dict(
         {
-            tx.AliasedKey(["name", "clientSessionToken"])
+            tx.AliasedKey(["name", "session_name", "clientSessionToken"])
             >> "session_name": t.Regexp(r"^(?=.{4,64}$)\w[\w.-]*\w$", re.ASCII),
         }
     ),
 )
 async def rename_session(request: web.Request, params: Any) -> web.Response:
     root_ctx: RootContext = request.app["_root.context"]
     session_name = request.match_info["session_name"]
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/session_template.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/stream.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/stream.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/types.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/userconfig.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/userconfig.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/utils.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/vfolder.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/api/wsproxy.py` & `backend.ai-manager-23.3.9/ai/backend/manager/api/wsproxy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/__main__.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/context.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/dbschema.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/dbschema.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/etcd.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/etcd.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/fixture.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/fixture.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/gql.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/image.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/cli/image_impl.py` & `backend.ai-manager-23.3.9/ai/backend/manager/cli/image_impl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/config.py` & `backend.ai-manager-23.3.9/ai/backend/manager/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/__init__.py` & `backend.ai-manager-23.3.9/ai/backend/manager/container_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/base.py` & `backend.ai-manager-23.3.9/ai/backend/manager/container_registry/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/docker.py` & `backend.ai-manager-23.3.9/ai/backend/manager/container_registry/docker.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/harbor.py` & `backend.ai-manager-23.3.9/ai/backend/manager/container_registry/harbor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/container_registry/local.py` & `backend.ai-manager-23.3.9/ai/backend/manager/container_registry/local.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/defs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/defs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/exceptions.py` & `backend.ai-manager-23.3.9/ai/backend/manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/idle.py` & `backend.ai-manager-23.3.9/ai/backend/manager/idle.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/__init__.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/acl.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/acl.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/agent.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/env.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/env.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/01456c812164_add_idle_timeout_to_keypair_resource_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/015d84d5a5ef_add_image_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0262e50e90e0_add_ssh_keypair_into_keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/02950808ca3d_add_agent_version.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0c5733f80e4d_index_kernel_timestamps.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0d553d59f369_users_replace_is_active_to_status_and_its_info.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/0f3bc98edaa0_more_status.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/10c58e701d87_add_is_local_to_images.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/10e39a34eed5_enlarge_kernels_lang_column_length.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/11146ba02235_change_char_col_to_str.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/185852ff9872_add_vfolder_permissions_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1e8531583e20_add_dotfile_column_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1f55a65cfc4f_add_status_column_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/1fa6a31ea8e3_add_inviter_field_for_vfolder_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/202b6dcbc159_add_internal_data_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/210c4d9be768_add_keypair_resource_policy_max_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/22964745c12b_add_total_resource_slots_to_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/22e52d03fc61_add_allowed_docker_registries_in_domains.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/250e8656cf45_add_status_data.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/25e903510fa1_add_dotfiles_to_domains_and_groups.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/26d0c387e764_create_vfolder_invitations_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/2a82340fa30e_add_mounts_info_in_kernel_db.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/2b0931e4a059_convert_lang_to_image_and_registry.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/352fa4f88f61_add_tpu_slot_on_kernel_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/35923972eddb_create_kernels_status_history_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3bb80d1887d6_add_preopen_ports.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/3efd66393bd0_add_totp_activated_at_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/405aa2c39458_job_queue.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4545f5c948b3_add_io_scratch_size_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/48ab2dfefba9_reindex_kernel_updated_order.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4b7b650bc30e_add_creator_in_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4b8a66fb8d82_revamp_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/4cc87e7fbfdf_stats_refactor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/513164749de4_add_cancelled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/518ecf41f567_add_index_for_cluster_role.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/529113b08c2c_add_vfolder_type_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/548cc8aa49c8_update_cluster_columns_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/57b523dec0e8_add_tpu_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5b45f28d2cac_add_resource_opts_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5bce905c21e5_add_vfolder_host_permission.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5d8e6043455e_add_user_group_ids_in_vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5de06da3c2b5_init.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/5fbd368d12a2_add_quota_scope_id.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/60a1effa77d2_add_coordinator_address_column_on_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6129745f49b6_add_local_rank_column_in_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/69c059996cbd_add_agent_ids_col_to_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6f1c1b83870a_merge_user_s_first__last_name_into_full_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/6f5fe19894b7_vfolder_invitation_state_to_enum_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7a82e0c70122_add_group_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7dd1d81c3204_add_vfolder_mounts_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/7ea324d0535b_vfolder_and_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/80176413d8aa_keypairs_get_is_admin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/819c2b3830a9_add_user_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/81c264528f20_add_max_session_lifetime.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/854bd902b1bc_change_kernel_identification.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/857bdec5abda_add_auto_terminate_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/85984c98b90f_update_endpoint_and_routing_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/8679d0a7e22b_add_scheduled_to_kernelstatus.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/8e660aa31fe3_add_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/911023380bc9_add_architecture_column_on_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/93e9d31d40bf_agent_add_region.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9a91532c8534_add_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9bd986a75a2a_allow_kernels_scaling_group_nullable.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9c89b9011872_add_attached_devices_field_in_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9cd61b1ae70d_add_scheduable_field_to_agents.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/9e599b62f6f1_update_kernels_vfolder_mounts_vfid_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/a1fd4e7b7782_enumerate_vfolder_perms.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/a9eb2b002330_add_new_resource_policies.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ac4e179c57fe_add_totp_key_column_at_user_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/b5be363ab05c_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/b6b884fbae1f_add_session_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/babc74594aa6_add_partial_index_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/bae1a7326e8a_add_domain_model.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/bedd92de93af_add_role_column_on_kernels_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c092dabf3ee5_add_batch_session.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c401d78cc7b9_add_allowed_vfolder_hosts_to_domain_and_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c481d3dc6c7d_add_shared_memory_to_resource_presets.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c53397a490be_add_use_host_network_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/c5e4e764f9e3_add_domain_group_user_fields_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/cace152eefac_change_keypair_s_ssh_key_column_type.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ce209920f654_create_task_template_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d2aafa234374_create_error_logs_table.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d452bacd085c_add_mount_map_column_to_kernel.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d463fc5d6109_add_clone_allowed_to_vfolders.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d52bf5ec9ef3_convert_cpu_gpu_slots_to_float.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d582942886ad_add_tag_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d58a526bf837_add_password_changed_at_col.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d59ff89e7514_remove_keypair_concurrency_used.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d5cc54fd36b5_update_for_multicontainer_sessions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d6a02307a057_remove_session_resource_opts.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/d727b5da20e6_add_callback_url_to_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/f9971fbb34d9_add_state_column_to_vfolder_invitations.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/fdc9d6ac49b4_add_public_host_to_agent.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/alembic/versions/fe59ec332c07_add_is_public_flag_to_scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/base.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/base.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/domain.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/domain.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/dotfile.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/dotfile.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/endpoint.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/endpoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/error_logs.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/error_logs.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/gql.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/gql.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/image.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/image.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/kernel.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/kernel.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,16 +68,17 @@
     StructuredJSONObjectListColumn,
     URLColumn,
     batch_multiresult,
     batch_result,
     mapper_registry,
 )
 from .group import groups
-from .minilang.ordering import OrderSpecItem, QueryOrderParser
-from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
+from .minilang import JSONFieldItem
+from .minilang.ordering import ColumnMapType, QueryOrderParser
+from .minilang.queryfilter import FieldSpecType, QueryFilterParser
 from .user import users
 from .utils import ExtendedAsyncSAEngine, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
     from .gql import GraphQueryContext
 
 __all__ = (
@@ -782,14 +783,15 @@
     status = graphene.String()
     status_changed = GQLDateTime()
     status_info = graphene.String()
     status_data = graphene.JSONString()
     created_at = GQLDateTime()
     terminated_at = GQLDateTime()
     starts_at = GQLDateTime()
+    scheduled_at = GQLDateTime()
     abusing_report = graphene.JSONString()
 
     # resources
     agent = graphene.String()
     agent_addr = graphene.String()
     container_id = graphene.String()
     resource_opts = graphene.JSONString()
@@ -803,14 +805,15 @@
         from .user import UserRole
 
         is_superadmin = ctx.user["role"] == UserRole.SUPERADMIN
         if is_superadmin:
             hide_agents = False
         else:
             hide_agents = ctx.local_config["manager"]["hide-agents"]
+        status_history = row["status_history"] or {}
         return {
             # identity
             "id": row["id"],
             "idx": row["cluster_idx"],
             "role": row["cluster_role"],
             "hostname": row["cluster_hostname"],
             "cluster_idx": row["cluster_idx"],
@@ -826,14 +829,15 @@
             "status": row["status"].name,
             "status_changed": row["status_changed"],
             "status_info": row["status_info"],
             "status_data": row["status_data"],
             "created_at": row["created_at"],
             "terminated_at": row["terminated_at"],
             "starts_at": row["starts_at"],
+            "scheduled_at": status_history.get(KernelStatus.SCHEDULED.name),
             "occupied_slots": row["occupied_slots"].to_json(),
             # resources
             "agent": row["agent"] if not hide_agents else None,
             "agent_addr": row["agent_addr"] if not hide_agents else None,
             "container_id": row["container_id"] if not hide_agents else None,
             "resource_opts": row["resource_opts"],
             # statistics
@@ -864,44 +868,46 @@
         access_key: AccessKey | None,
     ) -> Optional[Mapping[str, Any]]:
         graph_ctx: GraphQueryContext = info.context
         if access_key is None:
             return None
         return await graph_ctx.registry.get_abusing_report(self.id)
 
-    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
+    _queryfilter_fieldspec: FieldSpecType = {
         "image": ("image", None),
         "architecture": ("architecture", None),
         "agent": ("agent", None),
         "agent_addr": ("agent_addr", None),
         "cluster_idx": ("cluster_idx", None),
         "local_rank": ("local_rank", None),
         "cluster_role": ("cluster_role", None),
         "cluster_hostname": ("cluster_hostname", None),
         "status": ("status", lambda s: KernelStatus[s]),
         "status_info": ("status_info", None),
         "created_at": ("created_at", dtparse),
         "status_changed": ("status_changed", dtparse),
         "terminated_at": ("terminated_at", dtparse),
+        "scheduled_at": (JSONFieldItem("status_history", KernelStatus.SCHEDULED.name), dtparse),
     }
 
-    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+    _queryorder_colmap: ColumnMapType = {
         "image": ("image", None),
         "architecture": ("architecture", None),
         "agent": ("agent", None),
         "agent_addr": ("agent_addr", None),
         "cluster_idx": ("cluster_idx", None),
         "local_rank": ("local_rank", None),
         "cluster_role": ("cluster_role", None),
         "cluster_hostname": ("cluster_hostname", None),
         "status": ("status", None),
         "status_info": ("status_info", None),
         "status_changed": ("status_info", None),
         "created_at": ("created_at", None),
         "terminated_at": ("terminated_at", None),
+        "scheduled_at": (JSONFieldItem("status_history", KernelStatus.SCHEDULED.name), None),
     }
 
     @classmethod
     async def load_count(
         cls,
         ctx: GraphQueryContext,
         session_id: SessionId,
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/keypair.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/keypair.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/ordering.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/ordering.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import Any, Callable, Mapping, Optional
+from typing import Mapping, TypeAlias
 
 import sqlalchemy as sa
 from lark import Lark, LarkError, Transformer
 from lark.lexer import Token
 
+from . import JSONFieldItem, OrderSpecItem
+
 __all__ = (
+    "ColumnMapType",
     "QueryOrderParser",
-    "OrderSpecItem",
 )
 
-OrderSpecItem = tuple[str, Optional[Callable[[sa.Column], Any]]]
-
 _grammar = r"""
     ?start: expr
     expr   : [col ("," col)*]
     col    : ORDER? CNAME
     ORDER  : "+" | "-"
     %import common.CNAME
     %import common.WS
@@ -22,31 +22,35 @@
 """
 _parser = Lark(
     _grammar,
     parser="lalr",
     maybe_placeholders=False,
 )
 
+ColumnMapType: TypeAlias = Mapping[str, OrderSpecItem] | None
+
 
 class QueryOrderTransformer(Transformer):
-    def __init__(
-        self, sa_table: sa.Table, column_map: Optional[Mapping[str, OrderSpecItem]] = None
-    ) -> None:
+    def __init__(self, sa_table: sa.Table, column_map: ColumnMapType = None) -> None:
         super().__init__()
         self._sa_table = sa_table
         self._column_map = column_map
 
     def _get_col(self, col_name: str) -> sa.Column:
         try:
             if self._column_map:
                 col_value, func = self._column_map[col_name]
-                if func is not None:
-                    col = func(self._sa_table.c[col_value])
-                else:
-                    col = self._sa_table.c[col_value]
+                match col_value:
+                    case str(column):
+                        matched_col = self._sa_table.c[column]
+                    case JSONFieldItem(_col, _key):
+                        matched_col = self._sa_table.c[_col].op("->>")(_key)
+                    case _:
+                        raise ValueError("Invalid type of field name", col_name)
+                col = func(matched_col) if func is not None else matched_col
             else:
                 col = self._sa_table.c[col_name]
             return col
         except KeyError:
             raise ValueError("Unknown/unsupported field name", col_name)
 
     def col(self, *args) -> sa.sql.elements.UnaryExpression:
@@ -62,15 +66,15 @@
         elif op == "-":
             return col.desc()
 
     expr = tuple
 
 
 class QueryOrderParser:
-    def __init__(self, column_map: Optional[Mapping[str, OrderSpecItem]] = None) -> None:
+    def __init__(self, column_map: ColumnMapType = None) -> None:
         self._column_map = column_map
         self._parser = _parser
 
     def append_ordering(
         self,
         sa_query: sa.sql.Select,
         order_expr: str,
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/minilang/queryfilter.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/minilang/queryfilter.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-from typing import Any, Callable, Mapping, Optional, Tuple, Type, Union
+from typing import Any, Mapping, Type, TypeAlias, Union
 
 import sqlalchemy as sa
 from lark import Lark, LarkError, Transformer, Tree
 from lark.lexer import Token
 
+from . import ArrayFieldItem, FieldSpecItem, JSONFieldItem
+
 __all__ = (
+    "FieldSpecType",
     "FilterableSQLQuery",
     "QueryFilterParser",
-    "FieldSpecItem",
 )
 
-FieldSpecItem = Tuple[str, Optional[Callable[[str], Any]]]
-
-FilterableSQLQuery = Union[sa.sql.Select, sa.sql.Update, sa.sql.Delete]
-
 _grammar = r"""
     ?start: expr
     value: string
            | number
            | array
            | ATOM -> atom
     ATOM       : "null" | "true" | "false"
@@ -44,19 +42,20 @@
 """
 _parser = Lark(
     _grammar,
     parser="lalr",
     maybe_placeholders=False,
 )
 
+FilterableSQLQuery = Union[sa.sql.Select, sa.sql.Update, sa.sql.Delete]
+FieldSpecType: TypeAlias = Mapping[str, FieldSpecItem] | None
+
 
 class QueryFilterTransformer(Transformer):
-    def __init__(
-        self, sa_table: sa.Table, fieldspec: Optional[Mapping[str, FieldSpecItem]] = None
-    ) -> None:
+    def __init__(self, sa_table: sa.Table, fieldspec: FieldSpecType = None) -> None:
         super().__init__()
         self._sa_table = sa_table
         self._fieldspec = fieldspec
 
     def string(self, token: list[Token]) -> str:
         s = token[0]
         # SQL-side escaping is handled by SQLAlchemy
@@ -76,73 +75,97 @@
             return sa.null()
         elif a.value == "true":
             return sa.true()
         elif a.value == "false":
             return sa.false()
         raise ValueError("Unknown/unsupported atomic token", a.value)
 
-    def _get_col(self, col_name: str) -> sa.Column:
-        try:
-            if self._fieldspec:
-                col = self._sa_table.c[self._fieldspec[col_name][0]]
-            else:
-                col = self._sa_table.c[col_name]
-            return col
-        except KeyError:
-            raise ValueError("Unknown/unsupported field name", col_name)
-
-    def _transform_val_leaf(self, col_name: str, value: Any) -> Any:
+    def _transform_val_leaf(self, col_name: str, op: str, value: Any) -> Any:
         if self._fieldspec:
             try:
                 func = self._fieldspec[col_name][1]
             except KeyError:
                 raise ValueError("Unknown/unsupported field name", col_name)
             return func(value) if func is not None else value
         else:
             return value
 
-    def _transform_val(self, col_name: str, value: Any) -> Any:
+    def _transform_val(self, col_name: str, op: str, value: Any) -> Any:
         if isinstance(value, Tree):
-            val = self._transform_val(col_name, value.children[0])
+            val = self._transform_val(col_name, op, value.children[0])
         elif isinstance(value, list):
-            val = [self._transform_val(col_name, v) for v in value]
+            val = [self._transform_val(col_name, op, v) for v in value]
         else:
-            val = self._transform_val_leaf(col_name, value)
+            val = self._transform_val_leaf(col_name, op, value)
         return val
 
     def binary_expr(self, *args) -> sa.sql.elements.BinaryExpression:
         children: list[Token] = args[0]
-        col = self._get_col(children[0].value)
+        col_name = children[0].value
         op = children[1].value
-        val = self._transform_val(children[0].value, children[2])
-        if op == "==":
-            return col == val
-        elif op == "!=":
-            return col != val
-        elif op == ">":
-            return col > val
-        elif op == ">=":
-            return col >= val
-        elif op == "<":
-            return col < val
-        elif op == "<=":
-            return col <= val
-        elif op == "contains":
-            return col.contains(val)
-        elif op == "in":
-            return col.in_(val)
-        elif op == "isnot":
-            return col.isnot(val)
-        elif op == "is":
-            return col.is_(val)
-        elif op == "like":
-            return col.like(val)
-        elif op == "ilike":
-            return col.ilike(val)
-        return args
+        val = self._transform_val(col_name, op, children[2])
+
+        def build_expr(op: str, col, val):
+            match op:
+                case "==":
+                    expr = col == val
+                case "!=":
+                    expr = col != val
+                case ">":
+                    expr = col > val
+                case ">=":
+                    expr = col >= val
+                case "<":
+                    expr = col < val
+                case "<=":
+                    expr = col <= val
+                case "contains":
+                    expr = col.contains(val)
+                case "in":
+                    expr = col.in_(val)
+                case "isnot":
+                    expr = col.isnot(val)
+                case "is":
+                    expr = col.is_(val)
+                case "like":
+                    expr = col.like(val)
+                case "ilike":
+                    expr = col.ilike(val)
+                case _:
+                    expr = args
+            return expr
+
+        try:
+            if self._fieldspec is not None:
+                match self._fieldspec[children[0].value][0]:
+                    case ArrayFieldItem(col_name):
+                        # For array columns, let's apply the expression on every item,
+                        # and select the row if anyone makes the result true.
+                        col = self._sa_table.c[col_name]
+                        unnested_col = sa.func.unnest(col).alias("item")
+                        subq = (
+                            sa.select([sa.column("item")])
+                            .select_from(unnested_col)
+                            .where(build_expr(op, sa.column("item"), val))
+                        )
+                        expr = sa.exists(subq)
+                    case JSONFieldItem(col_name, obj_key):
+                        # For json columns, we additionally indicate the object key
+                        # to retrieve the value used in the expression.
+                        col = self._sa_table.c[col_name].op("->>")(obj_key)
+                        expr = build_expr(op, col, val)
+                    case str(col_name):
+                        col = self._sa_table.c[col_name]
+                        expr = build_expr(op, col, val)
+            else:
+                col = self._sa_table.c[col_name]
+                expr = build_expr(op, col, val)
+        except KeyError:
+            raise ValueError("Unknown/unsupported field name", col_name)
+        return expr
 
     def unary_expr(self, *args):
         children = args[0]
         op = children[0].value
         expr = children[1]
         if op in ("not", "!"):
             return sa.not_(expr)
@@ -161,15 +184,15 @@
 
     def paren_expr(self, *args):
         children = args[0]
         return children[0]
 
 
 class QueryFilterParser:
-    def __init__(self, fieldspec: Optional[Mapping[str, FieldSpecItem]] = None) -> None:
+    def __init__(self, fieldspec: FieldSpecType = None) -> None:
         self._fieldspec = fieldspec
         self._parser = _parser
 
     def append_filter(
         self,
         sa_query: FilterableSQLQuery,
         filter_expr: str,
@@ -187,8 +210,10 @@
         else:
             raise ValueError("Unsupported SQLAlchemy query object type")
         try:
             ast = self._parser.parse(filter_expr)
             where_clause = QueryFilterTransformer(table, self._fieldspec).transform(ast)
         except LarkError as e:
             raise ValueError(f"Query filter parsing error: {e}")
-        return sa_query.where(where_clause)
+        final_query = sa_query.where(where_clause)
+        assert final_query is not None
+        return final_query
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/resource_policy.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/resource_policy.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/resource_preset.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/resource_preset.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/routing.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/routing.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/scaling_group.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/scaling_group.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/session.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,17 @@
     StructuredJSONObjectListColumn,
     URLColumn,
     batch_multiresult_in_session,
     batch_result_in_session,
 )
 from .group import GroupRow
 from .kernel import ComputeContainer, KernelRow, KernelStatus
-from .minilang.ordering import OrderSpecItem, QueryOrderParser
-from .minilang.queryfilter import FieldSpecItem, QueryFilterParser
+from .minilang import ArrayFieldItem, JSONFieldItem
+from .minilang.ordering import ColumnMapType, QueryOrderParser
+from .minilang.queryfilter import FieldSpecType, QueryFilterParser
 from .user import UserRow
 from .utils import ExtendedAsyncSAEngine, agg_to_array, execute_with_retry, sql_json_merge
 
 if TYPE_CHECKING:
     from sqlalchemy.engine import Row
 
     from .gql import GraphQueryContext
@@ -577,19 +578,16 @@
     group_id = ForeignKeyIDColumn("group_id", "groups.id", nullable=False)
     group = relationship("GroupRow", back_populates="sessions")
     user_uuid = ForeignKeyIDColumn("user_uuid", "users.uuid", nullable=False)
     user = relationship("UserRow", back_populates="sessions")
     access_key = sa.Column("access_key", sa.String(length=20), sa.ForeignKey("keypairs.access_key"))
     access_key_row = relationship("KeyPairRow", back_populates="sessions")
 
-    # # if image_id is null, should find a image field from related kernel row.
-    # image_id = ForeignKeyIDColumn("image_id", "images.id")
-    # # `image` column is identical to kernels `image` column.
-    # image = sa.Column("image", sa.String(length=512))
-    # image_row = relationship("ImageRow", back_populates="sessions")
+    # `image` column is identical to kernels `image` column.
+    images = sa.Column("images", sa.ARRAY(sa.String), nullable=True)
     tag = sa.Column("tag", sa.String(length=64), nullable=True)
 
     # Resource occupation
     # occupied_slots = sa.Column('occupied_slots', ResourceSlotColumn(), nullable=False)
     occupying_slots = sa.Column("occupying_slots", ResourceSlotColumn(), nullable=False)
     requested_slots = sa.Column("requested_slots", ResourceSlotColumn(), nullable=False)
     vfolder_mounts = sa.Column(
@@ -1236,22 +1234,24 @@
     status_changed = GQLDateTime()
     status_info = graphene.String()
     status_data = graphene.JSONString()
     status_history = graphene.JSONString()
     created_at = GQLDateTime()
     terminated_at = GQLDateTime()
     starts_at = GQLDateTime()
+    scheduled_at = GQLDateTime()
     startup_command = graphene.String()
     result = graphene.String()
     commit_status = graphene.String()
     abusing_reports = graphene.List(lambda: graphene.JSONString)
     idle_checks = graphene.JSONString()
 
     # resources
     agent_ids = graphene.List(lambda: graphene.String)
+    agents = graphene.List(lambda: graphene.String)
     resource_opts = graphene.JSONString()
     scaling_group = graphene.String()
     service_ports = graphene.JSONString()
     mounts = graphene.List(lambda: graphene.String)
     vfolder_mounts = graphene.List(lambda: graphene.String)
     occupying_slots = graphene.JSONString()
     occupied_slots = graphene.JSONString()  # legacy
@@ -1270,26 +1270,27 @@
     @classmethod
     def parse_row(cls, ctx: GraphQueryContext, row: Row) -> Mapping[str, Any]:
         assert row is not None
         email = getattr(row, "email")
         full_name = getattr(row, "full_name")
         group_name = getattr(row, "group_name")
         row = row.SessionRow
+        status_history = row.status_history or {}
+        raw_scheduled_at = status_history.get(SessionStatus.SCHEDULED.name)
         return {
             # identity
             "id": row.id,
             "session_id": row.id,
             "main_kernel_id": row.main_kernel.id,
             "tag": row.tag,
             "name": row.name,
             "type": row.session_type.name,
             "main_kernel_role": row.main_kernel.role.name,
             # image
-            # "image": row.image_id,
-            "image": row.main_kernel.image,
+            "image": row.images[0] if row.images is not None else "",
             "architecture": row.main_kernel.architecture,
             "registry": row.main_kernel.registry,
             "cluster_template": None,  # TODO: implement
             "cluster_mode": row.cluster_mode,
             "cluster_size": row.cluster_size,
             # ownership
             "domain_name": row.domain_name,
@@ -1302,22 +1303,26 @@
             "created_user_email": None,  # TODO: implement
             "created_user_id": None,  # TODO: implement
             # status
             "status": row.status.name,
             "status_changed": row.status_changed,
             "status_info": row.status_info,
             "status_data": row.status_data,
-            "status_history": row.status_history or {},
+            "status_history": status_history,
             "created_at": row.created_at,
             "terminated_at": row.terminated_at,
             "starts_at": row.starts_at,
+            "scheduled_at": (
+                datetime.fromisoformat(raw_scheduled_at) if raw_scheduled_at is not None else None
+            ),
             "startup_command": row.startup_command,
             "result": row.result.name,
             # resources
             "agent_ids": row.agent_ids,
+            "agents": row.agent_ids,  # for backward compatibility
             "scaling_group": row.scaling_group_name,
             "service_ports": row.main_kernel.service_ports,
             "mounts": [mount.name for mount in row.vfolder_mounts],
             "vfolder_mounts": row.vfolder_mounts,
             # statistics
             "num_queries": row.num_queries,
         }
@@ -1414,43 +1419,51 @@
         self.containers = containers
         return [(await con.resolve_abusing_report(info, self.access_key)) for con in containers]
 
     async def resolve_idle_checks(self, info: graphene.ResolveInfo) -> Mapping[str, Any]:
         graph_ctx: GraphQueryContext = info.context
         return await graph_ctx.idle_checker_host.get_idle_check_report(self.session_id)
 
-    _queryfilter_fieldspec: Mapping[str, FieldSpecItem] = {
+    _queryfilter_fieldspec: FieldSpecType = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", lambda s: SessionTypes[s]),
         "name": ("sessions_name", None),
-        "agent_ids": ("sessions_agent_ids", None),
+        "image": (ArrayFieldItem("sessions_images"), None),
+        "agent_ids": (ArrayFieldItem("sessions_agent_ids"), None),
+        "agent_id": (ArrayFieldItem("sessions_agent_ids"), None),
+        "agents": (ArrayFieldItem("sessions_agent_ids"), None),  # for backward compatibility
         "domain_name": ("sessions_domain_name", None),
         "group_name": ("group_name", None),
         "user_email": ("users_email", None),
         "full_name": ("users_full_name", None),
         "access_key": ("sessions_access_key", None),
         "scaling_group": ("sessions_scaling_group_name", None),
         "cluster_mode": ("sessions_cluster_mode", lambda s: ClusterMode[s]),
         "cluster_size": ("sessions_cluster_size", None),
         "status": ("sessions_status", lambda s: SessionStatus[s]),
         "status_info": ("sessions_status_info", None),
         "result": ("sessions_result", lambda s: SessionResult[s]),
         "created_at": ("sessions_created_at", dtparse),
         "terminated_at": ("sessions_terminated_at", dtparse),
         "starts_at": ("sessions_starts_at", dtparse),
+        "scheduled_at": (
+            JSONFieldItem("sessions_status_history", SessionStatus.SCHEDULED.name),
+            dtparse,
+        ),
         "startup_command": ("sessions_startup_command", None),
     }
 
-    _queryorder_colmap: Mapping[str, OrderSpecItem] = {
+    _queryorder_colmap: ColumnMapType = {
         "id": ("sessions_id", None),
         "type": ("sessions_session_type", None),
         "name": ("sessions_name", None),
-        # "image": "image",
-        # "architecture": "architecture",
+        "image": ("sessions_images", None),
         "agent_ids": ("sessions_agent_ids", None),
+        "agent_id": ("sessions_agent_ids", None),
+        "agents": ("sessions_agent_ids", None),
         "domain_name": ("sessions_domain_name", None),
         "group_name": ("group_name", None),
         "user_email": ("users_email", None),
         "full_name": ("users_full_name", None),
         "access_key": ("sessions_access_key", None),
         "scaling_group": ("sessions_scaling_group_name", None),
         "cluster_mode": ("sessions_cluster_mode", None),
@@ -1458,14 +1471,18 @@
         "cluster_size": ("sessions_cluster_size", None),
         "status": ("sessions_status", None),
         "status_info": ("sessions_status_info", None),
         "result": ("sessions_result", None),
         "created_at": ("sessions_created_at", None),
         "terminated_at": ("sessions_terminated_at", None),
         "starts_at": ("sessions_starts_at", None),
+        "scheduled_at": (
+            JSONFieldItem("sessions_status_history", SessionStatus.SCHEDULED.name),
+            None,
+        ),
     }
 
     @classmethod
     async def load_count(
         cls,
         ctx: GraphQueryContext,
         *,
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/session_template.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/session_template.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/storage.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/storage.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/user.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,15 +347,19 @@
             query = query.where(users.c.status == UserStatus(status))
         elif is_active is not None:  # consider is_active field only if status is empty
             _statuses = ACTIVE_USER_STATUSES if is_active else INACTIVE_USER_STATUSES
             query = query.where(users.c.status.in_(_statuses))
         if filter is not None:
             if group_id is not None:
                 qfparser = QueryFilterParser(
-                    {k: ("users_" + v[0], v[1]) for k, v in cls._queryfilter_fieldspec.items()}
+                    {
+                        k: ("users_" + v[0], v[1])
+                        for k, v in cls._queryfilter_fieldspec.items()
+                        if isinstance(v[0], str)
+                    }
                 )
             else:
                 qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         async with ctx.db.begin_readonly() as conn:
             result = await conn.execute(query)
         return result.scalar()
@@ -393,23 +397,31 @@
             query = query.where(users.c.status == UserStatus(status))
         elif is_active is not None:  # consider is_active field only if status is empty
             _statuses = ACTIVE_USER_STATUSES if is_active else INACTIVE_USER_STATUSES
             query = query.where(users.c.status.in_(_statuses))
         if filter is not None:
             if group_id is not None:
                 qfparser = QueryFilterParser(
-                    {k: ("users_" + v[0], v[1]) for k, v in cls._queryfilter_fieldspec.items()}
+                    {
+                        k: ("users_" + v[0], v[1])
+                        for k, v in cls._queryfilter_fieldspec.items()
+                        if isinstance(v[0], str)
+                    }
                 )
             else:
                 qfparser = QueryFilterParser(cls._queryfilter_fieldspec)
             query = qfparser.append_filter(query, filter)
         if order is not None:
             if group_id is not None:
                 qoparser = QueryOrderParser(
-                    {k: ("users_" + v[0], v[1]) for k, v in cls._queryorder_colmap.items()}
+                    {
+                        k: ("users_" + v[0], v[1])
+                        for k, v in cls._queryorder_colmap.items()
+                        if isinstance(v[0], str)
+                    }
                 )
             else:
                 qoparser = QueryOrderParser(cls._queryorder_colmap)
             query = qoparser.append_ordering(query, order)
         else:
             query = query.order_by(
                 users.c.created_at.desc(),
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/utils.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/models/vfolder.py` & `backend.ai-manager-23.3.9/ai/backend/manager/models/vfolder.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/openapi.py` & `backend.ai-manager-23.3.9/ai/backend/manager/openapi.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/pglock.py` & `backend.ai-manager-23.3.9/ai/backend/manager/pglock.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/plugin/error_monitor.py` & `backend.ai-manager-23.3.9/ai/backend/manager/plugin/error_monitor.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/plugin/webapp.py` & `backend.ai-manager-23.3.9/ai/backend/manager/plugin/webapp.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/registry.py` & `backend.ai-manager-23.3.9/ai/backend/manager/registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1101,14 +1101,15 @@
             "stdin_port": 0,
             "stdout_port": 0,
             "preopen_ports": sa.bindparam("preopen_ports"),
             "use_host_network": use_host_network,
         }
 
         kernel_data = []
+        session_images: list[str] = []
 
         for idx, kernel in enumerate(kernel_enqueue_configs):
             kernel_id = KernelId(uuid.uuid4())
             creation_config = kernel["creation_config"]
             image_ref = kernel["image_ref"]
             resource_opts = creation_config.get("resource_opts") or {}
 
@@ -1269,14 +1270,20 @@
                     "resource_opts": resource_opts,
                     "environ": [f"{k}={v}" for k, v in environ.items()],
                     "bootstrap_script": kernel.get("bootstrap_script"),
                     "preopen_ports": creation_config.get("preopen_ports", []),
                 }
             )
 
+            if image_ref.canonical not in session_images:
+                if kernel["cluster_role"] == DEFAULT_ROLE:
+                    session_images.insert(0, image_ref.canonical)
+                else:
+                    session_images.append(image_ref.canonical)
+        session_data["images"] = session_images
         try:
 
             async def _enqueue() -> None:
                 async with self.db.begin_session() as db_sess:
                     session_data["requested_slots"] = session_requested_slots
                     session = SessionRow(**session_data)
                     kernels = [KernelRow(**kernel) for kernel in kernel_data]
@@ -1452,15 +1459,15 @@
                         "Attachable": True,
                         "Labels": {
                             "ai.backend.cluster-network": "1",
                         },
                         "Options": {},
                     }
                     if mtu:
-                        create_options["Options"] = {"com.docker.network.driver.mtu": mtu}
+                        create_options["Options"] = {"com.docker.network.driver.mtu": str(mtu)}
                     await self.docker.networks.create(create_options)
                 except Exception:
                     log.exception(f"Failed to create an overlay network {network_name}")
                     raise
         else:
             network_name = "host"
             if scheduled_session.cluster_size > 1:
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/dispatcher.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -718,47 +718,47 @@
             await execute_with_retry(_update_generic_failure)
             raise
 
         async def _finalize_scheduled() -> None:
             agent_ids: list[AgentId] = []
             async with self.db.begin_session() as db_sess:
                 now = datetime.now(tzutc())
-                kernel_query = (
-                    sa.update(KernelRow)
-                    .values(
-                        agent=agent_alloc_ctx.agent_id,
-                        agent_addr=agent_alloc_ctx.agent_addr,
-                        scaling_group=sgroup_name,
-                        status=KernelStatus.SCHEDULED,
-                        status_info="scheduled",
-                        status_data={},
-                        status_changed=now,
-                        status_history=sql_json_merge(
-                            KernelRow.status_history,
-                            (),
-                            {
-                                KernelStatus.SCHEDULED.name: now.isoformat(),
-                            },
-                        ),
+                for kernel in sess_ctx.kernels:
+                    kernel_query = (
+                        sa.update(KernelRow)
+                        .values(
+                            agent=agent_alloc_ctx.agent_id,
+                            agent_addr=agent_alloc_ctx.agent_addr,
+                            scaling_group=sgroup_name,
+                            status=KernelStatus.SCHEDULED,
+                            status_info="scheduled",
+                            status_data={},
+                            status_changed=now,
+                            status_history=sql_json_merge(
+                                KernelRow.status_history,
+                                (),
+                                {
+                                    KernelStatus.SCHEDULED.name: now.isoformat(),
+                                },
+                            ),
+                        )
+                        .where(KernelRow.id == kernel.id)
                     )
-                    .where(KernelRow.session_id == sess_ctx.id)
-                )
-                await db_sess.execute(kernel_query)
+                    await db_sess.execute(kernel_query)
                 if agent_alloc_ctx.agent_id is not None:
                     agent_ids.append(agent_alloc_ctx.agent_id)
 
                 session_query = (
                     sa.update(SessionRow)
                     .values(
                         scaling_group_name=sgroup_name,
                         agent_ids=agent_ids,
                         status=SessionStatus.SCHEDULED,
                         status_info="scheduled",
                         status_data={},
-                        # status_changed=now,
                         status_history=sql_json_merge(
                             SessionRow.status_history,
                             (),
                             {
                                 SessionStatus.SCHEDULED.name: now.isoformat(),
                             },
                         ),
@@ -944,15 +944,15 @@
                                 KernelRow.status_history,
                                 (),
                                 {
                                     KernelStatus.SCHEDULED.name: now.isoformat(),
                                 },
                             ),
                         )
-                        .where(KernelRow.session_id == sess_ctx.id)
+                        .where(KernelRow.id == binding.kernel.id)
                     )
                     await db_sess.execute(kernel_query)
                     if binding.agent_alloc_ctx.agent_id is not None:
                         agent_ids.append(binding.agent_alloc_ctx.agent_id)
 
                 session_query = (
                     sa.update(SessionRow)
```

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/drf.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/drf.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/fifo.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/fifo.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/mof.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/mof.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/predicates.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/predicates.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/scheduler/types.py` & `backend.ai-manager-23.3.9/ai/backend/manager/scheduler/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/server.py` & `backend.ai-manager-23.3.9/ai/backend/manager/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/types.py` & `backend.ai-manager-23.3.9/ai/backend/manager/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/ai/backend/manager/utils.py` & `backend.ai-manager-23.3.9/ai/backend/manager/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/PKG-INFO` & `backend.ai-manager-23.3.9/backend.ai_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-manager
-Version: 23.3.8
+Version: 23.3.9
 Summary: Backend.AI Manager
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/SOURCES.txt` & `backend.ai-manager-23.3.9/backend.ai_manager.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,15 @@
 ai/backend/manager/models/alembic/versions/da24ff520049_add_starts_at_field_into_kernels.py
 ai/backend/manager/models/alembic/versions/dbc1e053b880_add_keypair_resource_policy.py
 ai/backend/manager/models/alembic/versions/dc9b66466e43_remove_clusterized.py
 ai/backend/manager/models/alembic/versions/e18ed5fcfedf_add_superadmin_role_for_user.py
 ai/backend/manager/models/alembic/versions/e35332f8d23d_add_modified_at_to_users_and_kernels.py
 ai/backend/manager/models/alembic/versions/e421c02cf9e4_rename_kernel_dependencies_to_session_.py
 ai/backend/manager/models/alembic/versions/e7371ca5797a_rename_mem_stats.py
+ai/backend/manager/models/alembic/versions/eb9441fcf90a_add_images_col_to_session.py
 ai/backend/manager/models/alembic/versions/ed666f476f39_add_bootstrap_script_to_keypairs.py
 ai/backend/manager/models/alembic/versions/eec98e65902a_merge_with_vfolder_clone.py
 ai/backend/manager/models/alembic/versions/f0f4ee907155_dynamic_resource_slots.py
 ai/backend/manager/models/alembic/versions/f108628f032b_add_endpoint_and_routing_tables.py
 ai/backend/manager/models/alembic/versions/f5530eccf202_add_kernels_uuid_prefix_index.py
 ai/backend/manager/models/alembic/versions/f83d630c0bc9_add_allowed_ip_column.py
 ai/backend/manager/models/alembic/versions/f8a71c3bffa2_stringify_userid.py
```

### Comparing `backend.ai-manager-23.3.8/backend.ai_manager.egg-info/requires.txt` & `backend.ai-manager-23.3.9/backend.ai_manager.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 aiohttp_sse>=2.0
 aiohttp~=3.8.1
 aiomonitor-ng~=0.7.2
 aiotools~=1.6.1
 alembic~=1.8.1
 async_timeout~=4.0
 attrs>=20.3
-backend.ai-cli==23.03.8
-backend.ai-common==23.03.8
-backend.ai-plugin==23.03.8
+backend.ai-cli==23.03.9
+backend.ai-common==23.03.9
+backend.ai-plugin==23.03.9
 callosum~=0.9.10
 click>=7.1.2
 cryptography>=2.8
 graphene~=2.1.9
 lark-parser~=0.11.3
 more-itertools~=8.13.0
 msgpack>=1.0.5rc1
```

### Comparing `backend.ai-manager-23.3.8/backend_shim.py` & `backend.ai-manager-23.3.9/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-manager-23.3.8/setup.py` & `backend.ai-manager-23.3.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,19 @@
         'aiohttp_sse>=2.0',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'alembic~=1.8.1',
         'async_timeout~=4.0',
         'attrs>=20.3',
-        """backend.ai-cli==23.03.8
+        """backend.ai-cli==23.03.9
 """,
-        """backend.ai-common==23.03.8
+        """backend.ai-common==23.03.9
 """,
-        """backend.ai-plugin==23.03.8
+        """backend.ai-plugin==23.03.9
 """,
         'callosum~=0.9.10',
         'click>=7.1.2',
         'cryptography>=2.8',
         'graphene~=2.1.9',
         'lark-parser~=0.11.3',
         'more-itertools~=8.13.0',
@@ -378,11 +378,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.8
+    'version': """23.03.9
 """,
     'zip_safe': False,
 })
```

