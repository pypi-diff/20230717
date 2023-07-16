# Comparing `tmp/osxphotos-0.60.7.tar.gz` & `tmp/osxphotos-0.60.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.7.tar", last modified: Sat Jul 15 14:32:38 2023, max compression
+gzip compressed data, was "osxphotos-0.60.8.tar", last modified: Sun Jul 16 22:13:16 2023, max compression
```

## Comparing `osxphotos-0.60.7.tar` & `osxphotos-0.60.8.tar`

### file list

```diff
@@ -1,237 +1,238 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.750491 osxphotos-0.60.7/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.7/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.7/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-15 14:32:38.750274 osxphotos-0.60.7/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   226320 2023-07-15 14:32:27.000000 osxphotos-0.60.7/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.7/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.714928 osxphotos-0.60.7/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.7/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15892 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-15 14:32:15.000000 osxphotos-0.60.7/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.7/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.7/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.726683 osxphotos-0.60.7/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.7/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.7/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   108030 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.7/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.7/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.7/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.7/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.7/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.7/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.7/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.727202 osxphotos-0.60.7/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.7/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1477702 2023-07-15 14:32:34.000000 osxphotos-0.60.7/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.7/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.7/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.7/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.7/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    85034 2023-07-15 14:18:05.000000 osxphotos-0.60.7/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.729480 osxphotos-0.60.7/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10395 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   149958 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5460 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8564 2023-04-16 16:05:18.000000 osxphotos-0.60.7/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.7/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-15 14:32:26.000000 osxphotos-0.60.7/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.7/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.7/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.7/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/platform.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.7/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.730713 osxphotos-0.60.7/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.7/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.7/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.7/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.7/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.7/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.7/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.7/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.7/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.7/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.731774 osxphotos-0.60.7/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.7/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.7/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.7/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.7/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.715765 osxphotos-0.60.7/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6499 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-15 14:32:38.000000 osxphotos-0.60.7/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-15 14:32:38.750529 osxphotos-0.60.7/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.7/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.749369 osxphotos-0.60.7/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-15 14:32:38.749619 osxphotos-0.60.7/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.7/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.7/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.7/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.7/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.7/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.7/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.7/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.7/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.7/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.7/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.7/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.7/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.7/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.7/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_photosalbum_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.7/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.7/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.7/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.7/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.7/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.7/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.7/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.7/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.7/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.7/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.7/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.7/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.7/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.7/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.398621 osxphotos-0.60.8/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.8/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.8/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-16 22:13:16.398446 osxphotos-0.60.8/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   226455 2023-07-16 22:13:03.000000 osxphotos-0.60.8/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.8/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.355346 osxphotos-0.60.8/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.8/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17162 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-16 22:09:29.000000 osxphotos-0.60.8/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.8/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.8/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.369259 osxphotos-0.60.8/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.8/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.8/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   108030 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.8/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.8/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.8/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.8/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.8/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.8/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.378770 osxphotos-0.60.8/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.8/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1477940 2023-07-16 22:13:12.000000 osxphotos-0.60.8/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.8/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.8/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.8/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.8/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    85034 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.381563 osxphotos-0.60.8/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10525 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   150076 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5681 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8828 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.8/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-16 22:13:02.000000 osxphotos-0.60.8/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.8/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.8/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.8/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.8/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.383245 osxphotos-0.60.8/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.8/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.8/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.8/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.8/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.8/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.8/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.8/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.384316 osxphotos-0.60.8/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.8/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.360070 osxphotos-0.60.8/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6527 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-16 22:13:16.398661 osxphotos-0.60.8/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.8/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.397793 osxphotos-0.60.8/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.398162 osxphotos-0.60.8/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.8/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.8/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.8/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.8/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.8/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.8/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.8/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.8/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.8/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.8/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.8/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.8/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.8/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.8/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.8/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.8/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.8/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.8/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.8/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48444 2023-07-16 22:09:19.000000 osxphotos-0.60.8/tests/test_sonoma_14_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.8/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.8/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.8/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.8/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.8/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.7/LICENSE` & `osxphotos-0.60.8/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/PKG-INFO` & `osxphotos-0.60.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.7
+Version: 0.60.8
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.7/README.md` & `osxphotos-0.60.8/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,18 +35,20 @@
 
 Tested on Ubuntu Linux and macOS. Many features are only available on macOS.
 
 On Linux, macOS-specific features of the CLI will not be available (these will not be shown in the help output).
 The export and query CLI commands as well as the Python API will work on Linux which enables you to export photos
 from a Photos library on a Linux machine.
 
-Tested on macOS Sierra (10.12.6) through macOS Ventura (13.3). Tested on both x86 and Apple silicon (M1).
+Tested on macOS Sierra (10.12.6) through macOS Ventura (13.4). Tested on both x86 and Apple silicon (M1).
+macOS Sonoma (14.0) is currently supported but is still in alpha testing.
 
 | macOS Version     | macOS name | Photos.app version |
 | ----------------- |------------|:-------------------|
+| 14.0              | Sonoma     | 9.0 ✅ (alpha support) |
 | 13.0 - 13.4       | Ventura    | 8.0 ✅             |
 | 12.0 - 12.6       | Monterey   | 7.0 ✅             |
 | 10.16, 11.0-11.4  | Big Sur    | 6.0 ✅             |
 | 10.15.1 - 10.15.7 | Catalina   | 5.0 ✅             |
 | 10.14.5, 10.14.6  | Mojave     | 4.0 ✅             |
 | 10.13.6           | High Sierra| 3.0 ✅             |
 | 10.12.6           | Sierra     | 2.0 ✅             |
@@ -2114,15 +2116,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.7'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.8'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2601,15 +2603,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.7'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.8'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.7/README.rst` & `osxphotos-0.60.8/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/__init__.py` & `osxphotos-0.60.8/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/_constants.py` & `osxphotos-0.60.8/osxphotos/_constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,88 +19,114 @@
 TIME_DELTA = (datetime(2001, 1, 1, 0, 0) - datetime(1970, 1, 1, 0, 0)).total_seconds()
 
 # which Photos library database versions have been tested
 # Photos 2.0 (10.12.6) == 2622
 # Photos 3.0 (10.13.6) == 3301
 # Photos 4.0 (10.14.5) == 4016
 # Photos 4.0 (10.14.6) == 4025
-# Photos 5.0 (10.15.0) == 6000 or 5001
+# Photos 5.0+ (10.15.0) == 6000 or 5001
 _TESTED_DB_VERSIONS = ["6000", "5001", "4025", "4016", "3301", "2622"]
 
-# database model versions (applies to Photos 5, Photos 6)
+# database model versions (applies to Photos 5+)
 # these come from PLModelVersion key in binary plist in Z_METADATA.Z_PLIST
 # Photos 5 (10.15.1) == 13537
 # Photos 5 (10.15.4, 10.15.5, 10.15.6) == 13703
 # Photos 6 (10.16.0 Beta) == 14104
-_TEST_MODEL_VERSIONS = ["13537", "13703", "14104"]
+# Photos 7 (12.0.1) == 15323
+# Photos 8 (13.0.0) == 16320
+# Photos 9 (14.0.0 dev preview) = 17120
+_TEST_MODEL_VERSIONS = ["13537", "13703", "14104", "15323", "16320", "17120"]
 
 _PHOTOS_2_VERSION = "2622"
 
 # only version 3 - 4 have RKVersion.selfPortrait
 _PHOTOS_3_VERSION = "3301"
 
 # versions 5.0 and later have a different database structure
-_PHOTOS_4_VERSION = "4025"  # latest Mojove version on 10.14.6
+_PHOTOS_4_VERSION = "4025"  # latest Mojave version on 10.14.6
 _PHOTOS_5_VERSION = "5000"  # I've seen both 5001 and 6000.  6000 is most common on Catalina and up but there are some version 5001 database in the wild
 
 # Ranges for model version by Photos version
 _PHOTOS_5_MODEL_VERSION = [13000, 13999]
 _PHOTOS_6_MODEL_VERSION = [14000, 14999]
 _PHOTOS_7_MODEL_VERSION = [15000, 15999]  # Dev preview: 15134, 12.1: 15331
 _PHOTOS_8_MODEL_VERSION = [16000, 16999]  # Ventura dev preview: 16119
