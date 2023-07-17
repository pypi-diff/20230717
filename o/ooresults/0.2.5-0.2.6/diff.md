# Comparing `tmp/ooresults-0.2.5.tar.gz` & `tmp/ooresults-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ooresults-0.2.5.tar", last modified: Mon Jun  5 16:45:52 2023, max compression
+gzip compressed data, was "ooresults-0.2.6.tar", last modified: Mon Jul 17 16:34:16 2023, max compression
```

## Comparing `ooresults-0.2.5.tar` & `ooresults-0.2.6.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/
--rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.5/LICENSE
--rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.5/MANIFEST.in
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-06-05 16:45:52.971423 ooresults-0.2.5/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.5/README.rst
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    11381 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/_server.py
--rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/configuration.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.943423 ooresults-0.2.5/ooresults/handler/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/build_results.py
--rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/demo_reader.py
--rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/events.py
--rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/handler/handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    31158 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/handler/model.py
--rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/results.py
--rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/handler/series.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.943423 ooresults-0.2.5/ooresults/pdf/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.947423 ooresults-0.2.5/ooresults/pdf/fonts/
--rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Bold.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Italic.ttf
--rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Regular.ttf
--rw-r--r--   0 rainer    (1000) users      (100)     3687 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/pdf.py
--rw-r--r--   0 rainer    (1000) users      (100)    11389 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/result.py
--rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/pdf/series.py
--rw-r--r--   0 rainer    (1000) users      (100)    10868 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/pdf/splittimes.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/__init__.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults/plugins/imports/
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/plugins/imports/entries/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/imports/entries/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/plugins/imports/entries/text.py
--rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/iof_result_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/oe12.py
--rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/plugins/oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/reader.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/class_params.py
--rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/repo.py
--rw-r--r--   0 rainer    (1000) users      (100)    16754 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/repo/result_type.py
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/series_type.py
--rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/repo/sqlite_repo.py
--rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/start_type.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.951423 ooresults-0.2.5/ooresults/repo/update/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/update_008.py
--rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/repo/update/update_tables.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.955423 ooresults-0.2.5/ooresults/schema/
--rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/schema/IOF.xsd
--rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/schema/cardreader_log.json
--rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/server.py
--rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/set_legacy_mode.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.955423 ooresults-0.2.5/ooresults/static/
--rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/style-tab.css
--rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/style.css
--rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/static/w3.js
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/templates/
--rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/add_class.html
--rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_club.html
--rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_competitor.html
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_course.html
--rw-r--r--   0 rainer    (1000) users      (100)     6405 2023-05-07 16:05:24.000000 ooresults-0.2.5/ooresults/templates/add_entry.html
--rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_entry_competitors.html
--rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/add_entry_result.html
--rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/add_event.html
--rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/base.html
--rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/classes_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/classes_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/clubs_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/clubs_table.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/competitors_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/competitors_table.html
--rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/courses_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/courses_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.5/ooresults/templates/demo_reader.html
--rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/entries_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     3006 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/entries_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/events_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/events_table.html
--rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/main.html
--rw-r--r--   0 rainer    (1000) users      (100)     5925 2023-06-05 16:41:57.000000 ooresults-0.2.5/ooresults/templates/results_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/results_table.html
--rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/root.html
--rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/select_event.html
--rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/series_settings.html
--rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/series_tab_content.html
--rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/series_table.html
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/templates/si/
--rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/si/si1_data.html
--rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si1_error.html
--rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si1_page.html
--rw-r--r--   0 rainer    (1000) users      (100)     4161 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/templates/si/si2_data.html
--rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/si/si2_page.html
--rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/templates/unauthorized.html
--rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/user.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/utils/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/utils/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1666 2023-04-23 07:29:14.000000 ooresults-0.2.5/ooresults/utils/globals.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.963423 ooresults-0.2.5/ooresults/websocket_server/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/si.py
--rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/websocket_handler.py
--rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.5/ooresults/websocket_server/websocket_server.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.939423 ooresults-0.2.5/ooresults.egg-info/
--rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/PKG-INFO
--rw-r--r--   0 rainer    (1000) users      (100)     4563 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/SOURCES.txt
--rw-r--r--   0 rainer    (1000) users      (100)        1 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/dependency_links.txt
--rw-r--r--   0 rainer    (1000) users      (100)      102 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/entry_points.txt
--rw-r--r--   0 rainer    (1000) users      (100)      152 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/requires.txt
--rw-r--r--   0 rainer    (1000) users      (100)       10 2023-06-05 16:45:52.000000 ooresults-0.2.5/ooresults.egg-info/top_level.txt
--rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-06-05 16:41:57.000000 ooresults-0.2.5/pyproject.toml
--rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-06-05 16:45:52.971423 ooresults-0.2.5/setup.cfg
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.967423 ooresults-0.2.5/tests/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/competitor.py
--rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/entry.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.967423 ooresults-0.2.5/tests/model/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/model/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_build_series_result.py
--rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_event_class_results.py
--rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/model/test_parse_cardreader_log.py
--rw-r--r--   0 rainer    (1000) users      (100)    34026 2023-05-07 16:05:24.000000 ooresults-0.2.5/tests/model/test_store_cardreader_result.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/tests/plugins/
--rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_export_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_import_competitors_oe2003.py
--rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_class_list.py
--rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_competitor_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_course_data.py
--rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_entry_list.py
--rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/plugins/test_plugin_iof_result_list.py
-drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-06-05 16:45:52.971423 ooresults-0.2.5/tests/repo/
--rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/__init__.py
--rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_classes.py
--rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_clubs.py
--rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_competitors.py
--rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_courses.py
--rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/repo/test_entries.py
--rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_events.py
--rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/repo/test_settings.py
--rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_compute_result_net.py
--rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_compute_result_score.py
--rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_compute_result_standard.py
--rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_configuration.py
--rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_globals.py
--rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_handicap.py
--rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_ranking.py
--rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.5/tests/test_series.py
--rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.5/tests/test_user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.254811 ooresults-0.2.6/
+-rw-r--r--   0 rainer    (1000) users      (100)    34523 2023-03-01 18:09:04.000000 ooresults-0.2.6/LICENSE
+-rw-r--r--   0 rainer    (1000) users      (100)      260 2023-03-01 18:09:04.000000 ooresults-0.2.6/MANIFEST.in
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-07-17 16:34:16.254811 ooresults-0.2.6/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     2278 2023-03-01 18:09:04.000000 ooresults-0.2.6/README.rst
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.222811 ooresults-0.2.6/ooresults/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15992 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11495 2023-07-17 16:30:29.000000 ooresults-0.2.6/ooresults/_server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4363 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/configuration.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.226811 ooresults-0.2.6/ooresults/handler/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/handler/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9134 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/build_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7873 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2597 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4559 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/handler/competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5824 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1110 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/demo_reader.py
+-rw-r--r--   0 rainer    (1000) users      (100)    12416 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3351 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4504 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/handler/handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    31158 2023-05-07 16:05:24.000000 ooresults-0.2.6/ooresults/handler/model.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3536 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/results.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4892 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/handler/series.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.226811 ooresults-0.2.6/ooresults/pdf/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.230811 ooresults-0.2.6/ooresults/pdf/fonts/
+-rw-r--r--   0 rainer    (1000) users      (100)   690516 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Bold.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   816716 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/pdf/fonts/Carlito-BoldItalic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   623416 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Italic.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)   635996 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Regular.ttf
+-rw-r--r--   0 rainer    (1000) users      (100)     3687 2023-06-05 16:41:57.000000 ooresults-0.2.6/ooresults/pdf/pdf.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11389 2023-06-05 16:41:57.000000 ooresults-0.2.6/ooresults/pdf/result.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5283 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/pdf/series.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10868 2023-06-05 16:41:57.000000 ooresults-0.2.6/ooresults/pdf/splittimes.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.234811 ooresults-0.2.6/ooresults/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/plugins/__init__.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.218811 ooresults-0.2.6/ooresults/plugins/imports/
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.234811 ooresults-0.2.6/ooresults/plugins/imports/entries/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/plugins/imports/entries/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2948 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/plugins/imports/entries/text.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2813 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4068 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5935 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5184 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10702 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/iof_result_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7446 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/oe12.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14580 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/plugins/oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/reader.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.234811 ooresults-0.2.6/ooresults/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2237 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/class_params.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7358 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16754 2023-05-07 16:05:24.000000 ooresults-0.2.6/ooresults/repo/result_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/series_type.py
+-rw-r--r--   0 rainer    (1000) users      (100)    36849 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/repo/sqlite_repo.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1265 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/start_type.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.234811 ooresults-0.2.6/ooresults/repo/update/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/update/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4728 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/update/update_008.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1890 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/repo/update/update_tables.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.238811 ooresults-0.2.6/ooresults/schema/
+-rw-r--r--   0 rainer    (1000) users      (100)   177863 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/schema/IOF.xsd
+-rwxr-xr-x   0 rainer    (1000) users      (100)     2117 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/schema/cardreader_log.json
+-rw-r--r--   0 rainer    (1000) users      (100)      905 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/server.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2257 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/set_legacy_mode.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.238811 ooresults-0.2.6/ooresults/static/
+-rw-r--r--   0 rainer    (1000) users      (100)      643 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/static/style-tab.css
+-rw-r--r--   0 rainer    (1000) users      (100)     1267 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/static/style.css
+-rw-r--r--   0 rainer    (1000) users      (100)    12106 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/static/w3.js
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.242811 ooresults-0.2.6/ooresults/templates/
+-rw-r--r--   0 rainer    (1000) users      (100)     5964 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/add_class.html
+-rw-r--r--   0 rainer    (1000) users      (100)      883 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/add_club.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3093 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/add_competitor.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/add_course.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6405 2023-05-07 16:05:24.000000 ooresults-0.2.6/ooresults/templates/add_entry.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1811 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/add_entry_competitors.html
+-rw-r--r--   0 rainer    (1000) users      (100)     7204 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/add_entry_result.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2511 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/add_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)      466 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/base.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11941 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/classes_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2957 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/classes_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6858 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/clubs_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)      453 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/clubs_table.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    11673 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/competitors_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1030 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/competitors_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)    11955 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/courses_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1386 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/courses_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6529 2023-04-23 07:11:17.000000 ooresults-0.2.6/ooresults/templates/demo_reader.html
+-rwxr-xr-x   0 rainer    (1000) users      (100)    19221 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/entries_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3019 2023-07-17 16:30:29.000000 ooresults-0.2.6/ooresults/templates/entries_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     9445 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/events_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1339 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/events_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5937 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/main.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5925 2023-06-05 16:41:57.000000 ooresults-0.2.6/ooresults/templates/results_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     5390 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/results_table.html
+-rw-r--r--   0 rainer    (1000) users      (100)      528 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/root.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1084 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/select_event.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2500 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/series_settings.html
+-rw-r--r--   0 rainer    (1000) users      (100)     8367 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/series_tab_content.html
+-rw-r--r--   0 rainer    (1000) users      (100)     1541 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/series_table.html
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.246811 ooresults-0.2.6/ooresults/templates/si/
+-rw-r--r--   0 rainer    (1000) users      (100)      902 2023-04-23 07:29:14.000000 ooresults-0.2.6/ooresults/templates/si/si1_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)      396 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/si/si1_error.html
+-rw-r--r--   0 rainer    (1000) users      (100)     6992 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/si/si1_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)     4174 2023-07-17 16:30:29.000000 ooresults-0.2.6/ooresults/templates/si/si2_data.html
+-rw-r--r--   0 rainer    (1000) users      (100)     3589 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/si/si2_page.html
+-rw-r--r--   0 rainer    (1000) users      (100)      383 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/templates/unauthorized.html
+-rw-r--r--   0 rainer    (1000) users      (100)     2407 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/user.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.246811 ooresults-0.2.6/ooresults/utils/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/utils/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1751 2023-07-17 16:30:29.000000 ooresults-0.2.6/ooresults/utils/globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1411 2023-07-17 16:30:29.000000 ooresults-0.2.6/ooresults/utils/rental_cards.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.246811 ooresults-0.2.6/ooresults/websocket_server/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/websocket_server/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1749 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/websocket_server/si.py
+-rw-r--r--   0 rainer    (1000) users      (100)    14523 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/websocket_server/websocket_handler.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2143 2023-03-01 18:09:04.000000 ooresults-0.2.6/ooresults/websocket_server/websocket_server.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.222811 ooresults-0.2.6/ooresults.egg-info/
+-rw-r--r--   0 rainer    (1000) users      (100)    42907 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/PKG-INFO
+-rw-r--r--   0 rainer    (1000) users      (100)     4622 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/SOURCES.txt
+-rw-r--r--   0 rainer    (1000) users      (100)        1 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/dependency_links.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      102 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/entry_points.txt
+-rw-r--r--   0 rainer    (1000) users      (100)      152 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/requires.txt
+-rw-r--r--   0 rainer    (1000) users      (100)       10 2023-07-17 16:34:16.000000 ooresults-0.2.6/ooresults.egg-info/top_level.txt
+-rwxr-xr-x   0 rainer    (1000) users      (100)      977 2023-07-17 16:30:29.000000 ooresults-0.2.6/pyproject.toml
+-rwxr-xr-x   0 rainer    (1000) users      (100)      616 2023-07-17 16:34:16.254811 ooresults-0.2.6/setup.cfg
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.250811 ooresults-0.2.6/tests/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1414 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/competitor.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2061 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/entry.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.250811 ooresults-0.2.6/tests/model/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/model/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8015 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/model/test_build_series_result.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11820 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/model/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)     6578 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/model/test_event_class_results.py
+-rw-r--r--   0 rainer    (1000) users      (100)    16528 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/model/test_parse_cardreader_log.py
+-rw-r--r--   0 rainer    (1000) users      (100)    34026 2023-05-07 16:05:24.000000 ooresults-0.2.6/tests/model/test_store_cardreader_result.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.250811 ooresults-0.2.6/tests/plugins/
+-rw-r--r--   0 rainer    (1000) users      (100)    13070 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_export_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)    29297 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_import_competitors_oe2003.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2766 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_plugin_iof_class_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)     4000 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_plugin_iof_competitor_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10229 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_plugin_iof_course_data.py
+-rw-r--r--   0 rainer    (1000) users      (100)     8789 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_plugin_iof_entry_list.py
+-rw-r--r--   0 rainer    (1000) users      (100)    30446 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/plugins/test_plugin_iof_result_list.py
+drwxr-xr-x   0 rainer    (1000) users      (100)        0 2023-07-17 16:34:16.254811 ooresults-0.2.6/tests/repo/
+-rw-r--r--   0 rainer    (1000) users      (100)      803 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/repo/__init__.py
+-rw-r--r--   0 rainer    (1000) users      (100)    11959 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/repo/test_classes.py
+-rw-r--r--   0 rainer    (1000) users      (100)     5314 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/repo/test_clubs.py
+-rw-r--r--   0 rainer    (1000) users      (100)    10687 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/repo/test_competitors.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7336 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/repo/test_courses.py
+-rw-r--r--   0 rainer    (1000) users      (100)    39686 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/repo/test_entries.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7540 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/repo/test_events.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2353 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/repo/test_settings.py
+-rw-r--r--   0 rainer    (1000) users      (100)     9467 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/test_compute_result_net.py
+-rw-r--r--   0 rainer    (1000) users      (100)    15440 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/test_compute_result_score.py
+-rw-r--r--   0 rainer    (1000) users      (100)    38250 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/test_compute_result_standard.py
+-rw-r--r--   0 rainer    (1000) users      (100)     7257 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/test_configuration.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1973 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/test_globals.py
+-rw-r--r--   0 rainer    (1000) users      (100)     1758 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/test_handicap.py
+-rw-r--r--   0 rainer    (1000) users      (100)    23885 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/test_ranking.py
+-rw-r--r--   0 rainer    (1000) users      (100)     3671 2023-07-17 16:30:29.000000 ooresults-0.2.6/tests/test_rental_cards.py
+-rw-r--r--   0 rainer    (1000) users      (100)    26132 2023-04-23 07:29:14.000000 ooresults-0.2.6/tests/test_series.py
+-rw-r--r--   0 rainer    (1000) users      (100)     2326 2023-03-01 18:09:04.000000 ooresults-0.2.6/tests/test_user.py
```

### Comparing `ooresults-0.2.5/LICENSE` & `ooresults-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/PKG-INFO` & `ooresults-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.5
+Version: 0.2.6
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.5/README.rst` & `ooresults-0.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/__init__.py` & `ooresults-0.2.6/ooresults/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/_reader.py` & `ooresults-0.2.6/ooresults/_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/_server.py` & `ooresults-0.2.6/ooresults/_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 import ooresults.handler.events
 import ooresults.handler.demo_reader
 from ooresults import configuration
 from ooresults.handler import model
 from ooresults.handler import results
 from ooresults.repo.sqlite_repo import SqliteRepo
 from ooresults.user import Users
