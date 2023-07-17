# Comparing `tmp/webknossos-0.9.8.tar.gz` & `tmp/webknossos-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webknossos-0.9.8.tar", max compression
+gzip compressed data, was "webknossos-0.9.9.tar", max compression
```

## Comparing `webknossos-0.9.8.tar` & `webknossos-0.9.9.tar`

### file list

```diff
@@ -1,173 +1,181 @@
--rw-r--r--   0        0        0    34520 2022-02-28 14:24:49.985026 webknossos-0.9.8/LICENSE
--rw-r--r--   0        0        0     2307 2022-02-28 14:24:49.985026 webknossos-0.9.8/README.md
--rw-r--r--   0        0        0     1901 2022-02-28 14:25:01.805210 webknossos-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     3405 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/__init__.py
--rw-r--r--   0        0        0      179 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/_types.py
--rw-r--r--   0        0        0      150 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/administration/__init__.py
--rw-r--r--   0        0        0     4503 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/administration/project.py
--rw-r--r--   0        0        0     7595 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/administration/task.py
--rw-r--r--   0        0        0     3931 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/administration/user.py
--rw-r--r--   0        0        0      192 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/annotation/__init__.py
--rw-r--r--   0        0        0     9958 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/annotation/annotation.py
--rw-r--r--   0        0        0     1445 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/annotation/annotation_info.py
--rw-r--r--   0        0        0      430 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/README.md
--rw-r--r--   0        0        0       81 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/__init__.py
--rw-r--r--   0        0        0       78 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_defaults.py
--rw-r--r--   0        0        0      843 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_download_annotation.py
--rw-r--r--   0        0        0     5331 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_download_dataset.py
--rw-r--r--   0        0        0       98 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/__init__.py
--rw-r--r--   0        0        0       47 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/__init__.py
--rw-r--r--   0        0        0        0 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/__init__.py
--rw-r--r--   0        0        0     1912 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_cancel_upload.py
--rw-r--r--   0        0        0     3205 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_download.py
--rw-r--r--   0        0        0     1912 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_finish_upload.py
--rw-r--r--   0        0        0     1918 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_reserve_upload.py
--rw-r--r--   0        0        0     1553 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_upload_chunk.py
--rw-r--r--   0        0        0        0 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/__init__.py
--rw-r--r--   0        0        0     1396 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/add_annotation_layer.py
--rw-r--r--   0        0        0     2422 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_download.py
--rw-r--r--   0        0        0     2681 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_info.py
--rw-r--r--   0        0        0     2520 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_infos_by_task_id.py
--rw-r--r--   0        0        0     1196 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_upload.py
--rw-r--r--   0        0        0     1925 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/build_info.py
--rw-r--r--   0        0        0     1501 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/create_project.py
--rw-r--r--   0        0        0     1987 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/current_user_info.py
--rw-r--r--   0        0        0     3267 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/dataset_info.py
--rw-r--r--   0        0        0     2270 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/datastore_list.py
--rw-r--r--   0        0        0     2104 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/generate_token_for_data_store.py
--rw-r--r--   0        0        0     1182 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/health.py
--rw-r--r--   0        0        0     1629 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/new_dataset_name_is_valid.py
--rw-r--r--   0        0        0     2133 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/project_info_by_id.py
--rw-r--r--   0        0        0     2190 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/project_info_by_name.py
--rw-r--r--   0        0        0     1546 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/task_create_from_files.py
--rw-r--r--   0        0        0     2053 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/task_info.py
--rw-r--r--   0        0        0     3956 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/task_infos_by_project_id.py
--rw-r--r--   0        0        0     2091 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/user_info_by_id.py
--rw-r--r--   0        0        0     2220 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/user_list.py
--rw-r--r--   0        0        0     2119 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/api/default/user_logged_time.py
--rw-r--r--   0        0        0     1563 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/client.py
--rw-r--r--   0        0        0     8326 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/__init__.py
--rw-r--r--   0        0        0     1120 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action.py
--rw-r--r--   0        0        0     1254 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_annotation_layer_parameters.py
--rw-r--r--   0        0        0     1176 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_any_content.py
--rw-r--r--   0        0        0     1244 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_cancel_upload_information.py
--rw-r--r--   0        0        0     1161 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_js_value.py
--rw-r--r--   0        0        0     1285 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_multipart_form_data_temporary_file.py
--rw-r--r--   0        0        0     1249 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_reserve_upload_information.py
--rw-r--r--   0        0        0     1211 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/action_upload_information.py
--rw-r--r--   0        0        0     7196 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200.py
--rw-r--r--   0        0        0     1664 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_annotation_layers_item.py
--rw-r--r--   0        0        0     2295 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_data_store.py
--rw-r--r--   0        0        0     2117 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_restrictions.py
--rw-r--r--   0        0        0     2890 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_settings.py
--rw-r--r--   0        0        0     1407 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_settings_resolution_restrictions.py
--rw-r--r--   0        0        0     1252 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_stats.py
--rw-r--r--   0        0        0     1569 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_tracing_store.py
--rw-r--r--   0        0        0     3086 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_user.py
--rw-r--r--   0        0        0     1785 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_user_teams_item.py
--rw-r--r--   0        0        0     7955 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item.py
--rw-r--r--   0        0        0     1765 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_annotation_layers_item.py
--rw-r--r--   0        0        0     2396 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_data_store.py
--rw-r--r--   0        0        0     2218 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_restrictions.py
--rw-r--r--   0        0        0     2991 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings.py
--rw-r--r--   0        0        0     1514 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings_resolution_restrictions.py
--rw-r--r--   0        0        0     1329 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_stats.py
--rw-r--r--   0        0        0     5023 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task.py
--rw-r--r--   0        0        0     1749 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_needed_experience.py
--rw-r--r--   0        0        0     1852 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_status.py
--rw-r--r--   0        0        0     3125 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type.py
--rw-r--r--   0        0        0     3095 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings.py
--rw-r--r--   0        0        0     1565 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings_resolution_restrictions.py
--rw-r--r--   0        0        0     1670 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_tracing_store.py
--rw-r--r--   0        0        0     3219 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user.py
--rw-r--r--   0        0        0     1886 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user_teams_item.py
--rw-r--r--   0        0        0     2983 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200.py
--rw-r--r--   0        0        0     2882 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200_webknossos.py
--rw-r--r--   0        0        0     2591 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200_webknossos_wrap.py
--rw-r--r--   0        0        0     1204 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/create_project_json_body.py
--rw-r--r--   0        0        0     6037 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200.py
--rw-r--r--   0        0        0     1587 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_experiences.py
--rw-r--r--   0        0        0     1388 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_novel_user_experience_infos.py
--rw-r--r--   0        0        0     1770 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_teams_item.py
--rw-r--r--   0        0        0     1237 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_cancel_upload_json_body.py
--rw-r--r--   0        0        0     1237 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_finish_upload_json_body.py
--rw-r--r--   0        0        0     5790 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200.py
--rw-r--r--   0        0        0     2559 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source.py
--rw-r--r--   0        0        0     2951 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item.py
--rw-r--r--   0        0        0     2061 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item_bounding_box.py
--rw-r--r--   0        0        0     1566 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_id.py
--rw-r--r--   0        0        0     2280 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_store.py
--rw-r--r--   0        0        0     1242 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/dataset_reserve_upload_json_body.py
--rw-r--r--   0        0        0     2262 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/datastore_list_response_200_item.py
--rw-r--r--   0        0        0     1463 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/generate_token_for_data_store_response_200.py
--rw-r--r--   0        0        0     2919 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200.py
--rw-r--r--   0        0        0     3112 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200_owner.py
--rw-r--r--   0        0        0     1801 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200_owner_teams_item.py
--rw-r--r--   0        0        0     2937 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200.py
--rw-r--r--   0        0        0     3130 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200_owner.py
--rw-r--r--   0        0        0     1811 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200_owner_teams_item.py
--rw-r--r--   0        0        0     1240 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_create_from_files_json_body.py
--rw-r--r--   0        0        0     4530 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200.py
--rw-r--r--   0        0        0     1595 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_needed_experience.py
--rw-r--r--   0        0        0     1698 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_status.py
--rw-r--r--   0        0        0     2852 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type.py
--rw-r--r--   0        0        0     2876 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type_settings.py
--rw-r--r--   0        0        0     1400 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type_settings_resolution_restrictions.py
--rw-r--r--   0        0        0     4876 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item.py
--rw-r--r--   0        0        0     1711 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_needed_experience.py
--rw-r--r--   0        0        0     1790 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_status.py
--rw-r--r--   0        0        0     3034 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type.py
--rw-r--r--   0        0        0     3028 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings.py
--rw-r--r--   0        0        0     1522 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings_resolution_restrictions.py
--rw-r--r--   0        0        0     5967 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200.py
--rw-r--r--   0        0        0     1575 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_experiences.py
--rw-r--r--   0        0        0     1376 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_novel_user_experience_infos.py
--rw-r--r--   0        0        0     1758 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_teams_item.py
--rw-r--r--   0        0        0     5961 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item.py
--rw-r--r--   0        0        0     1572 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_experiences.py
--rw-r--r--   0        0        0     1373 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_novel_user_experience_infos.py
--rw-r--r--   0        0        0     1755 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_teams_item.py
--rw-r--r--   0        0        0     2029 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200.py
--rw-r--r--   0        0        0     2163 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item.py
--rw-r--r--   0        0        0     1708 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item_payment_interval.py
--rw-r--r--   0        0        0       25 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/py.typed
--rw-r--r--   0        0        0     1021 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_generated/types.py
--rw-r--r--   0        0        0       28 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_resumable/__init__.py
--rw-r--r--   0        0        0     3598 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_resumable/chunk.py
--rw-r--r--   0        0        0     4835 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_resumable/core.py
--rw-r--r--   0        0        0     3467 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_resumable/file.py
--rw-r--r--   0        0        0      959 2022-02-28 14:24:50.041026 webknossos-0.9.8/webknossos/client/_resumable/util.py
--rw-r--r--   0        0        0     6961 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/client/_upload_dataset.py
--rw-r--r--   0        0        0     7111 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/client/context.py
--rw-r--r--   0        0        0      766 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/client/download_dataset.py
--rw-r--r--   0        0        0      789 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/__init__.py
--rw-r--r--   0        0        0     4077 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/_utils/buffered_slice_reader.py
--rw-r--r--   0        0        0     6350 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/_utils/buffered_slice_writer.py
--rw-r--r--   0        0        0     1425 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/_utils/infer_bounding_box_existing_files.py
--rw-r--r--   0        0        0      868 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/compress_utils.py
--rw-r--r--   0        0        0    34295 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/dataset.py
--rw-r--r--   0        0        0       26 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/defaults.py
--rw-r--r--   0        0        0    11848 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/downsampling_utils.py
--rw-r--r--   0        0        0    33881 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/layer.py
--rw-r--r--   0        0        0      201 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/layer_categories.py
--rw-r--r--   0        0        0    11303 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/mag_view.py
--rw-r--r--   0        0        0     7267 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/properties.py
--rw-r--r--   0        0        0     3405 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/upsampling_utils.py
--rw-r--r--   0        0        0    37716 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/dataset/view.py
--rw-r--r--   0        0        0      102 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/geometry/__init__.py
--rw-r--r--   0        0        0    15818 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/geometry/bounding_box.py
--rw-r--r--   0        0        0     3194 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/geometry/mag.py
--rw-r--r--   0        0        0     5000 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/geometry/vec3_int.py
--rw-r--r--   0        0        0       25 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/py.typed
--rw-r--r--   0        0        0      499 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/__init__.py
--rw-r--r--   0        0        0     6956 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/graph.py
--rw-r--r--   0        0        0     4029 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/group.py
--rw-r--r--   0        0        0    23699 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/nml/__init__.py
--rw-r--r--   0        0        0     4975 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/nml/from_skeleton.py
--rw-r--r--   0        0        0     2895 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/nml/to_skeleton.py
--rw-r--r--   0        0        0     1220 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/node.py
--rw-r--r--   0        0        0     3511 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/skeleton/skeleton.py
--rw-r--r--   0        0        0     5697 2022-02-28 14:24:50.045027 webknossos-0.9.8/webknossos/utils.py
--rw-r--r--   0        0        0       22 2022-02-28 14:25:01.305186 webknossos-0.9.8/webknossos/version.py
--rw-r--r--   0        0        0     3871 2022-02-28 14:25:02.612512 webknossos-0.9.8/setup.py
--rw-r--r--   0        0        0     3615 2022-02-28 14:25:02.612924 webknossos-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    34520 2022-01-28 15:48:11.227549 webknossos-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2307 2022-02-03 15:54:14.432401 webknossos-0.9.9/README.md
+-rw-r--r--   0        0        0     1942 2022-03-03 15:41:49.630170 webknossos-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     3243 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/__init__.py
+-rw-r--r--   0        0        0      266 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/__init__.py
+-rw-r--r--   0        0        0      721 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/branchpoint.py
+-rw-r--r--   0        0        0      591 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/comment.py
+-rw-r--r--   0        0        0      552 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/edge.py
+-rw-r--r--   0        0        0      686 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/group.py
+-rw-r--r--   0        0        0      577 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/meta.py
+-rw-r--r--   0        0        0     5136 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/nml.py
+-rw-r--r--   0        0        0     3879 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/node.py
+-rw-r--r--   0        0        0     7950 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/parameters.py
+-rw-r--r--   0        0        0     2360 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/tree.py
+-rw-r--r--   0        0        0      640 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/utils.py
+-rw-r--r--   0        0        0     1221 2022-03-02 13:46:28.696438 webknossos-0.9.9/webknossos/_nml/volume.py
+-rw-r--r--   0        0        0      150 2022-02-07 16:07:28.125215 webknossos-0.9.9/webknossos/administration/__init__.py
+-rw-r--r--   0        0        0     4503 2022-02-07 16:07:28.129215 webknossos-0.9.9/webknossos/administration/project.py
+-rw-r--r--   0        0        0     7629 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/administration/task.py
+-rw-r--r--   0        0        0     3931 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/administration/user.py
+-rw-r--r--   0        0        0      192 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/annotation/__init__.py
+-rw-r--r--   0        0        0     6858 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/annotation/_nml_conversion.py
+-rw-r--r--   0        0        0    28246 2022-03-03 15:40:18.521222 webknossos-0.9.9/webknossos/annotation/annotation.py
+-rw-r--r--   0        0        0     1381 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/annotation/annotation_info.py
+-rw-r--r--   0        0        0      430 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/README.md
+-rw-r--r--   0        0        0       81 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/__init__.py
+-rw-r--r--   0        0        0       78 2022-02-03 15:54:14.516402 webknossos-0.9.9/webknossos/client/_defaults.py
+-rw-r--r--   0        0        0     5331 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/client/_download_dataset.py
+-rw-r--r--   0        0        0       98 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/__init__.py
+-rw-r--r--   0        0        0       47 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/datastore/__init__.py
+-rw-r--r--   0        0        0     1912 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_cancel_upload.py
+-rw-r--r--   0        0        0     3205 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_download.py
+-rw-r--r--   0        0        0     1912 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_finish_upload.py
+-rw-r--r--   0        0        0     1918 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_reserve_upload.py
+-rw-r--r--   0        0        0     1553 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_upload_chunk.py
+-rw-r--r--   0        0        0        0 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/__init__.py
+-rw-r--r--   0        0        0     1396 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/add_annotation_layer.py
+-rw-r--r--   0        0        0     2422 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_download.py
+-rw-r--r--   0        0        0     2681 2022-01-31 15:31:19.925490 webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_info.py
+-rw-r--r--   0        0        0     2520 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_infos_by_task_id.py
+-rw-r--r--   0        0        0     1196 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_upload.py
+-rw-r--r--   0        0        0     1925 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/build_info.py
+-rw-r--r--   0        0        0     1501 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/create_project.py
+-rw-r--r--   0        0        0     1987 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/current_user_info.py
+-rw-r--r--   0        0        0     3267 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/dataset_info.py
+-rw-r--r--   0        0        0     2270 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/datastore_list.py
+-rw-r--r--   0        0        0     2104 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/generate_token_for_data_store.py
+-rw-r--r--   0        0        0     1182 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/health.py
+-rw-r--r--   0        0        0     1629 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/new_dataset_name_is_valid.py
+-rw-r--r--   0        0        0     2133 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/project_info_by_id.py
+-rw-r--r--   0        0        0     2190 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/project_info_by_name.py
+-rw-r--r--   0        0        0     1546 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/task_create_from_files.py
+-rw-r--r--   0        0        0     2053 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/task_info.py
+-rw-r--r--   0        0        0     3956 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/task_infos_by_project_id.py
+-rw-r--r--   0        0        0     2091 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/api/default/user_info_by_id.py
+-rw-r--r--   0        0        0     2220 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/user_list.py
+-rw-r--r--   0        0        0     2119 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/api/default/user_logged_time.py
+-rw-r--r--   0        0        0     1563 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/client.py
+-rw-r--r--   0        0        0     8326 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/__init__.py
+-rw-r--r--   0        0        0     1120 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action.py
+-rw-r--r--   0        0        0     1254 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action_annotation_layer_parameters.py
+-rw-r--r--   0        0        0     1176 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action_any_content.py
+-rw-r--r--   0        0        0     1244 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/action_cancel_upload_information.py
+-rw-r--r--   0        0        0     1161 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/action_js_value.py
+-rw-r--r--   0        0        0     1285 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action_multipart_form_data_temporary_file.py
+-rw-r--r--   0        0        0     1249 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action_reserve_upload_information.py
+-rw-r--r--   0        0        0     1211 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/action_upload_information.py
+-rw-r--r--   0        0        0     7196 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200.py
+-rw-r--r--   0        0        0     1664 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_annotation_layers_item.py
+-rw-r--r--   0        0        0     2295 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_data_store.py
+-rw-r--r--   0        0        0     2117 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_restrictions.py
+-rw-r--r--   0        0        0     2890 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_settings.py
+-rw-r--r--   0        0        0     1407 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_settings_resolution_restrictions.py
+-rw-r--r--   0        0        0     1252 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_stats.py
+-rw-r--r--   0        0        0     1569 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_tracing_store.py
+-rw-r--r--   0        0        0     3086 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_user.py
+-rw-r--r--   0        0        0     1785 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_user_teams_item.py
+-rw-r--r--   0        0        0     7955 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item.py
+-rw-r--r--   0        0        0     1765 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_annotation_layers_item.py
+-rw-r--r--   0        0        0     2396 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_data_store.py
+-rw-r--r--   0        0        0     2218 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_restrictions.py
+-rw-r--r--   0        0        0     2991 2022-02-07 16:07:28.133215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings.py
+-rw-r--r--   0        0        0     1514 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings_resolution_restrictions.py
+-rw-r--r--   0        0        0     1329 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_stats.py
+-rw-r--r--   0        0        0     5023 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task.py
+-rw-r--r--   0        0        0     1749 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_needed_experience.py
+-rw-r--r--   0        0        0     1852 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_status.py
+-rw-r--r--   0        0        0     3125 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type.py
+-rw-r--r--   0        0        0     3095 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings.py
+-rw-r--r--   0        0        0     1565 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings_resolution_restrictions.py
+-rw-r--r--   0        0        0     1670 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_tracing_store.py
+-rw-r--r--   0        0        0     3219 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user.py
+-rw-r--r--   0        0        0     1886 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user_teams_item.py
+-rw-r--r--   0        0        0     2983 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200.py
+-rw-r--r--   0        0        0     2882 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200_webknossos.py
+-rw-r--r--   0        0        0     2591 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200_webknossos_wrap.py
+-rw-r--r--   0        0        0     1204 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/create_project_json_body.py
+-rw-r--r--   0        0        0     6037 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200.py
+-rw-r--r--   0        0        0     1587 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_experiences.py
+-rw-r--r--   0        0        0     1388 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_novel_user_experience_infos.py
+-rw-r--r--   0        0        0     1770 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_teams_item.py
+-rw-r--r--   0        0        0     1237 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/dataset_cancel_upload_json_body.py
+-rw-r--r--   0        0        0     1237 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_finish_upload_json_body.py
+-rw-r--r--   0        0        0     5790 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200.py
+-rw-r--r--   0        0        0     2559 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source.py
+-rw-r--r--   0        0        0     2951 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item.py
+-rw-r--r--   0        0        0     2061 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item_bounding_box.py
+-rw-r--r--   0        0        0     1566 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_id.py
+-rw-r--r--   0        0        0     2280 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_store.py
+-rw-r--r--   0        0        0     1242 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/dataset_reserve_upload_json_body.py
+-rw-r--r--   0        0        0     2262 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/datastore_list_response_200_item.py
+-rw-r--r--   0        0        0     1463 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/generate_token_for_data_store_response_200.py
+-rw-r--r--   0        0        0     2919 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200.py
+-rw-r--r--   0        0        0     3112 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200_owner.py
+-rw-r--r--   0        0        0     1801 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200_owner_teams_item.py
+-rw-r--r--   0        0        0     2937 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200.py
+-rw-r--r--   0        0        0     3130 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200_owner.py
+-rw-r--r--   0        0        0     1811 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200_owner_teams_item.py
+-rw-r--r--   0        0        0     1240 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_create_from_files_json_body.py
+-rw-r--r--   0        0        0     4530 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200.py
+-rw-r--r--   0        0        0     1595 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_needed_experience.py
+-rw-r--r--   0        0        0     1698 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_status.py
+-rw-r--r--   0        0        0     2852 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type.py
+-rw-r--r--   0        0        0     2876 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type_settings.py
+-rw-r--r--   0        0        0     1400 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type_settings_resolution_restrictions.py
+-rw-r--r--   0        0        0     4876 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item.py
+-rw-r--r--   0        0        0     1711 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_needed_experience.py
+-rw-r--r--   0        0        0     1790 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_status.py
+-rw-r--r--   0        0        0     3034 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type.py
+-rw-r--r--   0        0        0     3028 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings.py
+-rw-r--r--   0        0        0     1522 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings_resolution_restrictions.py
+-rw-r--r--   0        0        0     5967 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200.py
+-rw-r--r--   0        0        0     1575 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_experiences.py
+-rw-r--r--   0        0        0     1376 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_novel_user_experience_infos.py
+-rw-r--r--   0        0        0     1758 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_teams_item.py
+-rw-r--r--   0        0        0     5961 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item.py
+-rw-r--r--   0        0        0     1572 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_experiences.py
+-rw-r--r--   0        0        0     1373 2022-02-07 16:07:28.137215 webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_novel_user_experience_infos.py
+-rw-r--r--   0        0        0     1755 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_teams_item.py
+-rw-r--r--   0        0        0     2029 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200.py
+-rw-r--r--   0        0        0     2163 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item.py
+-rw-r--r--   0        0        0     1708 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item_payment_interval.py
+-rw-r--r--   0        0        0       25 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/py.typed
+-rw-r--r--   0        0        0     1021 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_generated/types.py
+-rw-r--r--   0        0        0       28 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_resumable/__init__.py
+-rw-r--r--   0        0        0     3598 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_resumable/chunk.py
+-rw-r--r--   0        0        0     4835 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_resumable/core.py
+-rw-r--r--   0        0        0     3467 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_resumable/file.py
+-rw-r--r--   0        0        0      959 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/_resumable/util.py
+-rw-r--r--   0        0        0     6961 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/client/_upload_dataset.py
+-rw-r--r--   0        0        0     7111 2022-02-03 16:46:49.250752 webknossos-0.9.9/webknossos/client/context.py
+-rw-r--r--   0        0        0      766 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/client/download_dataset.py
+-rw-r--r--   0        0        0      789 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/__init__.py
+-rw-r--r--   0        0        0     4077 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/_utils/buffered_slice_reader.py
+-rw-r--r--   0        0        0     6350 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/_utils/buffered_slice_writer.py
+-rw-r--r--   0        0        0     1425 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/_utils/infer_bounding_box_existing_files.py
+-rw-r--r--   0        0        0      868 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/compress_utils.py
+-rw-r--r--   0        0        0    34295 2022-02-07 09:10:18.999641 webknossos-0.9.9/webknossos/dataset/dataset.py
+-rw-r--r--   0        0        0       26 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/defaults.py
+-rw-r--r--   0        0        0    11848 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/downsampling_utils.py
+-rw-r--r--   0        0        0    33881 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/dataset/layer.py
+-rw-r--r--   0        0        0      201 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/layer_categories.py
+-rw-r--r--   0        0        0    11835 2022-03-03 15:40:18.521222 webknossos-0.9.9/webknossos/dataset/mag_view.py
+-rw-r--r--   0        0        0     7267 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/properties.py
+-rw-r--r--   0        0        0     3405 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/dataset/upsampling_utils.py
+-rw-r--r--   0        0        0    37716 2022-02-21 10:48:45.394919 webknossos-0.9.9/webknossos/dataset/view.py
+-rw-r--r--   0        0        0      102 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/geometry/__init__.py
+-rw-r--r--   0        0        0    15818 2022-02-09 14:58:50.654040 webknossos-0.9.9/webknossos/geometry/bounding_box.py
+-rw-r--r--   0        0        0     3194 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/geometry/mag.py
+-rw-r--r--   0        0        0     5000 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/geometry/vec3_int.py
+-rw-r--r--   0        0        0       25 2022-01-28 15:48:11.599553 webknossos-0.9.9/webknossos/py.typed
+-rw-r--r--   0        0        0      518 2022-03-03 15:40:18.521222 webknossos-0.9.9/webknossos/skeleton/__init__.py
+-rw-r--r--   0        0        0     6957 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/skeleton/graph.py
+-rw-r--r--   0        0        0     4056 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/skeleton/group.py
+-rw-r--r--   0        0        0     1221 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/skeleton/node.py
+-rw-r--r--   0        0        0     2918 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/skeleton/skeleton.py
+-rw-r--r--   0        0        0     5697 2022-03-02 13:46:28.700438 webknossos-0.9.9/webknossos/utils.py
+-rw-r--r--   0        0        0       22 2022-03-03 15:41:47.174145 webknossos-0.9.9/webknossos/version.py
+-rw-r--r--   0        0        0     3886 2022-03-03 15:41:54.733540 webknossos-0.9.9/setup.py
+-rw-r--r--   0        0        0     3652 2022-03-03 15:41:54.734195 webknossos-0.9.9/PKG-INFO
```

### Comparing `webknossos-0.9.8/LICENSE` & `webknossos-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/README.md` & `webknossos-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/pyproject.toml` & `webknossos-0.9.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 [tool.poetry]
 name = "webknossos"