+_PHOTOS_9_MODEL_VERSION = [17000, 17999]  # Sonoma dev preview: 17120
 
-# some table names differ between Photos 5 and Photos 6
+# some table names differ between Photos 5 and later versions
 _DB_TABLE_NAMES = {
     5: {
         "ASSET": "ZGENERICASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_37KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_34ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_34ASSETS",
         "IMPORT_FOK": "ZGENERICASSET.Z_FOK_IMPORTSESSION",
         "DEPTH_STATE": "ZGENERICASSET.ZDEPTHSTATES",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER",
         "ASSET_ALBUM_JOIN": "Z_26ASSETS.Z_26ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_26ASSETS",
         "HDR_TYPE": "ZCUSTOMRENDEREDVALUE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     6: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_36KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER",
         "ASSET_ALBUM_JOIN": "Z_26ASSETS.Z_26ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_26ASSETS",
         "HDR_TYPE": "ZCUSTOMRENDEREDVALUE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     7: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_38KEYWORDS",
         "ALBUM_JOIN": "Z_27ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_27ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
         "ASSET_ALBUM_JOIN": "Z_27ASSETS.Z_27ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_27ASSETS",
         "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     8: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_40KEYWORDS",
         "ALBUM_JOIN": "Z_28ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_28ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
         "ASSET_ALBUM_JOIN": "Z_28ASSETS.Z_28ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_28ASSETS",
         "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
+    },
+    9: {
+        "ASSET": "ZASSET",
+        "KEYWORD_JOIN": "Z_1KEYWORDS.Z_40KEYWORDS",
+        "ALBUM_JOIN": "Z_28ASSETS.Z_3ASSETS",
+        "ALBUM_SORT_ORDER": "Z_28ASSETS.Z_FOK_3ASSETS",
+        "IMPORT_FOK": "null",
+        "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
+        "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
+        "ASSET_ALBUM_JOIN": "Z_28ASSETS.Z_28ALBUMS",
+        "ASSET_ALBUM_TABLE": "Z_28ASSETS",
+        "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSONFORFACE",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSETFORFACE",
     },
 }
 
 # which version operating systems have been tested
 _TESTED_OS_VERSIONS = [
     ("10", "12"),
     ("10", "13"),
@@ -123,14 +149,15 @@
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
     ("13", "3"),
     ("13", "4"),
+    ("14", "0"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

### Comparing `osxphotos-0.60.7/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.8/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/albuminfo.py` & `osxphotos-0.60.8/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/__init__.py` & `osxphotos-0.60.8/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/about.py` & `osxphotos-0.60.8/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/add_locations.py` & `osxphotos-0.60.8/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/albums.py` & `osxphotos-0.60.8/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.8/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/cli.py` & `osxphotos-0.60.8/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.8/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/cli_params.py` & `osxphotos-0.60.8/osxphotos/cli/cli_params.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.8/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/color_themes.py` & `osxphotos-0.60.8/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/common.py` & `osxphotos-0.60.8/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/darkmode.py` & `osxphotos-0.60.8/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.8/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/docs.py` & `osxphotos-0.60.8/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/dump.py` & `osxphotos-0.60.8/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.8/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/export.py` & `osxphotos-0.60.8/osxphotos/cli/export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/exportdb.py` & `osxphotos-0.60.8/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/grep.py` & `osxphotos-0.60.8/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/help.py` & `osxphotos-0.60.8/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/import_cli.py` & `osxphotos-0.60.8/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/info.py` & `osxphotos-0.60.8/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.8/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/keywords.py` & `osxphotos-0.60.8/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/kvstore.py` & `osxphotos-0.60.8/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/labels.py` & `osxphotos-0.60.8/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/list.py` & `osxphotos-0.60.8/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/orphans.py` & `osxphotos-0.60.8/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/param_types.py` & `osxphotos-0.60.8/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/persons.py` & `osxphotos-0.60.8/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.8/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/places.py` & `osxphotos-0.60.8/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.8/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/query.py` & `osxphotos-0.60.8/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/repl.py` & `osxphotos-0.60.8/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/report_writer.py` & `osxphotos-0.60.8/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.8/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/show_command.py` & `osxphotos-0.60.8/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.8/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/sync.py` & `osxphotos-0.60.8/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/sync_results.py` & `osxphotos-0.60.8/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/theme.py` & `osxphotos-0.60.8/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/timewarp.py` & `osxphotos-0.60.8/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/tutorial.py` & `osxphotos-0.60.8/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/uuid.py` & `osxphotos-0.60.8/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/verbose.py` & `osxphotos-0.60.8/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/cli/version.py` & `osxphotos-0.60.8/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/compare_exif.py` & `osxphotos-0.60.8/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/configoptions.py` & `osxphotos-0.60.8/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/crash_reporter.py` & `osxphotos-0.60.8/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/datetime_formatter.py` & `osxphotos-0.60.8/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/datetime_utils.py` & `osxphotos-0.60.8/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/debug.py` & `osxphotos-0.60.8/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/docs/docs.zip` & `osxphotos-0.60.8/osxphotos/docs/docs.zip`

 * *Files 11% similar despite different names*

#### zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1477702 bytes, number of entries: 99
+Zip file size: 1477940 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jul-15 14:32 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jul-16 22:13 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   333770 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
@@ -15,87 +15,87 @@
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
 -rw-r--r--  3.0 unx   314708 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   526465 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx   527258 tx defN 23-Jul-16 22:13 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    99009 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
 -rw-r--r--  3.0 unx    61579 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
--rw-r--r--  3.0 unx    61830 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/_constants.html
+-rw-r--r--  3.0 unx    66040 tx defN 23-Jul-16 22:13 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jul-15 14:32 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jul-16 22:13 docs/_sources/template_help.rst.txt
 -rw-r--r--  3.0 unx    31240 tx defN 21-Apr-26 18:30 docs/_sources/tutorial.md.txt
 -rw-r--r--  3.0 unx       52 tx defN 21-Jan-24 17:13 docs/_sources/modules.rst.txt
 -rw-r--r--  3.0 unx    41238 tx defN 22-Aug-27 16:24 docs/_sources/tutorial.rst.txt
 -rw-r--r--  3.0 unx       93 tx defN 23-Feb-12 16:23 docs/_sources/reference.rst.txt
 -rw-r--r--  3.0 unx     7548 tx defN 22-Apr-23 18:28 docs/_sources/package_overview.rst.txt
 -rw-r--r--  3.0 unx      149 tx defN 22-Apr-21 04:29 docs/_sources/cli_export.rst.txt
 -rw-r--r--  3.0 unx   147706 tx defN 23-Feb-12 16:20 docs/_sources/API_README.rst.txt
 -rw-r--r--  3.0 unx      502 tx defN 23-Feb-12 16:24 docs/_sources/index.rst.txt
 -rw-r--r--  3.0 unx     4241 tx defN 22-May-01 15:46 docs/_sources/overview.rst.txt
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_static/
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/plus.png
 -rw-r--r--  3.0 unx     4712 tx defN 22-Nov-13 03:13 docs/_static/sphinx_highlight.js
 -rw-r--r--  3.0 unx    19530 tx defN 21-Jun-05 18:07 docs/_static/underscore.js
 -rw-r--r--  3.0 unx    11185 tx defN 21-Mar-22 05:50 docs/_static/alabaster.css
--rw-r--r--  3.0 unx      421 tx defN 23-Jul-15 14:32 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jul-16 22:13 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jul-15 14:32 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jul-16 22:13 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jul-15 14:32 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jul-16 22:13 docs/_static/language_data.js
 -rw-r--r--  3.0 unx      411 tx defN 22-Apr-21 05:12 docs/_static/copy-button.svg
 -rw-r--r--  3.0 unx     2698 tx defN 22-Dec-03 06:57 docs/_static/copybutton_funcs.js
 -rw-r--r--  3.0 unx       90 bx defN 21-Mar-14 19:14 docs/_static/minus.png
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-24 15:32 docs/_static/styles/
 -rw-r--r--  3.0 unx    72647 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css.map
 -rw-r--r--  3.0 unx     5529 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css
 -rw-r--r--  3.0 unx    48032 tx defN 22-Dec-03 06:57 docs/_static/styles/furo.css
 -rw-r--r--  3.0 unx     7809 tx defN 22-Apr-21 04:34 docs/_static/styles/furo-extensions.css.map
 -rw-r--r--  3.0 unx     6034 tx defN 22-Nov-13 03:13 docs/_static/skeleton.css
 -rw-r--r--  3.0 unx   288580 tx defN 22-Nov-13 03:13 docs/_static/jquery-3.6.0.js
--rw-r--r--  3.0 unx    14810 tx defN 23-Jul-15 14:32 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jul-16 22:13 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jul-15 14:32 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jul-16 22:13 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   423876 tx defN 23-Jul-15 14:32 docs/cli.html
+-rw-r--r--  3.0 unx   423876 tx defN 23-Jul-16 22:13 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   252162 tx defN 23-Jul-15 14:32 docs/genindex.html
--rw-r--r--  3.0 unx   110079 tx defN 23-Jul-15 14:32 docs/index.html
+-rw-r--r--  3.0 unx   252162 tx defN 23-Jul-16 22:13 docs/genindex.html
+-rw-r--r--  3.0 unx   110079 tx defN 23-Jul-16 22:13 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9767 bx stor 23-Jul-15 14:32 docs/objects.inv
+-rw-r--r--  3.0 unx     9767 bx stor 23-Jul-16 22:13 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jul-15 14:32 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jul-15 14:32 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jul-15 14:32 docs/py-modindex.html
--rw-r--r--  3.0 unx   468865 tx defN 23-Jul-15 14:32 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jul-16 22:13 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jul-16 22:13 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jul-16 22:13 docs/py-modindex.html
+-rw-r--r--  3.0 unx   468865 tx defN 23-Jul-16 22:13 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jul-15 14:32 docs/search.html
--rw-r--r--  3.0 unx   223521 tx defN 23-Jul-15 14:32 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jul-15 14:32 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jul-15 14:32 docs/tutorial.html
-99 files, 7011007 bytes uncompressed, 1458970 bytes compressed:  79.2%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jul-16 22:13 docs/search.html
+-rw-r--r--  3.0 unx   223524 tx defN 23-Jul-16 22:13 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jul-16 22:13 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jul-16 22:13 docs/tutorial.html
+99 files, 7016013 bytes uncompressed, 1459208 bytes compressed:  79.2%
```

#### docs/_modules/index.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../genindex.html" /><link rel="search" title="Search" href="../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>Overview: module code - osxphotos 0.60.7 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photosdb/photosdb.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../../genindex.html" /><link rel="search" title="Search" href="../../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1899,23 +1899,24 @@
             <span class="k">try</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_dbpersons_fullname</span><span class="p">[</span><span class="n">fullname</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">pk</span><span class="p">)</span>
             <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_dbpersons_fullname</span><span class="p">[</span><span class="n">fullname</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">pk</span><span class="p">]</span>
 
         <span class="c1"># get info on keyface -- some photos have null keyface so can&#39;t do a single query</span>
         <span class="c1"># (at least not with my SQL skills)</span>
+        <span class="n">asset_fk</span> <span class="o">=</span> <span class="n">_DB_TABLE_NAMES</span><span class="p">[</span><span class="n">photos_ver</span><span class="p">][</span><span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">]</span>
         <span class="n">c</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;&quot;&quot; SELECT</span>
 <span class="s2">                ZPERSON.Z_PK,</span>
 <span class="s2">                ZPERSON.ZKEYFACE,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZUUID,</span>
 <span class="s2">                ZDETECTEDFACE.ZUUID</span>
 <span class="s2">                FROM ZPERSON, ZDETECTEDFACE, </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2"></span>
 <span class="s2">                WHERE ZDETECTEDFACE.Z_PK = ZPERSON.ZKEYFACE AND</span>
-<span class="s2">                ZDETECTEDFACE.ZASSET = </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK</span>
+<span class="s2">                </span><span class="si">{</span><span class="n">asset_fk</span><span class="si">}</span><span class="s2"> = </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK</span>
 <span class="s2">            &quot;&quot;&quot;</span>
         <span class="p">)</span>
 
         <span class="c1"># 0 ZPERSON.Z_PK,</span>
         <span class="c1"># 1 ZPERSON.ZKEYFACE,</span>
         <span class="c1"># 2 ZGENERICASSET.ZUUID,</span>
         <span class="c1"># 3 ZDETECTEDFACE.ZUUID</span>
@@ -1926,21 +1927,22 @@
                 <span class="bp">self</span><span class="o">.</span><span class="n">_dbpersons_pk</span><span class="p">[</span><span class="n">pk</span><span class="p">][</span><span class="s2">&quot;photo_uuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">person</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_dbpersons_pk</span><span class="p">[</span><span class="n">pk</span><span class="p">][</span><span class="s2">&quot;keyface_uuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">person</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span>
             <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
                 <span class="n">logger</span><span class="o">.</span><span class="n">debug</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;Unexpected KeyError _dbpersons_pk[</span><span class="si">{</span><span class="n">pk</span><span class="si">}</span><span class="s2">]&quot;</span><span class="p">)</span>
 
         <span class="c1"># get information on detected faces</span>
         <span class="n">verbose</span><span class="p">(</span><span class="s2">&quot;Processing detected faces in photos.&quot;</span><span class="p">)</span>
+        <span class="n">person_fk</span> <span class="o">=</span> <span class="n">_DB_TABLE_NAMES</span><span class="p">[</span><span class="n">photos_ver</span><span class="p">][</span><span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">]</span>
         <span class="n">c</span><span class="o">.</span><span class="n">execute</span><span class="p">(</span>
             <span class="sa">f</span><span class="s2">&quot;&quot;&quot; SELECT</span>
 <span class="s2">                ZPERSON.Z_PK,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZUUID</span>
 <span class="s2">                FROM ZPERSON, ZDETECTEDFACE, </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2"></span>
-<span class="s2">                WHERE ZDETECTEDFACE.ZPERSON = ZPERSON.Z_PK AND</span>
-<span class="s2">                ZDETECTEDFACE.ZASSET = </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK</span>
+<span class="s2">                WHERE </span><span class="si">{</span><span class="n">person_fk</span><span class="si">}</span><span class="s2"> = ZPERSON.Z_PK AND</span>
+<span class="s2">                </span><span class="si">{</span><span class="n">asset_fk</span><span class="si">}</span><span class="s2"> = </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK</span>
 <span class="s2">            &quot;&quot;&quot;</span>
         <span class="p">)</span>
 
         <span class="c1"># 0     ZPERSON.Z_PK,</span>
         <span class="c1"># 1     ZGENERICASSET.ZUUID,</span>
 
         <span class="k">for</span> <span class="n">face</span> <span class="ow">in</span> <span class="n">c</span><span class="p">:</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1872,23 +1872,24 @@
                 self._dbpersons_fullname[fullname].append(pk)
             except KeyError:
                 self._dbpersons_fullname[fullname] = [pk]
 
         # get info on keyface -- some photos have null keyface so can't do a
 single query
         # (at least not with my SQL skills)
+        asset_fk = _DB_TABLE_NAMES[photos_ver]["DETECTED_FACE_ASSET_FK"]
         c.execute(
             f""" SELECT
                 ZPERSON.Z_PK,
                 ZPERSON.ZKEYFACE,
                 {asset_table}.ZUUID,
                 ZDETECTEDFACE.ZUUID
                 FROM ZPERSON, ZDETECTEDFACE, {asset_table}
                 WHERE ZDETECTEDFACE.Z_PK = ZPERSON.ZKEYFACE AND
-                ZDETECTEDFACE.ZASSET = {asset_table}.Z_PK
+                {asset_fk} = {asset_table}.Z_PK
             """
         )
 
         # 0 ZPERSON.Z_PK,
         # 1 ZPERSON.ZKEYFACE,
         # 2 ZGENERICASSET.ZUUID,
         # 3 ZDETECTEDFACE.ZUUID
@@ -1899,21 +1900,22 @@
                 self._dbpersons_pk[pk]["photo_uuid"] = person[2]
                 self._dbpersons_pk[pk]["keyface_uuid"] = person[3]
             except KeyError:
                 logger.debug(f"Unexpected KeyError _dbpersons_pk[{pk}]")
 
         # get information on detected faces
         verbose("Processing detected faces in photos.")
+        person_fk = _DB_TABLE_NAMES[photos_ver]["DETECTED_FACE_PERSON_FK"]
         c.execute(
             f""" SELECT
                 ZPERSON.Z_PK,
                 {asset_table}.ZUUID
                 FROM ZPERSON, ZDETECTEDFACE, {asset_table}
-                WHERE ZDETECTEDFACE.ZPERSON = ZPERSON.Z_PK AND
-                ZDETECTEDFACE.ZASSET = {asset_table}.Z_PK
+                WHERE {person_fk} = ZPERSON.Z_PK AND
+                {asset_fk} = {asset_table}.Z_PK
             """
         )
 
         # 0     ZPERSON.Z_PK,
         # 1     ZGENERICASSET.ZUUID,
 
         for face in c:
```

#### docs/_modules/osxphotos/_constants.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos._constants - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos._constants - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="../../_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="../../_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="../../_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -119,15 +119,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.5 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -142,15 +142,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="../../index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.5 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -216,88 +216,114 @@
 <span class="n">TIME_DELTA</span> <span class="o">=</span> <span class="p">(</span><span class="n">datetime</span><span class="p">(</span><span class="mi">2001</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">)</span> <span class="o">-</span> <span class="n">datetime</span><span class="p">(</span><span class="mi">1970</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">0</span><span class="p">,</span> <span class="mi">0</span><span class="p">))</span><span class="o">.</span><span class="n">total_seconds</span><span class="p">()</span>
 
 <span class="c1"># which Photos library database versions have been tested</span>
 <span class="c1"># Photos 2.0 (10.12.6) == 2622</span>
 <span class="c1"># Photos 3.0 (10.13.6) == 3301</span>
 <span class="c1"># Photos 4.0 (10.14.5) == 4016</span>
 <span class="c1"># Photos 4.0 (10.14.6) == 4025</span>
-<span class="c1"># Photos 5.0 (10.15.0) == 6000 or 5001</span>
+<span class="c1"># Photos 5.0+ (10.15.0) == 6000 or 5001</span>
 <span class="n">_TESTED_DB_VERSIONS</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;6000&quot;</span><span class="p">,</span> <span class="s2">&quot;5001&quot;</span><span class="p">,</span> <span class="s2">&quot;4025&quot;</span><span class="p">,</span> <span class="s2">&quot;4016&quot;</span><span class="p">,</span> <span class="s2">&quot;3301&quot;</span><span class="p">,</span> <span class="s2">&quot;2622&quot;</span><span class="p">]</span>
 
-<span class="c1"># database model versions (applies to Photos 5, Photos 6)</span>
+<span class="c1"># database model versions (applies to Photos 5+)</span>
 <span class="c1"># these come from PLModelVersion key in binary plist in Z_METADATA.Z_PLIST</span>
 <span class="c1"># Photos 5 (10.15.1) == 13537</span>
 <span class="c1"># Photos 5 (10.15.4, 10.15.5, 10.15.6) == 13703</span>
 <span class="c1"># Photos 6 (10.16.0 Beta) == 14104</span>
-<span class="n">_TEST_MODEL_VERSIONS</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;13537&quot;</span><span class="p">,</span> <span class="s2">&quot;13703&quot;</span><span class="p">,</span> <span class="s2">&quot;14104&quot;</span><span class="p">]</span>
+<span class="c1"># Photos 7 (12.0.1) == 15323</span>
+<span class="c1"># Photos 8 (13.0.0) == 16320</span>
+<span class="c1"># Photos 9 (14.0.0 dev preview) = 17120</span>
+<span class="n">_TEST_MODEL_VERSIONS</span> <span class="o">=</span> <span class="p">[</span><span class="s2">&quot;13537&quot;</span><span class="p">,</span> <span class="s2">&quot;13703&quot;</span><span class="p">,</span> <span class="s2">&quot;14104&quot;</span><span class="p">,</span> <span class="s2">&quot;15323&quot;</span><span class="p">,</span> <span class="s2">&quot;16320&quot;</span><span class="p">,</span> <span class="s2">&quot;17120&quot;</span><span class="p">]</span>
 
 <span class="n">_PHOTOS_2_VERSION</span> <span class="o">=</span> <span class="s2">&quot;2622&quot;</span>
 
 <span class="c1"># only version 3 - 4 have RKVersion.selfPortrait</span>
 <span class="n">_PHOTOS_3_VERSION</span> <span class="o">=</span> <span class="s2">&quot;3301&quot;</span>
 
 <span class="c1"># versions 5.0 and later have a different database structure</span>
