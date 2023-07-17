# Comparing `tmp/osxphotos-0.60.8.tar.gz` & `tmp/osxphotos-0.60.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osxphotos-0.60.8.tar", last modified: Sun Jul 16 22:13:16 2023, max compression
+gzip compressed data, was "osxphotos-0.60.9.tar", last modified: Mon Jul 17 01:15:27 2023, max compression
```

## Comparing `osxphotos-0.60.8.tar` & `osxphotos-0.60.9.tar`

### file list

```diff
@@ -1,238 +1,238 @@
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.398621 osxphotos-0.60.8/
--rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.8/LICENSE
--rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.8/MANIFEST.in
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-16 22:13:16.398446 osxphotos-0.60.8/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)   226455 2023-07-16 22:13:03.000000 osxphotos-0.60.8/README.md
--rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.8/README.rst
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.355346 osxphotos-0.60.8/osxphotos/
--rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.8/osxphotos/__main__.py
--rw-r--r--   0 rhet       (501) staff       (20)    17162 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/_constants.py
--rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-16 22:09:29.000000 osxphotos-0.60.8/osxphotos/_version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.8/osxphotos/adjustmentsinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.8/osxphotos/albuminfo.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.369259 osxphotos-0.60.8/osxphotos/cli/
--rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.8/osxphotos/cli/about.py
--rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/albums.py
--rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/cli/cli.py
--rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/cli_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)    27388 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/cli_params.py
--rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/click_rich_echo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.8/osxphotos/cli/color_themes.py
--rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/common.py
--rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/darkmode.py
--rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/debug_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/docs.py
--rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/dump.py
--rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/exiftool_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)   108030 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/cli/export.py
--rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/cli/exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/grep.py
--rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/help.py
--rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.8/osxphotos/cli/import_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/info.py
--rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/install_uninstall_run.py
--rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/keywords.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/kvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/labels.py
--rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/list.py
--rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.8/osxphotos/cli/orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/persons.py
--rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/photo_inspect.py
--rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/places.py
--rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/print_photo_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.8/osxphotos/cli/query.py
--rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/repl.py
--rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/cli/report_writer.py
--rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.8/osxphotos/cli/rich_progress.py
--rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/show_command.py
--rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/snap_diff.py
--rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/sync.py
--rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/sync_results.py
--rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.8/osxphotos/cli/theme.py
--rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.8/osxphotos/cli/tutorial.py
--rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/cli/uuid.py
--rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/cli/verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/cli/version.py
--rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/compare_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/crash_reporter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.8/osxphotos/datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/debug.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.378770 osxphotos-0.60.8/osxphotos/docs/
--rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.8/osxphotos/docs/README.md
--rw-r--r--   0 rhet       (501) staff       (20)  1477940 2023-07-16 22:13:12.000000 osxphotos-0.60.8/osxphotos/docs/docs.zip
--rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/exif_datetime_updater.py
--rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.8/osxphotos/exifinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.8/osxphotos/exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.8/osxphotos/exiftool_filetypes.json
--rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/export_db_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/frozen_photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/imageconverter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.8/osxphotos/momentinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/photodates.py
--rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/photoexporter.py
--rw-r--r--   0 rhet       (501) staff       (20)    85034 2023-07-15 14:18:05.000000 osxphotos-0.60.8/osxphotos/photoinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosalbum.py
--rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photoscript_utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.381563 osxphotos-0.60.8/osxphotos/photosdb/
--rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_exif.py
--rw-r--r--   0 rhet       (501) staff       (20)    10525 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)   150076 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/photosdb.py
--rw-r--r--   0 rhet       (501) staff       (20)     5681 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/photosdb/photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8828 2023-07-16 22:09:18.000000 osxphotos-0.60.8/osxphotos/phototables.py
--rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.8/osxphotos/phototemplate.cog.md
--rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-16 22:13:02.000000 osxphotos-0.60.8/osxphotos/phototemplate.md
--rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.8/osxphotos/phototemplate.py
--rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.8/osxphotos/phototemplate.tx
--rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/phototz.py
--rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.8/osxphotos/placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/platform.py
--rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.8/osxphotos/pyrepl.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.383245 osxphotos-0.60.8/osxphotos/queries/
--rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.8/osxphotos/queries/README.md
--rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.8/osxphotos/queries/cloud_album_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.8/osxphotos/queries/shared_owner.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.8/osxphotos/queries/title.sql.mako
--rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.8/osxphotos/query_builder.py
--rw-r--r--   0 rhet       (501) staff       (20)    14179 2023-06-19 14:34:40.000000 osxphotos-0.60.8/osxphotos/queryoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.8/osxphotos/rich_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/scoreinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/searchinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.8/osxphotos/sqlgrep.py
--rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.8/osxphotos/sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/template_counter.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.384316 osxphotos-0.60.8/osxphotos/templates/
--rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.8/osxphotos/templates/DESCRIPTION.txt
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/templates/xmp_sidecar.mako
--rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/templates/xmp_sidecar_beta.mako
--rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/text_detection.py
--rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.8/osxphotos/timeutils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/timezones.py
--rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.8/osxphotos/tutorial.md
--rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/uti.py
--rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.8/osxphotos/utils.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.360070 osxphotos-0.60.8/osxphotos.egg-info/
--rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/PKG-INFO
--rw-r--r--   0 rhet       (501) staff       (20)     6527 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/SOURCES.txt
--rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/dependency_links.txt
--rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/entry_points.txt
--rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/requires.txt
--rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-16 22:13:16.000000 osxphotos-0.60.8/osxphotos.egg-info/top_level.txt
--rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-16 22:13:16.398661 osxphotos-0.60.8/setup.cfg
--rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.8/setup.py
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.397793 osxphotos-0.60.8/tests/
-drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-16 22:13:16.398162 osxphotos-0.60.8/tests/plugins/
--rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.8/tests/plugins/__init__.py
--rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.8/tests/plugins/env_vars.py
--rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_10_12_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_albums_folders_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_bigsur_10_16_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.8/tests/test_cli.py
--rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_add_locations.py
--rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_add_to_album.py
--rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_all_commands.py
--rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_batch_edit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_dump.py
--rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.8/tests/test_cli_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_export_cloud.py
--rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.8/tests/test_cli_export_projects.py
--rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_exportdb.py
--rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_import.py
--rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_orphans.py
--rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_param_types.py
--rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_cli_sync.py
--rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_timewarp.py
--rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_cli_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_cli_verbose.py
--rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.8/tests/test_cloud_owner_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.8/tests/test_comments.py
--rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.8/tests/test_concurrent_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.8/tests/test_configoptions.py
--rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_datetime_formatter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_datetime_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_debug.py
--rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_empty_library_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.8/tests/test_exif_info.py
--rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_exiftool.py
--rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_exiftool_caching.py
--rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_export_catalina_10_15_7_use_photos_export.py
--rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.8/tests/test_export_convert_to_jpeg.py
--rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_db.py
--rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_export_raw_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_exportresults.py
--rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_faceinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_fileutil.py
--rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_highsierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_image_converter.py
--rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_incloud_big_sur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.8/tests/test_incloud_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_incloud_catalina_10_15_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_incloud_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.8/tests/test_live_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_modified_date_catalina_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_modified_date_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.8/tests/test_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_mojave_10_14_6_path_edited.py
--rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_monterey_12_0_1.py
--rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_monterey_dev_beta_12_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_movies_4_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_movies_5_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_path_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_personinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_photokit.py
--rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_photosalbum_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_photosdb_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_placeinfo.py
--rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_places_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.8/tests/test_places_high_sierra_10_13_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.8/tests/test_places_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.8/tests/test_projects_catalina.py
--rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.8/tests/test_projects_sierra.py
--rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_score_info.py
--rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_15_4.py
--rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_search_info_10_15_5.py
--rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_search_info_10_15_7.py
--rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_shared_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_shared_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_shared_ventura_13_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.8/tests/test_sidecar_xmp.py
--rw-r--r--   0 rhet       (501) staff       (20)    48444 2023-07-16 22:09:19.000000 osxphotos-0.60.8/tests/test_sonoma_14_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_specials_bigsur_10_16_0.py
--rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.8/tests/test_specials_catalina_10_15_1.py
--rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.8/tests/test_specials_mojave_10_14_6.py
--rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.8/tests/test_specials_sierra_10_12.py
--rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_sqlite_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_sqlitekvstore.py
--rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_template.py
--rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.8/tests/test_template_counter.py
--rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.8/tests/test_template_today.py
--rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_unicode.py
--rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.8/tests/test_uti.py
--rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.8/tests/test_utils.py
--rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.8/tests/test_ventura_13_0_0.py
--rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.8/tests/test_ventura_dev_preview_13_0_0.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.001562 osxphotos-0.60.9/
+-rw-r--r--   0 rhet       (501) staff       (20)     1075 2021-01-12 14:41:12.000000 osxphotos-0.60.9/LICENSE
+-rw-r--r--   0 rhet       (501) staff       (20)      212 2022-04-19 16:54:15.000000 osxphotos-0.60.9/MANIFEST.in
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-17 01:15:27.001150 osxphotos-0.60.9/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)   226697 2023-07-17 01:15:15.000000 osxphotos-0.60.9/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)    12887 2023-03-09 14:25:54.000000 osxphotos-0.60.9/README.rst
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.951934 osxphotos-0.60.9/osxphotos/
+-rw-r--r--   0 rhet       (501) staff       (20)     1981 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      118 2022-02-27 00:52:03.000000 osxphotos-0.60.9/osxphotos/__main__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17162 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/_constants.py
+-rw-r--r--   0 rhet       (501) staff       (20)       45 2023-07-17 01:15:06.000000 osxphotos-0.60.9/osxphotos/_version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5986 2022-01-22 17:23:57.000000 osxphotos-0.60.9/osxphotos/adjustmentsinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18200 2023-04-11 02:03:56.000000 osxphotos-0.60.9/osxphotos/albuminfo.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.961505 osxphotos-0.60.9/osxphotos/cli/
+-rw-r--r--   0 rhet       (501) staff       (20)     3568 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15763 2022-05-18 03:47:35.000000 osxphotos-0.60.9/osxphotos/cli/about.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6899 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1313 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/albums.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9936 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3727 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/cli/cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10147 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/cli_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27724 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/cli/cli_params.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8531 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/click_rich_echo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6843 2022-05-01 15:18:25.000000 osxphotos-0.60.9/osxphotos/cli/color_themes.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3585 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/common.py
+-rw-r--r--   0 rhet       (501) staff       (20)      715 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/darkmode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3615 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/debug_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2265 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/docs.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3452 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)    15185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/exiftool_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)   108212 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/cli/export.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17529 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/cli/exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1649 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/grep.py
+-rw-r--r--   0 rhet       (501) staff       (20)    22104 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/help.py
+-rw-r--r--   0 rhet       (501) staff       (20)    62220 2023-07-02 16:32:35.000000 osxphotos-0.60.9/osxphotos/cli/import_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2292 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2479 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/install_uninstall_run.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1103 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/keywords.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/kvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1106 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/labels.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1720 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/list.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5119 2023-02-12 16:12:07.000000 osxphotos-0.60.9/osxphotos/cli/orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9657 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1101 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/persons.py
+-rw-r--r--   0 rhet       (501) staff       (20)    20594 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/photo_inspect.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1860 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/places.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4585 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/print_photo_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5845 2023-06-24 17:50:43.000000 osxphotos-0.60.9/osxphotos/cli/query.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8757 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/repl.py
+-rw-r--r--   0 rhet       (501) staff       (20)    23058 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/cli/report_writer.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1930 2022-03-06 01:00:55.000000 osxphotos-0.60.9/osxphotos/cli/rich_progress.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3385 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/show_command.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5080 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/snap_diff.py
+-rw-r--r--   0 rhet       (501) staff       (20)    26965 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5675 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/sync_results.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4054 2022-04-18 05:53:56.000000 osxphotos-0.60.9/osxphotos/cli/theme.py
+-rw-r--r--   0 rhet       (501) staff       (20)    28075 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1212 2022-02-27 00:52:03.000000 osxphotos-0.60.9/osxphotos/cli/tutorial.py
+-rw-r--r--   0 rhet       (501) staff       (20)      695 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/cli/uuid.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8720 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/cli/verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1263 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/cli/version.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5111 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/compare_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8060 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2084 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/crash_reporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1631 2022-01-22 17:24:00.000000 osxphotos-0.60.9/osxphotos/datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6211 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3612 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/debug.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.962091 osxphotos-0.60.9/osxphotos/docs/
+-rw-r--r--   0 rhet       (501) staff       (20)      165 2022-05-24 06:26:41.000000 osxphotos-0.60.9/osxphotos/docs/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)  1479305 2023-07-17 01:15:23.000000 osxphotos-0.60.9/osxphotos/docs/docs.zip
+-rw-r--r--   0 rhet       (501) staff       (20)    13126 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/exif_datetime_updater.py
+-rw-r--r--   0 rhet       (501) staff       (20)      622 2022-01-22 17:22:59.000000 osxphotos-0.60.9/osxphotos/exifinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18945 2023-04-02 19:36:56.000000 osxphotos-0.60.9/osxphotos/exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)   116283 2022-02-07 05:54:46.000000 osxphotos-0.60.9/osxphotos/exiftool_filetypes.json
+-rw-r--r--   0 rhet       (501) staff       (20)    51792 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    19809 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/export_db_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10765 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5936 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/frozen_photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5124 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/imageconverter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2514 2022-05-04 05:28:10.000000 osxphotos-0.60.9/osxphotos/momentinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3789 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    16570 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9696 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/photodates.py
+-rw-r--r--   0 rhet       (501) staff       (20)    93623 2023-07-15 14:18:05.000000 osxphotos-0.60.9/osxphotos/photoexporter.py
+-rw-r--r--   0 rhet       (501) staff       (20)    87376 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/photoinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    46280 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6551 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosalbum.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5335 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photoscript_utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.964193 osxphotos-0.60.9/osxphotos/photosdb/
+-rw-r--r--   0 rhet       (501) staff       (20)      215 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5388 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1789 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_exif.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10525 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6082 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7578 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1687 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_syndicationinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)   150545 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/photosdb/photosdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5681 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/photosdb/photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8828 2023-07-16 22:09:18.000000 osxphotos-0.60.9/osxphotos/phototables.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9930 2022-05-28 01:33:26.000000 osxphotos-0.60.9/osxphotos/phototemplate.cog.md
+-rw-r--r--   0 rhet       (501) staff       (20)    13636 2023-07-17 01:15:14.000000 osxphotos-0.60.9/osxphotos/phototemplate.md
+-rw-r--r--   0 rhet       (501) staff       (20)    78791 2023-05-07 13:56:16.000000 osxphotos-0.60.9/osxphotos/phototemplate.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1899 2022-08-27 02:50:57.000000 osxphotos-0.60.9/osxphotos/phototemplate.tx
+-rw-r--r--   0 rhet       (501) staff       (20)     6680 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/phototz.py
+-rw-r--r--   0 rhet       (501) staff       (20)    25757 2023-07-03 07:44:41.000000 osxphotos-0.60.9/osxphotos/placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)      696 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/platform.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4486 2022-01-22 17:24:20.000000 osxphotos-0.60.9/osxphotos/pyrepl.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.965558 osxphotos-0.60.9/osxphotos/queries/
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2021-09-26 05:30:35.000000 osxphotos-0.60.9/osxphotos/queries/README.md
+-rw-r--r--   0 rhet       (501) staff       (20)      157 2021-09-26 03:53:10.000000 osxphotos-0.60.9/osxphotos/queries/cloud_album_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1139 2021-09-26 20:40:00.000000 osxphotos-0.60.9/osxphotos/queries/shared_owner.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)      231 2021-09-25 19:22:39.000000 osxphotos-0.60.9/osxphotos/queries/title.sql.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     1416 2022-01-22 17:22:59.000000 osxphotos-0.60.9/osxphotos/query_builder.py
+-rw-r--r--   0 rhet       (501) staff       (20)    14487 2023-07-17 01:14:39.000000 osxphotos-0.60.9/osxphotos/queryoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)      496 2022-03-06 05:45:15.000000 osxphotos-0.60.9/osxphotos/rich_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1144 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/scoreinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7866 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/searchinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2413 2023-05-07 14:33:19.000000 osxphotos-0.60.9/osxphotos/sqlgrep.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1813 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8064 2023-04-08 16:08:11.000000 osxphotos-0.60.9/osxphotos/sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4150 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/template_counter.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.968771 osxphotos-0.60.9/osxphotos/templates/
+-rw-r--r--   0 rhet       (501) staff       (20)      356 2021-01-20 23:58:08.000000 osxphotos-0.60.9/osxphotos/templates/DESCRIPTION.txt
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/templates/xmp_sidecar.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     6185 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/templates/xmp_sidecar_beta.mako
+-rw-r--r--   0 rhet       (501) staff       (20)     3245 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/text_detection.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2281 2023-06-18 23:22:55.000000 osxphotos-0.60.9/osxphotos/timeutils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3445 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/timezones.py
+-rw-r--r--   0 rhet       (501) staff       (20)    39982 2023-03-09 14:25:54.000000 osxphotos-0.60.9/osxphotos/tutorial.md
+-rw-r--r--   0 rhet       (501) staff       (20)     2607 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)    27216 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)    17290 2023-06-24 17:50:21.000000 osxphotos-0.60.9/osxphotos/utils.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:26.953863 osxphotos-0.60.9/osxphotos.egg-info/
+-rw-r--r--   0 rhet       (501) staff       (20)    13834 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/PKG-INFO
+-rw-r--r--   0 rhet       (501) staff       (20)     6527 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/SOURCES.txt
+-rw-r--r--   0 rhet       (501) staff       (20)        1 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/dependency_links.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       58 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/entry_points.txt
+-rw-r--r--   0 rhet       (501) staff       (20)      888 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/requires.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       16 2023-07-17 01:15:26.000000 osxphotos-0.60.9/osxphotos.egg-info/top_level.txt
+-rw-r--r--   0 rhet       (501) staff       (20)       38 2023-07-17 01:15:27.001674 osxphotos-0.60.9/setup.cfg
+-rwxr-xr-x   0 rhet       (501) staff       (20)     4378 2023-03-09 14:25:54.000000 osxphotos-0.60.9/setup.py
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.000543 osxphotos-0.60.9/tests/
+drwxr-xr-x   0 rhet       (501) staff       (20)        0 2023-07-17 01:15:27.000830 osxphotos-0.60.9/tests/plugins/
+-rw-r--r--   0 rhet       (501) staff       (20)        0 2022-03-06 06:50:07.000000 osxphotos-0.60.9/tests/plugins/__init__.py
+-rw-r--r--   0 rhet       (501) staff       (20)      167 2022-03-06 06:50:24.000000 osxphotos-0.60.9/tests/plugins/env_vars.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4550 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_10_12_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    11011 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4848 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5333 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_albums_folders_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43711 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_bigsur_10_16_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    54734 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)   275628 2023-07-15 14:18:05.000000 osxphotos-0.60.9/tests/test_cli.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1803 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_add_locations.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4575 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_add_to_album.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2225 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_all_commands.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6802 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_batch_edit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3675 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_dump.py
+-rw-r--r--   0 rhet       (501) staff       (20)     8091 2022-05-21 14:25:18.000000 osxphotos-0.60.9/tests/test_cli_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2914 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_export_cloud.py
+-rw-r--r--   0 rhet       (501) staff       (20)      670 2023-04-08 21:34:18.000000 osxphotos-0.60.9/tests/test_cli_export_projects.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1009 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_exportdb.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31269 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_import.py
+-rw-r--r--   0 rhet       (501) staff       (20)      953 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_orphans.py
+-rw-r--r--   0 rhet       (501) staff       (20)     6395 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_param_types.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3456 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_cli_sync.py
+-rw-r--r--   0 rhet       (501) staff       (20)    31670 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_timewarp.py
+-rw-r--r--   0 rhet       (501) staff       (20)      815 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_cli_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3056 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_cli_verbose.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1185 2021-09-26 04:07:28.000000 osxphotos-0.60.9/tests/test_cloud_owner_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2644 2021-09-26 20:50:17.000000 osxphotos-0.60.9/tests/test_comments.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2519 2023-04-08 16:08:11.000000 osxphotos-0.60.9/tests/test_concurrent_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2699 2023-02-05 16:52:41.000000 osxphotos-0.60.9/tests/test_configoptions.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1945 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_datetime_formatter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2750 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_datetime_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)      742 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_debug.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2212 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_empty_library_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2439 2022-01-02 15:24:11.000000 osxphotos-0.60.9/tests/test_exif_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18508 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_exiftool.py
+-rw-r--r--   0 rhet       (501) staff       (20)     9784 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_exiftool_caching.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18294 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5913 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_export_catalina_10_15_7_use_photos_export.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2836 2022-01-29 16:49:11.000000 osxphotos-0.60.9/tests/test_export_convert_to_jpeg.py
+-rw-r--r--   0 rhet       (501) staff       (20)    21901 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_db.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10298 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3892 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_export_raw_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2485 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_exportresults.py
+-rw-r--r--   0 rhet       (501) staff       (20)   155128 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_faceinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5148 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_fileutil.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3633 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_highsierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4014 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_image_converter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1211 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_incloud_big_sur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1327 2021-06-12 05:41:38.000000 osxphotos-0.60.9/tests/test_incloud_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1944 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_incloud_catalina_10_15_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1271 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_incloud_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3786 2021-06-12 05:44:48.000000 osxphotos-0.60.9/tests/test_live_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)      861 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_modified_date_catalina_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)      931 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_modified_date_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)    18573 2023-04-16 16:05:18.000000 osxphotos-0.60.9/tests/test_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1207 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_mojave_10_14_6_path_edited.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43641 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_monterey_12_0_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50371 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_monterey_dev_beta_12_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4733 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_movies_4_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4872 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_movies_5_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3779 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_path_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4377 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_personinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13434 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_photokit.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3080 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_photosalbum_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1460 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_photosdb_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    13801 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_placeinfo.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5795 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_places_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7224 2020-03-28 15:14:51.000000 osxphotos-0.60.9/tests/test_places_high_sierra_10_13_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3431 2020-10-27 13:36:55.000000 osxphotos-0.60.9/tests/test_places_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4762 2023-04-08 16:49:38.000000 osxphotos-0.60.9/tests/test_projects_catalina.py
+-rw-r--r--   0 rhet       (501) staff       (20)     4224 2021-12-31 05:42:49.000000 osxphotos-0.60.9/tests/test_projects_sierra.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3373 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_score_info.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3695 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7529 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_15_4.py
+-rw-r--r--   0 rhet       (501) staff       (20)    10046 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_search_info_10_15_5.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2191 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_search_info_10_15_7.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2791 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_shared_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     1744 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_shared_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)      441 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_shared_ventura_13_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2100 2022-01-29 16:49:32.000000 osxphotos-0.60.9/tests/test_sidecar_xmp.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48444 2023-07-16 22:09:19.000000 osxphotos-0.60.9/tests/test_sonoma_14_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3018 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_specials_bigsur_10_16_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2535 2020-03-08 17:47:46.000000 osxphotos-0.60.9/tests/test_specials_catalina_10_15_1.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2621 2020-03-28 14:53:05.000000 osxphotos-0.60.9/tests/test_specials_mojave_10_14_6.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2261 2020-03-08 19:17:16.000000 osxphotos-0.60.9/tests/test_specials_sierra_10_12.py
+-rw-r--r--   0 rhet       (501) staff       (20)      487 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_sqlite_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)     7328 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_sqlitekvstore.py
+-rw-r--r--   0 rhet       (501) staff       (20)    50020 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_template.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2432 2023-03-09 14:25:57.000000 osxphotos-0.60.9/tests/test_template_counter.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2346 2023-05-07 13:56:16.000000 osxphotos-0.60.9/tests/test_template_today.py
+-rw-r--r--   0 rhet       (501) staff       (20)     3158 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_unicode.py
+-rw-r--r--   0 rhet       (501) staff       (20)     2035 2023-06-24 17:50:21.000000 osxphotos-0.60.9/tests/test_uti.py
+-rw-r--r--   0 rhet       (501) staff       (20)     5514 2023-04-08 16:08:11.000000 osxphotos-0.60.9/tests/test_utils.py
+-rw-r--r--   0 rhet       (501) staff       (20)    48316 2023-04-16 16:05:18.000000 osxphotos-0.60.9/tests/test_ventura_13_0_0.py
+-rw-r--r--   0 rhet       (501) staff       (20)    43503 2023-06-18 23:22:55.000000 osxphotos-0.60.9/tests/test_ventura_dev_preview_13_0_0.py
```

### Comparing `osxphotos-0.60.8/LICENSE` & `osxphotos-0.60.9/LICENSE`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/PKG-INFO` & `osxphotos-0.60.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.8
+Version: 0.60.9
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.8/README.md` & `osxphotos-0.60.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -878,14 +878,18 @@
   --not-syndicated                Search for photos that have not been shared
                                   via syndication ('Shared with You' album via
                                   Messages, etc.)
   --saved-to-library              Search for syndicated photos that have saved
                                   to the library
   --not-saved-to-library          Search for syndicated photos that have not
                                   saved to the library
+  --shared-moment                 Search for photos that are part of a shared
+                                  moment
+  --not-shared-moment             Search for photos that are not part of a
+                                  shared moment
   --regex REGEX TEMPLATE          Search for photos where TEMPLATE matches
                                   regular expression REGEX. For example, to find
                                   photos in an album that begins with 'Beach': '
                                   --regex "^Beach" "{album}"'. You may specify
                                   more than one regular expression match by
                                   repeating '--regex' with different arguments.
   --selected                      Filter for photos that are currently selected
@@ -2116,15 +2120,15 @@
 {openbracket}                   An open bracket: '['
 {closebracket}                  A close bracket: ']'
 {newline}                       A newline: '\n'
 {lf}                            A line feed: '\n', alias for {newline}
 {cr}                            A carriage return: '\r'
 {crlf}                          A carriage return + line feed: '\r\n'
 {tab}                           :A tab: '\t'
-{osxphotos_version}             The osxphotos version, e.g. '0.60.8'
+{osxphotos_version}             The osxphotos version, e.g. '0.60.9'
 {osxphotos_cmd_line}            The full command line used to run osxphotos
 
 The following substitutions may result in multiple values. Thus if specified
 for --directory these could result in multiple copies of a photo being being
 exported, one to each directory.  For example: --directory
 '{created.year}/{album}' could result in the same photo being exported to each
 of the following directories if the photos were created in 2019 and were in
@@ -2603,15 +2607,15 @@
 |{openbracket}|An open bracket: '['|
 |{closebracket}|A close bracket: ']'|
 |{newline}|A newline: '\n'|
 |{lf}|A line feed: '\n', alias for {newline}|
 |{cr}|A carriage return: '\r'|
 |{crlf}|A carriage return + line feed: '\r\n'|
 |{tab}|:A tab: '\t'|
-|{osxphotos_version}|The osxphotos version, e.g. '0.60.8'|
+|{osxphotos_version}|The osxphotos version, e.g. '0.60.9'|
 |{osxphotos_cmd_line}|The full command line used to run osxphotos|
 |{album}|Album(s) photo is contained in|
 |{folder_album}|Folder path + album photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{project}|Project(s) photo is contained in (such as greeting cards, calendars, slideshows)|
 |{album_project}|Album(s) and project(s) photo is contained in; treats projects as regular albums|
 |{folder_album_project}|Folder path + album (includes projects as albums) photo is contained in. e.g. 'Folder/Subfolder/Album' or just 'Album' if no enclosing folder|
 |{keyword}|Keyword(s) assigned to photo|
```

### Comparing `osxphotos-0.60.8/README.rst` & `osxphotos-0.60.9/README.rst`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/__init__.py` & `osxphotos-0.60.9/osxphotos/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/_constants.py` & `osxphotos-0.60.9/osxphotos/_constants.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/adjustmentsinfo.py` & `osxphotos-0.60.9/osxphotos/adjustmentsinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/albuminfo.py` & `osxphotos-0.60.9/osxphotos/albuminfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/__init__.py` & `osxphotos-0.60.9/osxphotos/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/about.py` & `osxphotos-0.60.9/osxphotos/cli/about.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/add_locations.py` & `osxphotos-0.60.9/osxphotos/cli/add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/albums.py` & `osxphotos-0.60.9/osxphotos/cli/albums.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/batch_edit.py` & `osxphotos-0.60.9/osxphotos/cli/batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/cli.py` & `osxphotos-0.60.9/osxphotos/cli/cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/cli_commands.py` & `osxphotos-0.60.9/osxphotos/cli/cli_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/cli_params.py` & `osxphotos-0.60.9/osxphotos/cli/cli_params.py`

 * *Files 1% similar despite different names*

```diff
@@ -607,14 +607,24 @@
         help="Search for syndicated photos that have saved to the library",
     ),
     "--not-saved-to-library": click.Option(
         ["--not-saved-to-library"],
         is_flag=True,
         help="Search for syndicated photos that have not saved to the library",
     ),
+    "--shared-moment": click.Option(
+        ["--shared-moment"],
+        is_flag=True,
+        help="Search for photos that are part of a shared moment",
+    ),
+    "--not-shared-moment": click.Option(
+        ["--not-shared-moment"],
+        is_flag=True,
+        help="Search for photos that are not part of a shared moment",
+    ),
     "--regex": click.Option(
         ["--regex"],
         metavar="REGEX TEMPLATE",
         nargs=2,
         multiple=True,
         help="Search for photos where TEMPLATE matches regular expression REGEX. "
         "For example, to find photos in an album that begins with 'Beach': '--regex \"^Beach\" \"{album}\"'. "
```

### Comparing `osxphotos-0.60.8/osxphotos/cli/click_rich_echo.py` & `osxphotos-0.60.9/osxphotos/cli/click_rich_echo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/color_themes.py` & `osxphotos-0.60.9/osxphotos/cli/color_themes.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/common.py` & `osxphotos-0.60.9/osxphotos/cli/common.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/darkmode.py` & `osxphotos-0.60.9/osxphotos/cli/darkmode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/debug_dump.py` & `osxphotos-0.60.9/osxphotos/cli/debug_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/docs.py` & `osxphotos-0.60.9/osxphotos/cli/docs.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/dump.py` & `osxphotos-0.60.9/osxphotos/cli/dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/exiftool_cli.py` & `osxphotos-0.60.9/osxphotos/cli/exiftool_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/export.py` & `osxphotos-0.60.9/osxphotos/cli/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -890,14 +890,16 @@
     verbose_flag,
     xattr_template,
     year,
     syndicated,
     not_syndicated,
     saved_to_library,
     not_saved_to_library,