+from ooresults.utils import rental_cards
 from ooresults.utils.globals import t_globals
 from ooresults.websocket_server.websocket_handler import WebSocketHandler
 from ooresults.websocket_server.websocket_server import WebSocketServer
 
 
 web.config.debug = False
 
@@ -282,14 +283,16 @@
     try:
         config = configuration.Config(path=main_path)
     except (RuntimeError, FileNotFoundError) as e:
         print(f'Error in file {str(main_path / "config.ini")}:')
         print(f"  {str(e)}")
         return 2
 
+    rental_cards.read_rental_cards(path=main_path / "rental_cards.txt")
+
     try:
         model.db = SqliteRepo(
             db=str(database),
         )
     except (RuntimeError, sqlite3.Error):
         exc_type, exc_value, _ = sys.exc_info()
         logging.error(f"{exc_type.__module__}.{exc_type.__name__}: {exc_value}")
```

### Comparing `ooresults-0.2.5/ooresults/configuration.py` & `ooresults-0.2.6/ooresults/configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/__init__.py` & `ooresults-0.2.6/ooresults/handler/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/build_results.py` & `ooresults-0.2.6/ooresults/handler/build_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/classes.py` & `ooresults-0.2.6/ooresults/handler/classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/clubs.py` & `ooresults-0.2.6/ooresults/handler/clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/competitors.py` & `ooresults-0.2.6/ooresults/handler/competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/courses.py` & `ooresults-0.2.6/ooresults/handler/courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/demo_reader.py` & `ooresults-0.2.6/ooresults/handler/demo_reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/entries.py` & `ooresults-0.2.6/ooresults/handler/entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/events.py` & `ooresults-0.2.6/ooresults/handler/events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/handicap.py` & `ooresults-0.2.6/ooresults/handler/handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/model.py` & `ooresults-0.2.6/ooresults/handler/model.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/results.py` & `ooresults-0.2.6/ooresults/handler/results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/handler/series.py` & `ooresults-0.2.6/ooresults/handler/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Bold.ttf` & `ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Bold.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-BoldItalic.ttf` & `ooresults-0.2.6/ooresults/pdf/fonts/Carlito-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Italic.ttf` & `ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Italic.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/fonts/Carlito-Regular.ttf` & `ooresults-0.2.6/ooresults/pdf/fonts/Carlito-Regular.ttf`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/pdf.py` & `ooresults-0.2.6/ooresults/pdf/pdf.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/result.py` & `ooresults-0.2.6/ooresults/pdf/result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/series.py` & `ooresults-0.2.6/ooresults/pdf/series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/pdf/splittimes.py` & `ooresults-0.2.6/ooresults/pdf/splittimes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/__init__.py` & `ooresults-0.2.6/ooresults/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/imports/entries/__init__.py` & `ooresults-0.2.6/ooresults/plugins/imports/entries/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/imports/entries/text.py` & `ooresults-0.2.6/ooresults/plugins/imports/entries/text.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/iof_class_list.py` & `ooresults-0.2.6/ooresults/plugins/iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/iof_competitor_list.py` & `ooresults-0.2.6/ooresults/plugins/iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/iof_course_data.py` & `ooresults-0.2.6/ooresults/plugins/iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/iof_entry_list.py` & `ooresults-0.2.6/ooresults/plugins/iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/iof_result_list.py` & `ooresults-0.2.6/ooresults/plugins/iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/oe12.py` & `ooresults-0.2.6/ooresults/plugins/oe12.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/plugins/oe2003.py` & `ooresults-0.2.6/ooresults/plugins/oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/reader.py` & `ooresults-0.2.6/ooresults/reader.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/__init__.py` & `ooresults-0.2.6/ooresults/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/class_params.py` & `ooresults-0.2.6/ooresults/repo/class_params.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/repo.py` & `ooresults-0.2.6/ooresults/repo/repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/result_type.py` & `ooresults-0.2.6/ooresults/repo/result_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/series_type.py` & `ooresults-0.2.6/ooresults/repo/series_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/sqlite_repo.py` & `ooresults-0.2.6/ooresults/repo/sqlite_repo.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/start_type.py` & `ooresults-0.2.6/ooresults/repo/start_type.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/update/__init__.py` & `ooresults-0.2.6/ooresults/repo/update/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/update/update_008.py` & `ooresults-0.2.6/ooresults/repo/update/update_008.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/repo/update/update_tables.py` & `ooresults-0.2.6/ooresults/repo/update/update_tables.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/schema/IOF.xsd` & `ooresults-0.2.6/ooresults/schema/IOF.xsd`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/schema/cardreader_log.json` & `ooresults-0.2.6/ooresults/schema/cardreader_log.json`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/server.py` & `ooresults-0.2.6/ooresults/server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/set_legacy_mode.py` & `ooresults-0.2.6/ooresults/set_legacy_mode.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/static/style-tab.css` & `ooresults-0.2.6/ooresults/static/style-tab.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/static/style.css` & `ooresults-0.2.6/ooresults/static/style.css`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/static/w3.js` & `ooresults-0.2.6/ooresults/static/w3.js`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_class.html` & `ooresults-0.2.6/ooresults/templates/add_class.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_club.html` & `ooresults-0.2.6/ooresults/templates/add_club.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_competitor.html` & `ooresults-0.2.6/ooresults/templates/add_competitor.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_course.html` & `ooresults-0.2.6/ooresults/templates/add_course.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_entry.html` & `ooresults-0.2.6/ooresults/templates/add_entry.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_entry_competitors.html` & `ooresults-0.2.6/ooresults/templates/add_entry_competitors.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_entry_result.html` & `ooresults-0.2.6/ooresults/templates/add_entry_result.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/add_event.html` & `ooresults-0.2.6/ooresults/templates/add_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/classes_tab_content.html` & `ooresults-0.2.6/ooresults/templates/classes_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/classes_table.html` & `ooresults-0.2.6/ooresults/templates/classes_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/clubs_tab_content.html` & `ooresults-0.2.6/ooresults/templates/clubs_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/competitors_tab_content.html` & `ooresults-0.2.6/ooresults/templates/competitors_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/competitors_table.html` & `ooresults-0.2.6/ooresults/templates/competitors_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/courses_tab_content.html` & `ooresults-0.2.6/ooresults/templates/courses_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/courses_table.html` & `ooresults-0.2.6/ooresults/templates/courses_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/demo_reader.html` & `ooresults-0.2.6/ooresults/templates/demo_reader.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/entries_tab_content.html` & `ooresults-0.2.6/ooresults/templates/entries_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/entries_table.html` & `ooresults-0.2.6/ooresults/templates/entries_table.html`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
         <tbody id="entries_tbody">
         $for competitor in competitors:
             <tr class="dt" id="$competitor.get('id', '')">
                 <td class="dt">$competitor.get('first_name', '')</td>
                 <td class="dt" id="entr_table_lastname">$competitor.get('last_name', '')</td>
                 <td class="dt">$competitor.get('gender', '')</td>
                 <td class="dt">$format_year(competitor.get('year', None))</td>