-<span class="n">_PHOTOS_4_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4025&quot;</span>  <span class="c1"># latest Mojove version on 10.14.6</span>
+<span class="n">_PHOTOS_4_VERSION</span> <span class="o">=</span> <span class="s2">&quot;4025&quot;</span>  <span class="c1"># latest Mojave version on 10.14.6</span>
 <span class="n">_PHOTOS_5_VERSION</span> <span class="o">=</span> <span class="s2">&quot;5000&quot;</span>  <span class="c1"># I&#39;ve seen both 5001 and 6000.  6000 is most common on Catalina and up but there are some version 5001 database in the wild</span>
 
 <span class="c1"># Ranges for model version by Photos version</span>
 <span class="n">_PHOTOS_5_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">13000</span><span class="p">,</span> <span class="mi">13999</span><span class="p">]</span>
 <span class="n">_PHOTOS_6_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">14000</span><span class="p">,</span> <span class="mi">14999</span><span class="p">]</span>
 <span class="n">_PHOTOS_7_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">15000</span><span class="p">,</span> <span class="mi">15999</span><span class="p">]</span>  <span class="c1"># Dev preview: 15134, 12.1: 15331</span>
 <span class="n">_PHOTOS_8_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">16000</span><span class="p">,</span> <span class="mi">16999</span><span class="p">]</span>  <span class="c1"># Ventura dev preview: 16119</span>