+    shared_moment,
+    not_shared_moment,
     selected=False,  # Isn't provided on unsupported platforms
     # debug,  # debug, watch, breakpoint handled in cli/__init__.py
     # watch,
     # breakpoint,
 ):
     """Export photos from the Photos database.
     Export path DEST is required.
@@ -1116,14 +1118,16 @@
         verbose_flag = cfg.verbose
         xattr_template = cfg.xattr_template
         year = cfg.year
         syndicated = cfg.syndicated
         not_syndicated = cfg.not_syndicated
         saved_to_library = cfg.saved_to_library
         not_saved_to_library = cfg.not_saved_to_library
+        shared_moment = cfg.shared_moment
+        not_shared_moment = cfg.not_shared_moment
 
         # config file might have changed verbose
         verbose = verbose_print(verbose=verbose_flag, timestamp=timestamp, theme=theme)
         verbose(f"Loaded options from file [filepath]{load_config}")
 
         set_crash_data("cfg", cfg.asdict())
 
@@ -1167,14 +1171,15 @@
         ("shared", "not_shared"),
         ("skip_edited", "skip_original_if_edited"),
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("title", "no_title"),
         ("syndicated", "not_syndicated"),
         ("saved_to_library", "not_saved_to_library"),
+        ("shared_moment", "not_shared_moment"),
     ]
     dependent_options = [
         ("append", ("report")),
         ("exiftool_merge_keywords", ("exiftool", "sidecar")),
         ("exiftool_merge_persons", ("exiftool", "sidecar")),
         ("exiftool_option", ("exiftool")),
         ("favorite_rating", ("exiftool", "sidecar")),
```

### Comparing `osxphotos-0.60.8/osxphotos/cli/exportdb.py` & `osxphotos-0.60.9/osxphotos/cli/exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/grep.py` & `osxphotos-0.60.9/osxphotos/cli/grep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/help.py` & `osxphotos-0.60.9/osxphotos/cli/help.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/import_cli.py` & `osxphotos-0.60.9/osxphotos/cli/import_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/info.py` & `osxphotos-0.60.9/osxphotos/cli/info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/install_uninstall_run.py` & `osxphotos-0.60.9/osxphotos/cli/install_uninstall_run.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/keywords.py` & `osxphotos-0.60.9/osxphotos/cli/keywords.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/kvstore.py` & `osxphotos-0.60.9/osxphotos/cli/kvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/labels.py` & `osxphotos-0.60.9/osxphotos/cli/labels.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/list.py` & `osxphotos-0.60.9/osxphotos/cli/list.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/orphans.py` & `osxphotos-0.60.9/osxphotos/cli/orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/param_types.py` & `osxphotos-0.60.9/osxphotos/cli/param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/persons.py` & `osxphotos-0.60.9/osxphotos/cli/persons.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/photo_inspect.py` & `osxphotos-0.60.9/osxphotos/cli/photo_inspect.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/places.py` & `osxphotos-0.60.9/osxphotos/cli/places.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/print_photo_info.py` & `osxphotos-0.60.9/osxphotos/cli/print_photo_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/query.py` & `osxphotos-0.60.9/osxphotos/cli/query.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/repl.py` & `osxphotos-0.60.9/osxphotos/cli/repl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/report_writer.py` & `osxphotos-0.60.9/osxphotos/cli/report_writer.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/rich_progress.py` & `osxphotos-0.60.9/osxphotos/cli/rich_progress.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/show_command.py` & `osxphotos-0.60.9/osxphotos/cli/show_command.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/snap_diff.py` & `osxphotos-0.60.9/osxphotos/cli/snap_diff.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/sync.py` & `osxphotos-0.60.9/osxphotos/cli/sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/sync_results.py` & `osxphotos-0.60.9/osxphotos/cli/sync_results.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/theme.py` & `osxphotos-0.60.9/osxphotos/cli/theme.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/timewarp.py` & `osxphotos-0.60.9/osxphotos/cli/timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/tutorial.py` & `osxphotos-0.60.9/osxphotos/cli/tutorial.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/uuid.py` & `osxphotos-0.60.9/osxphotos/cli/uuid.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/verbose.py` & `osxphotos-0.60.9/osxphotos/cli/verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/cli/version.py` & `osxphotos-0.60.9/osxphotos/cli/version.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/compare_exif.py` & `osxphotos-0.60.9/osxphotos/compare_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/configoptions.py` & `osxphotos-0.60.9/osxphotos/configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/crash_reporter.py` & `osxphotos-0.60.9/osxphotos/crash_reporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/datetime_formatter.py` & `osxphotos-0.60.9/osxphotos/datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/datetime_utils.py` & `osxphotos-0.60.9/osxphotos/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/debug.py` & `osxphotos-0.60.9/osxphotos/debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/docs/docs.zip` & `osxphotos-0.60.9/osxphotos/docs/docs.zip`

 * *Files 12% similar despite different names*

#### zipinfo {}

```diff
@@ -1,101 +1,101 @@
-Zip file size: 1477940 bytes, number of entries: 99
+Zip file size: 1479305 bytes, number of entries: 99
 -rw-r--r--  3.0 unx   331458 tx defN 23-Feb-12 16:23 docs/API_README.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:17 docs/_modules/
--rw-r--r--  3.0 unx    11779 tx defN 23-Jul-16 22:13 docs/_modules/index.html
+-rw-r--r--  3.0 unx    11779 tx defN 23-Jul-17 01:15 docs/_modules/index.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-06 02:15 docs/_modules/osxphotos/
 -rw-r--r--  3.0 unx   333770 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoexporter.html
 -rw-r--r--  3.0 unx   296439 tx defN 23-May-07 14:38 docs/_modules/osxphotos/phototemplate.html
 -rw-r--r--  3.0 unx   201029 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/export_db.html
 -rw-r--r--  3.0 unx    14791 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/scoreinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:55 docs/_modules/osxphotos/photoinfo/
 -rw-r--r--  3.0 unx    14017 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_exifinfo.html
 -rw-r--r--  3.0 unx   284197 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/_photoinfo_export.html
 -rw-r--r--  3.0 unx   195566 tx defN 21-Dec-11 03:36 docs/_modules/osxphotos/photoinfo/photoinfo.html
 -rw-r--r--  3.0 unx    33978 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_searchinfo.html
 -rw-r--r--  3.0 unx    17959 tx defN 21-Mar-22 05:50 docs/_modules/osxphotos/photoinfo/_photoinfo_scoreinfo.html
 -rw-r--r--  3.0 unx    43160 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/searchinfo.html
 -rw-r--r--  3.0 unx    52397 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/fileutil.html
--rw-r--r--  3.0 unx   314708 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/photoinfo.html
+-rw-r--r--  3.0 unx   321986 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/photoinfo.html
 -rw-r--r--  3.0 unx     5599 tx defN 22-Apr-21 04:10 docs/_modules/osxphotos/exifinfo.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Jan-16 03:03 docs/_modules/osxphotos/photosdb/
 -rw-r--r--  3.0 unx    29242 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosdb/_photosdb_process_comments.html
--rw-r--r--  3.0 unx   527258 tx defN 23-Jul-16 22:13 docs/_modules/osxphotos/photosdb/photosdb.html
+-rw-r--r--  3.0 unx   529210 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/photosdb/photosdb.html
 -rw-r--r--  3.0 unx    39730 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/photosalbum.html
 -rw-r--r--  3.0 unx    99009 tx defN 23-Jul-15 14:32 docs/_modules/osxphotos/placeinfo.html
 -rw-r--r--  3.0 unx    21299 tx defN 22-May-06 00:24 docs/_modules/osxphotos/momentinfo.html
 -rw-r--r--  3.0 unx    82289 tx defN 23-Apr-11 02:04 docs/_modules/osxphotos/albuminfo.html
 -rw-r--r--  3.0 unx    78750 tx defN 23-Apr-03 02:59 docs/_modules/osxphotos/exiftool.html
 -rw-r--r--  3.0 unx    26012 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/debug.html
--rw-r--r--  3.0 unx    61579 tx defN 23-Jun-24 17:51 docs/_modules/osxphotos/queryoptions.html
+-rw-r--r--  3.0 unx    62444 tx defN 23-Jul-17 01:15 docs/_modules/osxphotos/queryoptions.html
 -rw-r--r--  3.0 unx    80476 tx defN 23-Mar-09 14:49 docs/_modules/osxphotos/personinfo.html
 -rw-r--r--  3.0 unx    66040 tx defN 23-Jul-16 22:13 docs/_modules/osxphotos/_constants.html
 drwxr-xr-x  3.0 unx        0 bx stor 23-Feb-12 16:20 docs/_sources/
 -rw-r--r--  3.0 unx      198 tx defN 22-Apr-23 14:44 docs/_sources/cli.rst.txt
--rw-r--r--  3.0 unx    31854 tx defN 23-Jul-16 22:13 docs/_sources/template_help.rst.txt
+-rw-r--r--  3.0 unx    31854 tx defN 23-Jul-17 01:15 docs/_sources/template_help.rst.txt
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
--rw-r--r--  3.0 unx      421 tx defN 23-Jul-16 22:13 docs/_static/documentation_options.js
+-rw-r--r--  3.0 unx      421 tx defN 23-Jul-17 01:15 docs/_static/documentation_options.js
 -rw-r--r--  3.0 unx    18215 tx defN 22-Nov-13 03:13 docs/_static/searchtools.js
 -rw-r--r--  3.0 unx     1266 tx defN 22-Nov-13 03:13 docs/_static/debug.css
 -rw-r--r--  3.0 unx      313 tx defN 22-Apr-21 05:12 docs/_static/check-solid.svg
 -rw-r--r--  3.0 unx     9031 tx defN 22-Apr-21 05:12 docs/_static/clipboard.min.js
 -rw-r--r--  3.0 unx      286 bx stor 21-Mar-14 19:14 docs/_static/file.png
 -rw-r--r--  3.0 unx     4418 tx defN 22-Nov-13 03:13 docs/_static/_sphinx_javascript_frameworks_compat.js
--rw-r--r--  3.0 unx     8472 tx defN 23-Jul-16 22:13 docs/_static/copybutton.js
+-rw-r--r--  3.0 unx     8472 tx defN 23-Jul-17 01:15 docs/_static/copybutton.js
 -rw-r--r--  3.0 unx   287630 tx defN 21-Mar-14 19:14 docs/_static/jquery-3.5.1.js
 -rw-r--r--  3.0 unx       42 tx stor 21-Mar-14 19:14 docs/_static/custom.css
--rw-r--r--  3.0 unx     4758 tx defN 23-Jul-16 22:13 docs/_static/language_data.js
+-rw-r--r--  3.0 unx     4758 tx defN 23-Jul-17 01:15 docs/_static/language_data.js
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
--rw-r--r--  3.0 unx    14810 tx defN 23-Jul-16 22:13 docs/_static/basic.css
+-rw-r--r--  3.0 unx    14810 tx defN 23-Jul-17 01:15 docs/_static/basic.css
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:21 docs/_static/scripts/
 -rw-r--r--  3.0 unx      187 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js.LICENSE.txt
 -rw-r--r--  3.0 unx    28242 tx defN 22-Nov-13 03:13 docs/_static/scripts/furo.js.map
 -rw-r--r--  3.0 unx        0 bx stor 22-Apr-21 04:34 docs/_static/scripts/furo-extensions.js
 -rw-r--r--  3.0 unx     5265 tx defN 22-Apr-21 04:34 docs/_static/scripts/furo.js
--rw-r--r--  3.0 unx    21072 tx defN 23-Jul-16 22:13 docs/_static/pygments.css
+-rw-r--r--  3.0 unx    21072 tx defN 23-Jul-17 01:15 docs/_static/pygments.css
 -rw-r--r--  3.0 unx     2060 tx defN 22-Dec-03 06:57 docs/_static/copybutton.css
 -rw-r--r--  3.0 unx     4472 tx defN 22-Nov-13 03:13 docs/_static/doctools.js
 -rw-r--r--  3.0 unx    67692 tx defN 21-Mar-14 19:14 docs/_static/underscore-1.12.0.js
 -rw-r--r--  3.0 unx    89501 tx defN 22-Nov-13 03:13 docs/_static/jquery.js
 -rw-r--r--  3.0 unx    68420 tx defN 21-Jun-05 18:07 docs/_static/underscore-1.13.1.js
--rw-r--r--  3.0 unx   423876 tx defN 23-Jul-16 22:13 docs/cli.html
+-rw-r--r--  3.0 unx   428174 tx defN 23-Jul-17 01:15 docs/cli.html
 -rw-r--r--  3.0 unx    85854 tx defN 22-Apr-21 04:30 docs/cli_export.html
--rw-r--r--  3.0 unx   252162 tx defN 23-Jul-16 22:13 docs/genindex.html
--rw-r--r--  3.0 unx   110079 tx defN 23-Jul-16 22:13 docs/index.html
+-rw-r--r--  3.0 unx   254995 tx defN 23-Jul-17 01:15 docs/genindex.html
+-rw-r--r--  3.0 unx   110750 tx defN 23-Jul-17 01:15 docs/index.html
 -rw-r--r--  3.0 unx     2984 tx defN 22-Apr-20 14:01 docs/modules.html
--rw-r--r--  3.0 unx     9767 bx stor 23-Jul-16 22:13 docs/objects.inv
+-rw-r--r--  3.0 unx     9859 bx stor 23-Jul-17 01:15 docs/objects.inv
 -rw-r--r--  3.0 unx   267506 bx defN 21-May-10 00:50 docs/osxphotos.pdf
--rw-r--r--  3.0 unx    26446 tx defN 23-Jul-16 22:13 docs/overview.html
--rw-r--r--  3.0 unx    32469 tx defN 23-Jul-16 22:13 docs/package_overview.html
--rw-r--r--  3.0 unx    10831 tx defN 23-Jul-16 22:13 docs/py-modindex.html
--rw-r--r--  3.0 unx   468865 tx defN 23-Jul-16 22:13 docs/reference.html
+-rw-r--r--  3.0 unx    26446 tx defN 23-Jul-17 01:15 docs/overview.html
+-rw-r--r--  3.0 unx    32469 tx defN 23-Jul-17 01:15 docs/package_overview.html
+-rw-r--r--  3.0 unx    10831 tx defN 23-Jul-17 01:15 docs/py-modindex.html
+-rw-r--r--  3.0 unx   472096 tx defN 23-Jul-17 01:15 docs/reference.html
 drwxr-xr-x  3.0 unx        0 bx stor 22-Dec-04 07:53 docs/screencast/
 -rw-r--r--  3.0 unx     8007 tx defN 21-Jan-24 17:13 docs/screencast/terminalizer-demo.yml
 -rw-r--r--  3.0 unx    77927 bx defN 21-Jan-24 17:13 docs/screencast/osx-screenshot.png
 -rw-r--r--  3.0 unx   224316 bx defN 21-Jan-24 17:13 docs/screencast/demo.gif
--rw-r--r--  3.0 unx    10567 tx defN 23-Jul-16 22:13 docs/search.html
--rw-r--r--  3.0 unx   223524 tx defN 23-Jul-16 22:13 docs/searchindex.js
--rw-r--r--  3.0 unx    64566 tx defN 23-Jul-16 22:13 docs/template_help.html
--rw-r--r--  3.0 unx    84995 tx defN 23-Jul-16 22:13 docs/tutorial.html
-99 files, 7016013 bytes uncompressed, 1459208 bytes compressed:  79.2%
+-rw-r--r--  3.0 unx    10567 tx defN 23-Jul-17 01:15 docs/search.html
+-rw-r--r--  3.0 unx   225831 tx defN 23-Jul-17 01:15 docs/searchindex.js
+-rw-r--r--  3.0 unx    64566 tx defN 23-Jul-17 01:15 docs/template_help.html
+-rw-r--r--  3.0 unx    84995 tx defN 23-Jul-17 01:15 docs/tutorial.html
+99 files, 7039540 bytes uncompressed, 1460573 bytes compressed:  79.3%
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
-        <title>Overview: module code - osxphotos 0.60.8 documentation</title>
+        <title>Overview: module code - osxphotos 0.60.9 documentation</title>
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
-      <a href="../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

#### docs/_modules/osxphotos/photoinfo.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.photoinfo - osxphotos 0.60.7 documentation</title>
+        <title>osxphotos.photoinfo - osxphotos 0.60.9 documentation</title>
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
-      <a href="../../index.html"><div class="brand">osxphotos 0.60.7 documentation</div></a>
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.7 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -366,14 +366,20 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_path</span> <span class="o">=</span> <span class="n">photopath</span>
             <span class="k">return</span> <span class="n">photopath</span>
 
     <span class="k">def</span> <span class="nf">_path_5</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns candidate path for original photo on Photos &gt;= version 5&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;shared&quot;</span><span class="p">]:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_5_shared</span><span class="p">()</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_shared_moment</span><span class="p">():</span>
+            <span class="c1"># path for photos in shared moments if it&#39;s in the shared moment folder</span>
+            <span class="c1"># the file may also be in the originals folder which the next check will catch</span>
+            <span class="c1"># check shared_moment first as a photo can be both a shared moment and syndicated</span>
+            <span class="c1"># and if so, will be in the shared moment folder</span>
+            <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_shared_moment</span><span class="p">()</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
             <span class="c1"># path for &quot;shared with you&quot; syndicated photos that have not yet been saved to the library</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_syndication</span><span class="p">()</span>
         <span class="k">return</span> <span class="p">(</span>
             <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">],</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;filename&quot;</span><span class="p">])</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;directory&quot;</span><span class="p">]</span><span class="o">.</span><span class="n">startswith</span><span class="p">(</span><span class="s2">&quot;/&quot;</span><span class="p">)</span>
             <span class="k">else</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
@@ -423,14 +429,29 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">syndication_path</span><span class="p">,</span>
             <span class="n">uuid_dir</span><span class="p">,</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
         <span class="k">return</span> <span class="n">path</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
 
+    <span class="k">def</span> <span class="nf">_path_shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for shared moment photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 8+ stores shared moment photos in a separate directory</span>
+        <span class="c1"># in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID.ext</span>
+        <span class="c1"># where X is first digit of UUID</span>
+        <span class="n">momentshared_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/originals&quot;</span>
+        <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+        <span class="n">path</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
+            <span class="n">momentshared_path</span><span class="p">,</span>
+            <span class="n">uuid_dir</span><span class="p">,</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">,</span>
+        <span class="p">)</span>
+        <span class="k">return</span> <span class="n">path</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">path</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
+
     <span class="k">def</span> <span class="nf">_path_4</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;Returns candidate path for original photo on Photos &lt;= version 4&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;has_raw&quot;</span><span class="p">]:</span>
             <span class="c1"># return the path to JPEG even if RAW is original</span>
             <span class="n">vol</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_dbvolumes</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;raw_pair_info&quot;</span><span class="p">][</span><span class="s2">&quot;volumeId&quot;</span><span class="p">]]</span>
                 <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;raw_pair_info&quot;</span><span class="p">][</span><span class="s2">&quot;volumeId&quot;</span><span class="p">]</span> <span class="ow">is</span> <span class="ow">not</span> <span class="kc">None</span>
@@ -1103,14 +1124,16 @@
 
         <span class="n">photopath</span> <span class="o">=</span> <span class="kc">None</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_4</span><span class="p">()</span>
         <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">live_photo</span> <span class="ow">and</span> <span class="bp">self</span><span class="o">.</span><span class="n">path</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">ismissing</span><span class="p">:</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_photo_shared_5</span><span class="p">()</span>
+            <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">:</span>
+                <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_shared_moment</span><span class="p">()</span>
             <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
                 <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
                 <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_live_syndicated</span><span class="p">()</span>
 
             <span class="n">filename</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">path</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="n">filename</span><span class="o">.</span><span class="n">parent</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">filename</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span><span class="p">)</span>
             <span class="n">photopath</span> <span class="o">=</span> <span class="nb">str</span><span class="p">(</span><span class="n">photopath</span><span class="p">)</span>
@@ -1180,37 +1203,63 @@
             <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
             <span class="n">syndication_path</span><span class="p">,</span>
             <span class="n">uuid_dir</span><span class="p">,</span>
             <span class="n">filename</span><span class="p">,</span>
         <span class="p">)</span>
         <span class="k">return</span> <span class="n">live_photo</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">live_photo</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
 
+    <span class="k">def</span> <span class="nf">_path_live_shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
+        <span class="sd">&quot;&quot;&quot;Return path for live shared moment photo on Photos &gt;= version 8&quot;&quot;&quot;</span>
+        <span class="c1"># Photos 8+ stores live shared moment photos in a separate directory</span>
+        <span class="c1"># in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID_3.mov</span>
+        <span class="c1"># where X is first digit of UUID</span>
+        <span class="n">shared_moment_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/originals&quot;</span>
+        <span class="n">uuid_dir</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
+        <span class="n">filename</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">filename</span><span class="p">)</span><span class="o">.</span><span class="n">stem</span><span class="si">}</span><span class="s2">_3.mov&quot;</span>
+        <span class="n">live_photo</span> <span class="o">=</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">join</span><span class="p">(</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">,</span>
+            <span class="n">shared_moment_path</span><span class="p">,</span>
+            <span class="n">uuid_dir</span><span class="p">,</span>
+            <span class="n">filename</span><span class="p">,</span>
+        <span class="p">)</span>
+        <span class="k">return</span> <span class="n">live_photo</span> <span class="k">if</span> <span class="n">os</span><span class="o">.</span><span class="n">path</span><span class="o">.</span><span class="n">isfile</span><span class="p">(</span><span class="n">live_photo</span><span class="p">)</span> <span class="k">else</span> <span class="kc">None</span>
+
     <span class="nd">@cached_property</span>
     <span class="k">def</span> <span class="nf">path_derivatives</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">list</span><span class="p">[</span><span class="nb">str</span><span class="p">]:</span>
         <span class="sd">&quot;&quot;&quot;Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)&quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_4</span><span class="p">()</span>
 
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_path_derivatives_5_shared</span><span class="p">()</span>
 
         <span class="n">directory</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_uuid</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>  <span class="c1"># first char of uuid</span>
-        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
+        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">:</span>
+            <span class="c1"># shared moments</span>
+            <span class="n">derivative_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/momentshared/resources/derivatives&quot;</span>
+            <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
+                <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">derivative_path</span><span class="si">}</span><span class="s2">/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
+            <span class="p">)</span>
+        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
             <span class="c1"># syndicated (&quot;Shared with you&quot;) photos not yet saved to library</span>
             <span class="n">derivative_path</span> <span class="o">=</span> <span class="s2">&quot;scopes/syndication/resources/derivatives&quot;</span>
             <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">derivative_path</span><span class="si">}</span><span class="s2">/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
             <span class="p">)</span>
         <span class="k">else</span><span class="p">:</span>
-            <span class="n">derivative_path</span> <span class="o">=</span> <span class="sa">f</span><span class="s2">&quot;resources/derivatives/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">&quot;</span>
+            <span class="n">derivative_path</span> <span class="o">=</span> <span class="s2">&quot;resources/derivatives&quot;</span>
             <span class="n">thumb_path</span> <span class="o">=</span> <span class="p">(</span>
                 <span class="sa">f</span><span class="s2">&quot;resources/derivatives/masters/</span><span class="si">{</span><span class="n">directory</span><span class="si">}</span><span class="s2">/</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">_4_5005_c.jpeg&quot;</span>
             <span class="p">)</span>
 
-        <span class="n">derivative_path</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">derivative_path</span><span class="p">)</span>
+        <span class="n">derivative_path</span> <span class="o">=</span> <span class="p">(</span>
+            <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span>
+            <span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">derivative_path</span><span class="p">)</span>
+            <span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">directory</span><span class="p">)</span>
+        <span class="p">)</span>
         <span class="n">thumb_path</span> <span class="o">=</span> <span class="n">pathlib</span><span class="o">.</span><span class="n">Path</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_library_path</span><span class="p">)</span><span class="o">.</span><span class="n">joinpath</span><span class="p">(</span><span class="n">thumb_path</span><span class="p">)</span>
 
         <span class="c1"># find all files that start with uuid in derivative path</span>
         <span class="n">files</span> <span class="o">=</span> <span class="nb">list</span><span class="p">(</span><span class="n">derivative_path</span><span class="o">.</span><span class="n">glob</span><span class="p">(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="si">}</span><span class="s2">*.*&quot;</span><span class="p">))</span>
 
         <span class="c1"># previews may be missing from derivatives path</span>
         <span class="c1"># there are what appear to be low res thumbnails in the &quot;masters&quot; subfolder</span>
@@ -1570,14 +1619,19 @@
             <span class="k">return</span> <span class="kc">None</span>
 
         <span class="k">try</span><span class="p">:</span>
             <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_syndication_uuid</span><span class="p">[</span><span class="bp">self</span><span class="o">.</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;syndication_history&quot;</span><span class="p">]</span> <span class="o">!=</span> <span class="mi">0</span>
         <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
             <span class="k">return</span> <span class="kc">False</span>
 
+    <span class="nd">@cached_property</span>
+    <span class="k">def</span> <span class="nf">shared_moment</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="nb">bool</span><span class="p">:</span>
+        <span class="sd">&quot;&quot;&quot;Returns True if photo is part of a shared moment otherwise False&quot;&quot;&quot;</span>
+        <span class="k">return</span> <span class="nb">bool</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">_info</span><span class="p">[</span><span class="s2">&quot;moment_share&quot;</span><span class="p">])</span>
+
     <span class="nd">@property</span>
     <span class="k">def</span> <span class="nf">labels</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="sd">&quot;&quot;&quot;returns list of labels applied to photo by Photos image categorization</span>
 <span class="sd">        only valid on Photos 5, on older libraries returns empty list</span>
 <span class="sd">        &quot;&quot;&quot;</span>
         <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">_db</span><span class="o">.</span><span class="n">_db_version</span> <span class="o">&lt;=</span> <span class="n">_PHOTOS_4_VERSION</span><span class="p">:</span>
             <span class="k">return</span> <span class="p">[]</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.7_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -211,14 +211,23 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
+        if self.shared_moment and self._path_shared_moment():
+            # path for photos in shared moments if it's in the shared moment
+folder
+            # the file may also be in the originals folder which the next check
+will catch
+            # check shared_moment first as a photo can be both a shared moment
+and syndicated
+            # and if so, will be in the shared moment folder
+            return self._path_shared_moment()
         if self.syndicated and not self.saved_to_library:
             # path for "shared with you" syndicated photos that have not yet
 been saved to the library
             return self._path_syndication()
         return (
             os.path.join(self._info["directory"], self._info["filename"])
             if self._info["directory"].startswith("/")
@@ -270,14 +279,30 @@
             self._db._library_path,
             syndication_path,
             uuid_dir,
             self.filename,
         )
         return path if os.path.isfile(path) else None
 
+    def _path_shared_moment(self):
+        """Return path for shared moment photo on Photos >= version 8"""
+        # Photos 8+ stores shared moment photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/
+UUID.ext
+        # where X is first digit of UUID
+        momentshared_path = "scopes/momentshared/originals"
+        uuid_dir = self.uuid[0]
+        path = os.path.join(
+            self._db._library_path,
+            momentshared_path,
+            uuid_dir,
+            self.filename,
+        )
+        return path if os.path.isfile(path) else None
+
     def _path_4(self):
         """Returns candidate path for original photo on Photos <= version 4"""
         if self._info["has_raw"]:
             # return the path to JPEG even if RAW is original
             vol = (
                 self._db._dbvolumes[self._info["raw_pair_info"]["volumeId"]]
                 if self._info["raw_pair_info"]["volumeId"] is not None
@@ -1003,14 +1028,16 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
+            if self.shared_moment:
+                return self._path_live_shared_moment()
             if self.syndicated and not self.saved_to_library:
                 # syndicated ("Shared with you") photos not yet saved to
 library
                 return self._path_live_syndicated()
 
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
@@ -1085,41 +1112,68 @@
             self._db._library_path,
             syndication_path,
             uuid_dir,
             filename,
         )
         return live_photo if os.path.isfile(live_photo) else None
 
+    def _path_live_shared_moment(self):
+        """Return path for live shared moment photo on Photos >= version 8"""
+        # Photos 8+ stores live shared moment photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/
+UUID_3.mov
+        # where X is first digit of UUID
+        shared_moment_path = "scopes/momentshared/originals"
+        uuid_dir = self.uuid[0]
+        filename = f"{pathlib.Path(self.filename).stem}_3.mov"
+        live_photo = os.path.join(
+            self._db._library_path,
+            shared_moment_path,
+            uuid_dir,
+            filename,
+        )
+        return live_photo if os.path.isfile(live_photo) else None
+
     @cached_property
     def path_derivatives(self) -> list[str]:
         """Return any derivative (preview) images associated with the photo as
 a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        if self.syndicated and not self.saved_to_library:
+        if self.shared_moment:
+            # shared moments
+            derivative_path = "scopes/momentshared/resources/derivatives"
+            thumb_path = (
+                f"{derivative_path}/masters/{directory}/
+{self.uuid}_4_5005_c.jpeg"
+            )
+        elif self.syndicated and not self.saved_to_library:
             # syndicated ("Shared with you") photos not yet saved to library
             derivative_path = "scopes/syndication/resources/derivatives"
             thumb_path = (
                 f"{derivative_path}/masters/{directory}/
 {self.uuid}_4_5005_c.jpeg"
             )
         else:
-            derivative_path = f"resources/derivatives/{directory}"
+            derivative_path = "resources/derivatives"
             thumb_path = (
                 f"resources/derivatives/masters/{directory}/
 {self.uuid}_4_5005_c.jpeg"
             )
 
-        derivative_path = pathlib.Path(self._db._library_path).joinpath
-(derivative_path)
+        derivative_path = (
+            pathlib.Path(self._db._library_path)
+            .joinpath(derivative_path)
+            .joinpath(directory)
+        )
         thumb_path = pathlib.Path(self._db._library_path).joinpath(thumb_path)
 
         # find all files that start with uuid in derivative path
         files = list(derivative_path.glob(f"{self.uuid}*.*"))
 
         # previews may be missing from derivatives path
         # there are what appear to be low res thumbnails in the "masters"
@@ -1509,14 +1563,19 @@
 
         try:
             return self._db._db_syndication_uuid[self.uuid]
 ["syndication_history"] != 0
         except KeyError:
             return False
 
+    @cached_property
+    def shared_moment(self) -> bool:
+        """Returns True if photo is part of a shared moment otherwise False"""
+        return bool(self._info["moment_share"])
+
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image
 categorization
         only valid on Photos 5, on older libraries returns empty list
         """
         if self._db._db_version <= _PHOTOS_4_VERSION:
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
-        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.8 documentation</title>
+        <title>osxphotos.photosdb.photosdb - osxphotos 0.60.9 documentation</title>
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
-      <a href="../../../index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="../../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1428,14 +1428,17 @@
 
             <span class="c1"># fingerprint</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;masterFingerprint&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">45</span><span class="p">]</span>
 
             <span class="c1"># photos 5+ only, for shared photos</span>
             <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;cloudownerhashedpersonid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
+            <span class="c1"># photos 8+ only, shared moments</span>
+            <span class="bp">self</span><span class="o">.</span><span class="n">_dbphotos</span><span class="p">[</span><span class="n">uuid</span><span class="p">][</span><span class="s2">&quot;moment_share&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+
             <span class="c1"># compute signatures for finding possible duplicates</span>
             <span class="n">signature</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">_duplicate_signature</span><span class="p">(</span><span class="n">uuid</span><span class="p">)</span>
             <span class="k">try</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db_signatures</span><span class="p">[</span><span class="n">signature</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">uuid</span><span class="p">)</span>
             <span class="k">except</span> <span class="ne">KeyError</span><span class="p">:</span>
                 <span class="bp">self</span><span class="o">.</span><span class="n">_db_signatures</span><span class="p">[</span><span class="n">signature</span><span class="p">]</span> <span class="o">=</span> <span class="p">[</span><span class="n">uuid</span><span class="p">]</span>
 
@@ -2142,15 +2145,16 @@
 <span class="s2">                </span><span class="si">{</span><span class="n">depth_state</span><span class="si">}</span><span class="s2">,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZADJUSTMENTTIMESTAMP,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZVISIBILITYSTATE,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZTRASHEDDATE,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZSAVEDASSETTYPE,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZADDEDDATE,</span>
 <span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK,</span>
-<span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZCLOUDOWNERHASHEDPERSONID</span>
+<span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZCLOUDOWNERHASHEDPERSONID,</span>
+<span class="s2">                </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZMOMENTSHARE</span>
 <span class="s2">                FROM </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2"> </span>
 <span class="s2">                JOIN ZADDITIONALASSETATTRIBUTES ON ZADDITIONALASSETATTRIBUTES.ZASSET = </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.Z_PK </span>
 <span class="s2">                ORDER BY </span><span class="si">{</span><span class="n">asset_table</span><span class="si">}</span><span class="s2">.ZUUID  &quot;&quot;&quot;</span>
         <span class="p">)</span>
         <span class="c1"># Order of results</span>
         <span class="c1"># 0    SELECT ZGENERICASSET.ZUUID,</span>
         <span class="c1"># 1    ZADDITIONALASSETATTRIBUTES.ZMASTERFINGERPRINT,</span>
@@ -2193,14 +2197,15 @@
         <span class="c1"># 37   ZGENERICASSET.ZADJUSTMENTTIMESTAMP -- when was photo edited?</span>
         <span class="c1"># 38   ZGENERICASSET.ZVISIBILITYSTATE -- 0 if visible, 2 if not (e.g. a burst image)</span>
         <span class="c1"># 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or null if not in trash</span>
         <span class="c1"># 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported</span>
         <span class="c1"># 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library</span>
         <span class="c1"># 42   ZGENERICASSET.Z_PK -- primary key</span>
         <span class="c1"># 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner name (for shared photos)</span>
+        <span class="c1"># 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)</span>
 
         <span class="k">for</span> <span class="n">row</span> <span class="ow">in</span> <span class="n">c</span><span class="p">:</span>
             <span class="n">uuid</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span>
             <span class="n">info</span> <span class="o">=</span> <span class="p">{}</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;_uuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">uuid</span>  <span class="c1"># stored here for easier debugging</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;modelID&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;masterUuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
@@ -2380,14 +2385,16 @@
                 <span class="n">info</span><span class="p">[</span><span class="s2">&quot;added_date&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">datetime</span><span class="o">.</span><span class="n">fromtimestamp</span><span class="p">(</span><span class="n">row</span><span class="p">[</span><span class="mi">41</span><span class="p">]</span> <span class="o">+</span> <span class="n">TIME_DELTA</span><span class="p">)</span>
             <span class="k">except</span> <span class="p">(</span><span class="ne">ValueError</span><span class="p">,</span> <span class="ne">TypeError</span><span class="p">):</span>
                 <span class="n">info</span><span class="p">[</span><span class="s2">&quot;added_date&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">datetime</span><span class="p">(</span><span class="mi">1970</span><span class="p">,</span> <span class="mi">1</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span>
 
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;pk&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">42</span><span class="p">]</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;cloudownerhashedpersonid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">43</span><span class="p">]</span>
 
+            <span class="n">info</span><span class="p">[</span><span class="s2">&quot;moment_share&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="n">row</span><span class="p">[</span><span class="mi">44</span><span class="p">]</span>
+
             <span class="c1"># initialize import session info which will be filled in later</span>
             <span class="c1"># not every photo has an import session so initialize all records now</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;import_session&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;fok_import_session&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
             <span class="n">info</span><span class="p">[</span><span class="s2">&quot;import_uuid&quot;</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
             <span class="c1"># associated RAW image info</span>
@@ -3725,14 +3732,19 @@
             <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span><span class="p">]</span>
 
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">:</span>
             <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="n">p</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">]</span>
         <span class="k">elif</span> <span class="n">options</span><span class="o">.</span><span class="n">not_saved_to_library</span><span class="p">:</span>
             <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">syndicated</span> <span class="ow">and</span> <span class="ow">not</span> <span class="n">p</span><span class="o">.</span><span class="n">saved_to_library</span><span class="p">]</span>
 
+        <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="n">p</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">]</span>
+        <span class="k">elif</span> <span class="n">options</span><span class="o">.</span><span class="n">not_shared_moment</span><span class="p">:</span>
+            <span class="n">photos</span> <span class="o">=</span> <span class="p">[</span><span class="n">p</span> <span class="k">for</span> <span class="n">p</span> <span class="ow">in</span> <span class="n">photos</span> <span class="k">if</span> <span class="ow">not</span> <span class="n">p</span><span class="o">.</span><span class="n">shared_moment</span><span class="p">]</span>
+
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">function</span><span class="p">:</span>
             <span class="k">for</span> <span class="n">function</span> <span class="ow">in</span> <span class="n">options</span><span class="o">.</span><span class="n">function</span><span class="p">:</span>
                 <span class="n">photos</span> <span class="o">=</span> <span class="n">function</span><span class="p">[</span><span class="mi">0</span><span class="p">](</span><span class="n">photos</span><span class="p">)</span>
 
         <span class="c1"># burst should be checked last, ref #640</span>
         <span class="k">if</span> <span class="n">options</span><span class="o">.</span><span class="n">burst_photos</span><span class="p">:</span>
             <span class="c1"># add the burst_photos to the export set</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1370,14 +1370,17 @@
 
             # fingerprint
             self._dbphotos[uuid]["masterFingerprint"] = row[45]
 
             # photos 5+ only, for shared photos
             self._dbphotos[uuid]["cloudownerhashedpersonid"] = None
 
+            # photos 8+ only, shared moments
+            self._dbphotos[uuid]["moment_share"] = None
+
             # compute signatures for finding possible duplicates
             signature = self._duplicate_signature(uuid)
             try:
                 self._db_signatures[signature].append(uuid)
             except KeyError:
                 self._db_signatures[signature] = [uuid]
 
@@ -2121,15 +2124,16 @@
                 {depth_state},
                 {asset_table}.ZADJUSTMENTTIMESTAMP,
                 {asset_table}.ZVISIBILITYSTATE,
                 {asset_table}.ZTRASHEDDATE,
                 {asset_table}.ZSAVEDASSETTYPE,
                 {asset_table}.ZADDEDDATE,
                 {asset_table}.Z_PK,
-                {asset_table}.ZCLOUDOWNERHASHEDPERSONID
+                {asset_table}.ZCLOUDOWNERHASHEDPERSONID,
+                {asset_table}.ZMOMENTSHARE
                 FROM {asset_table}
                 JOIN ZADDITIONALASSETATTRIBUTES ON
 ZADDITIONALASSETATTRIBUTES.ZASSET = {asset_table}.Z_PK
                 ORDER BY {asset_table}.ZUUID  """
         )
         # Order of results
         # 0    SELECT ZGENERICASSET.ZUUID,
@@ -2182,14 +2186,15 @@
         # 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or
 null if not in trash
         # 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported
         # 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library
         # 42   ZGENERICASSET.Z_PK -- primary key
         # 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner
 name (for shared photos)
+        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)
 
         for row in c:
             uuid = row[0]
             info = {}
             info["_uuid"] = uuid  # stored here for easier debugging
             info["modelID"] = None
             info["masterUuid"] = None
@@ -2378,14 +2383,16 @@
 TIME_DELTA)
             except (ValueError, TypeError):
                 info["added_date"] = datetime(1970, 1, 1)
 
             info["pk"] = row[42]
             info["cloudownerhashedpersonid"] = row[43]
 
+            info["moment_share"] = row[44]
+
             # initialize import session info which will be filled in later
             # not every photo has an import session so initialize all records
 now
             info["import_session"] = None
             info["fok_import_session"] = None
             info["import_uuid"] = None
 
@@ -3833,14 +3840,19 @@
 
         if options.saved_to_library:
             photos = [p for p in photos if p.syndicated and p.saved_to_library]
         elif options.not_saved_to_library:
             photos = [p for p in photos if p.syndicated and not
 p.saved_to_library]
 
+        if options.shared_moment:
+            photos = [p for p in photos if p.shared_moment]
+        elif options.not_shared_moment:
+            photos = [p for p in photos if not p.shared_moment]
+
         if options.function:
             for function in options.function:
                 photos = function[0](photos)
 
         # burst should be checked last, ref #640
         if options.burst_photos:
             # add the burst_photos to the export set
```

#### docs/_modules/osxphotos/queryoptions.html

```diff
@@ -1,15 +1,15 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="../../genindex.html" /><link rel="search" title="Search" href="../../search.html" />
 
     <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/>
-        <title>osxphotos.queryoptions - osxphotos 0.60.5 documentation</title>
+        <title>osxphotos.queryoptions - osxphotos 0.60.9 documentation</title>
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
+      <a href="../../index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="../../search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -305,14 +305,16 @@
 <span class="sd">        uti: list of UTIs to search for</span>
 <span class="sd">        uuid: list of uuids to search for</span>
 <span class="sd">        year: search for photos taken in a given year</span>
 <span class="sd">        syndicated: search for photos that have been shared via syndication (&quot;Shared with You&quot; album via Messages, etc.)</span>
 <span class="sd">        not_syndicated: search for photos that have not been shared via syndication (&quot;Shared with You&quot; album via Messages, etc.)</span>
 <span class="sd">        saved_to_library: search for syndicated photos that have been saved to the Photos library</span>
 <span class="sd">        not_saved_to_library: search for syndicated photos that have not been saved to the Photos library</span>
+<span class="sd">        shared_moment: search for photos that have been shared via a shared moment</span>
+<span class="sd">        not_shared_moment: search for photos that have not been shared via a shared moment</span>
 <span class="sd">    &quot;&quot;&quot;</span>
 
     <span class="n">added_after</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">added_before</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">datetime</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">added_in_last</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">datetime</span><span class="o">.</span><span class="n">timedelta</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">album</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">burst_photos</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
@@ -393,14 +395,16 @@
     <span class="n">uti</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">uuid</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">str</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">year</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="n">Iterable</span><span class="p">[</span><span class="nb">int</span><span class="p">]]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">syndicated</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">not_syndicated</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">saved_to_library</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
     <span class="n">not_saved_to_library</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">shared_moment</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
+    <span class="n">not_shared_moment</span><span class="p">:</span> <span class="n">Optional</span><span class="p">[</span><span class="nb">bool</span><span class="p">]</span> <span class="o">=</span> <span class="kc">None</span>
 
     <span class="k">def</span> <span class="nf">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
         <span class="k">return</span> <span class="n">asdict</span><span class="p">(</span><span class="bp">self</span><span class="p">)</span></div>
 
 
 <span class="k">def</span> <span class="nf">query_options_from_kwargs</span><span class="p">(</span><span class="o">**</span><span class="n">kwargs</span><span class="p">)</span> <span class="o">-&gt;</span> <span class="n">QueryOptions</span><span class="p">:</span>
     <span class="sd">&quot;&quot;&quot;Validate query options and create a QueryOptions instance.</span>
@@ -464,14 +468,15 @@
         <span class="p">(</span><span class="s2">&quot;slow_mo&quot;</span><span class="p">,</span> <span class="s2">&quot;not_slow_mo&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;time_lapse&quot;</span><span class="p">,</span> <span class="s2">&quot;not_time_lapse&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted&quot;</span><span class="p">,</span> <span class="s2">&quot;not_deleted&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted&quot;</span><span class="p">,</span> <span class="s2">&quot;deleted_only&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;deleted_only&quot;</span><span class="p">,</span> <span class="s2">&quot;not_deleted&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;syndicated&quot;</span><span class="p">,</span> <span class="s2">&quot;not_syndicated&quot;</span><span class="p">),</span>
         <span class="p">(</span><span class="s2">&quot;saved_to_library&quot;</span><span class="p">,</span> <span class="s2">&quot;not_saved_to_library&quot;</span><span class="p">),</span>
