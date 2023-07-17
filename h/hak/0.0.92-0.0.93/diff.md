# Comparing `tmp/hak-0.0.92.tar.gz` & `tmp/hak-0.0.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hak-0.0.92.tar", last modified: Mon Jul 17 06:42:04 2023, max compression
+gzip compressed data, was "hak-0.0.93.tar", last modified: Mon Jul 17 10:49:56 2023, max compression
```

## Comparing `hak-0.0.92.tar` & `hak-0.0.93.tar`

### file list

```diff
@@ -1,530 +1,532 @@
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/
--rw-rw-r--   0 q         (1000) q         (1000)     1068 2023-07-07 13:22:08.000000 hak-0.0.92/LICENSE
--rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-17 06:42:04.895896 hak-0.0.92/PKG-INFO
--rw-rw-r--   0 q         (1000) q         (1000)      583 2023-07-10 13:04:07.000000 hak-0.0.92/README.md
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 04:34:17.000000 hak-0.0.92/hak/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/data/
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-04 23:50:58.000000 hak-0.0.92/hak/data/months.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/fake/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.92/hak/fake/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/fake/os/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.92/hak/fake/os/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      418 2023-04-23 03:18:31.000000 hak-0.0.92/hak/fake/os/system.py
--rw-rw-r--   0 q         (1000) q         (1000)      424 2023-04-23 03:18:31.000000 hak-0.0.92/hak/fake/printer.py
--rw-rw-r--   0 q         (1000) q         (1000)       45 2023-04-23 03:18:31.000000 hak-0.0.92/hak/fake/sleep.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/fake/subprocess/
--rw-rw-r--   0 q         (1000) q         (1000)     5858 2023-07-06 06:52:44.000000 hak-0.0.92/hak/fake/subprocess/run.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/many/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/bools/
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 06:52:37.000000 hak-0.0.92/hak/many/bools/count_true.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/dicts/
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 06:52:47.000000 hak-0.0.92/hak/many/dicts/a_into_b.py
--rw-rw-r--   0 q         (1000) q         (1000)     1136 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/dicts/compare.py
--rw-rw-r--   0 q         (1000) q         (1000)      911 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/dicts/compare_relevant_only.py
--rw-rw-r--   0 q         (1000) q         (1000)      797 2023-07-10 13:05:10.000000 hak-0.0.92/hak/many/dicts/convert_date_strings_to_dates.py
--rw-rw-r--   0 q         (1000) q         (1000)      306 2023-07-17 06:38:48.000000 hak-0.0.92/hak/many/dicts/get_all_keys.py
--rw-rw-r--   0 q         (1000) q         (1000)      666 2023-07-17 06:38:53.000000 hak-0.0.92/hak/many/dicts/get_datatypes.py
--rw-rw-r--   0 q         (1000) q         (1000)      493 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/dicts/get_first_and_last_dates.py
--rw-rw-r--   0 q         (1000) q         (1000)     1429 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/dicts/get_keys_with_none_or_zero_vals.py
--rw-rw-r--   0 q         (1000) q         (1000)      199 2023-07-06 06:53:17.000000 hak-0.0.92/hak/many/dicts/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      663 2023-07-06 06:53:28.000000 hak-0.0.92/hak/many/dicts/merge_freq_dicts.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 06:53:38.000000 hak-0.0.92/hak/many/dicts/reindex.py
--rw-rw-r--   0 q         (1000) q         (1000)      203 2023-07-06 06:53:48.000000 hak-0.0.92/hak/many/dicts/sort_by_key.py
--rw-rw-r--   0 q         (1000) q         (1000)      384 2023-07-10 13:05:47.000000 hak-0.0.92/hak/many/dicts/sum_by_key.py
--rw-rw-r--   0 q         (1000) q         (1000)    10015 2023-07-17 06:38:58.000000 hak-0.0.92/hak/many/dicts/to_table.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/directories/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/directories/empty/
--rw-rw-r--   0 q         (1000) q         (1000)      701 2023-07-10 13:07:02.000000 hak-0.0.92/hak/many/directories/empty/find.py
--rw-rw-r--   0 q         (1000) q         (1000)      649 2023-07-10 13:07:36.000000 hak-0.0.92/hak/many/directories/empty/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 06:54:08.000000 hak-0.0.92/hak/many/directories/exist.py
--rw-rw-r--   0 q         (1000) q         (1000)      606 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/directories/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      440 2023-07-07 05:17:37.000000 hak-0.0.92/hak/many/directories/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/many/files/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/files/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)     1789 2023-07-06 06:54:28.000000 hak-0.0.92/hak/many/files/pyfiles/dismantle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/lists/
--rw-rw-r--   0 q         (1000) q         (1000)      216 2023-07-06 06:54:38.000000 hak-0.0.92/hak/many/lists/merge.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/numbers/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:09:58.000000 hak-0.0.92/hak/many/numbers/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/numbers/ints/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:11:47.000000 hak-0.0.92/hak/many/numbers/ints/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/numbers/ints/mode/
--rw-rw-r--   0 q         (1000) q         (1000)      405 2023-07-10 13:08:08.000000 hak-0.0.92/hak/many/numbers/ints/mode/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      148 2023-07-10 12:30:14.000000 hak-0.0.92/hak/many/numbers/ints/remove_zeroes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)      161 2023-07-06 06:54:46.000000 hak-0.0.92/hak/many/pyfiles/format.py
--rw-rw-r--   0 q         (1000) q         (1000)      847 2023-07-06 06:54:53.000000 hak-0.0.92/hak/many/pyfiles/format_and_commit.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:00.000000 hak-0.0.92/hak/many/strings/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      130 2023-07-06 06:55:08.000000 hak-0.0.92/hak/many/strings/add_src_funks_prefix.py
--rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-06 06:55:15.000000 hak-0.0.92/hak/many/strings/compare.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/contain/
--rw-rw-r--   0 q         (1000) q         (1000)      145 2023-07-06 06:55:23.000000 hak-0.0.92/hak/many/strings/contain/version.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/date_pieces/
--rw-rw-r--   0 q         (1000) q         (1000)      676 2023-07-10 13:09:01.000000 hak-0.0.92/hak/many/strings/date_pieces/get.py
--rw-rw-r--   0 q         (1000) q         (1000)     3832 2023-07-10 13:10:37.000000 hak-0.0.92/hak/many/strings/date_pieces/separate_day.py
--rw-rw-r--   0 q         (1000) q         (1000)      834 2023-07-10 13:12:11.000000 hak-0.0.92/hak/many/strings/date_pieces/separate_year.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/dates/
--rw-rw-r--   0 q         (1000) q         (1000)     3259 2023-07-10 13:12:55.000000 hak-0.0.92/hak/many/strings/dates/detect_format.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/filepaths/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:30.000000 hak-0.0.92/hak/many/strings/filepaths/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1238 2023-07-10 13:15:48.000000 hak-0.0.92/hak/many/strings/filepaths/get_least_recently_modified.py
--rw-rw-r--   0 q         (1000) q         (1000)     1196 2023-07-10 13:16:18.000000 hak-0.0.92/hak/many/strings/filepaths/get_most_recently_modified.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/filepaths/py/
--rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-06 06:55:37.000000 hak-0.0.92/hak/many/strings/filepaths/py/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/filepaths/py/testables/
--rw-rw-r--   0 q         (1000) q         (1000)     2077 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/strings/filepaths/py/testables/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      660 2023-07-06 06:55:52.000000 hak-0.0.92/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py
--rw-rw-r--   0 q         (1000) q         (1000)     2234 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/strings/find_first_diff.py
--rw-rw-r--   0 q         (1000) q         (1000)      291 2023-07-10 13:16:37.000000 hak-0.0.92/hak/many/strings/get_index_of_first_difference.py
--rw-rw-r--   0 q         (1000) q         (1000)      444 2023-07-06 06:56:07.000000 hak-0.0.92/hak/many/strings/make_patch_version_change_to_py.py
--rw-rw-r--   0 q         (1000) q         (1000)      297 2023-07-06 06:56:14.000000 hak-0.0.92/hak/many/strings/module_names_from_py_filenames.py
--rw-rw-r--   0 q         (1000) q         (1000)      416 2023-07-06 06:56:22.000000 hak-0.0.92/hak/many/strings/patch_setup_cfg.py
--rw-rw-r--   0 q         (1000) q         (1000)      632 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/strings/patch_setup_py.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/strings/pyfiles/
--rw-rw-r--   0 q         (1000) q         (1000)     1514 2023-07-06 06:56:37.000000 hak-0.0.92/hak/many/strings/pyfiles/filter_out_items.py
--rw-rw-r--   0 q         (1000) q         (1000)      782 2023-07-10 13:03:40.000000 hak-0.0.92/hak/many/strings/show_diff.py
--rw-rw-r--   0 q         (1000) q         (1000)      667 2023-07-06 06:56:51.000000 hak-0.0.92/hak/many/strings/to_dict.py
--rw-rw-r--   0 q         (1000) q         (1000)      357 2023-07-06 06:56:59.000000 hak-0.0.92/hak/many/strings/two_char_combinations.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/tuples/
--rw-rw-r--   0 q         (1000) q         (1000)      261 2023-07-10 13:16:50.000000 hak-0.0.92/hak/many/tuples/to_dict.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/many/values/
--rw-rw-r--   0 q         (1000) q         (1000)     2157 2023-07-17 06:39:03.000000 hak-0.0.92/hak/many/values/get_datatype.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/none/
--rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 06:57:14.000000 hak-0.0.92/hak/none/nop.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/one/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/one/bool/
--rw-rw-r--   0 q         (1000) q         (1000)       86 2023-07-06 06:57:21.000000 hak-0.0.92/hak/one/bool/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      103 2023-07-06 06:57:28.000000 hak-0.0.92/hak/one/bool/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak/one/bool/or_none/
--rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 06:57:36.000000 hak-0.0.92/hak/one/bool/or_none/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      125 2023-07-06 06:57:43.000000 hak-0.0.92/hak/one/bool/or_none/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      762 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/check_if_ok_to_proceed.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/date/
--rw-rw-r--   0 q         (1000) q         (1000)      143 2023-07-06 06:57:58.000000 hak-0.0.92/hak/one/date/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      347 2023-07-06 06:58:06.000000 hak-0.0.92/hak/one/date/is_first_second_or_third_day_of_month.py
--rw-rw-r--   0 q         (1000) q         (1000)      414 2023-07-06 06:58:13.000000 hak-0.0.92/hak/one/date/is_first_week_of_quarter.py
--rw-rw-r--   0 q         (1000) q         (1000)      208 2023-07-06 06:58:20.000000 hak-0.0.92/hak/one/date/is_monday.py
--rw-rw-r--   0 q         (1000) q         (1000)      462 2023-07-06 06:58:28.000000 hak-0.0.92/hak/one/date/is_weekday.py
--rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 06:58:35.000000 hak-0.0.92/hak/one/date/is_weekend.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/date/public_holiday/
--rw-rw-r--   0 q         (1000) q         (1000)     4981 2023-07-10 13:17:27.000000 hak-0.0.92/hak/one/date/public_holiday/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 06:58:50.000000 hak-0.0.92/hak/one/date/select_from_last_n_days.py
--rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 06:58:57.000000 hak-0.0.92/hak/one/date/to_dd_mm_yyyy_str.py
--rw-rw-r--   0 q         (1000) q         (1000)     1216 2023-07-10 13:17:49.000000 hak-0.0.92/hak/one/date/to_financial_year.py
--rw-rw-r--   0 q         (1000) q         (1000)      609 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/date/to_utc_timestamp.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/date/year/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/date/year/easter_sunday/
--rw-rw-r--   0 q         (1000) q         (1000)      940 2023-07-10 13:18:07.000000 hak-0.0.92/hak/one/date/year/easter_sunday/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/datetime/
--rw-rw-r--   0 q         (1000) q         (1000)      149 2023-07-06 06:59:20.000000 hak-0.0.92/hak/one/datetime/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      272 2023-07-06 06:59:27.000000 hak-0.0.92/hak/one/datetime/select_from_last_n_days.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:34.000000 hak-0.0.92/hak/one/dict/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/cell/
--rw-rw-r--   0 q         (1000) q         (1000)     2118 2023-07-17 06:39:08.000000 hak-0.0.92/hak/one/dict/cell/get_width.py
--rw-rw-r--   0 q         (1000) q         (1000)     2595 2023-07-17 06:39:13.000000 hak-0.0.92/hak/one/dict/cell/make.py
--rw-rw-r--   0 q         (1000) q         (1000)     1474 2023-07-17 06:39:17.000000 hak-0.0.92/hak/one/dict/cell/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)      219 2023-07-06 06:59:42.000000 hak-0.0.92/hak/one/dict/convert_to_sql_insertable.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/custom_order/
--rw-rw-r--   0 q         (1000) q         (1000)      384 2023-07-17 06:39:22.000000 hak-0.0.92/hak/one/dict/custom_order/apply.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/durations/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:49.000000 hak-0.0.92/hak/one/dict/durations/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1147 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/durations/load.py
--rw-rw-r--   0 q         (1000) q         (1000)      800 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/durations/save.py
--rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 07:00:12.000000 hak-0.0.92/hak/one/dict/durations/to_tuple_list_sorted_by_duration.py
--rw-rw-r--   0 q         (1000) q         (1000)      769 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/durations/update_one.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/frequencies/
--rw-rw-r--   0 q         (1000) q         (1000)      519 2023-07-06 07:00:27.000000 hak-0.0.92/hak/one/dict/frequencies/choose.py
--rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 07:00:35.000000 hak-0.0.92/hak/one/dict/frequencies/make_from_strings.py
--rw-rw-r--   0 q         (1000) q         (1000)      187 2023-07-06 07:00:42.000000 hak-0.0.92/hak/one/dict/get_or_default.py
--rw-rw-r--   0 q         (1000) q         (1000)      616 2023-07-10 13:19:02.000000 hak-0.0.92/hak/one/dict/get_or_zero.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/header/
--rw-rw-r--   0 q         (1000) q         (1000)     2425 2023-07-17 06:39:27.000000 hak-0.0.92/hak/one/dict/header/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/hidden_fields/
--rw-rw-r--   0 q         (1000) q         (1000)      240 2023-07-17 06:39:32.000000 hak-0.0.92/hak/one/dict/hidden_fields/hide.py
--rw-rw-r--   0 q         (1000) q         (1000)      190 2023-07-06 07:00:57.000000 hak-0.0.92/hak/one/dict/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 07:01:05.000000 hak-0.0.92/hak/one/dict/make_from_key_value_lists.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/period/
--rw-rw-r--   0 q         (1000) q         (1000)     1016 2023-07-10 14:58:58.000000 hak-0.0.92/hak/one/dict/period/contains_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/period/financial_year/
--rw-rw-r--   0 q         (1000) q         (1000)      896 2023-07-10 14:58:56.000000 hak-0.0.92/hak/one/dict/period/financial_year/contains_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/period/financial_year/ge.py
--rw-rw-r--   0 q         (1000) q         (1000)      317 2023-07-10 14:58:55.000000 hak-0.0.92/hak/one/dict/period/financial_year/get_end_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      589 2023-07-10 14:58:54.000000 hak-0.0.92/hak/one/dict/period/financial_year/get_start_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/period/financial_year/gt.py
--rw-rw-r--   0 q         (1000) q         (1000)      388 2023-07-10 13:04:13.000000 hak-0.0.92/hak/one/dict/period/financial_year/increment.py
--rw-rw-r--   0 q         (1000) q         (1000)     1415 2023-07-10 13:06:36.000000 hak-0.0.92/hak/one/dict/period/financial_year/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:07:10.000000 hak-0.0.92/hak/one/dict/period/financial_year/le.py
--rw-rw-r--   0 q         (1000) q         (1000)      856 2023-07-10 13:07:47.000000 hak-0.0.92/hak/one/dict/period/financial_year/leq.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:08:14.000000 hak-0.0.92/hak/one/dict/period/financial_year/lt.py
--rw-rw-r--   0 q         (1000) q         (1000)     1733 2023-07-10 14:58:59.000000 hak-0.0.92/hak/one/dict/period/financial_year/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      255 2023-07-10 13:11:06.000000 hak-0.0.92/hak/one/dict/period/financial_year/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)     1307 2023-07-10 14:58:54.000000 hak-0.0.92/hak/one/dict/period/get_end.py
--rw-rw-r--   0 q         (1000) q         (1000)     1457 2023-07-10 15:00:35.000000 hak-0.0.92/hak/one/dict/period/get_start.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/period/month/
--rw-rw-r--   0 q         (1000) q         (1000)      460 2023-07-10 14:58:53.000000 hak-0.0.92/hak/one/dict/period/month/contains_date.py
--rw-rw-r--   0 q         (1000) q         (1000)     1179 2023-07-10 14:58:51.000000 hak-0.0.92/hak/one/dict/period/month/get_end_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-10 14:58:50.000000 hak-0.0.92/hak/one/dict/period/month/get_start_date.py
--rw-rw-r--   0 q         (1000) q         (1000)      283 2023-07-10 13:20:49.000000 hak-0.0.92/hak/one/dict/pick_by_keys.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/proposed_dismantlement/
--rw-rw-r--   0 q         (1000) q         (1000)     1544 2023-07-06 07:01:20.000000 hak-0.0.92/hak/one/dict/proposed_dismantlement/show.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/rate/
--rw-rw-r--   0 q         (1000) q         (1000)      614 2023-07-17 06:39:37.000000 hak-0.0.92/hak/one/dict/rate/abs.py
--rw-rw-r--   0 q         (1000) q         (1000)     1388 2023-07-17 06:39:42.000000 hak-0.0.92/hak/one/dict/rate/add.py
--rw-rw-r--   0 q         (1000) q         (1000)      884 2023-07-17 06:39:47.000000 hak-0.0.92/hak/one/dict/rate/div_number_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)     1379 2023-07-17 06:39:51.000000 hak-0.0.92/hak/one/dict/rate/div_rate_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)     1190 2023-07-17 06:39:56.000000 hak-0.0.92/hak/one/dict/rate/eq.py
--rw-rw-r--   0 q         (1000) q         (1000)      755 2023-07-17 06:40:01.000000 hak-0.0.92/hak/one/dict/rate/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)     4623 2023-07-17 06:40:06.000000 hak-0.0.92/hak/one/dict/rate/make.py
--rw-rw-r--   0 q         (1000) q         (1000)     1033 2023-07-17 06:40:11.000000 hak-0.0.92/hak/one/dict/rate/mult_rate_by_number.py
--rw-rw-r--   0 q         (1000) q         (1000)     1321 2023-07-17 06:40:16.000000 hak-0.0.92/hak/one/dict/rate/mult_rate_by_rate.py
--rw-rw-r--   0 q         (1000) q         (1000)     1351 2023-07-17 06:40:21.000000 hak-0.0.92/hak/one/dict/rate/sub.py
--rw-rw-r--   0 q         (1000) q         (1000)      597 2023-07-17 06:40:25.000000 hak-0.0.92/hak/one/dict/rate/to_float.py
--rw-rw-r--   0 q         (1000) q         (1000)      643 2023-07-17 06:40:30.000000 hak-0.0.92/hak/one/dict/rate/to_num.py
--rw-rw-r--   0 q         (1000) q         (1000)      323 2023-07-17 06:40:35.000000 hak-0.0.92/hak/one/dict/rate/to_str.py
--rw-rw-r--   0 q         (1000) q         (1000)      241 2023-07-17 06:40:40.000000 hak-0.0.92/hak/one/dict/rate/to_str_frac.py
--rw-rw-r--   0 q         (1000) q         (1000)      837 2023-07-17 06:40:45.000000 hak-0.0.92/hak/one/dict/remove_zeroes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/table/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:26.000000 hak-0.0.92/hak/one/dict/table/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1344 2023-07-17 06:40:50.000000 hak-0.0.92/hak/one/dict/table/get_field_widths.py
--rw-rw-r--   0 q         (1000) q         (1000)     4031 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/dict/to_max_line_width_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/values/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:43.000000 hak-0.0.92/hak/one/dict/values/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/values/numbers/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:50.000000 hak-0.0.92/hak/one/dict/values/numbers/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/values/numbers/negative/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:58.000000 hak-0.0.92/hak/one/dict/values/numbers/negative/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:21:57.000000 hak-0.0.92/hak/one/dict/values/numbers/negative/count.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/dict/values/numbers/positive/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:13.000000 hak-0.0.92/hak/one/dict/values/numbers/positive/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:22:10.000000 hak-0.0.92/hak/one/dict/values/numbers/positive/count.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/directory/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:28.000000 hak-0.0.92/hak/one/directory/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1568 2023-07-06 07:03:35.000000 hak-0.0.92/hak/one/directory/compress_to_tar.py
--rw-rw-r--   0 q         (1000) q         (1000)      728 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/directory/empty.py
--rw-rw-r--   0 q         (1000) q         (1000)       88 2023-07-06 07:03:51.000000 hak-0.0.92/hak/one/directory/exists.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/directory/filepaths/
--rw-rw-r--   0 q         (1000) q         (1000)     1463 2023-07-10 13:28:32.000000 hak-0.0.92/hak/one/directory/filepaths/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/directory/filepaths/packages/
--rw-rw-r--   0 q         (1000) q         (1000)     1311 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/directory/filepaths/packages/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      641 2023-07-10 13:22:24.000000 hak-0.0.92/hak/one/directory/is_empty.py
--rw-rw-r--   0 q         (1000) q         (1000)      662 2023-07-06 07:04:36.000000 hak-0.0.92/hak/one/directory/is_module.py
--rw-rw-r--   0 q         (1000) q         (1000)      763 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/directory/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      810 2023-07-07 01:06:11.000000 hak-0.0.92/hak/one/directory/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)     3737 2023-07-06 07:04:58.000000 hak-0.0.92/hak/one/duration.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.883895 hak-0.0.92/hak/one/file/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:06.000000 hak-0.0.92/hak/one/file/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      793 2023-07-06 07:05:13.000000 hak-0.0.92/hak/one/file/decrypt.py
--rw-rw-r--   0 q         (1000) q         (1000)      945 2023-07-06 07:05:20.000000 hak-0.0.92/hak/one/file/encrypt.py
--rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-10 13:22:54.000000 hak-0.0.92/hak/one/file/get_next_line_as_int.py
--rw-rw-r--   0 q         (1000) q         (1000)      705 2023-07-06 07:05:35.000000 hak-0.0.92/hak/one/file/load.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/pickle/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:42.000000 hak-0.0.92/hak/one/file/pickle/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     1265 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/file/pickle/load_if_exists.py
--rw-rw-r--   0 q         (1000) q         (1000)      922 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/file/pickle/save.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/py/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:06:05.000000 hak-0.0.92/hak/one/file/py/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      566 2023-07-06 07:06:12.000000 hak-0.0.92/hak/one/file/py/create.py
--rw-rw-r--   0 q         (1000) q         (1000)     2645 2023-07-06 07:06:19.000000 hak-0.0.92/hak/one/file/py/dismantle.py
--rw-rw-r--   0 q         (1000) q         (1000)     3827 2023-07-06 07:06:27.000000 hak-0.0.92/hak/one/file/py/extract_fn.py
--rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 07:06:34.000000 hak-0.0.92/hak/one/file/py/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 07:06:42.000000 hak-0.0.92/hak/one/file/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      963 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/file/save.py
--rw-rw-r--   0 q         (1000) q         (1000)      770 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/file/save_lines.py
--rw-rw-r--   0 q         (1000) q         (1000)      324 2023-07-06 07:07:04.000000 hak-0.0.92/hak/one/file/save_lines_or_string.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/file/secret/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/secret/password/
--rw-rw-r--   0 q         (1000) q         (1000)      696 2023-07-06 07:07:12.000000 hak-0.0.92/hak/one/file/secret/password/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/secret/username/
--rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 07:07:19.000000 hak-0.0.92/hak/one/file/secret/username/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/tar/
--rw-rw-r--   0 q         (1000) q         (1000)     1574 2023-07-06 07:07:26.000000 hak-0.0.92/hak/one/file/tar/extract.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/file/zip/
--rw-rw-r--   0 q         (1000) q         (1000)      507 2023-07-06 07:07:35.000000 hak-0.0.92/hak/one/file/zip/extract.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/function/
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:33:41.000000 hak-0.0.92/hak/one/function/function.py
--rw-rw-r--   0 q         (1000) q         (1000)      439 2023-07-06 08:33:48.000000 hak-0.0.92/hak/one/function/write_to_file.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/list/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:33:56.000000 hak-0.0.92/hak/one/list/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 08:34:03.000000 hak-0.0.92/hak/one/list/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      115 2023-07-06 08:34:11.000000 hak-0.0.92/hak/one/list/to_comma_separated_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/duration_ms/
--rw-rw-r--   0 q         (1000) q         (1000)     2120 2023-07-06 08:34:18.000000 hak-0.0.92/hak/one/number/duration_ms/to_bar.py
--rw-rw-r--   0 q         (1000) q         (1000)      296 2023-07-06 08:34:26.000000 hak-0.0.92/hak/one/number/duration_ms/to_bar_width.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/float/
--rw-rw-r--   0 q         (1000) q         (1000)       70 2023-07-06 08:34:33.000000 hak-0.0.92/hak/one/number/float/epsilon.py
--rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:41.000000 hak-0.0.92/hak/one/number/float/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:48.000000 hak-0.0.92/hak/one/number/float/is_not.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/float/nan/
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:34:55.000000 hak-0.0.92/hak/one/number/float/nan/to_none.py
--rw-rw-r--   0 q         (1000) q         (1000)      740 2023-07-10 13:23:05.000000 hak-0.0.92/hak/one/number/float/snap_to_zero.py
--rw-rw-r--   0 q         (1000) q         (1000)      475 2023-07-17 06:40:55.000000 hak-0.0.92/hak/one/number/float/to_rate.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/days/
--rw-rw-r--   0 q         (1000) q         (1000)      227 2023-07-06 08:35:11.000000 hak-0.0.92/hak/one/number/int/days/a_to_b_inclusive.py
--rw-rw-r--   0 q         (1000) q         (1000)      104 2023-07-06 08:35:18.000000 hak-0.0.92/hak/one/number/int/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      434 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/number/int/is_prime.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/polarity/
--rw-rw-r--   0 q         (1000) q         (1000)      499 2023-07-10 13:23:20.000000 hak-0.0.92/hak/one/number/int/polarity/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/primes/
--rw-rw-r--   0 q         (1000) q         (1000)      867 2023-07-06 08:35:40.000000 hak-0.0.92/hak/one/number/int/primes/download_prime_10.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/primes/prime_factors/
--rw-rw-r--   0 q         (1000) q         (1000)     1993 2023-07-17 06:41:00.000000 hak-0.0.92/hak/one/number/int/primes/prime_factors/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/width/
--rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 08:35:55.000000 hak-0.0.92/hak/one/number/int/width/to_text_colour.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/year/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/year/days/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/year/days/count/
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:36:03.000000 hak-0.0.92/hak/one/number/int/year/days/count/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/number/int/year/days/first/
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:36:10.000000 hak-0.0.92/hak/one/number/int/year/days/first/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      431 2023-07-06 08:36:18.000000 hak-0.0.92/hak/one/number/int/year/days/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      916 2023-07-10 13:23:34.000000 hak-0.0.92/hak/one/number/int/year/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      153 2023-07-06 08:36:26.000000 hak-0.0.92/hak/one/number/int/year/now.py
--rw-rw-r--   0 q         (1000) q         (1000)      824 2023-07-14 04:32:30.000000 hak-0.0.92/hak/one/number/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      123 2023-07-06 08:36:33.000000 hak-0.0.92/hak/one/number/log_2.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/period/
--rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:36:40.000000 hak-0.0.92/hak/one/period/contains_day.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/schedule/
--rw-rw-r--   0 q         (1000) q         (1000)     3465 2023-07-06 08:36:48.000000 hak-0.0.92/hak/one/schedule/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/session/
--rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 08:36:55.000000 hak-0.0.92/hak/one/session/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/set/
--rw-rw-r--   0 q         (1000) q         (1000)      114 2023-07-06 08:37:03.000000 hak-0.0.92/hak/one/set/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:37:10.000000 hak-0.0.92/hak/one/string/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/alphanumeric/
--rw-rw-r--   0 q         (1000) q         (1000)      264 2023-07-06 08:37:18.000000 hak-0.0.92/hak/one/string/alphanumeric/fake.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/append/
--rw-rw-r--   0 q         (1000) q         (1000)       54 2023-07-06 08:37:25.000000 hak-0.0.92/hak/one/string/append/new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      549 2023-07-06 08:37:33.000000 hak-0.0.92/hak/one/string/camel_to_snake.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/char/
--rw-rw-r--   0 q         (1000) q         (1000)      326 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/char/find_all_indices.py
--rw-rw-r--   0 q         (1000) q         (1000)      128 2023-07-06 08:37:47.000000 hak-0.0.92/hak/one/string/char/is_digit.py
--rw-rw-r--   0 q         (1000) q         (1000)      207 2023-07-06 08:37:55.000000 hak-0.0.92/hak/one/string/char/is_upper.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/char/last/
--rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-06 08:38:02.000000 hak-0.0.92/hak/one/string/char/last/find.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.887895 hak-0.0.92/hak/one/string/chars/
--rw-rw-r--   0 q         (1000) q         (1000)      561 2023-07-06 08:38:10.000000 hak-0.0.92/hak/one/string/chars/remove.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/colour/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:38:17.000000 hak-0.0.92/hak/one/string/colour/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/colour/bright/
--rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:25.000000 hak-0.0.92/hak/one/string/colour/bright/blue.py
--rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:32.000000 hak-0.0.92/hak/one/string/colour/bright/cyan.py
--rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:38:40.000000 hak-0.0.92/hak/one/string/colour/bright/green.py
--rw-rw-r--   0 q         (1000) q         (1000)      172 2023-07-06 08:38:47.000000 hak-0.0.92/hak/one/string/colour/bright/magenta.py
--rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 08:38:55.000000 hak-0.0.92/hak/one/string/colour/bright/red.py
--rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:39:02.000000 hak-0.0.92/hak/one/string/colour/bright/white.py
--rw-rw-r--   0 q         (1000) q         (1000)      170 2023-07-06 08:39:10.000000 hak-0.0.92/hak/one/string/colour/bright/yellow.py
--rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 08:39:17.000000 hak-0.0.92/hak/one/string/colour/danger.py
--rw-rw-r--   0 q         (1000) q         (1000)      178 2023-07-06 08:39:25.000000 hak-0.0.92/hak/one/string/colour/danger_if_zero.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/colour/dark/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:39:32.000000 hak-0.0.92/hak/one/string/colour/dark/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:40.000000 hak-0.0.92/hak/one/string/colour/dark/blue.py
--rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:47.000000 hak-0.0.92/hak/one/string/colour/dark/cyan.py
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:39:55.000000 hak-0.0.92/hak/one/string/colour/dark/default.py
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:03.000000 hak-0.0.92/hak/one/string/colour/dark/green.py
--rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:40:10.000000 hak-0.0.92/hak/one/string/colour/dark/magenta.py
--rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-06 08:40:18.000000 hak-0.0.92/hak/one/string/colour/dark/red.py
--rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:25.000000 hak-0.0.92/hak/one/string/colour/dark/white.py
--rw-rw-r--   0 q         (1000) q         (1000)      156 2023-07-06 08:40:33.000000 hak-0.0.92/hak/one/string/colour/dark/yellow.py
--rw-rw-r--   0 q         (1000) q         (1000)       64 2023-07-06 08:40:40.000000 hak-0.0.92/hak/one/string/colour/data.py
--rw-rw-r--   0 q         (1000) q         (1000)     3430 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/colour/decolour.py
--rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:47.000000 hak-0.0.92/hak/one/string/colour/info.py
--rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:55.000000 hak-0.0.92/hak/one/string/colour/primary.py
--rw-rw-r--   0 q         (1000) q         (1000)     2321 2023-07-06 08:41:02.000000 hak-0.0.92/hak/one/string/colour/rainbow.py
--rw-rw-r--   0 q         (1000) q         (1000)      138 2023-07-06 08:41:10.000000 hak-0.0.92/hak/one/string/colour/secondary.py
--rw-rw-r--   0 q         (1000) q         (1000)      275 2023-07-06 08:41:17.000000 hak-0.0.92/hak/one/string/colour/tgfr.py
--rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:41:25.000000 hak-0.0.92/hak/one/string/colour/warning.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/contains/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:32.000000 hak-0.0.92/hak/one/string/contains/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/contains/function/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:40.000000 hak-0.0.92/hak/one/string/contains/function/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 08:41:47.000000 hak-0.0.92/hak/one/string/contains/function/run.py
--rw-rw-r--   0 q         (1000) q         (1000)      192 2023-07-07 05:12:17.000000 hak-0.0.92/hak/one/string/contains/function/test.py
--rw-rw-r--   0 q         (1000) q         (1000)      224 2023-07-06 08:42:02.000000 hak-0.0.92/hak/one/string/contains/l.py
--rw-rw-r--   0 q         (1000) q         (1000)       76 2023-07-06 08:42:10.000000 hak-0.0.92/hak/one/string/contains/version.py
--rw-rw-r--   0 q         (1000) q         (1000)      105 2023-07-06 08:42:17.000000 hak-0.0.92/hak/one/string/count_x_in_y.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/date/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/date/separator/
--rw-rw-r--   0 q         (1000) q         (1000)      923 2023-07-10 13:23:48.000000 hak-0.0.92/hak/one/string/date/separator/get.py
--rw-rw-r--   0 q         (1000) q         (1000)     1924 2023-07-10 14:58:52.000000 hak-0.0.92/hak/one/string/date/to_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/day/
--rw-rw-r--   0 q         (1000) q         (1000)     1076 2023-07-10 13:25:17.000000 hak-0.0.92/hak/one/string/day/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-06 08:42:32.000000 hak-0.0.92/hak/one/string/delete_character_safely.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/digits/
--rw-rw-r--   0 q         (1000) q         (1000)      206 2023-07-06 08:42:40.000000 hak-0.0.92/hak/one/string/digits/remove.py
--rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:42:47.000000 hak-0.0.92/hak/one/string/double_single_quotes.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/family_name/
--rw-rw-r--   0 q         (1000) q         (1000)   121166 2023-07-07 04:10:06.000000 hak-0.0.92/hak/one/string/family_name/fake.py
--rw-rw-r--   0 q         (1000) q         (1000)      303 2023-07-06 08:43:10.000000 hak-0.0.92/hak/one/string/family_name/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/filename/
--rw-rw-r--   0 q         (1000) q         (1000)      126 2023-07-06 08:43:25.000000 hak-0.0.92/hak/one/string/filename/to_module_name.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/filepath/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:43:32.000000 hak-0.0.92/hak/one/string/filepath/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/filepath/py/
--rw-rw-r--   0 q         (1000) q         (1000)      720 2023-07-06 08:43:39.000000 hak-0.0.92/hak/one/string/filepath/py/get_t.py
--rw-rw-r--   0 q         (1000) q         (1000)      100 2023-07-06 08:43:47.000000 hak-0.0.92/hak/one/string/find_first_parenthesis.py
--rw-rw-r--   0 q         (1000) q         (1000)      213 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/find_last_comma_index.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/fn_name/
--rw-rw-r--   0 q         (1000) q         (1000)      226 2023-07-06 08:44:02.000000 hak-0.0.92/hak/one/string/fn_name/is_ignorable.py
--rw-rw-r--   0 q         (1000) q         (1000)     5035 2023-07-06 08:44:09.000000 hak-0.0.92/hak/one/string/format.py
--rw-rw-r--   0 q         (1000) q         (1000)       73 2023-07-06 08:44:17.000000 hak-0.0.92/hak/one/string/has_at_symbol.py
--rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:24.000000 hak-0.0.92/hak/one/string/has_digit.py
--rw-rw-r--   0 q         (1000) q         (1000)      131 2023-07-06 08:44:32.000000 hak-0.0.92/hak/one/string/has_lowercase.py
--rw-rw-r--   0 q         (1000) q         (1000)      263 2023-07-06 08:44:39.000000 hak-0.0.92/hak/one/string/has_other_char.py
--rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:44:47.000000 hak-0.0.92/hak/one/string/has_seven_digits.py
--rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:54.000000 hak-0.0.92/hak/one/string/has_uppercase.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/hbar/
--rw-rw-r--   0 q         (1000) q         (1000)      122 2023-07-06 08:45:02.000000 hak-0.0.92/hak/one/string/hbar/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/string/header/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/header/python_file/
--rw-rw-r--   0 q         (1000) q         (1000)      322 2023-07-06 08:45:09.000000 hak-0.0.92/hak/one/string/header/python_file/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/header/test_table/
--rw-rw-r--   0 q         (1000) q         (1000)      461 2023-07-06 08:45:17.000000 hak-0.0.92/hak/one/string/header/test_table/make.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/indent/
--rw-rw-r--   0 q         (1000) q         (1000)      137 2023-07-06 08:45:25.000000 hak-0.0.92/hak/one/string/indent/run_if_class_method.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/insert/
--rw-rw-r--   0 q         (1000) q         (1000)      602 2023-07-06 08:45:32.000000 hak-0.0.92/hak/one/string/insert/new_line_after_last_import_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      278 2023-07-06 08:45:40.000000 hak-0.0.92/hak/one/string/insert/new_line_before_comment.py
--rw-rw-r--   0 q         (1000) q         (1000)      584 2023-07-06 08:45:48.000000 hak-0.0.92/hak/one/string/insert/new_line_before_def.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:45:56.000000 hak-0.0.92/hak/one/string/insert/new_line_before_if_main.py
--rw-rw-r--   0 q         (1000) q         (1000)      670 2023-07-06 08:46:04.000000 hak-0.0.92/hak/one/string/insert/new_line_before_lambda.py
--rw-rw-r--   0 q         (1000) q         (1000)      292 2023-07-06 08:46:12.000000 hak-0.0.92/hak/one/string/insert/new_line_before_new_line_and_cea_.py
--rw-rw-r--   0 q         (1000) q         (1000)      102 2023-07-06 08:46:20.000000 hak-0.0.92/hak/one/string/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      124 2023-07-06 08:46:27.000000 hak-0.0.92/hak/one/string/is_or_none.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/json/
--rw-rw-r--   0 q         (1000) q         (1000)      179 2023-07-06 08:46:35.000000 hak-0.0.92/hak/one/string/json/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      552 2023-07-06 08:46:42.000000 hak-0.0.92/hak/one/string/lambdarise.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/string/line/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/string/line/last/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/line/last/length/
--rw-rw-r--   0 q         (1000) q         (1000)      423 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/line/last/length/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      368 2023-07-06 08:46:58.000000 hak-0.0.92/hak/one/string/make_content_without_function.py
--rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:47:06.000000 hak-0.0.92/hak/one/string/make_function_text.py
--rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-06 08:47:13.000000 hak-0.0.92/hak/one/string/make_initial_content.py
--rw-rw-r--   0 q         (1000) q         (1000)      327 2023-07-06 08:47:21.000000 hak-0.0.92/hak/one/string/make_new_function_text.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/money/
--rw-rw-r--   0 q         (1000) q         (1000)      541 2023-07-10 13:25:31.000000 hak-0.0.92/hak/one/string/money/to_float.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/month/
--rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-10 13:25:45.000000 hak-0.0.92/hak/one/string/month/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      559 2023-07-10 14:58:57.000000 hak-0.0.92/hak/one/string/month/to_number.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/nest_level/
--rw-rw-r--   0 q         (1000) q         (1000)      688 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/nest_level/get.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/password/
--rw-rw-r--   0 q         (1000) q         (1000)     1187 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/password/create.py
--rw-rw-r--   0 q         (1000) q         (1000)      555 2023-07-06 08:47:50.000000 hak-0.0.92/hak/one/string/password/has_chars_from_3_sets.py
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/pop_left.py
--rw-rw-r--   0 q         (1000) q         (1000)      223 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/pop_right.py
--rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:48:13.000000 hak-0.0.92/hak/one/string/prepend_import.py
--rw-rw-r--   0 q         (1000) q         (1000)      756 2023-07-06 08:48:20.000000 hak-0.0.92/hak/one/string/print_and_return_false.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/refactor/
--rw-rw-r--   0 q         (1000) q         (1000)     1218 2023-07-06 08:48:28.000000 hak-0.0.92/hak/one/string/refactor/by_two_char_combinations.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/remove/
--rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:48:35.000000 hak-0.0.92/hak/one/string/remove/empty_line_spaces.py
--rw-rw-r--   0 q         (1000) q         (1000)      162 2023-07-06 08:48:42.000000 hak-0.0.92/hak/one/string/remove/empty_lines.py
--rw-rw-r--   0 q         (1000) q         (1000)      441 2023-07-06 08:48:50.000000 hak-0.0.92/hak/one/string/remove/extra_new_line_following_class_definition.py
--rw-rw-r--   0 q         (1000) q         (1000)      210 2023-07-06 08:48:57.000000 hak-0.0.92/hak/one/string/remove/first_new_line_if_starts_with_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)       81 2023-07-06 08:49:04.000000 hak-0.0.92/hak/one/string/remove/whitespace_between_newlines.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/replace/
--rw-rw-r--   0 q         (1000) q         (1000)      241 2023-07-06 08:49:12.000000 hak-0.0.92/hak/one/string/replace/double_new_line_with_single_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      129 2023-07-06 08:49:20.000000 hak-0.0.92/hak/one/string/replace/single_new_line_with_empty_string.py
--rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:49:27.000000 hak-0.0.92/hak/one/string/replace/triple_new_line_with_double_new_line.py
--rw-rw-r--   0 q         (1000) q         (1000)      487 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/string/replace_unprintable.py
--rw-rw-r--   0 q         (1000) q         (1000)     3365 2023-07-06 08:49:42.000000 hak-0.0.92/hak/one/string/separate_function_from_context.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/single_line_function/
--rw-rw-r--   0 q         (1000) q         (1000)      432 2023-07-06 08:49:49.000000 hak-0.0.92/hak/one/string/single_line_function/is_a.py
--rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 08:49:57.000000 hak-0.0.92/hak/one/string/single_line_function/to_lambda_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/spaces/
--rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:50:05.000000 hak-0.0.92/hak/one/string/spaces/count.py
--rw-rw-r--   0 q         (1000) q         (1000)      331 2023-07-06 08:50:12.000000 hak-0.0.92/hak/one/string/split_fn_name_and_text.py
--rw-rw-r--   0 q         (1000) q         (1000)      344 2023-07-06 08:50:20.000000 hak-0.0.92/hak/one/string/strip_unprintable.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/table/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:43.000000 hak-0.0.92/hak/one/string/table/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/table/bar/
--rw-rw-r--   0 q         (1000) q         (1000)      363 2023-07-17 06:41:04.000000 hak-0.0.92/hak/one/string/table/bar/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      265 2023-07-06 08:50:27.000000 hak-0.0.92/hak/one/string/to_cond_freq_dict.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/token/
--rw-rw-r--   0 q         (1000) q         (1000)     1263 2023-07-06 08:50:35.000000 hak-0.0.92/hak/one/string/token/substitute.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/year/
--rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-10 13:26:13.000000 hak-0.0.92/hak/one/string/year/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/string/yyyymmdd/
--rw-rw-r--   0 q         (1000) q         (1000)      238 2023-07-06 08:50:42.000000 hak-0.0.92/hak/one/string/yyyymmdd/to_date.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/one/subprocess/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/subprocess/completed_process/
--rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-07 01:06:09.000000 hak-0.0.92/hak/one/subprocess/completed_process/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/system/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:50:57.000000 hak-0.0.92/hak/one/system/__init__.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/system/git/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/system/git/commit/
--rw-rw-r--   0 q         (1000) q         (1000)     2527 2023-07-06 08:51:35.000000 hak-0.0.92/hak/one/system/git/commit/run.py
--rw-rw-r--   0 q         (1000) q         (1000)      393 2023-07-06 08:51:42.000000 hak-0.0.92/hak/one/system/git/commit_if_test_and_app_ok.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/system/git/gitignore/
--rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-06 08:51:51.000000 hak-0.0.92/hak/one/system/git/gitignore/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      485 2023-07-07 01:09:02.000000 hak-0.0.92/hak/one/system/git/init.py
--rw-rw-r--   0 q         (1000) q         (1000)      745 2023-07-06 08:52:07.000000 hak-0.0.92/hak/one/system/git/log_oneline.py
--rw-rw-r--   0 q         (1000) q         (1000)      870 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/system/git/push_after_delay.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/system/screen/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:52:21.000000 hak-0.0.92/hak/one/system/screen/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)      786 2023-07-06 08:52:29.000000 hak-0.0.92/hak/one/system/screen/clear.py
--rw-rw-r--   0 q         (1000) q         (1000)     3127 2023-07-10 13:03:40.000000 hak-0.0.92/hak/one/terminal.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/one/tup/
--rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:52:44.000000 hak-0.0.92/hak/one/tup/is_a.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/other/
--rw-rw-r--   0 q         (1000) q         (1000)      430 2023-07-07 01:09:29.000000 hak-0.0.92/hak/other/l.py
--rw-rw-r--   0 q         (1000) q         (1000)       91 2023-07-06 08:52:59.000000 hak-0.0.92/hak/other/nop_state_x.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.891896 hak-0.0.92/hak/other/patch/
--rw-rw-r--   0 q         (1000) q         (1000)     7954 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/patch/do.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/pip/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/pip/dist_tar/
--rw-rw-r--   0 q         (1000) q         (1000)     3093 2023-07-10 13:27:41.000000 hak-0.0.92/hak/other/pip/dist_tar/make.py
--rw-rw-r--   0 q         (1000) q         (1000)      805 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/pip/dist_tar/remove.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/pip/setup/
--rw-rw-r--   0 q         (1000) q         (1000)     1321 2023-07-06 08:53:29.000000 hak-0.0.92/hak/other/pip/setup/update.py
--rw-rw-r--   0 q         (1000) q         (1000)     1808 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/pip/upload.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/pip/version/
--rw-rw-r--   0 q         (1000) q         (1000)      897 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/pip/version/get.py
--rw-rw-r--   0 q         (1000) q         (1000)      120 2023-07-06 22:28:42.000000 hak-0.0.92/hak/other/pip/version/to_str.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/report/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/report/fail/
--rw-rw-r--   0 q         (1000) q         (1000)      822 2023-07-06 22:28:49.000000 hak-0.0.92/hak/other/report/fail/no_xyz.py
--rw-rw-r--   0 q         (1000) q         (1000)     1936 2023-07-06 22:28:57.000000 hak-0.0.92/hak/other/report/fail/xyz.py
--rw-rw-r--   0 q         (1000) q         (1000)     1462 2023-07-06 22:29:04.000000 hak-0.0.92/hak/other/report/fail/z_return_neq_y_return.py
--rw-rw-r--   0 q         (1000) q         (1000)     1623 2023-07-06 22:29:12.000000 hak-0.0.92/hak/other/report/fail/z_stdo_neq_y_stdo.py
--rw-rw-r--   0 q         (1000) q         (1000)      895 2023-07-06 22:29:19.000000 hak-0.0.92/hak/other/report/property_failure.py
--rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 22:29:27.000000 hak-0.0.92/hak/other/report/success.py
--rw-rw-r--   0 q         (1000) q         (1000)      394 2023-07-06 22:29:34.000000 hak-0.0.92/hak/other/report/summarise_file.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.875895 hak-0.0.92/hak/other/setup/
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/setup/cfg/
--rw-rw-r--   0 q         (1000) q         (1000)     1547 2023-07-06 22:29:41.000000 hak-0.0.92/hak/other/setup/cfg/update.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/other/setup/py/
--rw-rw-r--   0 q         (1000) q         (1000)     1653 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/setup/py/update.py
--rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-10 13:03:40.000000 hak-0.0.92/hak/other/ternary.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/pair/
--rw-rw-r--   0 q         (1000) q         (1000)      140 2023-07-06 22:30:04.000000 hak-0.0.92/hak/pair/eq.py
--rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-10 13:03:46.000000 hak-0.0.92/hak/pxyz.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/
--rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.92/hak/test/__init__.py
--rw-rw-r--   0 q         (1000) q         (1000)     2658 2023-07-06 06:52:54.000000 hak-0.0.92/hak/test/do.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/failed/
--rw-rw-r--   0 q         (1000) q         (1000)     1112 2023-07-06 06:53:05.000000 hak-0.0.92/hak/test/failed/handle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/final_line/
--rw-rw-r--   0 q         (1000) q         (1000)     2531 2023-07-10 13:03:40.000000 hak-0.0.92/hak/test/final_line/check.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/line_lengths/
--rw-rw-r--   0 q         (1000) q         (1000)     2717 2023-07-10 13:03:40.000000 hak-0.0.92/hak/test/line_lengths/check.py
--rw-rw-r--   0 q         (1000) q         (1000)      790 2023-07-10 13:03:40.000000 hak-0.0.92/hak/test/line_lengths_check.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/oldest_file/
--rw-rw-r--   0 q         (1000) q         (1000)     4789 2023-07-10 13:03:40.000000 hak-0.0.92/hak/test/oldest_file/print.py
--rw-rw-r--   0 q         (1000) q         (1000)      937 2023-07-06 06:53:55.000000 hak-0.0.92/hak/test/oldest_file_print.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.895896 hak-0.0.92/hak/test/passed/
--rw-rw-r--   0 q         (1000) q         (1000)      961 2023-07-06 06:54:05.000000 hak-0.0.92/hak/test/passed/handle.py
-drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 06:42:04.879895 hak-0.0.92/hak.egg-info/
--rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-17 06:42:04.000000 hak-0.0.92/hak.egg-info/PKG-INFO
--rw-rw-r--   0 q         (1000) q         (1000)    12798 2023-07-17 06:42:04.000000 hak-0.0.92/hak.egg-info/SOURCES.txt
--rw-rw-r--   0 q         (1000) q         (1000)        1 2023-07-17 06:42:04.000000 hak-0.0.92/hak.egg-info/dependency_links.txt
--rw-rw-r--   0 q         (1000) q         (1000)     3372 2023-07-17 06:42:04.000000 hak-0.0.92/hak.egg-info/top_level.txt
--rw-rw-r--   0 q         (1000) q         (1000)      537 2023-07-17 06:42:04.895896 hak-0.0.92/setup.cfg
--rw-rw-r--   0 q         (1000) q         (1000)      576 2023-07-17 06:42:04.000000 hak-0.0.92/setup.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/
+-rw-rw-r--   0 q         (1000) q         (1000)     1068 2023-07-07 13:22:08.000000 hak-0.0.93/LICENSE
+-rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-17 10:49:56.684413 hak-0.0.93/PKG-INFO
+-rw-rw-r--   0 q         (1000) q         (1000)      583 2023-07-10 13:04:07.000000 hak-0.0.93/README.md
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 04:34:17.000000 hak-0.0.93/hak/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/data/
+-rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-04 23:50:58.000000 hak-0.0.93/hak/data/months.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/fake/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.93/hak/fake/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/fake/os/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.93/hak/fake/os/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      418 2023-04-23 03:18:31.000000 hak-0.0.93/hak/fake/os/system.py
+-rw-rw-r--   0 q         (1000) q         (1000)      424 2023-04-23 03:18:31.000000 hak-0.0.93/hak/fake/printer.py
+-rw-rw-r--   0 q         (1000) q         (1000)       45 2023-04-23 03:18:31.000000 hak-0.0.93/hak/fake/sleep.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/fake/subprocess/
+-rw-rw-r--   0 q         (1000) q         (1000)     5858 2023-07-06 06:52:44.000000 hak-0.0.93/hak/fake/subprocess/run.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.664413 hak-0.0.93/hak/many/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/bools/
+-rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 06:52:37.000000 hak-0.0.93/hak/many/bools/count_true.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/dicts/
+-rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 06:52:47.000000 hak-0.0.93/hak/many/dicts/a_into_b.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1136 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/dicts/compare.py
+-rw-rw-r--   0 q         (1000) q         (1000)      911 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/dicts/compare_relevant_only.py
+-rw-rw-r--   0 q         (1000) q         (1000)      797 2023-07-10 13:05:10.000000 hak-0.0.93/hak/many/dicts/convert_date_strings_to_dates.py
+-rw-rw-r--   0 q         (1000) q         (1000)      306 2023-07-17 06:38:48.000000 hak-0.0.93/hak/many/dicts/get_all_keys.py
+-rw-rw-r--   0 q         (1000) q         (1000)      666 2023-07-17 06:38:53.000000 hak-0.0.93/hak/many/dicts/get_datatypes.py
+-rw-rw-r--   0 q         (1000) q         (1000)      493 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/dicts/get_first_and_last_dates.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1429 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/dicts/get_keys_with_none_or_zero_vals.py
+-rw-rw-r--   0 q         (1000) q         (1000)      199 2023-07-06 06:53:17.000000 hak-0.0.93/hak/many/dicts/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      663 2023-07-06 06:53:28.000000 hak-0.0.93/hak/many/dicts/merge_freq_dicts.py
+-rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 06:53:38.000000 hak-0.0.93/hak/many/dicts/reindex.py
+-rw-rw-r--   0 q         (1000) q         (1000)      203 2023-07-06 06:53:48.000000 hak-0.0.93/hak/many/dicts/sort_by_key.py
+-rw-rw-r--   0 q         (1000) q         (1000)      384 2023-07-10 13:05:47.000000 hak-0.0.93/hak/many/dicts/sum_by_key.py
+-rw-rw-r--   0 q         (1000) q         (1000)    10015 2023-07-17 06:38:58.000000 hak-0.0.93/hak/many/dicts/to_table.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/directories/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/directories/empty/
+-rw-rw-r--   0 q         (1000) q         (1000)      701 2023-07-10 13:07:02.000000 hak-0.0.93/hak/many/directories/empty/find.py
+-rw-rw-r--   0 q         (1000) q         (1000)      649 2023-07-10 13:07:36.000000 hak-0.0.93/hak/many/directories/empty/remove.py
+-rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 06:54:08.000000 hak-0.0.93/hak/many/directories/exist.py
+-rw-rw-r--   0 q         (1000) q         (1000)      606 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/directories/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      440 2023-07-07 05:17:37.000000 hak-0.0.93/hak/many/directories/make.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.664413 hak-0.0.93/hak/many/files/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/files/pyfiles/
+-rw-rw-r--   0 q         (1000) q         (1000)     1789 2023-07-06 06:54:28.000000 hak-0.0.93/hak/many/files/pyfiles/dismantle.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/lists/
+-rw-rw-r--   0 q         (1000) q         (1000)      216 2023-07-06 06:54:38.000000 hak-0.0.93/hak/many/lists/merge.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/numbers/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:09:58.000000 hak-0.0.93/hak/many/numbers/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/numbers/ints/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 02:11:47.000000 hak-0.0.93/hak/many/numbers/ints/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/numbers/ints/mode/
+-rw-rw-r--   0 q         (1000) q         (1000)      405 2023-07-10 13:08:08.000000 hak-0.0.93/hak/many/numbers/ints/mode/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      148 2023-07-10 12:30:14.000000 hak-0.0.93/hak/many/numbers/ints/remove_zeroes.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/pyfiles/
+-rw-rw-r--   0 q         (1000) q         (1000)      161 2023-07-06 06:54:46.000000 hak-0.0.93/hak/many/pyfiles/format.py
+-rw-rw-r--   0 q         (1000) q         (1000)      847 2023-07-06 06:54:53.000000 hak-0.0.93/hak/many/pyfiles/format_and_commit.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/strings/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:00.000000 hak-0.0.93/hak/many/strings/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      130 2023-07-06 06:55:08.000000 hak-0.0.93/hak/many/strings/add_src_funks_prefix.py
+-rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-06 06:55:15.000000 hak-0.0.93/hak/many/strings/compare.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/many/strings/contain/
+-rw-rw-r--   0 q         (1000) q         (1000)      145 2023-07-06 06:55:23.000000 hak-0.0.93/hak/many/strings/contain/version.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/date_pieces/
+-rw-rw-r--   0 q         (1000) q         (1000)      676 2023-07-10 13:09:01.000000 hak-0.0.93/hak/many/strings/date_pieces/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3832 2023-07-10 13:10:37.000000 hak-0.0.93/hak/many/strings/date_pieces/separate_day.py
+-rw-rw-r--   0 q         (1000) q         (1000)      834 2023-07-10 13:12:11.000000 hak-0.0.93/hak/many/strings/date_pieces/separate_year.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/dates/
+-rw-rw-r--   0 q         (1000) q         (1000)     3259 2023-07-10 13:12:55.000000 hak-0.0.93/hak/many/strings/dates/detect_format.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/filepaths/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:55:30.000000 hak-0.0.93/hak/many/strings/filepaths/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1238 2023-07-10 13:15:48.000000 hak-0.0.93/hak/many/strings/filepaths/get_least_recently_modified.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1196 2023-07-10 13:16:18.000000 hak-0.0.93/hak/many/strings/filepaths/get_most_recently_modified.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/filepaths/py/
+-rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-06 06:55:37.000000 hak-0.0.93/hak/many/strings/filepaths/py/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/filepaths/py/testables/
+-rw-rw-r--   0 q         (1000) q         (1000)     2077 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/strings/filepaths/py/testables/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      660 2023-07-06 06:55:52.000000 hak-0.0.93/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py
+-rw-rw-r--   0 q         (1000) q         (1000)     2234 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/strings/find_first_diff.py
+-rw-rw-r--   0 q         (1000) q         (1000)      291 2023-07-10 13:16:37.000000 hak-0.0.93/hak/many/strings/get_index_of_first_difference.py
+-rw-rw-r--   0 q         (1000) q         (1000)      444 2023-07-06 06:56:07.000000 hak-0.0.93/hak/many/strings/make_patch_version_change_to_py.py
+-rw-rw-r--   0 q         (1000) q         (1000)      297 2023-07-06 06:56:14.000000 hak-0.0.93/hak/many/strings/module_names_from_py_filenames.py
+-rw-rw-r--   0 q         (1000) q         (1000)      416 2023-07-06 06:56:22.000000 hak-0.0.93/hak/many/strings/patch_setup_cfg.py
+-rw-rw-r--   0 q         (1000) q         (1000)      632 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/strings/patch_setup_py.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/strings/pyfiles/
+-rw-rw-r--   0 q         (1000) q         (1000)     1514 2023-07-06 06:56:37.000000 hak-0.0.93/hak/many/strings/pyfiles/filter_out_items.py
+-rw-rw-r--   0 q         (1000) q         (1000)      782 2023-07-10 13:03:40.000000 hak-0.0.93/hak/many/strings/show_diff.py
+-rw-rw-r--   0 q         (1000) q         (1000)      667 2023-07-06 06:56:51.000000 hak-0.0.93/hak/many/strings/to_dict.py
+-rw-rw-r--   0 q         (1000) q         (1000)      357 2023-07-06 06:56:59.000000 hak-0.0.93/hak/many/strings/two_char_combinations.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/tuples/
+-rw-rw-r--   0 q         (1000) q         (1000)      261 2023-07-10 13:16:50.000000 hak-0.0.93/hak/many/tuples/to_dict.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/many/values/
+-rw-rw-r--   0 q         (1000) q         (1000)     2157 2023-07-17 06:39:03.000000 hak-0.0.93/hak/many/values/get_datatype.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/none/
+-rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 06:57:14.000000 hak-0.0.93/hak/none/nop.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/bool/
+-rw-rw-r--   0 q         (1000) q         (1000)       86 2023-07-06 06:57:21.000000 hak-0.0.93/hak/one/bool/fake.py
+-rw-rw-r--   0 q         (1000) q         (1000)      103 2023-07-06 06:57:28.000000 hak-0.0.93/hak/one/bool/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/bool/or_none/
+-rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 06:57:36.000000 hak-0.0.93/hak/one/bool/or_none/fake.py
+-rw-rw-r--   0 q         (1000) q         (1000)      125 2023-07-06 06:57:43.000000 hak-0.0.93/hak/one/bool/or_none/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      762 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/check_if_ok_to_proceed.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/date/
+-rw-rw-r--   0 q         (1000) q         (1000)      143 2023-07-06 06:57:58.000000 hak-0.0.93/hak/one/date/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      347 2023-07-06 06:58:06.000000 hak-0.0.93/hak/one/date/is_first_second_or_third_day_of_month.py
+-rw-rw-r--   0 q         (1000) q         (1000)      414 2023-07-06 06:58:13.000000 hak-0.0.93/hak/one/date/is_first_week_of_quarter.py
+-rw-rw-r--   0 q         (1000) q         (1000)      208 2023-07-06 06:58:20.000000 hak-0.0.93/hak/one/date/is_monday.py
+-rw-rw-r--   0 q         (1000) q         (1000)      462 2023-07-06 06:58:28.000000 hak-0.0.93/hak/one/date/is_weekday.py
+-rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 06:58:35.000000 hak-0.0.93/hak/one/date/is_weekend.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/date/public_holiday/
+-rw-rw-r--   0 q         (1000) q         (1000)     4981 2023-07-10 13:17:27.000000 hak-0.0.93/hak/one/date/public_holiday/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 06:58:50.000000 hak-0.0.93/hak/one/date/select_from_last_n_days.py
+-rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 06:58:57.000000 hak-0.0.93/hak/one/date/to_dd_mm_yyyy_str.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1216 2023-07-10 13:17:49.000000 hak-0.0.93/hak/one/date/to_financial_year.py
+-rw-rw-r--   0 q         (1000) q         (1000)      609 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/date/to_utc_timestamp.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.664413 hak-0.0.93/hak/one/date/year/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/date/year/easter_sunday/
+-rw-rw-r--   0 q         (1000) q         (1000)      940 2023-07-10 13:18:07.000000 hak-0.0.93/hak/one/date/year/easter_sunday/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/datetime/
+-rw-rw-r--   0 q         (1000) q         (1000)      149 2023-07-06 06:59:20.000000 hak-0.0.93/hak/one/datetime/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      272 2023-07-06 06:59:27.000000 hak-0.0.93/hak/one/datetime/select_from_last_n_days.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:34.000000 hak-0.0.93/hak/one/dict/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/cell/
+-rw-rw-r--   0 q         (1000) q         (1000)     2118 2023-07-17 06:39:08.000000 hak-0.0.93/hak/one/dict/cell/get_width.py
+-rw-rw-r--   0 q         (1000) q         (1000)     2595 2023-07-17 06:39:13.000000 hak-0.0.93/hak/one/dict/cell/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1474 2023-07-17 06:39:17.000000 hak-0.0.93/hak/one/dict/cell/to_str.py
+-rw-rw-r--   0 q         (1000) q         (1000)      219 2023-07-06 06:59:42.000000 hak-0.0.93/hak/one/dict/convert_to_sql_insertable.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/custom_order/
+-rw-rw-r--   0 q         (1000) q         (1000)      384 2023-07-17 06:39:22.000000 hak-0.0.93/hak/one/dict/custom_order/apply.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/durations/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 06:59:49.000000 hak-0.0.93/hak/one/dict/durations/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1147 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/durations/load.py
+-rw-rw-r--   0 q         (1000) q         (1000)      800 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/durations/save.py
+-rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 07:00:12.000000 hak-0.0.93/hak/one/dict/durations/to_tuple_list_sorted_by_duration.py
+-rw-rw-r--   0 q         (1000) q         (1000)      769 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/durations/update_one.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/frequencies/
+-rw-rw-r--   0 q         (1000) q         (1000)      519 2023-07-06 07:00:27.000000 hak-0.0.93/hak/one/dict/frequencies/choose.py
+-rw-rw-r--   0 q         (1000) q         (1000)      385 2023-07-06 07:00:35.000000 hak-0.0.93/hak/one/dict/frequencies/make_from_strings.py
+-rw-rw-r--   0 q         (1000) q         (1000)      187 2023-07-06 07:00:42.000000 hak-0.0.93/hak/one/dict/get_or_default.py
+-rw-rw-r--   0 q         (1000) q         (1000)      616 2023-07-10 13:19:02.000000 hak-0.0.93/hak/one/dict/get_or_zero.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/header/
+-rw-rw-r--   0 q         (1000) q         (1000)     2425 2023-07-17 06:39:27.000000 hak-0.0.93/hak/one/dict/header/to_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/hidden_fields/
+-rw-rw-r--   0 q         (1000) q         (1000)      240 2023-07-17 06:39:32.000000 hak-0.0.93/hak/one/dict/hidden_fields/hide.py
+-rw-rw-r--   0 q         (1000) q         (1000)      190 2023-07-06 07:00:57.000000 hak-0.0.93/hak/one/dict/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 07:01:05.000000 hak-0.0.93/hak/one/dict/make_from_key_value_lists.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/period/
+-rw-rw-r--   0 q         (1000) q         (1000)     1016 2023-07-10 14:58:58.000000 hak-0.0.93/hak/one/dict/period/contains_date.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/period/financial_year/
+-rw-rw-r--   0 q         (1000) q         (1000)      896 2023-07-10 14:58:56.000000 hak-0.0.93/hak/one/dict/period/financial_year/contains_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/period/financial_year/ge.py
+-rw-rw-r--   0 q         (1000) q         (1000)      317 2023-07-10 14:58:55.000000 hak-0.0.93/hak/one/dict/period/financial_year/get_end_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)      589 2023-07-10 14:58:54.000000 hak-0.0.93/hak/one/dict/period/financial_year/get_start_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/period/financial_year/gt.py
+-rw-rw-r--   0 q         (1000) q         (1000)      388 2023-07-10 13:04:13.000000 hak-0.0.93/hak/one/dict/period/financial_year/increment.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1415 2023-07-10 13:06:36.000000 hak-0.0.93/hak/one/dict/period/financial_year/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      866 2023-07-10 13:07:10.000000 hak-0.0.93/hak/one/dict/period/financial_year/le.py
+-rw-rw-r--   0 q         (1000) q         (1000)      856 2023-07-10 13:07:47.000000 hak-0.0.93/hak/one/dict/period/financial_year/leq.py
+-rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-10 13:08:14.000000 hak-0.0.93/hak/one/dict/period/financial_year/lt.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1733 2023-07-10 14:58:59.000000 hak-0.0.93/hak/one/dict/period/financial_year/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)      255 2023-07-10 13:11:06.000000 hak-0.0.93/hak/one/dict/period/financial_year/to_str.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1307 2023-07-10 14:58:54.000000 hak-0.0.93/hak/one/dict/period/get_end.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1457 2023-07-10 15:00:35.000000 hak-0.0.93/hak/one/dict/period/get_start.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/period/month/
+-rw-rw-r--   0 q         (1000) q         (1000)      460 2023-07-10 14:58:53.000000 hak-0.0.93/hak/one/dict/period/month/contains_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1179 2023-07-10 14:58:51.000000 hak-0.0.93/hak/one/dict/period/month/get_end_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-10 14:58:50.000000 hak-0.0.93/hak/one/dict/period/month/get_start_date.py
+-rw-rw-r--   0 q         (1000) q         (1000)      283 2023-07-10 13:20:49.000000 hak-0.0.93/hak/one/dict/pick_by_keys.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.672413 hak-0.0.93/hak/one/dict/proposed_dismantlement/
+-rw-rw-r--   0 q         (1000) q         (1000)     1544 2023-07-06 07:01:20.000000 hak-0.0.93/hak/one/dict/proposed_dismantlement/show.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/rate/
+-rw-rw-r--   0 q         (1000) q         (1000)      614 2023-07-17 06:39:37.000000 hak-0.0.93/hak/one/dict/rate/abs.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1388 2023-07-17 06:39:42.000000 hak-0.0.93/hak/one/dict/rate/add.py
+-rw-rw-r--   0 q         (1000) q         (1000)      884 2023-07-17 06:39:47.000000 hak-0.0.93/hak/one/dict/rate/div_number_by_rate.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1379 2023-07-17 06:39:51.000000 hak-0.0.93/hak/one/dict/rate/div_rate_by_rate.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1190 2023-07-17 06:39:56.000000 hak-0.0.93/hak/one/dict/rate/eq.py
+-rw-rw-r--   0 q         (1000) q         (1000)      755 2023-07-17 06:40:01.000000 hak-0.0.93/hak/one/dict/rate/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)     4623 2023-07-17 06:40:06.000000 hak-0.0.93/hak/one/dict/rate/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1033 2023-07-17 06:40:11.000000 hak-0.0.93/hak/one/dict/rate/mult_rate_by_number.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1321 2023-07-17 06:40:16.000000 hak-0.0.93/hak/one/dict/rate/mult_rate_by_rate.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1351 2023-07-17 06:40:21.000000 hak-0.0.93/hak/one/dict/rate/sub.py
+-rw-rw-r--   0 q         (1000) q         (1000)      597 2023-07-17 06:40:25.000000 hak-0.0.93/hak/one/dict/rate/to_float.py
+-rw-rw-r--   0 q         (1000) q         (1000)      643 2023-07-17 06:40:30.000000 hak-0.0.93/hak/one/dict/rate/to_num.py
+-rw-rw-r--   0 q         (1000) q         (1000)      323 2023-07-17 06:40:35.000000 hak-0.0.93/hak/one/dict/rate/to_str.py
+-rw-rw-r--   0 q         (1000) q         (1000)      241 2023-07-17 06:40:40.000000 hak-0.0.93/hak/one/dict/rate/to_str_frac.py
+-rw-rw-r--   0 q         (1000) q         (1000)      837 2023-07-17 06:40:45.000000 hak-0.0.93/hak/one/dict/remove_zeroes.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/table/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:26.000000 hak-0.0.93/hak/one/dict/table/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1344 2023-07-17 06:40:50.000000 hak-0.0.93/hak/one/dict/table/get_field_widths.py
+-rw-rw-r--   0 q         (1000) q         (1000)     4031 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/dict/to_max_line_width_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/unit/
+-rw-rw-r--   0 q         (1000) q         (1000)     1836 2023-07-17 10:49:27.000000 hak-0.0.93/hak/one/dict/unit/to_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/values/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:43.000000 hak-0.0.93/hak/one/dict/values/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/values/numbers/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:50.000000 hak-0.0.93/hak/one/dict/values/numbers/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/values/numbers/negative/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:02:58.000000 hak-0.0.93/hak/one/dict/values/numbers/negative/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:21:57.000000 hak-0.0.93/hak/one/dict/values/numbers/negative/count.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/dict/values/numbers/positive/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:13.000000 hak-0.0.93/hak/one/dict/values/numbers/positive/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      281 2023-07-10 13:22:10.000000 hak-0.0.93/hak/one/dict/values/numbers/positive/count.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/directory/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:03:28.000000 hak-0.0.93/hak/one/directory/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1568 2023-07-06 07:03:35.000000 hak-0.0.93/hak/one/directory/compress_to_tar.py
+-rw-rw-r--   0 q         (1000) q         (1000)      728 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/directory/empty.py
+-rw-rw-r--   0 q         (1000) q         (1000)       88 2023-07-06 07:03:51.000000 hak-0.0.93/hak/one/directory/exists.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/directory/filepaths/
+-rw-rw-r--   0 q         (1000) q         (1000)     1463 2023-07-10 13:28:32.000000 hak-0.0.93/hak/one/directory/filepaths/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/directory/filepaths/packages/
+-rw-rw-r--   0 q         (1000) q         (1000)     1311 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/directory/filepaths/packages/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      641 2023-07-10 13:22:24.000000 hak-0.0.93/hak/one/directory/is_empty.py
+-rw-rw-r--   0 q         (1000) q         (1000)      662 2023-07-06 07:04:36.000000 hak-0.0.93/hak/one/directory/is_module.py
+-rw-rw-r--   0 q         (1000) q         (1000)      763 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/directory/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)      810 2023-07-07 01:06:11.000000 hak-0.0.93/hak/one/directory/remove.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3737 2023-07-06 07:04:58.000000 hak-0.0.93/hak/one/duration.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:06.000000 hak-0.0.93/hak/one/file/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      793 2023-07-06 07:05:13.000000 hak-0.0.93/hak/one/file/decrypt.py
+-rw-rw-r--   0 q         (1000) q         (1000)      945 2023-07-06 07:05:20.000000 hak-0.0.93/hak/one/file/encrypt.py
+-rw-rw-r--   0 q         (1000) q         (1000)      586 2023-07-10 13:22:54.000000 hak-0.0.93/hak/one/file/get_next_line_as_int.py
+-rw-rw-r--   0 q         (1000) q         (1000)      705 2023-07-06 07:05:35.000000 hak-0.0.93/hak/one/file/load.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/pickle/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:05:42.000000 hak-0.0.93/hak/one/file/pickle/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1265 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/file/pickle/load_if_exists.py
+-rw-rw-r--   0 q         (1000) q         (1000)      922 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/file/pickle/save.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/py/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 07:06:05.000000 hak-0.0.93/hak/one/file/py/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      566 2023-07-06 07:06:12.000000 hak-0.0.93/hak/one/file/py/create.py
+-rw-rw-r--   0 q         (1000) q         (1000)     2645 2023-07-06 07:06:19.000000 hak-0.0.93/hak/one/file/py/dismantle.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3827 2023-07-06 07:06:27.000000 hak-0.0.93/hak/one/file/py/extract_fn.py
+-rw-rw-r--   0 q         (1000) q         (1000)       84 2023-07-06 07:06:34.000000 hak-0.0.93/hak/one/file/py/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 07:06:42.000000 hak-0.0.93/hak/one/file/remove.py
+-rw-rw-r--   0 q         (1000) q         (1000)      963 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/file/save.py
+-rw-rw-r--   0 q         (1000) q         (1000)      770 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/file/save_lines.py
+-rw-rw-r--   0 q         (1000) q         (1000)      324 2023-07-06 07:07:04.000000 hak-0.0.93/hak/one/file/save_lines_or_string.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.664413 hak-0.0.93/hak/one/file/secret/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/secret/password/
+-rw-rw-r--   0 q         (1000) q         (1000)      696 2023-07-06 07:07:12.000000 hak-0.0.93/hak/one/file/secret/password/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/secret/username/
+-rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 07:07:19.000000 hak-0.0.93/hak/one/file/secret/username/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/tar/
+-rw-rw-r--   0 q         (1000) q         (1000)     1574 2023-07-06 07:07:26.000000 hak-0.0.93/hak/one/file/tar/extract.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/file/zip/
+-rw-rw-r--   0 q         (1000) q         (1000)      507 2023-07-06 07:07:35.000000 hak-0.0.93/hak/one/file/zip/extract.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/function/
+-rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:33:41.000000 hak-0.0.93/hak/one/function/function.py
+-rw-rw-r--   0 q         (1000) q         (1000)      439 2023-07-06 08:33:48.000000 hak-0.0.93/hak/one/function/write_to_file.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/list/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:33:56.000000 hak-0.0.93/hak/one/list/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      116 2023-07-06 08:34:03.000000 hak-0.0.93/hak/one/list/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      115 2023-07-06 08:34:11.000000 hak-0.0.93/hak/one/list/to_comma_separated_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/duration_ms/
+-rw-rw-r--   0 q         (1000) q         (1000)     2120 2023-07-06 08:34:18.000000 hak-0.0.93/hak/one/number/duration_ms/to_bar.py
+-rw-rw-r--   0 q         (1000) q         (1000)      296 2023-07-06 08:34:26.000000 hak-0.0.93/hak/one/number/duration_ms/to_bar_width.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/float/
+-rw-rw-r--   0 q         (1000) q         (1000)       70 2023-07-06 08:34:33.000000 hak-0.0.93/hak/one/number/float/epsilon.py
+-rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:41.000000 hak-0.0.93/hak/one/number/float/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      106 2023-07-06 08:34:48.000000 hak-0.0.93/hak/one/number/float/is_not.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/float/nan/
+-rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:34:55.000000 hak-0.0.93/hak/one/number/float/nan/to_none.py
+-rw-rw-r--   0 q         (1000) q         (1000)      740 2023-07-10 13:23:05.000000 hak-0.0.93/hak/one/number/float/snap_to_zero.py
+-rw-rw-r--   0 q         (1000) q         (1000)      475 2023-07-17 06:40:55.000000 hak-0.0.93/hak/one/number/float/to_rate.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/days/
+-rw-rw-r--   0 q         (1000) q         (1000)      227 2023-07-06 08:35:11.000000 hak-0.0.93/hak/one/number/int/days/a_to_b_inclusive.py
+-rw-rw-r--   0 q         (1000) q         (1000)      104 2023-07-06 08:35:18.000000 hak-0.0.93/hak/one/number/int/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      434 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/number/int/is_prime.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/polarity/
+-rw-rw-r--   0 q         (1000) q         (1000)      499 2023-07-10 13:23:20.000000 hak-0.0.93/hak/one/number/int/polarity/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/primes/
+-rw-rw-r--   0 q         (1000) q         (1000)      867 2023-07-06 08:35:40.000000 hak-0.0.93/hak/one/number/int/primes/download_prime_10.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/primes/prime_factors/
+-rw-rw-r--   0 q         (1000) q         (1000)     1993 2023-07-17 06:41:00.000000 hak-0.0.93/hak/one/number/int/primes/prime_factors/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/width/
+-rw-rw-r--   0 q         (1000) q         (1000)      579 2023-07-06 08:35:55.000000 hak-0.0.93/hak/one/number/int/width/to_text_colour.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/year/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/year/days/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/year/days/count/
+-rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:36:03.000000 hak-0.0.93/hak/one/number/int/year/days/count/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/number/int/year/days/first/
+-rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:36:10.000000 hak-0.0.93/hak/one/number/int/year/days/first/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      431 2023-07-06 08:36:18.000000 hak-0.0.93/hak/one/number/int/year/days/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      916 2023-07-10 13:23:34.000000 hak-0.0.93/hak/one/number/int/year/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      153 2023-07-06 08:36:26.000000 hak-0.0.93/hak/one/number/int/year/now.py
+-rw-rw-r--   0 q         (1000) q         (1000)      824 2023-07-14 04:32:30.000000 hak-0.0.93/hak/one/number/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      123 2023-07-06 08:36:33.000000 hak-0.0.93/hak/one/number/log_2.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/period/
+-rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:36:40.000000 hak-0.0.93/hak/one/period/contains_day.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/schedule/
+-rw-rw-r--   0 q         (1000) q         (1000)     3465 2023-07-06 08:36:48.000000 hak-0.0.93/hak/one/schedule/make.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/session/
+-rw-rw-r--   0 q         (1000) q         (1000)      146 2023-07-06 08:36:55.000000 hak-0.0.93/hak/one/session/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.676413 hak-0.0.93/hak/one/set/
+-rw-rw-r--   0 q         (1000) q         (1000)      114 2023-07-06 08:37:03.000000 hak-0.0.93/hak/one/set/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:37:10.000000 hak-0.0.93/hak/one/string/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/alphanumeric/
+-rw-rw-r--   0 q         (1000) q         (1000)      264 2023-07-06 08:37:18.000000 hak-0.0.93/hak/one/string/alphanumeric/fake.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/append/
+-rw-rw-r--   0 q         (1000) q         (1000)       54 2023-07-06 08:37:25.000000 hak-0.0.93/hak/one/string/append/new_line.py
+-rw-rw-r--   0 q         (1000) q         (1000)      549 2023-07-06 08:37:33.000000 hak-0.0.93/hak/one/string/camel_to_snake.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/char/
+-rw-rw-r--   0 q         (1000) q         (1000)      326 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/char/find_all_indices.py
+-rw-rw-r--   0 q         (1000) q         (1000)      128 2023-07-06 08:37:47.000000 hak-0.0.93/hak/one/string/char/is_digit.py
+-rw-rw-r--   0 q         (1000) q         (1000)      207 2023-07-06 08:37:55.000000 hak-0.0.93/hak/one/string/char/is_upper.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/char/last/
+-rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-06 08:38:02.000000 hak-0.0.93/hak/one/string/char/last/find.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/chars/
+-rw-rw-r--   0 q         (1000) q         (1000)      561 2023-07-06 08:38:10.000000 hak-0.0.93/hak/one/string/chars/remove.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/colour/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:38:17.000000 hak-0.0.93/hak/one/string/colour/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/colour/bright/
+-rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:25.000000 hak-0.0.93/hak/one/string/colour/bright/blue.py
+-rw-rw-r--   0 q         (1000) q         (1000)      166 2023-07-06 08:38:32.000000 hak-0.0.93/hak/one/string/colour/bright/cyan.py
+-rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:38:40.000000 hak-0.0.93/hak/one/string/colour/bright/green.py
+-rw-rw-r--   0 q         (1000) q         (1000)      172 2023-07-06 08:38:47.000000 hak-0.0.93/hak/one/string/colour/bright/magenta.py
+-rw-rw-r--   0 q         (1000) q         (1000)      164 2023-07-06 08:38:55.000000 hak-0.0.93/hak/one/string/colour/bright/red.py
+-rw-rw-r--   0 q         (1000) q         (1000)      168 2023-07-06 08:39:02.000000 hak-0.0.93/hak/one/string/colour/bright/white.py
+-rw-rw-r--   0 q         (1000) q         (1000)      170 2023-07-06 08:39:10.000000 hak-0.0.93/hak/one/string/colour/bright/yellow.py
+-rw-rw-r--   0 q         (1000) q         (1000)      134 2023-07-06 08:39:17.000000 hak-0.0.93/hak/one/string/colour/danger.py
+-rw-rw-r--   0 q         (1000) q         (1000)      178 2023-07-06 08:39:25.000000 hak-0.0.93/hak/one/string/colour/danger_if_zero.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/colour/dark/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:39:32.000000 hak-0.0.93/hak/one/string/colour/dark/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:40.000000 hak-0.0.93/hak/one/string/colour/dark/blue.py
+-rw-rw-r--   0 q         (1000) q         (1000)      152 2023-07-06 08:39:47.000000 hak-0.0.93/hak/one/string/colour/dark/cyan.py
+-rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:39:55.000000 hak-0.0.93/hak/one/string/colour/dark/default.py
+-rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:03.000000 hak-0.0.93/hak/one/string/colour/dark/green.py
+-rw-rw-r--   0 q         (1000) q         (1000)      158 2023-07-06 08:40:10.000000 hak-0.0.93/hak/one/string/colour/dark/magenta.py
+-rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-06 08:40:18.000000 hak-0.0.93/hak/one/string/colour/dark/red.py
+-rw-rw-r--   0 q         (1000) q         (1000)      154 2023-07-06 08:40:25.000000 hak-0.0.93/hak/one/string/colour/dark/white.py
+-rw-rw-r--   0 q         (1000) q         (1000)      156 2023-07-06 08:40:33.000000 hak-0.0.93/hak/one/string/colour/dark/yellow.py
+-rw-rw-r--   0 q         (1000) q         (1000)       64 2023-07-06 08:40:40.000000 hak-0.0.93/hak/one/string/colour/data.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3430 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/colour/decolour.py
+-rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:47.000000 hak-0.0.93/hak/one/string/colour/info.py
+-rw-rw-r--   0 q         (1000) q         (1000)      135 2023-07-06 08:40:55.000000 hak-0.0.93/hak/one/string/colour/primary.py
+-rw-rw-r--   0 q         (1000) q         (1000)     2321 2023-07-06 08:41:02.000000 hak-0.0.93/hak/one/string/colour/rainbow.py
+-rw-rw-r--   0 q         (1000) q         (1000)      138 2023-07-06 08:41:10.000000 hak-0.0.93/hak/one/string/colour/secondary.py
+-rw-rw-r--   0 q         (1000) q         (1000)      275 2023-07-06 08:41:17.000000 hak-0.0.93/hak/one/string/colour/tgfr.py
+-rw-rw-r--   0 q         (1000) q         (1000)      139 2023-07-06 08:41:25.000000 hak-0.0.93/hak/one/string/colour/warning.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/contains/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:32.000000 hak-0.0.93/hak/one/string/contains/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/contains/function/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:41:40.000000 hak-0.0.93/hak/one/string/contains/function/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-06 08:41:47.000000 hak-0.0.93/hak/one/string/contains/function/run.py
+-rw-rw-r--   0 q         (1000) q         (1000)      192 2023-07-07 05:12:17.000000 hak-0.0.93/hak/one/string/contains/function/test.py
+-rw-rw-r--   0 q         (1000) q         (1000)      224 2023-07-06 08:42:02.000000 hak-0.0.93/hak/one/string/contains/l.py
+-rw-rw-r--   0 q         (1000) q         (1000)       76 2023-07-06 08:42:10.000000 hak-0.0.93/hak/one/string/contains/version.py
+-rw-rw-r--   0 q         (1000) q         (1000)      105 2023-07-06 08:42:17.000000 hak-0.0.93/hak/one/string/count_x_in_y.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/date/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/date/separator/
+-rw-rw-r--   0 q         (1000) q         (1000)      923 2023-07-10 13:23:48.000000 hak-0.0.93/hak/one/string/date/separator/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1924 2023-07-10 14:58:52.000000 hak-0.0.93/hak/one/string/date/to_date.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/day/
+-rw-rw-r--   0 q         (1000) q         (1000)     1076 2023-07-10 13:25:17.000000 hak-0.0.93/hak/one/string/day/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      996 2023-07-06 08:42:32.000000 hak-0.0.93/hak/one/string/delete_character_safely.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/digits/
+-rw-rw-r--   0 q         (1000) q         (1000)      206 2023-07-06 08:42:40.000000 hak-0.0.93/hak/one/string/digits/remove.py
+-rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:42:47.000000 hak-0.0.93/hak/one/string/double_single_quotes.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/family_name/
+-rw-rw-r--   0 q         (1000) q         (1000)   121166 2023-07-07 04:10:06.000000 hak-0.0.93/hak/one/string/family_name/fake.py
+-rw-rw-r--   0 q         (1000) q         (1000)      303 2023-07-06 08:43:10.000000 hak-0.0.93/hak/one/string/family_name/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/filename/
+-rw-rw-r--   0 q         (1000) q         (1000)      126 2023-07-06 08:43:25.000000 hak-0.0.93/hak/one/string/filename/to_module_name.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/filepath/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:43:32.000000 hak-0.0.93/hak/one/string/filepath/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/filepath/py/
+-rw-rw-r--   0 q         (1000) q         (1000)      720 2023-07-06 08:43:39.000000 hak-0.0.93/hak/one/string/filepath/py/get_t.py
+-rw-rw-r--   0 q         (1000) q         (1000)      100 2023-07-06 08:43:47.000000 hak-0.0.93/hak/one/string/find_first_parenthesis.py
+-rw-rw-r--   0 q         (1000) q         (1000)      213 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/find_last_comma_index.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/fn_name/
+-rw-rw-r--   0 q         (1000) q         (1000)      226 2023-07-06 08:44:02.000000 hak-0.0.93/hak/one/string/fn_name/is_ignorable.py
+-rw-rw-r--   0 q         (1000) q         (1000)     5035 2023-07-06 08:44:09.000000 hak-0.0.93/hak/one/string/format.py
+-rw-rw-r--   0 q         (1000) q         (1000)       73 2023-07-06 08:44:17.000000 hak-0.0.93/hak/one/string/has_at_symbol.py
+-rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:24.000000 hak-0.0.93/hak/one/string/has_digit.py
+-rw-rw-r--   0 q         (1000) q         (1000)      131 2023-07-06 08:44:32.000000 hak-0.0.93/hak/one/string/has_lowercase.py
+-rw-rw-r--   0 q         (1000) q         (1000)      263 2023-07-06 08:44:39.000000 hak-0.0.93/hak/one/string/has_other_char.py
+-rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:44:47.000000 hak-0.0.93/hak/one/string/has_seven_digits.py
+-rw-rw-r--   0 q         (1000) q         (1000)      132 2023-07-06 08:44:54.000000 hak-0.0.93/hak/one/string/has_uppercase.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/hbar/
+-rw-rw-r--   0 q         (1000) q         (1000)      122 2023-07-06 08:45:02.000000 hak-0.0.93/hak/one/string/hbar/make.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/one/string/header/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/header/python_file/
+-rw-rw-r--   0 q         (1000) q         (1000)      322 2023-07-06 08:45:09.000000 hak-0.0.93/hak/one/string/header/python_file/make.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/header/test_table/
+-rw-rw-r--   0 q         (1000) q         (1000)      461 2023-07-06 08:45:17.000000 hak-0.0.93/hak/one/string/header/test_table/make.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/indent/
+-rw-rw-r--   0 q         (1000) q         (1000)      137 2023-07-06 08:45:25.000000 hak-0.0.93/hak/one/string/indent/run_if_class_method.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/insert/
+-rw-rw-r--   0 q         (1000) q         (1000)      602 2023-07-06 08:45:32.000000 hak-0.0.93/hak/one/string/insert/new_line_after_last_import_line.py
+-rw-rw-r--   0 q         (1000) q         (1000)      278 2023-07-06 08:45:40.000000 hak-0.0.93/hak/one/string/insert/new_line_before_comment.py
+-rw-rw-r--   0 q         (1000) q         (1000)      584 2023-07-06 08:45:48.000000 hak-0.0.93/hak/one/string/insert/new_line_before_def.py
+-rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:45:56.000000 hak-0.0.93/hak/one/string/insert/new_line_before_if_main.py
+-rw-rw-r--   0 q         (1000) q         (1000)      670 2023-07-06 08:46:04.000000 hak-0.0.93/hak/one/string/insert/new_line_before_lambda.py
+-rw-rw-r--   0 q         (1000) q         (1000)      292 2023-07-06 08:46:12.000000 hak-0.0.93/hak/one/string/insert/new_line_before_new_line_and_cea_.py
+-rw-rw-r--   0 q         (1000) q         (1000)      102 2023-07-06 08:46:20.000000 hak-0.0.93/hak/one/string/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      124 2023-07-06 08:46:27.000000 hak-0.0.93/hak/one/string/is_or_none.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/json/
+-rw-rw-r--   0 q         (1000) q         (1000)      179 2023-07-06 08:46:35.000000 hak-0.0.93/hak/one/string/json/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      552 2023-07-06 08:46:42.000000 hak-0.0.93/hak/one/string/lambdarise.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/one/string/line/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/one/string/line/last/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/line/last/length/
+-rw-rw-r--   0 q         (1000) q         (1000)      423 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/line/last/length/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      368 2023-07-06 08:46:58.000000 hak-0.0.93/hak/one/string/make_content_without_function.py
+-rw-rw-r--   0 q         (1000) q         (1000)      333 2023-07-06 08:47:06.000000 hak-0.0.93/hak/one/string/make_function_text.py
+-rw-rw-r--   0 q         (1000) q         (1000)      346 2023-07-06 08:47:13.000000 hak-0.0.93/hak/one/string/make_initial_content.py
+-rw-rw-r--   0 q         (1000) q         (1000)      327 2023-07-06 08:47:21.000000 hak-0.0.93/hak/one/string/make_new_function_text.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/money/
+-rw-rw-r--   0 q         (1000) q         (1000)      541 2023-07-10 13:25:31.000000 hak-0.0.93/hak/one/string/money/to_float.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/month/
+-rw-rw-r--   0 q         (1000) q         (1000)     1009 2023-07-10 13:25:45.000000 hak-0.0.93/hak/one/string/month/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      559 2023-07-10 14:58:57.000000 hak-0.0.93/hak/one/string/month/to_number.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/nest_level/
+-rw-rw-r--   0 q         (1000) q         (1000)      688 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/nest_level/get.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/password/
+-rw-rw-r--   0 q         (1000) q         (1000)     1187 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/password/create.py
+-rw-rw-r--   0 q         (1000) q         (1000)      555 2023-07-06 08:47:50.000000 hak-0.0.93/hak/one/string/password/has_chars_from_3_sets.py
+-rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/pop_left.py
+-rw-rw-r--   0 q         (1000) q         (1000)      223 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/pop_right.py
+-rw-rw-r--   0 q         (1000) q         (1000)      151 2023-07-06 08:48:13.000000 hak-0.0.93/hak/one/string/prepend_import.py
+-rw-rw-r--   0 q         (1000) q         (1000)      756 2023-07-06 08:48:20.000000 hak-0.0.93/hak/one/string/print_and_return_false.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.680413 hak-0.0.93/hak/one/string/refactor/
+-rw-rw-r--   0 q         (1000) q         (1000)     1218 2023-07-06 08:48:28.000000 hak-0.0.93/hak/one/string/refactor/by_two_char_combinations.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/remove/
+-rw-rw-r--   0 q         (1000) q         (1000)      211 2023-07-06 08:48:35.000000 hak-0.0.93/hak/one/string/remove/empty_line_spaces.py
+-rw-rw-r--   0 q         (1000) q         (1000)      162 2023-07-06 08:48:42.000000 hak-0.0.93/hak/one/string/remove/empty_lines.py
+-rw-rw-r--   0 q         (1000) q         (1000)      441 2023-07-06 08:48:50.000000 hak-0.0.93/hak/one/string/remove/extra_new_line_following_class_definition.py
+-rw-rw-r--   0 q         (1000) q         (1000)      210 2023-07-06 08:48:57.000000 hak-0.0.93/hak/one/string/remove/first_new_line_if_starts_with_new_line.py
+-rw-rw-r--   0 q         (1000) q         (1000)       81 2023-07-06 08:49:04.000000 hak-0.0.93/hak/one/string/remove/whitespace_between_newlines.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/replace/
+-rw-rw-r--   0 q         (1000) q         (1000)      241 2023-07-06 08:49:12.000000 hak-0.0.93/hak/one/string/replace/double_new_line_with_single_new_line.py
+-rw-rw-r--   0 q         (1000) q         (1000)      129 2023-07-06 08:49:20.000000 hak-0.0.93/hak/one/string/replace/single_new_line_with_empty_string.py
+-rw-rw-r--   0 q         (1000) q         (1000)      251 2023-07-06 08:49:27.000000 hak-0.0.93/hak/one/string/replace/triple_new_line_with_double_new_line.py
+-rw-rw-r--   0 q         (1000) q         (1000)      487 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/string/replace_unprintable.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3365 2023-07-06 08:49:42.000000 hak-0.0.93/hak/one/string/separate_function_from_context.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/single_line_function/
+-rw-rw-r--   0 q         (1000) q         (1000)      432 2023-07-06 08:49:49.000000 hak-0.0.93/hak/one/string/single_line_function/is_a.py
+-rw-rw-r--   0 q         (1000) q         (1000)      467 2023-07-06 08:49:57.000000 hak-0.0.93/hak/one/string/single_line_function/to_lambda_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/spaces/
+-rw-rw-r--   0 q         (1000) q         (1000)      111 2023-07-06 08:50:05.000000 hak-0.0.93/hak/one/string/spaces/count.py
+-rw-rw-r--   0 q         (1000) q         (1000)      331 2023-07-06 08:50:12.000000 hak-0.0.93/hak/one/string/split_fn_name_and_text.py
+-rw-rw-r--   0 q         (1000) q         (1000)      344 2023-07-06 08:50:20.000000 hak-0.0.93/hak/one/string/strip_unprintable.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/table/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-07 05:28:43.000000 hak-0.0.93/hak/one/string/table/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/table/bar/
+-rw-rw-r--   0 q         (1000) q         (1000)      363 2023-07-17 06:41:04.000000 hak-0.0.93/hak/one/string/table/bar/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)      265 2023-07-06 08:50:27.000000 hak-0.0.93/hak/one/string/to_cond_freq_dict.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/token/
+-rw-rw-r--   0 q         (1000) q         (1000)     1263 2023-07-06 08:50:35.000000 hak-0.0.93/hak/one/string/token/substitute.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/year/
+-rw-rw-r--   0 q         (1000) q         (1000)      177 2023-07-10 13:26:13.000000 hak-0.0.93/hak/one/string/year/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/string/yyyymmdd/
+-rw-rw-r--   0 q         (1000) q         (1000)      238 2023-07-06 08:50:42.000000 hak-0.0.93/hak/one/string/yyyymmdd/to_date.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/one/subprocess/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/subprocess/completed_process/
+-rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-07 01:06:09.000000 hak-0.0.93/hak/one/subprocess/completed_process/to_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/system/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:50:57.000000 hak-0.0.93/hak/one/system/__init__.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/system/git/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/system/git/commit/
+-rw-rw-r--   0 q         (1000) q         (1000)     2527 2023-07-06 08:51:35.000000 hak-0.0.93/hak/one/system/git/commit/run.py
+-rw-rw-r--   0 q         (1000) q         (1000)      393 2023-07-06 08:51:42.000000 hak-0.0.93/hak/one/system/git/commit_if_test_and_app_ok.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/system/git/gitignore/
+-rw-rw-r--   0 q         (1000) q         (1000)      647 2023-07-06 08:51:51.000000 hak-0.0.93/hak/one/system/git/gitignore/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)      485 2023-07-07 01:09:02.000000 hak-0.0.93/hak/one/system/git/init.py
+-rw-rw-r--   0 q         (1000) q         (1000)      745 2023-07-06 08:52:07.000000 hak-0.0.93/hak/one/system/git/log_oneline.py
+-rw-rw-r--   0 q         (1000) q         (1000)      870 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/system/git/push_after_delay.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/system/screen/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-07-06 08:52:21.000000 hak-0.0.93/hak/one/system/screen/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)      786 2023-07-06 08:52:29.000000 hak-0.0.93/hak/one/system/screen/clear.py
+-rw-rw-r--   0 q         (1000) q         (1000)     3127 2023-07-10 13:03:40.000000 hak-0.0.93/hak/one/terminal.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/one/tup/
+-rw-rw-r--   0 q         (1000) q         (1000)      176 2023-07-06 08:52:44.000000 hak-0.0.93/hak/one/tup/is_a.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/
+-rw-rw-r--   0 q         (1000) q         (1000)      430 2023-07-07 01:09:29.000000 hak-0.0.93/hak/other/l.py
+-rw-rw-r--   0 q         (1000) q         (1000)       91 2023-07-06 08:52:59.000000 hak-0.0.93/hak/other/nop_state_x.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/patch/
+-rw-rw-r--   0 q         (1000) q         (1000)     7954 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/patch/do.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/pip/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/pip/dist_tar/
+-rw-rw-r--   0 q         (1000) q         (1000)     3093 2023-07-10 13:27:41.000000 hak-0.0.93/hak/other/pip/dist_tar/make.py
+-rw-rw-r--   0 q         (1000) q         (1000)      805 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/pip/dist_tar/remove.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/pip/setup/
+-rw-rw-r--   0 q         (1000) q         (1000)     1321 2023-07-06 08:53:29.000000 hak-0.0.93/hak/other/pip/setup/update.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1808 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/pip/upload.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/pip/version/
+-rw-rw-r--   0 q         (1000) q         (1000)      897 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/pip/version/get.py
+-rw-rw-r--   0 q         (1000) q         (1000)      120 2023-07-06 22:28:42.000000 hak-0.0.93/hak/other/pip/version/to_str.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/report/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/report/fail/
+-rw-rw-r--   0 q         (1000) q         (1000)      822 2023-07-06 22:28:49.000000 hak-0.0.93/hak/other/report/fail/no_xyz.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1936 2023-07-06 22:28:57.000000 hak-0.0.93/hak/other/report/fail/xyz.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1462 2023-07-06 22:29:04.000000 hak-0.0.93/hak/other/report/fail/z_return_neq_y_return.py
+-rw-rw-r--   0 q         (1000) q         (1000)     1623 2023-07-06 22:29:12.000000 hak-0.0.93/hak/other/report/fail/z_stdo_neq_y_stdo.py
+-rw-rw-r--   0 q         (1000) q         (1000)      895 2023-07-06 22:29:19.000000 hak-0.0.93/hak/other/report/property_failure.py
+-rw-rw-r--   0 q         (1000) q         (1000)      737 2023-07-06 22:29:27.000000 hak-0.0.93/hak/other/report/success.py
+-rw-rw-r--   0 q         (1000) q         (1000)      394 2023-07-06 22:29:34.000000 hak-0.0.93/hak/other/report/summarise_file.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak/other/setup/
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/setup/cfg/
+-rw-rw-r--   0 q         (1000) q         (1000)     1547 2023-07-06 22:29:41.000000 hak-0.0.93/hak/other/setup/cfg/update.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/other/setup/py/
+-rw-rw-r--   0 q         (1000) q         (1000)     1653 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/setup/py/update.py
+-rw-rw-r--   0 q         (1000) q         (1000)      341 2023-07-10 13:03:40.000000 hak-0.0.93/hak/other/ternary.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/pair/
+-rw-rw-r--   0 q         (1000) q         (1000)      140 2023-07-06 22:30:04.000000 hak-0.0.93/hak/pair/eq.py
+-rw-rw-r--   0 q         (1000) q         (1000)      150 2023-07-10 13:03:46.000000 hak-0.0.93/hak/pxyz.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/
+-rw-rw-r--   0 q         (1000) q         (1000)        0 2023-04-23 03:18:31.000000 hak-0.0.93/hak/test/__init__.py
+-rw-rw-r--   0 q         (1000) q         (1000)     2658 2023-07-06 06:52:54.000000 hak-0.0.93/hak/test/do.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/failed/
+-rw-rw-r--   0 q         (1000) q         (1000)     1112 2023-07-06 06:53:05.000000 hak-0.0.93/hak/test/failed/handle.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/final_line/
+-rw-rw-r--   0 q         (1000) q         (1000)     2531 2023-07-10 13:03:40.000000 hak-0.0.93/hak/test/final_line/check.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/line_lengths/
+-rw-rw-r--   0 q         (1000) q         (1000)     2717 2023-07-10 13:03:40.000000 hak-0.0.93/hak/test/line_lengths/check.py
+-rw-rw-r--   0 q         (1000) q         (1000)      790 2023-07-10 13:03:40.000000 hak-0.0.93/hak/test/line_lengths_check.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/oldest_file/
+-rw-rw-r--   0 q         (1000) q         (1000)     4789 2023-07-10 13:03:40.000000 hak-0.0.93/hak/test/oldest_file/print.py
+-rw-rw-r--   0 q         (1000) q         (1000)      937 2023-07-06 06:53:55.000000 hak-0.0.93/hak/test/oldest_file_print.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.684413 hak-0.0.93/hak/test/passed/
+-rw-rw-r--   0 q         (1000) q         (1000)      961 2023-07-06 06:54:05.000000 hak-0.0.93/hak/test/passed/handle.py
+drwxrwxr-x   0 q         (1000) q         (1000)        0 2023-07-17 10:49:56.668413 hak-0.0.93/hak.egg-info/
+-rw-rw-r--   0 q         (1000) q         (1000)     1212 2023-07-17 10:49:56.000000 hak-0.0.93/hak.egg-info/PKG-INFO
+-rw-rw-r--   0 q         (1000) q         (1000)    12826 2023-07-17 10:49:56.000000 hak-0.0.93/hak.egg-info/SOURCES.txt
+-rw-rw-r--   0 q         (1000) q         (1000)        1 2023-07-17 10:49:56.000000 hak-0.0.93/hak.egg-info/dependency_links.txt
+-rw-rw-r--   0 q         (1000) q         (1000)     3390 2023-07-17 10:49:56.000000 hak-0.0.93/hak.egg-info/top_level.txt
+-rw-rw-r--   0 q         (1000) q         (1000)      537 2023-07-17 10:49:56.684413 hak-0.0.93/setup.cfg
+-rw-rw-r--   0 q         (1000) q         (1000)      576 2023-07-17 10:49:56.000000 hak-0.0.93/setup.py
```

### Comparing `hak-0.0.92/LICENSE` & `hak-0.0.93/LICENSE`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/PKG-INFO` & `hak-0.0.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.92
+Version: 0.0.93
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.92/README.md` & `hak-0.0.93/README.md`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/fake/subprocess/run.py` & `hak-0.0.93/hak/fake/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/compare.py` & `hak-0.0.93/hak/many/dicts/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/compare_relevant_only.py` & `hak-0.0.93/hak/many/dicts/compare_relevant_only.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/convert_date_strings_to_dates.py` & `hak-0.0.93/hak/many/dicts/convert_date_strings_to_dates.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/get_datatypes.py` & `hak-0.0.93/hak/many/dicts/get_datatypes.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/get_keys_with_none_or_zero_vals.py` & `hak-0.0.93/hak/many/dicts/get_keys_with_none_or_zero_vals.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/merge_freq_dicts.py` & `hak-0.0.93/hak/many/dicts/merge_freq_dicts.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/dicts/to_table.py` & `hak-0.0.93/hak/many/dicts/to_table.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/directories/empty/find.py` & `hak-0.0.93/hak/many/directories/empty/find.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/directories/empty/remove.py` & `hak-0.0.93/hak/many/directories/empty/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/directories/exist.py` & `hak-0.0.93/hak/many/directories/exist.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/directories/get.py` & `hak-0.0.93/hak/many/directories/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/files/pyfiles/dismantle.py` & `hak-0.0.93/hak/many/files/pyfiles/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/pyfiles/format_and_commit.py` & `hak-0.0.93/hak/many/pyfiles/format_and_commit.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/compare.py` & `hak-0.0.93/hak/many/strings/compare.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/date_pieces/get.py` & `hak-0.0.93/hak/many/strings/date_pieces/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/date_pieces/separate_day.py` & `hak-0.0.93/hak/many/strings/date_pieces/separate_day.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/date_pieces/separate_year.py` & `hak-0.0.93/hak/many/strings/date_pieces/separate_year.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/dates/detect_format.py` & `hak-0.0.93/hak/many/strings/dates/detect_format.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/filepaths/get_least_recently_modified.py` & `hak-0.0.93/hak/many/strings/filepaths/get_least_recently_modified.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/filepaths/get_most_recently_modified.py` & `hak-0.0.93/hak/many/strings/filepaths/get_most_recently_modified.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/filepaths/py/get.py` & `hak-0.0.93/hak/many/strings/filepaths/py/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/filepaths/py/testables/get.py` & `hak-0.0.93/hak/many/strings/filepaths/py/testables/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py` & `hak-0.0.93/hak/many/strings/filepaths/py/to_filepath_file_content_dict.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/find_first_diff.py` & `hak-0.0.93/hak/many/strings/find_first_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/patch_setup_py.py` & `hak-0.0.93/hak/many/strings/patch_setup_py.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/pyfiles/filter_out_items.py` & `hak-0.0.93/hak/many/strings/pyfiles/filter_out_items.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/show_diff.py` & `hak-0.0.93/hak/many/strings/show_diff.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/strings/to_dict.py` & `hak-0.0.93/hak/many/strings/to_dict.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/many/values/get_datatype.py` & `hak-0.0.93/hak/many/values/get_datatype.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/check_if_ok_to_proceed.py` & `hak-0.0.93/hak/one/check_if_ok_to_proceed.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/date/public_holiday/is_a.py` & `hak-0.0.93/hak/one/date/public_holiday/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/date/to_financial_year.py` & `hak-0.0.93/hak/one/date/to_financial_year.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/date/to_utc_timestamp.py` & `hak-0.0.93/hak/one/date/to_utc_timestamp.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/date/year/easter_sunday/get.py` & `hak-0.0.93/hak/one/date/year/easter_sunday/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/cell/get_width.py` & `hak-0.0.93/hak/one/dict/cell/get_width.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/cell/make.py` & `hak-0.0.93/hak/one/dict/cell/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/cell/to_str.py` & `hak-0.0.93/hak/one/dict/cell/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/durations/load.py` & `hak-0.0.93/hak/one/dict/durations/load.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/durations/save.py` & `hak-0.0.93/hak/one/dict/durations/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/durations/update_one.py` & `hak-0.0.93/hak/one/dict/durations/update_one.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/frequencies/choose.py` & `hak-0.0.93/hak/one/dict/frequencies/choose.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/get_or_zero.py` & `hak-0.0.93/hak/one/dict/get_or_zero.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/header/to_str.py` & `hak-0.0.93/hak/one/dict/header/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/contains_date.py` & `hak-0.0.93/hak/one/dict/period/contains_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/contains_date.py` & `hak-0.0.93/hak/one/dict/period/financial_year/contains_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/ge.py` & `hak-0.0.93/hak/one/dict/period/financial_year/ge.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/get_start_date.py` & `hak-0.0.93/hak/one/dict/period/financial_year/get_start_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/is_a.py` & `hak-0.0.93/hak/one/dict/period/financial_year/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/le.py` & `hak-0.0.93/hak/one/dict/period/financial_year/le.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/leq.py` & `hak-0.0.93/hak/one/dict/period/financial_year/leq.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/financial_year/make.py` & `hak-0.0.93/hak/one/dict/period/financial_year/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/get_end.py` & `hak-0.0.93/hak/one/dict/period/get_end.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/get_start.py` & `hak-0.0.93/hak/one/dict/period/get_start.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/month/get_end_date.py` & `hak-0.0.93/hak/one/dict/period/month/get_end_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/period/month/get_start_date.py` & `hak-0.0.93/hak/one/dict/period/month/get_start_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/proposed_dismantlement/show.py` & `hak-0.0.93/hak/one/dict/proposed_dismantlement/show.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/abs.py` & `hak-0.0.93/hak/one/dict/rate/abs.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/add.py` & `hak-0.0.93/hak/one/dict/rate/add.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/div_number_by_rate.py` & `hak-0.0.93/hak/one/dict/rate/div_number_by_rate.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/div_rate_by_rate.py` & `hak-0.0.93/hak/one/dict/rate/div_rate_by_rate.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/eq.py` & `hak-0.0.93/hak/one/dict/rate/eq.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/is_a.py` & `hak-0.0.93/hak/one/dict/rate/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/make.py` & `hak-0.0.93/hak/one/dict/rate/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/mult_rate_by_number.py` & `hak-0.0.93/hak/one/dict/rate/mult_rate_by_number.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/mult_rate_by_rate.py` & `hak-0.0.93/hak/one/dict/rate/mult_rate_by_rate.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/sub.py` & `hak-0.0.93/hak/one/dict/rate/sub.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/to_float.py` & `hak-0.0.93/hak/one/dict/rate/to_float.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/rate/to_num.py` & `hak-0.0.93/hak/one/dict/rate/to_num.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/remove_zeroes.py` & `hak-0.0.93/hak/one/dict/remove_zeroes.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/table/get_field_widths.py` & `hak-0.0.93/hak/one/dict/table/get_field_widths.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/dict/to_max_line_width_str.py` & `hak-0.0.93/hak/one/dict/to_max_line_width_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/compress_to_tar.py` & `hak-0.0.93/hak/one/directory/compress_to_tar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/empty.py` & `hak-0.0.93/hak/one/directory/empty.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/filepaths/get.py` & `hak-0.0.93/hak/one/directory/filepaths/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/filepaths/packages/get.py` & `hak-0.0.93/hak/one/directory/filepaths/packages/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/is_empty.py` & `hak-0.0.93/hak/one/directory/is_empty.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/is_module.py` & `hak-0.0.93/hak/one/directory/is_module.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/make.py` & `hak-0.0.93/hak/one/directory/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/directory/remove.py` & `hak-0.0.93/hak/one/directory/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/duration.py` & `hak-0.0.93/hak/one/duration.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/decrypt.py` & `hak-0.0.93/hak/one/file/decrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/encrypt.py` & `hak-0.0.93/hak/one/file/encrypt.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/get_next_line_as_int.py` & `hak-0.0.93/hak/one/file/get_next_line_as_int.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/load.py` & `hak-0.0.93/hak/one/file/load.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/pickle/load_if_exists.py` & `hak-0.0.93/hak/one/file/pickle/load_if_exists.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/pickle/save.py` & `hak-0.0.93/hak/one/file/pickle/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/py/create.py` & `hak-0.0.93/hak/one/file/py/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/py/dismantle.py` & `hak-0.0.93/hak/one/file/py/dismantle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/py/extract_fn.py` & `hak-0.0.93/hak/one/file/py/extract_fn.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/save.py` & `hak-0.0.93/hak/one/file/save.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/save_lines.py` & `hak-0.0.93/hak/one/file/save_lines.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/secret/password/get.py` & `hak-0.0.93/hak/one/file/secret/password/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/secret/username/get.py` & `hak-0.0.93/hak/one/file/secret/username/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/file/tar/extract.py` & `hak-0.0.93/hak/one/file/tar/extract.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/duration_ms/to_bar.py` & `hak-0.0.93/hak/one/number/duration_ms/to_bar.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/float/snap_to_zero.py` & `hak-0.0.93/hak/one/number/float/snap_to_zero.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/int/primes/download_prime_10.py` & `hak-0.0.93/hak/one/number/int/primes/download_prime_10.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/int/primes/prime_factors/get.py` & `hak-0.0.93/hak/one/number/int/primes/prime_factors/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/int/width/to_text_colour.py` & `hak-0.0.93/hak/one/number/int/width/to_text_colour.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/int/year/is_a.py` & `hak-0.0.93/hak/one/number/int/year/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/number/is_a.py` & `hak-0.0.93/hak/one/number/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/schedule/make.py` & `hak-0.0.93/hak/one/schedule/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/camel_to_snake.py` & `hak-0.0.93/hak/one/string/camel_to_snake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/chars/remove.py` & `hak-0.0.93/hak/one/string/chars/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/colour/decolour.py` & `hak-0.0.93/hak/one/string/colour/decolour.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/colour/rainbow.py` & `hak-0.0.93/hak/one/string/colour/rainbow.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/date/separator/get.py` & `hak-0.0.93/hak/one/string/date/separator/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/date/to_date.py` & `hak-0.0.93/hak/one/string/date/to_date.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/day/is_a.py` & `hak-0.0.93/hak/one/string/day/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/delete_character_safely.py` & `hak-0.0.93/hak/one/string/delete_character_safely.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/family_name/fake.py` & `hak-0.0.93/hak/one/string/family_name/fake.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/filepath/py/get_t.py` & `hak-0.0.93/hak/one/string/filepath/py/get_t.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/format.py` & `hak-0.0.93/hak/one/string/format.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/insert/new_line_after_last_import_line.py` & `hak-0.0.93/hak/one/string/insert/new_line_after_last_import_line.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/insert/new_line_before_def.py` & `hak-0.0.93/hak/one/string/insert/new_line_before_def.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/insert/new_line_before_lambda.py` & `hak-0.0.93/hak/one/string/insert/new_line_before_lambda.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/lambdarise.py` & `hak-0.0.93/hak/one/string/lambdarise.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/money/to_float.py` & `hak-0.0.93/hak/one/string/money/to_float.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/month/is_a.py` & `hak-0.0.93/hak/one/string/month/is_a.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/month/to_number.py` & `hak-0.0.93/hak/one/string/month/to_number.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/nest_level/get.py` & `hak-0.0.93/hak/one/string/nest_level/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/password/create.py` & `hak-0.0.93/hak/one/string/password/create.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/password/has_chars_from_3_sets.py` & `hak-0.0.93/hak/one/string/password/has_chars_from_3_sets.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/print_and_return_false.py` & `hak-0.0.93/hak/one/string/print_and_return_false.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/refactor/by_two_char_combinations.py` & `hak-0.0.93/hak/one/string/refactor/by_two_char_combinations.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/separate_function_from_context.py` & `hak-0.0.93/hak/one/string/separate_function_from_context.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/string/token/substitute.py` & `hak-0.0.93/hak/one/string/token/substitute.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/subprocess/completed_process/to_str.py` & `hak-0.0.93/hak/one/subprocess/completed_process/to_str.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/system/git/commit/run.py` & `hak-0.0.93/hak/one/system/git/commit/run.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/system/git/gitignore/make.py` & `hak-0.0.93/hak/one/system/git/gitignore/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/system/git/log_oneline.py` & `hak-0.0.93/hak/one/system/git/log_oneline.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/system/git/push_after_delay.py` & `hak-0.0.93/hak/one/system/git/push_after_delay.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/system/screen/clear.py` & `hak-0.0.93/hak/one/system/screen/clear.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/one/terminal.py` & `hak-0.0.93/hak/one/terminal.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/patch/do.py` & `hak-0.0.93/hak/other/patch/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/pip/dist_tar/make.py` & `hak-0.0.93/hak/other/pip/dist_tar/make.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/pip/dist_tar/remove.py` & `hak-0.0.93/hak/other/pip/dist_tar/remove.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/pip/setup/update.py` & `hak-0.0.93/hak/other/pip/setup/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/pip/upload.py` & `hak-0.0.93/hak/other/pip/upload.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/pip/version/get.py` & `hak-0.0.93/hak/other/pip/version/get.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/fail/no_xyz.py` & `hak-0.0.93/hak/other/report/fail/no_xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/fail/xyz.py` & `hak-0.0.93/hak/other/report/fail/xyz.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/fail/z_return_neq_y_return.py` & `hak-0.0.93/hak/other/report/fail/z_return_neq_y_return.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/fail/z_stdo_neq_y_stdo.py` & `hak-0.0.93/hak/other/report/fail/z_stdo_neq_y_stdo.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/property_failure.py` & `hak-0.0.93/hak/other/report/property_failure.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/report/success.py` & `hak-0.0.93/hak/other/report/success.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/setup/cfg/update.py` & `hak-0.0.93/hak/other/setup/cfg/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/other/setup/py/update.py` & `hak-0.0.93/hak/other/setup/py/update.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/do.py` & `hak-0.0.93/hak/test/do.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/failed/handle.py` & `hak-0.0.93/hak/test/failed/handle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/final_line/check.py` & `hak-0.0.93/hak/test/final_line/check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/line_lengths/check.py` & `hak-0.0.93/hak/test/line_lengths/check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/line_lengths_check.py` & `hak-0.0.93/hak/test/line_lengths_check.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/oldest_file/print.py` & `hak-0.0.93/hak/test/oldest_file/print.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/oldest_file_print.py` & `hak-0.0.93/hak/test/oldest_file_print.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak/test/passed/handle.py` & `hak-0.0.93/hak/test/passed/handle.py`

 * *Files identical despite different names*

### Comparing `hak-0.0.92/hak.egg-info/PKG-INFO` & `hak-0.0.93/hak.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hak
-Version: 0.0.92
+Version: 0.0.93
 Summary: Function Test Pair Toolbox
 Home-page: https://github.com/JohnForbes/hak
 Author: @JohnRForbes
 Author-email: john.robert.forbes@gmail.com
 License: MIT
 Description: # hak
         This project is a collection of function test pairs for common tasks.
