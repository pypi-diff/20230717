# Comparing `tmp/pmagpy-cli-4.2.97.tar.gz` & `tmp/pmagpy-cli-4.2.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pmagpy-cli-4.2.97.tar", last modified: Tue Mar 22 20:01:51 2022, max compression
+gzip compressed data, was "pmagpy-cli-4.2.98.tar", last modified: Fri Mar 25 00:16:18 2022, max compression
```

## Comparing `pmagpy-cli-4.2.97.tar` & `pmagpy-cli-4.2.98.tar`

### file list

```diff
@@ -1,308 +1,308 @@
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.469155 pmagpy-cli-4.2.97/
--rw-r--r--   0 ltauxe     (501) staff       (20)      167 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/MANIFEST.in
--rw-r--r--   0 ltauxe     (501) staff       (20)     7956 2022-03-22 20:01:51.468718 pmagpy-cli-4.2.97/PKG-INFO
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7513 2021-03-22 16:05:20.000000 pmagpy-cli-4.2.97/README.md
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.337403 pmagpy-cli-4.2.97/SPD/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      326 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/SPD/__init__.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.339986 pmagpy-cli-4.2.97/SPD/lib/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      710 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/__init__.py
--rw-r--r--   0 ltauxe     (501) staff       (20)     3794 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/leastsq_jacobian.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3400 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_IZZI_MD.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3574 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_additivity_check_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    12899 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_arai_plot_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    12671 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_curvature.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9892 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_directional_statistics.py
--rw-r--r--   0 ltauxe     (501) staff       (20)     2375 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_leastsquares.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    10445 2020-02-07 04:43:37.000000 pmagpy-cli-4.2.97/SPD/lib/lib_ptrm_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2298 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/lib_tail_check_statistics.py
--rw-r--r--   0 ltauxe     (501) staff       (20)     2397 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/lib/new_lib_curvature.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)   104407 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/new_lj_thellier_gui_spd.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      319 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/SPD/run_tests.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    38099 2020-06-23 22:26:35.000000 pmagpy-cli-4.2.97/SPD/spd.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3635 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/test_instance.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.342095 pmagpy-cli-4.2.97/SPD/tests/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      664 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5234 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/SPD/tests/known_values.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3461 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/test_additivity_check_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      929 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/SPD/tests/test_all.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    18181 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/test_arai_plot_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2267 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/SPD/tests/test_curvature.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7512 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/test_directional_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7199 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/test_ptrm_statistics.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2520 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/SPD/tests/test_tail_check_statistics.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.345353 pmagpy-cli-4.2.97/bin/
--rw-r--r--   0 ltauxe     (501) staff       (20)      324 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/bin/ani_depthplot_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)      325 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/bin/core_depthplot_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)      320 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/bin/demag_gui_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)      321 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/bin/magic_gui2_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)      320 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/bin/magic_gui_anaconda
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      319 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/bin/pmag_gui_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)      323 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/bin/thellier_gui_anaconda
--rw-r--r--   0 ltauxe     (501) staff       (20)     6345 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/command_line_setup.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.350202 pmagpy-cli-4.2.97/dialogs/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    11299 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.97/dialogs/ErMagicBuilder.py
--rw-r--r--   0 ltauxe     (501) staff       (20)      694 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.97/dialogs/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    76159 2019-02-12 21:10:34.000000 pmagpy-cli-4.2.97/dialogs/demag_dialogs.py
--rw-r--r--   0 ltauxe     (501) staff       (20)    47902 2021-02-18 21:51:45.000000 pmagpy-cli-4.2.97/dialogs/demag_interpretation_editor.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    20519 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/dialogs/drop_down_menus3.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    53773 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.97/dialogs/grid_frame3.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.352290 pmagpy-cli-4.2.97/dialogs/help_files/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2226 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicAgeHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7171 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicBuilderHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1281 2019-05-03 14:11:24.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicHeadersHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1172 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicLocationHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2845 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSampleHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      925 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSampleHelp1.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2951 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSiteHelp.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      994 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSpecimenHelp.html
--rw-r--r--   0 ltauxe     (501) staff       (20)     6488 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/dialogs/help_files/magic_gui.html
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    22282 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/dialogs/magic_grid2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    24463 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.97/dialogs/magic_grid3.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    14887 2020-03-10 20:41:00.000000 pmagpy-cli-4.2.97/dialogs/pmag_er_magic_dialogs.py
--rw-r--r--   0 ltauxe     (501) staff       (20)   140430 2021-03-13 20:54:46.000000 pmagpy-cli-4.2.97/dialogs/pmag_gui_dialogs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9798 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.97/dialogs/pmag_gui_menu3.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    92478 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.97/dialogs/pmag_menu_dialogs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    45718 2021-03-15 20:57:30.000000 pmagpy-cli-4.2.97/dialogs/pmag_widgets.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    27187 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/dialogs/thellier_consistency_test.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    80057 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/dialogs/thellier_gui_dialogs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    15006 2020-03-05 23:54:00.000000 pmagpy-cli-4.2.97/dialogs/thellier_gui_lib.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    70728 2021-05-17 16:51:12.000000 pmagpy-cli-4.2.97/dialogs/thellier_interpreter.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.352913 pmagpy-cli-4.2.97/help_files/
--rw-r--r--   0 ltauxe     (501) staff       (20)       16 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/help_files/__init__.py
--rw-r--r--   0 ltauxe     (501) staff       (20)     4885 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/help_files/demag_gui_help.py
--rw-r--r--   0 ltauxe     (501) staff       (20)     4639 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/help_files/demag_interpretation_editor_help.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.353298 pmagpy-cli-4.2.97/locator/
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/locator/__init__.py
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/locator/resource.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.333981 pmagpy-cli-4.2.97/pmagpy/
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.358447 pmagpy-cli-4.2.97/pmagpy/data_model/
--rw-r--r--   0 ltauxe     (501) staff       (20)   168811 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy/data_model/MagIC-data-model.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)     1988 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/age_methods.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)    54547 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/all_codes.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)     2069 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/code_types.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)   303645 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies2.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   179238 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_August_9_2018.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   235187 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_December_10_2018.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   125757 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_February_6_2017.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   236158 2019-10-04 04:09:12.000000 pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_October_3_2019.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   342358 2020-03-03 20:13:56.000000 pmagpy-cli-4.2.97/pmagpy/data_model/data_model.json
--rw-r--r--   0 ltauxe     (501) staff       (20)     9249 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy/data_model/er_methods.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)    94254 2019-10-04 04:09:12.000000 pmagpy-cli-4.2.97/pmagpy/data_model/method_codes.json
--rw-r--r--   0 ltauxe     (501) staff       (20)     5620 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/pmag_methods.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)   160203 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_August_9_2018.json
--rw-r--r--   0 ltauxe     (501) staff       (20)    88937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_December_10_2018.json
--rw-r--r--   0 ltauxe     (501) staff       (20)   112229 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_February_6_2017.json
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.359204 pmagpy-cli-4.2.97/pmagpy/mapping/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      414 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/pmagpy/mapping/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    35331 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/pmagpy/mapping/map_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    18208 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/pmagpy/mapping/maps.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.360221 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/
--rw-r--r--   0 ltauxe     (501) staff       (20)     7956 2022-03-22 20:01:51.000000 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/PKG-INFO
--rw-r--r--   0 ltauxe     (501) staff       (20)     8526 2022-03-22 20:01:51.000000 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/SOURCES.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)        1 2022-03-22 20:01:51.000000 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/dependency_links.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)     7647 2022-03-22 20:01:51.000000 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/entry_points.txt
--rw-r--r--   0 ltauxe     (501) staff       (20)       60 2022-03-22 20:01:51.000000 pmagpy-cli-4.2.97/pmagpy_cli.egg-info/top_level.txt
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.334303 pmagpy-cli-4.2.97/pmagpy_tests/
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.360516 pmagpy-cli-4.2.97/pmagpy_tests/examples/
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy_tests/examples/__init__.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.360837 pmagpy-cli-4.2.97/pmagpy_tests/examples/empty_dir/
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy_tests/examples/empty_dir/__init__.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.361096 pmagpy-cli-4.2.97/pmagpy_tests/examples/my_project/
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy_tests/examples/my_project/__init__.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.361491 pmagpy-cli-4.2.97/pmagpy_tests/examples/my_project_with_errors/
--rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.97/pmagpy_tests/examples/my_project_with_errors/__init__.py
--rw-r--r--   0 ltauxe     (501) staff       (20)       88 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/pmagpy_tests/examples/my_project_with_errors/something.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.436881 pmagpy-cli-4.2.97/programs/
--rw-r--r--   0 ltauxe     (501) staff       (20)     1586 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2799 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/aarm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9777 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/agm_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2248 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/angle.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5110 2019-03-15 20:28:42.000000 pmagpy-cli-4.2.97/programs/ani_depthplot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5157 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/ani_depthplot2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7373 2020-02-24 23:28:08.000000 pmagpy-cli-4.2.97/programs/aniso_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    27211 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/aniso_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3732 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/apwp.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2209 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/atrm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3475 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/azdip_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1862 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/b_vdm.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2924 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/bootams.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2287 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/cart_dir.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1175 2019-06-13 19:51:45.000000 pmagpy-cli-4.2.97/programs/chartmaker.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1310 2019-03-12 20:36:43.000000 pmagpy-cli-4.2.97/programs/chi_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    10879 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/chi_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2141 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/combine_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2637 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/common_mean.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.455426 pmagpy-cli-4.2.97/programs/conversion_scripts/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5878 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/_2g_bin_magic.py
--rw-r--r--   0 ltauxe     (501) staff       (20)      717 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3663 2021-04-16 21:42:14.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/agm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4644 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/bgc_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5133 2020-11-07 00:13:09.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/cit_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9043 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/generic_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7160 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/huji_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3816 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/huji_sample_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2433 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_dscr_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2644 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_jr6_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1045 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_samples_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2638 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_srm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3055 2021-07-27 03:15:09.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/irm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4474 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/jr6_jr6_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4567 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/jr6_txt_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3546 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/k15_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4911 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/kly4s_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6352 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/ldeo_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    19399 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/livdb_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    16137 2021-07-27 03:15:09.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/magic_geomagia.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3220 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/mst_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3224 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/pmd_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4089 2021-05-03 22:11:24.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/run_multi_samples.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3590 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/s_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9292 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/sio_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    33307 2020-12-08 19:59:19.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/squidm_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5813 2020-07-13 03:20:10.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/sufar4_asc_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    21369 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/tdt_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4695 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/template_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4422 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/utrecht_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5817 2021-06-29 21:58:11.000000 pmagpy-cli-4.2.97/programs/conversion_scripts/xpeem_magic.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.466025 pmagpy-cli-4.2.97/programs/conversion_scripts2/
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    19342 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/_2g_bin_magic2.py
--rw-r--r--   0 ltauxe     (501) staff       (20)      645 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/__init__.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     8598 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/bgc_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    19762 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/cit_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    43057 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/generic_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    27908 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/huji_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    28336 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/huji_magic_new2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9728 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_dscr_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9341 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_jr6_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    15484 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_srm_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    11785 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/jr6_jr6_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    11399 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/jr6_txt_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    15885 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/ldeo_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    10840 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/pmd_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    32445 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/sio_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    52404 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/tdt_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    16592 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/conversion_scripts2/utrecht_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      595 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/convert2unix.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     8467 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/core_depthplot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9123 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/curie.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1339 2019-04-19 05:24:35.000000 pmagpy-cli-4.2.97/programs/dayplot_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5111 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dayplot_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)   402031 2021-05-21 23:44:51.000000 pmagpy-cli-4.2.97/programs/demag_gui.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1144 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/di_eq.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1872 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/di_geo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2186 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/di_rot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1917 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/di_tilt.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3026 2019-06-26 20:39:29.000000 pmagpy-cli-4.2.97/programs/di_vgp.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3475 2020-07-30 23:57:37.000000 pmagpy-cli-4.2.97/programs/dia_vgp.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1214 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dipole_pinc.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1221 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dipole_plat.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2198 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dir_cart.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2657 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dir_redo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2595 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.97/programs/dmag_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6182 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/dmag_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2240 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/download_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1674 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/eigs_s.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1780 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/eq_di.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3024 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/eqarea.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    10107 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/eqarea_ell.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3665 2019-01-12 20:35:12.000000 pmagpy-cli-4.2.97/programs/eqarea_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    19351 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/eqarea_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5048 2021-06-11 23:02:59.000000 pmagpy-cli-4.2.97/programs/find_ei.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1393 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/fisher.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5671 2021-06-17 20:57:22.000000 pmagpy-cli-4.2.97/programs/fishqq.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1796 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/fishrot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6053 2021-01-14 22:38:11.000000 pmagpy-cli-4.2.97/programs/foldtest.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9946 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/foldtest_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7984 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/foldtest_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    13145 2019-06-26 20:39:29.000000 pmagpy-cli-4.2.97/programs/forc_diagram.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1441 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/gaussian.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2022 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/gobing.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1976 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/gofish.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2272 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/gokent.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2135 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/goprinc.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1162 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/grab_magic_key.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1769 2019-05-10 11:15:55.000000 pmagpy-cli-4.2.97/programs/histplot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1746 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/hysteresis_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    13221 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/hysteresis_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7391 2020-11-29 01:36:58.000000 pmagpy-cli-4.2.97/programs/igrf.py
-drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-22 20:01:51.468039 pmagpy-cli-4.2.97/programs/images/
--rw-r--r--   0 ltauxe     (501) staff       (20)   203040 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.97/programs/images/PmagPy.ico
--rw-r--r--   0 ltauxe     (501) staff       (20)     1150 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.97/programs/images/PmagPy_16x16.ico
--rw-r--r--   0 ltauxe     (501) staff       (20)     4286 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.97/programs/images/PmagPy_32x32.ico
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1761 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/incfish.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2652 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/install_etopo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    23725 2021-10-24 20:19:26.000000 pmagpy-cli-4.2.97/programs/irm_unmix.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6781 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/irmaq_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3152 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/k15_s.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7909 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/lnp_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1727 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/lowes.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4410 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/lowrie.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4567 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/lowrie_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5377 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/lsq_redo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    19236 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.97/programs/magic_gui.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3228 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/magic_select.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    25127 2020-03-17 22:34:25.000000 pmagpy-cli-4.2.97/programs/make_magic_plots.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    25307 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/microwave_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3316 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/mk_redo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2706 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.97/programs/move_data_files.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3216 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/mst_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6870 2019-01-11 23:20:51.000000 pmagpy-cli-4.2.97/programs/orientation_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2750 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/pca.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1652 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_2cdfs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1617 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_cdf.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4592 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_geomagia.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5279 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_magmap.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_magmap_basemap.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     7147 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plot_map_pts.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2721 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plotdi_a.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9892 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plotdi_e.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4183 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/plotxy.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    34718 2021-10-11 17:45:37.000000 pmagpy-cli-4.2.97/programs/pmag_gui.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1411 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/pmag_results_extract.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2550 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/pmm_redo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3453 2019-02-05 21:11:03.000000 pmagpy-cli-4.2.97/programs/polemap_magic.py
--rw-r--r--   0 ltauxe     (501) staff       (20)      295 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.97/programs/program_envs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5446 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/pt_rot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2180 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/qqplot.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1916 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/qqunf.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1487 2019-04-13 05:05:12.000000 pmagpy-cli-4.2.97/programs/quick_hyst.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     9268 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/quick_hyst2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    27367 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/remanence_anisotropy_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)      392 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/remove_bad_chars.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3444 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/replace_ac_specimens.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2187 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/revtest.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4886 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/revtest_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6688 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/revtest_mm1990.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1741 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/s_eigs.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1741 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/s_geo.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3258 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/s_hext.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1814 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/s_tilt.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2683 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/scalc.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/scalc_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    11126 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/site_edit_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2541 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/sort_specimens.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1534 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/squish.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1632 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/stats.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    14657 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/strip_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2921 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/sundec.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)   405936 2021-11-20 18:45:10.000000 pmagpy-cli-4.2.97/programs/thellier_gui.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4250 2019-03-15 20:28:42.000000 pmagpy-cli-4.2.97/programs/thellier_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    36588 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/thellier_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     4730 2020-02-11 20:52:36.000000 pmagpy-cli-4.2.97/programs/thumbnails.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2295 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/tk03.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     6492 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/trmaq_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1008 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/uniform.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1630 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/unsquish.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1392 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/upload_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1698 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/vdm_b.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     1322 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/vector_mean.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2751 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/vgp_di.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3240 2019-04-17 07:12:20.000000 pmagpy-cli-4.2.97/programs/vgpmap_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     8701 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/vgpmap_magic2.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     2246 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/watsons_f.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     5236 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/watsons_v.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    10254 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/zeq.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)     3183 2019-03-29 02:40:45.000000 pmagpy-cli-4.2.97/programs/zeq_magic.py
--rwxr-xr-x   0 ltauxe     (501) staff       (20)    43374 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.97/programs/zeq_magic2.py
--rw-r--r--   0 ltauxe     (501) staff       (20)       38 2022-03-22 20:01:51.469265 pmagpy-cli-4.2.97/setup.cfg
--rw-r--r--   0 ltauxe     (501) staff       (20)     7858 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.97/setup.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.278784 pmagpy-cli-4.2.98/
+-rw-r--r--   0 ltauxe     (501) staff       (20)      167 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/MANIFEST.in
+-rw-r--r--   0 ltauxe     (501) staff       (20)     7956 2022-03-25 00:16:18.278564 pmagpy-cli-4.2.98/PKG-INFO
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7513 2021-03-22 16:05:20.000000 pmagpy-cli-4.2.98/README.md
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.143121 pmagpy-cli-4.2.98/SPD/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      326 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/SPD/__init__.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.147393 pmagpy-cli-4.2.98/SPD/lib/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      710 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/__init__.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)     3794 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/leastsq_jacobian.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3400 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_IZZI_MD.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3574 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_additivity_check_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    12899 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_arai_plot_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    12671 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_curvature.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9892 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_directional_statistics.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)     2375 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_leastsquares.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    10445 2020-02-07 04:43:37.000000 pmagpy-cli-4.2.98/SPD/lib/lib_ptrm_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2298 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/lib_tail_check_statistics.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)     2397 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/lib/new_lib_curvature.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)   104407 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/new_lj_thellier_gui_spd.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      319 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/SPD/run_tests.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    38099 2020-06-23 22:26:35.000000 pmagpy-cli-4.2.98/SPD/spd.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3635 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/test_instance.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.150147 pmagpy-cli-4.2.98/SPD/tests/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      664 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5234 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/SPD/tests/known_values.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3461 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/test_additivity_check_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      929 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/SPD/tests/test_all.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    18181 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/test_arai_plot_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2267 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/SPD/tests/test_curvature.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7512 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/test_directional_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7199 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/test_ptrm_statistics.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2520 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/SPD/tests/test_tail_check_statistics.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.153229 pmagpy-cli-4.2.98/bin/
+-rw-r--r--   0 ltauxe     (501) staff       (20)      324 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/bin/ani_depthplot_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)      325 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/bin/core_depthplot_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)      320 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/bin/demag_gui_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)      321 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/bin/magic_gui2_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)      320 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/bin/magic_gui_anaconda
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      319 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/bin/pmag_gui_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)      323 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/bin/thellier_gui_anaconda
+-rw-r--r--   0 ltauxe     (501) staff       (20)     6345 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/command_line_setup.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.158207 pmagpy-cli-4.2.98/dialogs/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    11299 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.98/dialogs/ErMagicBuilder.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)      694 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.98/dialogs/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    76159 2019-02-12 21:10:34.000000 pmagpy-cli-4.2.98/dialogs/demag_dialogs.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)    47902 2021-02-18 21:51:45.000000 pmagpy-cli-4.2.98/dialogs/demag_interpretation_editor.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    20519 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/dialogs/drop_down_menus3.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    53773 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.98/dialogs/grid_frame3.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.160751 pmagpy-cli-4.2.98/dialogs/help_files/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2226 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicAgeHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7171 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicBuilderHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1281 2019-05-03 14:11:24.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicHeadersHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1172 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicLocationHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2845 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSampleHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      925 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSampleHelp1.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2951 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSiteHelp.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      994 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSpecimenHelp.html
+-rw-r--r--   0 ltauxe     (501) staff       (20)     6488 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/dialogs/help_files/magic_gui.html
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    22282 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/dialogs/magic_grid2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    24463 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.98/dialogs/magic_grid3.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    14887 2020-03-10 20:41:00.000000 pmagpy-cli-4.2.98/dialogs/pmag_er_magic_dialogs.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)   140430 2021-03-13 20:54:46.000000 pmagpy-cli-4.2.98/dialogs/pmag_gui_dialogs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9798 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.98/dialogs/pmag_gui_menu3.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    92478 2019-06-12 03:08:16.000000 pmagpy-cli-4.2.98/dialogs/pmag_menu_dialogs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    45718 2021-03-15 20:57:30.000000 pmagpy-cli-4.2.98/dialogs/pmag_widgets.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    27187 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/dialogs/thellier_consistency_test.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    80057 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/dialogs/thellier_gui_dialogs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    15006 2020-03-05 23:54:00.000000 pmagpy-cli-4.2.98/dialogs/thellier_gui_lib.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    70728 2021-05-17 16:51:12.000000 pmagpy-cli-4.2.98/dialogs/thellier_interpreter.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.161523 pmagpy-cli-4.2.98/help_files/
+-rw-r--r--   0 ltauxe     (501) staff       (20)       16 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/help_files/__init__.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)     4885 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/help_files/demag_gui_help.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)     4639 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/help_files/demag_interpretation_editor_help.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.161925 pmagpy-cli-4.2.98/locator/
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/locator/__init__.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/locator/resource.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.138813 pmagpy-cli-4.2.98/pmagpy/
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.167961 pmagpy-cli-4.2.98/pmagpy/data_model/
+-rw-r--r--   0 ltauxe     (501) staff       (20)   168811 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy/data_model/MagIC-data-model.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)     1988 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/age_methods.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)    54547 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/all_codes.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)     2069 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/code_types.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)   303645 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies2.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   179238 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_August_9_2018.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   235187 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_December_10_2018.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   125757 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_February_6_2017.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   236158 2019-10-04 04:09:12.000000 pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_October_3_2019.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   342358 2020-03-03 20:13:56.000000 pmagpy-cli-4.2.98/pmagpy/data_model/data_model.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)     9249 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy/data_model/er_methods.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)    94254 2019-10-04 04:09:12.000000 pmagpy-cli-4.2.98/pmagpy/data_model/method_codes.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)     5620 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/pmag_methods.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)   160203 2019-01-06 01:38:43.000000 pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_August_9_2018.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)    88937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_December_10_2018.json
+-rw-r--r--   0 ltauxe     (501) staff       (20)   112229 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_February_6_2017.json
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.168799 pmagpy-cli-4.2.98/pmagpy/mapping/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      414 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/pmagpy/mapping/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    35331 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/pmagpy/mapping/map_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    18208 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/pmagpy/mapping/maps.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.169946 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/
+-rw-r--r--   0 ltauxe     (501) staff       (20)     7956 2022-03-25 00:16:18.000000 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/PKG-INFO
+-rw-r--r--   0 ltauxe     (501) staff       (20)     8526 2022-03-25 00:16:18.000000 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)        1 2022-03-25 00:16:18.000000 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)     7647 2022-03-25 00:16:18.000000 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/entry_points.txt
+-rw-r--r--   0 ltauxe     (501) staff       (20)       60 2022-03-25 00:16:18.000000 pmagpy-cli-4.2.98/pmagpy_cli.egg-info/top_level.txt
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.139135 pmagpy-cli-4.2.98/pmagpy_tests/
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.170160 pmagpy-cli-4.2.98/pmagpy_tests/examples/
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy_tests/examples/__init__.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.170329 pmagpy-cli-4.2.98/pmagpy_tests/examples/empty_dir/
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy_tests/examples/empty_dir/__init__.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.170500 pmagpy-cli-4.2.98/pmagpy_tests/examples/my_project/
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy_tests/examples/my_project/__init__.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.170922 pmagpy-cli-4.2.98/pmagpy_tests/examples/my_project_with_errors/
+-rw-r--r--   0 ltauxe     (501) staff       (20)        0 2018-11-21 00:00:34.000000 pmagpy-cli-4.2.98/pmagpy_tests/examples/my_project_with_errors/__init__.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)       88 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/pmagpy_tests/examples/my_project_with_errors/something.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.242620 pmagpy-cli-4.2.98/programs/
+-rw-r--r--   0 ltauxe     (501) staff       (20)     1586 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2799 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/aarm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9777 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/agm_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2248 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/angle.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5110 2019-03-15 20:28:42.000000 pmagpy-cli-4.2.98/programs/ani_depthplot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5157 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/ani_depthplot2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7373 2020-02-24 23:28:08.000000 pmagpy-cli-4.2.98/programs/aniso_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    27211 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/aniso_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3732 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/apwp.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2209 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/atrm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3475 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/azdip_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1862 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/b_vdm.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2924 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/bootams.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2287 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/cart_dir.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1175 2019-06-13 19:51:45.000000 pmagpy-cli-4.2.98/programs/chartmaker.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1310 2019-03-12 20:36:43.000000 pmagpy-cli-4.2.98/programs/chi_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    10879 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/chi_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2141 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/combine_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2637 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/common_mean.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.267037 pmagpy-cli-4.2.98/programs/conversion_scripts/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5878 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/_2g_bin_magic.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)      717 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3663 2021-04-16 21:42:14.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/agm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4644 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/bgc_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5133 2020-11-07 00:13:09.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/cit_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9043 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/generic_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7160 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/huji_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3816 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/huji_sample_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2433 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_dscr_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2644 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_jr6_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1045 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_samples_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2638 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_srm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3055 2021-07-27 03:15:09.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/irm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4474 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/jr6_jr6_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4567 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/jr6_txt_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3546 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/k15_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4911 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/kly4s_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6352 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/ldeo_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    19399 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/livdb_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    16137 2021-07-27 03:15:09.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/magic_geomagia.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3220 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/mst_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3224 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/pmd_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4089 2021-05-03 22:11:24.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/run_multi_samples.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3590 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/s_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9292 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/sio_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    33307 2020-12-08 19:59:19.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/squidm_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5813 2020-07-13 03:20:10.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/sufar4_asc_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    21411 2022-03-23 23:57:57.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/tdt_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4695 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/template_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4422 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/utrecht_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5817 2021-06-29 21:58:11.000000 pmagpy-cli-4.2.98/programs/conversion_scripts/xpeem_magic.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.277137 pmagpy-cli-4.2.98/programs/conversion_scripts2/
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    19342 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/_2g_bin_magic2.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)      645 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/__init__.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     8598 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/bgc_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    19762 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/cit_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    43057 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/generic_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    27908 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/huji_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    28336 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/huji_magic_new2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9728 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_dscr_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9341 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_jr6_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    15484 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_srm_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    11785 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/jr6_jr6_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    11399 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/jr6_txt_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    15885 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/ldeo_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    10840 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/pmd_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    32445 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/sio_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    52404 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/tdt_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    16592 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/conversion_scripts2/utrecht_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      595 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/convert2unix.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     8467 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/core_depthplot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9123 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/curie.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1339 2019-04-19 05:24:35.000000 pmagpy-cli-4.2.98/programs/dayplot_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5111 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dayplot_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)   402031 2021-05-21 23:44:51.000000 pmagpy-cli-4.2.98/programs/demag_gui.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1144 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/di_eq.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1872 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/di_geo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2186 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/di_rot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1917 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/di_tilt.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3026 2019-06-26 20:39:29.000000 pmagpy-cli-4.2.98/programs/di_vgp.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3475 2020-07-30 23:57:37.000000 pmagpy-cli-4.2.98/programs/dia_vgp.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1214 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dipole_pinc.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1221 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dipole_plat.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2198 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dir_cart.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2657 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dir_redo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2595 2019-05-29 22:22:29.000000 pmagpy-cli-4.2.98/programs/dmag_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6182 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/dmag_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2240 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/download_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1674 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/eigs_s.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1780 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/eq_di.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3024 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/eqarea.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    10107 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/eqarea_ell.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3665 2019-01-12 20:35:12.000000 pmagpy-cli-4.2.98/programs/eqarea_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    19351 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/eqarea_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5048 2021-06-11 23:02:59.000000 pmagpy-cli-4.2.98/programs/find_ei.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1393 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/fisher.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5671 2021-06-17 20:57:22.000000 pmagpy-cli-4.2.98/programs/fishqq.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1796 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/fishrot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6053 2021-01-14 22:38:11.000000 pmagpy-cli-4.2.98/programs/foldtest.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9946 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/foldtest_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7984 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/foldtest_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    13145 2019-06-26 20:39:29.000000 pmagpy-cli-4.2.98/programs/forc_diagram.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1441 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/gaussian.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2022 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/gobing.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1976 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/gofish.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2272 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/gokent.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2135 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/goprinc.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1162 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/grab_magic_key.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1769 2019-05-10 11:15:55.000000 pmagpy-cli-4.2.98/programs/histplot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1746 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/hysteresis_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    13221 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/hysteresis_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7391 2020-11-29 01:36:58.000000 pmagpy-cli-4.2.98/programs/igrf.py
+drwxr-xr-x   0 ltauxe     (501) staff       (20)        0 2022-03-25 00:16:18.278265 pmagpy-cli-4.2.98/programs/images/
+-rw-r--r--   0 ltauxe     (501) staff       (20)   203040 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.98/programs/images/PmagPy.ico
+-rw-r--r--   0 ltauxe     (501) staff       (20)     1150 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.98/programs/images/PmagPy_16x16.ico
+-rw-r--r--   0 ltauxe     (501) staff       (20)     4286 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.98/programs/images/PmagPy_32x32.ico
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1761 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/incfish.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2652 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/install_etopo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    23725 2021-10-24 20:19:26.000000 pmagpy-cli-4.2.98/programs/irm_unmix.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6781 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/irmaq_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3152 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/k15_s.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7909 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/lnp_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1727 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/lowes.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4410 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/lowrie.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4567 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/lowrie_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5377 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/lsq_redo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    19236 2021-10-08 21:24:03.000000 pmagpy-cli-4.2.98/programs/magic_gui.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3228 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/magic_select.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    26603 2022-03-25 00:11:44.000000 pmagpy-cli-4.2.98/programs/make_magic_plots.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    25307 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/microwave_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3316 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/mk_redo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2706 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.98/programs/move_data_files.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3216 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/mst_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6870 2019-01-11 23:20:51.000000 pmagpy-cli-4.2.98/programs/orientation_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2750 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/pca.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1652 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_2cdfs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1617 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_cdf.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4592 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_geomagia.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5279 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_magmap.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_magmap_basemap.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     7147 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plot_map_pts.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2721 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plotdi_a.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9892 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plotdi_e.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4183 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/plotxy.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    34718 2021-10-11 17:45:37.000000 pmagpy-cli-4.2.98/programs/pmag_gui.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1411 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/pmag_results_extract.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2550 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/pmm_redo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3453 2019-02-05 21:11:03.000000 pmagpy-cli-4.2.98/programs/polemap_magic.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)      295 2018-11-21 00:00:35.000000 pmagpy-cli-4.2.98/programs/program_envs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5446 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/pt_rot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2180 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/qqplot.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1916 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/qqunf.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1487 2019-04-13 05:05:12.000000 pmagpy-cli-4.2.98/programs/quick_hyst.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     9268 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/quick_hyst2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    27367 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/remanence_anisotropy_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)      392 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/remove_bad_chars.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3444 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/replace_ac_specimens.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2187 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/revtest.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4886 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/revtest_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6688 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/revtest_mm1990.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1741 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/s_eigs.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1741 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/s_geo.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3258 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/s_hext.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1814 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/s_tilt.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2683 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/scalc.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3937 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/scalc_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    11126 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/site_edit_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2541 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/sort_specimens.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1534 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/squish.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1632 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/stats.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    14657 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/strip_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2921 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/sundec.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)   405936 2021-11-20 18:45:10.000000 pmagpy-cli-4.2.98/programs/thellier_gui.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4250 2019-03-15 20:28:42.000000 pmagpy-cli-4.2.98/programs/thellier_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    36588 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/thellier_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     4730 2020-02-11 20:52:36.000000 pmagpy-cli-4.2.98/programs/thumbnails.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2295 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/tk03.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     6492 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/trmaq_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1008 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/uniform.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1630 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/unsquish.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1392 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/upload_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1698 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/vdm_b.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     1322 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/vector_mean.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2751 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/vgp_di.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3240 2019-04-17 07:12:20.000000 pmagpy-cli-4.2.98/programs/vgpmap_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     8701 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/vgpmap_magic2.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     2246 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/watsons_f.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     5236 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/watsons_v.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    10254 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/zeq.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)     3183 2019-03-29 02:40:45.000000 pmagpy-cli-4.2.98/programs/zeq_magic.py
+-rwxr-xr-x   0 ltauxe     (501) staff       (20)    43374 2019-01-06 01:38:44.000000 pmagpy-cli-4.2.98/programs/zeq_magic2.py
+-rw-r--r--   0 ltauxe     (501) staff       (20)       38 2022-03-25 00:16:18.278851 pmagpy-cli-4.2.98/setup.cfg
+-rw-r--r--   0 ltauxe     (501) staff       (20)     7858 2019-06-03 23:28:45.000000 pmagpy-cli-4.2.98/setup.py
```

### Comparing `pmagpy-cli-4.2.97/PKG-INFO` & `pmagpy-cli-4.2.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmagpy-cli
-Version: 4.2.97
+Version: 4.2.98
 Summary: Analysis tools for paleo/rock magnetic data
 Home-page: https://github.com/PmagPy/PmagPy
 Author: PmagPy team
 Author-email: ltauxe@ucsd.edu
 License: BSD-3
 Keywords: geology paleomagnetism
 Platform: UNKNOWN