+        <span class="p">(</span><span class="s2">&quot;shared_moment&quot;</span><span class="p">,</span> <span class="s2">&quot;not_shared_moment&quot;</span><span class="p">),</span>
     <span class="p">]</span>
     <span class="c1"># TODO: add option to validate requiring at least one query arg</span>
     <span class="k">for</span> <span class="n">arg</span><span class="p">,</span> <span class="n">not_arg</span> <span class="ow">in</span> <span class="n">exclusive</span><span class="p">:</span>
         <span class="k">if</span> <span class="n">kwargs</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">arg</span><span class="p">)</span> <span class="ow">and</span> <span class="n">kwargs</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="n">not_arg</span><span class="p">):</span>
             <span class="n">arg</span> <span class="o">=</span> <span class="n">arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;_&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">)</span>
             <span class="n">not_arg</span> <span class="o">=</span> <span class="n">not_arg</span><span class="o">.</span><span class="n">replace</span><span class="p">(</span><span class="s2">&quot;_&quot;</span><span class="p">,</span> <span class="s2">&quot;-&quot;</span><span class="p">)</span>
             <span class="k">raise</span> <span class="n">IncompatibleQueryOptions</span><span class="p">(</span>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.5_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -156,14 +156,18 @@
 ("Shared with You" album via Messages, etc.)
         not_syndicated: search for photos that have not been shared via
 syndication ("Shared with You" album via Messages, etc.)
         saved_to_library: search for syndicated photos that have been saved to
 the Photos library
         not_saved_to_library: search for syndicated photos that have not been
 saved to the Photos library
+        shared_moment: search for photos that have been shared via a shared
+moment
+        not_shared_moment: search for photos that have not been shared via a
+shared moment
     """
 
     added_after: Optional[datetime.datetime] = None
     added_before: Optional[datetime.datetime] = None
     added_in_last: Optional[datetime.timedelta] = None
     album: Optional[Iterable[str]] = None
     burst_photos: Optional[bool] = None
@@ -244,14 +248,16 @@
     uti: Optional[Iterable[str]] = None
     uuid: Optional[Iterable[str]] = None
     year: Optional[Iterable[int]] = None
     syndicated: Optional[bool] = None
     not_syndicated: Optional[bool] = None
     saved_to_library: Optional[bool] = None
     not_saved_to_library: Optional[bool] = None
+    shared_moment: Optional[bool] = None
+    not_shared_moment: Optional[bool] = None
 
     def asdict(self):
         return asdict(self)
 
 
 
 def query_options_from_kwargs(**kwargs) -> QueryOptions:
@@ -316,14 +322,15 @@
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("deleted", "not_deleted"),
         ("deleted", "deleted_only"),
         ("deleted_only", "not_deleted"),
         ("syndicated", "not_syndicated"),
         ("saved_to_library", "not_saved_to_library"),
+        ("shared_moment", "not_shared_moment"),
     ]
     # TODO: add option to validate requiring at least one query arg
     for arg, not_arg in exclusive:
         if kwargs.get(arg) and kwargs.get(not_arg):
             arg = arg.replace("_", "-")
             not_arg = not_arg.replace("_", "-")
             raise IncompatibleQueryOptions(
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
-     - The osxphotos version, e.g. '0.60.8'
+     - The osxphotos version, e.g. '0.60.9'
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
-    VERSION: '0.60.8',
+    VERSION: '0.60.9',
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
-        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos Command Line Interface (CLI) - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -737,14 +737,26 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-not-saved-to-library">
 <span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-not-saved-to-library" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for syndicated photos that have not saved to the library</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-shared-moment">
+<span class="sig-name descname"><span class="pre">--shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-not-shared-moment">
+<span class="sig-name descname"><span class="pre">--not-shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-not-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are not part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-add-locations-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-add-locations-selected">
@@ -1692,14 +1704,26 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-not-saved-to-library">
 <span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-not-saved-to-library" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for syndicated photos that have not saved to the library</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-shared-moment">
+<span class="sig-name descname"><span class="pre">--shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-export-not-shared-moment">
+<span class="sig-name descname"><span class="pre">--not-shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-export-not-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are not part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-export-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-export-selected">
@@ -3298,14 +3322,26 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-not-saved-to-library">
 <span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-not-saved-to-library" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for syndicated photos that have not saved to the library</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-shared-moment">
+<span class="sig-name descname"><span class="pre">--shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-query-not-shared-moment">
+<span class="sig-name descname"><span class="pre">--not-shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-query-not-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are not part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-query-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-query-selected">
@@ -3859,14 +3895,26 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-not-saved-to-library">
 <span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-not-saved-to-library" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for syndicated photos that have not saved to the library</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-shared-moment">
+<span class="sig-name descname"><span class="pre">--shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-repl-not-shared-moment">
+<span class="sig-name descname"><span class="pre">--not-shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-repl-not-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are not part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-repl-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-repl-selected">
@@ -4542,14 +4590,26 @@
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-not-saved-to-library">
 <span class="sig-name descname"><span class="pre">--not-saved-to-library</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-not-saved-to-library" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for syndicated photos that have not saved to the library</p>
 </dd></dl>
 
 <dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-shared-moment">
+<span class="sig-name descname"><span class="pre">--shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
+<dt class="sig sig-object std" id="cmdoption-osxphotos-sync-not-shared-moment">
+<span class="sig-name descname"><span class="pre">--not-shared-moment</span></span><span class="sig-prename descclassname"></span><a class="headerlink" href="#cmdoption-osxphotos-sync-not-shared-moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Search for photos that are not part of a shared moment</p>
+</dd></dl>
+
+<dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-regex">
 <span class="sig-name descname"><span class="pre">--regex</span></span><span class="sig-prename descclassname"> <span class="pre">&lt;REGEX</span> <span class="pre">TEMPLATE&gt;</span></span><a class="headerlink" href="#cmdoption-osxphotos-sync-regex" title="Permalink to this definition">#</a></dt>
 <dd><p>Search for photos where TEMPLATE matches regular expression REGEX. For example, to find photos in an album that begins with ‘Beach’: ‘–regex “^Beach” “{album}”’. You may specify more than one regular expression match by repeating ‘–regex’ with different arguments.</p>
 </dd></dl>
 
 <dl class="std option">
 <dt class="sig sig-object std" id="cmdoption-osxphotos-sync-selected">
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -284,14 +284,18 @@
   --not-syndicated#
       Search for photos that have not been shared via syndication (âShared
       with Youâ album via Messages, etc.)
   --saved-to-library#
       Search for syndicated photos that have saved to the library
   --not-saved-to-library#
       Search for syndicated photos that have not saved to the library
+  --shared-moment#
+      Search for photos that are part of a shared moment
+  --not-shared-moment#
+      Search for photos that are not part of a shared moment
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -801,14 +805,18 @@
   --not-syndicated#
       Search for photos that have not been shared via syndication (âShared
       with Youâ album via Messages, etc.)
   --saved-to-library#
       Search for syndicated photos that have saved to the library
   --not-saved-to-library#
       Search for syndicated photos that have not saved to the library
+  --shared-moment#
+      Search for photos that are part of a shared moment
+  --not-shared-moment#
+      Search for photos that are not part of a shared moment
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -1824,14 +1832,18 @@
   --not-syndicated#
       Search for photos that have not been shared via syndication (âShared
       with Youâ album via Messages, etc.)
   --saved-to-library#
       Search for syndicated photos that have saved to the library
   --not-saved-to-library#
       Search for syndicated photos that have not saved to the library
+  --shared-moment#
+      Search for photos that are part of a shared moment
+  --not-shared-moment#
+      Search for photos that are not part of a shared moment
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -2098,14 +2110,18 @@
   --not-syndicated#
       Search for photos that have not been shared via syndication (âShared
       with Youâ album via Messages, etc.)
   --saved-to-library#
       Search for syndicated photos that have saved to the library
   --not-saved-to-library#
       Search for syndicated photos that have not saved to the library
+  --shared-moment#
+      Search for photos that are part of a shared moment
+  --not-shared-moment#
+      Search for photos that are not part of a shared moment
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
@@ -2478,14 +2494,18 @@
   --not-syndicated#
       Search for photos that have not been shared via syndication (âShared
       with Youâ album via Messages, etc.)
   --saved-to-library#
       Search for syndicated photos that have saved to the library
   --not-saved-to-library#
       Search for syndicated photos that have not saved to the library
+  --shared-moment#
+      Search for photos that are part of a shared moment
+  --not-shared-moment#
+      Search for photos that are not part of a shared moment
   --regex <REGEX TEMPLATE>#
       Search for photos where TEMPLATE matches regular expression REGEX. For
       example, to find photos in an album that begins with âBeachâ:
       ââregex â^Beachâ â{album}ââ. You may specify more than one
       regular expression match by repeating ââregexâ with different
       arguments.
   --selected#
```

#### docs/genindex.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="#" /><link rel="search" title="Search" href="search.html" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.8 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Index - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -1597,16 +1597,14 @@
           <li><a href="cli.html#cmdoption-osxphotos-query-not-favorite">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-favorite">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-favorite">osxphotos-sync command line option</a>
 </li>
         </ul></li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     --not-hdr
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-hdr">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-hdr">osxphotos-export command line option</a>
@@ -1614,14 +1612,16 @@
           <li><a href="cli.html#cmdoption-osxphotos-query-not-hdr">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-hdr">osxphotos-repl command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-hdr">osxphotos-sync command line option</a>
 </li>
         </ul></li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li>
     --not-hidden
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-hidden">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-hidden">osxphotos-export command line option</a>
@@ -1793,14 +1793,29 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-shared">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-shared">osxphotos-repl command line option</a>
 </li>
         </ul></li>
         <li>
+    --not-shared-moment
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-shared-moment">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-shared-moment">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-shared-moment">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-shared-moment">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-shared-moment">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --not-slow-mo
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-slow-mo">osxphotos-add-locations command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-slow-mo">osxphotos-export command line option</a>
 </li>
@@ -2249,14 +2264,29 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-shared">osxphotos-query command line option</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-shared">osxphotos-repl command line option</a>
 </li>
         </ul></li>
         <li>
+    --shared-moment
+
+        <ul>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-shared-moment">osxphotos-add-locations command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-shared-moment">osxphotos-export command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-shared-moment">osxphotos-query command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-shared-moment">osxphotos-repl command line option</a>
+</li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-shared-moment">osxphotos-sync command line option</a>
+</li>
+        </ul></li>
+        <li>
     --sidecar
 
         <ul>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar">osxphotos-export command line option</a>
 </li>
         </ul></li>
         <li>
@@ -3760,18 +3790,18 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_cloudasset">not_cloudasset (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_edited">not_edited (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_favorite">not_favorite (osxphotos.QueryOptions attribute)</a>
 </li>
-    </ul></td>
-    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.QueryOptions.not_hdr">not_hdr (osxphotos.QueryOptions attribute)</a>
 </li>
+    </ul></td>
+    <td style="width: 33%; vertical-align: top;"><ul>
         <li><a href="reference.html#osxphotos.QueryOptions.not_hidden">not_hidden (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_in_album">not_in_album (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_incloud">not_incloud (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_live">not_live (osxphotos.QueryOptions attribute)</a>
@@ -3788,14 +3818,16 @@
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_screenshot">not_screenshot (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_selfie">not_selfie (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_shared">not_shared (osxphotos.QueryOptions attribute)</a>
 </li>
+        <li><a href="reference.html#osxphotos.QueryOptions.not_shared_moment">not_shared_moment (osxphotos.QueryOptions attribute)</a>
+</li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_slow_mo">not_slow_mo (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_syndicated">not_syndicated (osxphotos.QueryOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.QueryOptions.not_time_lapse">not_time_lapse (osxphotos.QueryOptions attribute)</a>
 </li>
     </ul></td>
@@ -3948,14 +3980,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-shared">--not-shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-shared-moment">--not-shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-slow-mo">--not-slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-syndicated">--not-syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-only-movies">--only-movies</a>
@@ -3982,14 +4016,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-shared">--shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-add-locations-shared-moment">--shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-slow-mo">--slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-syndicated">--syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-theme">--theme</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-add-locations-time-lapse">--time-lapse</a>
@@ -4362,14 +4398,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-shared">--not-shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-not-shared-moment">--not-shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-slow-mo">--not-slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-syndicated">--not-syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-only-movies">--only-movies</a>
@@ -4426,14 +4464,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-shared">--shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-export-shared-moment">--shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar">--sidecar</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-sidecar-drop-ext">--sidecar-drop-ext</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-bursts">--skip-bursts</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-export-skip-edited">--skip-edited</a>
@@ -4909,14 +4949,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-shared">--not-shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-not-shared-moment">--not-shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-slow-mo">--not-slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-syndicated">--not-syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-only-movies">--only-movies</a>
@@ -4947,14 +4989,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-shared">--shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-query-shared-moment">--shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-query-slow-mo">--slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-syndicated">--syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-query-title">--title</a>
@@ -5100,14 +5144,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-selfie">--not-selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-shared">--not-shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-not-shared-moment">--not-shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-slow-mo">--not-slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-syndicated">--not-syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-only-movies">--only-movies</a>
@@ -5134,14 +5180,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-shared">--shared</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-repl-shared-moment">--shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-slow-mo">--slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-syndicated">--syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-time-lapse">--time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-repl-title">--title</a>
@@ -5318,14 +5366,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-saved-to-library">--not-saved-to-library</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-screenshot">--not-screenshot</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-selfie">--not-selfie</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-not-shared-moment">--not-shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-slow-mo">--not-slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-syndicated">--not-syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-not-time-lapse">--not-time-lapse</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-only-movies">--only-movies</a>
@@ -5354,14 +5404,16 @@
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-selected">--selected</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-selfie">--selfie</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-s">--set</a>
 </li>
+          <li><a href="cli.html#cmdoption-osxphotos-sync-shared-moment">--shared-moment</a>
+</li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-slow-mo">--slow-mo</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-syndicated">--syndicated</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-theme">--theme</a>
 </li>
           <li><a href="cli.html#cmdoption-osxphotos-sync-time-lapse">--time-lapse</a>
@@ -5818,14 +5870,20 @@
 
         <ul>
           <li><a href="reference.html#osxphotos.QueryOptions.shared">(osxphotos.QueryOptions attribute)</a>
 </li>
         </ul></li>
     </ul></td>
     <td style="width: 33%; vertical-align: top;"><ul>
+        <li><a href="reference.html#osxphotos.PhotoInfo.shared_moment">shared_moment (osxphotos.PhotoInfo property)</a>
+
+        <ul>
+          <li><a href="reference.html#osxphotos.QueryOptions.shared_moment">(osxphotos.QueryOptions attribute)</a>
+</li>
+        </ul></li>
         <li><a href="reference.html#osxphotos.ExportOptions.sidecar">sidecar (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.ExportOptions.sidecar_drop_ext">sidecar_drop_ext (osxphotos.ExportOptions attribute)</a>
 </li>
         <li><a href="reference.html#osxphotos.FaceInfo.size_pixels">size_pixels (osxphotos.FaceInfo property)</a>
 </li>
         <li><a href="reference.html#osxphotos.PhotoInfo.slow_mo">slow_mo (osxphotos.PhotoInfo property)</a>
```

##### html2text {}

```diff
@@ -12,21 +12,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -42,154 +42,154 @@
 
 ***** Symbols *****
     * --add-exported-to-album
           o osxphotos-export_command
             line_option
     * --add-missing-to-album
           o osxphotos-export_command
-            line_option                     * --not-hdr
+            line_option                     * --not-hidden
     * --add-skipped-to-album                      o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
     * --add-to-album                                line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-timewarp_command            o osxphotos-repl_command_line
             line_option                             option
     * --added-after                               o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-hidden
+            command_line_option             * --not-in-album
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --added-before                              o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-in-album
+            command_line_option             * --not-incloud
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --added-in-last                             o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-incloud
+            command_line_option             * --not-live
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-query_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
     * --album                                     o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
-            command_line_option             * --not-live
+            command_line_option             * --not-missing
           o osxphotos-export_command              o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-import_command              o osxphotos-export_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-query_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-repl_command_line
             option                                  option
           o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-    * --album-keyword                       * --not-missing
+    * --album-keyword                       * --not-panorama
           o osxphotos-exiftool_command            o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
     * --alt-copy                                  o osxphotos-query_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-repl_command_line
     * --append                                      option
           o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --not-panorama
+          o osxphotos-export_command        * --not-portrait
             line_option                           o osxphotos-add-locations
           o osxphotos-exportdb_command              command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-import_command                line_option
             line_option                           o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
     * --burst                                       option
           o osxphotos-add-locations               o osxphotos-sync_command_line
             command_line_option                     option
-          o osxphotos-export_command        * --not-portrait
+          o osxphotos-export_command        * --not-reference
             line_option                           o osxphotos-add-locations
           o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-repl_command_line
     * --check-signatures                            option
           o osxphotos-exportdb_command            o osxphotos-sync_command_line
             line_option                             option
-    * --check-templates                     * --not-reference
+    * --check-templates                     * --not-saved-to-library
           o osxphotos-import_command              o osxphotos-add-locations
             line_option                             command_line_option
     * --cleanup                                   o osxphotos-export_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
     * --clear-location                              line_option
           o osxphotos-import_command              o osxphotos-repl_command_line
             line_option                             option
     * --clear-metadata                            o osxphotos-sync_command_line
           o osxphotos-import_command                option
-            line_option                     * --not-saved-to-library
+            line_option                     * --not-screenshot
     * --clone                                     o osxphotos-add-locations
           o osxphotos-theme_command                 command_line_option
             line_option                           o osxphotos-export_command
     * --cloudasset                                  line_option
           o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-query_command               o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-repl_command_line     * --not-screenshot
+          o osxphotos-repl_command_line     * --not-selfie
             option                                o osxphotos-add-locations
           o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
     * --compare-exif                                line_option
           o osxphotos-timewarp_command            o osxphotos-query_command
             line_option                             line_option
     * --config                                    o osxphotos-repl_command_line
           o osxphotos-theme_command                 option
             line_option                           o osxphotos-sync_command_line
     * --config-only                                 option
-          o osxphotos-export_command        * --not-selfie
+          o osxphotos-export_command        * --not-shared
             line_option                           o osxphotos-add-locations
     * --convert-to-jpeg                             command_line_option
           o osxphotos-export_command              o osxphotos-export_command
             line_option                             line_option
     * --count                                     o osxphotos-query_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
     * --current-name                                option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-    * --date                                * --not-shared
-          o osxphotos-timewarp_command            o osxphotos-add-locations
-            line_option                             command_line_option
-    * --date-added                                o osxphotos-export_command
+          o osxphotos-export_command        * --not-shared-moment
+            line_option                           o osxphotos-add-locations
+    * --date                                        command_line_option
+          o osxphotos-timewarp_command            o osxphotos-export_command
+            line_option                             line_option
+    * --date-added                                o osxphotos-query_command
           o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-query_command
-    * --date-added-from-photo                       line_option
-          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+            line_option                           o osxphotos-repl_command_line
+    * --date-added-from-photo                       option
+          o osxphotos-timewarp_command            o osxphotos-sync_command_line
             line_option                             option
     * --date-delta                          * --not-slow-mo
           o osxphotos-timewarp_command            o osxphotos-add-locations
             line_option                             command_line_option
     * --db                                        o osxphotos-export_command
           o osxphotos-albums_command                line_option
             line_option                           o osxphotos-query_command
@@ -471,461 +471,472 @@
           o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-export_command
     * --from-time                                   line_option
           o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-repl_command_line
             line_option                             option
-          o osxphotos-query_command         * --sidecar
+          o osxphotos-query_command         * --shared-moment
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
+            option                                o osxphotos-export_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-query_command
+    * --function                                    line_option
+          o osxphotos-timewarp_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --glob                                      o osxphotos-sync_command_line
+          o osxphotos-import_command                option
+            line_option                     * --sidecar
+    * --has-comment                               o osxphotos-export_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --sidecar-drop-ext
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-query_command         * --skip-bursts
             line_option                           o osxphotos-export_command
           o osxphotos-repl_command_line             line_option
-            option                          * --sidecar-drop-ext
+            option                          * --skip-edited
           o osxphotos-sync_command_line           o osxphotos-export_command
             option                                  line_option
-    * --function                            * --skip-bursts
-          o osxphotos-timewarp_command            o osxphotos-export_command
-            line_option                             line_option
-    * --glob                                * --skip-edited
-          o osxphotos-import_command              o osxphotos-export_command
-            line_option                             line_option
-    * --has-comment                         * --skip-live
+    * --has-likes                           * --skip-live
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
           o osxphotos-export_command        * --skip-original-if-edited
             line_option                           o osxphotos-export_command
           o osxphotos-query_command                 line_option
             line_option                     * --skip-raw
           o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
           o osxphotos-sync_command_line     * --skip-uuid
             option                                o osxphotos-export_command
-    * --has-likes                                   line_option
+    * --has-raw                                     line_option
           o osxphotos-add-locations         * --skip-uuid-from-file
             command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
             line_option                     * --slow-mo
           o osxphotos-query_command               o osxphotos-add-locations
             line_option                             command_line_option
           o osxphotos-repl_command_line           o osxphotos-export_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-query_command
             option                                  line_option
-    * --has-raw                                   o osxphotos-repl_command_line
+    * --hdr                                       o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
             command_line_option                   o osxphotos-sync_command_line
           o osxphotos-export_command                option
             line_option                     * --split-folder
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line     * --sql
             option                                o osxphotos-exportdb_command
           o osxphotos-sync_command_line             line_option
             option                          * --strip
-    * --hdr                                       o osxphotos-export_command
-          o osxphotos-add-locations                 line_option
-            command_line_option             * --style
-          o osxphotos-export_command              o osxphotos-diff_command_line
-            line_option                             option
-          o osxphotos-query_command         * --syndicated
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-query_command
-    * --help                                        line_option
-          o osxphotos-run_command_line            o osxphotos-repl_command_line
+    * --help                                      o osxphotos-export_command
+          o osxphotos-run_command_line              line_option
+            option                          * --style
+    * --hidden                                    o osxphotos-diff_command_line
+          o osxphotos-add-locations                 option
+            command_line_option             * --syndicated
+          o osxphotos-export_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-sync_command_line           o osxphotos-repl_command_line
             option                                  option
-    * --hidden                                    o osxphotos-sync_command_line
+    * --ignore-case                               o osxphotos-sync_command_line
           o osxphotos-add-locations                 option
             command_line_option             * --template
           o osxphotos-export_command              o osxphotos-inspect_command
             line_option                             line_option
           o osxphotos-query_command         * --theme
             line_option                           o osxphotos-add-locations
           o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-batch-edit
           o osxphotos-sync_command_line             command_line_option
             option                                o osxphotos-exiftool_command
-    * --ignore-case                                 line_option
-          o osxphotos-add-locations               o osxphotos-export_command
-            command_line_option                     line_option
-          o osxphotos-export_command              o osxphotos-exportdb_command
+    * --ignore-date-modified                        line_option
+          o osxphotos-exiftool_command            o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-import_command
+          o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-inspect_command
-            option                                  line_option
+    * --ignore-signature                          o osxphotos-import_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-inspect_command
+    * --import                                      line_option
           o osxphotos-sync_command_line           o osxphotos-orphans_command
             option                                  line_option
-    * --ignore-date-modified                      o osxphotos-sync_command_line
-          o osxphotos-exiftool_command              option
-            line_option                           o osxphotos-timewarp_command
+    * --in-album                                  o osxphotos-sync_command_line
+          o osxphotos-add-locations                 option
+            command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
             line_option                     * --time
-    * --ignore-signature                          o osxphotos-timewarp_command
-          o osxphotos-export_command                line_option
-            line_option                     * --time-delta
-    * --import                                    o osxphotos-timewarp_command
+          o osxphotos-query_command               o osxphotos-timewarp_command
+            line_option                             line_option
+          o osxphotos-repl_command_line     * --time-delta
+            option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
             option                          * --time-lapse
-    * --in-album                                  o osxphotos-add-locations
+    * --incloud                                   o osxphotos-add-locations
           o osxphotos-add-locations                 command_line_option
             command_line_option                   o osxphotos-export_command
           o osxphotos-export_command                line_option
             line_option                           o osxphotos-query_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-repl_command_line
           o osxphotos-repl_command_line             option
             option                                o osxphotos-sync_command_line
           o osxphotos-sync_command_line             option
             option                          * --timestamp
-    * --incloud                                   o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-batch-edit
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-exiftool_command
+    * --info                                      o osxphotos-add-locations
+          o osxphotos-exportdb_command              command_line_option
+            line_option                           o osxphotos-batch-edit
+    * --inspect                                     command_line_option
+          o osxphotos-timewarp_command            o osxphotos-diff_command_line
+            line_option                             option
+    * --is-reference                              o osxphotos-exiftool_command
+          o osxphotos-add-locations                 line_option
+            command_line_option                   o osxphotos-export_command
+          o osxphotos-export_command                line_option
+            line_option                           o osxphotos-exportdb_command
+          o osxphotos-query_command                 line_option
+            line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-export_command
+            option                                o osxphotos-orphans_command
           o osxphotos-sync_command_line             line_option
-            option                                o osxphotos-exportdb_command
-    * --info                                        line_option
-          o osxphotos-exportdb_command            o osxphotos-import_command
+            option                                o osxphotos-sync_command_line
+    * --jpeg-ext                                    option
+          o osxphotos-export_command              o osxphotos-timewarp_command
+            line_option                             line_option, [1]
+    * --jpeg-quality                        * --timezone
+          o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
-    * --inspect                                   o osxphotos-orphans_command
-          o osxphotos-timewarp_command              line_option
-            line_option                           o osxphotos-sync_command_line
-    * --is-reference                                option
-          o osxphotos-add-locations               o osxphotos-timewarp_command
-            command_line_option                     line_option, [1]
-          o osxphotos-export_command        * --timezone
-            line_option                           o osxphotos-timewarp_command
-          o osxphotos-query_command                 line_option
-            line_option                     * --title
-          o osxphotos-repl_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-          o osxphotos-sync_command_line           o osxphotos-batch-edit
+    * --json                                * --title
+          o osxphotos-albums_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-dump_command_line           o osxphotos-batch-edit
             option                                  command_line_option
-    * --jpeg-ext                                  o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                           o osxphotos-import_command
-    * --jpeg-quality                                line_option
-          o osxphotos-export_command              o osxphotos-query_command
-            line_option                             line_option
-    * --json                                      o osxphotos-repl_command_line
-          o osxphotos-albums_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-dump_command_line             option
-            option                          * --tmpdir
           o osxphotos-info_command_line           o osxphotos-export_command
             option                                  line_option
-          o osxphotos-keywords_command      * --to-date
-            line_option                           o osxphotos-add-locations
-          o osxphotos-labels_command                command_line_option
+          o osxphotos-keywords_command            o osxphotos-import_command
+            line_option                             line_option
+          o osxphotos-labels_command              o osxphotos-query_command
+            line_option                             line_option
+          o osxphotos-list_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-persons_command             o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-places_command        * --tmpdir
             line_option                           o osxphotos-export_command
-          o osxphotos-list_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-persons_command               line_option
-            line_option                           o osxphotos-repl_command_line
-          o osxphotos-places_command                option
-            line_option                           o osxphotos-sync_command_line
-          o osxphotos-query_command                 option
-            line_option                     * --to-time
+          o osxphotos-query_command                 line_option
+            line_option                     * --to-date
     * --keep                                      o osxphotos-add-locations
           o osxphotos-export_command                command_line_option
             line_option                           o osxphotos-export_command
     * --keyword                                     line_option
           o osxphotos-add-locations               o osxphotos-query_command
             command_line_option                     line_option
           o osxphotos-batch-edit                  o osxphotos-repl_command_line
             command_line_option                     option
           o osxphotos-export_command              o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-import_command        * --touch-file
+          o osxphotos-import_command        * --to-time
+            line_option                           o osxphotos-add-locations
+          o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-export_command
-          o osxphotos-query_command                 line_option
-            line_option                           o osxphotos-exportdb_command
           o osxphotos-repl_command_line             line_option
-            option                          * --undo
-          o osxphotos-sync_command_line           o osxphotos-batch-edit
-            option                                  command_line_option
-    * --keyword-template                    * --unmatched
+            option                                o osxphotos-query_command
+          o osxphotos-sync_command_line             line_option
+            option                                o osxphotos-repl_command_line
+    * --keyword-template                            option
           o osxphotos-exiftool_command            o osxphotos-sync_command_line
             line_option                             option
-          o osxphotos-export_command        * --update
+          o osxphotos-export_command        * --touch-file
             line_option                           o osxphotos-export_command
     * --label                                       line_option
-          o osxphotos-add-locations         * --update-errors
-            command_line_option                   o osxphotos-export_command
-          o osxphotos-export_command                line_option
-            line_option                     * --update-signatures
-          o osxphotos-query_command               o osxphotos-exportdb_command
-            line_option                             line_option
-          o osxphotos-repl_command_line     * --upgrade
-            option                                o osxphotos-install_command
-          o osxphotos-sync_command_line             line_option
-            option                          * --use-file-time
-    * --last-errors                               o osxphotos-timewarp_command
-          o osxphotos-exportdb_command              line_option
-            line_option                     * --use-photokit
-    * --last-run                                  o osxphotos-export_command
-          o osxphotos-exportdb_command              line_option
-            line_option                     * --use-photos-export
-    * --library                                   o osxphotos-export_command
-          o osxphotos-albums_command                line_option
-            line_option                     * --uti
-          o osxphotos-batch-edit                  o osxphotos-add-locations
-            command_line_option                     command_line_option
-          o osxphotos-diff_command_line           o osxphotos-export_command
-            option                                  line_option
-          o osxphotos-dump_command_line           o osxphotos-query_command
+          o osxphotos-add-locations               o osxphotos-exportdb_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * --undo
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-query_command                 command_line_option
+            line_option                     * --unmatched
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-sync_command_line     * --update
+            option                                o osxphotos-export_command
+    * --last-errors                                 line_option
+          o osxphotos-exportdb_command      * --update-errors
+            line_option                           o osxphotos-export_command
+    * --last-run                                    line_option
+          o osxphotos-exportdb_command      * --update-signatures
+            line_option                           o osxphotos-exportdb_command
+    * --library                                     line_option
+          o osxphotos-albums_command        * --upgrade
+            line_option                           o osxphotos-install_command
+          o osxphotos-batch-edit                    line_option
+            command_line_option             * --use-file-time
+          o osxphotos-diff_command_line           o osxphotos-timewarp_command
             option                                  line_option
-          o osxphotos-exiftool_command            o osxphotos-repl_command_line
-            line_option                             option
-          o osxphotos-export_command              o osxphotos-sync_command_line
-            line_option                             option
-          o osxphotos-info_command_line     * --uuid
+          o osxphotos-dump_command_line     * --use-photokit
+            option                                o osxphotos-export_command
+          o osxphotos-exiftool_command              line_option
+            line_option                     * --use-photos-export
+          o osxphotos-export_command              o osxphotos-export_command
+            line_option                             line_option
+          o osxphotos-info_command_line     * --uti
             option                                o osxphotos-add-locations
           o osxphotos-inspect_command               command_line_option
             line_option                           o osxphotos-export_command
           o osxphotos-keywords_command              line_option
             line_option                           o osxphotos-query_command
           o osxphotos-labels_command                line_option
             line_option                           o osxphotos-repl_command_line
           o osxphotos-orphans_command               option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-persons_command               option
-            line_option                     * --uuid-files
-          o osxphotos-places_command              o osxphotos-exportdb_command
+            line_option                     * --uuid
+          o osxphotos-places_command              o osxphotos-add-locations
+            line_option                             command_line_option
+          o osxphotos-query_command               o osxphotos-export_command
             line_option                             line_option
-          o osxphotos-query_command         * --uuid-from-file
-            line_option                           o osxphotos-add-locations
-          o osxphotos-repl_command_line             command_line_option
-            option                                o osxphotos-export_command
-          o osxphotos-show_command_line             line_option
-            option                                o osxphotos-query_command
-          o osxphotos-snap_command_line             line_option
-            option                                o osxphotos-repl_command_line
-          o osxphotos-sync_command_line             option
-            option                                o osxphotos-sync_command_line
-          o osxphotos-timewarp_command              option
-            line_option                     * --uuid-info
-    * --limit                                     o osxphotos-exportdb_command
-          o osxphotos-export_command                line_option
-            line_option                     * --vacuum
-    * --list                                      o osxphotos-exportdb_command
-          o osxphotos-theme_command                 line_option
-            line_option                     * --verbose
-    * --live                                      o osxphotos-add-locations
-          o osxphotos-add-locations                 command_line_option
-            command_line_option                   o osxphotos-batch-edit
-          o osxphotos-export_command                command_line_option
-            line_option                           o osxphotos-diff_command_line
-          o osxphotos-query_command                 option
-            line_option                           o osxphotos-exiftool_command
-          o osxphotos-repl_command_line             line_option
-            option                                o osxphotos-export_command
-          o osxphotos-sync_command_line             line_option
+          o osxphotos-repl_command_line           o osxphotos-query_command
+            option                                  line_option
+          o osxphotos-show_command_line           o osxphotos-repl_command_line
+            option                                  option
+          o osxphotos-snap_command_line           o osxphotos-sync_command_line
+            option                                  option
+          o osxphotos-sync_command_line     * --uuid-files
             option                                o osxphotos-exportdb_command
-    * --load-config                                 line_option
-          o osxphotos-exiftool_command            o osxphotos-import_command
-            line_option                             line_option
-          o osxphotos-export_command              o osxphotos-orphans_command
+          o osxphotos-timewarp_command              line_option
+            line_option                     * --uuid-from-file
+    * --limit                                     o osxphotos-add-locations
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-export_command
+    * --list                                        line_option
+          o osxphotos-theme_command               o osxphotos-query_command
             line_option                             line_option
-    * --location                                  o osxphotos-sync_command_line
+    * --live                                      o osxphotos-repl_command_line
           o osxphotos-add-locations                 option
-            command_line_option                   o osxphotos-timewarp_command
-          o osxphotos-batch-edit                    line_option
-            command_line_option             * --version
-          o osxphotos-export_command              o osxphotos_command_line
-            line_option                             option
-          o osxphotos-import_command              o osxphotos-exportdb_command
+            command_line_option                   o osxphotos-sync_command_line
+          o osxphotos-export_command                option
+            line_option                     * --uuid-info
+          o osxphotos-query_command               o osxphotos-exportdb_command
             line_option                             line_option
-          o osxphotos-query_command         * --walk
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                          * --window
-          o osxphotos-sync_command_line           o osxphotos-add-locations
-            option                                  command_line_option
-    * --match-time                          * --xattr-template
-          o osxphotos-timewarp_command            o osxphotos-export_command
+          o osxphotos-repl_command_line     * --vacuum
+            option                                o osxphotos-exportdb_command
+          o osxphotos-sync_command_line             line_option
+            option                          * --verbose
+    * --load-config                               o osxphotos-add-locations
+          o osxphotos-exiftool_command              command_line_option
+            line_option                           o osxphotos-batch-edit
+          o osxphotos-export_command                command_line_option
+            line_option                           o osxphotos-diff_command_line
+    * --location                                    option
+          o osxphotos-add-locations               o osxphotos-exiftool_command
+            command_line_option                     line_option
+          o osxphotos-batch-edit                  o osxphotos-export_command
+            command_line_option                     line_option
+          o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
-    * --max-size                            * --year
-          o osxphotos-add-locations               o osxphotos-add-locations
-            command_line_option                     command_line_option
-          o osxphotos-export_command              o osxphotos-export_command
+          o osxphotos-import_command              o osxphotos-import_command
             line_option                             line_option
-          o osxphotos-query_command               o osxphotos-query_command
+          o osxphotos-query_command               o osxphotos-orphans_command
             line_option                             line_option
-          o osxphotos-repl_command_line           o osxphotos-repl_command_line
-            option                                  option
-          o osxphotos-sync_command_line           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option
-    * --merge                               * --yes
-          o osxphotos-sync_command_line           o osxphotos-uninstall_command
+          o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --merge-keywords                      * -A
-          o osxphotos-import_command              o osxphotos-sync_command_line
+    * --match-time                          * --version
+          o osxphotos-timewarp_command            o osxphotos_command_line
             line_option                             option
-    * --migrate                             * -a
-          o osxphotos-exportdb_command            o osxphotos-import_command
+    * --max-size                                  o osxphotos-exportdb_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * --walk
+          o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
-    * --migrate-photos-library                    o osxphotos-timewarp_command
-          o osxphotos-exportdb_command              line_option
-            line_option                     * -C
-    * --min-size                                  o osxphotos-import_command
+          o osxphotos-query_command         * --window
+            line_option                           o osxphotos-add-locations
+          o osxphotos-repl_command_line             command_line_option
+            option                          * --xattr-template
+          o osxphotos-sync_command_line           o osxphotos-export_command
+            option                                  line_option
+    * --merge                               * --year
+          o osxphotos-sync_command_line           o osxphotos-add-locations
+            option                                  command_line_option
+    * --merge-keywords                            o osxphotos-export_command
+          o osxphotos-import_command                line_option
+            line_option                           o osxphotos-query_command
+    * --migrate                                     line_option
+          o osxphotos-exportdb_command            o osxphotos-repl_command_line
+            line_option                             option
+    * --migrate-photos-library                    o osxphotos-sync_command_line
+          o osxphotos-exportdb_command              option
+            line_option                     * --yes
+    * --min-size                                  o osxphotos-uninstall_command
+          o osxphotos-add-locations                 line_option
+            command_line_option             * -A
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-query_command         * -a
+            line_option                           o osxphotos-import_command
+          o osxphotos-repl_command_line             line_option
+            option                                o osxphotos-timewarp_command
+          o osxphotos-sync_command_line             line_option
+            option                          * -C
+    * --missing                                   o osxphotos-import_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -c
           o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
           o osxphotos-query_command         * -D
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
             option                          * -d
-    * --missing                                   o osxphotos-import_command
+    * --name                                      o osxphotos-import_command
           o osxphotos-add-locations                 line_option
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
             line_option                     * -e
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --name                                * -F
+    * --no-comment                          * -F
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
           o osxphotos-export_command        * -f
             line_option                           o osxphotos-dump_command_line
           o osxphotos-query_command                 option
             line_option                           o osxphotos-import_command
           o osxphotos-repl_command_line             line_option
             option                                o osxphotos-query_command
           o osxphotos-sync_command_line             line_option
             option                                o osxphotos-timewarp_command
-    * --no-comment                                  line_option
+    * --no-description                              line_option
           o osxphotos-add-locations               o osxphotos-uuid_command_line
             command_line_option                     option
           o osxphotos-export_command        * -g
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                     * -h
           o osxphotos-repl_command_line           o osxphotos-run_command_line
             option                                  option
           o osxphotos-sync_command_line     * -i
             option                                o osxphotos-add-locations
-    * --no-description                              command_line_option
+    * --no-keyword                                  command_line_option
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-query_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-repl_command_line
             line_option                             option
           o osxphotos-repl_command_line           o osxphotos-sync_command_line
             option                                  option, [1]
           o osxphotos-sync_command_line           o osxphotos-timewarp_command
             option                                  line_option
-    * --no-keyword                          * -k
+    * --no-likes                            * -k
           o osxphotos-add-locations               o osxphotos-import_command
             command_line_option                     line_option
           o osxphotos-export_command        * -L
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-timewarp_command
           o osxphotos-repl_command_line             line_option
             option                          * -l
           o osxphotos-sync_command_line           o osxphotos-import_command
             option                                  line_option
-    * --no-likes                            * -M
+    * --no-location                         * -M
           o osxphotos-add-locations               o osxphotos-timewarp_command
             command_line_option                     line_option
           o osxphotos-export_command        * -m
             line_option                           o osxphotos-import_command
           o osxphotos-query_command                 line_option
             line_option                           o osxphotos-sync_command_line
           o osxphotos-repl_command_line             option
             option                                o osxphotos-timewarp_command
           o osxphotos-sync_command_line             line_option
             option                          * -P
-    * --no-location                               o osxphotos-import_command
+    * --no-place                                  o osxphotos-import_command
           o osxphotos-add-locations                 line_option
             command_line_option                   o osxphotos-timewarp_command
           o osxphotos-export_command                line_option
             line_option                     * -p
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
           o osxphotos-sync_command_line     * -R
             option                                o osxphotos-import_command
-    * --no-place                                    line_option
-          o osxphotos-add-locations               o osxphotos-sync_command_line
-            command_line_option                     option
-          o osxphotos-export_command        * -r
+    * --no-progress                                 line_option
+          o osxphotos-export_command              o osxphotos-sync_command_line
+            line_option                             option
+          o osxphotos-import_command        * -r
+            line_option                           o osxphotos-diff_command_line
+    * --no-title                                    option
+          o osxphotos-add-locations               o osxphotos-import_command
+            command_line_option                     line_option
+          o osxphotos-export_command        * -s
             line_option                           o osxphotos-diff_command_line
           o osxphotos-query_command                 option
-            line_option                           o osxphotos-import_command
-          o osxphotos-repl_command_line             line_option
-            option                          * -s
-          o osxphotos-sync_command_line           o osxphotos-diff_command_line
-            option                                  option
-    * --no-progress                               o osxphotos-sync_command_line
-          o osxphotos-export_command                option
-            line_option                     * -T
-          o osxphotos-import_command              o osxphotos-inspect_command
-            line_option                             line_option
-    * --no-title                                  o osxphotos-timewarp_command
+            line_option                           o osxphotos-sync_command_line
+          o osxphotos-repl_command_line             option
+            option                          * -T
+          o osxphotos-sync_command_line           o osxphotos-inspect_command
+            option                                  line_option
+    * --not-burst                                 o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -t
           o osxphotos-export_command              o osxphotos-import_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-inspect_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-timewarp_command
             option                                  line_option
           o osxphotos-sync_command_line     * -U
             option                                o osxphotos-install_command
-    * --not-burst                                   line_option
+    * --not-cloudasset                              line_option
           o osxphotos-add-locations               o osxphotos-sync_command_line
             command_line_option                     option
           o osxphotos-export_command        * -V
             line_option                           o osxphotos-add-locations
           o osxphotos-query_command                 command_line_option
             line_option                           o osxphotos-batch-edit
           o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-diff_command_line
           o osxphotos-sync_command_line             option
             option                                o osxphotos-exiftool_command
-    * --not-cloudasset                              line_option
+    * --not-edited                                  line_option
           o osxphotos-add-locations               o osxphotos-export_command
             command_line_option                     line_option
           o osxphotos-export_command              o osxphotos-exportdb_command
             line_option                             line_option
           o osxphotos-query_command               o osxphotos-import_command
             line_option                             line_option
           o osxphotos-repl_command_line           o osxphotos-orphans_command
             option                                  line_option
           o osxphotos-sync_command_line           o osxphotos-sync_command_line
             option                                  option
-    * --not-edited                                o osxphotos-timewarp_command
+    * --not-favorite                              o osxphotos-timewarp_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -v
           o osxphotos-export_command              o osxphotos_command_line
             line_option                             option
           o osxphotos-query_command         * -w
             line_option                           o osxphotos-add-locations
           o osxphotos-repl_command_line             command_line_option
             option                                o osxphotos-import_command
           o osxphotos-sync_command_line             line_option
             option                          * -y
-    * --not-favorite                              o osxphotos-uninstall_command
+    * --not-hdr                                   o osxphotos-uninstall_command
           o osxphotos-add-locations                 line_option
             command_line_option             * -z
           o osxphotos-export_command              o osxphotos-timewarp_command
             line_option                             line_option
           o osxphotos-query_command
             line_option
           o osxphotos-repl_command_line
@@ -1225,274 +1236,277 @@
     * missing_bursts_                       * mwg_rs_area_(osxphotos.FaceInfo
       (osxphotos.QueryOptions                 property)
       attribute)
     * modification_date_
       (osxphotos.MomentInfo_property)
 
 ***** N *****
-                                            * not_hdr_(osxphotos.QueryOptions
-                                              attribute)
                                             * not_hidden_
                                               (osxphotos.QueryOptions
-    * name_(osxphotos.PlaceInfo               attribute)
-      property)                             * not_in_album_
-          o (osxphotos.QueryOptions           (osxphotos.QueryOptions
-            attribute)                        attribute)
-    * names_(osxphotos.PlaceInfo            * not_incloud_
-      property)                               (osxphotos.QueryOptions
+                                              attribute)
+                                            * not_in_album_
+    * name_(osxphotos.PlaceInfo               (osxphotos.QueryOptions
+      property)                               attribute)
+          o (osxphotos.QueryOptions         * not_incloud_
+            attribute)                        (osxphotos.QueryOptions
+    * names_(osxphotos.PlaceInfo              attribute)
+      property)                             * not_live_(osxphotos.QueryOptions
     * neighborhoods_                          attribute)
-      (osxphotos.SearchInfo_property)       * not_live_(osxphotos.QueryOptions
-    * no_comment_                             attribute)
-      (osxphotos.QueryOptions               * not_missing_
-      attribute)                              (osxphotos.QueryOptions
-    * no_description_                         attribute)
-      (osxphotos.QueryOptions               * not_panorama_
-      attribute)                              (osxphotos.QueryOptions
-    * no_keyword_                             attribute)
-      (osxphotos.QueryOptions               * not_portrait_
-      attribute)                              (osxphotos.QueryOptions
-    * no_likes_(osxphotos.QueryOptions        attribute)
-      attribute)                            * not_reference_
-    * no_location_                            (osxphotos.QueryOptions
+      (osxphotos.SearchInfo_property)       * not_missing_
+    * no_comment_                             (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
+      attribute)                            * not_panorama_
+    * no_description_                         (osxphotos.QueryOptions
       (osxphotos.QueryOptions                 attribute)
-      attribute)                            * not_saved_to_library_
-    * no_place_(osxphotos.QueryOptions        (osxphotos.QueryOptions
+      attribute)                            * not_portrait_
+    * no_keyword_                             (osxphotos.QueryOptions
+      (osxphotos.QueryOptions                 attribute)
+      attribute)                            * not_reference_
+    * no_likes_(osxphotos.QueryOptions        (osxphotos.QueryOptions
       attribute)                              attribute)
-    * no_title_(osxphotos.QueryOptions      * not_screenshot_
+    * no_location_                          * not_saved_to_library_
+      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * no_place_(osxphotos.QueryOptions      * not_screenshot_
       attribute)                              (osxphotos.QueryOptions
-    * not_burst_(osxphotos.QueryOptions       attribute)
+    * no_title_(osxphotos.QueryOptions        attribute)
       attribute)                            * not_selfie_
-    * not_cloudasset_                         (osxphotos.QueryOptions
-      (osxphotos.QueryOptions                 attribute)
-      attribute)                            * not_shared_
-    * not_edited_                             (osxphotos.QueryOptions
-      (osxphotos.QueryOptions                 attribute)
-      attribute)                            * not_slow_mo_
-    * not_favorite_                           (osxphotos.QueryOptions
-      (osxphotos.QueryOptions                 attribute)
-      attribute)                            * not_syndicated_
-                                              (osxphotos.QueryOptions
+    * not_burst_(osxphotos.QueryOptions       (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * not_cloudasset_                       * not_shared_
+      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * not_edited_                           * not_shared_moment_
+      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * not_favorite_                         * not_slow_mo_
+      (osxphotos.QueryOptions                 (osxphotos.QueryOptions
+      attribute)                              attribute)
+    * not_hdr_(osxphotos.QueryOptions       * not_syndicated_
+      attribute)                              (osxphotos.QueryOptions
                                               attribute)
                                             * not_time_lapse_
                                               (osxphotos.QueryOptions
                                               attribute)
 
 ***** O *****
-    * orientation_(osxphotos.PhotoInfo
-      property)                             * osxphotos-inspect command line
-    * original_filename_                      option
-      (osxphotos.PhotoInfo_property)              o --db
-    * original_filesize_                          o --detect-text
-      (osxphotos.PhotoInfo_property)              o --library
-    * original_height_                            o --template
-      (osxphotos.PhotoInfo_property)              o --theme
-    * original_orientation_                       o -t
-      (osxphotos.PhotoInfo_property)              o -T
-    * original_width_                       * osxphotos-install command line
-      (osxphotos.PhotoInfo_property)          option
-    * osxphotos                                   o --upgrade
-          o module                                o -U
-    * osxphotos command line option               o PACKAGES
-          o --version                       * osxphotos-keywords command line
-          o -v                                option
-    * osxphotos-add-locations command             o --db
-      line option                                 o --json
-          o --added-after                         o --library
-          o --added-before                        o PHOTOS_LIBRARY
-          o --added-in-last                 * osxphotos-labels command line
-          o --album                           option
-          o --burst                               o --db
-          o --cloudasset                          o --json
-          o --description                         o --library
-          o --dry-run                             o PHOTOS_LIBRARY
-          o --duplicate                     * osxphotos-list command line
-          o --edited                          option
-          o --exif                                o --json
-          o --external-edit                 * osxphotos-orphans command line
-          o --favorite                        option
-          o --folder                              o --db
-          o --from-date                           o --export
-          o --from-time                           o --library
-          o --has-comment                         o --theme
-          o --has-likes                           o --timestamp
-          o --has-raw                             o --verbose
-          o --hdr                                 o -V
-          o --hidden                        * osxphotos-persons command line
-          o --ignore-case                     option
-          o --in-album                            o --db
-          o --incloud                             o --json
-          o --is-reference                        o --library
-          o --keyword                             o PHOTOS_LIBRARY
-          o --label                         * osxphotos-places command line
-          o --live                            option
-          o --location                            o --db
-          o --max-size                            o --json
-          o --min-size                            o --library
-          o --missing                             o PHOTOS_LIBRARY
-          o --name                          * osxphotos-query command line
-          o --no-comment                      option
-          o --no-description                      o --add-to-album
-          o --no-keyword                          o --added-after
-          o --no-likes                            o --added-before
-          o --no-location                         o --added-in-last
-          o --no-place                            o --album
-          o --no-title                            o --burst
-          o --not-burst                           o --cloudasset
-          o --not-cloudasset                      o --count
-          o --not-edited                          o --db
-          o --not-favorite                        o --deleted
-          o --not-hdr                             o --deleted-only
-          o --not-hidden                          o --description
-          o --not-in-album                        o --duplicate
-          o --not-incloud                         o --edited
-          o --not-live                            o --exif
-          o --not-missing                         o --external-edit
-          o --not-panorama                        o --favorite
-          o --not-portrait                        o --field
-          o --not-reference                       o --folder
-          o --not-saved-to-library                o --from-date
-          o --not-screenshot                      o --from-time
-          o --not-selfie                          o --has-comment
-          o --not-shared                          o --has-likes
-          o --not-slow-mo                         o --has-raw
-          o --not-syndicated                      o --hdr
-          o --not-time-lapse                      o --hidden
-          o --only-movies                         o --ignore-case
-          o --only-photos                         o --in-album
-          o --panorama                            o --incloud
-          o --person                              o --is-reference
-          o --place                               o --json
-          o --portrait                            o --keyword
-          o --query-eval                          o --label
-          o --query-function                      o --library
-          o --regex                               o --live
-          o --saved-to-library                    o --location
-          o --screenshot                          o --max-size
-          o --selected                            o --min-size
-          o --selfie                              o --missing
-          o --shared                              o --name
-          o --slow-mo                             o --no-comment
-          o --syndicated                          o --no-description
-          o --theme                               o --no-keyword
-          o --time-lapse                          o --no-likes
-          o --timestamp                           o --no-location
-          o --title                               o --no-place
-          o --to-date                             o --no-title
-          o --to-time                             o --not-burst
-          o --uti                                 o --not-cloudasset
-          o --uuid                                o --not-edited
-          o --uuid-from-file                      o --not-favorite
-          o --verbose                             o --not-hdr
-          o --window                              o --not-hidden
-          o --year                                o --not-in-album
-          o -i                                    o --not-incloud
-          o -V                                    o --not-live
-          o -w                                    o --not-missing
-    * osxphotos-albums command line               o --not-panorama
-      option                                      o --not-portrait
-          o --db                                  o --not-reference
-          o --json                                o --not-saved-to-library
-          o --library                             o --not-screenshot
-          o PHOTOS_LIBRARY                        o --not-selfie
-    * osxphotos-batch-edit command line           o --not-shared
-      option                                      o --not-slow-mo
-          o --db                                  o --not-syndicated
-          o --description                         o --not-time-lapse
-          o --dry-run                             o --only-movies
-          o --keyword                             o --only-photos
-          o --library                             o --panorama
-          o --location                            o --person
-          o --replace-keywords                    o --place
-          o --theme                               o --portrait
-          o --timestamp                           o --print
-          o --title                               o --query-eval
-          o --undo                                o --query-function
-          o --verbose                             o --quiet
-          o -V                                    o --regex
-    * osxphotos-diff command line                 o --saved-to-library
-      option                                      o --screenshot
-          o --db                                  o --selected
-          o --library                             o --selfie
-          o --raw-output                          o --shared
-          o --style                               o --slow-mo
-          o --timestamp                           o --syndicated
-          o --verbose                             o --time-lapse
-          o -r                                    o --title
-          o -s                                    o --to-date
-          o -V                                    o --to-time
-          o DB2                                   o --uti
-    * osxphotos-dump command line                 o --uuid
-      option                                      o --uuid-from-file
-          o --db                                  o --year
-          o --deleted                             o -f
-          o --deleted-only                        o -i
-          o --field                               o PHOTOS_LIBRARY
-          o --json                          * osxphotos-repl command line
-          o --library                         option
-          o --print                               o --added-after
-          o -f                                    o --added-before
-          o PHOTOS_LIBRARY                        o --added-in-last
-    * osxphotos-exiftool command line             o --album
-      option                                      o --burst
-          o --album-keyword                       o --cloudasset
-          o --append                              o --db
-          o --db                                  o --deleted
-          o --db-config                           o --deleted-only
-          o --description-template                o --description
-          o --dry-run                             o --duplicate
-          o --exiftool-merge-keywords             o --edited
-          o --exiftool-merge-persons              o --emacs
-          o --exiftool-option                     o --exif
-          o --exiftool-path                       o --external-edit
-          o --exportdb                            o --favorite
-          o --ignore-date-modified                o --folder
-          o --keyword-template                    o --from-date
-          o --library                             o --from-time
-          o --load-config                         o --has-comment
-          o --person-keyword                      o --has-likes
-          o --replace-keywords                    o --has-raw
-          o --report                              o --hdr
-          o --save-config                         o --hidden
-          o --theme                               o --ignore-case
-          o --timestamp                           o --in-album
-          o --verbose                             o --incloud
-          o -V                                    o --is-reference
-          o EXPORT_DIRECTORY                      o --keyword
-    * osxphotos-export command line               o --label
-      option                                      o --library
-          o --add-exported-to-album               o --live
-          o --add-missing-to-album                o --location
-          o --add-skipped-to-album                o --max-size
-          o --added-after                         o --min-size
-          o --added-before                        o --missing
-          o --added-in-last                       o --name
-          o --album                               o --no-comment
-          o --album-keyword                       o --no-description
-          o --alt-copy                            o --no-keyword
-          o --append                              o --no-likes
-          o --burst                               o --no-location
-          o --cleanup                             o --no-place
-          o --cloudasset                          o --no-title
-          o --config-only                         o --not-burst
-          o --convert-to-jpeg                     o --not-cloudasset
-          o --current-name                        o --not-edited
-          o --db                                  o --not-favorite
-          o --deleted                             o --not-hdr
-          o --deleted-only                        o --not-hidden
-          o --description                         o --not-in-album
-          o --description-template                o --not-incloud
-          o --directory                           o --not-live
-          o --download-missing                    o --not-missing
-          o --dry-run                             o --not-panorama
-          o --duplicate                           o --not-portrait
-          o --edited                              o --not-reference
-          o --edited-suffix                       o --not-saved-to-library
-          o --exif                                o --not-screenshot
-          o --exiftool                            o --not-selfie
-          o --exiftool-merge-keywords             o --not-shared
+    * orientation_(osxphotos.PhotoInfo      * osxphotos-inspect command line
+      property)                               option
+    * original_filename_                          o --db
+      (osxphotos.PhotoInfo_property)              o --detect-text
+    * original_filesize_                          o --library
+      (osxphotos.PhotoInfo_property)              o --template
+    * original_height_                            o --theme
+      (osxphotos.PhotoInfo_property)              o -t
+    * original_orientation_                       o -T
+      (osxphotos.PhotoInfo_property)        * osxphotos-install command line
+    * original_width_                         option
+      (osxphotos.PhotoInfo_property)              o --upgrade
+    * osxphotos                                   o -U
+          o module                                o PACKAGES
+    * osxphotos command line option         * osxphotos-keywords command line
+          o --version                         option
+          o -v                                    o --db
+    * osxphotos-add-locations command             o --json
+      line option                                 o --library
+          o --added-after                         o PHOTOS_LIBRARY
+          o --added-before                  * osxphotos-labels command line
+          o --added-in-last                   option
+          o --album                               o --db
+          o --burst                               o --json
+          o --cloudasset                          o --library
+          o --description                         o PHOTOS_LIBRARY
+          o --dry-run                       * osxphotos-list command line
+          o --duplicate                       option
+          o --edited                              o --json
+          o --exif                          * osxphotos-orphans command line
+          o --external-edit                   option
+          o --favorite                            o --db
+          o --folder                              o --export
+          o --from-date                           o --library
+          o --from-time                           o --theme
+          o --has-comment                         o --timestamp
+          o --has-likes                           o --verbose
+          o --has-raw                             o -V
+          o --hdr                           * osxphotos-persons command line
+          o --hidden                          option
+          o --ignore-case                         o --db
+          o --in-album                            o --json
+          o --incloud                             o --library
+          o --is-reference                        o PHOTOS_LIBRARY
+          o --keyword                       * osxphotos-places command line
+          o --label                           option
+          o --live                                o --db
+          o --location                            o --json
+          o --max-size                            o --library
+          o --min-size                            o PHOTOS_LIBRARY
+          o --missing                       * osxphotos-query command line
+          o --name                            option
+          o --no-comment                          o --add-to-album
+          o --no-description                      o --added-after
+          o --no-keyword                          o --added-before
+          o --no-likes                            o --added-in-last
+          o --no-location                         o --album
+          o --no-place                            o --burst
+          o --no-title                            o --cloudasset
+          o --not-burst                           o --count
+          o --not-cloudasset                      o --db
+          o --not-edited                          o --deleted
+          o --not-favorite                        o --deleted-only
+          o --not-hdr                             o --description
+          o --not-hidden                          o --duplicate
+          o --not-in-album                        o --edited
+          o --not-incloud                         o --exif
+          o --not-live                            o --external-edit
+          o --not-missing                         o --favorite
+          o --not-panorama                        o --field
+          o --not-portrait                        o --folder
+          o --not-reference                       o --from-date
+          o --not-saved-to-library                o --from-time
+          o --not-screenshot                      o --has-comment
+          o --not-selfie                          o --has-likes
+          o --not-shared                          o --has-raw
+          o --not-shared-moment                   o --hdr
+          o --not-slow-mo                         o --hidden
+          o --not-syndicated                      o --ignore-case
+          o --not-time-lapse                      o --in-album
+          o --only-movies                         o --incloud
+          o --only-photos                         o --is-reference
+          o --panorama                            o --json
+          o --person                              o --keyword
+          o --place                               o --label
+          o --portrait                            o --library
+          o --query-eval                          o --live
+          o --query-function                      o --location
+          o --regex                               o --max-size
+          o --saved-to-library                    o --min-size
+          o --screenshot                          o --missing
+          o --selected                            o --name
+          o --selfie                              o --no-comment
+          o --shared                              o --no-description
+          o --shared-moment                       o --no-keyword
+          o --slow-mo                             o --no-likes
+          o --syndicated                          o --no-location
+          o --theme                               o --no-place
+          o --time-lapse                          o --no-title
+          o --timestamp                           o --not-burst
+          o --title                               o --not-cloudasset
+          o --to-date                             o --not-edited
+          o --to-time                             o --not-favorite
+          o --uti                                 o --not-hdr
+          o --uuid                                o --not-hidden
+          o --uuid-from-file                      o --not-in-album
+          o --verbose                             o --not-incloud
+          o --window                              o --not-live
+          o --year                                o --not-missing
+          o -i                                    o --not-panorama
+          o -V                                    o --not-portrait
+          o -w                                    o --not-reference
+    * osxphotos-albums command line               o --not-saved-to-library
+      option                                      o --not-screenshot
+          o --db                                  o --not-selfie
+          o --json                                o --not-shared
+          o --library                             o --not-shared-moment
+          o PHOTOS_LIBRARY                        o --not-slow-mo
+    * osxphotos-batch-edit command line           o --not-syndicated
+      option                                      o --not-time-lapse
+          o --db                                  o --only-movies
+          o --description                         o --only-photos
+          o --dry-run                             o --panorama
+          o --keyword                             o --person
+          o --library                             o --place
+          o --location                            o --portrait
+          o --replace-keywords                    o --print
+          o --theme                               o --query-eval
+          o --timestamp                           o --query-function
+          o --title                               o --quiet
+          o --undo                                o --regex
+          o --verbose                             o --saved-to-library
+          o -V                                    o --screenshot
+    * osxphotos-diff command line                 o --selected
+      option                                      o --selfie
+          o --db                                  o --shared
+          o --library                             o --shared-moment
+          o --raw-output                          o --slow-mo
+          o --style                               o --syndicated
+          o --timestamp                           o --time-lapse
+          o --verbose                             o --title
+          o -r                                    o --to-date
+          o -s                                    o --to-time
+          o -V                                    o --uti
+          o DB2                                   o --uuid
+    * osxphotos-dump command line                 o --uuid-from-file
+      option                                      o --year
+          o --db                                  o -f
+          o --deleted                             o -i
+          o --deleted-only                        o PHOTOS_LIBRARY
+          o --field                         * osxphotos-repl command line
+          o --json                            option
+          o --library                             o --added-after
+          o --print                               o --added-before
+          o -f                                    o --added-in-last
+          o PHOTOS_LIBRARY                        o --album
+    * osxphotos-exiftool command line             o --burst
+      option                                      o --cloudasset
+          o --album-keyword                       o --db
+          o --append                              o --deleted
+          o --db                                  o --deleted-only
+          o --db-config                           o --description
+          o --description-template                o --duplicate
+          o --dry-run                             o --edited
+          o --exiftool-merge-keywords             o --emacs
+          o --exiftool-merge-persons              o --exif
+          o --exiftool-option                     o --external-edit
+          o --exiftool-path                       o --favorite
+          o --exportdb                            o --folder
+          o --ignore-date-modified                o --from-date
+          o --keyword-template                    o --from-time
+          o --library                             o --has-comment
+          o --load-config                         o --has-likes
+          o --person-keyword                      o --has-raw
+          o --replace-keywords                    o --hdr
+          o --report                              o --hidden
+          o --save-config                         o --ignore-case
+          o --theme                               o --in-album
+          o --timestamp                           o --incloud
+          o --verbose                             o --is-reference
+          o -V                                    o --keyword
+          o EXPORT_DIRECTORY                      o --label
+    * osxphotos-export command line               o --library
+      option                                      o --live
+          o --add-exported-to-album               o --location
+          o --add-missing-to-album                o --max-size
+          o --add-skipped-to-album                o --min-size
+          o --added-after                         o --missing
+          o --added-before                        o --name
+          o --added-in-last                       o --no-comment
+          o --album                               o --no-description
+          o --album-keyword                       o --no-keyword
+          o --alt-copy                            o --no-likes
+          o --append                              o --no-location
+          o --burst                               o --no-place
+          o --cleanup                             o --no-title
+          o --cloudasset                          o --not-burst
+          o --config-only                         o --not-cloudasset
+          o --convert-to-jpeg                     o --not-edited
+          o --current-name                        o --not-favorite
+          o --db                                  o --not-hdr
+          o --deleted                             o --not-hidden
+          o --deleted-only                        o --not-in-album
+          o --description                         o --not-incloud
+          o --description-template                o --not-live
+          o --directory                           o --not-missing
+          o --download-missing                    o --not-panorama
+          o --dry-run                             o --not-portrait
+          o --duplicate                           o --not-reference
+          o --edited                              o --not-saved-to-library
+          o --edited-suffix                       o --not-screenshot
+          o --exif                                o --not-selfie
+          o --exiftool                            o --not-shared
+          o --exiftool-merge-keywords             o --not-shared-moment
           o --exiftool-merge-persons              o --not-slow-mo
           o --exiftool-option                     o --not-syndicated
           o --exiftool-path                       o --not-time-lapse
           o --export-aae                          o --only-movies
           o --export-as-hardlink                  o --only-photos
           o --export-by-date                      o --panorama
           o --exportdb                            o --person
@@ -1502,65 +1516,66 @@
           o --filename                            o --query-function
           o --finder-tag-keywords                 o --regex
           o --finder-tag-template                 o --saved-to-library
           o --folder                              o --screenshot
           o --force-update                        o --selected
           o --from-date                           o --selfie
           o --from-time                           o --shared
-          o --has-comment                         o --slow-mo
-          o --has-likes                           o --syndicated
-          o --has-raw                             o --time-lapse
-          o --hdr                                 o --title
-          o --hidden                              o --to-date
-          o --ignore-case                         o --to-time
-          o --ignore-date-modified                o --uti
-          o --ignore-signature                    o --uuid
-          o --in-album                            o --uuid-from-file
-          o --incloud                             o --year
-          o --is-reference                        o -i
-          o --jpeg-ext                      * osxphotos-run command line option
-          o --jpeg-quality                        o --help
-          o --keep                                o -h
-          o --keyword                             o ARGS
-          o --keyword-template                    o PYTHON_FILE
-          o --label                         * osxphotos-show command line
-          o --library                         option
-          o --limit                               o --db
-          o --live                                o --library
-          o --load-config                         o UUID_OR_NAME
-          o --location                      * osxphotos-snap command line
-          o --max-size                        option
-          o --min-size                            o --db
-          o --missing                             o --library
-          o --name                          * osxphotos-sync command line
-          o --no-comment                      option
-          o --no-description                      o --added-after
-          o --no-keyword                          o --added-before
-          o --no-likes                            o --added-in-last
-          o --no-location                         o --album
-          o --no-place                            o --append
-          o --no-progress                         o --burst
-          o --no-title                            o --cloudasset
-          o --not-burst                           o --db
-          o --not-cloudasset                      o --description
-          o --not-edited                          o --dry-run
-          o --not-favorite                        o --duplicate
-          o --not-hdr                             o --edited
-          o --not-hidden                          o --exif
-          o --not-in-album                        o --export
-          o --not-incloud                         o --external-edit
-          o --not-live                            o --favorite
-          o --not-missing                         o --folder
-          o --not-panorama                        o --from-date
-          o --not-portrait                        o --from-time
-          o --not-reference                       o --has-comment
-          o --not-saved-to-library                o --has-likes
-          o --not-screenshot                      o --has-raw
-          o --not-selfie                          o --hdr
-          o --not-shared                          o --hidden
+          o --has-comment                         o --shared-moment
+          o --has-likes                           o --slow-mo
+          o --has-raw                             o --syndicated
+          o --hdr                                 o --time-lapse
+          o --hidden                              o --title
+          o --ignore-case                         o --to-date
+          o --ignore-date-modified                o --to-time
+          o --ignore-signature                    o --uti
+          o --in-album                            o --uuid
+          o --incloud                             o --uuid-from-file
+          o --is-reference                        o --year
+          o --jpeg-ext                            o -i
+          o --jpeg-quality                  * osxphotos-run command line option
+          o --keep                                o --help
+          o --keyword                             o -h
+          o --keyword-template                    o ARGS
+          o --label                               o PYTHON_FILE
+          o --library                       * osxphotos-show command line
+          o --limit                           option
+          o --live                                o --db
+          o --load-config                         o --library
+          o --location                            o UUID_OR_NAME
+          o --max-size                      * osxphotos-snap command line
+          o --min-size                        option
+          o --missing                             o --db
+          o --name                                o --library
+          o --no-comment                    * osxphotos-sync command line
+          o --no-description                  option
+          o --no-keyword                          o --added-after
+          o --no-likes                            o --added-before
+          o --no-location                         o --added-in-last
+          o --no-place                            o --album
+          o --no-progress                         o --append
+          o --no-title                            o --burst
+          o --not-burst                           o --cloudasset
+          o --not-cloudasset                      o --db
+          o --not-edited                          o --description
+          o --not-favorite                        o --dry-run
+          o --not-hdr                             o --duplicate
+          o --not-hidden                          o --edited
+          o --not-in-album                        o --exif
+          o --not-incloud                         o --export
+          o --not-live                            o --external-edit
+          o --not-missing                         o --favorite
+          o --not-panorama                        o --folder
+          o --not-portrait                        o --from-date
+          o --not-reference                       o --from-time
+          o --not-saved-to-library                o --has-comment
+          o --not-screenshot                      o --has-likes
+          o --not-selfie                          o --has-raw
+          o --not-shared                          o --hdr
+          o --not-shared-moment                   o --hidden
           o --not-slow-mo                         o --ignore-case
           o --not-syndicated                      o --import
           o --not-time-lapse                      o --in-album
           o --only-movies                         o --incloud
           o --only-new                            o --is-reference
           o --only-photos                         o --keyword
           o --original-suffix                     o --label
@@ -1585,20 +1600,21 @@
           o --retry                               o --not-favorite
           o --save-config                         o --not-hdr
           o --saved-to-library                    o --not-hidden
           o --screenshot                          o --not-in-album
           o --selected                            o --not-incloud
           o --selfie                              o --not-live
           o --shared                              o --not-missing
-          o --sidecar                             o --not-panorama
-          o --sidecar-drop-ext                    o --not-portrait
-          o --skip-bursts                         o --not-reference
-          o --skip-edited                         o --not-saved-to-library
-          o --skip-live                           o --not-screenshot
-          o --skip-original-if-edited             o --not-selfie
+          o --shared-moment                       o --not-panorama
+          o --sidecar                             o --not-portrait
+          o --sidecar-drop-ext                    o --not-reference
+          o --skip-bursts                         o --not-saved-to-library
+          o --skip-edited                         o --not-screenshot
+          o --skip-live                           o --not-selfie
+          o --skip-original-if-edited             o --not-shared-moment
           o --skip-raw                            o --not-slow-mo
           o --skip-uuid                           o --not-syndicated
           o --skip-uuid-from-file                 o --not-time-lapse
           o --slow-mo                             o --only-movies
           o --strip                               o --only-photos
           o --syndicated                          o --panorama
           o --theme                               o --person
@@ -1609,108 +1625,108 @@
           o --to-date                             o --regex
           o --to-time                             o --report
           o --touch-file                          o --saved-to-library
           o --update                              o --screenshot
           o --update-errors                       o --selected
           o --use-photokit                        o --selfie
           o --use-photos-export                   o --set
-          o --uti                                 o --slow-mo
-          o --uuid                                o --syndicated
-          o --uuid-from-file                      o --theme
-          o --verbose                             o --time-lapse
-          o --xattr-template                      o --timestamp
-          o --year                                o --title
-          o -i                                    o --to-date
-          o -V                                    o --to-time
-          o DEST                                  o --unmatched
-          o PHOTOS_LIBRARY                        o --uti
-    * osxphotos-exportdb command line             o --uuid
-      option                                      o --uuid-from-file
-          o --append                              o --verbose
-          o --check-signatures                    o --year
-          o --delete-file                         o -A
-          o --delete-uuid                         o -e
-          o --dry-run                             o -i, [1]
-          o --errors                              o -m
-          o --export-dir                          o -R
-          o --info                                o -s
-          o --last-errors                         o -U
-          o --last-run                            o -V
-          o --migrate                       * osxphotos-theme command line
-          o --migrate-photos-library          option
-          o --report                              o --clone
-          o --save-config                         o --config
-          o --sql                                 o --default
-          o --theme                               o --delete
-          o --timestamp                           o --edit
-          o --touch-file                          o --list
-          o --update-signatures                   o --preview
-          o --uuid-files                    * osxphotos-timewarp command line
-          o --uuid-info                       option
-          o --vacuum                              o --add-to-album
-          o --verbose                             o --compare-exif
-          o --version                             o --date
-          o -V                                    o --date-added
-          o EXPORT_DATABASE                       o --date-added-from-photo
-    * osxphotos-help command line                 o --date-delta
-      option                                      o --exiftool-path
-          o SUBTOPIC                              o --force
-          o TOPIC                                 o --function
-    * osxphotos-import command line               o --inspect
-      option                                      o --library
-          o --album                               o --match-time
-          o --append                              o --parse-date
-          o --check-templates                     o --plain
-          o --clear-location                      o --pull-exif
-          o --clear-metadata                      o --push-exif
-          o --description                         o --theme
-          o --dup-check                           o --time
-          o --exiftool                            o --time-delta
-          o --exiftool-path                       o --timestamp, [1]
-          o --glob                                o --timezone
-          o --keyword                             o --use-file-time
-          o --location                            o --verbose
-          o --merge-keywords                      o -a
-          o --no-progress                         o -c
-          o --parse-date                          o -d
-          o --post-function                       o -D
-          o --relative-to                         o -e
-          o --report                              o -F
-          o --resume                              o -f
-          o --split-folder                        o -i
-          o --theme                               o -L
-          o --timestamp                           o -M
-          o --title                               o -m
-          o --verbose                             o -p
-          o --walk                                o -P
-          o -a                                    o -t
-          o -C                                    o -T
-          o -d                                    o -V
-          o -D                                    o -z
-          o -e                              * osxphotos-tutorial command line
-          o -f                                option
-          o -g                                    o WIDTH
-          o -k                              * osxphotos-uninstall command line
-          o -l                                option
-          o -L                                    o --yes
-          o -m                                    o -y
-          o -P                                    o PACKAGES
-          o -p                              * osxphotos-uuid command line
-          o -r                                option
-          o -R                                    o --filename
-          o -t                                    o -f
-          o -V                              * osxphotos-version command line
-          o -w                                option
-          o FILES                                 o --run
-    * osxphotos-info command line           * overwrite_
-      option                                  (osxphotos.ExportOptions
-          o --db                              attribute)
-          o --json                          * owner_(osxphotos.PhotoInfo
-          o --library                         property)
-          o PHOTOS_LIBRARY
+          o --uti                                 o --shared-moment
+          o --uuid                                o --slow-mo
+          o --uuid-from-file                      o --syndicated
+          o --verbose                             o --theme
+          o --xattr-template                      o --time-lapse
+          o --year                                o --timestamp
+          o -i                                    o --title
+          o -V                                    o --to-date
+          o DEST                                  o --to-time
+          o PHOTOS_LIBRARY                        o --unmatched
+    * osxphotos-exportdb command line             o --uti
+      option                                      o --uuid
+          o --append                              o --uuid-from-file
+          o --check-signatures                    o --verbose
+          o --delete-file                         o --year
+          o --delete-uuid                         o -A
+          o --dry-run                             o -e
+          o --errors                              o -i, [1]
+          o --export-dir                          o -m
+          o --info                                o -R
+          o --last-errors                         o -s
+          o --last-run                            o -U
+          o --migrate                             o -V
+          o --migrate-photos-library        * osxphotos-theme command line
+          o --report                          option
+          o --save-config                         o --clone
+          o --sql                                 o --config
+          o --theme                               o --default
+          o --timestamp                           o --delete
+          o --touch-file                          o --edit
+          o --update-signatures                   o --list
+          o --uuid-files                          o --preview
+          o --uuid-info                     * osxphotos-timewarp command line
+          o --vacuum                          option
+          o --verbose                             o --add-to-album
+          o --version                             o --compare-exif
+          o -V                                    o --date
+          o EXPORT_DATABASE                       o --date-added
+    * osxphotos-help command line                 o --date-added-from-photo
+      option                                      o --date-delta
+          o SUBTOPIC                              o --exiftool-path
+          o TOPIC                                 o --force
+    * osxphotos-import command line               o --function
+      option                                      o --inspect
+          o --album                               o --library
+          o --append                              o --match-time
+          o --check-templates                     o --parse-date
+          o --clear-location                      o --plain
+          o --clear-metadata                      o --pull-exif
+          o --description                         o --push-exif
+          o --dup-check                           o --theme
+          o --exiftool                            o --time
+          o --exiftool-path                       o --time-delta
+          o --glob                                o --timestamp, [1]
+          o --keyword                             o --timezone
+          o --location                            o --use-file-time
+          o --merge-keywords                      o --verbose
+          o --no-progress                         o -a
+          o --parse-date                          o -c
+          o --post-function                       o -d
+          o --relative-to                         o -D
+          o --report                              o -e
+          o --resume                              o -F
+          o --split-folder                        o -f
+          o --theme                               o -i
+          o --timestamp                           o -L
+          o --title                               o -M
+          o --verbose                             o -m
+          o --walk                                o -p
+          o -a                                    o -P
+          o -C                                    o -t
+          o -d                                    o -T
+          o -D                                    o -V
+          o -e                                    o -z
+          o -f                              * osxphotos-tutorial command line
+          o -g                                option
+          o -k                                    o WIDTH
+          o -l                              * osxphotos-uninstall command line
+          o -L                                option
+          o -m                                    o --yes
+          o -P                                    o -y
+          o -p                                    o PACKAGES
+          o -r                              * osxphotos-uuid command line
+          o -R                                option
+          o -t                                    o --filename
+          o -V                                    o -f
+          o -w                              * osxphotos-version command line
+          o FILES                             option
+    * osxphotos-info command line                 o --run
+      option                                * overwrite_
+          o --db                              (osxphotos.ExportOptions
+          o --json                            attribute)
+          o --library                       * owner_(osxphotos.PhotoInfo
+          o PHOTOS_LIBRARY                    property)
 
 ***** P *****
     * PACKAGES                              * photos()_(osxphotos.PhotosDB
           o osxphotos-install_command         method)
             line_option                     * photos_by_uuid()_
           o osxphotos-uninstall_command       (osxphotos.PhotosDB_method)
             line_option                     * PHOTOS_LIBRARY
@@ -1790,51 +1806,55 @@
       method)                                 property)
     * render_options_                       * roll_pitch_yaw()_
       (osxphotos.ExportOptions                (osxphotos.FaceInfo_method)
       attribute)                            * run_commands()_
                                               (osxphotos.ExifTool_method)
 
 ***** S *****
-    * saved_to_library_                     * sidecar_(osxphotos.ExportOptions
-      (osxphotos.PhotoInfo_property)          attribute)
-          o (osxphotos.QueryOptions         * sidecar_drop_ext_
-            attribute)                        (osxphotos.ExportOptions
-    * score_(osxphotos.PhotoInfo              attribute)
-      property)                             * size_pixels_(osxphotos.FaceInfo
-    * ScoreInfo_(class_in_osxphotos)          property)
-    * screenshot_(osxphotos.PhotoInfo       * slow_mo_(osxphotos.PhotoInfo
-      property)                               property)
-          o (osxphotos.QueryOptions               o (osxphotos.QueryOptions
-            attribute)                              attribute)
-    * search_info_(osxphotos.PhotoInfo      * sort_order_(osxphotos.AlbumInfo
+                                            * shared_moment_
+                                              (osxphotos.PhotoInfo_property)
+    * saved_to_library_                           o (osxphotos.QueryOptions
+      (osxphotos.PhotoInfo_property)                attribute)
+          o (osxphotos.QueryOptions         * sidecar_(osxphotos.ExportOptions
+            attribute)                        attribute)
+    * score_(osxphotos.PhotoInfo            * sidecar_drop_ext_
+      property)                               (osxphotos.ExportOptions
+    * ScoreInfo_(class_in_osxphotos)          attribute)
+    * screenshot_(osxphotos.PhotoInfo       * size_pixels_(osxphotos.FaceInfo
       property)                               property)
-    * search_info_normalized_                     o (osxphotos.PersonInfo
-      (osxphotos.PhotoInfo_property)                property)
-    * SearchInfo_(class_in_osxphotos)       * source_(osxphotos.SearchInfo
-    * season_(osxphotos.SearchInfo            property)
-      property)                             * start_date_(osxphotos.MomentInfo
+          o (osxphotos.QueryOptions         * slow_mo_(osxphotos.PhotoInfo
+            attribute)                        property)
+    * search_info_(osxphotos.PhotoInfo            o (osxphotos.QueryOptions
+      property)                                     attribute)
+    * search_info_normalized_               * sort_order_(osxphotos.AlbumInfo
+      (osxphotos.PhotoInfo_property)          property)
+    * SearchInfo_(class_in_osxphotos)             o (osxphotos.PersonInfo
+    * season_(osxphotos.SearchInfo                  property)
+      property)                             * source_(osxphotos.SearchInfo
     * selected_(osxphotos.QueryOptions        property)
-      attribute)                            * state_(osxphotos.SearchInfo
+      attribute)                            * start_date_(osxphotos.MomentInfo
     * selfie_(osxphotos.PhotoInfo             property)
-      property)                             * state_abbreviation_
-          o (osxphotos.QueryOptions           (osxphotos.SearchInfo_property)
-            attribute)                      * streets_(osxphotos.SearchInfo
-    * set_config()_(osxphotos.ExportDB        property)
-      method)                               * strip_(osxphotos.ExportOptions
-    * set_debug()_(in_module_osxphotos)       attribute)
-    * set_export_results()_                 * subfolders_(osxphotos.FolderInfo
-      (osxphotos.ExportDB_method)             property)
-    * set_photoinfo_for_uuid()_             * subtitle_(osxphotos.MomentInfo
-      (osxphotos.ExportDB_method)             property)
-    * setvalue()_(osxphotos.ExifTool        * SUBTOPIC
-      method)                                     o osxphotos-help_command_line
-    * shared_(osxphotos.PhotoInfo                   option
-      property)                             * syndicated_(osxphotos.PhotoInfo
+      property)                             * state_(osxphotos.SearchInfo
           o (osxphotos.QueryOptions           property)
-            attribute)                            o (osxphotos.QueryOptions
+            attribute)                      * state_abbreviation_
+    * set_config()_(osxphotos.ExportDB        (osxphotos.SearchInfo_property)
+      method)                               * streets_(osxphotos.SearchInfo
+    * set_debug()_(in_module_osxphotos)       property)
+    * set_export_results()_                 * strip_(osxphotos.ExportOptions
+      (osxphotos.ExportDB_method)             attribute)
+    * set_photoinfo_for_uuid()_             * subfolders_(osxphotos.FolderInfo
+      (osxphotos.ExportDB_method)             property)
+    * setvalue()_(osxphotos.ExifTool        * subtitle_(osxphotos.MomentInfo
+      method)                                 property)
+    * shared_(osxphotos.PhotoInfo           * SUBTOPIC
+      property)                                   o osxphotos-help_command_line
+          o (osxphotos.QueryOptions                 option
+            attribute)                      * syndicated_(osxphotos.PhotoInfo
+                                              property)
+                                                  o (osxphotos.QueryOptions
                                                     attribute)
 
 ***** T *****
     * tables()_(osxphotos.PhotoInfo
       method)
     * text_found_(osxphotos.SearchInfo
       property)
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
-        <title>osxphotos 0.60.8 documentation</title>
+        <title>osxphotos 0.60.9 documentation</title>
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
-      <a href="#"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="#"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -538,14 +538,15 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.saved_to_library"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.saved_to_library</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.shared_moment"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared_moment</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.syndicated"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.syndicated</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
@@ -706,14 +707,16 @@
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.uti"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uti</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.uuid"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uuid</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.year"><code class="docutils literal notranslate"><span class="pre">QueryOptions.year</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.syndicated</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.not_syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_syndicated</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.saved_to_library</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.not_saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_saved_to_library</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.shared_moment"><code class="docutils literal notranslate"><span class="pre">QueryOptions.shared_moment</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.QueryOptions.not_shared_moment"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_shared_moment</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.ScoreInfo"><code class="docutils literal notranslate"><span class="pre">ScoreInfo</span></code></a><ul>
 <li class="toctree-l3"><a class="reference internal" href="reference.html#osxphotos.ScoreInfo.asdict"><code class="docutils literal notranslate"><span class="pre">ScoreInfo.asdict()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="reference.html#osxphotos.SearchInfo"><code class="docutils literal notranslate"><span class="pre">SearchInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -340,14 +340,15 @@
                 # PhotoInfo.saved_to_library
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
+                # PhotoInfo.shared_moment
                 # PhotoInfo.slow_mo
                 # PhotoInfo.syndicated
                 # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
@@ -498,14 +499,16 @@
                 # QueryOptions.uti
                 # QueryOptions.uuid
                 # QueryOptions.year
                 # QueryOptions.syndicated
                 # QueryOptions.not_syndicated
                 # QueryOptions.saved_to_library
                 # QueryOptions.not_saved_to_library
+                # QueryOptions.shared_moment
+                # QueryOptions.not_shared_moment
           o ScoreInfo
                 # ScoreInfo.asdict()
           o SearchInfo
                 # SearchInfo.activities
                 # SearchInfo.all
                 # SearchInfo.asdict()
                 # SearchInfo.bodies_of_water
```

#### docs/objects.inv

##### Sphinx inventory

```diff
@@ -1,47 +1,1257 @@
 # Sphinx inventory version 2
 # Project: osxphotos
 # Version: 
 # The remainder of this file is compressed using zlib.
-#Ev|5WWxmLHudkL<ja*2ܾ	իHmp4q}%ߵQ
 
-xڵv8~
-Y,ҧzsU>jklYݽ⡒H%KL2dJV5Iwą?+R3A n~>vc7ܜ_tKn~فݳA~77w=trߔpǥam9T~l<vX_4 }wfh0¹/wO*_zz1k~6W=%Ӊo֓mpuM۲d[_usì]i=e[!_s`l"CW}؇3n2xo!"]׶l?v߳rdšnXѳ=5(Hl$*0Ϊʱ,(hr<n\j䊘ja$ѳҌpUIP@iO I.d2fq)
-(g?a|#d{asޱ9s|c߀Y}mo!<(C8edy)FT)m*N0-ׂj>tQ |VDDLwRlP˾jCSãN0.r=ub5˹uzI?CMz5n']Y˝^1l9R65>q{}_S?35'Q ݾ4581[b)jԎ[/{r8	|!?2cbKĻ 6xjz$ueO'#>BtkA]GJ !9M
-]Oy.+J6_fU %QzD`AodLz[6`j%aO|,U5pݪjk}iH6o՚}-w+}ѧn\J^uڢw)L?B}4a!u_C;NЪWNM/?o3d+h*7;Uv9TybI Ɨ/fTV?FukV:ȝ&c<\Tw Ol^k$f{4d7c^v[S^e'vqL7sLҴ !8Se?h8`/1϶X:d?}s噽@F͙S-g ych:XṊG-2ZfVS`D|04F~da/#J>d^XUb~c~zCXܰC=r|ypӂ@!TP^O{cʂ0u5oKU<fK{ӑ)e}q,#
-rTFؠܲ(
-^Dl?0e(Q>Ũ Ku97d3|lqk`jԖ|rl˦y89W6Y #}݂ߝE_63&;ǪYxD5^Տ5~^˥8q[9rF6'
-2kgp' se`jS>d/mOeSΩMNfЙOrs|+Z̊ea"2f[vRW
-Tzܘ<5z/3ڳ$eY%
-j7M v nD(Д!}W^!|oRfz"HP	enJd9b/{p;bw=CM{ځge?n Ok{6m6k[u3(>YICe}bES 񗱆Is xfanʝ3,^oĎLVsv{ёg>VNry=ֈ+;&k $qЉNYgRS"4ebyu:I<¼F*}̍8\Z{y+ӥQF<]s
-%*/z5>e#*w33NJsn^ޓSnB(|@Ik[(5g>tP
-vVtw2N-e/];1wY')˾ vMj!Dʆd?PlIy kf%23o/Bs3f) rӈ徻#!bv=hLY浶znd! /c[5z+bs>
-<Cy>@ۂ1N9fnNF1*TE6,c	#?;z>a  G}ߝt' t!bC8B򂀊p+ ^Aٗf8:F 7uyLzNʌp*&$-_'+(,L2`oWкn9vԁVO8<`(a,@l
-)O"(P`'3E!NhB<
-DF89@8eI^`B8,9-nS2u9Cn+@On$={dq:=Hݝ|.E&cmf5XP0WYq23O̚-c\un+*Z_CW+.CRf-s({vKXELUΕcU k̗vn~ƁLp0kюm+N<t*T_U<!/w>k<f_Ãd}gň6<Łw
-<HO$fJTov"N!,"= fUx*9CR@a`0".R$R
-g?d|XsxO?߁qPZPS8?P1O'Yzˬb9dq+}U6CZ:ϻDV˯I~/-Ty+ψf
->E)r~]J5k(짃2?|c$ǎR-VH6Ycq'"U)ʣ2q'].,sx픰oaTu{+v?ݿyxnGQ[Ծ>G֪7^
-
-sB}?>O5{\8v79ooD&_3P_ԻNm]YU;xv2Empr3/w[yud=Y۝L#+PRRI+ABRN@PRbn`brN{"IG{t4!)")>-r
-Д\PJ	jRiEHiW	*%kS$$%u,@Ӈb.fMNedMJ[")S<aīD"DTnNvHK-#-2jH:
-φ1hɬ#hDJF7$DEA'LE0RBNf,#)}aT"IG!R22畠!CY^VD7ʊy޶5zYSS4-XR'4!H5Yf- җdeMlě&Ht)bUZ:5-g]59KckB.fM&,gU$RgMp'~ZQL*?V/`JkJOUQJTU1JSU{ٝ:ƬMٴTŉ&*vv*(R N#(U9|OӘUc>@QՅ^dPw'/ʺ-)%NW %5m3]9ٓ)X"NWL)rir)q<2f$%6}yǆ<Z
-"n3j R2AB'/ThR(RϬh]>)RUG
-52S@	Y-L4;&kz^AbNŧ?~yw+Pw{2~98"8\IwrEN3(;3aʹX8Urf=ȝJy$9:7c+t"پL`x>!liECC7bV p,؝4kо|u|n"ks%aC	"8F7aئ?_ H8rHfWt|C^.NV|=`ޥdyaCMRoG*;xئ(d8>r`Ąg
-8z2fݾk#cB,2n?wb#ZHvy7&&k;_Ww!1dDDd
-`<bSd:DQYQAS׵Tӕmr	$"E[0[ry.ǟP\DG":H3.!",-_`ly3KG ZX}{-~rW|ws}'I\Qe 5QGHQQvG@Q~_$CϓRB 9<So^H@g͓~3OYhLaEF>^_A6V/koam[v0~˩0|>&Q#*2c.}8LdT\@P");iȦ`F	0fA rX*F~zͬu޽vBpb`YMY`wpɮ`r3|3|4qh2
-F!vRǫVR(rsJ*X$^T=諦nH2&%
-$ͥ"!N}5X~j~KKFXnYZ}7,Y$9'!NX(mc46߳w ,1`9<?օ{X1 pg7zYfWs<<Ȇ:XfI,)1-AR-aC*x(A'-?~=
-<+c%ރ!5xJ<1mOIZLn*Rʜ
-T82:^i	w2}f 9֪xTR+[z آ2N4MF=uwiRiXݜDK.M1+4^!\Vɡ'VHi'g{ 	 υw#!.4EK3.mOWI˗P99_D
-($<Z2i!{"I3E)`L (t%DLP7Ъ>8ZɒsIރ+.0
-0~9(s<Rt*.rFLDJ Xֈ8)a&~EU]2BϬ:')d~HO8魯-=aLXy&W#XiGcM
-`ra.BѪ_)D/+G&0֭,ra	s<~0IbGUA(4D28d:蚯X5U]sѨ	^~Klsئp̃F>.@r>d[ϙo`ŅlkGs^1[D*M%vry=}qeJ[աr:,g>gsxFtjlצalgm
-%`8c+T_G;A<!K.c}na'p>%h:-ic$s53xW8"(_Rý2ya+%~vQTP(lOQyCDDl4%ȩmpJ.!-*HdtQ"1/!=%tљHy9?" ^ŊCܴq	)ZT?:738aoiZ"I4q3qJĠccK0<NR$_^(y)fsbқW+Ma# q6qGKakּ{㻯?SƐ\#ko~yTP}d}«(]!*7Ԭ{dsyΧƒk%DD85[c#m^]Ϊ 0;,·kac=@00ȧ06a&~&d8\ccV\6X56BT48bEzƇ;cI1lo`	k/apn:0p5w'(pMw!P#ȗ慗 Oz I_6y>冾d367NO͆iC⼡{o8͎/ۍ?WKuaCTfF˂$zoY8h4}$Ąv8\Q|hN331k}i4ػM/r{4M#wd|-%sHk7+XW#pG.KF/뮙2YL@]e7znPs_+5}aĚc"7N[[c"	LH[bAЊ-h(i효]p0A륌2D#<P{K&ڊ7AbmzVK!A#h3 
-bG^ @pBopG[2~Dk(nwJ2wQPDT*/@ۯ?	W²x 4rI1Yhvv\ipgC~6XI$}J8Tɂ?a<@bŃ57X;x?⠽(VX`ԇ~}8}o/Yl=r[TDȖC[|@.tY,\JWct@#nPb,PV{^iXDIYc|",SGCC!VPi	TK1\BUULv&RTՁDIUGГ#U8<_˩`BoSu@-&19` wǂx*.M8uEG©x jΰm)^R\ buM]<:`i
-x?Xo& }sBu\fJ*%MJbI3A^#.4J9~u(pG38Raš`IG!\AkL"2&F._bKgx¨5xʸPEgq39f55+hhDe)8c'\IJeB/h[CWAgeitX'dOdI0&/ĵ2i&
-^סP*1tFՌrYˎh޲؈D+MH!##_Hb@x,Uov:C¥$^h]8@%]8P΅iP`oA.	4FfFHdY0<$/BBCis(75=mXFB"4ٕA]^x
-+47[X,	~"AbyLp>s $:E`ao`F{	g>HnD<̷X`_S-|s9PXSC!MTe' E49ؒXU!CaV$6`PRr,	iI#l	Mg#y,	p=a}w~,vdLZ%	͏8h<p;p:p%s0ãJ,k0sK,cA=K\<2𡨙x<Gޱ:+y&pǕ "2ʸh .3ЌF3;q`f4`$?W	*p{3
-talLh_#;`_K !zI#~Mӣ6WPl~bA|'A4{@хYtUn]Cxm[g%p7@-[p$
-%o'_Z͚#nwI-(k>GDwϻ|[!jaT(|Yp<hvKC}ۻ_~f@[VfV<vOѼp聼p#Y.o w!(ah ޑv#R+KP`#ػ5
-\fUX\~m3}-ZKvp`s4P`wu'j0!ѱ,ڏv9]hh<ȅQ#	hHA	 g`(b0!3>9PXCc2>Դe| x)M|$VPH[cf|x X,T?#襏\G"#&G&	| LhtF8XG&80d?1a]J7*-vWrLZ%G	xIqG<>1,>BQG,>	N4}dGXg`X·x(D:CaROq7# -huHWBNB@+D'9tHob}.Mpϑ@CV"pr<\819N$R㡠~A>Q!"`Hx8` r<$@pK}̀M51	q󺃣>}$Ҵ27HZ?|݈%`l]*B9-
-Em_S9Г-Mee'(2II2I;k$>Ϲ,/Fm$m~fE>'6&{xf4ՆAdG,CЊK3"TcƊUZq(ދ ]x_ Lc:Ϥ{ߝeπ	eV)JuB`UBbd5}`,A1c׉{>+ZZ1~*cXhjbXzN%#?0J/%Jnm64e#|G?cIRd`Y:]rpi=2c"bCi?Bb#O?o< xevntRnT7v$HtxX7LN;qimuټwDj[yFٻKh/7275}ݚx_(W2ĥ6'HrONh	5˙9vg(;iy?nߜSȊoۛȯV}؛fWu[HN	tեa7?_F8US_oى/>FVZnׁ3Ko	
+osxphotos py:module 0 reference.html#module-$ -
+osxphotos.AlbumInfo py:class 1 reference.html#$ -
+osxphotos.AlbumInfo.asdict py:method 1 reference.html#$ -
+osxphotos.AlbumInfo.folder_list py:property 1 reference.html#$ -
+osxphotos.AlbumInfo.folder_names py:property 1 reference.html#$ -
+osxphotos.AlbumInfo.parent py:property 1 reference.html#$ -
+osxphotos.AlbumInfo.photo_index py:method 1 reference.html#$ -
+osxphotos.AlbumInfo.photos py:property 1 reference.html#$ -
+osxphotos.AlbumInfo.sort_order py:property 1 reference.html#$ -
+osxphotos.AlbumInfo.title py:property 1 reference.html#$ -
+osxphotos.AlbumSortOrder py:class 1 reference.html#$ -
+osxphotos.CommentInfo py:class 1 reference.html#$ -
+osxphotos.ExifInfo py:class 1 reference.html#$ -
+osxphotos.ExifTool py:class 1 reference.html#$ -
+osxphotos.ExifTool.addvalues py:method 1 reference.html#$ -
+osxphotos.ExifTool.asdict py:method 1 reference.html#$ -
+osxphotos.ExifTool.json py:method 1 reference.html#$ -
+osxphotos.ExifTool.pid py:property 1 reference.html#$ -
+osxphotos.ExifTool.run_commands py:method 1 reference.html#$ -
+osxphotos.ExifTool.setvalue py:method 1 reference.html#$ -
+osxphotos.ExifTool.version py:property 1 reference.html#$ -
+osxphotos.ExportDB py:class 1 reference.html#$ -
+osxphotos.ExportDB.close py:method 1 reference.html#$ -
+osxphotos.ExportDB.connection py:property 1 reference.html#$ -
+osxphotos.ExportDB.create_file_record py:method 1 reference.html#$ -
+osxphotos.ExportDB.create_or_get_file_record py:method 1 reference.html#$ -
+osxphotos.ExportDB.delete_data_for_filepath py:method 1 reference.html#$ -
+osxphotos.ExportDB.delete_data_for_uuid py:method 1 reference.html#$ -
+osxphotos.ExportDB.export_dir py:property 1 reference.html#$ -
+osxphotos.ExportDB.get_export_results py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_exported_files py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_file_record py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_files_for_uuid py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_photoinfo_for_uuid py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_previous_uuids py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_target_for_file py:method 1 reference.html#$ -
+osxphotos.ExportDB.get_uuid_for_file py:method 1 reference.html#$ -
+osxphotos.ExportDB.path py:property 1 reference.html#$ -
+osxphotos.ExportDB.set_config py:method 1 reference.html#$ -
+osxphotos.ExportDB.set_export_results py:method 1 reference.html#$ -
+osxphotos.ExportDB.set_photoinfo_for_uuid py:method 1 reference.html#$ -
+osxphotos.ExportDBTemp py:class 1 reference.html#$ -
+osxphotos.ExportOptions py:class 1 reference.html#$ -
+osxphotos.ExportOptions.bit_flags py:property 1 reference.html#$ -
+osxphotos.ExportOptions.convert_to_jpeg py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.description_template py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.download_missing py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.dry_run py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.edited py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.exiftool py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.exiftool_flags py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.export_aae py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.export_as_hardlink py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.export_db py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.face_regions py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.favorite_rating py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.fileutil py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.force_update py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.ignore_date_modified py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.ignore_signature py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.increment py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.jpeg_ext py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.jpeg_quality py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.keyword_template py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.live_photo py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.location py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.merge_exif_keywords py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.merge_exif_persons py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.overwrite py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.persons py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.preview py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.preview_suffix py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.raw_photo py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.render_options py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.replace_keywords py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.rich py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.sidecar py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.sidecar_drop_ext py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.strip py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.timeout py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.tmpdir py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.touch_file py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.update py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.update_errors py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.use_albums_as_keywords py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.use_persons_as_keywords py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.use_photokit py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.use_photos_export py:attribute 1 reference.html#$ -
+osxphotos.ExportOptions.verbose py:attribute 1 reference.html#$ -
+osxphotos.ExportResults py:class 1 reference.html#$ -
+osxphotos.ExportResults.all_files py:method 1 reference.html#$ -
+osxphotos.ExportResults.attributes py:property 1 reference.html#$ -
+osxphotos.ExportResults.datetime py:property 1 reference.html#$ -
+osxphotos.FaceInfo py:class 1 reference.html#$ -
+osxphotos.FaceInfo.asdict py:method 1 reference.html#$ -
+osxphotos.FaceInfo.center py:property 1 reference.html#$ -
+osxphotos.FaceInfo.face_rect py:method 1 reference.html#$ -
+osxphotos.FaceInfo.json py:method 1 reference.html#$ -
+osxphotos.FaceInfo.mpri_reg_rect py:property 1 reference.html#$ -
+osxphotos.FaceInfo.mwg_rs_area py:property 1 reference.html#$ -
+osxphotos.FaceInfo.person_info py:property 1 reference.html#$ -
+osxphotos.FaceInfo.photo py:property 1 reference.html#$ -
+osxphotos.FaceInfo.pitch py:property 1 reference.html#$ -
+osxphotos.FaceInfo.roll py:property 1 reference.html#$ -
+osxphotos.FaceInfo.roll_pitch_yaw py:method 1 reference.html#$ -
+osxphotos.FaceInfo.size_pixels py:property 1 reference.html#$ -
+osxphotos.FaceInfo.yaw py:property 1 reference.html#$ -
+osxphotos.FileUtil py:class 1 reference.html#$ -
+osxphotos.FileUtilNoOp py:class 1 reference.html#$ -
+osxphotos.FileUtilNoOp.convert_to_jpeg py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.copy py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.file_sig py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.hardlink py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.rename py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.rmdir py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.tmpdir py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.unlink py:method 1 reference.html#$ -
+osxphotos.FileUtilNoOp.utime py:method 1 reference.html#$ -
+osxphotos.FolderInfo py:class 1 reference.html#$ -
+osxphotos.FolderInfo.album_info py:property 1 reference.html#$ -
+osxphotos.FolderInfo.asdict py:method 1 reference.html#$ -
+osxphotos.FolderInfo.parent py:property 1 reference.html#$ -
+osxphotos.FolderInfo.subfolders py:property 1 reference.html#$ -
+osxphotos.FolderInfo.title py:property 1 reference.html#$ -
+osxphotos.FolderInfo.uuid py:property 1 reference.html#$ -
+osxphotos.ImportInfo py:class 1 reference.html#$ -
+osxphotos.ImportInfo.asdict py:method 1 reference.html#$ -
+osxphotos.ImportInfo.photos py:property 1 reference.html#$ -
+osxphotos.ImportInfo.title py:property 1 reference.html#$ -
+osxphotos.LikeInfo py:class 1 reference.html#$ -
+osxphotos.MomentInfo py:class 1 reference.html#$ -
+osxphotos.MomentInfo.asdict py:method 1 reference.html#$ -
+osxphotos.MomentInfo.date py:property 1 reference.html#$ -
+osxphotos.MomentInfo.end_date py:property 1 reference.html#$ -
+osxphotos.MomentInfo.location py:property 1 reference.html#$ -
+osxphotos.MomentInfo.modification_date py:property 1 reference.html#$ -
+osxphotos.MomentInfo.photos py:property 1 reference.html#$ -
+osxphotos.MomentInfo.pk py:property 1 reference.html#$ -
+osxphotos.MomentInfo.start_date py:property 1 reference.html#$ -
+osxphotos.MomentInfo.subtitle py:property 1 reference.html#$ -
+osxphotos.MomentInfo.title py:property 1 reference.html#$ -
+osxphotos.PersonInfo py:class 1 reference.html#$ -
+osxphotos.PersonInfo.asdict py:method 1 reference.html#$ -
+osxphotos.PersonInfo.face_info py:property 1 reference.html#$ -
+osxphotos.PersonInfo.favorite py:property 1 reference.html#$ -
+osxphotos.PersonInfo.feature_less py:property 1 reference.html#$ -
+osxphotos.PersonInfo.json py:method 1 reference.html#$ -
+osxphotos.PersonInfo.photos py:property 1 reference.html#$ -
+osxphotos.PersonInfo.sort_order py:property 1 reference.html#$ -
+osxphotos.PhotoExporter py:class 1 reference.html#$ -
+osxphotos.PhotoExporter.exiftool_json_sidecar py:method 1 reference.html#$ -
+osxphotos.PhotoExporter.export py:method 1 reference.html#$ -
+osxphotos.PhotoExporter.write_exiftool_metadata_to_file py:method 1 reference.html#$ -
+osxphotos.PhotoInfo py:class 1 reference.html#$ -
+osxphotos.PhotoInfo.adjustments py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.adjustments_path py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.album_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.albums py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.asdict py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.burst py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_album_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_albums py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_default_pick py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_key py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_photos py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.burst_selected py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.cloud_guid py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.cloud_metadata py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.cloud_owner_hashed_id py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.comments py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.date py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.date_added py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.date_modified py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.date_trashed py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.description py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.detected_text py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.duplicates py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.exif_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.exiftool py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.export py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.external_edit py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.face_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.favorite py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.filename py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.fingerprint py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.has_raw py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.hasadjustments py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.hdr py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.height py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.hexdigest py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.hidden py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.import_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.incloud py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.intrash py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.iscloudasset py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.ismissing py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.ismovie py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.isphoto py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.israw py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.isreference py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.json py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.keywords py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.labels py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.labels_normalized py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.likes py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.live_photo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.location py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.moment_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.orientation py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.original_filename py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.original_filesize py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.original_height py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.original_orientation py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.original_width py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.owner py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.panorama py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path_derivatives py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path_edited py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path_edited_live_photo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path_live_photo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.path_raw py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.person_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.persons py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.place py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.portrait py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.project_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.raw_original py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.render_template py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.saved_to_library py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.score py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.screenshot py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.search_info py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.search_info_normalized py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.selfie py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.shared py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.shared_moment py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.slow_mo py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.syndicated py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.tables py:method 1 reference.html#$ -
+osxphotos.PhotoInfo.time_lapse py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.title py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.tzoffset py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.uti py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.uti_edited py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.uti_original py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.uti_raw py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.uuid py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.visible py:property 1 reference.html#$ -
+osxphotos.PhotoInfo.width py:property 1 reference.html#$ -
+osxphotos.PhotoTemplate py:class 1 reference.html#$ -
+osxphotos.PhotoTemplate.expand_variables py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.expand_variables_to_str py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.filter_predicate py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_field_values py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_filter_values py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_format_values py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_media_type py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_photo_bool_attribute py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_photo_video_type py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value_exiftool py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value_filter_function py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value_function py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value_multi py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.get_template_value_pathlib py:method 1 reference.html#$ -
+osxphotos.PhotoTemplate.render py:method 1 reference.html#$ -
+osxphotos.PhotosAlbum py:class 1 reference.html#$ -
+osxphotos.PhotosAlbumPhotoScript py:class 1 reference.html#$ -
+osxphotos.PhotosDB py:class 1 reference.html#$ -
+osxphotos.PhotosDB.album_info py:property 1 reference.html#$ -
+osxphotos.PhotosDB.album_info_shared py:property 1 reference.html#$ -
+osxphotos.PhotosDB.albums py:property 1 reference.html#$ -
+osxphotos.PhotosDB.albums_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.albums_shared py:property 1 reference.html#$ -
+osxphotos.PhotosDB.albums_shared_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.db_path py:property 1 reference.html#$ -
+osxphotos.PhotosDB.db_version py:property 1 reference.html#$ -
+osxphotos.PhotosDB.execute py:method 1 reference.html#$ -
+osxphotos.PhotosDB.folder_info py:property 1 reference.html#$ -
+osxphotos.PhotosDB.folders py:property 1 reference.html#$ -
+osxphotos.PhotosDB.get_db_connection py:method 1 reference.html#$ -
+osxphotos.PhotosDB.get_photo py:method 1 reference.html#$ -
+osxphotos.PhotosDB.import_info py:property 1 reference.html#$ -
+osxphotos.PhotosDB.keywords py:property 1 reference.html#$ -
+osxphotos.PhotosDB.keywords_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.labels py:property 1 reference.html#$ -
+osxphotos.PhotosDB.labels_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.labels_normalized py:property 1 reference.html#$ -
+osxphotos.PhotosDB.labels_normalized_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.library_path py:property 1 reference.html#$ -
+osxphotos.PhotosDB.person_info py:property 1 reference.html#$ -
+osxphotos.PhotosDB.persons py:property 1 reference.html#$ -
+osxphotos.PhotosDB.persons_as_dict py:property 1 reference.html#$ -
+osxphotos.PhotosDB.photos py:method 1 reference.html#$ -
+osxphotos.PhotosDB.photos_by_uuid py:method 1 reference.html#$ -
+osxphotos.PhotosDB.photos_version py:property 1 reference.html#$ -
+osxphotos.PhotosDB.project_info py:property 1 reference.html#$ -
+osxphotos.PhotosDB.query py:method 1 reference.html#$ -
+osxphotos.PlaceInfo py:class 1 reference.html#$ -
+osxphotos.PlaceInfo.address py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.address_str py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.asdict py:method 1 reference.html#$ -
+osxphotos.PlaceInfo.country_code py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.ishome py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.name py:property 1 reference.html#$ -
+osxphotos.PlaceInfo.names py:property 1 reference.html#$ -
+osxphotos.ProjectInfo py:class 1 reference.html#$ -
+osxphotos.ProjectInfo.folder_list py:property 1 reference.html#$ -
+osxphotos.ProjectInfo.folder_names py:property 1 reference.html#$ -
+osxphotos.QueryOptions py:class 1 reference.html#$ -
+osxphotos.QueryOptions.added_after py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.added_before py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.added_in_last py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.album py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.burst py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.burst_photos py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.cloudasset py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.deleted py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.deleted_only py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.description py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.duplicate py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.edited py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.exif py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.external_edit py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.favorite py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.folder py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.from_date py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.function py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.has_comment py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.has_likes py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.has_raw py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.hdr py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.hidden py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.ignore_case py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.in_album py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.incloud py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.is_reference py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.keyword py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.label py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.live py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.location py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.max_size py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.min_size py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.missing py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.missing_bursts py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.movies py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.name py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_comment py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_description py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_keyword py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_likes py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_location py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_place py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.no_title py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_burst py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_cloudasset py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_edited py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_favorite py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_hdr py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_hidden py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_in_album py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_incloud py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_live py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_missing py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_panorama py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_portrait py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_reference py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_saved_to_library py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_screenshot py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_selfie py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_shared py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_shared_moment py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_slow_mo py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_syndicated py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.not_time_lapse py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.panorama py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.person py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.photos py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.place py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.portrait py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.query_eval py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.regex py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.saved_to_library py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.screenshot py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.selected py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.selfie py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.shared py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.shared_moment py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.slow_mo py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.syndicated py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.time_lapse py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.title py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.to_date py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.uti py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.uuid py:attribute 1 reference.html#$ -
+osxphotos.QueryOptions.year py:attribute 1 reference.html#$ -
+osxphotos.ScoreInfo py:class 1 reference.html#$ -
+osxphotos.ScoreInfo.asdict py:method 1 reference.html#$ -
+osxphotos.SearchInfo py:class 1 reference.html#$ -
+osxphotos.SearchInfo.activities py:property 1 reference.html#$ -
+osxphotos.SearchInfo.all py:property 1 reference.html#$ -
+osxphotos.SearchInfo.asdict py:method 1 reference.html#$ -
+osxphotos.SearchInfo.bodies_of_water py:property 1 reference.html#$ -
+osxphotos.SearchInfo.camera py:property 1 reference.html#$ -
+osxphotos.SearchInfo.city py:property 1 reference.html#$ -
+osxphotos.SearchInfo.country py:property 1 reference.html#$ -
+osxphotos.SearchInfo.detected_text py:property 1 reference.html#$ -
+osxphotos.SearchInfo.holidays py:property 1 reference.html#$ -
+osxphotos.SearchInfo.labels py:property 1 reference.html#$ -
+osxphotos.SearchInfo.locality_names py:property 1 reference.html#$ -
+osxphotos.SearchInfo.media_types py:property 1 reference.html#$ -
+osxphotos.SearchInfo.month py:property 1 reference.html#$ -
+osxphotos.SearchInfo.neighborhoods py:property 1 reference.html#$ -
+osxphotos.SearchInfo.place_names py:property 1 reference.html#$ -
+osxphotos.SearchInfo.season py:property 1 reference.html#$ -
+osxphotos.SearchInfo.source py:property 1 reference.html#$ -
+osxphotos.SearchInfo.state py:property 1 reference.html#$ -
+osxphotos.SearchInfo.state_abbreviation py:property 1 reference.html#$ -
+osxphotos.SearchInfo.streets py:property 1 reference.html#$ -
+osxphotos.SearchInfo.text_found py:property 1 reference.html#$ -
+osxphotos.SearchInfo.venue_types py:property 1 reference.html#$ -
+osxphotos.SearchInfo.venues py:property 1 reference.html#$ -
+osxphotos.SearchInfo.year py:property 1 reference.html#$ -
+osxphotos._constants.AlbumSortOrder py:class -1 reference.html#osxphotos.AlbumSortOrder -
+osxphotos.albuminfo.AlbumInfo py:class -1 reference.html#osxphotos.AlbumInfo -
+osxphotos.albuminfo.FolderInfo py:class -1 reference.html#osxphotos.FolderInfo -
+osxphotos.albuminfo.ImportInfo py:class -1 reference.html#osxphotos.ImportInfo -
+osxphotos.albuminfo.ProjectInfo py:class -1 reference.html#osxphotos.ProjectInfo -
+osxphotos.exifinfo.ExifInfo py:class -1 reference.html#osxphotos.ExifInfo -
+osxphotos.exiftool.ExifTool py:class -1 reference.html#osxphotos.ExifTool -
+osxphotos.export_db.ExportDB py:class -1 reference.html#osxphotos.ExportDB -
+osxphotos.export_db.ExportDBTemp py:class -1 reference.html#osxphotos.ExportDBTemp -
+osxphotos.fileutil.FileUtil py:class -1 reference.html#osxphotos.FileUtil -
+osxphotos.fileutil.FileUtilNoOp py:class -1 reference.html#osxphotos.FileUtilNoOp -
+osxphotos.is_debug py:function 1 reference.html#$ -
+osxphotos.momentinfo.MomentInfo py:class -1 reference.html#osxphotos.MomentInfo -
+osxphotos.personinfo.FaceInfo py:class -1 reference.html#osxphotos.FaceInfo -
+osxphotos.personinfo.PersonInfo py:class -1 reference.html#osxphotos.PersonInfo -
+osxphotos.photoexporter.ExportOptions py:class -1 reference.html#osxphotos.ExportOptions -
+osxphotos.photoexporter.ExportResults py:class -1 reference.html#osxphotos.ExportResults -
+osxphotos.photoexporter.PhotoExporter py:class -1 reference.html#osxphotos.PhotoExporter -
+osxphotos.photoinfo.PhotoInfo py:class -1 reference.html#osxphotos.PhotoInfo -
+osxphotos.photosalbum.PhotosAlbum py:class -1 reference.html#osxphotos.PhotosAlbum -
+osxphotos.photosalbum.PhotosAlbumPhotoScript py:class -1 reference.html#osxphotos.PhotosAlbumPhotoScript -
+osxphotos.photosdb._photosdb_process_comments.CommentInfo py:class -1 reference.html#osxphotos.CommentInfo -
+osxphotos.photosdb._photosdb_process_comments.LikeInfo py:class -1 reference.html#osxphotos.LikeInfo -
+osxphotos.photosdb.photosdb.PhotosDB py:class -1 reference.html#osxphotos.PhotosDB -
+osxphotos.phototemplate.PhotoTemplate py:class -1 reference.html#osxphotos.PhotoTemplate -
+osxphotos.placeinfo.PlaceInfo py:class -1 reference.html#osxphotos.PlaceInfo -
+osxphotos.queryoptions.QueryOptions py:class -1 reference.html#osxphotos.QueryOptions -
+osxphotos.scoreinfo.ScoreInfo py:class -1 reference.html#osxphotos.ScoreInfo -
+osxphotos.searchinfo.SearchInfo py:class -1 reference.html#osxphotos.SearchInfo -
+osxphotos.set_debug py:function 1 reference.html#$ -
+cli std:doc -1 cli.html OSXPhotos Command Line Interface (CLI)
+genindex std:label -1 genindex.html Index
+index std:doc -1 index.html Welcome to OSXPhotos’s documentation!
+modindex std:label -1 py-modindex.html Module Index
+osxphotos-add-locations.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-after -
+osxphotos-add-locations.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-before -
+osxphotos-add-locations.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-added-in-last -
+osxphotos-add-locations.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-album -
+osxphotos-add-locations.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-burst -
+osxphotos-add-locations.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-cloudasset -
+osxphotos-add-locations.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-description -
+osxphotos-add-locations.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-dry-run -
+osxphotos-add-locations.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-duplicate -
+osxphotos-add-locations.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-edited -
+osxphotos-add-locations.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-exif -
+osxphotos-add-locations.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-external-edit -
+osxphotos-add-locations.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-favorite -
+osxphotos-add-locations.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-folder -
+osxphotos-add-locations.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-from-date -
+osxphotos-add-locations.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-from-time -
+osxphotos-add-locations.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-comment -
+osxphotos-add-locations.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-likes -
+osxphotos-add-locations.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-has-raw -
+osxphotos-add-locations.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-hdr -
+osxphotos-add-locations.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-hidden -
+osxphotos-add-locations.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-i -
+osxphotos-add-locations.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-in-album -
+osxphotos-add-locations.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-incloud -
+osxphotos-add-locations.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-is-reference -
+osxphotos-add-locations.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-keyword -
+osxphotos-add-locations.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-label -
+osxphotos-add-locations.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-live -
+osxphotos-add-locations.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-location -
+osxphotos-add-locations.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-max-size -
+osxphotos-add-locations.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-min-size -
+osxphotos-add-locations.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-missing -
+osxphotos-add-locations.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-name -
+osxphotos-add-locations.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-comment -
+osxphotos-add-locations.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-description -
+osxphotos-add-locations.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-keyword -
+osxphotos-add-locations.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-likes -
+osxphotos-add-locations.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-location -
+osxphotos-add-locations.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-place -
+osxphotos-add-locations.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-no-title -
+osxphotos-add-locations.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-burst -
+osxphotos-add-locations.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-cloudasset -
+osxphotos-add-locations.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-edited -
+osxphotos-add-locations.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-favorite -
+osxphotos-add-locations.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-hdr -
+osxphotos-add-locations.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-hidden -
+osxphotos-add-locations.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-in-album -
+osxphotos-add-locations.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-incloud -
+osxphotos-add-locations.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-live -
+osxphotos-add-locations.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-missing -
+osxphotos-add-locations.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-panorama -
+osxphotos-add-locations.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-portrait -
+osxphotos-add-locations.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-reference -
+osxphotos-add-locations.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-saved-to-library -
+osxphotos-add-locations.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-screenshot -
+osxphotos-add-locations.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-selfie -
+osxphotos-add-locations.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-shared -
+osxphotos-add-locations.--not-shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-shared-moment -
+osxphotos-add-locations.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-slow-mo -
+osxphotos-add-locations.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-syndicated -
+osxphotos-add-locations.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-not-time-lapse -
+osxphotos-add-locations.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-movies -
+osxphotos-add-locations.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-only-photos -
+osxphotos-add-locations.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-panorama -
+osxphotos-add-locations.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-person -
+osxphotos-add-locations.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-place -
+osxphotos-add-locations.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-portrait -
+osxphotos-add-locations.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-eval -
+osxphotos-add-locations.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-query-function -
+osxphotos-add-locations.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-regex -
+osxphotos-add-locations.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-saved-to-library -
+osxphotos-add-locations.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-screenshot -
+osxphotos-add-locations.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selected -
+osxphotos-add-locations.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-selfie -
+osxphotos-add-locations.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-shared -
+osxphotos-add-locations.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-shared-moment -
+osxphotos-add-locations.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-slow-mo -
+osxphotos-add-locations.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-syndicated -
+osxphotos-add-locations.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-theme -
+osxphotos-add-locations.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-time-lapse -
+osxphotos-add-locations.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-timestamp -
+osxphotos-add-locations.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-title -
+osxphotos-add-locations.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-date -
+osxphotos-add-locations.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-to-time -
+osxphotos-add-locations.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uti -
+osxphotos-add-locations.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uuid -
+osxphotos-add-locations.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-uuid-from-file -
+osxphotos-add-locations.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-V -
+osxphotos-add-locations.--window std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-w -
+osxphotos-add-locations.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-year -
+osxphotos-add-locations.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-V -
+osxphotos-add-locations.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-i -
+osxphotos-add-locations.-w std:cmdoption 1 cli.html#cmdoption-osxphotos-add-locations-w -
+osxphotos-albums.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-library -
+osxphotos-albums.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-json -
+osxphotos-albums.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-library -
+osxphotos-albums.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-albums-arg-PHOTOS_LIBRARY -
+osxphotos-batch-edit.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-library -
+osxphotos-batch-edit.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-description -
+osxphotos-batch-edit.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-dry-run -
+osxphotos-batch-edit.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-keyword -
+osxphotos-batch-edit.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-library -
+osxphotos-batch-edit.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-location -
+osxphotos-batch-edit.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-replace-keywords -
+osxphotos-batch-edit.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-theme -
+osxphotos-batch-edit.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-timestamp -
+osxphotos-batch-edit.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-title -
+osxphotos-batch-edit.--undo std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-undo -
+osxphotos-batch-edit.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-V -
+osxphotos-batch-edit.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-batch-edit-V -
+osxphotos-diff.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-library -
+osxphotos-diff.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-library -
+osxphotos-diff.--raw-output std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-r -
+osxphotos-diff.--style std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-s -
+osxphotos-diff.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-timestamp -
+osxphotos-diff.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-V -
+osxphotos-diff.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-V -
+osxphotos-diff.-r std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-r -
+osxphotos-diff.-s std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-s -
+osxphotos-diff.DB2 std:cmdoption 1 cli.html#cmdoption-osxphotos-diff-arg-DB2 -
+osxphotos-dump.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-library -
+osxphotos-dump.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-deleted -
+osxphotos-dump.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-deleted-only -
+osxphotos-dump.--field std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-f -
+osxphotos-dump.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-json -
+osxphotos-dump.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-library -
+osxphotos-dump.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-print -
+osxphotos-dump.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-f -
+osxphotos-dump.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-dump-arg-PHOTOS_LIBRARY -
+osxphotos-exiftool.--album-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-album-keyword -
+osxphotos-exiftool.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-append -
+osxphotos-exiftool.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-library -
+osxphotos-exiftool.--db-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-db-config -
+osxphotos-exiftool.--description-template std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-description-template -
+osxphotos-exiftool.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-dry-run -
+osxphotos-exiftool.--exiftool-merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-merge-keywords -
+osxphotos-exiftool.--exiftool-merge-persons std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-merge-persons -
+osxphotos-exiftool.--exiftool-option std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-option -
+osxphotos-exiftool.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exiftool-path -
+osxphotos-exiftool.--exportdb std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-exportdb -
+osxphotos-exiftool.--ignore-date-modified std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-ignore-date-modified -
+osxphotos-exiftool.--keyword-template std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-keyword-template -
+osxphotos-exiftool.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-library -
+osxphotos-exiftool.--load-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-load-config -
+osxphotos-exiftool.--person-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-person-keyword -
+osxphotos-exiftool.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-replace-keywords -
+osxphotos-exiftool.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-report -
+osxphotos-exiftool.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-save-config -
+osxphotos-exiftool.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-theme -
+osxphotos-exiftool.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-timestamp -
+osxphotos-exiftool.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-V -
+osxphotos-exiftool.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-V -
+osxphotos-exiftool.EXPORT_DIRECTORY std:cmdoption 1 cli.html#cmdoption-osxphotos-exiftool-arg-EXPORT_DIRECTORY -
+osxphotos-export.--add-exported-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-exported-to-album -
+osxphotos-export.--add-missing-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-missing-to-album -
+osxphotos-export.--add-skipped-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-add-skipped-to-album -
+osxphotos-export.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-after -
+osxphotos-export.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-before -
+osxphotos-export.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-export-added-in-last -
+osxphotos-export.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-album -
+osxphotos-export.--album-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-album-keyword -
+osxphotos-export.--alt-copy std:cmdoption 1 cli.html#cmdoption-osxphotos-export-alt-copy -
+osxphotos-export.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-export-append -
+osxphotos-export.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-export-burst -
+osxphotos-export.--cleanup std:cmdoption 1 cli.html#cmdoption-osxphotos-export-cleanup -
+osxphotos-export.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-export-cloudasset -
+osxphotos-export.--config-only std:cmdoption 1 cli.html#cmdoption-osxphotos-export-config-only -
+osxphotos-export.--convert-to-jpeg std:cmdoption 1 cli.html#cmdoption-osxphotos-export-convert-to-jpeg -
+osxphotos-export.--current-name std:cmdoption 1 cli.html#cmdoption-osxphotos-export-current-name -
+osxphotos-export.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-export-library -
+osxphotos-export.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-export-deleted -
+osxphotos-export.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-export-deleted-only -
+osxphotos-export.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-export-description -
+osxphotos-export.--description-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-description-template -
+osxphotos-export.--directory std:cmdoption 1 cli.html#cmdoption-osxphotos-export-directory -
+osxphotos-export.--download-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-download-missing -
+osxphotos-export.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-export-dry-run -
+osxphotos-export.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-export-duplicate -
+osxphotos-export.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-edited -
+osxphotos-export.--edited-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-edited-suffix -
+osxphotos-export.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exif -
+osxphotos-export.--exiftool std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool -
+osxphotos-export.--exiftool-merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-merge-keywords -
+osxphotos-export.--exiftool-merge-persons std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-merge-persons -
+osxphotos-export.--exiftool-option std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-option -
+osxphotos-export.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exiftool-path -
+osxphotos-export.--export-aae std:cmdoption 1 cli.html#cmdoption-osxphotos-export-export-aae -
+osxphotos-export.--export-as-hardlink std:cmdoption 1 cli.html#cmdoption-osxphotos-export-export-as-hardlink -
+osxphotos-export.--export-by-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-export-by-date -
+osxphotos-export.--exportdb std:cmdoption 1 cli.html#cmdoption-osxphotos-export-exportdb -
+osxphotos-export.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-external-edit -
+osxphotos-export.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-favorite -
+osxphotos-export.--favorite-rating std:cmdoption 1 cli.html#cmdoption-osxphotos-export-favorite-rating -
+osxphotos-export.--filename std:cmdoption 1 cli.html#cmdoption-osxphotos-export-filename -
+osxphotos-export.--finder-tag-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-finder-tag-keywords -
+osxphotos-export.--finder-tag-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-finder-tag-template -
+osxphotos-export.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-export-folder -
+osxphotos-export.--force-update std:cmdoption 1 cli.html#cmdoption-osxphotos-export-force-update -
+osxphotos-export.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-from-date -
+osxphotos-export.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-export-from-time -
+osxphotos-export.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-comment -
+osxphotos-export.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-likes -
+osxphotos-export.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-has-raw -
+osxphotos-export.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-export-hdr -
+osxphotos-export.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-export-hidden -
+osxphotos-export.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-export-i -
+osxphotos-export.--ignore-date-modified std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ignore-date-modified -
+osxphotos-export.--ignore-signature std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ignore-signature -
+osxphotos-export.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-in-album -
+osxphotos-export.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-export-incloud -
+osxphotos-export.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-export-is-reference -
+osxphotos-export.--jpeg-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-jpeg-ext -
+osxphotos-export.--jpeg-quality std:cmdoption 1 cli.html#cmdoption-osxphotos-export-jpeg-quality -
+osxphotos-export.--keep std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keep -
+osxphotos-export.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keyword -
+osxphotos-export.--keyword-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-keyword-template -
+osxphotos-export.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-export-label -
+osxphotos-export.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-library -
+osxphotos-export.--limit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-limit -
+osxphotos-export.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-live -
+osxphotos-export.--load-config std:cmdoption 1 cli.html#cmdoption-osxphotos-export-load-config -
+osxphotos-export.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-export-location -
+osxphotos-export.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-export-max-size -
+osxphotos-export.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-export-min-size -
+osxphotos-export.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-missing -
+osxphotos-export.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-export-name -
+osxphotos-export.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-comment -
+osxphotos-export.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-description -
+osxphotos-export.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-keyword -
+osxphotos-export.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-likes -
+osxphotos-export.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-location -
+osxphotos-export.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-place -
+osxphotos-export.--no-progress std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-progress -
+osxphotos-export.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-export-no-title -
+osxphotos-export.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-burst -
+osxphotos-export.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-cloudasset -
+osxphotos-export.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-edited -
+osxphotos-export.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-favorite -
+osxphotos-export.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-hdr -
+osxphotos-export.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-hidden -
+osxphotos-export.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-in-album -
+osxphotos-export.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-incloud -
+osxphotos-export.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-live -
+osxphotos-export.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-missing -
+osxphotos-export.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-panorama -
+osxphotos-export.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-portrait -
+osxphotos-export.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-reference -
+osxphotos-export.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-saved-to-library -
+osxphotos-export.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-screenshot -
+osxphotos-export.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-selfie -
+osxphotos-export.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-shared -
+osxphotos-export.--not-shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-shared-moment -
+osxphotos-export.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-slow-mo -
+osxphotos-export.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-syndicated -
+osxphotos-export.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-not-time-lapse -
+osxphotos-export.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-movies -
+osxphotos-export.--only-new std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-new -
+osxphotos-export.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-export-only-photos -
+osxphotos-export.--original-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-original-suffix -
+osxphotos-export.--overwrite std:cmdoption 1 cli.html#cmdoption-osxphotos-export-overwrite -
+osxphotos-export.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-export-panorama -
+osxphotos-export.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-export-person -
+osxphotos-export.--person-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-export-person-keyword -
+osxphotos-export.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-export-place -
+osxphotos-export.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-export-portrait -
+osxphotos-export.--post-command std:cmdoption 1 cli.html#cmdoption-osxphotos-export-post-command -
+osxphotos-export.--post-function std:cmdoption 1 cli.html#cmdoption-osxphotos-export-post-function -
+osxphotos-export.--preview std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview -
+osxphotos-export.--preview-if-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview-if-missing -
+osxphotos-export.--preview-suffix std:cmdoption 1 cli.html#cmdoption-osxphotos-export-preview-suffix -
+osxphotos-export.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-export-print -
+osxphotos-export.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-export-query-eval -
+osxphotos-export.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-export-query-function -
+osxphotos-export.--ramdb std:cmdoption 1 cli.html#cmdoption-osxphotos-export-ramdb -
+osxphotos-export.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-export-regex -
+osxphotos-export.--replace-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-export-replace-keywords -
+osxphotos-export.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-export-report -
+osxphotos-export.--retry std:cmdoption 1 cli.html#cmdoption-osxphotos-export-retry -
+osxphotos-export.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-export-save-config -
+osxphotos-export.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-export-saved-to-library -
+osxphotos-export.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-export-screenshot -
+osxphotos-export.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selected -
+osxphotos-export.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-export-selfie -
+osxphotos-export.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared -
+osxphotos-export.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-export-shared-moment -
+osxphotos-export.--sidecar std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar -
+osxphotos-export.--sidecar-drop-ext std:cmdoption 1 cli.html#cmdoption-osxphotos-export-sidecar-drop-ext -
+osxphotos-export.--skip-bursts std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-bursts -
+osxphotos-export.--skip-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-edited -
+osxphotos-export.--skip-live std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-live -
+osxphotos-export.--skip-original-if-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-original-if-edited -
+osxphotos-export.--skip-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-raw -
+osxphotos-export.--skip-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid -
+osxphotos-export.--skip-uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-skip-uuid-from-file -
+osxphotos-export.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-export-slow-mo -
+osxphotos-export.--strip std:cmdoption 1 cli.html#cmdoption-osxphotos-export-strip -
+osxphotos-export.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-export-syndicated -
+osxphotos-export.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-export-theme -
+osxphotos-export.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-export-time-lapse -
+osxphotos-export.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-export-timestamp -
+osxphotos-export.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-export-title -
+osxphotos-export.--tmpdir std:cmdoption 1 cli.html#cmdoption-osxphotos-export-tmpdir -
+osxphotos-export.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-date -
+osxphotos-export.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-export-to-time -
+osxphotos-export.--touch-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-touch-file -
+osxphotos-export.--update std:cmdoption 1 cli.html#cmdoption-osxphotos-export-update -
+osxphotos-export.--update-errors std:cmdoption 1 cli.html#cmdoption-osxphotos-export-update-errors -
+osxphotos-export.--use-photokit std:cmdoption 1 cli.html#cmdoption-osxphotos-export-use-photokit -
+osxphotos-export.--use-photos-export std:cmdoption 1 cli.html#cmdoption-osxphotos-export-use-photos-export -
+osxphotos-export.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uti -
+osxphotos-export.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uuid -
+osxphotos-export.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-export-uuid-from-file -
+osxphotos-export.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-export-V -
+osxphotos-export.--xattr-template std:cmdoption 1 cli.html#cmdoption-osxphotos-export-xattr-template -
+osxphotos-export.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-export-year -
+osxphotos-export.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-export-V -
+osxphotos-export.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-export-i -
+osxphotos-export.DEST std:cmdoption 1 cli.html#cmdoption-osxphotos-export-arg-DEST -
+osxphotos-export.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-export-arg-PHOTOS_LIBRARY -
+osxphotos-exportdb.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-append -
+osxphotos-exportdb.--check-signatures std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-check-signatures -
+osxphotos-exportdb.--delete-file std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-delete-file -
+osxphotos-exportdb.--delete-uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-delete-uuid -
+osxphotos-exportdb.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-dry-run -
+osxphotos-exportdb.--errors std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-errors -
+osxphotos-exportdb.--export-dir std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-export-dir -
+osxphotos-exportdb.--info std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-info -
+osxphotos-exportdb.--last-errors std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-last-errors -
+osxphotos-exportdb.--last-run std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-last-run -
+osxphotos-exportdb.--migrate std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-migrate -
+osxphotos-exportdb.--migrate-photos-library std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-migrate-photos-library -
+osxphotos-exportdb.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-report -
+osxphotos-exportdb.--save-config std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-save-config -
+osxphotos-exportdb.--sql std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-sql -
+osxphotos-exportdb.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-theme -
+osxphotos-exportdb.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-timestamp -
+osxphotos-exportdb.--touch-file std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-touch-file -
+osxphotos-exportdb.--update-signatures std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-update-signatures -
+osxphotos-exportdb.--uuid-files std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-uuid-files -
+osxphotos-exportdb.--uuid-info std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-uuid-info -
+osxphotos-exportdb.--vacuum std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-vacuum -
+osxphotos-exportdb.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-V -
+osxphotos-exportdb.--version std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-version -
+osxphotos-exportdb.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-V -
+osxphotos-exportdb.EXPORT_DATABASE std:cmdoption 1 cli.html#cmdoption-osxphotos-exportdb-arg-EXPORT_DATABASE -
+osxphotos-help.SUBTOPIC std:cmdoption 1 cli.html#cmdoption-osxphotos-help-arg-SUBTOPIC -
+osxphotos-help.TOPIC std:cmdoption 1 cli.html#cmdoption-osxphotos-help-arg-TOPIC -
+osxphotos-import.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-import-a -
+osxphotos-import.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-import-append -
+osxphotos-import.--check-templates std:cmdoption 1 cli.html#cmdoption-osxphotos-import-check-templates -
+osxphotos-import.--clear-location std:cmdoption 1 cli.html#cmdoption-osxphotos-import-L -
+osxphotos-import.--clear-metadata std:cmdoption 1 cli.html#cmdoption-osxphotos-import-C -
+osxphotos-import.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-import-d -
+osxphotos-import.--dup-check std:cmdoption 1 cli.html#cmdoption-osxphotos-import-D -
+osxphotos-import.--exiftool std:cmdoption 1 cli.html#cmdoption-osxphotos-import-e -
+osxphotos-import.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-import-0 -
+osxphotos-import.--glob std:cmdoption 1 cli.html#cmdoption-osxphotos-import-g -
+osxphotos-import.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-import-k -
+osxphotos-import.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-import-l -
+osxphotos-import.--merge-keywords std:cmdoption 1 cli.html#cmdoption-osxphotos-import-m -
+osxphotos-import.--no-progress std:cmdoption 1 cli.html#cmdoption-osxphotos-import-no-progress -
+osxphotos-import.--parse-date std:cmdoption 1 cli.html#cmdoption-osxphotos-import-P -
+osxphotos-import.--post-function std:cmdoption 1 cli.html#cmdoption-osxphotos-import-post-function -
+osxphotos-import.--relative-to std:cmdoption 1 cli.html#cmdoption-osxphotos-import-r -
+osxphotos-import.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-import-report -
+osxphotos-import.--resume std:cmdoption 1 cli.html#cmdoption-osxphotos-import-R -
+osxphotos-import.--split-folder std:cmdoption 1 cli.html#cmdoption-osxphotos-import-f -
+osxphotos-import.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-import-theme -
+osxphotos-import.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-import-timestamp -
+osxphotos-import.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-import-t -
+osxphotos-import.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-import-V -
+osxphotos-import.--walk std:cmdoption 1 cli.html#cmdoption-osxphotos-import-w -
+osxphotos-import.-C std:cmdoption 1 cli.html#cmdoption-osxphotos-import-C -
+osxphotos-import.-D std:cmdoption 1 cli.html#cmdoption-osxphotos-import-D -
+osxphotos-import.-L std:cmdoption 1 cli.html#cmdoption-osxphotos-import-L -
+osxphotos-import.-P std:cmdoption 1 cli.html#cmdoption-osxphotos-import-P -
+osxphotos-import.-R std:cmdoption 1 cli.html#cmdoption-osxphotos-import-R -
+osxphotos-import.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-import-V -
+osxphotos-import.-a std:cmdoption 1 cli.html#cmdoption-osxphotos-import-a -
+osxphotos-import.-d std:cmdoption 1 cli.html#cmdoption-osxphotos-import-d -
+osxphotos-import.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-import-e -
+osxphotos-import.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-import-f -
+osxphotos-import.-g std:cmdoption 1 cli.html#cmdoption-osxphotos-import-g -
+osxphotos-import.-k std:cmdoption 1 cli.html#cmdoption-osxphotos-import-k -
+osxphotos-import.-l std:cmdoption 1 cli.html#cmdoption-osxphotos-import-l -
+osxphotos-import.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-import-m -
+osxphotos-import.-p std:cmdoption 1 cli.html#cmdoption-osxphotos-import-0 -
+osxphotos-import.-r std:cmdoption 1 cli.html#cmdoption-osxphotos-import-r -
+osxphotos-import.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-import-t -
+osxphotos-import.-w std:cmdoption 1 cli.html#cmdoption-osxphotos-import-w -
+osxphotos-import.FILES std:cmdoption 1 cli.html#cmdoption-osxphotos-import-arg-FILES -
+osxphotos-info.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-info-library -
+osxphotos-info.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-info-json -
+osxphotos-info.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-info-library -
+osxphotos-info.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-info-arg-PHOTOS_LIBRARY -
+osxphotos-inspect.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-library -
+osxphotos-inspect.--detect-text std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-t -
+osxphotos-inspect.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-library -
+osxphotos-inspect.--template std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-T -
+osxphotos-inspect.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-theme -
+osxphotos-inspect.-T std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-T -
+osxphotos-inspect.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-inspect-t -
+osxphotos-install.--upgrade std:cmdoption 1 cli.html#cmdoption-osxphotos-install-U -
+osxphotos-install.-U std:cmdoption 1 cli.html#cmdoption-osxphotos-install-U -
+osxphotos-install.PACKAGES std:cmdoption 1 cli.html#cmdoption-osxphotos-install-arg-PACKAGES -
+osxphotos-keywords.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-library -
+osxphotos-keywords.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-json -
+osxphotos-keywords.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-library -
+osxphotos-keywords.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-keywords-arg-PHOTOS_LIBRARY -
+osxphotos-labels.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-library -
+osxphotos-labels.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-json -
+osxphotos-labels.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-library -
+osxphotos-labels.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-labels-arg-PHOTOS_LIBRARY -
+osxphotos-list.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-list-json -
+osxphotos-orphans.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-library -
+osxphotos-orphans.--export std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-export -
+osxphotos-orphans.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-library -
+osxphotos-orphans.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-theme -
+osxphotos-orphans.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-timestamp -
+osxphotos-orphans.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-V -
+osxphotos-orphans.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-orphans-V -
+osxphotos-persons.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-library -
+osxphotos-persons.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-json -
+osxphotos-persons.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-library -
+osxphotos-persons.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-persons-arg-PHOTOS_LIBRARY -
+osxphotos-places.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-places-library -
+osxphotos-places.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-places-json -
+osxphotos-places.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-places-library -
+osxphotos-places.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-places-arg-PHOTOS_LIBRARY -
+osxphotos-query.--add-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-add-to-album -
+osxphotos-query.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-after -
+osxphotos-query.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-before -
+osxphotos-query.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-query-added-in-last -
+osxphotos-query.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-album -
+osxphotos-query.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-query-burst -
+osxphotos-query.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-query-cloudasset -
+osxphotos-query.--count std:cmdoption 1 cli.html#cmdoption-osxphotos-query-count -
+osxphotos-query.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-query-library -
+osxphotos-query.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted -
+osxphotos-query.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-query-deleted-only -
+osxphotos-query.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-query-description -
+osxphotos-query.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-query-duplicate -
+osxphotos-query.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-query-edited -
+osxphotos-query.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-query-exif -
+osxphotos-query.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-query-external-edit -
+osxphotos-query.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-query-favorite -
+osxphotos-query.--field std:cmdoption 1 cli.html#cmdoption-osxphotos-query-f -
+osxphotos-query.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-query-folder -
+osxphotos-query.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-query-from-date -
+osxphotos-query.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-query-from-time -
+osxphotos-query.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-comment -
+osxphotos-query.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-likes -
+osxphotos-query.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-query-has-raw -
+osxphotos-query.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-query-hdr -
+osxphotos-query.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-query-hidden -
+osxphotos-query.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-query-i -
+osxphotos-query.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-in-album -
+osxphotos-query.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-query-incloud -
+osxphotos-query.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-query-is-reference -
+osxphotos-query.--json std:cmdoption 1 cli.html#cmdoption-osxphotos-query-json -
+osxphotos-query.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-query-keyword -
+osxphotos-query.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-query-label -
+osxphotos-query.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-library -
+osxphotos-query.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-query-live -
+osxphotos-query.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-query-location -
+osxphotos-query.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-query-max-size -
+osxphotos-query.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-query-min-size -
+osxphotos-query.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-query-missing -
+osxphotos-query.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-query-name -
+osxphotos-query.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-comment -
+osxphotos-query.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-description -
+osxphotos-query.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-keyword -
+osxphotos-query.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-likes -
+osxphotos-query.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-location -
+osxphotos-query.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-place -
+osxphotos-query.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-query-no-title -
+osxphotos-query.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-burst -
+osxphotos-query.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-cloudasset -
+osxphotos-query.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-edited -
+osxphotos-query.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-favorite -
+osxphotos-query.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-hdr -
+osxphotos-query.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-hidden -
+osxphotos-query.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-in-album -
+osxphotos-query.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-incloud -
+osxphotos-query.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-live -
+osxphotos-query.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-missing -
+osxphotos-query.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-panorama -
+osxphotos-query.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-portrait -
+osxphotos-query.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-reference -
+osxphotos-query.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-saved-to-library -
+osxphotos-query.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-screenshot -
+osxphotos-query.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-selfie -
+osxphotos-query.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-shared -
+osxphotos-query.--not-shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-shared-moment -
+osxphotos-query.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-slow-mo -
+osxphotos-query.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-syndicated -
+osxphotos-query.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-not-time-lapse -
+osxphotos-query.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-movies -
+osxphotos-query.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-query-only-photos -
+osxphotos-query.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-query-panorama -
+osxphotos-query.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-query-person -
+osxphotos-query.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-query-place -
+osxphotos-query.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-query-portrait -
+osxphotos-query.--print std:cmdoption 1 cli.html#cmdoption-osxphotos-query-print -
+osxphotos-query.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-eval -
+osxphotos-query.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-query-query-function -
+osxphotos-query.--quiet std:cmdoption 1 cli.html#cmdoption-osxphotos-query-quiet -
+osxphotos-query.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-query-regex -
+osxphotos-query.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-query-saved-to-library -
+osxphotos-query.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-query-screenshot -
+osxphotos-query.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selected -
+osxphotos-query.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-query-selfie -
+osxphotos-query.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-query-shared -
+osxphotos-query.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-query-shared-moment -
+osxphotos-query.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-query-slow-mo -
+osxphotos-query.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-query-syndicated -
+osxphotos-query.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-query-time-lapse -
+osxphotos-query.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-query-title -
+osxphotos-query.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-date -
+osxphotos-query.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-query-to-time -
+osxphotos-query.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uti -
+osxphotos-query.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid -
+osxphotos-query.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-query-uuid-from-file -
+osxphotos-query.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-query-year -
+osxphotos-query.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-query-f -
+osxphotos-query.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-query-i -
+osxphotos-query.PHOTOS_LIBRARY std:cmdoption 1 cli.html#cmdoption-osxphotos-query-arg-PHOTOS_LIBRARY -
+osxphotos-repl.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-after -
+osxphotos-repl.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-before -
+osxphotos-repl.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-added-in-last -
+osxphotos-repl.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-album -
+osxphotos-repl.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-burst -
+osxphotos-repl.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-cloudasset -
+osxphotos-repl.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-library -
+osxphotos-repl.--deleted std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-deleted -
+osxphotos-repl.--deleted-only std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-deleted-only -
+osxphotos-repl.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-description -
+osxphotos-repl.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-duplicate -
+osxphotos-repl.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-edited -
+osxphotos-repl.--emacs std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-emacs -
+osxphotos-repl.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-exif -
+osxphotos-repl.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-external-edit -
+osxphotos-repl.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-favorite -
+osxphotos-repl.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-folder -
+osxphotos-repl.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-from-date -
+osxphotos-repl.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-from-time -
+osxphotos-repl.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-comment -
+osxphotos-repl.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-likes -
+osxphotos-repl.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-has-raw -
+osxphotos-repl.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-hdr -
+osxphotos-repl.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-hidden -
+osxphotos-repl.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-i -
+osxphotos-repl.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-in-album -
+osxphotos-repl.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-incloud -
+osxphotos-repl.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-is-reference -
+osxphotos-repl.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-keyword -
+osxphotos-repl.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-label -
+osxphotos-repl.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-library -
+osxphotos-repl.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-live -
+osxphotos-repl.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-location -
+osxphotos-repl.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-max-size -
+osxphotos-repl.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-min-size -
+osxphotos-repl.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-missing -
+osxphotos-repl.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-name -
+osxphotos-repl.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-comment -
+osxphotos-repl.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-description -
+osxphotos-repl.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-keyword -
+osxphotos-repl.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-likes -
+osxphotos-repl.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-location -
+osxphotos-repl.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-place -
+osxphotos-repl.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-no-title -
+osxphotos-repl.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-burst -
+osxphotos-repl.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-cloudasset -
+osxphotos-repl.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-edited -
+osxphotos-repl.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-favorite -
+osxphotos-repl.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-hdr -
+osxphotos-repl.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-hidden -
+osxphotos-repl.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-in-album -
+osxphotos-repl.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-incloud -
+osxphotos-repl.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-live -
+osxphotos-repl.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-missing -
+osxphotos-repl.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-panorama -
+osxphotos-repl.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-portrait -
+osxphotos-repl.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-reference -
+osxphotos-repl.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-saved-to-library -
+osxphotos-repl.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-screenshot -
+osxphotos-repl.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-selfie -
+osxphotos-repl.--not-shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-shared -
+osxphotos-repl.--not-shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-shared-moment -
+osxphotos-repl.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-slow-mo -
+osxphotos-repl.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-syndicated -
+osxphotos-repl.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-not-time-lapse -
+osxphotos-repl.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-movies -
+osxphotos-repl.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-only-photos -
+osxphotos-repl.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-panorama -
+osxphotos-repl.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-person -
+osxphotos-repl.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-place -
+osxphotos-repl.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-portrait -
+osxphotos-repl.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-eval -
+osxphotos-repl.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-query-function -
+osxphotos-repl.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-regex -
+osxphotos-repl.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-saved-to-library -
+osxphotos-repl.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-screenshot -
+osxphotos-repl.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selected -
+osxphotos-repl.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-selfie -
+osxphotos-repl.--shared std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-shared -
+osxphotos-repl.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-shared-moment -
+osxphotos-repl.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-slow-mo -
+osxphotos-repl.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-syndicated -
+osxphotos-repl.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-time-lapse -
+osxphotos-repl.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-title -
+osxphotos-repl.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-date -
+osxphotos-repl.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-to-time -
+osxphotos-repl.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uti -
+osxphotos-repl.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid -
+osxphotos-repl.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-uuid-from-file -
+osxphotos-repl.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-year -
+osxphotos-repl.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-repl-i -
+osxphotos-run.--help std:cmdoption 1 cli.html#cmdoption-osxphotos-run-h -
+osxphotos-run.-h std:cmdoption 1 cli.html#cmdoption-osxphotos-run-h -
+osxphotos-run.ARGS std:cmdoption 1 cli.html#cmdoption-osxphotos-run-arg-ARGS -
+osxphotos-run.PYTHON_FILE std:cmdoption 1 cli.html#cmdoption-osxphotos-run-arg-PYTHON_FILE -
+osxphotos-show.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-show-library -
+osxphotos-show.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-show-library -
+osxphotos-show.UUID_OR_NAME std:cmdoption 1 cli.html#cmdoption-osxphotos-show-arg-UUID_OR_NAME -
+osxphotos-snap.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-snap-library -
+osxphotos-snap.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-snap-library -
+osxphotos-sync.--added-after std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-after -
+osxphotos-sync.--added-before std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-before -
+osxphotos-sync.--added-in-last std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-added-in-last -
+osxphotos-sync.--album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-album -
+osxphotos-sync.--append std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-A -
+osxphotos-sync.--burst std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-burst -
+osxphotos-sync.--cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-cloudasset -
+osxphotos-sync.--db std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-library -
+osxphotos-sync.--description std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-description -
+osxphotos-sync.--dry-run std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-dry-run -
+osxphotos-sync.--duplicate std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-duplicate -
+osxphotos-sync.--edited std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-edited -
+osxphotos-sync.--exif std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-exif -
+osxphotos-sync.--export std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-e -
+osxphotos-sync.--external-edit std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-external-edit -
+osxphotos-sync.--favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-favorite -
+osxphotos-sync.--folder std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-folder -
+osxphotos-sync.--from-date std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-from-date -
+osxphotos-sync.--from-time std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-from-time -
+osxphotos-sync.--has-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-comment -
+osxphotos-sync.--has-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-likes -
+osxphotos-sync.--has-raw std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-has-raw -
+osxphotos-sync.--hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-hdr -
+osxphotos-sync.--hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-hidden -
+osxphotos-sync.--ignore-case std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-0 -
+osxphotos-sync.--import std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-i -
+osxphotos-sync.--in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-in-album -
+osxphotos-sync.--incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-incloud -
+osxphotos-sync.--is-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-is-reference -
+osxphotos-sync.--keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-keyword -
+osxphotos-sync.--label std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-label -
+osxphotos-sync.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-library -
+osxphotos-sync.--live std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-live -
+osxphotos-sync.--location std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-location -
+osxphotos-sync.--max-size std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-max-size -
+osxphotos-sync.--merge std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-m -
+osxphotos-sync.--min-size std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-min-size -
+osxphotos-sync.--missing std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-missing -
+osxphotos-sync.--name std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-name -
+osxphotos-sync.--no-comment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-comment -
+osxphotos-sync.--no-description std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-description -
+osxphotos-sync.--no-keyword std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-keyword -
+osxphotos-sync.--no-likes std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-likes -
+osxphotos-sync.--no-location std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-location -
+osxphotos-sync.--no-place std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-place -
+osxphotos-sync.--no-title std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-no-title -
+osxphotos-sync.--not-burst std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-burst -
+osxphotos-sync.--not-cloudasset std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-cloudasset -
+osxphotos-sync.--not-edited std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-edited -
+osxphotos-sync.--not-favorite std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-favorite -
+osxphotos-sync.--not-hdr std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-hdr -
+osxphotos-sync.--not-hidden std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-hidden -
+osxphotos-sync.--not-in-album std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-in-album -
+osxphotos-sync.--not-incloud std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-incloud -
+osxphotos-sync.--not-live std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-live -
+osxphotos-sync.--not-missing std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-missing -
+osxphotos-sync.--not-panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-panorama -
+osxphotos-sync.--not-portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-portrait -
+osxphotos-sync.--not-reference std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-reference -
+osxphotos-sync.--not-saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-saved-to-library -
+osxphotos-sync.--not-screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-screenshot -
+osxphotos-sync.--not-selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-selfie -
+osxphotos-sync.--not-shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-shared-moment -
+osxphotos-sync.--not-slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-slow-mo -
+osxphotos-sync.--not-syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-syndicated -
+osxphotos-sync.--not-time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-not-time-lapse -
+osxphotos-sync.--only-movies std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-movies -
+osxphotos-sync.--only-photos std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-only-photos -
+osxphotos-sync.--panorama std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-panorama -
+osxphotos-sync.--person std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-person -
+osxphotos-sync.--place std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-place -
+osxphotos-sync.--portrait std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-portrait -
+osxphotos-sync.--query-eval std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-eval -
+osxphotos-sync.--query-function std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-query-function -
+osxphotos-sync.--regex std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-regex -
+osxphotos-sync.--report std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-R -
+osxphotos-sync.--saved-to-library std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-saved-to-library -
+osxphotos-sync.--screenshot std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-screenshot -
+osxphotos-sync.--selected std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selected -
+osxphotos-sync.--selfie std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-selfie -
+osxphotos-sync.--set std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-s -
+osxphotos-sync.--shared-moment std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-shared-moment -
+osxphotos-sync.--slow-mo std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-slow-mo -
+osxphotos-sync.--syndicated std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-syndicated -
+osxphotos-sync.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-theme -
+osxphotos-sync.--time-lapse std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-time-lapse -
+osxphotos-sync.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-timestamp -
+osxphotos-sync.--title std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-title -
+osxphotos-sync.--to-date std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-date -
+osxphotos-sync.--to-time std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-to-time -
+osxphotos-sync.--unmatched std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-U -
+osxphotos-sync.--uti std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uti -
+osxphotos-sync.--uuid std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uuid -
+osxphotos-sync.--uuid-from-file std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-uuid-from-file -
+osxphotos-sync.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-V -
+osxphotos-sync.--year std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-year -
+osxphotos-sync.-A std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-A -
+osxphotos-sync.-R std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-R -
+osxphotos-sync.-U std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-U -
+osxphotos-sync.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-V -
+osxphotos-sync.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-e -
+osxphotos-sync.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-i -
+osxphotos-sync.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-m -
+osxphotos-sync.-s std:cmdoption 1 cli.html#cmdoption-osxphotos-sync-s -
+osxphotos-theme.--clone std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-clone -
+osxphotos-theme.--config std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-config -
+osxphotos-theme.--default std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-default -
+osxphotos-theme.--delete std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-delete -
+osxphotos-theme.--edit std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-edit -
+osxphotos-theme.--list std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-list -
+osxphotos-theme.--preview std:cmdoption 1 cli.html#cmdoption-osxphotos-theme-preview -
+osxphotos-timewarp.--add-to-album std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-a -
+osxphotos-timewarp.--compare-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-c -
+osxphotos-timewarp.--date std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-d -
+osxphotos-timewarp.--date-added std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-date-added -
+osxphotos-timewarp.--date-added-from-photo std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-date-added-from-photo -
+osxphotos-timewarp.--date-delta std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-D -
+osxphotos-timewarp.--exiftool-path std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-e -
+osxphotos-timewarp.--force std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-force -
+osxphotos-timewarp.--function std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-F -
+osxphotos-timewarp.--inspect std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-i -
+osxphotos-timewarp.--library std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-L -
+osxphotos-timewarp.--match-time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-0 -
+osxphotos-timewarp.--parse-date std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-M -
+osxphotos-timewarp.--plain std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-plain -
+osxphotos-timewarp.--pull-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-P -
+osxphotos-timewarp.--push-exif std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-p -
+osxphotos-timewarp.--theme std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-theme -
+osxphotos-timewarp.--time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-t -
+osxphotos-timewarp.--time-delta std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-T -
+osxphotos-timewarp.--timestamp std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-timestamp -
+osxphotos-timewarp.--timezone std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-z -
+osxphotos-timewarp.--use-file-time std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-1 -
+osxphotos-timewarp.--verbose std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-V -
+osxphotos-timewarp.-D std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-D -
+osxphotos-timewarp.-F std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-F -
+osxphotos-timewarp.-L std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-L -
+osxphotos-timewarp.-M std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-M -
+osxphotos-timewarp.-P std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-P -
+osxphotos-timewarp.-T std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-T -
+osxphotos-timewarp.-V std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-V -
+osxphotos-timewarp.-a std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-a -
+osxphotos-timewarp.-c std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-c -
+osxphotos-timewarp.-d std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-d -
+osxphotos-timewarp.-e std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-e -
+osxphotos-timewarp.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-1 -
+osxphotos-timewarp.-i std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-i -
+osxphotos-timewarp.-m std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-0 -
+osxphotos-timewarp.-p std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-p -
+osxphotos-timewarp.-t std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-t -
+osxphotos-timewarp.-z std:cmdoption 1 cli.html#cmdoption-osxphotos-timewarp-z -
+osxphotos-tutorial.WIDTH std:cmdoption 1 cli.html#cmdoption-osxphotos-tutorial-arg-WIDTH -
+osxphotos-uninstall.--yes std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
+osxphotos-uninstall.-y std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-y -
+osxphotos-uninstall.PACKAGES std:cmdoption 1 cli.html#cmdoption-osxphotos-uninstall-arg-PACKAGES -
+osxphotos-uuid.--filename std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
+osxphotos-uuid.-f std:cmdoption 1 cli.html#cmdoption-osxphotos-uuid-f -
+osxphotos-version.--run std:cmdoption 1 cli.html#cmdoption-osxphotos-version-run -
+osxphotos.--version std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
+osxphotos.-v std:cmdoption 1 cli.html#cmdoption-osxphotos-v -
+overview std:doc -1 overview.html OSXPhotos
+package_overview std:doc -1 package_overview.html OSXPhotos Python Package Overview
+py-modindex std:label -1 py-modindex.html Python Module Index
+reference std:doc -1 reference.html OSXPhotos Python Reference
+search std:label -1 search.html Search Page
+template_help std:doc -1 template_help.html OSXPhotos Template System
+tutorial std:doc -1 tutorial.html OSXPhotos Tutorial
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
-        <title>OSXPhotos - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
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
-        <title>OSXPhotos Python Package Overview - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos Python Package Overview - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
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
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.8 documentation</title>
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Python Module Index - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
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
-        <title>OSXPhotos Python Reference - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos Python Reference - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
 </a><form class="sidebar-search-container" method="get" action="search.html" role="search">
   <input class="sidebar-search" placeholder=Search name="q" aria-label="Search">
   <input type="hidden" name="check_keywords" value="yes">
   <input type="hidden" name="area" value="default">
 </form>
 <div id="searchbox"></div><div class="sidebar-scroll"><div class="sidebar-tree">
@@ -2234,14 +2234,20 @@
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.shared">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">shared</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.shared" title="Permalink to this definition">#</a></dt>
 <dd><p>returns True if photos is in a shared iCloud album otherwise false
 Only valid on Photos 5; returns None on older versions</p>
 </dd></dl>
 
 <dl class="py property">
+<dt class="sig sig-object py" id="osxphotos.PhotoInfo.shared_moment">
+<em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">shared_moment</span></span><em class="property"><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="pre">bool</span></em><a class="headerlink" href="#osxphotos.PhotoInfo.shared_moment" title="Permalink to this definition">#</a></dt>
+<dd><p>Returns True if photo is part of a shared moment otherwise False</p>
+</dd></dl>
+
+<dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.slow_mo">
 <em class="property"><span class="pre">property</span><span class="w"> </span></em><span class="sig-name descname"><span class="pre">slow_mo</span></span><a class="headerlink" href="#osxphotos.PhotoInfo.slow_mo" title="Permalink to this definition">#</a></dt>
 <dd><p>Returns True if photo is a slow motion video, otherwise False</p>
 </dd></dl>
 
 <dl class="py property">
 <dt class="sig sig-object py" id="osxphotos.PhotoInfo.syndicated">
@@ -2884,15 +2890,15 @@
 or empty list if album is not in any folders</p>
 </dd></dl>
 
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.QueryOptions">
-<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">QueryOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">added_after</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_before</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_in_last</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst_photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duplicate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">external_edit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">function</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">callable</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_case</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">max_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">min_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_bursts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">movies</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">person</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">query_eval</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">regex</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selected</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uti</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/queryoptions.html#QueryOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.QueryOptions" title="Permalink to this definition">#</a></dt>
+<em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">QueryOptions</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">added_after</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_before</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">added_in_last</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">timedelta</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst_photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted_only</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">deleted</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">duplicate</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exif</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">external_edit</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">folder</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">from_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">function</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">List</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">callable</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">has_raw</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ignore_case</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">is_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">label</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">max_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">min_size</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Byte</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing_bursts</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">movies</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">name</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_comment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_description</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_likes</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_location</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_keyword</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">no_title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_burst</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_cloudasset</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_edited</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_favorite</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hdr</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_hidden</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_in_album</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_incloud</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_live</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_missing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_reference</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">panorama</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">person</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">photos</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">place</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">portrait</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">query_eval</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">regex</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">Tuple</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">,</span></span><span class="w"> </span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">screenshot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selected</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">selfie</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">slow_mo</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time_lapse</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">title</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_date</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">datetime</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">to_time</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">time</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uti</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">uuid</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">str</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">year</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">Iterable</span><span class="p"><span class="pre">[</span></span><span class="pre">int</span><span class="p"><span class="pre">]</span></span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_syndicated</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_saved_to_library</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">shared_moment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">not_shared_moment</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">Optional</span><span class="p"><span class="pre">[</span></span><span class="pre">bool</span><span class="p"><span class="pre">]</span></span></span><span class="w"> </span><span class="o"><span class="pre">=</span></span><span class="w"> </span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/queryoptions.html#QueryOptions"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.QueryOptions" title="Permalink to this definition">#</a></dt>
 <dd><p>QueryOptions class for PhotosDB.query</p>
 <dl class="py attribute">
 <dt class="sig sig-object py" id="osxphotos.QueryOptions.added_after">
 <span class="sig-name descname"><span class="pre">added_after</span></span><a class="headerlink" href="#osxphotos.QueryOptions.added_after" title="Permalink to this definition">#</a></dt>
 <dd><p>search for photos added after a given date</p>
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
@@ -3810,14 +3816,36 @@
 <dl class="field-list simple">
 <dt class="field-odd">Type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>Optional[bool]</p>
 </dd>
 </dl>
 </dd></dl>
 
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.shared_moment">
+<span class="sig-name descname"><span class="pre">shared_moment</span></span><a class="headerlink" href="#osxphotos.QueryOptions.shared_moment" title="Permalink to this definition">#</a></dt>
+<dd><p>search for photos that have been shared via a shared moment</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py attribute">
+<dt class="sig sig-object py" id="osxphotos.QueryOptions.not_shared_moment">
+<span class="sig-name descname"><span class="pre">not_shared_moment</span></span><a class="headerlink" href="#osxphotos.QueryOptions.not_shared_moment" title="Permalink to this definition">#</a></dt>
+<dd><p>search for photos that have not been shared via a shared moment</p>
+<dl class="field-list simple">
+<dt class="field-odd">Type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>Optional[bool]</p>
+</dd>
+</dl>
+</dd></dl>
+
 </dd></dl>
 
 <dl class="py class">
 <dt class="sig sig-object py" id="osxphotos.ScoreInfo">
 <em class="property"><span class="pre">class</span><span class="w"> </span></em><span class="sig-prename descclassname"><span class="pre">osxphotos.</span></span><span class="sig-name descname"><span class="pre">ScoreInfo</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">overall</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">curation</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">promotion</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">highlight_visibility</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">behavioral</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">failure</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">harmonious_color</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">immersiveness</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">interaction</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">interesting_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">intrusive_object_presence</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">lively_color</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">low_light</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">noise</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_camera_tilt</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_composition</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_lighting</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_pattern</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_perspective</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_post_processing</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_reflection</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pleasant_symmetry</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">sharply_focused_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">tastefully_blurred</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_chosen_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_framed_subject</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">well_timed_shot</span></span><span class="p"><span class="pre">:</span></span><span class="w"> </span><span class="n"><span class="pre">float</span></span></em><span class="sig-paren">)</span><a class="reference internal" href="_modules/osxphotos/scoreinfo.html#ScoreInfo"><span class="viewcode-link"><span class="pre">[source]</span></span></a><a class="headerlink" href="#osxphotos.ScoreInfo" title="Permalink to this definition">#</a></dt>
 <dd><p>Computed photo score info associated with a photo from the Photos library</p>
 <dl class="py method">
@@ -4297,14 +4325,15 @@
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.saved_to_library"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.saved_to_library</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.score"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.score</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.screenshot"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.screenshot</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.search_info_normalized"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.search_info_normalized</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.selfie"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.selfie</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.shared"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.PhotoInfo.shared_moment"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.shared_moment</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.slow_mo"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.slow_mo</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.syndicated"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.syndicated</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.tables"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tables()</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.time_lapse"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.time_lapse</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.title"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.title</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.tzoffset"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.tzoffset</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.PhotoInfo.uti"><code class="docutils literal notranslate"><span class="pre">PhotoInfo.uti</span></code></a></li>
@@ -4465,14 +4494,16 @@
 <li><a class="reference internal" href="#osxphotos.QueryOptions.uti"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uti</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.uuid"><code class="docutils literal notranslate"><span class="pre">QueryOptions.uuid</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.year"><code class="docutils literal notranslate"><span class="pre">QueryOptions.year</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.syndicated</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.not_syndicated"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_syndicated</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.saved_to_library</span></code></a></li>
 <li><a class="reference internal" href="#osxphotos.QueryOptions.not_saved_to_library"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_saved_to_library</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.shared_moment"><code class="docutils literal notranslate"><span class="pre">QueryOptions.shared_moment</span></code></a></li>
+<li><a class="reference internal" href="#osxphotos.QueryOptions.not_shared_moment"><code class="docutils literal notranslate"><span class="pre">QueryOptions.not_shared_moment</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.ScoreInfo"><code class="docutils literal notranslate"><span class="pre">ScoreInfo</span></code></a><ul>
 <li><a class="reference internal" href="#osxphotos.ScoreInfo.asdict"><code class="docutils literal notranslate"><span class="pre">ScoreInfo.asdict()</span></code></a></li>
 </ul>
 </li>
 <li><a class="reference internal" href="#osxphotos.SearchInfo"><code class="docutils literal notranslate"><span class="pre">SearchInfo</span></code></a><ul>
```

##### html2text {}

```diff
@@ -13,21 +13,21 @@
 
            ⁰ ⁰
 Hide navigation sidebar
 
 Hide table of contents sidebar
 Toggle site navigation sidebar
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
@@ -1052,14 +1052,16 @@
             results only valid on Photos 5, on older libraries, returns None
         propertyselfie#
             Returns True if photo is a selfie (front facing camera), otherwise
             False
         propertyshared#
             returns True if photos is in a shared iCloud album otherwise false
             Only valid on Photos 5; returns None on older versions
+        propertyshared_moment: bool#
+            Returns True if photo is part of a shared moment otherwise False
         propertyslow_mo#
             Returns True if photo is a slow motion video, otherwise False
         propertysyndicated: bool | None#
             Return true if photo was shared via syndication (e.g. via Messages,
             etc.); these are photos that appear in âShared with youâ album.
             Photos 8+ only; returns None if not Photos 8+.
         tables() &#x2192; PhotoTables[source]#
@@ -1441,15 +1443,16 @@
   = None, selected: Optional[bool] = None, selfie: Optional[bool] = None,
   shared: Optional[bool] = None, slow_mo: Optional[bool] = None, time_lapse:
   Optional[bool] = None, title: Optional[Iterable[str]] = None, to_date:
   Optional[datetime] = None, to_time: Optional[time] = None, uti: Optional
   [Iterable[str]] = None, uuid: Optional[Iterable[str]] = None, year: Optional
   [Iterable[int]] = None, syndicated: Optional[bool] = None, not_syndicated:
   Optional[bool] = None, saved_to_library: Optional[bool] = None,
-  not_saved_to_library: Optional[bool] = None)[source]#
+  not_saved_to_library: Optional[bool] = None, shared_moment: Optional[bool] =
+  None, not_shared_moment: Optional[bool] = None)[source]#
       QueryOptions class for PhotosDB.query
         added_after#
             search for photos added after a given date
               Type:
                   Optional[datetime.datetime]
         added_before#
             search for photos added before a given date
@@ -1785,14 +1788,22 @@
               Type:
                   Optional[bool]
         not_saved_to_library#
             search for syndicated photos that have not been saved to the Photos
             library
               Type:
                   Optional[bool]
+        shared_moment#
+            search for photos that have been shared via a shared moment
+              Type:
+                  Optional[bool]
+        not_shared_moment#
+            search for photos that have not been shared via a shared moment
+              Type:
+                  Optional[bool]
   classosxphotos.ScoreInfo(overall: float, curation: float, promotion: float,
   highlight_visibility: float, behavioral: float, failure: float,
   harmonious_color: float, immersiveness: float, interaction: float,
   interesting_subject: float, intrusive_object_presence: float, lively_color:
   float, low_light: float, noise: float, pleasant_camera_tilt: float,
   pleasant_composition: float, pleasant_lighting: float, pleasant_pattern:
   float, pleasant_perspective: float, pleasant_post_processing: float,
@@ -2098,14 +2109,15 @@
                 # PhotoInfo.saved_to_library
                 # PhotoInfo.score
                 # PhotoInfo.screenshot
                 # PhotoInfo.search_info
                 # PhotoInfo.search_info_normalized
                 # PhotoInfo.selfie
                 # PhotoInfo.shared
+                # PhotoInfo.shared_moment
                 # PhotoInfo.slow_mo
                 # PhotoInfo.syndicated
                 # PhotoInfo.tables()
                 # PhotoInfo.time_lapse
                 # PhotoInfo.title
                 # PhotoInfo.tzoffset
                 # PhotoInfo.uti
@@ -2256,14 +2268,16 @@
                 # QueryOptions.uti
                 # QueryOptions.uuid
                 # QueryOptions.year
                 # QueryOptions.syndicated
                 # QueryOptions.not_syndicated
                 # QueryOptions.saved_to_library
                 # QueryOptions.not_saved_to_library
+                # QueryOptions.shared_moment
+                # QueryOptions.not_shared_moment
           o ScoreInfo
                 # ScoreInfo.asdict()
           o SearchInfo
                 # SearchInfo.activities
                 # SearchInfo.all
                 # SearchInfo.asdict()
                 # SearchInfo.bodies_of_water
```

#### docs/search.html

```diff
@@ -1,14 +1,14 @@
 <!doctype html>
 <html class="no-js" lang="en">
   <head><meta charset="utf-8"/>
     <meta name="viewport" content="width=device-width,initial-scale=1"/>
     <meta name="color-scheme" content="light dark"><link rel="index" title="Index" href="genindex.html" /><link rel="search" title="Search" href="#" />
 
-    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.8 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
+    <meta name="generator" content="sphinx-5.3.0, furo 2022.09.29"/><title>Search - osxphotos 0.60.9 documentation</title><link rel="stylesheet" type="text/css" href="_static/pygments.css" />
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
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
-        "8": [2, 4, 5],
+        "8": [2, 4],
         "recommend": [0, 2, 6],
         "wai": [2, 6],
         "pipx": [2, 3],
         "easiest": 2,
         "applic": [2, 6],
         "accord": 2,
         "instruct": [2, 6],
@@ -1139,15 +1139,15 @@
         "32": 3,
         "29": 3,
         "47": 3,
         "lock": 3,
         "6000": 3,
         "session": [3, 4, 5],
         "aesthet": [3, 5],
-        "moment": [3, 4, 5],
+        "moment": [0, 3, 4, 5],
         "took": [0, 3],
         "18": 3,
         "54": 3,
         "31581": 3,
         "77": 3,
         "instanc": [3, 4, 6],
         "len": [3, 5],
@@ -1746,15 +1746,15 @@
         "matter": 6,
         "subset": [0, 4, 6],
         "certainli": 6,
         "insid": 6,
         "2018": 6,
         "28": 6,
         "worst": 6,
-        "9": 6,
+        "9": [5, 6],
         "describ": [0, 6],
         "section": 6,
         "varieti": 6,
         "titlen": 6,
         "ndescript": 6,
         "advanc": 6,
         "explan": 6,
@@ -2268,15 +2268,17 @@
         "drawn": 4,
         "coreloc": 4,
         "aae": [0, 4],
         "succesfulli": 0,
         "04d": 0,
         "export_aa": [1, 4],
         "adjustments_path": [1, 4],
-        "aae_written": 4
+        "aae_written": 4,
+        "shared_mo": [1, 4],
+        "not_shared_mo": [1, 4]
     },
     "objects": {
         "": [
             [4, 0, 0, "-", "osxphotos"]
         ],
         "osxphotos": [
             [4, 1, 1, "", "AlbumInfo"],
@@ -2549,14 +2551,15 @@
             [4, 3, 1, "", "saved_to_library"],
             [4, 3, 1, "", "score"],
             [4, 3, 1, "", "screenshot"],
             [4, 3, 1, "", "search_info"],
             [4, 3, 1, "", "search_info_normalized"],
             [4, 3, 1, "", "selfie"],
             [4, 3, 1, "", "shared"],
+            [4, 3, 1, "", "shared_moment"],
             [4, 3, 1, "", "slow_mo"],
             [4, 3, 1, "", "syndicated"],
             [4, 2, 1, "", "tables"],
             [4, 3, 1, "", "time_lapse"],
             [4, 3, 1, "", "title"],
             [4, 3, 1, "", "tzoffset"],
             [4, 3, 1, "", "uti"],
@@ -2687,14 +2690,15 @@
             [4, 4, 1, "", "not_panorama"],
             [4, 4, 1, "", "not_portrait"],
             [4, 4, 1, "", "not_reference"],
             [4, 4, 1, "", "not_saved_to_library"],
             [4, 4, 1, "", "not_screenshot"],
             [4, 4, 1, "", "not_selfie"],
             [4, 4, 1, "", "not_shared"],
+            [4, 4, 1, "", "not_shared_moment"],
             [4, 4, 1, "", "not_slow_mo"],
             [4, 4, 1, "", "not_syndicated"],
             [4, 4, 1, "", "not_time_lapse"],
             [4, 4, 1, "", "panorama"],
             [4, 4, 1, "", "person"],
             [4, 4, 1, "", "photos"],
             [4, 4, 1, "", "place"],
@@ -2702,14 +2706,15 @@
             [4, 4, 1, "", "query_eval"],
             [4, 4, 1, "", "regex"],
             [4, 4, 1, "", "saved_to_library"],
             [4, 4, 1, "", "screenshot"],
             [4, 4, 1, "", "selected"],
             [4, 4, 1, "", "selfie"],
             [4, 4, 1, "", "shared"],
+            [4, 4, 1, "", "shared_moment"],
             [4, 4, 1, "", "slow_mo"],
             [4, 4, 1, "", "syndicated"],
             [4, 4, 1, "", "time_lapse"],
             [4, 4, 1, "", "title"],
             [4, 4, 1, "", "to_date"],
             [4, 4, 1, "", "uti"],
             [4, 4, 1, "", "uuid"],
@@ -2798,14 +2803,15 @@
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-reference", "--not-reference"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-shared", "--not-shared"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-not-shared-moment", "--not-shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-slow-mo", "--not-slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-person", "--person"],
@@ -2815,14 +2821,15 @@
             [0, 6, 1, "cmdoption-osxphotos-add-locations-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-shared", "--shared"],
+            [0, 6, 1, "cmdoption-osxphotos-add-locations-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-slow-mo", "--slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-theme", "--theme"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-timestamp", "--timestamp"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-add-locations-to-date", "--to-date"],
@@ -3002,14 +3009,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-reference", "--not-reference"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-shared", "--not-shared"],
+            [0, 6, 1, "cmdoption-osxphotos-export-not-shared-moment", "--not-shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-slow-mo", "--not-slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-export-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-new", "--only-new"],
             [0, 6, 1, "cmdoption-osxphotos-export-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-export-original-suffix", "--original-suffix"],
@@ -3034,14 +3042,15 @@
             [0, 6, 1, "cmdoption-osxphotos-export-retry", "--retry"],
             [0, 6, 1, "cmdoption-osxphotos-export-save-config", "--save-config"],
             [0, 6, 1, "cmdoption-osxphotos-export-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-export-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-export-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-export-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-export-shared", "--shared"],
+            [0, 6, 1, "cmdoption-osxphotos-export-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar", "--sidecar"],
             [0, 6, 1, "cmdoption-osxphotos-export-sidecar-drop-ext", "--sidecar-drop-ext"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-bursts", "--skip-bursts"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-edited", "--skip-edited"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-live", "--skip-live"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-original-if-edited", "--skip-original-if-edited"],
             [0, 6, 1, "cmdoption-osxphotos-export-skip-raw", "--skip-raw"],
@@ -3268,14 +3277,15 @@
             [0, 6, 1, "cmdoption-osxphotos-query-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-reference", "--not-reference"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-shared", "--not-shared"],
+            [0, 6, 1, "cmdoption-osxphotos-query-not-shared-moment", "--not-shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-slow-mo", "--not-slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-query-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-query-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-query-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-query-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-query-person", "--person"],
@@ -3287,14 +3297,15 @@
             [0, 6, 1, "cmdoption-osxphotos-query-quiet", "--quiet"],
             [0, 6, 1, "cmdoption-osxphotos-query-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-query-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-query-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-query-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-query-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-query-shared", "--shared"],
+            [0, 6, 1, "cmdoption-osxphotos-query-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-query-slow-mo", "--slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-query-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-query-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-query-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-query-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-query-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-query-uti", "--uti"],
@@ -3363,14 +3374,15 @@
             [0, 6, 1, "cmdoption-osxphotos-repl-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-reference", "--not-reference"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-selfie", "--not-selfie"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-shared", "--not-shared"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-not-shared-moment", "--not-shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-slow-mo", "--not-slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-repl-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-repl-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-repl-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-repl-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-repl-person", "--person"],
@@ -3380,14 +3392,15 @@
             [0, 6, 1, "cmdoption-osxphotos-repl-query-function", "--query-function"],
             [0, 6, 1, "cmdoption-osxphotos-repl-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-repl-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-repl-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-repl-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-repl-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-repl-shared", "--shared"],
+            [0, 6, 1, "cmdoption-osxphotos-repl-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-repl-slow-mo", "--slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-repl-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-repl-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-repl-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-repl-to-date", "--to-date"],
             [0, 6, 1, "cmdoption-osxphotos-repl-to-time", "--to-time"],
             [0, 6, 1, "cmdoption-osxphotos-repl-uti", "--uti"],
@@ -3470,14 +3483,15 @@
             [0, 6, 1, "cmdoption-osxphotos-sync-not-missing", "--not-missing"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-panorama", "--not-panorama"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-portrait", "--not-portrait"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-reference", "--not-reference"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-saved-to-library", "--not-saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-screenshot", "--not-screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-selfie", "--not-selfie"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-not-shared-moment", "--not-shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-slow-mo", "--not-slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-syndicated", "--not-syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-sync-not-time-lapse", "--not-time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-sync-only-movies", "--only-movies"],
             [0, 6, 1, "cmdoption-osxphotos-sync-only-photos", "--only-photos"],
             [0, 6, 1, "cmdoption-osxphotos-sync-panorama", "--panorama"],
             [0, 6, 1, "cmdoption-osxphotos-sync-person", "--person"],
@@ -3488,14 +3502,15 @@
             [0, 6, 1, "cmdoption-osxphotos-sync-regex", "--regex"],
             [0, 6, 1, "cmdoption-osxphotos-sync-R", "--report"],
             [0, 6, 1, "cmdoption-osxphotos-sync-saved-to-library", "--saved-to-library"],
             [0, 6, 1, "cmdoption-osxphotos-sync-screenshot", "--screenshot"],
             [0, 6, 1, "cmdoption-osxphotos-sync-selected", "--selected"],
             [0, 6, 1, "cmdoption-osxphotos-sync-selfie", "--selfie"],
             [0, 6, 1, "cmdoption-osxphotos-sync-s", "--set"],
+            [0, 6, 1, "cmdoption-osxphotos-sync-shared-moment", "--shared-moment"],
             [0, 6, 1, "cmdoption-osxphotos-sync-slow-mo", "--slow-mo"],
             [0, 6, 1, "cmdoption-osxphotos-sync-syndicated", "--syndicated"],
             [0, 6, 1, "cmdoption-osxphotos-sync-theme", "--theme"],
             [0, 6, 1, "cmdoption-osxphotos-sync-time-lapse", "--time-lapse"],
             [0, 6, 1, "cmdoption-osxphotos-sync-timestamp", "--timestamp"],
             [0, 6, 1, "cmdoption-osxphotos-sync-title", "--title"],
             [0, 6, 1, "cmdoption-osxphotos-sync-to-date", "--to-date"],
@@ -4880,14 +4895,21 @@
         ],
         "--not-shared": [
             [0, "cmdoption-osxphotos-add-locations-not-shared"],
             [0, "cmdoption-osxphotos-export-not-shared"],
             [0, "cmdoption-osxphotos-query-not-shared"],
             [0, "cmdoption-osxphotos-repl-not-shared"]
         ],
+        "--not-shared-moment": [
+            [0, "cmdoption-osxphotos-add-locations-not-shared-moment"],
+            [0, "cmdoption-osxphotos-export-not-shared-moment"],
+            [0, "cmdoption-osxphotos-query-not-shared-moment"],
+            [0, "cmdoption-osxphotos-repl-not-shared-moment"],
+            [0, "cmdoption-osxphotos-sync-not-shared-moment"]
+        ],
         "--not-slow-mo": [
             [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
             [0, "cmdoption-osxphotos-export-not-slow-mo"],
             [0, "cmdoption-osxphotos-query-not-slow-mo"],
             [0, "cmdoption-osxphotos-repl-not-slow-mo"],
             [0, "cmdoption-osxphotos-sync-not-slow-mo"]
         ],
@@ -5087,14 +5109,21 @@
         ],
         "--shared": [
             [0, "cmdoption-osxphotos-add-locations-shared"],
             [0, "cmdoption-osxphotos-export-shared"],
             [0, "cmdoption-osxphotos-query-shared"],
             [0, "cmdoption-osxphotos-repl-shared"]
         ],
+        "--shared-moment": [
+            [0, "cmdoption-osxphotos-add-locations-shared-moment"],
+            [0, "cmdoption-osxphotos-export-shared-moment"],
+            [0, "cmdoption-osxphotos-query-shared-moment"],
+            [0, "cmdoption-osxphotos-repl-shared-moment"],
+            [0, "cmdoption-osxphotos-sync-shared-moment"]
+        ],
         "--sidecar": [
             [0, "cmdoption-osxphotos-export-sidecar"]
         ],
         "--sidecar-drop-ext": [
             [0, "cmdoption-osxphotos-export-sidecar-drop-ext"]
         ],
         "--skip-bursts": [
@@ -5523,14 +5552,15 @@
             [0, "cmdoption-osxphotos-add-locations-not-panorama"],
             [0, "cmdoption-osxphotos-add-locations-not-portrait"],
             [0, "cmdoption-osxphotos-add-locations-not-reference"],
             [0, "cmdoption-osxphotos-add-locations-not-saved-to-library"],
             [0, "cmdoption-osxphotos-add-locations-not-screenshot"],
             [0, "cmdoption-osxphotos-add-locations-not-selfie"],
             [0, "cmdoption-osxphotos-add-locations-not-shared"],
+            [0, "cmdoption-osxphotos-add-locations-not-shared-moment"],
             [0, "cmdoption-osxphotos-add-locations-not-slow-mo"],
             [0, "cmdoption-osxphotos-add-locations-not-syndicated"],
             [0, "cmdoption-osxphotos-add-locations-not-time-lapse"],
             [0, "cmdoption-osxphotos-add-locations-only-movies"],
             [0, "cmdoption-osxphotos-add-locations-only-photos"],
             [0, "cmdoption-osxphotos-add-locations-panorama"],
             [0, "cmdoption-osxphotos-add-locations-person"],
@@ -5540,14 +5570,15 @@
             [0, "cmdoption-osxphotos-add-locations-query-function"],
             [0, "cmdoption-osxphotos-add-locations-regex"],
             [0, "cmdoption-osxphotos-add-locations-saved-to-library"],
             [0, "cmdoption-osxphotos-add-locations-screenshot"],
             [0, "cmdoption-osxphotos-add-locations-selected"],
             [0, "cmdoption-osxphotos-add-locations-selfie"],
             [0, "cmdoption-osxphotos-add-locations-shared"],
+            [0, "cmdoption-osxphotos-add-locations-shared-moment"],
             [0, "cmdoption-osxphotos-add-locations-slow-mo"],
             [0, "cmdoption-osxphotos-add-locations-syndicated"],
             [0, "cmdoption-osxphotos-add-locations-theme"],
             [0, "cmdoption-osxphotos-add-locations-time-lapse"],
             [0, "cmdoption-osxphotos-add-locations-timestamp"],
             [0, "cmdoption-osxphotos-add-locations-title"],
             [0, "cmdoption-osxphotos-add-locations-to-date"],
@@ -5714,14 +5745,15 @@
             [0, "cmdoption-osxphotos-export-not-panorama"],
             [0, "cmdoption-osxphotos-export-not-portrait"],
             [0, "cmdoption-osxphotos-export-not-reference"],
             [0, "cmdoption-osxphotos-export-not-saved-to-library"],
             [0, "cmdoption-osxphotos-export-not-screenshot"],
             [0, "cmdoption-osxphotos-export-not-selfie"],
             [0, "cmdoption-osxphotos-export-not-shared"],
+            [0, "cmdoption-osxphotos-export-not-shared-moment"],
             [0, "cmdoption-osxphotos-export-not-slow-mo"],
             [0, "cmdoption-osxphotos-export-not-syndicated"],
             [0, "cmdoption-osxphotos-export-not-time-lapse"],
             [0, "cmdoption-osxphotos-export-only-movies"],
             [0, "cmdoption-osxphotos-export-only-new"],
             [0, "cmdoption-osxphotos-export-only-photos"],
             [0, "cmdoption-osxphotos-export-original-suffix"],
@@ -5746,14 +5778,15 @@
             [0, "cmdoption-osxphotos-export-retry"],
             [0, "cmdoption-osxphotos-export-save-config"],
             [0, "cmdoption-osxphotos-export-saved-to-library"],
             [0, "cmdoption-osxphotos-export-screenshot"],
             [0, "cmdoption-osxphotos-export-selected"],
             [0, "cmdoption-osxphotos-export-selfie"],
             [0, "cmdoption-osxphotos-export-shared"],
+            [0, "cmdoption-osxphotos-export-shared-moment"],
             [0, "cmdoption-osxphotos-export-sidecar"],
             [0, "cmdoption-osxphotos-export-sidecar-drop-ext"],
             [0, "cmdoption-osxphotos-export-skip-bursts"],
             [0, "cmdoption-osxphotos-export-skip-edited"],
             [0, "cmdoption-osxphotos-export-skip-live"],
             [0, "cmdoption-osxphotos-export-skip-original-if-edited"],
             [0, "cmdoption-osxphotos-export-skip-raw"],
@@ -5945,14 +5978,15 @@
             [0, "cmdoption-osxphotos-query-not-panorama"],
             [0, "cmdoption-osxphotos-query-not-portrait"],
             [0, "cmdoption-osxphotos-query-not-reference"],
             [0, "cmdoption-osxphotos-query-not-saved-to-library"],
             [0, "cmdoption-osxphotos-query-not-screenshot"],
             [0, "cmdoption-osxphotos-query-not-selfie"],
             [0, "cmdoption-osxphotos-query-not-shared"],
+            [0, "cmdoption-osxphotos-query-not-shared-moment"],
             [0, "cmdoption-osxphotos-query-not-slow-mo"],
             [0, "cmdoption-osxphotos-query-not-syndicated"],
             [0, "cmdoption-osxphotos-query-not-time-lapse"],
             [0, "cmdoption-osxphotos-query-only-movies"],
             [0, "cmdoption-osxphotos-query-only-photos"],
             [0, "cmdoption-osxphotos-query-panorama"],
             [0, "cmdoption-osxphotos-query-person"],
@@ -5964,14 +5998,15 @@
             [0, "cmdoption-osxphotos-query-quiet"],
             [0, "cmdoption-osxphotos-query-regex"],
             [0, "cmdoption-osxphotos-query-saved-to-library"],
             [0, "cmdoption-osxphotos-query-screenshot"],
             [0, "cmdoption-osxphotos-query-selected"],
             [0, "cmdoption-osxphotos-query-selfie"],
             [0, "cmdoption-osxphotos-query-shared"],
+            [0, "cmdoption-osxphotos-query-shared-moment"],
             [0, "cmdoption-osxphotos-query-slow-mo"],
             [0, "cmdoption-osxphotos-query-syndicated"],
             [0, "cmdoption-osxphotos-query-time-lapse"],
             [0, "cmdoption-osxphotos-query-title"],
             [0, "cmdoption-osxphotos-query-to-date"],
             [0, "cmdoption-osxphotos-query-to-time"],
             [0, "cmdoption-osxphotos-query-uti"],
@@ -6036,14 +6071,15 @@
             [0, "cmdoption-osxphotos-repl-not-panorama"],
             [0, "cmdoption-osxphotos-repl-not-portrait"],
             [0, "cmdoption-osxphotos-repl-not-reference"],
             [0, "cmdoption-osxphotos-repl-not-saved-to-library"],
             [0, "cmdoption-osxphotos-repl-not-screenshot"],
             [0, "cmdoption-osxphotos-repl-not-selfie"],
             [0, "cmdoption-osxphotos-repl-not-shared"],
+            [0, "cmdoption-osxphotos-repl-not-shared-moment"],
             [0, "cmdoption-osxphotos-repl-not-slow-mo"],
             [0, "cmdoption-osxphotos-repl-not-syndicated"],
             [0, "cmdoption-osxphotos-repl-not-time-lapse"],
             [0, "cmdoption-osxphotos-repl-only-movies"],
             [0, "cmdoption-osxphotos-repl-only-photos"],
             [0, "cmdoption-osxphotos-repl-panorama"],
             [0, "cmdoption-osxphotos-repl-person"],
@@ -6053,14 +6089,15 @@
             [0, "cmdoption-osxphotos-repl-query-function"],
             [0, "cmdoption-osxphotos-repl-regex"],
             [0, "cmdoption-osxphotos-repl-saved-to-library"],
             [0, "cmdoption-osxphotos-repl-screenshot"],
             [0, "cmdoption-osxphotos-repl-selected"],
             [0, "cmdoption-osxphotos-repl-selfie"],
             [0, "cmdoption-osxphotos-repl-shared"],
+            [0, "cmdoption-osxphotos-repl-shared-moment"],
             [0, "cmdoption-osxphotos-repl-slow-mo"],
             [0, "cmdoption-osxphotos-repl-syndicated"],
             [0, "cmdoption-osxphotos-repl-time-lapse"],
             [0, "cmdoption-osxphotos-repl-title"],
             [0, "cmdoption-osxphotos-repl-to-date"],
             [0, "cmdoption-osxphotos-repl-to-time"],
             [0, "cmdoption-osxphotos-repl-uti"],
@@ -6141,14 +6178,15 @@
             [0, "cmdoption-osxphotos-sync-not-missing"],
             [0, "cmdoption-osxphotos-sync-not-panorama"],
             [0, "cmdoption-osxphotos-sync-not-portrait"],
             [0, "cmdoption-osxphotos-sync-not-reference"],
             [0, "cmdoption-osxphotos-sync-not-saved-to-library"],
             [0, "cmdoption-osxphotos-sync-not-screenshot"],
             [0, "cmdoption-osxphotos-sync-not-selfie"],
+            [0, "cmdoption-osxphotos-sync-not-shared-moment"],
             [0, "cmdoption-osxphotos-sync-not-slow-mo"],
             [0, "cmdoption-osxphotos-sync-not-syndicated"],
             [0, "cmdoption-osxphotos-sync-not-time-lapse"],
             [0, "cmdoption-osxphotos-sync-only-movies"],
             [0, "cmdoption-osxphotos-sync-only-photos"],
             [0, "cmdoption-osxphotos-sync-panorama"],
             [0, "cmdoption-osxphotos-sync-person"],
@@ -6158,14 +6196,15 @@
             [0, "cmdoption-osxphotos-sync-query-function"],
             [0, "cmdoption-osxphotos-sync-regex"],
             [0, "cmdoption-osxphotos-sync-s"],
             [0, "cmdoption-osxphotos-sync-saved-to-library"],
             [0, "cmdoption-osxphotos-sync-screenshot"],
             [0, "cmdoption-osxphotos-sync-selected"],
             [0, "cmdoption-osxphotos-sync-selfie"],
+            [0, "cmdoption-osxphotos-sync-shared-moment"],
             [0, "cmdoption-osxphotos-sync-slow-mo"],
             [0, "cmdoption-osxphotos-sync-syndicated"],
             [0, "cmdoption-osxphotos-sync-theme"],
             [0, "cmdoption-osxphotos-sync-time-lapse"],
             [0, "cmdoption-osxphotos-sync-timestamp"],
             [0, "cmdoption-osxphotos-sync-title"],
             [0, "cmdoption-osxphotos-sync-to-date"],
@@ -7056,14 +7095,17 @@
         ],
         "not_selfie (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_selfie"]
         ],
         "not_shared (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_shared"]
         ],
+        "not_shared_moment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.not_shared_moment"]
+        ],
         "not_slow_mo (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_slow_mo"]
         ],
         "not_syndicated (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.not_syndicated"]
         ],
         "not_time_lapse (osxphotos.queryoptions attribute)": [
@@ -7314,14 +7356,20 @@
         ],
         "shared (osxphotos.photoinfo property)": [
             [4, "osxphotos.PhotoInfo.shared"]
         ],
         "shared (osxphotos.queryoptions attribute)": [
             [4, "osxphotos.QueryOptions.shared"]
         ],
+        "shared_moment (osxphotos.photoinfo property)": [
+            [4, "osxphotos.PhotoInfo.shared_moment"]
+        ],
+        "shared_moment (osxphotos.queryoptions attribute)": [
+            [4, "osxphotos.QueryOptions.shared_moment"]
+        ],
         "sidecar (osxphotos.exportoptions attribute)": [
             [4, "osxphotos.ExportOptions.sidecar"]
         ],
         "sidecar_drop_ext (osxphotos.exportoptions attribute)": [
             [4, "osxphotos.ExportOptions.sidecar_drop_ext"]
         ],
         "size_pixels (osxphotos.faceinfo property)": [
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
-        <title>OSXPhotos Template System - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos Template System - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
-<td><p>The osxphotos version, e.g. ‘0.60.8’</p></td>
+<td><p>The osxphotos version, e.g. ‘0.60.9’</p></td>
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
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
-{osxphotos_version}            The osxphotos version, e.g. â0.60.8â
+{osxphotos_version}            The osxphotos version, e.g. â0.60.9â
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
-        <title>OSXPhotos Tutorial - osxphotos 0.60.8 documentation</title>
+        <title>OSXPhotos Tutorial - osxphotos 0.60.9 documentation</title>
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
-      <a href="index.html"><div class="brand">osxphotos 0.60.8 documentation</div></a>
+      <a href="index.html"><div class="brand">osxphotos 0.60.9 documentation</div></a>
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
   
   
-  <span class="sidebar-brand-text">osxphotos 0.60.8 documentation</span>
+  <span class="sidebar-brand-text">osxphotos 0.60.9 documentation</span>
   
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
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 Toggle Light / Dark / Auto color theme
 
 Toggle table of contents sidebar
 
 
-osxphotos_0.60.8_documentation
+osxphotos_0.60.9_documentation
 [q                   ]
     * OSXPhotos
     * OSXPhotos_Tutorial
     * OSXPhotos_Command_Line_Interface_(CLI)
     * OSXPhotos_Template_System
     * OSXPhotos_Python_Package_Overview
     * OSXPhotos_Python_Reference
```

### Comparing `osxphotos-0.60.8/osxphotos/exif_datetime_updater.py` & `osxphotos-0.60.9/osxphotos/exif_datetime_updater.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/exifinfo.py` & `osxphotos-0.60.9/osxphotos/exifinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/exiftool.py` & `osxphotos-0.60.9/osxphotos/exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/exiftool_filetypes.json` & `osxphotos-0.60.9/osxphotos/exiftool_filetypes.json`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/export_db.py` & `osxphotos-0.60.9/osxphotos/export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/export_db_utils.py` & `osxphotos-0.60.9/osxphotos/export_db_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/fileutil.py` & `osxphotos-0.60.9/osxphotos/fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/frozen_photoinfo.py` & `osxphotos-0.60.9/osxphotos/frozen_photoinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/imageconverter.py` & `osxphotos-0.60.9/osxphotos/imageconverter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/momentinfo.py` & `osxphotos-0.60.9/osxphotos/momentinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/path_utils.py` & `osxphotos-0.60.9/osxphotos/path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/personinfo.py` & `osxphotos-0.60.9/osxphotos/personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photodates.py` & `osxphotos-0.60.9/osxphotos/photodates.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photoexporter.py` & `osxphotos-0.60.9/osxphotos/photoexporter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photoinfo.py` & `osxphotos-0.60.9/osxphotos/photoinfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,20 @@
             self._path = photopath
             return photopath
 
     def _path_5(self):
         """Returns candidate path for original photo on Photos >= version 5"""
         if self._info["shared"]:
             return self._path_5_shared()
+        if self.shared_moment and self._path_shared_moment():
+            # path for photos in shared moments if it's in the shared moment folder
+            # the file may also be in the originals folder which the next check will catch
+            # check shared_moment first as a photo can be both a shared moment and syndicated
+            # and if so, will be in the shared moment folder
+            return self._path_shared_moment()
         if self.syndicated and not self.saved_to_library:
             # path for "shared with you" syndicated photos that have not yet been saved to the library
             return self._path_syndication()
         return (
             os.path.join(self._info["directory"], self._info["filename"])
             if self._info["directory"].startswith("/")
             else os.path.join(
@@ -226,14 +232,29 @@
             self._db._library_path,
             syndication_path,
             uuid_dir,
             self.filename,
         )
         return path if os.path.isfile(path) else None
 
+    def _path_shared_moment(self):
+        """Return path for shared moment photo on Photos >= version 8"""
+        # Photos 8+ stores shared moment photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID.ext
+        # where X is first digit of UUID
+        momentshared_path = "scopes/momentshared/originals"
+        uuid_dir = self.uuid[0]
+        path = os.path.join(
+            self._db._library_path,
+            momentshared_path,
+            uuid_dir,
+            self.filename,
+        )
+        return path if os.path.isfile(path) else None
+
     def _path_4(self):
         """Returns candidate path for original photo on Photos <= version 4"""
         if self._info["has_raw"]:
             # return the path to JPEG even if RAW is original
             vol = (
                 self._db._dbvolumes[self._info["raw_pair_info"]["volumeId"]]
                 if self._info["raw_pair_info"]["volumeId"] is not None
@@ -906,14 +927,16 @@
 
         photopath = None
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_live_photo_4()
         elif self.live_photo and self.path and not self.ismissing:
             if self.shared:
                 return self._path_live_photo_shared_5()
+            if self.shared_moment:
+                return self._path_live_shared_moment()
             if self.syndicated and not self.saved_to_library:
                 # syndicated ("Shared with you") photos not yet saved to library
                 return self._path_live_syndicated()
 
             filename = pathlib.Path(self.path)
             photopath = filename.parent.joinpath(f"{filename.stem}_3.mov")
             photopath = str(photopath)
@@ -983,37 +1006,63 @@
             self._db._library_path,
             syndication_path,
             uuid_dir,
             filename,
         )
         return live_photo if os.path.isfile(live_photo) else None
 
+    def _path_live_shared_moment(self):
+        """Return path for live shared moment photo on Photos >= version 8"""
+        # Photos 8+ stores live shared moment photos in a separate directory
+        # in ~/Photos Library.photoslibrary/scopes/momentshared/originals/X/UUID_3.mov
+        # where X is first digit of UUID
+        shared_moment_path = "scopes/momentshared/originals"
+        uuid_dir = self.uuid[0]
+        filename = f"{pathlib.Path(self.filename).stem}_3.mov"
+        live_photo = os.path.join(
+            self._db._library_path,
+            shared_moment_path,
+            uuid_dir,
+            filename,
+        )
+        return live_photo if os.path.isfile(live_photo) else None
+
     @cached_property
     def path_derivatives(self) -> list[str]:
         """Return any derivative (preview) images associated with the photo as a list of paths, sorted by file size (largest first)"""
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return self._path_derivatives_4()
 
         if self.shared:
             return self._path_derivatives_5_shared()
 
         directory = self._uuid[0]  # first char of uuid
-        if self.syndicated and not self.saved_to_library:
+        if self.shared_moment:
+            # shared moments
+            derivative_path = "scopes/momentshared/resources/derivatives"
+            thumb_path = (
+                f"{derivative_path}/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
+            )
+        elif self.syndicated and not self.saved_to_library:
             # syndicated ("Shared with you") photos not yet saved to library
             derivative_path = "scopes/syndication/resources/derivatives"
             thumb_path = (
                 f"{derivative_path}/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
             )
         else:
-            derivative_path = f"resources/derivatives/{directory}"
+            derivative_path = "resources/derivatives"
             thumb_path = (
                 f"resources/derivatives/masters/{directory}/{self.uuid}_4_5005_c.jpeg"
             )
 
-        derivative_path = pathlib.Path(self._db._library_path).joinpath(derivative_path)
+        derivative_path = (
+            pathlib.Path(self._db._library_path)
+            .joinpath(derivative_path)
+            .joinpath(directory)
+        )
         thumb_path = pathlib.Path(self._db._library_path).joinpath(thumb_path)
 
         # find all files that start with uuid in derivative path
         files = list(derivative_path.glob(f"{self.uuid}*.*"))
 
         # previews may be missing from derivatives path
         # there are what appear to be low res thumbnails in the "masters" subfolder
@@ -1373,14 +1422,19 @@
             return None
 
         try:
             return self._db._db_syndication_uuid[self.uuid]["syndication_history"] != 0
         except KeyError:
             return False
 
+    @cached_property
+    def shared_moment(self) -> bool:
+        """Returns True if photo is part of a shared moment otherwise False"""
+        return bool(self._info["moment_share"])
+
     @property
     def labels(self):
         """returns list of labels applied to photo by Photos image categorization
         only valid on Photos 5, on older libraries returns empty list
         """
         if self._db._db_version <= _PHOTOS_4_VERSION:
             return []
```

### Comparing `osxphotos-0.60.8/osxphotos/photokit.py` & `osxphotos-0.60.9/osxphotos/photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosalbum.py` & `osxphotos-0.60.9/osxphotos/photosalbum.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photoscript_utils.py` & `osxphotos-0.60.9/osxphotos/photoscript_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_comments.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_exif.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_exif.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_faceinfo.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_scoreinfo.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_searchinfo.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/_photosdb_process_syndicationinfo.py` & `osxphotos-0.60.9/osxphotos/photosdb/_photosdb_process_syndicationinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/photosdb.py` & `osxphotos-0.60.9/osxphotos/photosdb/photosdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1231,14 +1231,17 @@
 
             # fingerprint
             self._dbphotos[uuid]["masterFingerprint"] = row[45]
 
             # photos 5+ only, for shared photos
             self._dbphotos[uuid]["cloudownerhashedpersonid"] = None
 
+            # photos 8+ only, shared moments
+            self._dbphotos[uuid]["moment_share"] = None
+
             # compute signatures for finding possible duplicates
             signature = self._duplicate_signature(uuid)
             try:
                 self._db_signatures[signature].append(uuid)
             except KeyError:
                 self._db_signatures[signature] = [uuid]
 
@@ -1945,15 +1948,16 @@
                 {depth_state},
                 {asset_table}.ZADJUSTMENTTIMESTAMP,
                 {asset_table}.ZVISIBILITYSTATE,
                 {asset_table}.ZTRASHEDDATE,
                 {asset_table}.ZSAVEDASSETTYPE,
                 {asset_table}.ZADDEDDATE,
                 {asset_table}.Z_PK,
-                {asset_table}.ZCLOUDOWNERHASHEDPERSONID
+                {asset_table}.ZCLOUDOWNERHASHEDPERSONID,
+                {asset_table}.ZMOMENTSHARE
                 FROM {asset_table} 
                 JOIN ZADDITIONALASSETATTRIBUTES ON ZADDITIONALASSETATTRIBUTES.ZASSET = {asset_table}.Z_PK 
                 ORDER BY {asset_table}.ZUUID  """
         )
         # Order of results
         # 0    SELECT ZGENERICASSET.ZUUID,
         # 1    ZADDITIONALASSETATTRIBUTES.ZMASTERFINGERPRINT,