+<span class="n">_PHOTOS_9_MODEL_VERSION</span> <span class="o">=</span> <span class="p">[</span><span class="mi">17000</span><span class="p">,</span> <span class="mi">17999</span><span class="p">]</span>  <span class="c1"># Sonoma dev preview: 17120</span>
 
-<span class="c1"># some table names differ between Photos 5 and Photos 6</span>
+<span class="c1"># some table names differ between Photos 5 and later versions</span>
 <span class="n">_DB_TABLE_NAMES</span> <span class="o">=</span> <span class="p">{</span>
     <span class="mi">5</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZGENERICASSET&quot;</span><span class="p">,</span>
         <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_37KEYWORDS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_34ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_FOK_34ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;IMPORT_FOK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZGENERICASSET.Z_FOK_IMPORTSESSION&quot;</span><span class="p">,</span>
         <span class="s2">&quot;DEPTH_STATE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZGENERICASSET.ZDEPTHSTATES&quot;</span><span class="p">,</span>
         <span class="s2">&quot;UTI_ORIGINAL&quot;</span><span class="p">:</span> <span class="s2">&quot;ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_26ALBUMS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_TABLE&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;HDR_TYPE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZCUSTOMRENDEREDVALUE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZPERSON&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZASSET&quot;</span><span class="p">,</span>
     <span class="p">},</span>
     <span class="mi">6</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET&quot;</span><span class="p">,</span>
         <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_36KEYWORDS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_FOK_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;IMPORT_FOK&quot;</span><span class="p">:</span> <span class="s2">&quot;null&quot;</span><span class="p">,</span>
         <span class="s2">&quot;DEPTH_STATE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET.ZDEPTHTYPE&quot;</span><span class="p">,</span>
         <span class="s2">&quot;UTI_ORIGINAL&quot;</span><span class="p">:</span> <span class="s2">&quot;ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS.Z_26ALBUMS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_TABLE&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_26ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;HDR_TYPE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZCUSTOMRENDEREDVALUE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZPERSON&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZASSET&quot;</span><span class="p">,</span>
     <span class="p">},</span>
     <span class="mi">7</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET&quot;</span><span class="p">,</span>
         <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_38KEYWORDS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_27ASSETS.Z_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_27ASSETS.Z_FOK_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;IMPORT_FOK&quot;</span><span class="p">:</span> <span class="s2">&quot;null&quot;</span><span class="p">,</span>
         <span class="s2">&quot;DEPTH_STATE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET.ZDEPTHTYPE&quot;</span><span class="p">,</span>
         <span class="s2">&quot;UTI_ORIGINAL&quot;</span><span class="p">:</span> <span class="s2">&quot;ZINTERNALRESOURCE.ZCOMPACTUTI&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_27ASSETS.Z_27ALBUMS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_TABLE&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_27ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;HDR_TYPE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZHDRTYPE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZPERSON&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZASSET&quot;</span><span class="p">,</span>
     <span class="p">},</span>
     <span class="mi">8</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET&quot;</span><span class="p">,</span>
         <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_40KEYWORDS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_FOK_3ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;IMPORT_FOK&quot;</span><span class="p">:</span> <span class="s2">&quot;null&quot;</span><span class="p">,</span>
         <span class="s2">&quot;DEPTH_STATE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET.ZDEPTHTYPE&quot;</span><span class="p">,</span>
         <span class="s2">&quot;UTI_ORIGINAL&quot;</span><span class="p">:</span> <span class="s2">&quot;ZINTERNALRESOURCE.ZCOMPACTUTI&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_28ALBUMS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;ASSET_ALBUM_TABLE&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS&quot;</span><span class="p">,</span>
         <span class="s2">&quot;HDR_TYPE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZHDRTYPE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZPERSON&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZASSET&quot;</span><span class="p">,</span>