-                <td class="dt" style="text-align:right">$competitor.get('chip', '')</td>
+                <td class="dt" style="text-align:right">$format_card(competitor.get('chip', ''))</td>
                 <td class="dt">$competitor.get('club', '')</td>
                 <td class="dt">$competitor.get('class_', '')</td>
                 <td class="dt" style="text-align: center;">$('X' if competitor.get('not_competing', False) else '')</td>
                 $if event:
                     $for i in range(len(event.fields)):
                         <td class="dt">$competitor.fields.get(i, '')</td>
                 <td class="dt" style="text-align:right">$(format_date(competitor.start.start_time))</td>
```

#### html2text {}

```diff
@@ -3,11 +3,11 @@
 format_time(time): $if time is not None: $return minutes_seconds(time) $else:
 $return '' $def format_date(time): $if time is not None: $return time.strftime
 ('%H:%M:%S') $else: $return ''
 Event name: $event.get('name', '')
 Event date: $(date.isoformat() if date != '' else '')
 [                    ]
 First name      Last name       Gender          Year            Chip            Club            Class             NC          $event.fields[i]       Start                          Time                              Status
-$competitor.get $competitor.get                 $format_year                                                    $('X' if                                                                $(format_time
-('first_name',  ('last_name',   $competitor.get (competitor.get $competitor.get $competitor.get $competitor.get competitor.get    $competitor.fields.get $(format_date                  (competitor.result.extensions.get $MAP_STATUS
-'')             '')             ('gender', '')  ('year', None)) ('chip', '')    ('club', '')    ('class_', '')  ('not_competing', (i, '')                (competitor.start.start_time)) ('running_time',                  [competitor.result.status]
+$competitor.get $competitor.get                 $format_year    $format_card                                    $('X' if                                                                $(format_time
+('first_name',  ('last_name',   $competitor.get (competitor.get (competitor.get $competitor.get $competitor.get competitor.get    $competitor.fields.get $(format_date                  (competitor.result.extensions.get $MAP_STATUS
+'')             '')             ('gender', '')  ('year', None)) ('chip', ''))   ('club', '')    ('class_', '')  ('not_competing', (i, '')                (competitor.start.start_time)) ('running_time',                  [competitor.result.status]
                                                                                                                 False) else '')                                                         competitor.result.time)))
```

### Comparing `ooresults-0.2.5/ooresults/templates/events_tab_content.html` & `ooresults-0.2.6/ooresults/templates/events_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/events_table.html` & `ooresults-0.2.6/ooresults/templates/events_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/main.html` & `ooresults-0.2.6/ooresults/templates/main.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/results_tab_content.html` & `ooresults-0.2.6/ooresults/templates/results_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/results_table.html` & `ooresults-0.2.6/ooresults/templates/results_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/root.html` & `ooresults-0.2.6/ooresults/templates/root.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/select_event.html` & `ooresults-0.2.6/ooresults/templates/select_event.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/series_settings.html` & `ooresults-0.2.6/ooresults/templates/series_settings.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/series_tab_content.html` & `ooresults-0.2.6/ooresults/templates/series_tab_content.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/series_table.html` & `ooresults-0.2.6/ooresults/templates/series_table.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/si/si1_data.html` & `ooresults-0.2.6/ooresults/templates/si/si1_data.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/si/si1_page.html` & `ooresults-0.2.6/ooresults/templates/si/si1_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/templates/si/si2_data.html` & `ooresults-0.2.6/ooresults/templates/si/si2_data.html`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             </tr>
         </thead>
         <tbody>
         $for result in messages:
             $if event.get('id', -1) == result.get('eventId', '-2'):
                 <tr class="dt" style="background-color: $color(result.get('status'))">
                     <td class="dt">$result.get('entryTime', '')</td>
-                    <td class="dt" style="text-align:right">$result.get('controlCard')</td>
+                    <td class="dt" style="text-align:right">$format_card(result.get('controlCard'))</td>
                     <td class="dt">$MAP_STATUS[result.get('status')]</td>
                     <td class="dt" style="text-align:right">$format(result.get('time', 0))</td>
                     $if result.get('status') in (ResultStatus.OK, ResultStatus.MISSING_PUNCH, ResultStatus.DID_NOT_FINISH, ResultStatus.OVER_TIME):
                         <td class="dt">$result.get('lastName', ''), $result.get('firstName', '')</td>
                         <td class="dt">$result.get('class', '')</td>
                         <td class="dt">$missing(result.get('status'), result.get('missingControls', []))</td>
                     $else:
```

#### html2text {}

```diff
@@ -21,15 +21,15 @@
 1: return missing_controls[0] elif len(missing_controls) == 2: return
 missing_controls[0] + ', ' + missing_controls[1] elif len(missing_controls) ==
 3: return missing_controls[0] + ', ' + missing_controls[1] + ', ' +
 missing_controls[2] elif len(missing_controls) >= 4: return str(len
 (missing_controls)) + ' controls'
 Event name: $(event.get('name', '') if event is not None else '')
 Event date: $(date.isoformat() if date != '' else '')
-Read          Control card    Status      Time        Name          Class       Missing controls
-                                                      $result.get               $missing(result.get
-$result.get                   $MAP_STATUS $format     ('lastName',  $result.get ('status'),         $result.get
-('entryTime', $result.get     [result.get (result.get ''),          ('class',   result.get          ('error',
-'')           ('controlCard') ('status')] ('time',    $result.get   '')         ('missingControls', '')
-                                          0))         ('firstName',             []))
-                                                      '')
+Read          Control card     Status      Time        Name          Class       Missing controls
+                                                       $result.get               $missing(result.get
+$result.get   $format_card     $MAP_STATUS $format     ('lastName',  $result.get ('status'),         $result.get
+('entryTime', (result.get      [result.get (result.get ''),          ('class',   result.get          ('error',
+'')           ('controlCard')) ('status')] ('time',    $result.get   '')         ('missingControls', '')
+                                           0))         ('firstName',             []))
+                                                       '')
 $:format_cardreader_status(status)
```

### Comparing `ooresults-0.2.5/ooresults/templates/si/si2_page.html` & `ooresults-0.2.6/ooresults/templates/si/si2_page.html`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/user.py` & `ooresults-0.2.6/ooresults/user.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/utils/__init__.py` & `ooresults-0.2.6/ooresults/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/utils/globals.py` & `ooresults-0.2.6/ooresults/utils/globals.py`

 * *Files 19% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 # You should have received a copy of the GNU Affero General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 
 from typing import Optional
 
 from ooresults.repo.result_type import ResultStatus
+from ooresults.utils.rental_cards import format_card
 
 
 MAP_STATUS = {
     ResultStatus.INACTIVE: "",
     ResultStatus.FINISHED: "Finished",
     ResultStatus.OK: "OK",
     ResultStatus.MISSING_PUNCH: "MP",
@@ -49,8 +50,9 @@
 t_globals = {
     "str": str,
     "round": round,
     "ResultStatus": ResultStatus,
     "MAP_STATUS": MAP_STATUS,
     "EXPERIMENTAL": EXPERIMENTAL,
     "minutes_seconds": minutes_seconds,
+    "format_card": format_card,
 }
```

### Comparing `ooresults-0.2.5/ooresults/websocket_server/__init__.py` & `ooresults-0.2.6/ooresults/websocket_server/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/websocket_server/si.py` & `ooresults-0.2.6/ooresults/websocket_server/si.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/websocket_server/websocket_handler.py` & `ooresults-0.2.6/ooresults/websocket_server/websocket_handler.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults/websocket_server/websocket_server.py` & `ooresults-0.2.6/ooresults/websocket_server/websocket_server.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/ooresults.egg-info/PKG-INFO` & `ooresults-0.2.6/ooresults.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ooresults
-Version: 0.2.5
+Version: 0.2.6
 Summary: A software for the evaluation of the results of orienteering events
 Author: Rainer Garus
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `ooresults-0.2.5/ooresults.egg-info/SOURCES.txt` & `ooresults-0.2.6/ooresults.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -97,28 +97,30 @@
 ooresults/templates/si/si1_data.html
 ooresults/templates/si/si1_error.html
 ooresults/templates/si/si1_page.html
 ooresults/templates/si/si2_data.html
 ooresults/templates/si/si2_page.html
 ooresults/utils/__init__.py
 ooresults/utils/globals.py
+ooresults/utils/rental_cards.py
 ooresults/websocket_server/__init__.py
 ooresults/websocket_server/si.py
 ooresults/websocket_server/websocket_handler.py
 ooresults/websocket_server/websocket_server.py
 tests/__init__.py
 tests/competitor.py
 tests/entry.py
 tests/test_compute_result_net.py
 tests/test_compute_result_score.py
 tests/test_compute_result_standard.py
 tests/test_configuration.py
 tests/test_globals.py
 tests/test_handicap.py
 tests/test_ranking.py
+tests/test_rental_cards.py
 tests/test_series.py
 tests/test_user.py
 tests/model/__init__.py
 tests/model/test_build_series_result.py
 tests/model/test_courses.py
 tests/model/test_event_class_results.py
 tests/model/test_parse_cardreader_log.py
```

### Comparing `ooresults-0.2.5/pyproject.toml` & `ooresults-0.2.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ooresults"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   {name="Rainer Garus"},
 ]
 description = "A software for the evaluation of the results of orienteering events"
 readme = "README.rst"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
```

### Comparing `ooresults-0.2.5/setup.cfg` & `ooresults-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/__init__.py` & `ooresults-0.2.6/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/competitor.py` & `ooresults-0.2.6/tests/competitor.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/entry.py` & `ooresults-0.2.6/tests/entry.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/__init__.py` & `ooresults-0.2.6/tests/model/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/test_build_series_result.py` & `ooresults-0.2.6/tests/model/test_build_series_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/test_courses.py` & `ooresults-0.2.6/tests/model/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/test_event_class_results.py` & `ooresults-0.2.6/tests/model/test_event_class_results.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/test_parse_cardreader_log.py` & `ooresults-0.2.6/tests/model/test_parse_cardreader_log.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/model/test_store_cardreader_result.py` & `ooresults-0.2.6/tests/model/test_store_cardreader_result.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_export_competitors_oe2003.py` & `ooresults-0.2.6/tests/plugins/test_export_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_import_competitors_oe2003.py` & `ooresults-0.2.6/tests/plugins/test_import_competitors_oe2003.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_plugin_iof_class_list.py` & `ooresults-0.2.6/tests/plugins/test_plugin_iof_class_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_plugin_iof_competitor_list.py` & `ooresults-0.2.6/tests/plugins/test_plugin_iof_competitor_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_plugin_iof_course_data.py` & `ooresults-0.2.6/tests/plugins/test_plugin_iof_course_data.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_plugin_iof_entry_list.py` & `ooresults-0.2.6/tests/plugins/test_plugin_iof_entry_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/plugins/test_plugin_iof_result_list.py` & `ooresults-0.2.6/tests/plugins/test_plugin_iof_result_list.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/__init__.py` & `ooresults-0.2.6/tests/repo/__init__.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_classes.py` & `ooresults-0.2.6/tests/repo/test_classes.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_clubs.py` & `ooresults-0.2.6/tests/repo/test_clubs.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_competitors.py` & `ooresults-0.2.6/tests/repo/test_competitors.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_courses.py` & `ooresults-0.2.6/tests/repo/test_courses.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_entries.py` & `ooresults-0.2.6/tests/repo/test_entries.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_events.py` & `ooresults-0.2.6/tests/repo/test_events.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/repo/test_settings.py` & `ooresults-0.2.6/tests/repo/test_settings.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_compute_result_net.py` & `ooresults-0.2.6/tests/test_compute_result_net.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_compute_result_score.py` & `ooresults-0.2.6/tests/test_compute_result_score.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_compute_result_standard.py` & `ooresults-0.2.6/tests/test_compute_result_standard.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_configuration.py` & `ooresults-0.2.6/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_globals.py` & `ooresults-0.2.6/tests/test_globals.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_handicap.py` & `ooresults-0.2.6/tests/test_handicap.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_ranking.py` & `ooresults-0.2.6/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_series.py` & `ooresults-0.2.6/tests/test_series.py`

 * *Files identical despite different names*

### Comparing `ooresults-0.2.5/tests/test_user.py` & `ooresults-0.2.6/tests/test_user.py`

 * *Files identical despite different names*