@@ -1996,14 +2000,15 @@
         # 37   ZGENERICASSET.ZADJUSTMENTTIMESTAMP -- when was photo edited?
         # 38   ZGENERICASSET.ZVISIBILITYSTATE -- 0 if visible, 2 if not (e.g. a burst image)
         # 39   ZGENERICASSET.ZTRASHEDDATE -- date item placed in the trash or null if not in trash
         # 40   ZGENERICASSET.ZSAVEDASSETTYPE -- how item imported
         # 41   ZGENERICASSET.ZADDEDDATE -- date item added to the library
         # 42   ZGENERICASSET.Z_PK -- primary key
         # 43   ZGENERICASSET.ZCLOUDOWNERHASHEDPERSONID -- used to look up owner name (for shared photos)
+        # 44   ZASSET.ZMOMENTSHARE -- FK for ZSHARE (shared moments, Photos 8+)
 
         for row in c:
             uuid = row[0]
             info = {}
             info["_uuid"] = uuid  # stored here for easier debugging
             info["modelID"] = None
             info["masterUuid"] = None
@@ -2183,14 +2188,16 @@
                 info["added_date"] = datetime.fromtimestamp(row[41] + TIME_DELTA)
             except (ValueError, TypeError):
                 info["added_date"] = datetime(1970, 1, 1)
 
             info["pk"] = row[42]
             info["cloudownerhashedpersonid"] = row[43]
 