+    <span class="p">},</span>
+    <span class="mi">9</span><span class="p">:</span> <span class="p">{</span>
+        <span class="s2">&quot;ASSET&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;KEYWORD_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_1KEYWORDS.Z_40KEYWORDS&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_3ASSETS&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;ALBUM_SORT_ORDER&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_FOK_3ASSETS&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;IMPORT_FOK&quot;</span><span class="p">:</span> <span class="s2">&quot;null&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DEPTH_STATE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZASSET.ZDEPTHTYPE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;UTI_ORIGINAL&quot;</span><span class="p">:</span> <span class="s2">&quot;ZINTERNALRESOURCE.ZCOMPACTUTI&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;ASSET_ALBUM_JOIN&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS.Z_28ALBUMS&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;ASSET_ALBUM_TABLE&quot;</span><span class="p">:</span> <span class="s2">&quot;Z_28ASSETS&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;HDR_TYPE&quot;</span><span class="p">:</span> <span class="s2">&quot;ZHDRTYPE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_PERSON_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZPERSONFORFACE&quot;</span><span class="p">,</span>
+        <span class="s2">&quot;DETECTED_FACE_ASSET_FK&quot;</span><span class="p">:</span> <span class="s2">&quot;ZDETECTEDFACE.ZASSETFORFACE&quot;</span><span class="p">,</span>
     <span class="p">},</span>
 <span class="p">}</span>
 
 <span class="c1"># which version operating systems have been tested</span>
 <span class="n">_TESTED_OS_VERSIONS</span> <span class="o">=</span> <span class="p">[</span>
     <span class="p">(</span><span class="s2">&quot;10&quot;</span><span class="p">,</span> <span class="s2">&quot;12&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;10&quot;</span><span class="p">,</span> <span class="s2">&quot;13&quot;</span><span class="p">),</span>
@@ -320,14 +346,15 @@
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;5&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;12&quot;</span><span class="p">,</span> <span class="s2">&quot;6&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;0&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;1&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;2&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;3&quot;</span><span class="p">),</span>
     <span class="p">(</span><span class="s2">&quot;13&quot;</span><span class="p">,</span> <span class="s2">&quot;4&quot;</span><span class="p">),</span>
+    <span class="p">(</span><span class="s2">&quot;14&quot;</span><span class="p">,</span> <span class="s2">&quot;0&quot;</span><span class="p">),</span>
 <span class="p">]</span>
 
 <span class="c1"># Photos 5 has persons who are empty string if unidentified face</span>
 <span class="n">_UNKNOWN_PERSON</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
 
 <span class="c1"># photos with no reverse geolocation info (place)</span>
 <span class="n">_UNKNOWN_PLACE</span> <span class="o">=</span> <span class="s2">&quot;_UNKNOWN_&quot;</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -58,89 +58,115 @@
 0)).total_seconds()
 
 # which Photos library database versions have been tested
 # Photos 2.0 (10.12.6) == 2622
 # Photos 3.0 (10.13.6) == 3301
 # Photos 4.0 (10.14.5) == 4016
 # Photos 4.0 (10.14.6) == 4025
-# Photos 5.0 (10.15.0) == 6000 or 5001
+# Photos 5.0+ (10.15.0) == 6000 or 5001
 _TESTED_DB_VERSIONS = ["6000", "5001", "4025", "4016", "3301", "2622"]
 
-# database model versions (applies to Photos 5, Photos 6)
+# database model versions (applies to Photos 5+)
 # these come from PLModelVersion key in binary plist in Z_METADATA.Z_PLIST
 # Photos 5 (10.15.1) == 13537
 # Photos 5 (10.15.4, 10.15.5, 10.15.6) == 13703
 # Photos 6 (10.16.0 Beta) == 14104
-_TEST_MODEL_VERSIONS = ["13537", "13703", "14104"]
+# Photos 7 (12.0.1) == 15323
+# Photos 8 (13.0.0) == 16320
+# Photos 9 (14.0.0 dev preview) = 17120
+_TEST_MODEL_VERSIONS = ["13537", "13703", "14104", "15323", "16320", "17120"]
 
 _PHOTOS_2_VERSION = "2622"
 
 # only version 3 - 4 have RKVersion.selfPortrait
 _PHOTOS_3_VERSION = "3301"
 
 # versions 5.0 and later have a different database structure
-_PHOTOS_4_VERSION = "4025"  # latest Mojove version on 10.14.6
+_PHOTOS_4_VERSION = "4025"  # latest Mojave version on 10.14.6
 _PHOTOS_5_VERSION = "5000"  # I've seen both 5001 and 6000.  6000 is most
 common on Catalina and up but there are some version 5001 database in the wild
 
 # Ranges for model version by Photos version
 _PHOTOS_5_MODEL_VERSION = [13000, 13999]
 _PHOTOS_6_MODEL_VERSION = [14000, 14999]
 _PHOTOS_7_MODEL_VERSION = [15000, 15999]  # Dev preview: 15134, 12.1: 15331
 _PHOTOS_8_MODEL_VERSION = [16000, 16999]  # Ventura dev preview: 16119
+_PHOTOS_9_MODEL_VERSION = [17000, 17999]  # Sonoma dev preview: 17120
 