-version = "0.9.8"  # filled by dunamai
+version = "0.9.9"  # filled by dunamai
 description = "Python package to work with webKnossos datasets and annotations"
 authors = ["scalable minds <hello@scalableminds.com>"]
 readme = "README.md"
 license = "AGPL-3.0"
 repository = "https://github.com/scalableminds/webknossos-libs"
 homepage = "https://docs.webknossos.org"
 include = ["webknossos/version.py"]
 
 [tool.poetry.dependencies]
 python = "^3.7,>=3.7.1"
 attrs = "^21.1.0"
 boltons = "~21.0.0"
 cattrs = "1.7.1"
-cluster_tools = "0.9.8"
+cluster_tools = "0.9.9"
 httpx = ">=0.15.4,<0.19.0"
 loxun = "^2.0"
 networkx = "^2.6.2"
 numpy = "^1.15.0"  # see https://numpy.org/neps/nep-0029-deprecation_policy.html#support-table
 psutil = "^5.6.7"
 python-dateutil = "^2.8.0"
 python-dotenv = "^0.19.0"
 rich = "^10.9.0"
 scikit-image = "^0.18.3"
 scipy = "^1.4.0"
 typing-extensions = "^3.7"
 wkw = "1.1.11"
+zipp = "^3.5.0"
 
 [tool.poetry.dev-dependencies]
 # autoflake
 black = "21.7b0"
 hypothesis = "^6.35.0"
 icecream = "^2.1.1"
 inducoapi = "2.0.0"
 isort = "^5.9.3"
 mypy = "0.910"
 openapi-python-client = "0.10.3"