```

### Comparing `hak-0.0.92/hak.egg-info/SOURCES.txt` & `hak-0.0.93/hak.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
 hak/one/dict/rate/sub.py
 hak/one/dict/rate/to_float.py
 hak/one/dict/rate/to_num.py
 hak/one/dict/rate/to_str.py
 hak/one/dict/rate/to_str_frac.py
 hak/one/dict/table/__init__.py
 hak/one/dict/table/get_field_widths.py
+hak/one/dict/unit/to_str.py
 hak/one/dict/values/__init__.py
 hak/one/dict/values/numbers/__init__.py
 hak/one/dict/values/numbers/negative/__init__.py
 hak/one/dict/values/numbers/negative/count.py
 hak/one/dict/values/numbers/positive/__init__.py
 hak/one/dict/values/numbers/positive/count.py
 hak/one/directory/__init__.py
```

### Comparing `hak-0.0.92/hak.egg-info/top_level.txt` & `hak-0.0.93/hak.egg-info/top_level.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 hak/one/dict/hidden_fields
 hak/one/dict/period
 hak/one/dict/period/financial_year
 hak/one/dict/period/month
 hak/one/dict/proposed_dismantlement
 hak/one/dict/rate
 hak/one/dict/table
+hak/one/dict/unit
 hak/one/dict/values
 hak/one/dict/values/numbers
 hak/one/dict/values/numbers/negative
 hak/one/dict/values/numbers/positive
 hak/one/directory
 hak/one/directory/filepaths
 hak/one/directory/filepaths/packages
```

### Comparing `hak-0.0.92/setup.cfg` & `hak-0.0.93/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = hak
-version = 0.0.92
+version = 0.0.93
 author = John Forbes
 author_email = john.robert.forbes@gmail.com
 description = Function Test Pair Toolbox
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JohnForbes/hak
 license_files = LICENSE
```

### Comparing `hak-0.0.92/setup.py` & `hak-0.0.93/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from pathlib import Path
 from hak.one.directory.filepaths.packages.get import f as get_packages
 long_description = Path("./README.md").read_text()
 
 setup(
   name='hak',
-  version='0.0.92',
+  version='0.0.93',
   license='MIT',
   description='Function Test Pair Toolbox',
   long_description=long_description,
   long_description_content_type="text/markdown",
   author='@JohnRForbes',
   author_email='john.robert.forbes@gmail.com',
   url='https://github.com/JohnForbes/hak',
```