-# some table names differ between Photos 5 and Photos 6
+# some table names differ between Photos 5 and later versions
 _DB_TABLE_NAMES = {
     5: {
         "ASSET": "ZGENERICASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_37KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_34ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_34ASSETS",
         "IMPORT_FOK": "ZGENERICASSET.Z_FOK_IMPORTSESSION",
         "DEPTH_STATE": "ZGENERICASSET.ZDEPTHSTATES",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER",
         "ASSET_ALBUM_JOIN": "Z_26ASSETS.Z_26ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_26ASSETS",
         "HDR_TYPE": "ZCUSTOMRENDEREDVALUE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     6: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_36KEYWORDS",
         "ALBUM_JOIN": "Z_26ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_26ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZUNIFORMTYPEIDENTIFIER",
         "ASSET_ALBUM_JOIN": "Z_26ASSETS.Z_26ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_26ASSETS",
         "HDR_TYPE": "ZCUSTOMRENDEREDVALUE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     7: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_38KEYWORDS",
         "ALBUM_JOIN": "Z_27ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_27ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
         "ASSET_ALBUM_JOIN": "Z_27ASSETS.Z_27ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_27ASSETS",
         "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
     },
     8: {
         "ASSET": "ZASSET",
         "KEYWORD_JOIN": "Z_1KEYWORDS.Z_40KEYWORDS",
         "ALBUM_JOIN": "Z_28ASSETS.Z_3ASSETS",
         "ALBUM_SORT_ORDER": "Z_28ASSETS.Z_FOK_3ASSETS",
         "IMPORT_FOK": "null",
         "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
         "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
         "ASSET_ALBUM_JOIN": "Z_28ASSETS.Z_28ALBUMS",
         "ASSET_ALBUM_TABLE": "Z_28ASSETS",
         "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSON",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSET",
+    },
+    9: {
+        "ASSET": "ZASSET",
+        "KEYWORD_JOIN": "Z_1KEYWORDS.Z_40KEYWORDS",
+        "ALBUM_JOIN": "Z_28ASSETS.Z_3ASSETS",
+        "ALBUM_SORT_ORDER": "Z_28ASSETS.Z_FOK_3ASSETS",
+        "IMPORT_FOK": "null",
+        "DEPTH_STATE": "ZASSET.ZDEPTHTYPE",
+        "UTI_ORIGINAL": "ZINTERNALRESOURCE.ZCOMPACTUTI",
+        "ASSET_ALBUM_JOIN": "Z_28ASSETS.Z_28ALBUMS",
+        "ASSET_ALBUM_TABLE": "Z_28ASSETS",
+        "HDR_TYPE": "ZHDRTYPE",
+        "DETECTED_FACE_PERSON_FK": "ZDETECTEDFACE.ZPERSONFORFACE",
+        "DETECTED_FACE_ASSET_FK": "ZDETECTEDFACE.ZASSETFORFACE",
     },
 }
 
 # which version operating systems have been tested
 _TESTED_OS_VERSIONS = [
     ("10", "12"),
     ("10", "13"),
@@ -163,14 +189,15 @@
     ("12", "5"),
     ("12", "6"),
     ("13", "0"),
     ("13", "1"),
     ("13", "2"),
     ("13", "3"),
     ("13", "4"),
+    ("14", "0"),
 ]
 
 # Photos 5 has persons who are empty string if unidentified face
 _UNKNOWN_PERSON = "_UNKNOWN_"
 
 # photos with no reverse geolocation info (place)
 _UNKNOWN_PLACE = "_UNKNOWN_"
```

#### docs/_sources/template_help.rst.txt

```diff
@@ -357,15 +357,15 @@
    * - {cr}
      - A carriage return: '\r'
    * - {crlf}
      - A carriage return + line feed: '\r\n'
    * - {tab}
      - :A tab: '\t'
    * - {osxphotos_version}
-     - The osxphotos version, e.g. '0.60.7'
+     - The osxphotos version, e.g. '0.60.8'
    * - {osxphotos_cmd_line}
      - The full command line used to run osxphotos
    * - {album}
      - Album(s) photo is contained in
    * - {folder_album}
      - Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder
    * - {project}
```

#### docs/_static/documentation_options.js

##### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 var DOCUMENTATION_OPTIONS = {
     URL_ROOT: document.getElementById("documentation_options").getAttribute('data-url_root'),
-    VERSION: '0.60.7',
+    VERSION: '0.60.8',
     LANGUAGE: 'en',
     COLLAPSE_INDEX: false,
     BUILDER: 'html',
     FILE_SUFFIX: '.html',
     LINK_SUFFIX: '.html',
     HAS_SOURCE: true,
     SOURCELINK_SUFFIX: '.txt',
```

#### docs/cli.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Template System" href="template_help.html" /><link rel="prev" title="OSXPhotos Tutorial" href="tutorial.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.7 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.8 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/index.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos 0.60.7 documentation</title>
+        <title>osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="#"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="#">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Tutorial" href="tutorial.html" /><link rel="prev" title="Welcome to OSXPhotos’s documentation!" href="index.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/package_overview.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Reference" href="reference.html" /><link rel="prev" title="OSXPhotos Template System" href="template_help.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/py-modindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.7 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.8 documentation</title>
 <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -118,15 +118,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -141,15 +141,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/reference.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="prev" title="OSXPhotos Python Package Overview" href="package_overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Python Reference - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.7 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.8 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
 
@@ -117,15 +117,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -140,15 +140,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="#" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/searchindex.js

##### js-beautify {}

```diff
@@ -1083,15 +1083,15 @@
         "x": [2, 4, 5],
         "sierra": 2,
         "6": [2, 5],
         "monterei": [2, 5],
         "read": [0, 2, 4, 6],
         "vice": 2,
         "versa": 2,
-        "8": [2, 4],
+        "8": [2, 4, 5],
         "recommend": [0, 2, 6],
         "wai": [2, 6],
         "pipx": [2, 3],
         "easiest": 2,
         "applic": [2, 6],
         "accord": 2,
         "instruct": [2, 6],
```

#### docs/template_help.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Python Package Overview" href="package_overview.html" /><link rel="prev" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Template System - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -609,15 +609,15 @@
 <dt class="field-odd">A tab<span class="colon">:</span></dt>
 <dd class="field-odd"><p>‘t’</p>
 </dd>
 </dl>
 </td>
 </tr>
 <tr class="row-odd"><td><p>{osxphotos_version}</p></td>
-<td><p>The osxphotos version, e.g. ‘0.60.7’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.8’</p></td>
 </tr>
 <tr class="row-even"><td><p>{osxphotos_cmd_line}</p></td>
 <td><p>The full command line used to run osxphotos</p></td>
 </tr>
 <tr class="row-odd"><td><p>{album}</p></td>
 <td><p>Album(s) photo is contained in</p></td>
 </tr>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -428,15 +428,15 @@
 {closebracket}                 A close bracket: â]â
 {newline}                      A newline: ânâ
 {lf}                           A line feed: ânâ, alias for {newline}
 {cr}                           A carriage return: ârâ
 {crlf}                         A carriage return + line feed: ârnâ
 {tab}                            A tab:
                                      âtâ
-{osxphotos_version}            The osxphotos version, e.g. â0.60.7â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.8â
 {osxphotos_cmd_line}           The full command line used to run osxphotos
 {album}                        Album(s) photo is contained in
 {folder_album}                 Folder path + album photo is contained in. e.g. âFolder/Subfolder/Albumâ or just âAlbumâ if
                                no enclosing folder
 {project}                      Project(s) photo is contained in (such as greeting cards, calendars, slideshows)
 {album_project}                Album(s) and project(s) photo is contained in; treats projects as regular albums
 {folder_album_project}         Folder path + album (includes projects as albums) photo is contained in. e.g. âFolder/Subfolder/
```

#### docs/tutorial.html

```diff
@@ -2,15 +2,15 @@
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><meta name="generator" content="Docutils 0.19: https://docutils.sourceforge.io/" />
 <link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="search.html" /><link rel="next" title="OSXPhotos Command Line Interface (CLI)" href="cli.html" /><link rel="prev" title="OSXPhotos" href="overview.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>OSXPhotos Tutorial - osxphotos 0.60.7 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.8 documentation</title>
       <link rel="stylesheet" type="text/css" href="_static/pygments.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo.css?digest=d81277517bee4d6b0349d71bb2661d4890b5617c" />
     <link rel="stylesheet" type="text/css" href="_static/copybutton.css" />
     <link rel="stylesheet" type="text/css" href="_static/styles/furo-extensions.css?digest=30d1aed668e5c3a91c3e3bf6a60b675221979f0e" />
     
     
 
@@ -120,15 +120,15 @@
     <div class="header-left">
       <label class="nav-overlay-icon" for="__navigation">
         <div class="visually-hidden">Toggle site navigation sidebar</div>
         <i class="icon"><svg><use href="#svg-menu"></use></svg></i>
       </label>
     </div>
     <div class="header-center">
-      <a href="index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
     </div>
     <div class="header-right">
       <div class="theme-toggle-container theme-toggle-header">
         <button class="theme-toggle">
           <div class="visually-hidden">Toggle Light / Dark / Auto color theme</div>
           <svg class="theme-icon-when-auto"><use href="#svg-sun-half"></use></svg>
           <svg class="theme-icon-when-dark"><use href="#svg-moon"></use></svg>