```

### Comparing `pmagpy-cli-4.2.97/README.md` & `pmagpy-cli-4.2.98/README.md`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/__init__.py` & `pmagpy-cli-4.2.98/SPD/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/leastsq_jacobian.py` & `pmagpy-cli-4.2.98/SPD/lib/leastsq_jacobian.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_IZZI_MD.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_IZZI_MD.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_additivity_check_statistics.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_additivity_check_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_arai_plot_statistics.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_arai_plot_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_curvature.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_curvature.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_directional_statistics.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_directional_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_leastsquares.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_leastsquares.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_ptrm_statistics.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_ptrm_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/lib_tail_check_statistics.py` & `pmagpy-cli-4.2.98/SPD/lib/lib_tail_check_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/lib/new_lib_curvature.py` & `pmagpy-cli-4.2.98/SPD/lib/new_lib_curvature.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/new_lj_thellier_gui_spd.py` & `pmagpy-cli-4.2.98/SPD/new_lj_thellier_gui_spd.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/spd.py` & `pmagpy-cli-4.2.98/SPD/spd.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/test_instance.py` & `pmagpy-cli-4.2.98/SPD/test_instance.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/__init__.py` & `pmagpy-cli-4.2.98/SPD/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/known_values.py` & `pmagpy-cli-4.2.98/SPD/tests/known_values.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_additivity_check_statistics.py` & `pmagpy-cli-4.2.98/SPD/tests/test_additivity_check_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_all.py` & `pmagpy-cli-4.2.98/SPD/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_arai_plot_statistics.py` & `pmagpy-cli-4.2.98/SPD/tests/test_arai_plot_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_curvature.py` & `pmagpy-cli-4.2.98/SPD/tests/test_curvature.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_directional_statistics.py` & `pmagpy-cli-4.2.98/SPD/tests/test_directional_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_ptrm_statistics.py` & `pmagpy-cli-4.2.98/SPD/tests/test_ptrm_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/SPD/tests/test_tail_check_statistics.py` & `pmagpy-cli-4.2.98/SPD/tests/test_tail_check_statistics.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/command_line_setup.py` & `pmagpy-cli-4.2.98/command_line_setup.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/ErMagicBuilder.py` & `pmagpy-cli-4.2.98/dialogs/ErMagicBuilder.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/__init__.py` & `pmagpy-cli-4.2.98/dialogs/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/demag_dialogs.py` & `pmagpy-cli-4.2.98/dialogs/demag_dialogs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/demag_interpretation_editor.py` & `pmagpy-cli-4.2.98/dialogs/demag_interpretation_editor.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/drop_down_menus3.py` & `pmagpy-cli-4.2.98/dialogs/drop_down_menus3.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/grid_frame3.py` & `pmagpy-cli-4.2.98/dialogs/grid_frame3.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicAgeHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicAgeHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicBuilderHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicBuilderHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicHeadersHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicHeadersHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicLocationHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicLocationHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSampleHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSampleHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSampleHelp1.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSampleHelp1.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSiteHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSiteHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/ErMagicSpecimenHelp.html` & `pmagpy-cli-4.2.98/dialogs/help_files/ErMagicSpecimenHelp.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/help_files/magic_gui.html` & `pmagpy-cli-4.2.98/dialogs/help_files/magic_gui.html`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/magic_grid2.py` & `pmagpy-cli-4.2.98/dialogs/magic_grid2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/magic_grid3.py` & `pmagpy-cli-4.2.98/dialogs/magic_grid3.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/pmag_er_magic_dialogs.py` & `pmagpy-cli-4.2.98/dialogs/pmag_er_magic_dialogs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/pmag_gui_dialogs.py` & `pmagpy-cli-4.2.98/dialogs/pmag_gui_dialogs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/pmag_gui_menu3.py` & `pmagpy-cli-4.2.98/dialogs/pmag_gui_menu3.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/pmag_menu_dialogs.py` & `pmagpy-cli-4.2.98/dialogs/pmag_menu_dialogs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/pmag_widgets.py` & `pmagpy-cli-4.2.98/dialogs/pmag_widgets.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/thellier_consistency_test.py` & `pmagpy-cli-4.2.98/dialogs/thellier_consistency_test.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/thellier_gui_dialogs.py` & `pmagpy-cli-4.2.98/dialogs/thellier_gui_dialogs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/thellier_gui_lib.py` & `pmagpy-cli-4.2.98/dialogs/thellier_gui_lib.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/dialogs/thellier_interpreter.py` & `pmagpy-cli-4.2.98/dialogs/thellier_interpreter.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/help_files/demag_gui_help.py` & `pmagpy-cli-4.2.98/help_files/demag_gui_help.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/help_files/demag_interpretation_editor_help.py` & `pmagpy-cli-4.2.98/help_files/demag_interpretation_editor_help.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/MagIC-data-model.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/MagIC-data-model.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/age_methods.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/age_methods.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/all_codes.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/all_codes.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/code_types.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/code_types.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies2.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies2.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_August_9_2018.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_August_9_2018.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_December_10_2018.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_December_10_2018.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_February_6_2017.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_February_6_2017.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/controlled_vocabularies_October_3_2019.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/controlled_vocabularies_October_3_2019.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/data_model.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/data_model.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/er_methods.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/er_methods.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/method_codes.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/method_codes.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/pmag_methods.txt` & `pmagpy-cli-4.2.98/pmagpy/data_model/pmag_methods.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_August_9_2018.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_August_9_2018.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_December_10_2018.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_December_10_2018.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/data_model/suggested_vocabularies_February_6_2017.json` & `pmagpy-cli-4.2.98/pmagpy/data_model/suggested_vocabularies_February_6_2017.json`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/mapping/map_magic.py` & `pmagpy-cli-4.2.98/pmagpy/mapping/map_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy/mapping/maps.py` & `pmagpy-cli-4.2.98/pmagpy/mapping/maps.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy_cli.egg-info/PKG-INFO` & `pmagpy-cli-4.2.98/pmagpy_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pmagpy-cli
-Version: 4.2.97
+Version: 4.2.98
 Summary: Analysis tools for paleo/rock magnetic data
 Home-page: https://github.com/PmagPy/PmagPy
 Author: PmagPy team
 Author-email: ltauxe@ucsd.edu
 License: BSD-3
 Keywords: geology paleomagnetism
 Platform: UNKNOWN
```