+            info["moment_share"] = row[44]
+
             # initialize import session info which will be filled in later
             # not every photo has an import session so initialize all records now
             info["import_session"] = None
             info["fok_import_session"] = None
             info["import_uuid"] = None
 
             # associated RAW image info
@@ -3528,14 +3535,19 @@
             photos = [p for p in photos if not p.syndicated]
 
         if options.saved_to_library:
             photos = [p for p in photos if p.syndicated and p.saved_to_library]
         elif options.not_saved_to_library:
             photos = [p for p in photos if p.syndicated and not p.saved_to_library]
 
+        if options.shared_moment:
+            photos = [p for p in photos if p.shared_moment]
+        elif options.not_shared_moment:
+            photos = [p for p in photos if not p.shared_moment]
+
         if options.function:
             for function in options.function:
                 photos = function[0](photos)
 
         # burst should be checked last, ref #640
         if options.burst_photos:
             # add the burst_photos to the export set
```

### Comparing `osxphotos-0.60.8/osxphotos/photosdb/photosdb_utils.py` & `osxphotos-0.60.9/osxphotos/photosdb/photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototables.py` & `osxphotos-0.60.9/osxphotos/phototables.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototemplate.cog.md` & `osxphotos-0.60.9/osxphotos/phototemplate.cog.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototemplate.md` & `osxphotos-0.60.9/osxphotos/phototemplate.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototemplate.py` & `osxphotos-0.60.9/osxphotos/phototemplate.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototemplate.tx` & `osxphotos-0.60.9/osxphotos/phototemplate.tx`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/phototz.py` & `osxphotos-0.60.9/osxphotos/phototz.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/placeinfo.py` & `osxphotos-0.60.9/osxphotos/placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/platform.py` & `osxphotos-0.60.9/osxphotos/platform.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/pyrepl.py` & `osxphotos-0.60.9/osxphotos/pyrepl.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/queries/shared_owner.sql.mako` & `osxphotos-0.60.9/osxphotos/queries/shared_owner.sql.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/query_builder.py` & `osxphotos-0.60.9/osxphotos/query_builder.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/queryoptions.py` & `osxphotos-0.60.9/osxphotos/queryoptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,16 @@
         uti: list of UTIs to search for
         uuid: list of uuids to search for
         year: search for photos taken in a given year
         syndicated: search for photos that have been shared via syndication ("Shared with You" album via Messages, etc.)
         not_syndicated: search for photos that have not been shared via syndication ("Shared with You" album via Messages, etc.)
         saved_to_library: search for syndicated photos that have been saved to the Photos library
         not_saved_to_library: search for syndicated photos that have not been saved to the Photos library
+        shared_moment: search for photos that have been shared via a shared moment
+        not_shared_moment: search for photos that have not been shared via a shared moment
     """
 
     added_after: Optional[datetime.datetime] = None
     added_before: Optional[datetime.datetime] = None
     added_in_last: Optional[datetime.timedelta] = None
     album: Optional[Iterable[str]] = None
     burst_photos: Optional[bool] = None
@@ -196,14 +198,16 @@
     uti: Optional[Iterable[str]] = None
     uuid: Optional[Iterable[str]] = None
     year: Optional[Iterable[int]] = None
     syndicated: Optional[bool] = None
     not_syndicated: Optional[bool] = None
     saved_to_library: Optional[bool] = None
     not_saved_to_library: Optional[bool] = None
+    shared_moment: Optional[bool] = None
+    not_shared_moment: Optional[bool] = None
 
     def asdict(self):
         return asdict(self)
 
 
 def query_options_from_kwargs(**kwargs) -> QueryOptions:
     """Validate query options and create a QueryOptions instance.
@@ -267,14 +271,15 @@
         ("slow_mo", "not_slow_mo"),
         ("time_lapse", "not_time_lapse"),
         ("deleted", "not_deleted"),
         ("deleted", "deleted_only"),
         ("deleted_only", "not_deleted"),
         ("syndicated", "not_syndicated"),
         ("saved_to_library", "not_saved_to_library"),
+        ("shared_moment", "not_shared_moment"),
     ]
     # TODO: add option to validate requiring at least one query arg
     for arg, not_arg in exclusive:
         if kwargs.get(arg) and kwargs.get(not_arg):
             arg = arg.replace("_", "-")
             not_arg = not_arg.replace("_", "-")
             raise IncompatibleQueryOptions(
```

