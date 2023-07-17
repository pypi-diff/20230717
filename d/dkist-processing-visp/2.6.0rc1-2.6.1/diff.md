# Comparing `tmp/dkist_processing_visp-2.6.0rc1.tar.gz` & `tmp/dkist_processing_visp-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_visp-2.6.0rc1.tar", last modified: Fri Jul 14 00:14:39 2023, max compression
+gzip compressed data, was "dkist_processing_visp-2.6.1.tar", last modified: Mon Jul 17 21:53:49 2023, max compression
```

## Comparing `dkist_processing_visp-2.6.0rc1.tar` & `dkist_processing_visp-2.6.1.tar`

### file list

```diff
@@ -1,116 +1,115 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    21632 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     3428 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       85 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/changelog/121.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/
--rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3440 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     3005 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/modulator_states.py
--rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py
--rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/raster_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/task.py
--rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.051792 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    14744 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     4137 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)    41082 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    20368 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5343 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.051792 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5642 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/corrections.py
--rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/downsample.py
--rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10506 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)    28173 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)    28801 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1586 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16409 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
--rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    18443 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_background_light.py
--rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_build_quality_report.py
--rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_downsample.py
--rw-rw-rw-   0 root         (0) root         (0)    14009 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_geometric.py
--rw-rw-rw-   0 root         (0) root         (0)    12613 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py
--rw-rw-rw-   0 root         (0) root         (0)     5651 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_lamp.py
--rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_map_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    20093 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parse.py
--rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     9883 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_solar.py
--rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_submit_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)     5091 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_base.py
--rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/single_task_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     3314 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/trial_workflows.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.047791 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6216 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3949 2023-07-14 00:14:39.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-14 00:14:38.000000 dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/background_light.rst
--rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/gain_correction.rst
--rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/l0_to_l1_visp.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/polarization_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/science_calibration.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-14 00:14:39.055791 dkist_processing_visp-2.6.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-14 00:14:33.000000 dkist_processing_visp-2.6.0rc1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2461 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      841 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    22284 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5645 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3652 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3428 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.729856 dkist_processing_visp-2.6.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.729856 dkist_processing_visp-2.6.1/dkist_processing_visp/
+-rw-rw-rw-   0 root         (0) root         (0)      249 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.729856 dkist_processing_visp-2.6.1/dkist_processing_visp/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/fonts/Lato-Regular.ttf
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.733856 dkist_processing_visp-2.6.1/dkist_processing_visp/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3440 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    11306 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1271 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.733856 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5370 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     3005 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/modulator_states.py
+-rw-rw-rw-   0 root         (0) root         (0)      876 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/polarimeter_mode.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/raster_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/task.py
+-rw-rw-rw-   0 root         (0) root         (0)     1869 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1335 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/visp_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      859 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/visp_l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      843 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.737856 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    14744 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     4137 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)    41082 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    20368 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5343 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     7068 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.737856 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5642 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/corrections.py
+-rw-rw-rw-   0 root         (0) root         (0)     1343 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)     7112 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10506 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     4329 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     7944 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)    28173 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)    28801 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1611 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6846 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.737856 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16409 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    18994 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     8247 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2514 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    18443 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_background_light.py
+-rw-rw-rw-   0 root         (0) root         (0)     1171 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_build_quality_report.py
+-rw-rw-rw-   0 root         (0) root         (0)     5272 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     2173 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_downsample.py
+-rw-rw-rw-   0 root         (0) root         (0)    14009 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_geometric.py
+-rw-rw-rw-   0 root         (0) root         (0)    12613 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_instrument_polarization.py
+-rw-rw-rw-   0 root         (0) root         (0)     5651 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_lamp.py
+-rw-rw-rw-   0 root         (0) root         (0)     4021 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    11818 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_map_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    20093 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     4383 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    19734 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     9883 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_solar.py
+-rw-rw-rw-   0 root         (0) root         (0)     1121 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_submit_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     5340 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5091 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_visp_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1731 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_visp_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     5752 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3280 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/single_task_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     3314 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/trial_workflows.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.729856 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-07-17 21:53:49.000000 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3923 2023-07-17 21:53:49.000000 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 21:53:49.000000 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      621 2023-07-17 21:53:49.000000 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-07-17 21:53:49.000000 dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)     4844 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/background_light.rst
+-rw-rw-rw-   0 root         (0) root         (0)      346 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2028 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     6427 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/gain_correction.rst
+-rw-rw-rw-   0 root         (0) root         (0)      273 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      623 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/l0_to_l1_visp.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)     4995 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/polarization_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      292 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/science_calibration.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      776 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1687 2023-07-17 21:53:49.741856 dkist_processing_visp-2.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      422 2023-07-17 21:53:43.000000 dkist_processing_visp-2.6.1/towncrier_science.toml
```

### Comparing `dkist_processing_visp-2.6.0rc1/.gitignore` & `dkist_processing_visp-2.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/.pre-commit-config.yaml` & `dkist_processing_visp-2.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/CHANGELOG.rst` & `dkist_processing_visp-2.6.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+v2.6.1 (2023-07-17)
+===================
+
+Misc
+----
+
+- Update dkist-processing-common and the dkist-header-validator to propagate dependency breakages in PyYAML < 6.0. (`#122 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/122>`__)
+
+
+v2.6.0 (2023-07-14)
+===================
+
+Features
+--------
+
+- Enable intensity mode observations to be calibrated with polarized calibration data. (`#121 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/121>`__)
+
+
+Bugfixes
+--------
+
+- Include Lamp Gain intermediate files in default trial output. (`#120 <https://bitbucket.org/dkistdc/dkist-processing-visp/pull-requests/120>`__)
+
+
 v2.5.1 (2023-07-11)
 ===================
 
 Misc
 ----
 
 - Update dkist-processing-common to upgrade Airflow to 2.6.3.