### Comparing `pmagpy-cli-4.2.97/pmagpy_cli.egg-info/SOURCES.txt` & `pmagpy-cli-4.2.98/pmagpy_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/pmagpy_cli.egg-info/entry_points.txt` & `pmagpy-cli-4.2.98/pmagpy_cli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/__init__.py` & `pmagpy-cli-4.2.98/programs/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/aarm_magic.py` & `pmagpy-cli-4.2.98/programs/aarm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/agm_magic2.py` & `pmagpy-cli-4.2.98/programs/agm_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/angle.py` & `pmagpy-cli-4.2.98/programs/angle.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/ani_depthplot.py` & `pmagpy-cli-4.2.98/programs/ani_depthplot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/ani_depthplot2.py` & `pmagpy-cli-4.2.98/programs/ani_depthplot2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/aniso_magic.py` & `pmagpy-cli-4.2.98/programs/aniso_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/aniso_magic2.py` & `pmagpy-cli-4.2.98/programs/aniso_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/apwp.py` & `pmagpy-cli-4.2.98/programs/apwp.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/atrm_magic.py` & `pmagpy-cli-4.2.98/programs/atrm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/azdip_magic.py` & `pmagpy-cli-4.2.98/programs/azdip_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/b_vdm.py` & `pmagpy-cli-4.2.98/programs/b_vdm.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/bootams.py` & `pmagpy-cli-4.2.98/programs/bootams.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/cart_dir.py` & `pmagpy-cli-4.2.98/programs/cart_dir.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/chartmaker.py` & `pmagpy-cli-4.2.98/programs/chartmaker.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/chi_magic.py` & `pmagpy-cli-4.2.98/programs/chi_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/chi_magic2.py` & `pmagpy-cli-4.2.98/programs/chi_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/combine_magic.py` & `pmagpy-cli-4.2.98/programs/combine_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/common_mean.py` & `pmagpy-cli-4.2.98/programs/common_mean.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/_2g_bin_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/_2g_bin_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/__init__.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/agm_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/agm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/bgc_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/bgc_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/cit_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/cit_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/generic_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/generic_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/huji_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/huji_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/huji_sample_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/huji_sample_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_dscr_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_dscr_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_jr6_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_jr6_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_samples_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_samples_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/iodp_srm_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/iodp_srm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/irm_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/irm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/jr6_jr6_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/jr6_jr6_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/jr6_txt_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/jr6_txt_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/k15_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/k15_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/kly4s_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/kly4s_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/ldeo_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/ldeo_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/livdb_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/livdb_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/magic_geomagia.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/magic_geomagia.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/mst_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/mst_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/pmd_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/pmd_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/run_multi_samples.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/run_multi_samples.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/s_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/s_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/sio_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/sio_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/squidm_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/squidm_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/sufar4_asc_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/sufar4_asc_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/tdt_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/tdt_magic.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import matplotlib
 matplotlib.use('WXAgg')
 
 import wx
 import sys
 import os
 from dialogs import pmag_widgets as pw
