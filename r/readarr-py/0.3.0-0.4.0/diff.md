# Comparing `tmp/readarr-py-0.3.0.tar.gz` & `tmp/readarr-py-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "readarr-py-0.3.0.tar", last modified: Mon May 29 06:41:07 2023, max compression
+gzip compressed data, was "readarr-py-0.4.0.tar", last modified: Mon Jul 17 13:06:13 2023, max compression
```

## Comparing `readarr-py-0.3.0.tar` & `readarr-py-0.4.0.tar`

### file list

```diff
@@ -1,249 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-05-29 06:40:53.000000 readarr-py-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    40629 2023-05-29 06:41:07.296209 readarr-py-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    40153 2023-05-29 06:40:53.000000 readarr-py-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 06:40:53.000000 readarr-py-0.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.244208 readarr-py-0.3.0/readarr/
--rw-r--r--   0 runner    (1001) docker     (123)    14646 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.272209 readarr-py-0.3.0/readarr/api/
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/api_info_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/authentication_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29810 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/author_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/backup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/blocklist_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    42877 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_editor_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    37683 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/book_lookup_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/bookshelf_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13520 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/calendar_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/calendar_feed_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23476 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/command_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30451 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/custom_filter_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35519 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/custom_format_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12620 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/cutoff_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36259 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/delay_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18993 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/development_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/disk_space_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53859 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/download_client_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19204 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/download_client_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/edition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/file_system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11942 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/health_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/history_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18587 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/host_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53187 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/import_list_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    31188 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/import_list_exclusion_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52562 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/indexer_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/indexer_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/initialize_js_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12000 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/language_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/localization_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/log_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/manual_import_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/media_cover_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19262 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/media_management_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    52730 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30739 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19320 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/metadata_provider_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/missing_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29415 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/naming_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    53402 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/notification_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/parse_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/ping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    25233 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30643 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/quality_profile_schema_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_action_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    27554 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/queue_status_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30643 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_profile_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12846 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/release_push_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30996 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/remote_path_mapping_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/rename_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/retag_book_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    30259 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/root_folder_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/series_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/static_resource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/system_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29522 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/tag_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12059 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/tag_details_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    12010 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/task_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18471 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/ui_config_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/update_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api/update_log_file_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    29647 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/api_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/readarr/models/
--rw-r--r--   0 runner    (1001) docker     (123)    10175 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/add_author_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/add_book_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/allow_fingerprinting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/api_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/apply_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/authentication_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_metadata_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_status_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/author_title_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/backup_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/backup_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/blocklist_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_add_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_editor_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/book_statistics_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/books_monitored_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/bookshelf_author_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/bookshelf_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/certificate_validation_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_priority.py
--rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_status.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/command_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_filter_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/custom_format_specification_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/database_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/delay_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/development_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/disk_space_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_client_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_client_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/download_protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/edition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/entity_history_event_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/field.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/file_date_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/health_check_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/health_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/history_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/history_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/host_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/i_custom_format_specification.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_exclusion_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_monitor_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/import_list_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/indexer_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/indexer_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/iso_country.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/language_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/log_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/manual_import_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/manual_import_update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_cover_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_info_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_info_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/media_management_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_provider_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/metadata_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/monitoring_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/naming_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/new_item_monitor_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/notification_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/paging_resource_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parse_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parsed_book_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/parsed_track_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/profile_format_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/profile_format_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/proper_download_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/provider_message.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/provider_message_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/proxy_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_definition_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_quality_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_quality_item_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/quality_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_bulk_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     7951 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_resource_paging_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/queue_status_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ratings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rejection.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rejection_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/release_profile_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/release_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/remote_path_mapping_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rename_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/rescan_after_refresh_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/retag_book_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/revision.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/root_folder_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/runtime_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/select_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_book_link_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_list_lazy_loaded.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/series_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/sort_direction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/system_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_details_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_difference.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tag_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/task_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_state.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/tracked_download_status_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/ui_config_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_changes.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/update_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/write_audio_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/models/write_book_tags_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-05-29 06:40:53.000000 readarr-py-0.3.0/readarr/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 06:41:07.296209 readarr-py-0.3.0/readarr_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40629 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8436 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 06:41:07.000000 readarr-py-0.3.0/readarr_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 06:41:07.296209 readarr-py-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-29 06:40:53.000000 readarr-py-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.640531 readarr-py-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-17 13:05:58.000000 readarr-py-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-17 13:06:13.640531 readarr-py-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    40399 2023-07-17 13:05:58.000000 readarr-py-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-17 13:05:58.000000 readarr-py-0.4.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.588531 readarr-py-0.4.0/readarr/
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.604531 readarr-py-0.4.0/readarr/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/api_info_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/authentication_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31205 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6281 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/author_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22487 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/backup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17844 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/blocklist_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43863 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_editor_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37656 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6261 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/book_lookup_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/bookshelf_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/calendar_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/calendar_feed_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23449 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/command_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30424 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/custom_filter_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35492 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/custom_format_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/cutoff_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/delay_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18966 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/development_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6322 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/disk_space_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67048 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/download_client_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19177 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/download_client_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6767 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/edition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18408 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/file_system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/health_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27532 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/history_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18560 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/host_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66152 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/import_list_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31161 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/import_list_exclusion_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65318 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/indexer_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18734 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/indexer_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/initialize_js_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/language_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6166 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/localization_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/log_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11832 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/manual_import_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12793 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/media_cover_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19235 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/media_management_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53261 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30712 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19293 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/metadata_provider_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12612 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/missing_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29962 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/naming_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53933 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/notification_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/parse_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/ping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25206 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/quality_profile_schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12293 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_action_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8092 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/queue_status_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30616 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_profile_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/release_push_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30969 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/remote_path_mapping_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/rename_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/retag_book_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30232 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/root_folder_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6686 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/series_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21836 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/static_resource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26850 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/system_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29495 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/tag_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12032 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/tag_details_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11983 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/task_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/ui_config_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/update_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11964 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api/update_log_file_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29647 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.636531 readarr-py-0.4.0/readarr/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    10404 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/add_author_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/add_book_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/allow_fingerprinting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/api_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/apply_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/authentication_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_metadata_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_status_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/author_title_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/backup_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/backup_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/blocklist_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_add_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_editor_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/book_statistics_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/books_monitored_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/bookshelf_author_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/bookshelf_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/certificate_validation_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5324 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/command_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_filter_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4464 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/custom_format_specification_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/database_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/delay_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/development_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/disk_space_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_client_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/download_protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6786 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/edition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/entity_history_event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/file_date_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/health_check_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/health_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5256 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/history_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/history_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/host_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/i_custom_format_specification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_exclusion_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_monitor_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/import_list_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5962 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/indexer_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/iso_country.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/language_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/log_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/manual_import_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/manual_import_update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_cover_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_info_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_info_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/media_management_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3374 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3430 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_provider_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/metadata_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/monitoring_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/naming_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/new_item_monitor_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/notification_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/paging_resource_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parse_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parsed_book_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8825 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/parsed_track_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/profile_format_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/profile_format_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/proper_download_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/provider_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/provider_message_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/proxy_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3132 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_definition_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_quality_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_quality_item_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/quality_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_bulk_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8076 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_resource_paging_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2702 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/queue_status_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ratings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rejection_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/release_profile_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8900 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/release_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/remote_path_mapping_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rename_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/rescan_after_refresh_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/retag_book_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/root_folder_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/runtime_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/select_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3899 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_book_link_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_list_lazy_loaded.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/series_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/sort_direction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7074 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/system_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_details_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_difference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tag_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/task_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/tracked_download_status_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/ui_config_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_changes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/update_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/write_audio_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/models/write_book_tags_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-07-17 13:05:58.000000 readarr-py-0.4.0/readarr/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 13:06:13.640531 readarr-py-0.4.0/readarr_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40875 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 13:06:13.000000 readarr-py-0.4.0/readarr_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 13:06:13.640531 readarr-py-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-07-17 13:05:58.000000 readarr-py-0.4.0/setup.py
```

### Comparing `readarr-py-0.3.0/LICENSE` & `readarr-py-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/PKG-INFO` & `readarr-py-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: readarr-py
-Version: 0.3.0
+Version: 0.4.0
 Summary: Readarr API wrapper
 Project-URL: Homepage, https://github.com/devopsarr/readarr-py
 Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -13,15 +13,15 @@
 
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -177,56 +177,61 @@
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -287,31 +292,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameBookApi* | [**list_rename**](docs/RenameBookApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagBookApi* | [**list_retag**](docs/RetagBookApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -395,14 +395,15 @@
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
@@ -411,18 +412,20 @@
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `readarr-py-0.3.0/README.md` & `readarr-py-0.4.0/readarr_py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+Metadata-Version: 2.1
+Name: readarr-py
+Version: 0.4.0
+Summary: Readarr API wrapper
+Project-URL: Homepage, https://github.com/devopsarr/readarr-py
+Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -164,56 +177,61 @@
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -274,31 +292,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameBookApi* | [**list_rename**](docs/RenameBookApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagBookApi* | [**list_retag**](docs/RetagBookApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -382,14 +395,15 @@
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
@@ -398,18 +412,20 @@
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `readarr-py-0.3.0/pyproject.toml` & `readarr-py-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # coding: utf-8
 
 [project]
 name = "readarr-py"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "requests>=2.28.1",
     "pydantic>=1.10.2",
     "aenum"
 ]
```

### Comparing `readarr-py-0.3.0/readarr/__init__.py` & `readarr-py-0.4.0/readarr/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from __future__ import absolute_import
 
 # x-release-please-start-version
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 # x-release-please-end
 
 # import apis into sdk package
 from readarr.api.api_info_api import ApiInfoApi
 from readarr.api.authentication_api import AuthenticationApi
 from readarr.api.author_api import AuthorApi
 from readarr.api.author_editor_api import AuthorEditorApi
@@ -148,14 +148,15 @@
 from readarr.models.custom_format import CustomFormat
 from readarr.models.custom_format_resource import CustomFormatResource
 from readarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from readarr.models.database_type import DatabaseType
 from readarr.models.delay_profile_resource import DelayProfileResource
 from readarr.models.development_config_resource import DevelopmentConfigResource
 from readarr.models.disk_space_resource import DiskSpaceResource
+from readarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from readarr.models.download_client_config_resource import DownloadClientConfigResource
 from readarr.models.download_client_resource import DownloadClientResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.edition import Edition
 from readarr.models.edition_lazy_loaded import EditionLazyLoaded
 from readarr.models.edition_list_lazy_loaded import EditionListLazyLoaded
 from readarr.models.edition_resource import EditionResource
@@ -164,18 +165,20 @@
 from readarr.models.file_date_type import FileDateType
 from readarr.models.health_check_result import HealthCheckResult
 from readarr.models.health_resource import HealthResource
 from readarr.models.history_resource import HistoryResource
 from readarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from readarr.models.host_config_resource import HostConfigResource
 from readarr.models.i_custom_format_specification import ICustomFormatSpecification
+from readarr.models.import_list_bulk_resource import ImportListBulkResource
 from readarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from readarr.models.import_list_monitor_type import ImportListMonitorType
 from readarr.models.import_list_resource import ImportListResource
 from readarr.models.import_list_type import ImportListType
+from readarr.models.indexer_bulk_resource import IndexerBulkResource
 from readarr.models.indexer_config_resource import IndexerConfigResource
 from readarr.models.indexer_resource import IndexerResource
 from readarr.models.iso_country import IsoCountry
 from readarr.models.language_resource import LanguageResource
 from readarr.models.links import Links
 from readarr.models.log_file_resource import LogFileResource
 from readarr.models.log_resource import LogResource
```

### Comparing `readarr-py-0.3.0/readarr/api/__init__.py` & `readarr-py-0.4.0/readarr/api/__init__.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/api_info_api.py` & `readarr-py-0.4.0/readarr/api/api_info_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/authentication_api.py` & `readarr-py-0.4.0/readarr/api/authentication_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/author_api.py` & `readarr-py-0.4.0/readarr/api/author_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from readarr.models.author_resource import AuthorResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
@@ -187,25 +187,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_author(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_author(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_author(id, async_req=True)
+        >>> thread = api.delete_author(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -214,28 +218,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_author_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_author_with_http_info(id, delete_files, add_import_list_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_author_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_author_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_author_with_http_info(id, async_req=True)
+        >>> thread = api.delete_author_with_http_info(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -255,15 +263,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_list_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -288,14 +298,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_list_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportListExclusion', _params['add_import_list_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -436,15 +450,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "AuthorResource",
         }
@@ -597,25 +611,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_author(self, id : StrictStr, author_resource : Optional[AuthorResource] = None, **kwargs) -> AuthorResource:  # noqa: E501
+    def update_author(self, id : StrictStr, move_files : Optional[StrictBool] = None, author_resource : Optional[AuthorResource] = None, **kwargs) -> AuthorResource:  # noqa: E501
         """update_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_author(id, author_resource, async_req=True)
+        >>> thread = api.update_author(id, move_files, author_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param author_resource:
         :type author_resource: AuthorResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -626,28 +642,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: AuthorResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_author_with_http_info(id, author_resource, **kwargs)  # noqa: E501
+        return self.update_author_with_http_info(id, move_files, author_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_author_with_http_info(self, id : StrictStr, author_resource : Optional[AuthorResource] = None, **kwargs):  # noqa: E501
+    def update_author_with_http_info(self, id : StrictStr, move_files : Optional[StrictBool] = None, author_resource : Optional[AuthorResource] = None, **kwargs):  # noqa: E501
         """update_author  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_author_with_http_info(id, author_resource, async_req=True)
+        >>> thread = api.update_author_with_http_info(id, move_files, author_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param move_files:
+        :type move_files: bool
         :param author_resource:
         :type author_resource: AuthorResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -670,14 +688,15 @@
         :rtype: tuple(AuthorResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'move_files',
             'author_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -703,14 +722,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('move_files') is not None:  # noqa: E501
+            _query_params.append(('moveFiles', _params['move_files']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
```

### Comparing `readarr-py-0.3.0/readarr/api/author_editor_api.py` & `readarr-py-0.4.0/readarr/api/author_editor_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/author_lookup_api.py` & `readarr-py-0.4.0/readarr/api/author_lookup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/backup_api.py` & `readarr-py-0.4.0/readarr/api/backup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/blocklist_api.py` & `readarr-py-0.4.0/readarr/api/blocklist_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/book_api.py` & `readarr-py-0.4.0/readarr/api/book_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -188,25 +188,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_book(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+    def delete_book(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs) -> None:  # noqa: E501
         """delete_book  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book(id, async_req=True)
+        >>> thread = api.delete_book(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -215,28 +219,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_book_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_book_with_http_info(id, delete_files, add_import_list_exclusion, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_book_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+    def delete_book_with_http_info(self, id : StrictInt, delete_files : Optional[StrictBool] = None, add_import_list_exclusion : Optional[StrictBool] = None, **kwargs):  # noqa: E501
         """delete_book  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_book_with_http_info(id, async_req=True)
+        >>> thread = api.delete_book_with_http_info(id, delete_files, add_import_list_exclusion, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
+        :param delete_files:
+        :type delete_files: bool
+        :param add_import_list_exclusion:
+        :type add_import_list_exclusion: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -256,15 +264,17 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'id',
+            'delete_files',
+            'add_import_list_exclusion'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -289,14 +299,18 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('delete_files') is not None:  # noqa: E501
+            _query_params.append(('deleteFiles', _params['delete_files']))
+        if _params.get('add_import_list_exclusion') is not None:  # noqa: E501
+            _query_params.append(('addImportListExclusion', _params['add_import_list_exclusion']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -437,15 +451,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/book_editor_api.py` & `readarr-py-0.4.0/readarr/api/book_editor_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/book_file_api.py` & `readarr-py-0.4.0/readarr/api/book_file_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -431,15 +431,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookFileResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/book_lookup_api.py` & `readarr-py-0.4.0/readarr/api/book_lookup_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/bookshelf_api.py` & `readarr-py-0.4.0/readarr/api/bookshelf_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/calendar_api.py` & `readarr-py-0.4.0/readarr/api/calendar_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,15 +155,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/calendar_feed_api.py` & `readarr-py-0.4.0/readarr/api/calendar_feed_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/command_api.py` & `readarr-py-0.4.0/readarr/api/command_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CommandResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/custom_filter_api.py` & `readarr-py-0.4.0/readarr/api/custom_filter_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFilterResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/custom_format_api.py` & `readarr-py-0.4.0/readarr/api/custom_format_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "CustomFormatResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/cutoff_api.py` & `readarr-py-0.4.0/readarr/api/cutoff_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/delay_profile_api.py` & `readarr-py-0.4.0/readarr/api/delay_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DelayProfileResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/development_config_api.py` & `readarr-py-0.4.0/readarr/api/development_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DevelopmentConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/disk_space_api.py` & `readarr-py-0.4.0/readarr/api/disk_space_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/download_client_api.py` & `readarr-py-0.4.0/readarr/api/notification_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,81 +13,85 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
-from readarr.models.download_client_resource import DownloadClientResource
+from readarr.models.notification_resource import NotificationResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class DownloadClientApi(object):
+class NotificationApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """create_download_client  # noqa: E501
+    def create_notification(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client(download_client_resource, async_req=True)
+        >>> thread = api.create_notification(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_download_client_with_http_info(download_client_resource, **kwargs)  # noqa: E501
+        return self.create_notification_with_http_info(force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_download_client_with_http_info(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """create_download_client  # noqa: E501
+    def create_notification_with_http_info(self, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_with_http_info(download_client_resource, async_req=True)
+        >>> thread = api.create_notification_with_http_info(force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +105,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'download_client_resource'
+            'force_save',
+            'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,59 +131,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_download_client" % _key
+                    " to method create_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient', 'POST',
+            '/api/v1/notification', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,27 +194,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def create_download_client_action_by_name(self, name : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> None:  # noqa: E501
-        """create_download_client_action_by_name  # noqa: E501
+    def create_notification_action_by_name(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_action_by_name(name, download_client_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -216,30 +223,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_download_client_action_by_name_with_http_info(name, download_client_resource, **kwargs)  # noqa: E501
+        return self.create_notification_action_by_name_with_http_info(name, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_download_client_action_by_name_with_http_info(self, name : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """create_download_client_action_by_name  # noqa: E501
+    def create_notification_action_by_name_with_http_info(self, name : StrictStr, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """create_notification_action_by_name  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_download_client_action_by_name_with_http_info(name, download_client_resource, async_req=True)
+        >>> thread = api.create_notification_action_by_name_with_http_info(name, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param name: (required)
         :type name: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -260,15 +267,15 @@
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
             'name',
-            'download_client_resource'
+            'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -279,15 +286,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_download_client_action_by_name" % _key
+                    " to method create_notification_action_by_name" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -303,31 +310,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/action/{name}', 'POST',
+            '/api/v1/notification/action/{name}', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -336,21 +343,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def delete_download_client(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
-        """delete_download_client  # noqa: E501
+    def delete_notification(self, id : StrictInt, **kwargs) -> None:  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_download_client(id, async_req=True)
+        >>> thread = api.delete_notification(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -363,24 +370,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.delete_download_client_with_http_info(id, **kwargs)  # noqa: E501
+        return self.delete_notification_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def delete_download_client_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """delete_download_client  # noqa: E501
+    def delete_notification_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """delete_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.delete_download_client_with_http_info(id, async_req=True)
+        >>> thread = api.delete_notification_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -423,15 +430,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method delete_download_client" % _key
+                    " to method delete_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -454,15 +461,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/{id}', 'DELETE',
+            '/api/v1/notification/{id}', 'DELETE',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -471,21 +478,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_download_client_by_id(self, id : StrictInt, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """get_download_client_by_id  # noqa: E501
+    def get_notification_by_id(self, id : StrictInt, **kwargs) -> NotificationResource:  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_download_client_by_id(id, async_req=True)
+        >>> thread = api.get_notification_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -495,27 +502,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_download_client_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_notification_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_download_client_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_download_client_by_id  # noqa: E501
+    def get_notification_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_notification_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_download_client_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_notification_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -533,15 +540,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -558,15 +565,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_download_client_by_id" % _key
+                    " to method get_notification_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -585,25 +592,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/{id}', 'GET',
+            '/api/v1/notification/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -612,21 +619,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_download_client(self, **kwargs) -> List[DownloadClientResource]:  # noqa: E501
-        """list_download_client  # noqa: E501
+    def list_notification(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client(async_req=True)
+        >>> thread = api.list_notification(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -634,27 +641,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[DownloadClientResource]
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_download_client_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_download_client_with_http_info(self, **kwargs):  # noqa: E501
-        """list_download_client  # noqa: E501
+    def list_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_with_http_info(async_req=True)
+        >>> thread = api.list_notification_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -670,15 +677,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[DownloadClientResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -694,15 +701,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_download_client" % _key
+                    " to method list_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -719,25 +726,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[DownloadClientResource]",
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient', 'GET',
+            '/api/v1/notification', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -746,21 +753,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_download_client_schema(self, **kwargs) -> List[DownloadClientResource]:  # noqa: E501
-        """list_download_client_schema  # noqa: E501
+    def list_notification_schema(self, **kwargs) -> List[NotificationResource]:  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_schema(async_req=True)
+        >>> thread = api.list_notification_schema(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -768,27 +775,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[DownloadClientResource]
+        :rtype: List[NotificationResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_download_client_schema_with_http_info(**kwargs)  # noqa: E501
+        return self.list_notification_schema_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_download_client_schema_with_http_info(self, **kwargs):  # noqa: E501
-        """list_download_client_schema  # noqa: E501
+    def list_notification_schema_with_http_info(self, **kwargs):  # noqa: E501
+        """list_notification_schema  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_download_client_schema_with_http_info(async_req=True)
+        >>> thread = api.list_notification_schema_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -804,15 +811,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[DownloadClientResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[NotificationResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -828,15 +835,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_download_client_schema" % _key
+                    " to method list_notification_schema" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -853,25 +860,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[DownloadClientResource]",
+            '200': "List[NotificationResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/schema', 'GET',
+            '/api/v1/notification/schema', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -880,25 +887,25 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def test_download_client(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> None:  # noqa: E501
-        """test_download_client  # noqa: E501
+    def test_notification(self, notification_resource : Optional[NotificationResource] = None, **kwargs) -> None:  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_download_client(download_client_resource, async_req=True)
+        >>> thread = api.test_notification(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
@@ -907,28 +914,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.test_download_client_with_http_info(download_client_resource, **kwargs)  # noqa: E501
+        return self.test_notification_with_http_info(notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def test_download_client_with_http_info(self, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """test_download_client  # noqa: E501
+    def test_notification_with_http_info(self, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """test_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.test_download_client_with_http_info(download_client_resource, async_req=True)
+        >>> thread = api.test_notification_with_http_info(notification_resource, async_req=True)
         >>> result = thread.get()
 
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -948,15 +955,15 @@
                  returns the request thread.
         :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
-            'download_client_resource'
+            'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -967,15 +974,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method test_download_client" % _key
+                    " to method test_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -989,31 +996,31 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/test', 'POST',
+            '/api/v1/notification/test', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1022,21 +1029,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def testall_download_client(self, **kwargs) -> None:  # noqa: E501
-        """testall_download_client  # noqa: E501
+    def testall_notification(self, **kwargs) -> None:  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_download_client(async_req=True)
+        >>> thread = api.testall_notification(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1047,24 +1054,24 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.testall_download_client_with_http_info(**kwargs)  # noqa: E501
+        return self.testall_notification_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def testall_download_client_with_http_info(self, **kwargs):  # noqa: E501
-        """testall_download_client  # noqa: E501
+    def testall_notification_with_http_info(self, **kwargs):  # noqa: E501
+        """testall_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.testall_download_client_with_http_info(async_req=True)
+        >>> thread = api.testall_notification_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1104,15 +1111,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method testall_download_client" % _key
+                    " to method testall_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -1133,15 +1140,15 @@
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/testall', 'POST',
+            '/api/v1/notification/testall', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -1150,59 +1157,63 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_download_client(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs) -> DownloadClientResource:  # noqa: E501
-        """update_download_client  # noqa: E501
+    def update_notification(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs) -> NotificationResource:  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client(id, download_client_resource, async_req=True)
+        >>> thread = api.update_notification(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: DownloadClientResource
+        :rtype: NotificationResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_download_client_with_http_info(id, download_client_resource, **kwargs)  # noqa: E501
+        return self.update_notification_with_http_info(id, force_save, notification_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_download_client_with_http_info(self, id : StrictStr, download_client_resource : Optional[DownloadClientResource] = None, **kwargs):  # noqa: E501
-        """update_download_client  # noqa: E501
+    def update_notification_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, notification_resource : Optional[NotificationResource] = None, **kwargs):  # noqa: E501
+        """update_notification  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_download_client_with_http_info(id, download_client_resource, async_req=True)
+        >>> thread = api.update_notification_with_http_info(id, force_save, notification_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
-        :param download_client_resource:
-        :type download_client_resource: DownloadClientResource
+        :param force_save:
+        :type force_save: bool
+        :param notification_resource:
+        :type notification_resource: NotificationResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -1216,22 +1227,23 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(DownloadClientResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(NotificationResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
-            'download_client_resource'
+            'force_save',
+            'notification_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -1242,61 +1254,63 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method update_download_client" % _key
+                    " to method update_notification" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['download_client_resource']:
-            _body_params = _params['download_client_resource']
+        if _params['notification_resource']:
+            _body_params = _params['notification_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "DownloadClientResource",
+            '200': "NotificationResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/downloadclient/{id}', 'PUT',
+            '/api/v1/notification/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/download_client_config_api.py` & `readarr-py-0.4.0/readarr/api/download_client_config_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "DownloadClientConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/edition_api.py` & `readarr-py-0.4.0/readarr/api/edition_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/file_system_api.py` & `readarr-py-0.4.0/readarr/api/file_system_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/health_api.py` & `readarr-py-0.4.0/readarr/api/language_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from readarr.models.health_resource import HealthResource
+from readarr.models.language_resource import LanguageResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class HealthApi(object):
+class LanguageApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_health_by_id(self, id : StrictInt, **kwargs) -> HealthResource:  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_language_by_id(self, id : StrictInt, **kwargs) -> LanguageResource:  # noqa: E501
+        """get_language_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id(id, async_req=True)
+        >>> thread = api.get_language_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -63,27 +63,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: HealthResource
+        :rtype: LanguageResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_health_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_language_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_health_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_health_by_id  # noqa: E501
+    def get_language_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_language_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_health_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_language_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -101,15 +101,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(HealthResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(LanguageResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_health_by_id" % _key
+                    " to method get_language_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -153,25 +153,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "HealthResource",
+            '200': "LanguageResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health/{id}', 'GET',
+            '/api/v1/language/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,21 +180,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_health(self, **kwargs) -> List[HealthResource]:  # noqa: E501
-        """list_health  # noqa: E501
+    def list_language(self, **kwargs) -> List[LanguageResource]:  # noqa: E501
+        """list_language  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health(async_req=True)
+        >>> thread = api.list_language(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -202,27 +202,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[HealthResource]
+        :rtype: List[LanguageResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_health_with_http_info(**kwargs)  # noqa: E501
+        return self.list_language_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_health_with_http_info(self, **kwargs):  # noqa: E501
-        """list_health  # noqa: E501
+    def list_language_with_http_info(self, **kwargs):  # noqa: E501
+        """list_language  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_health_with_http_info(async_req=True)
+        >>> thread = api.list_language_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -238,15 +238,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[HealthResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[LanguageResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -262,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_health" % _key
+                    " to method list_language" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[HealthResource]",
+            '200': "List[LanguageResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/health', 'GET',
+            '/api/v1/language', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/history_api.py` & `readarr-py-0.4.0/readarr/api/history_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/host_config_api.py` & `readarr-py-0.4.0/readarr/api/host_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "HostConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/import_list_api.py` & `readarr-py-0.4.0/readarr/api/import_list_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from readarr.models.import_list_bulk_resource import ImportListBulkResource
 from readarr.models.import_list_resource import ImportListResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_import_list(self, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+    def create_import_list(self, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
         """create_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_import_list(import_list_resource, async_req=True)
+        >>> thread = api.create_import_list(force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +69,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ImportListResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_import_list_with_http_info(import_list_resource, **kwargs)  # noqa: E501
+        return self.create_import_list_with_http_info(force_save, import_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_import_list_with_http_info(self, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
+    def create_import_list_with_http_info(self, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
         """create_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_import_list_with_http_info(import_list_resource, async_req=True)
+        >>> thread = api.create_import_list_with_http_info(force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'import_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +144,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -153,20 +161,20 @@
         # process the body parameter
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -471,14 +479,156 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def delete_import_list_bulk(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_import_list_bulk(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_import_list_bulk_with_http_info(import_list_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_import_list_bulk_with_http_info(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_import_list_bulk_with_http_info(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'import_list_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_import_list_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['import_list_bulk_resource']:
+            _body_params = _params['import_list_bulk_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/v1/importlist/bulk', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_import_list_by_id(self, id : StrictInt, **kwargs) -> ImportListResource:  # noqa: E501
         """get_import_list_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_import_list_by_id(id, async_req=True)
@@ -585,15 +735,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListResource",
         }
@@ -719,15 +869,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ImportListResource]",
         }
@@ -853,15 +1003,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[ImportListResource]",
         }
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_import_list_bulk(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+        """put_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_import_list_bulk(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: ImportListResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_import_list_bulk_with_http_info(import_list_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_import_list_bulk_with_http_info(self, import_list_bulk_resource : Optional[ImportListBulkResource] = None, **kwargs):  # noqa: E501
+        """put_import_list_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_import_list_bulk_with_http_info(import_list_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param import_list_bulk_resource:
+        :type import_list_bulk_resource: ImportListBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'import_list_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method put_import_list_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['import_list_bulk_resource']:
+            _body_params = _params['import_list_bulk_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "ImportListResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/importlist/bulk', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def test_import_list(self, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> None:  # noqa: E501
         """test_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_import_list(import_list_resource, async_req=True)
@@ -995,15 +1293,15 @@
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1150,25 +1448,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_import_list(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
+    def update_import_list(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs) -> ImportListResource:  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1479,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: ImportListResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_import_list_with_http_info(id, import_list_resource, **kwargs)  # noqa: E501
+        return self.update_import_list_with_http_info(id, force_save, import_list_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_import_list_with_http_info(self, id : StrictStr, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
+    def update_import_list_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, import_list_resource : Optional[ImportListResource] = None, **kwargs):  # noqa: E501
         """update_import_list  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_import_list_with_http_info(id, import_list_resource, async_req=True)
+        >>> thread = api.update_import_list_with_http_info(id, force_save, import_list_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param import_list_resource:
         :type import_list_resource: ImportListResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1525,15 @@
         :rtype: tuple(ImportListResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'import_list_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1559,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1576,20 @@
         # process the body parameter
         _body_params = None
         if _params['import_list_resource']:
             _body_params = _params['import_list_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `readarr-py-0.3.0/readarr/api/import_list_exclusion_api.py` & `readarr-py-0.4.0/readarr/api/import_list_exclusion_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ImportListExclusionResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/indexer_api.py` & `readarr-py-0.4.0/readarr/api/indexer_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
+from readarr.models.indexer_bulk_resource import IndexerBulkResource
 from readarr.models.indexer_resource import IndexerResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -39,23 +40,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+    def create_indexer(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
         """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +69,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_indexer_with_http_info(indexer_resource, **kwargs)  # noqa: E501
+        return self.create_indexer_with_http_info(force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_indexer_with_http_info(self, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+    def create_indexer_with_http_info(self, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
         """create_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_indexer_with_http_info(indexer_resource, async_req=True)
+        >>> thread = api.create_indexer_with_http_info(force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +112,15 @@
                  returns the request thread.
         :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +144,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -153,20 +161,20 @@
         # process the body parameter
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +317,15 @@
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -471,14 +479,156 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def delete_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> None:  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_indexer_bulk(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.delete_indexer_bulk_with_http_info(indexer_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def delete_indexer_bulk_with_http_info(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs):  # noqa: E501
+        """delete_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.delete_indexer_bulk_with_http_info(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: None
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'indexer_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method delete_indexer_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['indexer_bulk_resource']:
+            _body_params = _params['indexer_bulk_resource']
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {}
+
+        return self.api_client.call_api(
+            '/api/v1/indexer/bulk', 'DELETE',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def get_indexer_by_id(self, id : StrictInt, **kwargs) -> IndexerResource:  # noqa: E501
         """get_indexer_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.get_indexer_by_id(id, async_req=True)
@@ -585,15 +735,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerResource",
         }
@@ -719,15 +869,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[IndexerResource]",
         }
@@ -853,15 +1003,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[IndexerResource]",
         }
@@ -880,14 +1030,162 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
+    def put_indexer_bulk(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_indexer_bulk(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: IndexerResource
+        """
+        kwargs['_return_http_data_only'] = True
+        return self.put_indexer_bulk_with_http_info(indexer_bulk_resource, **kwargs)  # noqa: E501
+
+    @validate_arguments
+    def put_indexer_bulk_with_http_info(self, indexer_bulk_resource : Optional[IndexerBulkResource] = None, **kwargs):  # noqa: E501
+        """put_indexer_bulk  # noqa: E501
+
+        This method makes a synchronous HTTP request by default. To make an
+        asynchronous HTTP request, please pass async_req=True
+
+        >>> thread = api.put_indexer_bulk_with_http_info(indexer_bulk_resource, async_req=True)
+        >>> result = thread.get()
+
+        :param indexer_bulk_resource:
+        :type indexer_bulk_resource: IndexerBulkResource
+        :param async_req: Whether to execute the request asynchronously.
+        :type async_req: bool, optional
+        :param _return_http_data_only: response data without head status code
+                                       and headers
+        :type _return_http_data_only: bool, optional
+        :param _preload_content: if False, the urllib3.HTTPResponse object will
+                                 be returned without reading/decoding response
+                                 data. Default is True.
+        :type _preload_content: bool, optional
+        :param _request_timeout: timeout setting for this request. If one
+                                 number provided, it will be total request
+                                 timeout. It can also be a pair (tuple) of
+                                 (connection, read) timeouts.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :type _request_auth: dict, optional
+        :type _content_type: string, optional: force content-type for the request
+        :return: Returns the result object.
+                 If the method is called asynchronously,
+                 returns the request thread.
+        :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
+        """
+
+        _params = locals()
+
+        _all_params = [
+            'indexer_bulk_resource'
+        ]
+        _all_params.extend(
+            [
+                'async_req',
+                '_return_http_data_only',
+                '_preload_content',
+                '_request_timeout',
+                '_request_auth',
+                '_content_type',
+                '_headers'
+            ]
+        )
+
+        # validate the arguments
+        for _key, _val in _params['kwargs'].items():
+            if _key not in _all_params:
+                raise ApiTypeError(
+                    "Got an unexpected keyword argument '%s'"
+                    " to method put_indexer_bulk" % _key
+                )
+            _params[_key] = _val
+        del _params['kwargs']
+
+        _collection_formats = {}
+
+        # process the path parameters
+        _path_params = {}
+
+        # process the query parameters
+        _query_params = []
+
+        # process the header parameters
+        _header_params = dict(_params.get('_headers', {}))
+
+        # process the form parameters
+        _form_params = []
+        _files = {}
+
+        # process the body parameter
+        _body_params = None
+        if _params['indexer_bulk_resource']:
+            _body_params = _params['indexer_bulk_resource']
+
+        # set the HTTP header `Accept`
+        _header_params['Accept'] = self.api_client.select_header_accept(
+            ['application/json'])  # noqa: E501
+
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
+        # authentication setting
+        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
+
+        _response_types_map = {
+            '200': "IndexerResource",
+        }
+
+        return self.api_client.call_api(
+            '/api/v1/indexer/bulk', 'PUT',
+            _path_params,
+            _query_params,
+            _header_params,
+            body=_body_params,
+            post_params=_form_params,
+            files=_files,
+            response_types_map=_response_types_map,
+            auth_settings=_auth_settings,
+            async_req=_params.get('async_req'),
+            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
+            _preload_content=_params.get('_preload_content', True),
+            _request_timeout=_params.get('_request_timeout'),
+            collection_formats=_collection_formats,
+            _request_auth=_params.get('_request_auth'))
+
+    @validate_arguments
     def test_indexer(self, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> None:  # noqa: E501
         """test_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
         >>> thread = api.test_indexer(indexer_resource, async_req=True)
@@ -995,15 +1293,15 @@
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1150,25 +1448,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_indexer(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
+    def update_indexer(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs) -> IndexerResource:  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1479,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: IndexerResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_indexer_with_http_info(id, indexer_resource, **kwargs)  # noqa: E501
+        return self.update_indexer_with_http_info(id, force_save, indexer_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_indexer_with_http_info(self, id : StrictStr, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
+    def update_indexer_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, indexer_resource : Optional[IndexerResource] = None, **kwargs):  # noqa: E501
         """update_indexer  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_indexer_with_http_info(id, indexer_resource, async_req=True)
+        >>> thread = api.update_indexer_with_http_info(id, force_save, indexer_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param indexer_resource:
         :type indexer_resource: IndexerResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1525,15 @@
         :rtype: tuple(IndexerResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'indexer_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1559,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1576,20 @@
         # process the body parameter
         _body_params = None
         if _params['indexer_resource']:
             _body_params = _params['indexer_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `readarr-py-0.3.0/readarr/api/indexer_config_api.py` & `readarr-py-0.4.0/readarr/api/indexer_config_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "IndexerConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/initialize_js_api.py` & `readarr-py-0.4.0/readarr/api/initialize_js_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/language_api.py` & `readarr-py-0.4.0/readarr/api/tag_details_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,43 @@
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
 from typing import List
 
-from readarr.models.language_resource import LanguageResource
+from readarr.models.tag_details_resource import TagDetailsResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class LanguageApi(object):
+class TagDetailsApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_language_by_id(self, id : StrictInt, **kwargs) -> LanguageResource:  # noqa: E501
-        """get_language_by_id  # noqa: E501
+    def get_tag_detail_by_id(self, id : StrictInt, **kwargs) -> TagDetailsResource:  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_language_by_id(id, async_req=True)
+        >>> thread = api.get_tag_detail_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -63,27 +63,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: LanguageResource
+        :rtype: TagDetailsResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_language_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_tag_detail_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_language_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_language_by_id  # noqa: E501
+    def get_tag_detail_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_tag_detail_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_language_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_tag_detail_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -101,15 +101,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(LanguageResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TagDetailsResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -126,15 +126,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_language_by_id" % _key
+                    " to method get_tag_detail_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -153,25 +153,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "LanguageResource",
+            '200': "TagDetailsResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/language/{id}', 'GET',
+            '/api/v1/tag/detail/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,21 +180,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_language(self, **kwargs) -> List[LanguageResource]:  # noqa: E501
-        """list_language  # noqa: E501
+    def list_tag_detail(self, **kwargs) -> List[TagDetailsResource]:  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_language(async_req=True)
+        >>> thread = api.list_tag_detail(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -202,27 +202,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[LanguageResource]
+        :rtype: List[TagDetailsResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_language_with_http_info(**kwargs)  # noqa: E501
+        return self.list_tag_detail_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_language_with_http_info(self, **kwargs):  # noqa: E501
-        """list_language  # noqa: E501
+    def list_tag_detail_with_http_info(self, **kwargs):  # noqa: E501
+        """list_tag_detail  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_language_with_http_info(async_req=True)
+        >>> thread = api.list_tag_detail_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -238,15 +238,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[LanguageResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TagDetailsResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
         ]
         _all_params.extend(
@@ -262,15 +262,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_language" % _key
+                    " to method list_tag_detail" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -293,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[LanguageResource]",
+            '200': "List[TagDetailsResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/language', 'GET',
+            '/api/v1/tag/detail', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/localization_api.py` & `readarr-py-0.4.0/readarr/api/localization_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/log_api.py` & `readarr-py-0.4.0/readarr/api/log_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/log_file_api.py` & `readarr-py-0.4.0/readarr/api/log_file_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/manual_import_api.py` & `readarr-py-0.4.0/readarr/api/manual_import_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/media_cover_api.py` & `readarr-py-0.4.0/readarr/api/media_cover_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/media_management_config_api.py` & `readarr-py-0.4.0/readarr/api/media_management_config_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MediaManagementConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/metadata_api.py` & `readarr-py-0.4.0/readarr/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt, StrictStr
+from pydantic import StrictBool, StrictInt, StrictStr
 
 from typing import List, Optional
 
 from readarr.models.metadata_resource import MetadataResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
@@ -39,23 +39,25 @@
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_metadata(self, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
+    def create_metadata(self, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
         """create_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_metadata(metadata_resource, async_req=True)
+        >>> thread = api.create_metadata(force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -66,26 +68,28 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MetadataResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_metadata_with_http_info(metadata_resource, **kwargs)  # noqa: E501
+        return self.create_metadata_with_http_info(force_save, metadata_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_metadata_with_http_info(self, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
+    def create_metadata_with_http_info(self, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
         """create_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_metadata_with_http_info(metadata_resource, async_req=True)
+        >>> thread = api.create_metadata_with_http_info(force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -107,14 +111,15 @@
                  returns the request thread.
         :rtype: tuple(MetadataResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
+            'force_save',
             'metadata_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -138,14 +143,16 @@
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -153,20 +160,20 @@
         # process the body parameter
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
@@ -309,15 +316,15 @@
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -585,15 +592,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataResource",
         }
@@ -719,15 +726,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[MetadataResource]",
         }
@@ -853,15 +860,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "List[MetadataResource]",
         }
@@ -995,15 +1002,15 @@
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {}
@@ -1150,25 +1157,27 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def update_metadata(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
+    def update_metadata(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs) -> MetadataResource:  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
@@ -1179,28 +1188,30 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: MetadataResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.update_metadata_with_http_info(id, metadata_resource, **kwargs)  # noqa: E501
+        return self.update_metadata_with_http_info(id, force_save, metadata_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def update_metadata_with_http_info(self, id : StrictStr, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
+    def update_metadata_with_http_info(self, id : StrictStr, force_save : Optional[StrictBool] = None, metadata_resource : Optional[MetadataResource] = None, **kwargs):  # noqa: E501
         """update_metadata  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.update_metadata_with_http_info(id, metadata_resource, async_req=True)
+        >>> thread = api.update_metadata_with_http_info(id, force_save, metadata_resource, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: str
+        :param force_save:
+        :type force_save: bool
         :param metadata_resource:
         :type metadata_resource: MetadataResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
@@ -1223,14 +1234,15 @@
         :rtype: tuple(MetadataResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id',
+            'force_save',
             'metadata_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
@@ -1256,14 +1268,16 @@
         # process the path parameters
         _path_params = {}
         if _params['id']:
             _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
+        if _params.get('force_save') is not None:  # noqa: E501
+            _query_params.append(('forceSave', _params['force_save']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -1271,20 +1285,20 @@
         # process the body parameter
         _body_params = None
         if _params['metadata_resource']:
             _body_params = _params['metadata_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # set the HTTP header `Content-Type`
         _content_types_list = _params.get('_content_type',
             self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
+                ['application/json']))
         if _content_types_list:
                 _header_params['Content-Type'] = _content_types_list
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
```

### Comparing `readarr-py-0.3.0/readarr/api/metadata_profile_api.py` & `readarr-py-0.4.0/readarr/api/metadata_profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProfileResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/metadata_profile_schema_api.py` & `readarr-py-0.4.0/readarr/api/metadata_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/metadata_provider_config_api.py` & `readarr-py-0.4.0/readarr/api/metadata_provider_config_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "MetadataProviderConfigResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/missing_api.py` & `readarr-py-0.4.0/readarr/api/missing_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "BookResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/naming_config_api.py` & `readarr-py-0.4.0/readarr/api/naming_config_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "NamingConfigResource",
         }
@@ -314,27 +314,29 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_naming_config_examples(self, rename_books : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, standard_book_format : Optional[StrictStr] = None, author_folder_format : Optional[StrictStr] = None, include_author_name : Optional[StrictBool] = None, include_book_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
+    def get_naming_config_examples(self, rename_books : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, standard_book_format : Optional[StrictStr] = None, author_folder_format : Optional[StrictStr] = None, include_author_name : Optional[StrictBool] = None, include_book_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs) -> None:  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples(rename_books, replace_illegal_characters, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples(rename_books, replace_illegal_characters, colon_replacement_format, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_books:
         :type rename_books: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param standard_book_format:
         :type standard_book_format: str
         :param author_folder_format:
         :type author_folder_format: str
         :param include_author_name:
         :type include_author_name: bool
         :param include_book_title:
@@ -363,30 +365,32 @@
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
         :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_naming_config_examples_with_http_info(rename_books, replace_illegal_characters, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
+        return self.get_naming_config_examples_with_http_info(rename_books, replace_illegal_characters, colon_replacement_format, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_naming_config_examples_with_http_info(self, rename_books : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, standard_book_format : Optional[StrictStr] = None, author_folder_format : Optional[StrictStr] = None, include_author_name : Optional[StrictBool] = None, include_book_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
+    def get_naming_config_examples_with_http_info(self, rename_books : Optional[StrictBool] = None, replace_illegal_characters : Optional[StrictBool] = None, colon_replacement_format : Optional[StrictInt] = None, standard_book_format : Optional[StrictStr] = None, author_folder_format : Optional[StrictStr] = None, include_author_name : Optional[StrictBool] = None, include_book_title : Optional[StrictBool] = None, include_quality : Optional[StrictBool] = None, replace_spaces : Optional[StrictBool] = None, separator : Optional[StrictStr] = None, number_style : Optional[StrictStr] = None, id : Optional[StrictInt] = None, resource_name : Optional[StrictStr] = None, **kwargs):  # noqa: E501
         """get_naming_config_examples  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_naming_config_examples_with_http_info(rename_books, replace_illegal_characters, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
+        >>> thread = api.get_naming_config_examples_with_http_info(rename_books, replace_illegal_characters, colon_replacement_format, standard_book_format, author_folder_format, include_author_name, include_book_title, include_quality, replace_spaces, separator, number_style, id, resource_name, async_req=True)
         >>> result = thread.get()
 
         :param rename_books:
         :type rename_books: bool
         :param replace_illegal_characters:
         :type replace_illegal_characters: bool
+        :param colon_replacement_format:
+        :type colon_replacement_format: int
         :param standard_book_format:
         :type standard_book_format: str
         :param author_folder_format:
         :type author_folder_format: str
         :param include_author_name:
         :type include_author_name: bool
         :param include_book_title:
@@ -428,14 +432,15 @@
         """
 
         _params = locals()
 
         _all_params = [
             'rename_books',
             'replace_illegal_characters',
+            'colon_replacement_format',
             'standard_book_format',
             'author_folder_format',
             'include_author_name',
             'include_book_title',
             'include_quality',
             'replace_spaces',
             'separator',
@@ -472,14 +477,16 @@
 
         # process the query parameters
         _query_params = []
         if _params.get('rename_books') is not None:  # noqa: E501
             _query_params.append(('RenameBooks', _params['rename_books']))
         if _params.get('replace_illegal_characters') is not None:  # noqa: E501
             _query_params.append(('ReplaceIllegalCharacters', _params['replace_illegal_characters']))
+        if _params.get('colon_replacement_format') is not None:  # noqa: E501
+            _query_params.append(('ColonReplacementFormat', _params['colon_replacement_format']))
         if _params.get('standard_book_format') is not None:  # noqa: E501
             _query_params.append(('StandardBookFormat', _params['standard_book_format']))
         if _params.get('author_folder_format') is not None:  # noqa: E501
             _query_params.append(('AuthorFolderFormat', _params['author_folder_format']))
         if _params.get('include_author_name') is not None:  # noqa: E501
             _query_params.append(('IncludeAuthorName', _params['include_author_name']))
         if _params.get('include_book_title') is not None:  # noqa: E501
```

### Comparing `readarr-py-0.3.0/readarr/api/parse_api.py` & `readarr-py-0.4.0/readarr/api/parse_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/ping_api.py` & `readarr-py-0.4.0/readarr/api/ping_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/quality_definition_api.py` & `readarr-py-0.4.0/readarr/api/quality_definition_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityDefinitionResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/quality_profile_api.py` & `readarr-py-0.4.0/readarr/api/quality_profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "QualityProfileResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/quality_profile_schema_api.py` & `readarr-py-0.4.0/readarr/api/quality_profile_schema_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/queue_action_api.py` & `readarr-py-0.4.0/readarr/api/queue_action_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/queue_api.py` & `readarr-py-0.4.0/readarr/api/queue_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 from typing_extensions import Annotated
 
 from pydantic import StrictBool, StrictInt
 
 from typing import Optional
 
 from readarr.models.queue_bulk_resource import QueueBulkResource
-from readarr.models.queue_resource import QueueResource
 from readarr.models.queue_resource_paging_resource import QueueResourcePagingResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
@@ -506,155 +505,14 @@
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
-            auth_settings=_auth_settings,
-            async_req=_params.get('async_req'),
-            _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
-            _preload_content=_params.get('_preload_content', True),
-            _request_timeout=_params.get('_request_timeout'),
-            collection_formats=_collection_formats,
-            _request_auth=_params.get('_request_auth'))
-
-    @validate_arguments
-    def get_queue_by_id(self, id : StrictInt, **kwargs) -> QueueResource:  # noqa: E501
-        """get_queue_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_queue_by_id(id, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: QueueResource
-        """
-        kwargs['_return_http_data_only'] = True
-        return self.get_queue_by_id_with_http_info(id, **kwargs)  # noqa: E501
-
-    @validate_arguments
-    def get_queue_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_by_id  # noqa: E501
-
-        This method makes a synchronous HTTP request by default. To make an
-        asynchronous HTTP request, please pass async_req=True
-
-        >>> thread = api.get_queue_by_id_with_http_info(id, async_req=True)
-        >>> result = thread.get()
-
-        :param id: (required)
-        :type id: int
-        :param async_req: Whether to execute the request asynchronously.
-        :type async_req: bool, optional
-        :param _return_http_data_only: response data without head status code
-                                       and headers
-        :type _return_http_data_only: bool, optional
-        :param _preload_content: if False, the urllib3.HTTPResponse object will
-                                 be returned without reading/decoding response
-                                 data. Default is True.
-        :type _preload_content: bool, optional
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_auth: dict, optional
-        :type _content_type: string, optional: force content-type for the request
-        :return: Returns the result object.
-                 If the method is called asynchronously,
-                 returns the request thread.
-        :rtype: tuple(QueueResource, status_code(int), headers(HTTPHeaderDict))
-        """
-
-        _params = locals()
-
-        _all_params = [
-            'id'
-        ]
-        _all_params.extend(
-            [
-                'async_req',
-                '_return_http_data_only',
-                '_preload_content',
-                '_request_timeout',
-                '_request_auth',
-                '_content_type',
-                '_headers'
-            ]
-        )
-
-        # validate the arguments
-        for _key, _val in _params['kwargs'].items():
-            if _key not in _all_params:
-                raise ApiTypeError(
-                    "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_by_id" % _key
-                )
-            _params[_key] = _val
-        del _params['kwargs']
-
-        _collection_formats = {}
-
-        # process the path parameters
-        _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
-
-        # process the query parameters
-        _query_params = []
-
-        # process the header parameters
-        _header_params = dict(_params.get('_headers', {}))
-
-        # process the form parameters
-        _form_params = []
-        _files = {}
-
-        # process the body parameter
-        _body_params = None
-
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # authentication setting
-        _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
-
-        _response_types_map = {
-            '200': "QueueResource",
-        }
-
-        return self.api_client.call_api(
-            '/api/v1/queue/{id}', 'GET',
-            _path_params,
-            _query_params,
-            _header_params,
-            body=_body_params,
-            post_params=_form_params,
-            files=_files,
-            response_types_map=_response_types_map,
             auth_settings=_auth_settings,
             async_req=_params.get('async_req'),
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
```

### Comparing `readarr-py-0.3.0/readarr/api/queue_details_api.py` & `readarr-py-0.4.0/readarr/api/release_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,81 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictBool, StrictInt, conlist
+from pydantic import StrictInt
 
 from typing import List, Optional
 
-from readarr.models.queue_resource import QueueResource
+from readarr.models.release_resource import ReleaseResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueDetailsApi(object):
+class ReleaseApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_queue_details_by_id(self, id : StrictInt, **kwargs) -> QueueResource:  # noqa: E501
-        """get_queue_details_by_id  # noqa: E501
+    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id(id, async_req=True)
+        >>> thread = api.create_release(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: QueueResource
+        :rtype: ReleaseResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_details_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.create_release_with_http_info(release_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_details_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_details_by_id  # noqa: E501
+    def create_release_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
+        """create_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_details_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.create_release_with_http_info(release_resource, async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
+        :param release_resource:
+        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
+            'release_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,52 +126,59 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_details_by_id" % _key
+                    " to method create_release" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['release_resource']:
+            _body_params = _params['release_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueResource",
+            '200': "ReleaseResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/details/{id}', 'GET',
+            '/api/v1/release', 'POST',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -180,67 +187,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_queue_details(self, author_id : Optional[StrictInt] = None, book_ids : Optional[conlist(StrictInt)] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs) -> List[QueueResource]:  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_release(self, book_id : Optional[StrictInt] = None, author_id : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details(author_id, book_ids, include_author, include_book, async_req=True)
+        >>> thread = api.list_release(book_id, author_id, async_req=True)
         >>> result = thread.get()
 
+        :param book_id:
+        :type book_id: int
         :param author_id:
         :type author_id: int
-        :param book_ids:
-        :type book_ids: List[int]
-        :param include_author:
-        :type include_author: bool
-        :param include_book:
-        :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[QueueResource]
+        :rtype: List[ReleaseResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_queue_details_with_http_info(author_id, book_ids, include_author, include_book, **kwargs)  # noqa: E501
+        return self.list_release_with_http_info(book_id, author_id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_queue_details_with_http_info(self, author_id : Optional[StrictInt] = None, book_ids : Optional[conlist(StrictInt)] = None, include_author : Optional[StrictBool] = None, include_book : Optional[StrictBool] = None, **kwargs):  # noqa: E501
-        """list_queue_details  # noqa: E501
+    def list_release_with_http_info(self, book_id : Optional[StrictInt] = None, author_id : Optional[StrictInt] = None, **kwargs):  # noqa: E501
+        """list_release  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_queue_details_with_http_info(author_id, book_ids, include_author, include_book, async_req=True)
+        >>> thread = api.list_release_with_http_info(book_id, author_id, async_req=True)
         >>> result = thread.get()
 
+        :param book_id:
+        :type book_id: int
         :param author_id:
         :type author_id: int
-        :param book_ids:
-        :type book_ids: List[int]
-        :param include_author:
-        :type include_author: bool
-        :param include_book:
-        :type include_book: bool
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -254,24 +253,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[QueueResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'author_id',
-            'book_ids',
-            'include_author',
-            'include_book'
+            'book_id',
+            'author_id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -282,35 +279,30 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_queue_details" % _key
+                    " to method list_release" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
 
         # process the query parameters
         _query_params = []
+        if _params.get('book_id') is not None:  # noqa: E501
+            _query_params.append(('bookId', _params['book_id']))
         if _params.get('author_id') is not None:  # noqa: E501
             _query_params.append(('authorId', _params['author_id']))
-        if _params.get('book_ids') is not None:  # noqa: E501
-            _query_params.append(('bookIds', _params['book_ids']))
-            _collection_formats['bookIds'] = 'multi'
-        if _params.get('include_author') is not None:  # noqa: E501
-            _query_params.append(('includeAuthor', _params['include_author']))
-        if _params.get('include_book') is not None:  # noqa: E501
-            _query_params.append(('includeBook', _params['include_book']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
@@ -322,19 +314,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[QueueResource]",
+            '200': "List[ReleaseResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/details', 'GET',
+            '/api/v1/release', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/queue_status_api.py` & `readarr-py-0.4.0/readarr/api/update_log_file_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,75 +13,81 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import constr, validator
 
-from readarr.models.queue_status_resource import QueueStatusResource
+from typing import List
+
+from readarr.models.log_file_resource import LogFileResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class QueueStatusApi(object):
+class UpdateLogFileApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def get_queue_status(self, **kwargs) -> QueueStatusResource:  # noqa: E501
-        """get_queue_status  # noqa: E501
+    def get_log_file_update_by_filename(self, filename : constr(strict=True), **kwargs) -> None:  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status(async_req=True)
+        >>> thread = api.get_log_file_update_by_filename(filename, async_req=True)
         >>> result = thread.get()
 
+        :param filename: (required)
+        :type filename: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: QueueStatusResource
+        :rtype: None
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_status_with_http_info(**kwargs)  # noqa: E501
+        return self.get_log_file_update_by_filename_with_http_info(filename, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_status_with_http_info(self, **kwargs):  # noqa: E501
-        """get_queue_status  # noqa: E501
+    def get_log_file_update_by_filename_with_http_info(self, filename : constr(strict=True), **kwargs):  # noqa: E501
+        """get_log_file_update_by_filename  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_with_http_info(async_req=True)
+        >>> thread = api.get_log_file_update_by_filename_with_http_info(filename, async_req=True)
         >>> result = thread.get()
 
+        :param filename: (required)
+        :type filename: str
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -95,20 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueStatusResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: None
         """
 
         _params = locals()
 
         _all_params = [
+            'filename'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -119,50 +126,46 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_status" % _key
+                    " to method get_log_file_update_by_filename" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['filename']:
+            _path_params['filename'] = _params['filename']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
 
-        # set the HTTP header `Accept`
-        _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
-        _response_types_map = {
-            '200': "QueueStatusResource",
-        }
+        _response_types_map = {}
 
         return self.api_client.call_api(
-            '/api/v1/queue/status', 'GET',
+            '/api/v1/log/file/update/{filename}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -171,55 +174,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_queue_status_by_id(self, id : StrictInt, **kwargs) -> QueueStatusResource:  # noqa: E501
-        """get_queue_status_by_id  # noqa: E501
+    def list_log_file_update(self, **kwargs) -> List[LogFileResource]:  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_by_id(id, async_req=True)
+        >>> thread = api.list_log_file_update(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: QueueStatusResource
+        :rtype: List[LogFileResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_queue_status_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_log_file_update_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_queue_status_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_queue_status_by_id  # noqa: E501
+    def list_log_file_update_with_http_info(self, **kwargs):  # noqa: E501
+        """list_log_file_update  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_queue_status_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_log_file_update_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -233,21 +232,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(QueueStatusResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[LogFileResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -258,25 +256,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_queue_status_by_id" % _key
+                    " to method list_log_file_update" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -291,19 +287,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "QueueStatusResource",
+            '200': "List[LogFileResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/queue/status/{id}', 'GET',
+            '/api/v1/log/file/update', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/release_api.py` & `readarr-py-0.4.0/readarr/api/ui_config_api.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,81 +13,77 @@
 from __future__ import absolute_import
 
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
-from pydantic import StrictInt
+from pydantic import StrictInt, StrictStr
 
-from typing import List, Optional
+from typing import Optional
 
-from readarr.models.release_resource import ReleaseResource
+from readarr.models.ui_config_resource import UiConfigResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ReleaseApi(object):
+class UiConfigApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_release(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
-        """create_release  # noqa: E501
+    def get_ui_config(self, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release(release_resource, async_req=True)
+        >>> thread = api.get_ui_config(async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_release_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.get_ui_config_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_release_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
-        """create_release  # noqa: E501
+    def get_ui_config_with_http_info(self, **kwargs):  # noqa: E501
+        """get_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_with_http_info(release_resource, async_req=True)
+        >>> thread = api.get_ui_config_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +97,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'release_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,15 +121,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_release" % _key
+                    " to method get_ui_config" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -148,37 +143,28 @@
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
-
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release', 'POST',
+            '/api/v1/config/ui', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,21 +173,21 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_release_by_id(self, id : StrictInt, **kwargs) -> ReleaseResource:  # noqa: E501
-        """get_release_by_id  # noqa: E501
+    def get_ui_config_by_id(self, id : StrictInt, **kwargs) -> UiConfigResource:  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_by_id(id, async_req=True)
+        >>> thread = api.get_ui_config_by_id(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
@@ -211,27 +197,27 @@
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_release_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.get_ui_config_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_release_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_release_by_id  # noqa: E501
+    def get_ui_config_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_ui_config_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.get_ui_config_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
         :param id: (required)
         :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
@@ -249,15 +235,15 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
             'id'
         ]
@@ -274,15 +260,15 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_release_by_id" % _key
+                    " to method get_ui_config_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
@@ -301,25 +287,25 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/{id}', 'GET',
+            '/api/v1/config/ui/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -328,59 +314,59 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def list_release(self, book_id : Optional[StrictInt] = None, author_id : Optional[StrictInt] = None, **kwargs) -> List[ReleaseResource]:  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs) -> UiConfigResource:  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release(book_id, author_id, async_req=True)
+        >>> thread = api.update_ui_config(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param book_id:
-        :type book_id: int
-        :param author_id:
-        :type author_id: int
+        :param id: (required)
+        :type id: str
+        :param ui_config_resource:
+        :type ui_config_resource: UiConfigResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: List[ReleaseResource]
+        :rtype: UiConfigResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.list_release_with_http_info(book_id, author_id, **kwargs)  # noqa: E501
+        return self.update_ui_config_with_http_info(id, ui_config_resource, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def list_release_with_http_info(self, book_id : Optional[StrictInt] = None, author_id : Optional[StrictInt] = None, **kwargs):  # noqa: E501
-        """list_release  # noqa: E501
+    def update_ui_config_with_http_info(self, id : StrictStr, ui_config_resource : Optional[UiConfigResource] = None, **kwargs):  # noqa: E501
+        """update_ui_config  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.list_release_with_http_info(book_id, author_id, async_req=True)
+        >>> thread = api.update_ui_config_with_http_info(id, ui_config_resource, async_req=True)
         >>> result = thread.get()
 
-        :param book_id:
-        :type book_id: int
-        :param author_id:
-        :type author_id: int
+        :param id: (required)
+        :type id: str
+        :param ui_config_resource:
+        :type ui_config_resource: UiConfigResource
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -394,22 +380,22 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(List[ReleaseResource], status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(UiConfigResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'book_id',
-            'author_id'
+            'id',
+            'ui_config_resource'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -420,54 +406,61 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method list_release" % _key
+                    " to method update_ui_config" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
-        if _params.get('book_id') is not None:  # noqa: E501
-            _query_params.append(('bookId', _params['book_id']))
-        if _params.get('author_id') is not None:  # noqa: E501
-            _query_params.append(('authorId', _params['author_id']))
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
+        if _params['ui_config_resource']:
+            _body_params = _params['ui_config_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
+        # set the HTTP header `Content-Type`
+        _content_types_list = _params.get('_content_type',
+            self.api_client.select_header_content_type(
+                ['application/json', 'text/json', 'application/*+json']))
+        if _content_types_list:
+                _header_params['Content-Type'] = _content_types_list
+
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "List[ReleaseResource]",
+            '200': "UiConfigResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release', 'GET',
+            '/api/v1/config/ui/{id}', 'PUT',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/release_profile_api.py` & `readarr-py-0.4.0/readarr/api/release_profile_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "ReleaseProfileResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/release_push_api.py` & `readarr-py-0.4.0/readarr/api/task_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,79 +15,79 @@
 import re  # noqa: F401
 
 from pydantic import validate_arguments, ValidationError
 from typing_extensions import Annotated
 
 from pydantic import StrictInt
 
-from typing import Optional
+from typing import List
 
-from readarr.models.release_resource import ReleaseResource
+from readarr.models.task_resource import TaskResource
 
 from readarr.api_client import ApiClient
 from readarr.exceptions import (  # noqa: F401
     ApiTypeError,
     ApiValueError
 )
 
 
-class ReleasePushApi(object):
+class TaskApi(object):
     """NOTE: This class is auto generated by OpenAPI Generator
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
 
     def __init__(self, api_client=None):
         if api_client is None:
             api_client = ApiClient.get_default()
         self.api_client = api_client
 
     @validate_arguments
-    def create_release_push(self, release_resource : Optional[ReleaseResource] = None, **kwargs) -> ReleaseResource:  # noqa: E501
-        """create_release_push  # noqa: E501
+    def get_system_task_by_id(self, id : StrictInt, **kwargs) -> TaskResource:  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_push(release_resource, async_req=True)
+        >>> thread = api.get_system_task_by_id(id, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: TaskResource
         """
         kwargs['_return_http_data_only'] = True
-        return self.create_release_push_with_http_info(release_resource, **kwargs)  # noqa: E501
+        return self.get_system_task_by_id_with_http_info(id, **kwargs)  # noqa: E501
 
     @validate_arguments
-    def create_release_push_with_http_info(self, release_resource : Optional[ReleaseResource] = None, **kwargs):  # noqa: E501
-        """create_release_push  # noqa: E501
+    def get_system_task_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
+        """get_system_task_by_id  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.create_release_push_with_http_info(release_resource, async_req=True)
+        >>> thread = api.get_system_task_by_id_with_http_info(id, async_req=True)
         >>> result = thread.get()
 
-        :param release_resource:
-        :type release_resource: ReleaseResource
+        :param id: (required)
+        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -101,21 +101,21 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(TaskResource, status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'release_resource'
+            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -126,59 +126,52 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method create_release_push" % _key
+                    " to method get_system_task_by_id" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
+        if _params['id']:
+            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
         # process the form parameters
         _form_params = []
         _files = {}
 
         # process the body parameter
         _body_params = None
-        if _params['release_resource']:
-            _body_params = _params['release_resource']
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
-
-        # set the HTTP header `Content-Type`
-        _content_types_list = _params.get('_content_type',
-            self.api_client.select_header_content_type(
-                ['application/json', 'text/json', 'application/*+json']))
-        if _content_types_list:
-                _header_params['Content-Type'] = _content_types_list
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "TaskResource",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/push', 'POST',
+            '/api/v1/system/task/{id}', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
@@ -187,55 +180,51 @@
             _return_http_data_only=_params.get('_return_http_data_only'),  # noqa: E501
             _preload_content=_params.get('_preload_content', True),
             _request_timeout=_params.get('_request_timeout'),
             collection_formats=_collection_formats,
             _request_auth=_params.get('_request_auth'))
 
     @validate_arguments
-    def get_release_push_by_id(self, id : StrictInt, **kwargs) -> ReleaseResource:  # noqa: E501
-        """get_release_push_by_id  # noqa: E501
+    def list_system_task(self, **kwargs) -> List[TaskResource]:  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_push_by_id(id, async_req=True)
+        >>> thread = api.list_system_task(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
                                  data. Default is True.
         :type _preload_content: bool, optional
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: ReleaseResource
+        :rtype: List[TaskResource]
         """
         kwargs['_return_http_data_only'] = True
-        return self.get_release_push_by_id_with_http_info(id, **kwargs)  # noqa: E501
+        return self.list_system_task_with_http_info(**kwargs)  # noqa: E501
 
     @validate_arguments
-    def get_release_push_by_id_with_http_info(self, id : StrictInt, **kwargs):  # noqa: E501
-        """get_release_push_by_id  # noqa: E501
+    def list_system_task_with_http_info(self, **kwargs):  # noqa: E501
+        """list_system_task  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
 
-        >>> thread = api.get_release_push_by_id_with_http_info(id, async_req=True)
+        >>> thread = api.list_system_task_with_http_info(async_req=True)
         >>> result = thread.get()
 
-        :param id: (required)
-        :type id: int
         :param async_req: Whether to execute the request asynchronously.
         :type async_req: bool, optional
         :param _return_http_data_only: response data without head status code
                                        and headers
         :type _return_http_data_only: bool, optional
         :param _preload_content: if False, the urllib3.HTTPResponse object will
                                  be returned without reading/decoding response
@@ -249,21 +238,20 @@
                               request; this effectively ignores the authentication
                               in the spec for a single request.
         :type _request_auth: dict, optional
         :type _content_type: string, optional: force content-type for the request
         :return: Returns the result object.
                  If the method is called asynchronously,
                  returns the request thread.
-        :rtype: tuple(ReleaseResource, status_code(int), headers(HTTPHeaderDict))
+        :rtype: tuple(List[TaskResource], status_code(int), headers(HTTPHeaderDict))
         """
 
         _params = locals()
 
         _all_params = [
-            'id'
         ]
         _all_params.extend(
             [
                 'async_req',
                 '_return_http_data_only',
                 '_preload_content',
                 '_request_timeout',
@@ -274,25 +262,23 @@
         )
 
         # validate the arguments
         for _key, _val in _params['kwargs'].items():
             if _key not in _all_params:
                 raise ApiTypeError(
                     "Got an unexpected keyword argument '%s'"
-                    " to method get_release_push_by_id" % _key
+                    " to method list_system_task" % _key
                 )
             _params[_key] = _val
         del _params['kwargs']
 
         _collection_formats = {}
 
         # process the path parameters
         _path_params = {}
-        if _params['id']:
-            _path_params['id'] = _params['id']
 
         # process the query parameters
         _query_params = []
 
         # process the header parameters
         _header_params = dict(_params.get('_headers', {}))
 
@@ -307,19 +293,19 @@
         _header_params['Accept'] = self.api_client.select_header_accept(
             ['text/plain', 'application/json', 'text/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
-            '200': "ReleaseResource",
+            '200': "List[TaskResource]",
         }
 
         return self.api_client.call_api(
-            '/api/v1/release/push/{id}', 'GET',
+            '/api/v1/system/task', 'GET',
             _path_params,
             _query_params,
             _header_params,
             body=_body_params,
             post_params=_form_params,
             files=_files,
             response_types_map=_response_types_map,
```

### Comparing `readarr-py-0.3.0/readarr/api/remote_path_mapping_api.py` & `readarr-py-0.4.0/readarr/api/remote_path_mapping_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RemotePathMappingResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/rename_book_api.py` & `readarr-py-0.4.0/readarr/api/rename_book_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/retag_book_api.py` & `readarr-py-0.4.0/readarr/api/retag_book_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/root_folder_api.py` & `readarr-py-0.4.0/readarr/api/root_folder_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "RootFolderResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/search_api.py` & `readarr-py-0.4.0/readarr/api/search_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/series_api.py` & `readarr-py-0.4.0/readarr/api/series_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/static_resource_api.py` & `readarr-py-0.4.0/readarr/api/static_resource_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/system_api.py` & `readarr-py-0.4.0/readarr/api/system_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api/tag_api.py` & `readarr-py-0.4.0/readarr/api/tag_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -436,15 +436,15 @@
         _files = {}
 
         # process the body parameter
         _body_params = None
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
-            ['text/plain', 'application/json', 'text/json'])  # noqa: E501
+            ['application/json'])  # noqa: E501
 
         # authentication setting
         _auth_settings = ['apikey', 'X-Api-Key']  # noqa: E501
 
         _response_types_map = {
             '200': "TagResource",
         }
```

### Comparing `readarr-py-0.3.0/readarr/api/update_api.py` & `readarr-py-0.4.0/readarr/api/update_api.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/api_client.py` & `readarr-py-0.4.0/readarr/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
         # x-release-please-start-version
-        self.user_agent = 'readarr-py/v0.3.0'
+        self.user_agent = 'readarr-py/v0.4.0'
         # x-release-please-end
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
```

### Comparing `readarr-py-0.3.0/readarr/api_response.py` & `readarr-py-0.4.0/readarr/api_response.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/configuration.py` & `readarr-py-0.4.0/readarr/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,15 @@
 
     def to_debug_report(self):
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         # x-release-please-start-version
-        sdkversion = '0.3.0'
+        sdkversion = '0.4.0'
         # x-release-please-end
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 1.0.0\n"\
                "SDK Package Version: {sdkversion}".\
                format(env=sys.platform, pyversion=sys.version, sdkversion=sdkversion)
```

### Comparing `readarr-py-0.3.0/readarr/exceptions.py` & `readarr-py-0.4.0/readarr/exceptions.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/__init__.py` & `readarr-py-0.4.0/readarr/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 from readarr.models.custom_format import CustomFormat
 from readarr.models.custom_format_resource import CustomFormatResource
 from readarr.models.custom_format_specification_schema import CustomFormatSpecificationSchema
 from readarr.models.database_type import DatabaseType
 from readarr.models.delay_profile_resource import DelayProfileResource
 from readarr.models.development_config_resource import DevelopmentConfigResource
 from readarr.models.disk_space_resource import DiskSpaceResource
+from readarr.models.download_client_bulk_resource import DownloadClientBulkResource
 from readarr.models.download_client_config_resource import DownloadClientConfigResource
 from readarr.models.download_client_resource import DownloadClientResource
 from readarr.models.download_protocol import DownloadProtocol
 from readarr.models.edition import Edition
 from readarr.models.edition_lazy_loaded import EditionLazyLoaded
 from readarr.models.edition_list_lazy_loaded import EditionListLazyLoaded
 from readarr.models.edition_resource import EditionResource
@@ -76,18 +77,20 @@
 from readarr.models.file_date_type import FileDateType
 from readarr.models.health_check_result import HealthCheckResult
 from readarr.models.health_resource import HealthResource
 from readarr.models.history_resource import HistoryResource
 from readarr.models.history_resource_paging_resource import HistoryResourcePagingResource
 from readarr.models.host_config_resource import HostConfigResource
 from readarr.models.i_custom_format_specification import ICustomFormatSpecification
+from readarr.models.import_list_bulk_resource import ImportListBulkResource
 from readarr.models.import_list_exclusion_resource import ImportListExclusionResource
 from readarr.models.import_list_monitor_type import ImportListMonitorType
 from readarr.models.import_list_resource import ImportListResource
 from readarr.models.import_list_type import ImportListType
+from readarr.models.indexer_bulk_resource import IndexerBulkResource
 from readarr.models.indexer_config_resource import IndexerConfigResource
 from readarr.models.indexer_resource import IndexerResource
 from readarr.models.iso_country import IsoCountry
 from readarr.models.language_resource import LanguageResource
 from readarr.models.links import Links
 from readarr.models.log_file_resource import LogFileResource
 from readarr.models.log_resource import LogResource
```

### Comparing `readarr-py-0.3.0/readarr/models/add_author_options.py` & `readarr-py-0.4.0/readarr/models/add_author_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/add_book_options.py` & `readarr-py-0.4.0/readarr/models/add_book_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/allow_fingerprinting.py` & `readarr-py-0.4.0/readarr/models/allow_fingerprinting.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/api_info_resource.py` & `readarr-py-0.4.0/readarr/models/api_info_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/apply_tags.py` & `readarr-py-0.4.0/readarr/models/apply_tags.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/authentication_type.py` & `readarr-py-0.4.0/readarr/models/authentication_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author.py` & `readarr-py-0.4.0/readarr/models/author.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_editor_resource.py` & `readarr-py-0.4.0/readarr/models/author_editor_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/author_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_metadata.py` & `readarr-py-0.4.0/readarr/models/author_metadata.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_metadata_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/author_metadata_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_resource.py` & `readarr-py-0.4.0/readarr/models/author_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_statistics_resource.py` & `readarr-py-0.4.0/readarr/models/author_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_status_type.py` & `readarr-py-0.4.0/readarr/models/author_status_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/author_title_info.py` & `readarr-py-0.4.0/readarr/models/author_title_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/backup_resource.py` & `readarr-py-0.4.0/readarr/models/backup_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/backup_type.py` & `readarr-py-0.4.0/readarr/models/backup_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/blocklist_bulk_resource.py` & `readarr-py-0.4.0/readarr/models/blocklist_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/blocklist_resource.py` & `readarr-py-0.4.0/readarr/models/blocklist_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/blocklist_resource_paging_resource.py` & `readarr-py-0.4.0/readarr/models/blocklist_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book.py` & `readarr-py-0.4.0/readarr/models/book.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_add_type.py` & `readarr-py-0.4.0/readarr/models/book_add_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_editor_resource.py` & `readarr-py-0.4.0/readarr/models/book_editor_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_file.py` & `readarr-py-0.4.0/readarr/models/book_file.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_file_list_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/book_file_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_file_list_resource.py` & `readarr-py-0.4.0/readarr/models/book_file_list_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_file_resource.py` & `readarr-py-0.4.0/readarr/models/book_file_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/book_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_list_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/book_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_resource.py` & `readarr-py-0.4.0/readarr/models/book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_resource_paging_resource.py` & `readarr-py-0.4.0/readarr/models/book_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/book_statistics_resource.py` & `readarr-py-0.4.0/readarr/models/book_statistics_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/books_monitored_resource.py` & `readarr-py-0.4.0/readarr/models/books_monitored_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/bookshelf_author_resource.py` & `readarr-py-0.4.0/readarr/models/bookshelf_author_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/bookshelf_resource.py` & `readarr-py-0.4.0/readarr/models/bookshelf_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/certificate_validation_type.py` & `readarr-py-0.4.0/readarr/models/certificate_validation_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/command.py` & `readarr-py-0.4.0/readarr/models/command.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/command_priority.py` & `readarr-py-0.4.0/readarr/models/command_priority.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/command_resource.py` & `readarr-py-0.4.0/readarr/models/command_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/command_status.py` & `readarr-py-0.4.0/readarr/models/command_status.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/command_trigger.py` & `readarr-py-0.4.0/readarr/models/command_trigger.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/custom_filter_resource.py` & `readarr-py-0.4.0/readarr/models/custom_filter_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/custom_format.py` & `readarr-py-0.4.0/readarr/models/custom_format.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/custom_format_resource.py` & `readarr-py-0.4.0/readarr/models/custom_format_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/custom_format_specification_schema.py` & `readarr-py-0.4.0/readarr/models/custom_format_specification_schema.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/database_type.py` & `readarr-py-0.4.0/readarr/models/database_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/delay_profile_resource.py` & `readarr-py-0.4.0/readarr/models/delay_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/development_config_resource.py` & `readarr-py-0.4.0/readarr/models/development_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/disk_space_resource.py` & `readarr-py-0.4.0/readarr/models/disk_space_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/download_client_config_resource.py` & `readarr-py-0.4.0/readarr/models/download_client_config_resource.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,18 +25,16 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     download_client_working_folders: Optional[str]
     enable_completed_download_handling: Optional[bool]
-    remove_completed_downloads: Optional[bool]
     auto_redownload_failed: Optional[bool]
-    remove_failed_downloads: Optional[bool]
-    __properties = ["id", "downloadClientWorkingFolders", "enableCompletedDownloadHandling", "removeCompletedDownloads", "autoRedownloadFailed", "removeFailedDownloads"]
+    __properties = ["id", "downloadClientWorkingFolders", "enableCompletedDownloadHandling", "autoRedownloadFailed"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -76,13 +74,11 @@
         if type(obj) is not dict:
             return DownloadClientConfigResource.parse_obj(obj)
 
         _obj = DownloadClientConfigResource.parse_obj({
             "id": obj.get("id"),
             "download_client_working_folders": obj.get("downloadClientWorkingFolders"),
             "enable_completed_download_handling": obj.get("enableCompletedDownloadHandling"),
-            "remove_completed_downloads": obj.get("removeCompletedDownloads"),
-            "auto_redownload_failed": obj.get("autoRedownloadFailed"),
-            "remove_failed_downloads": obj.get("removeFailedDownloads")
+            "auto_redownload_failed": obj.get("autoRedownloadFailed")
         })
         return _obj
```

### Comparing `readarr-py-0.3.0/readarr/models/download_client_resource.py` & `readarr-py-0.4.0/readarr/models/download_client_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     info_link: Optional[str]
     message: Optional[ProviderMessage]
     tags: Optional[List]
     presets: Optional[List]
     enable: Optional[bool]
     protocol: Optional[DownloadProtocol]
     priority: Optional[int]
-    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enable", "protocol", "priority"]
+    remove_completed_downloads: Optional[bool]
+    remove_failed_downloads: Optional[bool]
+    __properties = ["id", "name", "fields", "implementationName", "implementation", "configContract", "infoLink", "message", "tags", "presets", "enable", "protocol", "priority", "removeCompletedDownloads", "removeFailedDownloads"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -140,11 +142,13 @@
             "config_contract": obj.get("configContract"),
             "info_link": obj.get("infoLink"),
             "message": ProviderMessage.from_dict(obj.get("message")) if obj.get("message") is not None else None,
             "tags": obj.get("tags"),
             "presets": [DownloadClientResource.from_dict(_item) for _item in obj.get("presets")] if obj.get("presets") is not None else None,
             "enable": obj.get("enable"),
             "protocol": obj.get("protocol"),
-            "priority": obj.get("priority")
+            "priority": obj.get("priority"),
+            "remove_completed_downloads": obj.get("removeCompletedDownloads"),
+            "remove_failed_downloads": obj.get("removeFailedDownloads")
         })
         return _obj
```

### Comparing `readarr-py-0.3.0/readarr/models/download_protocol.py` & `readarr-py-0.4.0/readarr/models/download_protocol.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/edition.py` & `readarr-py-0.4.0/readarr/models/edition.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/edition_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/edition_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/edition_list_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/edition_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/edition_resource.py` & `readarr-py-0.4.0/readarr/models/edition_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/entity_history_event_type.py` & `readarr-py-0.4.0/readarr/models/entity_history_event_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/field.py` & `readarr-py-0.4.0/readarr/models/field.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,24 +28,25 @@
     Do not edit the class manually.
     """
     order: Optional[int]
     name: Optional[str]
     label: Optional[str]
     unit: Optional[str]
     help_text: Optional[str]
+    help_text_warning: Optional[str]
     help_link: Optional[str]
     value: Optional[object]
     type: Optional[str]
     advanced: Optional[bool]
     select_options: Optional[List]
     select_options_provider_action: Optional[str]
     section: Optional[str]
     hidden: Optional[str]
     placeholder: Optional[str]
-    __properties = ["order", "name", "label", "unit", "helpText", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "placeholder"]
+    __properties = ["order", "name", "label", "unit", "helpText", "helpTextWarning", "helpLink", "value", "type", "advanced", "selectOptions", "selectOptionsProviderAction", "section", "hidden", "placeholder"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -89,14 +90,18 @@
         if self.unit is None:
             _dict['unit'] = None
 
         # set to None if help_text (nullable) is None
         if self.help_text is None:
             _dict['helpText'] = None
 
+        # set to None if help_text_warning (nullable) is None
+        if self.help_text_warning is None:
+            _dict['helpTextWarning'] = None
+
         # set to None if help_link (nullable) is None
         if self.help_link is None:
             _dict['helpLink'] = None
 
         # set to None if value (nullable) is None
         if self.value is None:
             _dict['value'] = None
@@ -138,14 +143,15 @@
 
         _obj = Field.parse_obj({
             "order": obj.get("order"),
             "name": obj.get("name"),
             "label": obj.get("label"),
             "unit": obj.get("unit"),
             "help_text": obj.get("helpText"),
+            "help_text_warning": obj.get("helpTextWarning"),
             "help_link": obj.get("helpLink"),
             "value": obj.get("value"),
             "type": obj.get("type"),
             "advanced": obj.get("advanced"),
             "select_options": [SelectOption.from_dict(_item) for _item in obj.get("selectOptions")] if obj.get("selectOptions") is not None else None,
             "select_options_provider_action": obj.get("selectOptionsProviderAction"),
             "section": obj.get("section"),
```

### Comparing `readarr-py-0.3.0/readarr/models/file_date_type.py` & `readarr-py-0.4.0/readarr/models/file_date_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/health_check_result.py` & `readarr-py-0.4.0/readarr/models/health_check_result.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/health_resource.py` & `readarr-py-0.4.0/readarr/models/health_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/history_resource.py` & `readarr-py-0.4.0/readarr/models/history_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,22 +33,23 @@
     """
     id: Optional[int]
     book_id: Optional[int]
     author_id: Optional[int]
     source_title: Optional[str]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     quality_cutoff_not_met: Optional[bool]
     var_date: Optional[datetime]
     download_id: Optional[str]
     event_type: Optional[EntityHistoryEventType]
     data: Optional[Dict]
     book: Optional[BookResource]
     author: Optional[AuthorResource]
-    __properties = ["id", "bookId", "authorId", "sourceTitle", "quality", "customFormats", "qualityCutoffNotMet", "date", "downloadId", "eventType", "data", "book", "author"]
+    __properties = ["id", "bookId", "authorId", "sourceTitle", "quality", "customFormats", "customFormatScore", "qualityCutoffNotMet", "date", "downloadId", "eventType", "data", "book", "author"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -119,14 +120,15 @@
         _obj = HistoryResource.parse_obj({
             "id": obj.get("id"),
             "book_id": obj.get("bookId"),
             "author_id": obj.get("authorId"),
             "source_title": obj.get("sourceTitle"),
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "quality_cutoff_not_met": obj.get("qualityCutoffNotMet"),
             "var_date": obj.get("date"),
             "download_id": obj.get("downloadId"),
             "event_type": obj.get("eventType"),
             "data": obj.get("data"),
             "book": BookResource.from_dict(obj.get("book")) if obj.get("book") is not None else None,
             "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None
```

### Comparing `readarr-py-0.3.0/readarr/models/history_resource_paging_resource.py` & `readarr-py-0.4.0/readarr/models/history_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/host_config_resource.py` & `readarr-py-0.4.0/readarr/models/host_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/i_custom_format_specification.py` & `readarr-py-0.4.0/readarr/models/i_custom_format_specification.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/import_list_exclusion_resource.py` & `readarr-py-0.4.0/readarr/models/import_list_exclusion_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/import_list_monitor_type.py` & `readarr-py-0.4.0/readarr/models/import_list_monitor_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/import_list_resource.py` & `readarr-py-0.4.0/readarr/models/import_list_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/import_list_type.py` & `readarr-py-0.4.0/readarr/models/import_list_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/indexer_config_resource.py` & `readarr-py-0.4.0/readarr/models/indexer_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/indexer_resource.py` & `readarr-py-0.4.0/readarr/models/indexer_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/iso_country.py` & `readarr-py-0.4.0/readarr/models/iso_country.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/language_resource.py` & `readarr-py-0.4.0/readarr/models/language_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/links.py` & `readarr-py-0.4.0/readarr/models/links.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/log_file_resource.py` & `readarr-py-0.4.0/readarr/models/log_file_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/log_resource.py` & `readarr-py-0.4.0/readarr/models/log_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/log_resource_paging_resource.py` & `readarr-py-0.4.0/readarr/models/log_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/manual_import_resource.py` & `readarr-py-0.4.0/readarr/models/manual_import_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/manual_import_update_resource.py` & `readarr-py-0.4.0/readarr/models/manual_import_update_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/media_cover.py` & `readarr-py-0.4.0/readarr/models/media_cover.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/media_cover_types.py` & `readarr-py-0.4.0/readarr/models/media_cover_types.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,8 +35,9 @@
     BANNER = 'banner'
     FANART = 'fanart'
     SCREENSHOT = 'screenshot'
     HEADSHOT = 'headshot'
     COVER = 'cover'
     DISC = 'disc'
     LOGO = 'logo'
+    CLEARLOGO = 'clearlogo'
```

### Comparing `readarr-py-0.3.0/readarr/models/media_info_model.py` & `readarr-py-0.4.0/readarr/models/media_info_model.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/media_info_resource.py` & `readarr-py-0.4.0/readarr/models/media_info_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/media_management_config_resource.py` & `readarr-py-0.4.0/readarr/models/media_management_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/metadata_profile.py` & `readarr-py-0.4.0/readarr/models/metadata_profile.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional, Union
+from typing import List, Optional, Union
 from pydantic import BaseModel
 
 class MetadataProfile(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -31,15 +31,15 @@
     min_popularity: Optional[float]
     skip_missing_date: Optional[bool]
     skip_missing_isbn: Optional[bool]
     skip_parts_and_sets: Optional[bool]
     skip_series_secondary: Optional[bool]
     allowed_languages: Optional[str]
     min_pages: Optional[int]
-    ignored: Optional[str]
+    ignored: Optional[List]
     __properties = ["id", "name", "minPopularity", "skipMissingDate", "skipMissingIsbn", "skipPartsAndSets", "skipSeriesSecondary", "allowedLanguages", "minPages", "ignored"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
```

### Comparing `readarr-py-0.3.0/readarr/models/metadata_profile_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/metadata_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/metadata_profile_resource.py` & `readarr-py-0.4.0/readarr/models/metadata_profile_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from __future__ import annotations
 from inspect import getfullargspec
 import pprint
 import re  # noqa: F401
 import json
 
 
-from typing import Optional, Union
+from typing import List, Optional, Union
 from pydantic import BaseModel
 
 class MetadataProfileResource(BaseModel):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
@@ -31,15 +31,15 @@
     min_popularity: Optional[float]
     skip_missing_date: Optional[bool]
     skip_missing_isbn: Optional[bool]
     skip_parts_and_sets: Optional[bool]
     skip_series_secondary: Optional[bool]
     allowed_languages: Optional[str]
     min_pages: Optional[int]
-    ignored: Optional[str]
+    ignored: Optional[List]
     __properties = ["id", "name", "minPopularity", "skipMissingDate", "skipMissingIsbn", "skipPartsAndSets", "skipSeriesSecondary", "allowedLanguages", "minPages", "ignored"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
```

### Comparing `readarr-py-0.3.0/readarr/models/metadata_provider_config_resource.py` & `readarr-py-0.4.0/readarr/models/metadata_provider_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/metadata_resource.py` & `readarr-py-0.4.0/readarr/models/metadata_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/monitor_types.py` & `readarr-py-0.4.0/readarr/models/monitor_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/monitoring_options.py` & `readarr-py-0.4.0/readarr/models/monitoring_options.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/naming_config_resource.py` & `readarr-py-0.4.0/readarr/models/naming_config_resource.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,23 +25,24 @@
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
     """
     id: Optional[int]
     rename_books: Optional[bool]
     replace_illegal_characters: Optional[bool]
+    colon_replacement_format: Optional[int]
     standard_book_format: Optional[str]
     author_folder_format: Optional[str]
     include_author_name: Optional[bool]
     include_book_title: Optional[bool]
     include_quality: Optional[bool]
     replace_spaces: Optional[bool]
     separator: Optional[str]
     number_style: Optional[str]
-    __properties = ["id", "renameBooks", "replaceIllegalCharacters", "standardBookFormat", "authorFolderFormat", "includeAuthorName", "includeBookTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
+    __properties = ["id", "renameBooks", "replaceIllegalCharacters", "colonReplacementFormat", "standardBookFormat", "authorFolderFormat", "includeAuthorName", "includeBookTitle", "includeQuality", "replaceSpaces", "separator", "numberStyle"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -93,14 +94,15 @@
         if type(obj) is not dict:
             return NamingConfigResource.parse_obj(obj)
 
         _obj = NamingConfigResource.parse_obj({
             "id": obj.get("id"),
             "rename_books": obj.get("renameBooks"),
             "replace_illegal_characters": obj.get("replaceIllegalCharacters"),
+            "colon_replacement_format": obj.get("colonReplacementFormat"),
             "standard_book_format": obj.get("standardBookFormat"),
             "author_folder_format": obj.get("authorFolderFormat"),
             "include_author_name": obj.get("includeAuthorName"),
             "include_book_title": obj.get("includeBookTitle"),
             "include_quality": obj.get("includeQuality"),
             "replace_spaces": obj.get("replaceSpaces"),
             "separator": obj.get("separator"),
```

### Comparing `readarr-py-0.3.0/readarr/models/new_item_monitor_types.py` & `readarr-py-0.4.0/readarr/models/new_item_monitor_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/notification_resource.py` & `readarr-py-0.4.0/readarr/models/notification_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/paging_resource_filter.py` & `readarr-py-0.4.0/readarr/models/paging_resource_filter.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/parse_resource.py` & `readarr-py-0.4.0/readarr/models/parse_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/parsed_book_info.py` & `readarr-py-0.4.0/readarr/models/parsed_book_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/parsed_track_info.py` & `readarr-py-0.4.0/readarr/models/parsed_track_info.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/ping_resource.py` & `readarr-py-0.4.0/readarr/models/ping_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/profile_format_item.py` & `readarr-py-0.4.0/readarr/models/profile_format_item.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/profile_format_item_resource.py` & `readarr-py-0.4.0/readarr/models/profile_format_item_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/proper_download_types.py` & `readarr-py-0.4.0/readarr/models/proper_download_types.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/provider_message.py` & `readarr-py-0.4.0/readarr/models/provider_message.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/provider_message_type.py` & `readarr-py-0.4.0/readarr/models/provider_message_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/proxy_type.py` & `readarr-py-0.4.0/readarr/models/proxy_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality.py` & `readarr-py-0.4.0/readarr/models/quality.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_definition_resource.py` & `readarr-py-0.4.0/readarr/models/quality_definition_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_model.py` & `readarr-py-0.4.0/readarr/models/quality_model.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_profile.py` & `readarr-py-0.4.0/readarr/models/quality_profile.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_profile_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/quality_profile_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_profile_quality_item.py` & `readarr-py-0.4.0/readarr/models/quality_profile_quality_item.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_profile_quality_item_resource.py` & `readarr-py-0.4.0/readarr/models/quality_profile_quality_item_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/quality_profile_resource.py` & `readarr-py-0.4.0/readarr/models/quality_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/queue_bulk_resource.py` & `readarr-py-0.4.0/readarr/models/queue_bulk_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/queue_resource.py` & `readarr-py-0.4.0/readarr/models/queue_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     id: Optional[int]
     author_id: Optional[int]
     book_id: Optional[int]
     author: Optional[AuthorResource]
     book: Optional[BookResource]
     quality: Optional[QualityModel]
     custom_formats: Optional[List]
+    custom_format_score: Optional[int]
     size: Optional[float]
     title: Optional[str]
     sizeleft: Optional[float]
     timeleft: Optional[str]
     estimated_completion_time: Optional[datetime]
     status: Optional[str]
     tracked_download_status: Optional[TrackedDownloadStatus]
@@ -53,15 +54,15 @@
     error_message: Optional[str]
     download_id: Optional[str]
     protocol: Optional[DownloadProtocol]
     download_client: Optional[str]
     indexer: Optional[str]
     output_path: Optional[str]
     download_forced: Optional[bool]
-    __properties = ["id", "authorId", "bookId", "author", "book", "quality", "customFormats", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
+    __properties = ["id", "authorId", "bookId", "author", "book", "quality", "customFormats", "customFormatScore", "size", "title", "sizeleft", "timeleft", "estimatedCompletionTime", "status", "trackedDownloadStatus", "trackedDownloadState", "statusMessages", "errorMessage", "downloadId", "protocol", "downloadClient", "indexer", "outputPath", "downloadForced"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -172,14 +173,15 @@
             "id": obj.get("id"),
             "author_id": obj.get("authorId"),
             "book_id": obj.get("bookId"),
             "author": AuthorResource.from_dict(obj.get("author")) if obj.get("author") is not None else None,
             "book": BookResource.from_dict(obj.get("book")) if obj.get("book") is not None else None,
             "quality": QualityModel.from_dict(obj.get("quality")) if obj.get("quality") is not None else None,
             "custom_formats": [CustomFormatResource.from_dict(_item) for _item in obj.get("customFormats")] if obj.get("customFormats") is not None else None,
+            "custom_format_score": obj.get("customFormatScore"),
             "size": obj.get("size"),
             "title": obj.get("title"),
             "sizeleft": obj.get("sizeleft"),
             "timeleft": obj.get("timeleft"),
             "estimated_completion_time": obj.get("estimatedCompletionTime"),
             "status": obj.get("status"),
             "tracked_download_status": obj.get("trackedDownloadStatus"),
```

### Comparing `readarr-py-0.3.0/readarr/models/queue_resource_paging_resource.py` & `readarr-py-0.4.0/readarr/models/queue_resource_paging_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/queue_status_resource.py` & `readarr-py-0.4.0/readarr/models/queue_status_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/ratings.py` & `readarr-py-0.4.0/readarr/models/ratings.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/rejection.py` & `readarr-py-0.4.0/readarr/models/rejection.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/rejection_type.py` & `readarr-py-0.4.0/readarr/models/rejection_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/release_profile_resource.py` & `readarr-py-0.4.0/readarr/models/release_profile_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/release_resource.py` & `readarr-py-0.4.0/readarr/models/release_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/remote_path_mapping_resource.py` & `readarr-py-0.4.0/readarr/models/remote_path_mapping_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/rename_book_resource.py` & `readarr-py-0.4.0/readarr/models/rename_book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/rescan_after_refresh_type.py` & `readarr-py-0.4.0/readarr/models/rescan_after_refresh_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/retag_book_resource.py` & `readarr-py-0.4.0/readarr/models/retag_book_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/revision.py` & `readarr-py-0.4.0/readarr/models/revision.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/root_folder_resource.py` & `readarr-py-0.4.0/readarr/models/root_folder_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/runtime_mode.py` & `readarr-py-0.4.0/readarr/models/runtime_mode.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/select_option.py` & `readarr-py-0.4.0/readarr/models/select_option.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series.py` & `readarr-py-0.4.0/readarr/models/series.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_book_link.py` & `readarr-py-0.4.0/readarr/models/series_book_link.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_book_link_list_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/series_book_link_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_book_link_resource.py` & `readarr-py-0.4.0/readarr/models/series_book_link_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/series_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_list_lazy_loaded.py` & `readarr-py-0.4.0/readarr/models/series_list_lazy_loaded.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/series_resource.py` & `readarr-py-0.4.0/readarr/models/series_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/sort_direction.py` & `readarr-py-0.4.0/readarr/models/sort_direction.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/system_resource.py` & `readarr-py-0.4.0/readarr/models/system_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/tag_details_resource.py` & `readarr-py-0.4.0/readarr/models/tag_details_resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,17 @@
     id: Optional[int]
     label: Optional[str]
     delay_profile_ids: Optional[List]
     import_list_ids: Optional[List]
     notification_ids: Optional[List]
     restriction_ids: Optional[List]
     indexer_ids: Optional[List]
+    download_client_ids: Optional[List]
     author_ids: Optional[List]
-    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "authorIds"]
+    __properties = ["id", "label", "delayProfileIds", "importListIds", "notificationIds", "restrictionIds", "indexerIds", "downloadClientIds", "authorIds"]
 
     class Config:
         allow_population_by_field_name = True
         validate_assignment = True
         alias_generator = lambda x: x.split("_")[0] + "".join(word.capitalize() for word in x.split("_")[1:])
 
     def __getitem__(self, item):
@@ -83,14 +84,18 @@
         if self.restriction_ids is None:
             _dict['restrictionIds'] = None
 
         # set to None if indexer_ids (nullable) is None
         if self.indexer_ids is None:
             _dict['indexerIds'] = None
 
+        # set to None if download_client_ids (nullable) is None
+        if self.download_client_ids is None:
+            _dict['downloadClientIds'] = None
+
         # set to None if author_ids (nullable) is None
         if self.author_ids is None:
             _dict['authorIds'] = None
 
         return _dict
 
     @classmethod
@@ -106,11 +111,12 @@
             "id": obj.get("id"),
             "label": obj.get("label"),
             "delay_profile_ids": obj.get("delayProfileIds"),
             "import_list_ids": obj.get("importListIds"),
             "notification_ids": obj.get("notificationIds"),
             "restriction_ids": obj.get("restrictionIds"),
             "indexer_ids": obj.get("indexerIds"),
+            "download_client_ids": obj.get("downloadClientIds"),
             "author_ids": obj.get("authorIds")
         })
         return _obj
```

### Comparing `readarr-py-0.3.0/readarr/models/tag_difference.py` & `readarr-py-0.4.0/readarr/models/tag_difference.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/tag_resource.py` & `readarr-py-0.4.0/readarr/models/tag_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/task_resource.py` & `readarr-py-0.4.0/readarr/models/task_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/tracked_download_state.py` & `readarr-py-0.4.0/readarr/models/tracked_download_state.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/tracked_download_status.py` & `readarr-py-0.4.0/readarr/models/tracked_download_status.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/tracked_download_status_message.py` & `readarr-py-0.4.0/readarr/models/tracked_download_status_message.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/ui_config_resource.py` & `readarr-py-0.4.0/readarr/models/ui_config_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/update_changes.py` & `readarr-py-0.4.0/readarr/models/update_changes.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/update_mechanism.py` & `readarr-py-0.4.0/readarr/models/update_mechanism.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/update_resource.py` & `readarr-py-0.4.0/readarr/models/update_resource.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/write_audio_tags_type.py` & `readarr-py-0.4.0/readarr/models/write_audio_tags_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/models/write_book_tags_type.py` & `readarr-py-0.4.0/readarr/models/write_book_tags_type.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr/rest.py` & `readarr-py-0.4.0/readarr/rest.py`

 * *Files identical despite different names*

### Comparing `readarr-py-0.3.0/readarr_py.egg-info/PKG-INFO` & `readarr-py-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-Metadata-Version: 2.1
-Name: readarr-py
-Version: 0.3.0
-Summary: Readarr API wrapper
-Project-URL: Homepage, https://github.com/devopsarr/readarr-py
-Project-URL: Bug Tracker, https://github.com/devopsarr/readarr-py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # readarr-py
 Readarr API docs
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
 [comment]: # (x-release-please-start-version)
-- Package version: 0.3.0
+- Package version: 0.4.0
 
 [comment]: # (x-release-please-end)
 - API version: 1.0.0
 
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 
 ## Requirements.
@@ -177,56 +164,61 @@
 *DevelopmentConfigApi* | [**get_development_config**](docs/DevelopmentConfigApi.md#get_development_config) | **GET** /api/v1/config/development | 
 *DevelopmentConfigApi* | [**get_development_config_by_id**](docs/DevelopmentConfigApi.md#get_development_config_by_id) | **GET** /api/v1/config/development/{id} | 
 *DevelopmentConfigApi* | [**update_development_config**](docs/DevelopmentConfigApi.md#update_development_config) | **PUT** /api/v1/config/development/{id} | 
 *DiskSpaceApi* | [**list_disk_space**](docs/DiskSpaceApi.md#list_disk_space) | **GET** /api/v1/diskspace | 
 *DownloadClientApi* | [**create_download_client**](docs/DownloadClientApi.md#create_download_client) | **POST** /api/v1/downloadclient | 
 *DownloadClientApi* | [**create_download_client_action_by_name**](docs/DownloadClientApi.md#create_download_client_action_by_name) | **POST** /api/v1/downloadclient/action/{name} | 
 *DownloadClientApi* | [**delete_download_client**](docs/DownloadClientApi.md#delete_download_client) | **DELETE** /api/v1/downloadclient/{id} | 
+*DownloadClientApi* | [**delete_download_client_bulk**](docs/DownloadClientApi.md#delete_download_client_bulk) | **DELETE** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**get_download_client_by_id**](docs/DownloadClientApi.md#get_download_client_by_id) | **GET** /api/v1/downloadclient/{id} | 
 *DownloadClientApi* | [**list_download_client**](docs/DownloadClientApi.md#list_download_client) | **GET** /api/v1/downloadclient | 
 *DownloadClientApi* | [**list_download_client_schema**](docs/DownloadClientApi.md#list_download_client_schema) | **GET** /api/v1/downloadclient/schema | 
+*DownloadClientApi* | [**put_download_client_bulk**](docs/DownloadClientApi.md#put_download_client_bulk) | **PUT** /api/v1/downloadclient/bulk | 
 *DownloadClientApi* | [**test_download_client**](docs/DownloadClientApi.md#test_download_client) | **POST** /api/v1/downloadclient/test | 
 *DownloadClientApi* | [**testall_download_client**](docs/DownloadClientApi.md#testall_download_client) | **POST** /api/v1/downloadclient/testall | 
 *DownloadClientApi* | [**update_download_client**](docs/DownloadClientApi.md#update_download_client) | **PUT** /api/v1/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**get_download_client_config**](docs/DownloadClientConfigApi.md#get_download_client_config) | **GET** /api/v1/config/downloadclient | 
 *DownloadClientConfigApi* | [**get_download_client_config_by_id**](docs/DownloadClientConfigApi.md#get_download_client_config_by_id) | **GET** /api/v1/config/downloadclient/{id} | 
 *DownloadClientConfigApi* | [**update_download_client_config**](docs/DownloadClientConfigApi.md#update_download_client_config) | **PUT** /api/v1/config/downloadclient/{id} | 
 *EditionApi* | [**list_edition**](docs/EditionApi.md#list_edition) | **GET** /api/v1/edition | 
 *FileSystemApi* | [**get_file_system**](docs/FileSystemApi.md#get_file_system) | **GET** /api/v1/filesystem | 
 *FileSystemApi* | [**get_file_system_mediafiles**](docs/FileSystemApi.md#get_file_system_mediafiles) | **GET** /api/v1/filesystem/mediafiles | 
 *FileSystemApi* | [**get_file_system_type**](docs/FileSystemApi.md#get_file_system_type) | **GET** /api/v1/filesystem/type | 
-*HealthApi* | [**get_health_by_id**](docs/HealthApi.md#get_health_by_id) | **GET** /api/v1/health/{id} | 
 *HealthApi* | [**list_health**](docs/HealthApi.md#list_health) | **GET** /api/v1/health | 
 *HistoryApi* | [**create_history_failed_by_id**](docs/HistoryApi.md#create_history_failed_by_id) | **POST** /api/v1/history/failed/{id} | 
 *HistoryApi* | [**get_history**](docs/HistoryApi.md#get_history) | **GET** /api/v1/history | 
 *HistoryApi* | [**list_history_author**](docs/HistoryApi.md#list_history_author) | **GET** /api/v1/history/author | 
 *HistoryApi* | [**list_history_since**](docs/HistoryApi.md#list_history_since) | **GET** /api/v1/history/since | 
 *HostConfigApi* | [**get_host_config**](docs/HostConfigApi.md#get_host_config) | **GET** /api/v1/config/host | 
 *HostConfigApi* | [**get_host_config_by_id**](docs/HostConfigApi.md#get_host_config_by_id) | **GET** /api/v1/config/host/{id} | 
 *HostConfigApi* | [**update_host_config**](docs/HostConfigApi.md#update_host_config) | **PUT** /api/v1/config/host/{id} | 
 *ImportListApi* | [**create_import_list**](docs/ImportListApi.md#create_import_list) | **POST** /api/v1/importlist | 
 *ImportListApi* | [**create_import_list_action_by_name**](docs/ImportListApi.md#create_import_list_action_by_name) | **POST** /api/v1/importlist/action/{name} | 
 *ImportListApi* | [**delete_import_list**](docs/ImportListApi.md#delete_import_list) | **DELETE** /api/v1/importlist/{id} | 
+*ImportListApi* | [**delete_import_list_bulk**](docs/ImportListApi.md#delete_import_list_bulk) | **DELETE** /api/v1/importlist/bulk | 
 *ImportListApi* | [**get_import_list_by_id**](docs/ImportListApi.md#get_import_list_by_id) | **GET** /api/v1/importlist/{id} | 
 *ImportListApi* | [**list_import_list**](docs/ImportListApi.md#list_import_list) | **GET** /api/v1/importlist | 
 *ImportListApi* | [**list_import_list_schema**](docs/ImportListApi.md#list_import_list_schema) | **GET** /api/v1/importlist/schema | 
+*ImportListApi* | [**put_import_list_bulk**](docs/ImportListApi.md#put_import_list_bulk) | **PUT** /api/v1/importlist/bulk | 
 *ImportListApi* | [**test_import_list**](docs/ImportListApi.md#test_import_list) | **POST** /api/v1/importlist/test | 
 *ImportListApi* | [**testall_import_list**](docs/ImportListApi.md#testall_import_list) | **POST** /api/v1/importlist/testall | 
 *ImportListApi* | [**update_import_list**](docs/ImportListApi.md#update_import_list) | **PUT** /api/v1/importlist/{id} | 
 *ImportListExclusionApi* | [**create_import_list_exclusion**](docs/ImportListExclusionApi.md#create_import_list_exclusion) | **POST** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**delete_import_list_exclusion**](docs/ImportListExclusionApi.md#delete_import_list_exclusion) | **DELETE** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**get_import_list_exclusion_by_id**](docs/ImportListExclusionApi.md#get_import_list_exclusion_by_id) | **GET** /api/v1/importlistexclusion/{id} | 
 *ImportListExclusionApi* | [**list_import_list_exclusion**](docs/ImportListExclusionApi.md#list_import_list_exclusion) | **GET** /api/v1/importlistexclusion | 
 *ImportListExclusionApi* | [**update_import_list_exclusion**](docs/ImportListExclusionApi.md#update_import_list_exclusion) | **PUT** /api/v1/importlistexclusion/{id} | 
 *IndexerApi* | [**create_indexer**](docs/IndexerApi.md#create_indexer) | **POST** /api/v1/indexer | 
 *IndexerApi* | [**create_indexer_action_by_name**](docs/IndexerApi.md#create_indexer_action_by_name) | **POST** /api/v1/indexer/action/{name} | 
 *IndexerApi* | [**delete_indexer**](docs/IndexerApi.md#delete_indexer) | **DELETE** /api/v1/indexer/{id} | 
+*IndexerApi* | [**delete_indexer_bulk**](docs/IndexerApi.md#delete_indexer_bulk) | **DELETE** /api/v1/indexer/bulk | 
 *IndexerApi* | [**get_indexer_by_id**](docs/IndexerApi.md#get_indexer_by_id) | **GET** /api/v1/indexer/{id} | 
 *IndexerApi* | [**list_indexer**](docs/IndexerApi.md#list_indexer) | **GET** /api/v1/indexer | 
 *IndexerApi* | [**list_indexer_schema**](docs/IndexerApi.md#list_indexer_schema) | **GET** /api/v1/indexer/schema | 
+*IndexerApi* | [**put_indexer_bulk**](docs/IndexerApi.md#put_indexer_bulk) | **PUT** /api/v1/indexer/bulk | 
 *IndexerApi* | [**test_indexer**](docs/IndexerApi.md#test_indexer) | **POST** /api/v1/indexer/test | 
 *IndexerApi* | [**testall_indexer**](docs/IndexerApi.md#testall_indexer) | **POST** /api/v1/indexer/testall | 
 *IndexerApi* | [**update_indexer**](docs/IndexerApi.md#update_indexer) | **PUT** /api/v1/indexer/{id} | 
 *IndexerConfigApi* | [**get_indexer_config**](docs/IndexerConfigApi.md#get_indexer_config) | **GET** /api/v1/config/indexer | 
 *IndexerConfigApi* | [**get_indexer_config_by_id**](docs/IndexerConfigApi.md#get_indexer_config_by_id) | **GET** /api/v1/config/indexer/{id} | 
 *IndexerConfigApi* | [**update_indexer_config**](docs/IndexerConfigApi.md#update_indexer_config) | **PUT** /api/v1/config/indexer/{id} | 
 *InitializeJsApi* | [**get_initialize_js**](docs/InitializeJsApi.md#get_initialize_js) | **GET** /initialize.js | 
@@ -287,31 +279,26 @@
 *QualityProfileApi* | [**get_quality_profile_by_id**](docs/QualityProfileApi.md#get_quality_profile_by_id) | **GET** /api/v1/qualityprofile/{id} | 
 *QualityProfileApi* | [**list_quality_profile**](docs/QualityProfileApi.md#list_quality_profile) | **GET** /api/v1/qualityprofile | 
 *QualityProfileApi* | [**update_quality_profile**](docs/QualityProfileApi.md#update_quality_profile) | **PUT** /api/v1/qualityprofile/{id} | 
 *QualityProfileSchemaApi* | [**get_qualityprofile_schema**](docs/QualityProfileSchemaApi.md#get_qualityprofile_schema) | **GET** /api/v1/qualityprofile/schema | 
 *QueueApi* | [**delete_queue**](docs/QueueApi.md#delete_queue) | **DELETE** /api/v1/queue/{id} | 
 *QueueApi* | [**delete_queue_bulk**](docs/QueueApi.md#delete_queue_bulk) | **DELETE** /api/v1/queue/bulk | 
 *QueueApi* | [**get_queue**](docs/QueueApi.md#get_queue) | **GET** /api/v1/queue | 
-*QueueApi* | [**get_queue_by_id**](docs/QueueApi.md#get_queue_by_id) | **GET** /api/v1/queue/{id} | 
 *QueueActionApi* | [**create_queue_grab_bulk**](docs/QueueActionApi.md#create_queue_grab_bulk) | **POST** /api/v1/queue/grab/bulk | 
 *QueueActionApi* | [**create_queue_grab_by_id**](docs/QueueActionApi.md#create_queue_grab_by_id) | **POST** /api/v1/queue/grab/{id} | 
-*QueueDetailsApi* | [**get_queue_details_by_id**](docs/QueueDetailsApi.md#get_queue_details_by_id) | **GET** /api/v1/queue/details/{id} | 
 *QueueDetailsApi* | [**list_queue_details**](docs/QueueDetailsApi.md#list_queue_details) | **GET** /api/v1/queue/details | 
 *QueueStatusApi* | [**get_queue_status**](docs/QueueStatusApi.md#get_queue_status) | **GET** /api/v1/queue/status | 
-*QueueStatusApi* | [**get_queue_status_by_id**](docs/QueueStatusApi.md#get_queue_status_by_id) | **GET** /api/v1/queue/status/{id} | 
 *ReleaseApi* | [**create_release**](docs/ReleaseApi.md#create_release) | **POST** /api/v1/release | 
-*ReleaseApi* | [**get_release_by_id**](docs/ReleaseApi.md#get_release_by_id) | **GET** /api/v1/release/{id} | 
 *ReleaseApi* | [**list_release**](docs/ReleaseApi.md#list_release) | **GET** /api/v1/release | 
 *ReleaseProfileApi* | [**create_release_profile**](docs/ReleaseProfileApi.md#create_release_profile) | **POST** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**delete_release_profile**](docs/ReleaseProfileApi.md#delete_release_profile) | **DELETE** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**get_release_profile_by_id**](docs/ReleaseProfileApi.md#get_release_profile_by_id) | **GET** /api/v1/releaseprofile/{id} | 
 *ReleaseProfileApi* | [**list_release_profile**](docs/ReleaseProfileApi.md#list_release_profile) | **GET** /api/v1/releaseprofile | 
 *ReleaseProfileApi* | [**update_release_profile**](docs/ReleaseProfileApi.md#update_release_profile) | **PUT** /api/v1/releaseprofile/{id} | 
 *ReleasePushApi* | [**create_release_push**](docs/ReleasePushApi.md#create_release_push) | **POST** /api/v1/release/push | 
-*ReleasePushApi* | [**get_release_push_by_id**](docs/ReleasePushApi.md#get_release_push_by_id) | **GET** /api/v1/release/push/{id} | 
 *RemotePathMappingApi* | [**create_remote_path_mapping**](docs/RemotePathMappingApi.md#create_remote_path_mapping) | **POST** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**delete_remote_path_mapping**](docs/RemotePathMappingApi.md#delete_remote_path_mapping) | **DELETE** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**get_remote_path_mapping_by_id**](docs/RemotePathMappingApi.md#get_remote_path_mapping_by_id) | **GET** /api/v1/remotepathmapping/{id} | 
 *RemotePathMappingApi* | [**list_remote_path_mapping**](docs/RemotePathMappingApi.md#list_remote_path_mapping) | **GET** /api/v1/remotepathmapping | 
 *RemotePathMappingApi* | [**update_remote_path_mapping**](docs/RemotePathMappingApi.md#update_remote_path_mapping) | **PUT** /api/v1/remotepathmapping/{id} | 
 *RenameBookApi* | [**list_rename**](docs/RenameBookApi.md#list_rename) | **GET** /api/v1/rename | 
 *RetagBookApi* | [**list_retag**](docs/RetagBookApi.md#list_retag) | **GET** /api/v1/retag | 
@@ -395,14 +382,15 @@
  - [CustomFormat](docs/CustomFormat.md)
  - [CustomFormatResource](docs/CustomFormatResource.md)
  - [CustomFormatSpecificationSchema](docs/CustomFormatSpecificationSchema.md)
  - [DatabaseType](docs/DatabaseType.md)
  - [DelayProfileResource](docs/DelayProfileResource.md)
  - [DevelopmentConfigResource](docs/DevelopmentConfigResource.md)
  - [DiskSpaceResource](docs/DiskSpaceResource.md)
+ - [DownloadClientBulkResource](docs/DownloadClientBulkResource.md)
  - [DownloadClientConfigResource](docs/DownloadClientConfigResource.md)
  - [DownloadClientResource](docs/DownloadClientResource.md)
  - [DownloadProtocol](docs/DownloadProtocol.md)
  - [Edition](docs/Edition.md)
  - [EditionLazyLoaded](docs/EditionLazyLoaded.md)
  - [EditionListLazyLoaded](docs/EditionListLazyLoaded.md)
  - [EditionResource](docs/EditionResource.md)
@@ -411,18 +399,20 @@
  - [FileDateType](docs/FileDateType.md)
  - [HealthCheckResult](docs/HealthCheckResult.md)
  - [HealthResource](docs/HealthResource.md)
  - [HistoryResource](docs/HistoryResource.md)
  - [HistoryResourcePagingResource](docs/HistoryResourcePagingResource.md)
  - [HostConfigResource](docs/HostConfigResource.md)
  - [ICustomFormatSpecification](docs/ICustomFormatSpecification.md)
+ - [ImportListBulkResource](docs/ImportListBulkResource.md)
  - [ImportListExclusionResource](docs/ImportListExclusionResource.md)
  - [ImportListMonitorType](docs/ImportListMonitorType.md)
  - [ImportListResource](docs/ImportListResource.md)
  - [ImportListType](docs/ImportListType.md)
+ - [IndexerBulkResource](docs/IndexerBulkResource.md)
  - [IndexerConfigResource](docs/IndexerConfigResource.md)
  - [IndexerResource](docs/IndexerResource.md)
  - [IsoCountry](docs/IsoCountry.md)
  - [LanguageResource](docs/LanguageResource.md)
  - [Links](docs/Links.md)
  - [LogFileResource](docs/LogFileResource.md)
  - [LogResource](docs/LogResource.md)
```

### Comparing `readarr-py-0.3.0/readarr_py.egg-info/SOURCES.txt` & `readarr-py-0.4.0/readarr_py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 readarr/models/custom_format.py
 readarr/models/custom_format_resource.py
 readarr/models/custom_format_specification_schema.py
 readarr/models/database_type.py
 readarr/models/delay_profile_resource.py
 readarr/models/development_config_resource.py
 readarr/models/disk_space_resource.py
+readarr/models/download_client_bulk_resource.py
 readarr/models/download_client_config_resource.py
 readarr/models/download_client_resource.py
 readarr/models/download_protocol.py
 readarr/models/edition.py
 readarr/models/edition_lazy_loaded.py
 readarr/models/edition_list_lazy_loaded.py
 readarr/models/edition_resource.py
@@ -144,18 +145,20 @@
 readarr/models/file_date_type.py
 readarr/models/health_check_result.py
 readarr/models/health_resource.py
 readarr/models/history_resource.py
 readarr/models/history_resource_paging_resource.py
 readarr/models/host_config_resource.py
 readarr/models/i_custom_format_specification.py
+readarr/models/import_list_bulk_resource.py
 readarr/models/import_list_exclusion_resource.py
 readarr/models/import_list_monitor_type.py
 readarr/models/import_list_resource.py
 readarr/models/import_list_type.py
+readarr/models/indexer_bulk_resource.py
 readarr/models/indexer_config_resource.py
 readarr/models/indexer_resource.py
 readarr/models/iso_country.py
 readarr/models/language_resource.py
 readarr/models/links.py
 readarr/models/log_file_resource.py
 readarr/models/log_resource.py
```