```

### Comparing `dkist_processing_visp-2.6.0rc1/PKG-INFO` & `dkist_processing_visp-2.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_visp
-Version: 2.6.0rc1
+Version: 2.6.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.6.0rc1/README.rst` & `dkist_processing_visp-2.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/SCIENCE_CHANGELOG.rst` & `dkist_processing_visp-2.6.1/SCIENCE_CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/bitbucket-pipelines.yml` & `dkist_processing_visp-2.6.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/check_changelog_updated.sh` & `dkist_processing_visp-2.6.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/fonts/Lato-Regular.ttf` & `dkist_processing_visp-2.6.1/dkist_processing_visp/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/constants.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/parameters.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/models/tags.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/map_repeats.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/modulator_states.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/modulator_states.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/polarimeter_mode.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/polarimeter_mode.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/raster_step.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/raster_step.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/task.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/task.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/time.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l0_fits_access.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/visp_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/visp_l1_fits_access.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/visp_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/parsers/wavelength.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/parsers/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/assemble_movie.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/background_light.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/dark.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/geometric.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/instrument_polarization.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/lamp.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/make_movie_frames.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/corrections.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/corrections.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/downsample.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/input_frame_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/mixin/intermediate_frame_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/parse.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/quality_metrics.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/science.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/solar.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/trial_output_data.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/trial_output_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
     @property
     def intermediate_task_names(self) -> list[str]:
         """Grab all the Calibration products used to calibrate science data."""
         return [
             "DARK",
             "BACKGROUND",
+            "LAMP_GAIN",
             "GEOMETRIC_ANGLE",
             "GEOMETRIC_OFFSET",
             "GEOMETRIC_SPEC_SHIFTS",
             "SOLAR_GAIN",
             "DEMOD_MATRICES",
         ]
```

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/visp_base.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tasks/write_l1.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/conftest.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/l0_to_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/local_trial_workflows/local_trial_helpers.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_assemble_movie.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_background_light.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_background_light.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_build_quality_report.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_build_quality_report.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_dark.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_downsample.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_geometric.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_geometric.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_instrument_polarization.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_instrument_polarization.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_lamp.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_lamp.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_make_movie_frames.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_map_repeats.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_map_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parameters.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_parse.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_quality.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_science.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_solar.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_solar.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_submit_quality.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_submit_quality.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_trial_output_data.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_base.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_visp_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_visp_constants.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_visp_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/tests/test_write_l1.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/l0_processing.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp/workflows/trial_workflows.py` & `dkist_processing_visp-2.6.1/dkist_processing_visp/workflows/trial_workflows.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/PKG-INFO` & `dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-visp
-Version: 2.6.0rc1
+Version: 2.6.1
 Summary: Science processing code for the ViSP instrument on DKIST
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-visp/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/visp
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/SOURCES.txt` & `dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
-changelog/121.feature.rst
 dkist_processing_visp/__init__.py
 dkist_processing_visp.egg-info/PKG-INFO
 dkist_processing_visp.egg-info/SOURCES.txt
 dkist_processing_visp.egg-info/dependency_links.txt
 dkist_processing_visp.egg-info/requires.txt
 dkist_processing_visp.egg-info/top_level.txt
 dkist_processing_visp/fonts/Lato-Regular.ttf
```

### Comparing `dkist_processing_visp-2.6.0rc1/dkist_processing_visp.egg-info/requires.txt` & `dkist_processing_visp-2.6.1/dkist_processing_visp.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-dkist-processing-common==4.0.1
+dkist-processing-common==4.0.2
 dkist-processing-math==2.0.0
 dkist-processing-pac==3.0.0
-dkist-header-validator==3.0.5
+dkist-header-validator==4.0.0
 dkist-fits-specifications==3.6.0
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
 scipy==1.11.0
 scikit-image==0.21.0
 scikit-learn==1.2.2
```

### Comparing `dkist_processing_visp-2.6.0rc1/docs/Makefile` & `dkist_processing_visp-2.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/background_light.rst` & `dkist_processing_visp-2.6.1/docs/background_light.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/conf.py` & `dkist_processing_visp-2.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/gain_correction.rst` & `dkist_processing_visp-2.6.1/docs/gain_correction.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/l0_to_l1_visp.rst` & `dkist_processing_visp-2.6.1/docs/l0_to_l1_visp.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/make.bat` & `dkist_processing_visp-2.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/polarization_calibration.rst` & `dkist_processing_visp-2.6.1/docs/polarization_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/docs/science_calibration.rst` & `dkist_processing_visp-2.6.1/docs/science_calibration.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/licenses/LICENSE.rst` & `dkist_processing_visp-2.6.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/pyproject.toml` & `dkist_processing_visp-2.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_visp-2.6.0rc1/setup.cfg` & `dkist_processing_visp-2.6.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 4.0.1
+	dkist-processing-common == 4.0.2
 	dkist-processing-math == 2.0.0
 	dkist-processing-pac == 3.0.0
-	dkist-header-validator == 3.0.5
+	dkist-header-validator == 4.0.0
 	dkist-fits-specifications == 3.6.0
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
 	scipy == 1.11.0
 	scikit-image == 0.21.0
 	scikit-learn == 1.2.2
```