-from pmagpy import convert_2_magic as convert
+#from pmagpy import convert_2_magic as convert
 import pmagpy.contribution_builder as cb
 import pmagpy.pmag as pmag
 from pmagpy import ipmag
 from pmagpy import convert_2_magic
 
 # ===========================================
 # GUI
@@ -424,20 +424,20 @@
 
             # create temporary outfile name
             meas_file = os.path.join(self.WD, 'measurements_{}.txt'.format(i))
             spec_file = os.path.join(self.WD, 'specimens_{}.txt'.format(i))
             samp_file = os.path.join(self.WD, 'samples_{}.txt'.format(i))
             site_file = os.path.join(self.WD, 'sites_{}.txt'.format(i))
             loc_file = os.path.join(self.WD, 'locations_{}.txt'.format(i))
-
+            spec_name_con=1
             if dir_path:
                 res, fname = convert_2_magic.tdt(dir_path, experiment, meas_file,
                                                  spec_file, samp_file,
                                                  site_file, loc_file,
-                                                 user_name, location_name, lab_dec, lab_inc, moment_units,
+                                                 user_name, location_name, lab_dec, lab_inc, moment_units,spec_name_con,
                                                  samp_name_con, samp_name_chars,
                                                  site_name_con, site_name_chars, volume,
                                                  output_dir_path=self.WD)
                 outfiles.append(fname)
 
         # combine measurement files
         ipmag.combine_magic(outfiles, self.output_file_path.GetValue(), magic_table="measurements")