@@ -143,15 +143,15 @@
   </header>
   <aside class="sidebar-drawer">
     <div class="sidebar-container">
       
       <div class="sidebar-sticky"><a class="sidebar-brand" href="index.html">
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.8_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.7/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.8/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/exifinfo.py` & `osxphotos-0.60.8/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/exiftool.py` & `osxphotos-0.60.8/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.8/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/export_db.py` & `osxphotos-0.60.8/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/export_db_utils.py` & `osxphotos-0.60.8/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/fileutil.py` & `osxphotos-0.60.8/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.8/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/imageconverter.py` & `osxphotos-0.60.8/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/momentinfo.py` & `osxphotos-0.60.8/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/path_utils.py` & `osxphotos-0.60.8/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/personinfo.py` & `osxphotos-0.60.8/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photodates.py` & `osxphotos-0.60.8/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photoexporter.py` & `osxphotos-0.60.8/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photoinfo.py` & `osxphotos-0.60.8/osxphotos/photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photokit.py` & `osxphotos-0.60.8/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosalbum.py` & `osxphotos-0.60.8/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photoscript_utils.py` & `osxphotos-0.60.8/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files 4% similar despite different names*

```diff
@@ -175,24 +175,26 @@
     Args:
         photosdb: an OSXPhotosDB instance
     """
 
     db = photosdb._tmp_db
 
     asset_table = _DB_TABLE_NAMES[photosdb._photos_ver]["ASSET"]
+    asset_fk = _DB_TABLE_NAMES[photosdb._photos_ver]["DETECTED_FACE_ASSET_FK"]
+    person_fk = _DB_TABLE_NAMES[photosdb._photos_ver]["DETECTED_FACE_PERSON_FK"]
 
     (conn, cursor) = sqlite_open_ro(db)
 
     result = cursor.execute(
         f""" 
         SELECT
         ZDETECTEDFACE.Z_PK,
         {asset_table}.ZUUID,
         ZDETECTEDFACE.ZUUID,
-        ZDETECTEDFACE.ZPERSON,
+        {person_fk},
         ZPERSON.ZFULLNAME,
         ZDETECTEDFACE.ZAGETYPE,
         NULL, -- ZDETECTEDFACE.ZBALDTYPE (Removed in Monterey)
         ZDETECTEDFACE.ZEYEMAKEUPTYPE,
         ZDETECTEDFACE.ZEYESSTATE,
         ZDETECTEDFACE.ZFACIALHAIRTYPE,
         ZDETECTEDFACE.ZGENDERTYPE,
@@ -221,16 +223,16 @@
         NULL, -- ZDETECTEDFACE.ZRIGHTEYEX,
         NULL, -- ZDETECTEDFACE.ZRIGHTEYEY,
         ZDETECTEDFACE.ZROLL,
         ZDETECTEDFACE.ZSIZE,
         NULL, -- ZDETECTEDFACE.ZYAW,
         ZDETECTEDFACE.ZMASTERIDENTIFIER
         FROM ZDETECTEDFACE
-        JOIN {asset_table} ON {asset_table}.Z_PK = ZDETECTEDFACE.ZASSET
-        JOIN ZPERSON ON ZPERSON.Z_PK = ZDETECTEDFACE.ZPERSON;
+        JOIN {asset_table} ON {asset_table}.Z_PK = {asset_fk}
+        JOIN ZPERSON ON ZPERSON.Z_PK = {person_fk};
         """
     )
 
     # 0    ZDETECTEDFACE.Z_PK
     # 1    ZGENERICASSET.ZUUID,
     # 2    ZDETECTEDFACE.ZUUID,
     # 3    ZDETECTEDFACE.ZPERSON,
```

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.8/osxphotos/photosdb/photosdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1702,23 +1702,24 @@
             try:
                 self._dbpersons_fullname[fullname].append(pk)
             except KeyError:
                 self._dbpersons_fullname[fullname] = [pk]
 
         # get info on keyface -- some photos have null keyface so can't do a single query
         # (at least not with my SQL skills)
+        asset_fk = _DB_TABLE_NAMES[photos_ver]["DETECTED_FACE_ASSET_FK"]
         c.execute(
             f""" SELECT
                 ZPERSON.Z_PK,
                 ZPERSON.ZKEYFACE,
                 {asset_table}.ZUUID,
                 ZDETECTEDFACE.ZUUID
                 FROM ZPERSON, ZDETECTEDFACE, {asset_table}
                 WHERE ZDETECTEDFACE.Z_PK = ZPERSON.ZKEYFACE AND
-                ZDETECTEDFACE.ZASSET = {asset_table}.Z_PK
+                {asset_fk} = {asset_table}.Z_PK
             """
         )
 
         # 0 ZPERSON.Z_PK,
         # 1 ZPERSON.ZKEYFACE,
         # 2 ZGENERICASSET.ZUUID,
         # 3 ZDETECTEDFACE.ZUUID
@@ -1729,21 +1730,22 @@
                 self._dbpersons_pk[pk]["photo_uuid"] = person[2]
                 self._dbpersons_pk[pk]["keyface_uuid"] = person[3]
             except KeyError:
                 logger.debug(f"Unexpected KeyError _dbpersons_pk[{pk}]")
 
         # get information on detected faces
         verbose("Processing detected faces in photos.")
+        person_fk = _DB_TABLE_NAMES[photos_ver]["DETECTED_FACE_PERSON_FK"]
         c.execute(
             f""" SELECT
                 ZPERSON.Z_PK,
                 {asset_table}.ZUUID
                 FROM ZPERSON, ZDETECTEDFACE, {asset_table}
-                WHERE ZDETECTEDFACE.ZPERSON = ZPERSON.Z_PK AND
-                ZDETECTEDFACE.ZASSET = {asset_table}.Z_PK
+                WHERE {person_fk} = ZPERSON.Z_PK AND
+                {asset_fk} = {asset_table}.Z_PK
             """
         )
 
         # 0     ZPERSON.Z_PK,
         # 1     ZGENERICASSET.ZUUID,
 
         for face in c:
```

### Comparing `osxphotos-0.60.7/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.8/osxphotos/photosdb/photosdb_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     _PHOTOS_3_VERSION,
     _PHOTOS_4_VERSION,
     _PHOTOS_5_MODEL_VERSION,
     _PHOTOS_5_VERSION,
     _PHOTOS_6_MODEL_VERSION,
     _PHOTOS_7_MODEL_VERSION,
     _PHOTOS_8_MODEL_VERSION,
