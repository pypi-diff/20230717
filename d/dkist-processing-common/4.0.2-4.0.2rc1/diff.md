# Comparing `tmp/dkist-processing-common-4.0.2.tar.gz` & `tmp/dkist-processing-common-4.0.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-4.0.2.tar", last modified: Mon Jul 17 20:54:35 2023, max compression
+gzip compressed data, was "dkist-processing-common-4.0.2rc1.tar", last modified: Mon Jul 17 18:06:12 2023, max compression
```

## Comparing `dkist-processing-common-4.0.2.tar` & `dkist-processing-common-4.0.2rc1.tar`

### file list

```diff
@@ -1,128 +1,130 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    15229 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.424811 dkist-processing-common-4.0.2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/changelog/.gitempty
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.424811 dkist-processing-common-4.0.2/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.428811 dkist-processing-common-4.0.2/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.428811 dkist-processing-common-4.0.2/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/iobase.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.428811 dkist-processing-common-4.0.2/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.428811 dkist-processing-common-4.0.2/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.428811 dkist-processing-common-4.0.2/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.432811 dkist-processing-common-4.0.2/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.432811 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.432811 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10564 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_trial_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.424811 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4324 2023-07-17 20:54:35.000000 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4718 2023-07-17 20:54:35.000000 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 20:54:35.000000 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      609 2023-07-17 20:54:35.000000 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-17 20:54:35.000000 dkist-processing-common-4.0.2/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1698 2023-07-17 20:54:35.436811 dkist-processing-common-4.0.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-17 20:54:30.000000 dkist-processing-common-4.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    14872 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/142.bugfix.rst
+-rw-rw-rw-   0 root         (0) root         (0)       41 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/changelog/143.misc.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7037 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     8046 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.751940 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)    11473 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13491 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.755940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47891 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     2364 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     6770 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18462 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     3843 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10564 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    11883 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.747940 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      612 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-07-17 18:06:12.000000 dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2023-07-17 18:06:12.759940 dkist-processing-common-4.0.2rc1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-07-17 18:06:07.000000 dkist-processing-common-4.0.2rc1/setup.py
```

### Comparing `dkist-processing-common-4.0.2/.gitignore` & `dkist-processing-common-4.0.2rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/.pre-commit-config.yaml` & `dkist-processing-common-4.0.2rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/CHANGELOG.rst` & `dkist-processing-common-4.0.2rc1/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-v4.0.2 (2023-07-17)
-===================
-
-Bugfixes
---------
-
-- Updates to support new major revisions of `pillow` and `pydantic`. (`#142 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/142>`__)
-
-
-Misc
-----
-
-- Update to latest dkist-header-validator. (`#143 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/143>`__)
-
-
 v4.0.1 (2023-07-11)
 ===================
 
 Misc
 ----
 
 - Update core dependency for airflow upgrade. (`#143 <https://bitbucket.org/dkistdc/dkist-processing-common/pull-requests/143>`__)
```

### Comparing `dkist-processing-common-4.0.2/PKG-INFO` & `dkist-processing-common-4.0.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.0.2
+Version: 4.0.2rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.0.2/README.rst` & `dkist-processing-common-4.0.2rc1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/bitbucket-pipelines.yml` & `dkist-processing-common-4.0.2rc1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/check_changelog_updated.sh` & `dkist-processing-common-4.0.2rc1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/config.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/constants.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/_util/tags.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/codecs/iobase.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/iobase.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/codecs/json.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/codecs/str.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/manual.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/constants.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/graphql.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/message.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/parameters.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/quality.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/tags.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/time.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/globus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/output_data_base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/trial_output_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_codecs.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_output_data_base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_output_data_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_trial_output_data.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_trial_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-4.0.2rc1/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 4.0.2
+Version: 4.0.2rc1
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/142.bugfix.rst
+changelog/143.misc.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
 dkist_processing_common.egg-info/top_level.txt
```

### Comparing `dkist-processing-common-4.0.2/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-4.0.2rc1/dkist_processing_common.egg-info/requires.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-astropy>=5.1.1
-dkist-fits-specifications>=3.0.0
-dkist-header-validator>=4.0.0
 dkist-processing-core==2.0.2
 dkist-processing-pac>=2.1.1
-dkist-spectral-lines>=2.0.0
-globus-sdk>=3.12.0
-gqlclient==0.9.6
-hashids==1.3.1
-matplotlib>=3.4
-moviepy>=1.0.3
+dkist-header-validator>=4.0.0rc2
+dkist-fits-specifications>=3.0.0
+astropy>=5.1.1
 numpy>=1.20.2
-object-clerk==0.1.0
 pandas>=1.4.2
-pillow>=8.3.0
-pydantic>=1.8.1
+hashids==1.3.1
+globus-sdk>=3.12.0
+gqlclient==0.9.6
+talus==0.2.1
 redis==4.6.0
+object-clerk==0.1.0
 requests>=2.23
-retry>=0.9.2
 scipy>=1.6.3
 sunpy>=3.0.0
-talus==0.2.1
+pillow>=8.3.0
+moviepy>=1.0.3
+matplotlib>=3.4
+pydantic>=1.8.1
+retry>=0.9.2
+dkist-spectral-lines>=2.0.0
 
 [docs]
 sphinx
 sphinx-astropy
 sphinx-changelog
 sphinx-autoapi
 pytest
```

### Comparing `dkist-processing-common-4.0.2/docs/Makefile` & `dkist-processing-common-4.0.2rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/docs/conf.py` & `dkist-processing-common-4.0.2rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/docs/make.bat` & `dkist-processing-common-4.0.2rc1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/licenses/LICENSE.rst` & `dkist-processing-common-4.0.2rc1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/pyproject.toml` & `dkist-processing-common-4.0.2rc1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-4.0.2/setup.cfg` & `dkist-processing-common-4.0.2rc1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -15,36 +15,36 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	astropy >= 5.1.1
-	dkist-fits-specifications >= 3.0.0
-	dkist-header-validator >= 4.0.0
 	dkist-processing-core == 2.0.2
 	dkist-processing-pac >= 2.1.1
-	dkist-spectral-lines >= 2.0.0
-	globus-sdk >= 3.12.0
-	gqlclient == 0.9.6
-	hashids == 1.3.1
-	matplotlib >= 3.4
-	moviepy >= 1.0.3
+	dkist-header-validator >= 4.0.0rc2
+	dkist-fits-specifications >= 3.0.0
+	astropy >= 5.1.1
 	numpy >= 1.20.2
-	object-clerk == 0.1.0
 	pandas >= 1.4.2
-	pillow >= 8.3.0
-	pydantic >= 1.8.1
+	hashids == 1.3.1
+	globus-sdk >= 3.12.0
+	gqlclient == 0.9.6
+	talus == 0.2.1
 	redis == 4.6.0
+	object-clerk == 0.1.0
 	requests >= 2.23
-	retry >= 0.9.2
 	scipy >= 1.6.3
 	sunpy >= 3.0.0
-	talus == 0.2.1
+	pillow >= 8.3.0
+	moviepy >= 1.0.3
+	matplotlib >= 3.4
+	pydantic >= 1.8.1
+	retry >= 0.9.2
+	dkist-spectral-lines >= 2.0.0
 
 [options.extras_require]
 test = 
 	pytest
 	pytest-xdist
 	pytest-cov
 	pytest-mock
```