```

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/template_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/template_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/utrecht_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/utrecht_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts/xpeem_magic.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts/xpeem_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/_2g_bin_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/_2g_bin_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/__init__.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/__init__.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/bgc_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/bgc_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/cit_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/cit_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/generic_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/generic_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/huji_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/huji_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/huji_magic_new2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/huji_magic_new2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_dscr_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_dscr_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_jr6_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_jr6_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/iodp_srm_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/iodp_srm_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/jr6_jr6_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/jr6_jr6_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/jr6_txt_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/jr6_txt_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/ldeo_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/ldeo_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/pmd_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/pmd_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/sio_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/sio_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/tdt_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/tdt_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/conversion_scripts2/utrecht_magic2.py` & `pmagpy-cli-4.2.98/programs/conversion_scripts2/utrecht_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/convert2unix.py` & `pmagpy-cli-4.2.98/programs/convert2unix.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/core_depthplot.py` & `pmagpy-cli-4.2.98/programs/core_depthplot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/curie.py` & `pmagpy-cli-4.2.98/programs/curie.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dayplot_magic.py` & `pmagpy-cli-4.2.98/programs/dayplot_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dayplot_magic2.py` & `pmagpy-cli-4.2.98/programs/dayplot_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/demag_gui.py` & `pmagpy-cli-4.2.98/programs/demag_gui.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/di_eq.py` & `pmagpy-cli-4.2.98/programs/di_eq.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/di_geo.py` & `pmagpy-cli-4.2.98/programs/di_geo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/di_rot.py` & `pmagpy-cli-4.2.98/programs/di_rot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/di_tilt.py` & `pmagpy-cli-4.2.98/programs/di_tilt.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/di_vgp.py` & `pmagpy-cli-4.2.98/programs/di_vgp.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dia_vgp.py` & `pmagpy-cli-4.2.98/programs/dia_vgp.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dipole_pinc.py` & `pmagpy-cli-4.2.98/programs/dipole_pinc.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dipole_plat.py` & `pmagpy-cli-4.2.98/programs/dipole_plat.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dir_cart.py` & `pmagpy-cli-4.2.98/programs/dir_cart.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dir_redo.py` & `pmagpy-cli-4.2.98/programs/dir_redo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dmag_magic.py` & `pmagpy-cli-4.2.98/programs/dmag_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/dmag_magic2.py` & `pmagpy-cli-4.2.98/programs/dmag_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/download_magic.py` & `pmagpy-cli-4.2.98/programs/download_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eigs_s.py` & `pmagpy-cli-4.2.98/programs/eigs_s.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eq_di.py` & `pmagpy-cli-4.2.98/programs/eq_di.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eqarea.py` & `pmagpy-cli-4.2.98/programs/eqarea.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eqarea_ell.py` & `pmagpy-cli-4.2.98/programs/eqarea_ell.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eqarea_magic.py` & `pmagpy-cli-4.2.98/programs/eqarea_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/eqarea_magic2.py` & `pmagpy-cli-4.2.98/programs/eqarea_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/find_ei.py` & `pmagpy-cli-4.2.98/programs/find_ei.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/fisher.py` & `pmagpy-cli-4.2.98/programs/fisher.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/fishqq.py` & `pmagpy-cli-4.2.98/programs/fishqq.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/fishrot.py` & `pmagpy-cli-4.2.98/programs/fishrot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/foldtest.py` & `pmagpy-cli-4.2.98/programs/foldtest.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/foldtest_magic.py` & `pmagpy-cli-4.2.98/programs/foldtest_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/foldtest_magic2.py` & `pmagpy-cli-4.2.98/programs/foldtest_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/forc_diagram.py` & `pmagpy-cli-4.2.98/programs/forc_diagram.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/gaussian.py` & `pmagpy-cli-4.2.98/programs/gaussian.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/gobing.py` & `pmagpy-cli-4.2.98/programs/gobing.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/gofish.py` & `pmagpy-cli-4.2.98/programs/gofish.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/gokent.py` & `pmagpy-cli-4.2.98/programs/gokent.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/goprinc.py` & `pmagpy-cli-4.2.98/programs/goprinc.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/grab_magic_key.py` & `pmagpy-cli-4.2.98/programs/grab_magic_key.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/histplot.py` & `pmagpy-cli-4.2.98/programs/histplot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/hysteresis_magic.py` & `pmagpy-cli-4.2.98/programs/hysteresis_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/hysteresis_magic2.py` & `pmagpy-cli-4.2.98/programs/hysteresis_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/igrf.py` & `pmagpy-cli-4.2.98/programs/igrf.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/images/PmagPy.ico` & `pmagpy-cli-4.2.98/programs/images/PmagPy.ico`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/images/PmagPy_16x16.ico` & `pmagpy-cli-4.2.98/programs/images/PmagPy_16x16.ico`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/images/PmagPy_32x32.ico` & `pmagpy-cli-4.2.98/programs/images/PmagPy_32x32.ico`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/incfish.py` & `pmagpy-cli-4.2.98/programs/incfish.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/install_etopo.py` & `pmagpy-cli-4.2.98/programs/install_etopo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/irm_unmix.py` & `pmagpy-cli-4.2.98/programs/irm_unmix.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/irmaq_magic.py` & `pmagpy-cli-4.2.98/programs/irmaq_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/k15_s.py` & `pmagpy-cli-4.2.98/programs/k15_s.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/lnp_magic.py` & `pmagpy-cli-4.2.98/programs/lnp_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/lowes.py` & `pmagpy-cli-4.2.98/programs/lowes.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/lowrie.py` & `pmagpy-cli-4.2.98/programs/lowrie.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/lowrie_magic.py` & `pmagpy-cli-4.2.98/programs/lowrie_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/lsq_redo.py` & `pmagpy-cli-4.2.98/programs/lsq_redo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/magic_gui.py` & `pmagpy-cli-4.2.98/programs/magic_gui.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/magic_select.py` & `pmagpy-cli-4.2.98/programs/magic_select.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/make_magic_plots.py` & `pmagpy-cli-4.2.98/programs/make_magic_plots.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,27 +76,29 @@
     if '-f' in sys.argv:
         ind = sys.argv.index("-f")
         filelist = [sys.argv[ind + 1]]
     else:
         filelist = os.listdir(dir_path)
     ## initialize some variables
     samp_file = 'samples.txt'