### Comparing `osxphotos-0.60.8/osxphotos/scoreinfo.py` & `osxphotos-0.60.9/osxphotos/scoreinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/searchinfo.py` & `osxphotos-0.60.9/osxphotos/searchinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/sqlgrep.py` & `osxphotos-0.60.9/osxphotos/sqlgrep.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/sqlite_utils.py` & `osxphotos-0.60.9/osxphotos/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/sqlitekvstore.py` & `osxphotos-0.60.9/osxphotos/sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/template_counter.py` & `osxphotos-0.60.9/osxphotos/template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/templates/xmp_sidecar.mako` & `osxphotos-0.60.9/osxphotos/templates/xmp_sidecar.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/templates/xmp_sidecar_beta.mako` & `osxphotos-0.60.9/osxphotos/templates/xmp_sidecar_beta.mako`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/text_detection.py` & `osxphotos-0.60.9/osxphotos/text_detection.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/timeutils.py` & `osxphotos-0.60.9/osxphotos/timeutils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/timezones.py` & `osxphotos-0.60.9/osxphotos/timezones.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/tutorial.md` & `osxphotos-0.60.9/osxphotos/tutorial.md`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/unicode.py` & `osxphotos-0.60.9/osxphotos/unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/uti.py` & `osxphotos-0.60.9/osxphotos/uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos/utils.py` & `osxphotos-0.60.9/osxphotos/utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos.egg-info/PKG-INFO` & `osxphotos-0.60.9/osxphotos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osxphotos
-Version: 0.60.8
+Version: 0.60.9
 Summary: Export photos from Apple's macOS Photos app and query the Photos library database to access metadata about images.
 Home-page: https://github.com/RhetTbull/
 Download-URL: https://github.com/RhetTbull/osxphotos
 Author: Rhet Turnbull
 Author-email: rturnbull+git@gmail.com
 License: License :: OSI Approved :: MIT License
 Project-URL: GitHub, https://github.com/RhetTbull/osxphotos