-pandas = "^1.3.4"
-pooch = "^1.5.2"
 pylint = "^2.10.2"
 pytest = "^6.2.4"
 pytest-recording = "^0.12.0"
-tabulate = "^0.8.9"
 types-python-dateutil = "^0.1.6"
+# packages for examples:
 fastremap = "^1.12.2"
+pandas = "^1.3.4"
+pooch = "^1.5.2"
+tabulate = "^0.8.9"
 
 [tool.black]
 target_version = ['py37', 'py38']
 exclude = '''
 (
   /(
     | \.git
```

### Comparing `webknossos-0.9.8/webknossos/__init__.py` & `webknossos-0.9.9/webknossos/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 """
 This package package provides methods to modify or interact with webKnossos resources.
 
 The core classes and can be created and saved as shown:
 
-|                                                                    | Create ✨                                                            | Open/Load 📂                                                                  | Save 💾                                                                       | Download 📥                                                                                       | Upload 📤                                                                |
-|--------------------------------------------------------------------|----------------------------------------------------------------------|-------------------------------------------------------------------------------|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------|
-| **[Dataset](webknossos/dataset/dataset.html#Dataset)**             | [`Dataset(​…)`](webknossos/dataset/dataset.html#Dataset.__init__)     | [`Dataset.​open(…)`](webknossos/dataset/dataset.html#Dataset.open)             | *N/A*[^ds-save]                                                               | [`Dataset.​download(…)`](webknossos/dataset/dataset.html#Dataset.download)                         | [`dataset_obj.​upload(…)`](webknossos/dataset/dataset.html#Dataset.upload) |
-| **[Annotation](webknossos/annotation/annotation.html#Annotation)** | *N/A yet*                                                            | [`Annotation.​load(…)`](webknossos/annotation/annotation.html#Annotation.load) | [`annotation_obj.save(…)`](webknossos/annotation/annotation.html#Annotation.save) | [`Annotation.​download(…)`](webknossos/annotation/annotation.html#Annotation.download)[^anno-down] | *N/A yet*                                                                 |
-| **[Skeleton](webknossos/skeleton/skeleton.html#Skeleton)**         | [`Skeleton(​…)`](webknossos/skeleton/skeleton.html#Skeleton.__init__) | [`Skeleton.​load(…)`](webknossos/skeleton/skeleton.html#Skeleton.load)         | [`skeleton_obj.​save(…)`](webknossos/skeleton/skeleton.html#Skeleton.save)     | *only in an annotation*                                                                           | *only in an annotation*                                                   |
+|                  | Create ✨                                                                    | Open/Load 📂                                                                  | Save 💾                                                                       | Download 📥                                                                                       | Upload 📤                                                                         |
+|------------------|------------------------------------------------------------------------------|-------------------------------------------------------------------------------|-------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------|
+| **`Dataset`**    | [`Dataset(​…)`](webknossos/dataset/dataset.html#Dataset.__init__)             | [`Dataset.​open(…)`](webknossos/dataset/dataset.html#Dataset.open)             | *N/A*[^ds-save]                                                               | [`Dataset.​download(…)`](webknossos/dataset/dataset.html#Dataset.download)                         | [`dataset.​upload(…)`](webknossos/dataset/dataset.html#Dataset.upload)              |
+| **`Annotation`** | [`Annotation(​…)`](webknossos/annotation/annotation.html#Annotation.__init__) | [`Annotation.​load(…)`](webknossos/annotation/annotation.html#Annotation.load) | [`annotation.save(…)`](webknossos/annotation/annotation.html#Annotation.save) | [`Annotation.​download(…)`](webknossos/annotation/annotation.html#Annotation.download)[^anno-down] | [`annotation.​upload(…)`](webknossos/annotation/annotation.html#Annotation.upload)  |
+| **`Skeleton`**   | [`Skeleton(​…)`](webknossos/skeleton/skeleton.html#Skeleton.__init__)         | [`Skeleton.​load(…)`](webknossos/skeleton/skeleton.html#Skeleton.load)         | [`skeleton.​save(…)`](webknossos/skeleton/skeleton.html#Skeleton.save)         | *only in an annotation*                                                                           | *only in an annotation*                                                            |
 
 [^ds-save]: Since the state of a dataset is continously persisted it cannot be saved.
-[^anno-down]: Downloaded annotations are not persisted on disk so far.
+[^anno-down]: Downloaded annotations are not persisted on disk automatically.
 
-Additionally, we provide the geometrical primitives
-[Vec3Int](webknossos/geometry/vec3_int.html#Vec3Int),
-[BoundingBox](webknossos/geometry/bounding_box.html#BoundingBox) and
-[Mag](webknossos/geometry/mag.html#Mag).
+Additionally, we provide the geometrical primitives `Vec3Int`, `BoundingBox` and `Mag`.
 
-webKnossos user information can be retrieved via the [`User`](webknossos/client/user.html#User) class.
+The `User`, `Project` and `Task` classes provide webKnossos server interactions for administration purposes.
+Server interactions may require [authentication](webknossos/client/context.html) e.g. via `webknossos_context`.
 """
 
 # The table above contains zero-width spaces in the code examples after each dot to enforce correct line-breaks.
 
 from webknossos.administration import *
 from webknossos.annotation import *
 from webknossos.client import *
```

### Comparing `webknossos-0.9.8/webknossos/administration/project.py` & `webknossos-0.9.9/webknossos/administration/project.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/administration/task.py` & `webknossos-0.9.9/webknossos/administration/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     project_id: str
     dataset_name: str
     status: TaskStatus
 
     @classmethod
     def get_by_id(cls, task_id: str) -> "Task":
         """Returns the task specified by the passed id (if your token authorizes you to see it)"""
-        client = _get_generated_client()
+        client = _get_generated_client(enforce_auth=True)
         response = task_info.sync(id=task_id, client=client)
         assert (
             response is not None
         ), f"Requesting task infos from {client.base_url} failed."
         return cls._from_generated_response(response)
 
     @classmethod
@@ -65,15 +65,15 @@
     ) -> List["Task"]:
         """Submits tasks in webKnossos based on existing annotations, and returns the Task objects"""
 
         assert (
             len(base_annotations) > 0
         ), "Must supply at least one base annotation to create tasks"
 
-        client = _get_generated_client()
+        client = _get_generated_client(enforce_auth=True)
         url = f"{client.base_url}/api/tasks/createFromFiles"
         task_parameters = {
             "taskTypeId": task_type_id,
             "neededExperience": {
                 "domain": needed_experience_domain,
                 "value": needed_experience_value,
             },
@@ -82,28 +82,29 @@
             "scriptId": script_id,
             "boundingBox": bounding_box.to_wkw_dict()
             if bounding_box is not None
             else None,
         }
         form_data = {"formJSON": json.dumps(task_parameters)}
         files: Mapping[str, Tuple[str, Union[bytes, BinaryIO]]] = {
-            f"{a.name}.zip": (f"{a.name}.zip", a.binary()) for a in base_annotations
+            f"{a.name}.zip": (f"{a.name}.zip", a._binary_zip())
+            for a in base_annotations
         }
 
         response = httpx.post(
             url=url,
             headers=client.get_headers(),
             cookies=client.get_cookies(),
             timeout=client.get_timeout(),
             data=form_data,
             files=files,
         )
         assert (
             response.status_code == 200
-        ), f"Failed to create tasks from files: {response.status_code}: {response.content.decode('utf-8')}"
+        ), f"Failed to create tasks from files: {response.status_code}: {response.text}"
 
         return cls._handle_task_creation_response(response)
 
     @classmethod
     def create(
         cls,
         task_type_id: str,
@@ -115,15 +116,15 @@
         starting_rotation: Optional[Vec3Int] = Vec3Int(0, 0, 0),
         instances: int = 1,
         script_id: Optional[str] = None,
         bounding_box: Optional[BoundingBox] = None,
     ) -> List["Task"]:
         """Submits tasks in webKnossos based on a dataset, starting position + rotation, and returns the Task objects"""
 
-        client = _get_generated_client()
+        client = _get_generated_client(enforce_auth=True)
         url = f"{client.base_url}/api/tasks"
         task_parameters = {
             "taskTypeId": task_type_id,
             "neededExperience": {
                 "domain": needed_experience_domain,
                 "value": needed_experience_value,
             },
@@ -143,15 +144,15 @@
             headers=client.get_headers(),
             cookies=client.get_cookies(),
             timeout=client.get_timeout(),
             json=[task_parameters],
         )
         assert (
             response.status_code == 200
-        ), f"Failed to create tasks: {response.status_code}: {response.content.decode('utf-8')}"
+        ), f"Failed to create tasks: {response.status_code}: {response.text}"
 
         return cls._handle_task_creation_response(response)
 
     @classmethod
     def _from_dict(cls, response_dict: Dict) -> "Task":
         from webknossos.client._generated.models.task_info_response_200 import (
             TaskInfoResponse200,
@@ -173,28 +174,28 @@
             TaskStatus(
                 response.status.open_, response.status.active, response.status.finished
             ),
         )
 
     def get_annotation_infos(self) -> List[AnnotationInfo]:
         """Returns AnnotationInfo objects describing all task instances that have been started by annotators for this task"""
-        client = _get_generated_client()
+        client = _get_generated_client(enforce_auth=True)
         response = annotation_infos_by_task_id.sync(id=self.task_id, client=client)
         assert (
             response is not None
         ), f"Requesting annotation infos for task from {client.base_url} failed."
         return [AnnotationInfo._from_generated_response(a) for a in response]
 
     def get_project(self) -> Project:
         """Returns the project this task belongs to"""
         return Project.get_by_id(self.project_id)
 
     @classmethod
     def _handle_task_creation_response(cls, response: httpx.Response) -> List["Task"]:
-        result = json.loads(response.content)
+        result = response.json()
         if "warnings" in result:
             warnings = result["warnings"]
             if len(warnings) > 0:
                 logger.warning(
                     f"There were {len(warnings)} warnings during task creation:"
                 )
             for warning in warnings:
```

### Comparing `webknossos-0.9.8/webknossos/administration/user.py` & `webknossos-0.9.9/webknossos/administration/user.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/annotation/annotation_info.py` & `webknossos-0.9.9/webknossos/annotation/annotation_info.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     name: str
     description: str
     type: AnnotationType
     state: AnnotationState
 
     def download_annotation(self) -> Annotation:
         """Downloads and returns the annotation that is discribed by this AnnotationInfo object"""
-        from webknossos.client._download_annotation import download_annotation
-
-        return download_annotation(self.type, self.id)
+        return Annotation.download(self.id, annotation_type=self.type)
 
     @classmethod
     def _from_generated_response(
         cls,
         response: Union[
             "AnnotationInfoResponse200", "AnnotationInfosByTaskIdResponse200Item"
         ],
```

### Comparing `webknossos-0.9.8/webknossos/client/_download_dataset.py` & `webknossos-0.9.9/webknossos/client/_download_dataset.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_cancel_upload.py` & `webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_cancel_upload.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_download.py` & `webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_download.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_finish_upload.py` & `webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_finish_upload.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_reserve_upload.py` & `webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_reserve_upload.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/datastore/dataset_upload_chunk.py` & `webknossos-0.9.9/webknossos/client/_generated/api/datastore/dataset_upload_chunk.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/add_annotation_layer.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/add_annotation_layer.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_download.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_download.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_info.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_info.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_infos_by_task_id.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_infos_by_task_id.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/annotation_upload.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/annotation_upload.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/build_info.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/build_info.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/create_project.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/create_project.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/current_user_info.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/current_user_info.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/dataset_info.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/dataset_info.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/datastore_list.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/datastore_list.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/generate_token_for_data_store.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/generate_token_for_data_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/health.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/health.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/new_dataset_name_is_valid.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/new_dataset_name_is_valid.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/project_info_by_id.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/project_info_by_id.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/project_info_by_name.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/project_info_by_name.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/task_create_from_files.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/task_create_from_files.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/task_info.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/task_info.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/task_infos_by_project_id.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/task_infos_by_project_id.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/user_info_by_id.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/user_info_by_id.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/user_list.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/user_list.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/api/default/user_logged_time.py` & `webknossos-0.9.9/webknossos/client/_generated/api/default/user_logged_time.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/client.py` & `webknossos-0.9.9/webknossos/client/_generated/client.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/__init__.py` & `webknossos-0.9.9/webknossos/client/_generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_annotation_layer_parameters.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_annotation_layer_parameters.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_any_content.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_any_content.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_cancel_upload_information.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_cancel_upload_information.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_js_value.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_js_value.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_multipart_form_data_temporary_file.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_multipart_form_data_temporary_file.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_reserve_upload_information.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_reserve_upload_information.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/action_upload_information.py` & `webknossos-0.9.9/webknossos/client/_generated/models/action_upload_information.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_annotation_layers_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_annotation_layers_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_data_store.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_data_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_settings.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_settings.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_settings_resolution_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_settings_resolution_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_stats.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_stats.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_tracing_store.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_tracing_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_user.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_user.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_info_response_200_user_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_info_response_200_user_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_annotation_layers_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_annotation_layers_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_data_store.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_data_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings_resolution_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_settings_resolution_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_stats.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_stats.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_needed_experience.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_needed_experience.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_status.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_status.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings_resolution_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_task_type_settings_resolution_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_tracing_store.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_tracing_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/annotation_infos_by_task_id_response_200_item_user_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200_webknossos.py` & `webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200_webknossos.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/build_info_response_200_webknossos_wrap.py` & `webknossos-0.9.9/webknossos/client/_generated/models/build_info_response_200_webknossos_wrap.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/create_project_json_body.py` & `webknossos-0.9.9/webknossos/client/_generated/models/create_project_json_body.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_experiences.py` & `webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_experiences.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_novel_user_experience_infos.py` & `webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_novel_user_experience_infos.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/current_user_info_response_200_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/current_user_info_response_200_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_cancel_upload_json_body.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_cancel_upload_json_body.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_finish_upload_json_body.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_finish_upload_json_body.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item_bounding_box.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_data_layers_item_bounding_box.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_source_id.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_source_id.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_info_response_200_data_store.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_info_response_200_data_store.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/dataset_reserve_upload_json_body.py` & `webknossos-0.9.9/webknossos/client/_generated/models/dataset_reserve_upload_json_body.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/datastore_list_response_200_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/datastore_list_response_200_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/generate_token_for_data_store_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/generate_token_for_data_store_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200_owner.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200_owner.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_id_response_200_owner_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_id_response_200_owner_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200_owner.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200_owner.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/project_info_by_name_response_200_owner_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/project_info_by_name_response_200_owner_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_create_from_files_json_body.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_create_from_files_json_body.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_needed_experience.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_needed_experience.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_status.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_status.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type_settings.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type_settings.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_info_response_200_type_settings_resolution_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_info_response_200_type_settings_resolution_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_needed_experience.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_needed_experience.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_status.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_status.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings_resolution_restrictions.py` & `webknossos-0.9.9/webknossos/client/_generated/models/task_infos_by_project_id_response_200_item_type_settings_resolution_restrictions.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_experiences.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_experiences.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_novel_user_experience_infos.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_novel_user_experience_infos.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_info_by_id_response_200_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_info_by_id_response_200_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_experiences.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_experiences.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_novel_user_experience_infos.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_novel_user_experience_infos.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_list_response_200_item_teams_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_list_response_200_item_teams_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item_payment_interval.py` & `webknossos-0.9.9/webknossos/client/_generated/models/user_logged_time_response_200_logged_time_item_payment_interval.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_generated/types.py` & `webknossos-0.9.9/webknossos/client/_generated/types.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_resumable/chunk.py` & `webknossos-0.9.9/webknossos/client/_resumable/chunk.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_resumable/core.py` & `webknossos-0.9.9/webknossos/client/_resumable/core.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_resumable/file.py` & `webknossos-0.9.9/webknossos/client/_resumable/file.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_resumable/util.py` & `webknossos-0.9.9/webknossos/client/_resumable/util.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/_upload_dataset.py` & `webknossos-0.9.9/webknossos/client/_upload_dataset.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/context.py` & `webknossos-0.9.9/webknossos/client/context.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/client/download_dataset.py` & `webknossos-0.9.9/webknossos/client/download_dataset.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/__init__.py` & `webknossos-0.9.9/webknossos/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/_utils/buffered_slice_reader.py` & `webknossos-0.9.9/webknossos/dataset/_utils/buffered_slice_reader.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/_utils/buffered_slice_writer.py` & `webknossos-0.9.9/webknossos/dataset/_utils/buffered_slice_writer.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/_utils/infer_bounding_box_existing_files.py` & `webknossos-0.9.9/webknossos/dataset/_utils/infer_bounding_box_existing_files.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/compress_utils.py` & `webknossos-0.9.9/webknossos/dataset/compress_utils.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/dataset.py` & `webknossos-0.9.9/webknossos/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/downsampling_utils.py` & `webknossos-0.9.9/webknossos/dataset/downsampling_utils.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/layer.py` & `webknossos-0.9.9/webknossos/dataset/layer.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/mag_view.py` & `webknossos-0.9.9/webknossos/dataset/mag_view.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import shutil
 import warnings
 from argparse import Namespace
 from pathlib import Path
-from typing import TYPE_CHECKING, Generator, Optional, Union
+from typing import TYPE_CHECKING, Iterator, Optional, Union
 from uuid import uuid4
 
 import numpy as np
 from wkw import wkw
 
 from webknossos.geometry import BoundingBox, Mag, Vec3Int, Vec3IntLike
 from webknossos.utils import get_executor_for_args, wait_and_ensure_success
@@ -144,14 +144,17 @@
 
         mag1_bbox = self._get_mag1_bbox(
             abs_current_mag_offset=offset,
             rel_mag1_offset=relative_offset,
             abs_mag1_offset=absolute_offset,
             current_mag_size=Vec3Int(data.shape[-3:]),
         )
+
+        # Only update the layer's bbox if we are actually larger
+        # than the mag-aligned, rounded up bbox (self.bounding_box):
         if not self.bounding_box.contains_bbox(mag1_bbox):
             self.layer.bounding_box = self.layer.bounding_box.extended_by(mag1_bbox)
 
         super().write(data, absolute_offset=mag1_bbox.topleft)
 
     def read(
         self,
@@ -220,29 +223,41 @@
             relative_offset=relative_offset,
             absolute_offset=absolute_offset,
             read_only=read_only,
         )
 
     def get_bounding_boxes_on_disk(
         self,
-    ) -> Generator[BoundingBox, None, None]:
+    ) -> Iterator[BoundingBox]:
         """
         Returns a Mag(1) bounding box for each file on disk.
 
         This differs from the bounding box in the properties, which is an "overall" bounding box,
         abstracting from the files on disk.
         """
         cube_size = self._get_file_dimensions()
         for filename in self._wkw_dataset.list_files():
             file_path = Path(os.path.splitext(filename)[0]).relative_to(self._path)
             cube_index = _extract_file_index(file_path)
             cube_offset = cube_index * cube_size
 
             yield BoundingBox(cube_offset, cube_size).from_mag_to_mag1(self._mag)
 
+    def get_views_on_disk(
+        self,
+        read_only: Optional[bool] = None,
+    ) -> Iterator[View]:
+        """
+        Yields a view for each file on disk, which can be used for efficient parallelization.
+        """
+        for bbox in self.get_bounding_boxes_on_disk():
+            yield self.get_view(
+                absolute_offset=bbox.topleft, size=bbox.size, read_only=read_only
+            )
+
     def compress(
         self,
         target_path: Optional[Union[str, Path]] = None,
         args: Optional[Namespace] = None,
     ) -> None:
         """
         Compresses the files on disk. This has consequences for writing data (see `write`).
```

### Comparing `webknossos-0.9.8/webknossos/dataset/properties.py` & `webknossos-0.9.9/webknossos/dataset/properties.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/upsampling_utils.py` & `webknossos-0.9.9/webknossos/dataset/upsampling_utils.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/dataset/view.py` & `webknossos-0.9.9/webknossos/dataset/view.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/geometry/bounding_box.py` & `webknossos-0.9.9/webknossos/geometry/bounding_box.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/geometry/mag.py` & `webknossos-0.9.9/webknossos/geometry/mag.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/geometry/vec3_int.py` & `webknossos-0.9.9/webknossos/geometry/vec3_int.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/webknossos/skeleton/graph.py` & `webknossos-0.9.9/webknossos/skeleton/graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         self.group = group
         self.color = color
 
         # read-only member, exposed via properties
         if enforced_id is not None:
             self._id = enforced_id
         else:
-            self._id = skeleton.element_id_generator.__next__()
+            self._id = skeleton._element_id_generator.__next__()
 
         # only used internally
         self._skeleton = skeleton
 
     def __to_tuple_for_comparison(self) -> Tuple:
         return (
             self.name,
```

### Comparing `webknossos-0.9.8/webknossos/skeleton/group.py` & `webknossos-0.9.9/webknossos/skeleton/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import TYPE_CHECKING, Generator, Iterator, Optional, Set, Tuple, Union, cast
 
 import attr
 from boltons.strutils import unit_len
 
-import webknossos.skeleton.nml as wknml
+import webknossos._nml as wknml
 
 from .graph import Graph
 
 if TYPE_CHECKING:
     from webknossos.skeleton import Node, Skeleton
 
 
@@ -28,18 +28,19 @@
     _skeleton: "Skeleton" = attr.ib(eq=False, repr=False)
     _enforced_id: Optional[int] = attr.ib(None, eq=False, repr=False)
 
     def __attrs_post_init__(self) -> None:
         if self._enforced_id is not None:
             self._id = self._enforced_id
         else:
-            self._id = self._skeleton.element_id_generator.__next__()
+            self._id = self._skeleton._element_id_generator.__next__()
 
     @property
     def id(self) -> int:
+        """Read-only property."""
         return self._id
 
     def add_graph(
         self,
         name: str,
         color: Optional[Union[Vector4, Vector3]] = None,
         _enforced_id: Optional[int] = None,
```

### Comparing `webknossos-0.9.8/webknossos/skeleton/node.py` & `webknossos-0.9.9/webknossos/skeleton/node.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     branchpoint_time: Optional[int] = None
     _enforced_id: Optional[int] = attr.ib(None, eq=False, repr=False)
 
     def __attrs_post_init__(self) -> None:
         if self._enforced_id is not None:
             self._id = self._enforced_id
         else:
-            self._id = self._skeleton.element_id_generator.__next__()
+            self._id = self._skeleton._element_id_generator.__next__()
 
     @property
     def id(self) -> int:
         return self._id
 
     def __hash__(self) -> int:
         return self._id
```

### Comparing `webknossos-0.9.8/webknossos/utils.py` & `webknossos-0.9.9/webknossos/utils.py`

 * *Files identical despite different names*

### Comparing `webknossos-0.9.8/setup.py` & `webknossos-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['webknossos',
+ 'webknossos._nml',
  'webknossos.administration',
  'webknossos.annotation',
  'webknossos.client',
  'webknossos.client._generated',
  'webknossos.client._generated.api',
  'webknossos.client._generated.api.datastore',
  'webknossos.client._generated.api.default',
  'webknossos.client._generated.models',
  'webknossos.client._resumable',
  'webknossos.dataset',
  'webknossos.dataset._utils',
  'webknossos.geometry',
- 'webknossos.skeleton',
- 'webknossos.skeleton.nml']
+ 'webknossos.skeleton']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=21.1.0,<22.0.0',
  'boltons>=21.0.0,<21.1.0',
  'cattrs==1.7.1',
- 'cluster_tools==0.9.8',
+ 'cluster_tools==0.9.9',
  'httpx>=0.15.4,<0.19.0',
  'loxun>=2.0,<3.0',
  'networkx>=2.6.2,<3.0.0',
  'numpy>=1.15.0,<2.0.0',
  'psutil>=5.6.7,<6.0.0',
  'python-dateutil>=2.8.0,<3.0.0',
  'python-dotenv>=0.19.0,<0.20.0',
  'rich>=10.9.0,<11.0.0',
  'scikit-image>=0.18.3,<0.19.0',
  'scipy>=1.4.0,<2.0.0',
  'typing-extensions>=3.7,<4.0',
- 'wkw==1.1.11']
+ 'wkw==1.1.11',
+ 'zipp>=3.5.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'webknossos',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Python package to work with webKnossos datasets and annotations',
     'long_description': '# webKnossos Python Library\n[![PyPI version](https://img.shields.io/pypi/v/webknossos)](https://pypi.python.org/pypi/webknossos)\n[![Supported Python Versions](https://img.shields.io/pypi/pyversions/webknossos.svg)](https://pypi.python.org/pypi/webknossos)\n[![Build Status](https://img.shields.io/github/workflow/status/scalableminds/webknossos-libs/CI/master)](https://github.com/scalableminds/webknossos-libs/actions?query=workflow%3A%22CI%22)\n[![Documentation](https://img.shields.io/badge/docs-passing-brightgreen.svg)](https://docs.webknossos.org/webknossos-py)\n[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\nPython API for working with [webKnossos](https://webknossos.org) datasets, annotations, and for webKnossos server interaction.\n\nFor the webKnossos server, please refer to https://github.com/scalableminds/webknossos.\n\n## Features\n\n- easy-to-use dataset API for reading/writing/editing raw 2D/3D image data and volume annotations/segmentation in webKnossos wrap (*.wkw) format\n    - add/remove layers\n    - update metadata (`datasource-properties.json`) \n    - up/downsample layers\n    - compress layers \n    - add/remove magnifications\n    - execute any of the `wkCuber` operations from your code\n- manipulation of webKnossos skeleton annotations (*.nml) as Python objects\n    - access to nodes, comments, trees, bounding boxes, metadata, etc.\n    - create new skeleton annotation from Graph structures or Python objects\n- interaction, connection & scripting with your webKnossos instance over the REST API\n    - up- & downloading annotations and datasets\n\nPlease refer to [the documentation for further instructions](https://docs.webknossos.org/webknossos-py).\n\n## Installation\nThe `webknossos` package requires at least Python 3.7+.\n\nYou can install it from [pypi](https://pypi.org/project/webknossos/), e.g. via pip:\n\n```bash\npip install webknossos\n```\n\n## Examples\nSee the [examples folder](examples) or the [the documentation](https://docs.webknossos.org/webknossos-py).\n\n## Contributions & Development\nPlease see the [respective documentation page](https://docs.webknossos.org/webknossos-py/development.html).\n\n## License\n[AGPLv3](https://www.gnu.org/licenses/agpl-3.0.html)\nCopyright [scalable minds](https://scalableminds.com)\n',
     'author': 'scalable minds',
     'author_email': 'hello@scalableminds.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://docs.webknossos.org',
```

### Comparing `webknossos-0.9.8/PKG-INFO` & `webknossos-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: webknossos
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python package to work with webKnossos datasets and annotations
 Home-page: https://docs.webknossos.org
 License: AGPL-3.0
 Author: scalable minds
 Author-email: hello@scalableminds.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: attrs (>=21.1.0,<22.0.0)
 Requires-Dist: boltons (>=21.0.0,<21.1.0)
 Requires-Dist: cattrs (==1.7.1)
-Requires-Dist: cluster_tools (==0.9.8)
+Requires-Dist: cluster_tools (==0.9.9)
 Requires-Dist: httpx (>=0.15.4,<0.19.0)
 Requires-Dist: loxun (>=2.0,<3.0)
 Requires-Dist: networkx (>=2.6.2,<3.0.0)
 Requires-Dist: numpy (>=1.15.0,<2.0.0)
 Requires-Dist: psutil (>=5.6.7,<6.0.0)
 Requires-Dist: python-dateutil (>=2.8.0,<3.0.0)
 Requires-Dist: python-dotenv (>=0.19.0,<0.20.0)
 Requires-Dist: rich (>=10.9.0,<11.0.0)
 Requires-Dist: scikit-image (>=0.18.3,<0.19.0)
 Requires-Dist: scipy (>=1.4.0,<2.0.0)
 Requires-Dist: typing-extensions (>=3.7,<4.0)
 Requires-Dist: wkw (==1.1.11)
+Requires-Dist: zipp (>=3.5.0,<4.0.0)
 Project-URL: Repository, https://github.com/scalableminds/webknossos-libs
 Description-Content-Type: text/markdown
 
 # webKnossos Python Library
 [![PyPI version](https://img.shields.io/pypi/v/webknossos)](https://pypi.python.org/pypi/webknossos)
 [![Supported Python Versions](https://img.shields.io/pypi/pyversions/webknossos.svg)](https://pypi.python.org/pypi/webknossos)
 [![Build Status](https://img.shields.io/github/workflow/status/scalableminds/webknossos-libs/CI/master)](https://github.com/scalableminds/webknossos-libs/actions?query=workflow%3A%22CI%22)
```