+    spec_file = 'specimens.txt'
     meas_file = 'measurements.txt'
     #loc_key = 'location'
     loc_file = 'locations.txt'
     method_key = 'method_codes'
     dec_key = 'dir_dec'
     inc_key = 'dir_inc'
     tilt_corr_key = "dir_tilt_correction"
     aniso_tilt_corr_key = "aniso_tilt_correction"
     hyst_bcr_key = "hyst_bcr"
     hyst_mr_key = "hyst_mr_moment"
     hyst_ms_key = "hyst_ms_moment"
     hyst_bc_key = "hyst_bc"
     Mkeys = ['magnitude', 'magn_moment', 'magn_volume', 'magn_mass']
+    Hkeys = ['height', 'core_depth', 'composite_depth']
     results_file = 'sites.txt'
     hyst_file = 'specimens.txt'
     aniso_file = 'specimens.txt'
     # create contribution and propagate data throughout
     full_con = cb.Contribution()
     full_con.propagate_location_to_measurements()
     full_con.propagate_location_to_specimens()
@@ -193,15 +195,14 @@
             return [], []
 
         meas_data, meas_df = get_data('measurements', loc)
         spec_data, spec_df = get_data('specimens', loc)
         samp_data, samp_df = get_data('samples', loc)
         site_data, site_df = get_data('sites', loc)
         loc_data, loc_df = get_data('locations', loc)