```

### Comparing `osxphotos-0.60.8/osxphotos.egg-info/SOURCES.txt` & `osxphotos-0.60.9/osxphotos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/osxphotos.egg-info/requires.txt` & `osxphotos-0.60.9/osxphotos.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/setup.py` & `osxphotos-0.60.9/setup.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_10_12_6.py` & `osxphotos-0.60.9/tests/test_10_12_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_albums_folders_catalina_10_15_7.py` & `osxphotos-0.60.9/tests/test_albums_folders_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_albums_folders_high_sierra_10_13_6.py` & `osxphotos-0.60.9/tests/test_albums_folders_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_albums_folders_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_albums_folders_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_bigsur_10_16_0_1.py` & `osxphotos-0.60.9/tests/test_bigsur_10_16_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_catalina_10_15_7.py` & `osxphotos-0.60.9/tests/test_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli.py` & `osxphotos-0.60.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_add_locations.py` & `osxphotos-0.60.9/tests/test_cli_add_locations.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_add_to_album.py` & `osxphotos-0.60.9/tests/test_cli_add_to_album.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_all_commands.py` & `osxphotos-0.60.9/tests/test_cli_all_commands.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_batch_edit.py` & `osxphotos-0.60.9/tests/test_cli_batch_edit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_dump.py` & `osxphotos-0.60.9/tests/test_cli_dump.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_exiftool.py` & `osxphotos-0.60.9/tests/test_cli_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_export_cloud.py` & `osxphotos-0.60.9/tests/test_cli_export_cloud.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_export_projects.py` & `osxphotos-0.60.9/tests/test_cli_export_projects.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_exportdb.py` & `osxphotos-0.60.9/tests/test_cli_exportdb.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_import.py` & `osxphotos-0.60.9/tests/test_cli_import.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_orphans.py` & `osxphotos-0.60.9/tests/test_cli_orphans.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_param_types.py` & `osxphotos-0.60.9/tests/test_cli_param_types.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_sync.py` & `osxphotos-0.60.9/tests/test_cli_sync.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_timewarp.py` & `osxphotos-0.60.9/tests/test_cli_timewarp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_utils.py` & `osxphotos-0.60.9/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cli_verbose.py` & `osxphotos-0.60.9/tests/test_cli_verbose.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_cloud_owner_catalina.py` & `osxphotos-0.60.9/tests/test_cloud_owner_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_comments.py` & `osxphotos-0.60.9/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_concurrent_export.py` & `osxphotos-0.60.9/tests/test_concurrent_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_configoptions.py` & `osxphotos-0.60.9/tests/test_configoptions.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_datetime_formatter.py` & `osxphotos-0.60.9/tests/test_datetime_formatter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_datetime_utils.py` & `osxphotos-0.60.9/tests/test_datetime_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_debug.py` & `osxphotos-0.60.9/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_empty_library_4_0.py` & `osxphotos-0.60.9/tests/test_empty_library_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_exif_info.py` & `osxphotos-0.60.9/tests/test_exif_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_exiftool.py` & `osxphotos-0.60.9/tests/test_exiftool.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_exiftool_caching.py` & `osxphotos-0.60.9/tests/test_exiftool_caching.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_catalina_10_15_7.py` & `osxphotos-0.60.9/tests/test_export_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_catalina_10_15_7_use_photos_export.py` & `osxphotos-0.60.9/tests/test_export_catalina_10_15_7_use_photos_export.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_convert_to_jpeg.py` & `osxphotos-0.60.9/tests/test_export_convert_to_jpeg.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_db.py` & `osxphotos-0.60.9/tests/test_export_db.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_export_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_export_raw_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_export_raw_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_exportresults.py` & `osxphotos-0.60.9/tests/test_exportresults.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_faceinfo.py` & `osxphotos-0.60.9/tests/test_faceinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_fileutil.py` & `osxphotos-0.60.9/tests/test_fileutil.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_highsierra.py` & `osxphotos-0.60.9/tests/test_highsierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_image_converter.py` & `osxphotos-0.60.9/tests/test_image_converter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_incloud_big_sur_10_16_0.py` & `osxphotos-0.60.9/tests/test_incloud_big_sur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_incloud_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_incloud_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_incloud_catalina_10_15_6.py` & `osxphotos-0.60.9/tests/test_incloud_catalina_10_15_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_incloud_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_incloud_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_live_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_live_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_modified_date_catalina_10_15_7.py` & `osxphotos-0.60.9/tests/test_modified_date_catalina_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_modified_date_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_modified_date_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_mojave_10_14_6_path_edited.py` & `osxphotos-0.60.9/tests/test_mojave_10_14_6_path_edited.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_monterey_12_0_1.py` & `osxphotos-0.60.9/tests/test_monterey_12_0_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_monterey_dev_beta_12_0_0.py` & `osxphotos-0.60.9/tests/test_monterey_dev_beta_12_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_movies_4_0.py` & `osxphotos-0.60.9/tests/test_movies_4_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_movies_5_0.py` & `osxphotos-0.60.9/tests/test_movies_5_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_path_utils.py` & `osxphotos-0.60.9/tests/test_path_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_personinfo.py` & `osxphotos-0.60.9/tests/test_personinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_photokit.py` & `osxphotos-0.60.9/tests/test_photokit.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_photosalbum_unicode.py` & `osxphotos-0.60.9/tests/test_photosalbum_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_photosdb_utils.py` & `osxphotos-0.60.9/tests/test_photosdb_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_placeinfo.py` & `osxphotos-0.60.9/tests/test_placeinfo.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_places_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_places_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_places_high_sierra_10_13_6.py` & `osxphotos-0.60.9/tests/test_places_high_sierra_10_13_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_places_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_places_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_projects_catalina.py` & `osxphotos-0.60.9/tests/test_projects_catalina.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_projects_sierra.py` & `osxphotos-0.60.9/tests/test_projects_sierra.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_score_info.py` & `osxphotos-0.60.9/tests/test_score_info.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_search_info_10_14_6.py` & `osxphotos-0.60.9/tests/test_search_info_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_search_info_10_15_4.py` & `osxphotos-0.60.9/tests/test_search_info_10_15_4.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_search_info_10_15_5.py` & `osxphotos-0.60.9/tests/test_search_info_10_15_5.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_search_info_10_15_7.py` & `osxphotos-0.60.9/tests/test_search_info_10_15_7.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_shared_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_shared_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_shared_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_shared_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_sidecar_xmp.py` & `osxphotos-0.60.9/tests/test_sidecar_xmp.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_sonoma_14_0_0.py` & `osxphotos-0.60.9/tests/test_sonoma_14_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_specials_bigsur_10_16_0.py` & `osxphotos-0.60.9/tests/test_specials_bigsur_10_16_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_specials_catalina_10_15_1.py` & `osxphotos-0.60.9/tests/test_specials_catalina_10_15_1.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_specials_mojave_10_14_6.py` & `osxphotos-0.60.9/tests/test_specials_mojave_10_14_6.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_specials_sierra_10_12.py` & `osxphotos-0.60.9/tests/test_specials_sierra_10_12.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_sqlitekvstore.py` & `osxphotos-0.60.9/tests/test_sqlitekvstore.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_template.py` & `osxphotos-0.60.9/tests/test_template.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_template_counter.py` & `osxphotos-0.60.9/tests/test_template_counter.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_template_today.py` & `osxphotos-0.60.9/tests/test_template_today.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_unicode.py` & `osxphotos-0.60.9/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_uti.py` & `osxphotos-0.60.9/tests/test_uti.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_utils.py` & `osxphotos-0.60.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_ventura_13_0_0.py` & `osxphotos-0.60.9/tests/test_ventura_13_0_0.py`

 * *Files identical despite different names*

### Comparing `osxphotos-0.60.8/tests/test_ventura_dev_preview_13_0_0.py` & `osxphotos-0.60.9/tests/test_ventura_dev_preview_13_0_0.py`

 * *Files identical despite different names*