+    _PHOTOS_9_MODEL_VERSION,
     _TESTED_DB_VERSIONS,
 )
 from ..sqlite_utils import sqlite_open_ro
 
 __all__ = [
     "get_db_version",
     "get_model_version",
@@ -108,18 +109,20 @@
         return 5
     elif _PHOTOS_6_MODEL_VERSION[0] <= model_ver <= _PHOTOS_6_MODEL_VERSION[1]:
         return 6
     elif _PHOTOS_7_MODEL_VERSION[0] <= model_ver <= _PHOTOS_7_MODEL_VERSION[1]:
         return 7
     elif _PHOTOS_8_MODEL_VERSION[0] <= model_ver <= _PHOTOS_8_MODEL_VERSION[1]:
         return 8
+    elif _PHOTOS_9_MODEL_VERSION[0] <= model_ver <= _PHOTOS_9_MODEL_VERSION[1]:
+        return 9
     else:
         logging.warning(f"Unknown model version: {model_ver}")
         # cross our fingers and try latest version
-        return 8
+        return 9
 
 
 def get_photos_library_version(library_path: str | pathlib.Path) -> int:
     """Return int indicating which Photos version a library was created with
 
     Args:
         library_path: path to Photos library; may be path to the root of the library or the photos.db file
@@ -145,18 +148,20 @@
         return 5
     if _PHOTOS_6_MODEL_VERSION[0] <= model_ver <= _PHOTOS_6_MODEL_VERSION[1]:
         return 6
     if _PHOTOS_7_MODEL_VERSION[0] <= model_ver <= _PHOTOS_7_MODEL_VERSION[1]:
         return 7
     if _PHOTOS_8_MODEL_VERSION[0] <= model_ver <= _PHOTOS_8_MODEL_VERSION[1]:
         return 8
+    if _PHOTOS_9_MODEL_VERSION[0] <= model_ver <= _PHOTOS_9_MODEL_VERSION[1]:
+        return 9
     logging.warning(
         f"Unknown db / model version: db_ver={db_ver}, model_ver={model_ver}; assuming Photos 8"
     )
-    return 8
+    return 9
 
 
 def get_db_path_for_library(photos_library: str | pathlib.Path) -> pathlib.Path:
     """Returns path to Photos database file for Photos library
 
     Args:
         photos_library: path to Photos library; may be path to the root of the library or the photos.db file
```

### Comparing `osxphotos-0.60.7/osxphotos/phototables.py` & `osxphotos-0.60.8/osxphotos/phototables.py`

 * *Files 6% similar despite different names*

```diff
@@ -200,30 +200,34 @@
         super().__init__(db, version, uuid)
         self.columns = get_table_columns(self.conn, "ZPERSON")
         self.table_name = "ZPERSON"
 
     def rows(self) -> list[tuple[Any]]:
         """Return rows for this photo from the ZPERSON table."""
         conn, cursor = self.db.get_db_connection()
+        person_fk = _DB_TABLE_NAMES[self.version]["DETECTED_FACE_PERSON_FK"]
+        asset_fk = _DB_TABLE_NAMES[self.version]["DETECTED_FACE_ASSET_FK"]
         sql = f"""  SELECT ZPERSON.*
                     FROM ZPERSON 
-                    JOIN ZDETECTEDFACE ON ZDETECTEDFACE.ZPERSON = ZPERSON.Z_PK
-                    JOIN ZASSET ON ZASSET.Z_PK = ZDETECTEDFACE.ZASSET
+                    JOIN ZDETECTEDFACE ON {person_fk} = ZPERSON.Z_PK
+                    JOIN ZASSET ON ZASSET.Z_PK = {asset_fk}
                     WHERE {self.asset_table}.ZUUID = ?;
             """
         cursor.execute(sql, (self.uuid,))
         return result if (result := cursor.fetchall()) else []
 
     def _get_column(self, column: str) -> tuple[Any]:
         """Get column value for this photo from the ZPERSON table."""
         conn, cursor = self.db.get_db_connection()
+        person_fk = _DB_TABLE_NAMES[self.version]["DETECTED_FACE_PERSON_FK"]
+        asset_fk = _DB_TABLE_NAMES[self.version]["DETECTED_FACE_ASSET_FK"]
         sql = f"""  SELECT ZPERSON.{column}
                     FROM ZPERSON 
-                    JOIN ZDETECTEDFACE ON ZDETECTEDFACE.ZPERSON = ZPERSON.Z_PK
-                    JOIN ZASSET ON ZASSET.Z_PK = ZDETECTEDFACE.ZASSET
+                    JOIN ZDETECTEDFACE ON {person_fk} = ZPERSON.Z_PK
+                    JOIN ZASSET ON ZASSET.Z_PK = {asset_fk}
                     WHERE {self.asset_table}.ZUUID = ?;
             """
         cursor.execute(sql, (self.uuid,))
         return (
             tuple(result[0] for result in results)
             if (results := cursor.fetchall())
             else ()
```

### Comparing `osxphotos-0.60.7/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.8/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/phototemplate.md` & `osxphotos-0.60.8/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/phototemplate.py` & `osxphotos-0.60.8/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/phototemplate.tx` & `osxphotos-0.60.8/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/phototz.py` & `osxphotos-0.60.8/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/placeinfo.py` & `osxphotos-0.60.8/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/platform.py` & `osxphotos-0.60.8/osxphotos/platform.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/pyrepl.py` & `osxphotos-0.60.8/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.8/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/query_builder.py` & `osxphotos-0.60.8/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/queryoptions.py` & `osxphotos-0.60.8/osxphotos/queryoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/scoreinfo.py` & `osxphotos-0.60.8/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/searchinfo.py` & `osxphotos-0.60.8/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/sqlgrep.py` & `osxphotos-0.60.8/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/sqlite_utils.py` & `osxphotos-0.60.8/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.8/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/template_counter.py` & `osxphotos-0.60.8/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.8/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.8/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/text_detection.py` & `osxphotos-0.60.8/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/timeutils.py` & `osxphotos-0.60.8/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/timezones.py` & `osxphotos-0.60.8/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/tutorial.md` & `osxphotos-0.60.8/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/unicode.py` & `osxphotos-0.60.8/osxphotos/unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/uti.py` & `osxphotos-0.60.8/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos/utils.py` & `osxphotos-0.60.8/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.8/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.7
+Version: 0.60.8
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.7/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.8/osxphotos.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -203,14 +203,15 @@
 tests/test_search_info_10_15_4.py
 tests/test_search_info_10_15_5.py
 tests/test_search_info_10_15_7.py
 tests/test_shared_catalina_10_15_1.py
 tests/test_shared_mojave_10_14_6.py
 tests/test_shared_ventura_13_1.py
 tests/test_sidecar_xmp.py
+tests/test_sonoma_14_0_0.py
 tests/test_specials_bigsur_10_16_0.py
 tests/test_specials_catalina_10_15_1.py
 tests/test_specials_mojave_10_14_6.py
 tests/test_specials_sierra_10_12.py
 tests/test_sqlite_utils.py
 tests/test_sqlitekvstore.py
 tests/test_template.py
```

### Comparing `osxphotos-0.60.7/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.8/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/setup.py` & `osxphotos-0.60.8/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_10_12_6.py` & `osxphotos-0.60.8/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.8/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.8/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.8/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.8/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli.py` & `osxphotos-0.60.8/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_add_locations.py` & `osxphotos-0.60.8/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_add_to_album.py` & `osxphotos-0.60.8/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_all_commands.py` & `osxphotos-0.60.8/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_batch_edit.py` & `osxphotos-0.60.8/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_dump.py` & `osxphotos-0.60.8/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_exiftool.py` & `osxphotos-0.60.8/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_export_cloud.py` & `osxphotos-0.60.8/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_export_projects.py` & `osxphotos-0.60.8/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_exportdb.py` & `osxphotos-0.60.8/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_import.py` & `osxphotos-0.60.8/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_orphans.py` & `osxphotos-0.60.8/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_param_types.py` & `osxphotos-0.60.8/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_sync.py` & `osxphotos-0.60.8/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_timewarp.py` & `osxphotos-0.60.8/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_utils.py` & `osxphotos-0.60.8/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cli_verbose.py` & `osxphotos-0.60.8/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.8/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_comments.py` & `osxphotos-0.60.8/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_concurrent_export.py` & `osxphotos-0.60.8/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_configoptions.py` & `osxphotos-0.60.8/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_datetime_formatter.py` & `osxphotos-0.60.8/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_datetime_utils.py` & `osxphotos-0.60.8/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_debug.py` & `osxphotos-0.60.8/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_empty_library_4_0.py` & `osxphotos-0.60.8/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_exif_info.py` & `osxphotos-0.60.8/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_exiftool.py` & `osxphotos-0.60.8/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_exiftool_caching.py` & `osxphotos-0.60.8/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.8/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.8/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.8/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_db.py` & `osxphotos-0.60.8/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_exportresults.py` & `osxphotos-0.60.8/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_faceinfo.py` & `osxphotos-0.60.8/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_fileutil.py` & `osxphotos-0.60.8/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_highsierra.py` & `osxphotos-0.60.8/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_image_converter.py` & `osxphotos-0.60.8/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.8/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.8/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.8/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.8/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.8/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.8/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_movies_4_0.py` & `osxphotos-0.60.8/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_movies_5_0.py` & `osxphotos-0.60.8/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_path_utils.py` & `osxphotos-0.60.8/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_personinfo.py` & `osxphotos-0.60.8/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_photokit.py` & `osxphotos-0.60.8/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_photosalbum_unicode.py` & `osxphotos-0.60.8/tests/test_photosalbum_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_photosdb_utils.py` & `osxphotos-0.60.8/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_placeinfo.py` & `osxphotos-0.60.8/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.8/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_projects_catalina.py` & `osxphotos-0.60.8/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_projects_sierra.py` & `osxphotos-0.60.8/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_score_info.py` & `osxphotos-0.60.8/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.8/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.8/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.8/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.8/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_sidecar_xmp.py` & `osxphotos-0.60.8/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.8/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.8/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.8/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.8/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_sqlitekvstore.py` & `osxphotos-0.60.8/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_template.py` & `osxphotos-0.60.8/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_template_counter.py` & `osxphotos-0.60.8/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_template_today.py` & `osxphotos-0.60.8/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_unicode.py` & `osxphotos-0.60.8/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_uti.py` & `osxphotos-0.60.8/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_utils.py` & `osxphotos-0.60.8/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.8/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.7/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.8/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