-
         con = cb.Contribution(read_tables=[])
         con.tables['measurements'] = cb.MagicDataFrame(df=meas_df, dtype="measurements")
         con.tables['specimens'] = cb.MagicDataFrame(df=spec_df, dtype="specimens")
         con.tables['samples'] = cb.MagicDataFrame(df=samp_df, dtype="samples")
         con.tables['sites'] = cb.MagicDataFrame(df=site_df, dtype="sites")
         con.tables['locations'] = cb.MagicDataFrame(df=loc_df, dtype="locations")
 
@@ -381,16 +382,17 @@
                                                                 fmt="png", contribution=con,
                                                                 image_records=True)
                 image_recs.extend(vgpmap_recs)
             else:
                 print('-I- No vgps found')
 
             print('-I- Look for intensities')
-            # is there any intensity data?
+                         
             if site_data:
+            # are there any intensity data?
                 if int_key in site_data[0].keys():
                     # old way, wasn't working right:
                     #CMD = 'magic_select.py  -key ' + int_key + ' 0. has -F tmp1.txt -f tmp_sites.txt'
                     Selection = pmag.get_dictkey(site_data, int_key, dtype="f")
                     selection = [i * 1e6 for i in Selection if i != 0]
                     loc = loc.replace(" ", "_")
                     if loc == "./":
@@ -474,14 +476,39 @@
                     CMD = "ipmag.aniso_magic(iboot=0, ihext=1, crd='g', fmt='png', contribution={})".format(con)
                     print(CMD)
                     info_log(CMD, loc)
                     res, files, aniso_recs = ipmag.aniso_magic(iboot=0, ihext=1, crd="t", fmt="png",
                                                                contribution=con, image_records=True)
                     image_recs.extend(aniso_recs)
 
+        # are there any depth/height data?
+        h_key=False
+        if len(site_df)>0:
+                for key in Hkeys:
+                    if key in site_df.columns:
+                        h_key=key
+                if h_key: h_df=site_df[['site',h_key]]
+                #if h_key and len(meas_df)>0: 
+                #    meas_df=meas_df.merge(h_df,on='site',how='inner')
+                #    pmag.magic_write('tmp_measurements.txt',meas_df,'measurements',dataframe=True)
+                #    print ('adding ',h_key,' to measurements table')
+                locations=site_df['location'].unique()
+                if h_key and len(spec_df)>0: 
+                    spec_df=spec_df.merge(h_df,on='site',how='inner')
+                    #pmag.magic_write('tmp_specimens.txt',spec_df,'specimens',dataframe=True)
+                    print ('adding ',h_key,' to specimens table')
+                    for location in locations:
+                        loc_df=spec_df[spec_df['location']==location]
+                        ipmag.df_depthplot(spec_df,h_key,save=True,location=location)
+                if h_key and len(samp_df)>0: 
+                    samp_df=samp_df.merge(h_df,on='site',how='inner')
+                    #pmag.magic_write('tmp_samples.txt',samp_df,'samples',dataframe=True)
+                    print ('adding ',h_key,' to samples table')
+       
+ 
         # remove temporary files
         for fname in glob.glob('tmp*.txt'):
             os.remove(fname)
 
     # now we need full contribution data
     if loc_file in filelist and loc_data:
         #data, file_type = pmag.magic_read(loc_file)  # read in location data
```

### Comparing `pmagpy-cli-4.2.97/programs/microwave_magic.py` & `pmagpy-cli-4.2.98/programs/microwave_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/mk_redo.py` & `pmagpy-cli-4.2.98/programs/mk_redo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/move_data_files.py` & `pmagpy-cli-4.2.98/programs/move_data_files.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/mst_magic.py` & `pmagpy-cli-4.2.98/programs/mst_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/orientation_magic.py` & `pmagpy-cli-4.2.98/programs/orientation_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/pca.py` & `pmagpy-cli-4.2.98/programs/pca.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_2cdfs.py` & `pmagpy-cli-4.2.98/programs/plot_2cdfs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_cdf.py` & `pmagpy-cli-4.2.98/programs/plot_cdf.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_geomagia.py` & `pmagpy-cli-4.2.98/programs/plot_geomagia.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_magmap.py` & `pmagpy-cli-4.2.98/programs/plot_magmap.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_magmap_basemap.py` & `pmagpy-cli-4.2.98/programs/plot_magmap_basemap.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plot_map_pts.py` & `pmagpy-cli-4.2.98/programs/plot_map_pts.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plotdi_a.py` & `pmagpy-cli-4.2.98/programs/plotdi_a.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plotdi_e.py` & `pmagpy-cli-4.2.98/programs/plotdi_e.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/plotxy.py` & `pmagpy-cli-4.2.98/programs/plotxy.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/pmag_gui.py` & `pmagpy-cli-4.2.98/programs/pmag_gui.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/pmag_results_extract.py` & `pmagpy-cli-4.2.98/programs/pmag_results_extract.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/pmm_redo.py` & `pmagpy-cli-4.2.98/programs/pmm_redo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/polemap_magic.py` & `pmagpy-cli-4.2.98/programs/polemap_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/pt_rot.py` & `pmagpy-cli-4.2.98/programs/pt_rot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/qqplot.py` & `pmagpy-cli-4.2.98/programs/qqplot.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/qqunf.py` & `pmagpy-cli-4.2.98/programs/qqunf.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/quick_hyst.py` & `pmagpy-cli-4.2.98/programs/quick_hyst.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/quick_hyst2.py` & `pmagpy-cli-4.2.98/programs/quick_hyst2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/remanence_anisotropy_magic.py` & `pmagpy-cli-4.2.98/programs/remanence_anisotropy_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/replace_ac_specimens.py` & `pmagpy-cli-4.2.98/programs/replace_ac_specimens.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/revtest.py` & `pmagpy-cli-4.2.98/programs/revtest.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/revtest_magic.py` & `pmagpy-cli-4.2.98/programs/revtest_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/revtest_mm1990.py` & `pmagpy-cli-4.2.98/programs/revtest_mm1990.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/s_eigs.py` & `pmagpy-cli-4.2.98/programs/s_eigs.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/s_geo.py` & `pmagpy-cli-4.2.98/programs/s_geo.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/s_hext.py` & `pmagpy-cli-4.2.98/programs/s_hext.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/s_tilt.py` & `pmagpy-cli-4.2.98/programs/s_tilt.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/scalc.py` & `pmagpy-cli-4.2.98/programs/scalc.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/scalc_magic.py` & `pmagpy-cli-4.2.98/programs/scalc_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/site_edit_magic.py` & `pmagpy-cli-4.2.98/programs/site_edit_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/sort_specimens.py` & `pmagpy-cli-4.2.98/programs/sort_specimens.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/squish.py` & `pmagpy-cli-4.2.98/programs/squish.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/stats.py` & `pmagpy-cli-4.2.98/programs/stats.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/strip_magic.py` & `pmagpy-cli-4.2.98/programs/strip_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/sundec.py` & `pmagpy-cli-4.2.98/programs/sundec.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/thellier_gui.py` & `pmagpy-cli-4.2.98/programs/thellier_gui.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/thellier_magic.py` & `pmagpy-cli-4.2.98/programs/thellier_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/thellier_magic2.py` & `pmagpy-cli-4.2.98/programs/thellier_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/thumbnails.py` & `pmagpy-cli-4.2.98/programs/thumbnails.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/tk03.py` & `pmagpy-cli-4.2.98/programs/tk03.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/trmaq_magic.py` & `pmagpy-cli-4.2.98/programs/trmaq_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/uniform.py` & `pmagpy-cli-4.2.98/programs/uniform.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/unsquish.py` & `pmagpy-cli-4.2.98/programs/unsquish.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/upload_magic.py` & `pmagpy-cli-4.2.98/programs/upload_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/vdm_b.py` & `pmagpy-cli-4.2.98/programs/vdm_b.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/vector_mean.py` & `pmagpy-cli-4.2.98/programs/vector_mean.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/vgp_di.py` & `pmagpy-cli-4.2.98/programs/vgp_di.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/vgpmap_magic.py` & `pmagpy-cli-4.2.98/programs/vgpmap_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/vgpmap_magic2.py` & `pmagpy-cli-4.2.98/programs/vgpmap_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/watsons_f.py` & `pmagpy-cli-4.2.98/programs/watsons_f.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/watsons_v.py` & `pmagpy-cli-4.2.98/programs/watsons_v.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/zeq.py` & `pmagpy-cli-4.2.98/programs/zeq.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/zeq_magic.py` & `pmagpy-cli-4.2.98/programs/zeq_magic.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/programs/zeq_magic2.py` & `pmagpy-cli-4.2.98/programs/zeq_magic2.py`

 * *Files identical despite different names*

### Comparing `pmagpy-cli-4.2.97/setup.py` & `pmagpy-cli-4.2.98/setup.py`

 * *Files identical despite different names*

