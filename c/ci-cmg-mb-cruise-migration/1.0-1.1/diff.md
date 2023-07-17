# Comparing `tmp/ci_cmg_mb_cruise_migration-1.0.tar.gz` & `tmp/ci_cmg_mb_cruise_migration-1.1.tar.gz`

## Comparing `ci_cmg_mb_cruise_migration-1.0.tar` & `ci_cmg_mb_cruise_migration-1.1.tar`

### file list

```diff
@@ -1,169 +1,173 @@
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/config.yaml
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/requirements.txt
--rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/run.sh
--rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/start_background.sh
--rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/stop_background.sh
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/.gitignore
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/pyvenv.cfg
--rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.csh
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.fish
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.nu
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.ps1
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate_this.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/deactivate.nu
--rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/docutils
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/futurize
--rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/keyring
--rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/markdown-it
--rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/normalizer
--rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pasteurize
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pip
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pip3
--rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pip3.10
--rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pkginfo
--rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pygmentize
--rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/pyproject-build
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/python -> /opt/homebrew/bin/python3
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/python3.10 -> python
--rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html.py
--rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html4.py
--rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html5.py
--rwxr-xr-x   0        0        0      836 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2latex.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2man.py
--rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2odt.py
--rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2pseudoxml.py
--rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2s5.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2xetex.py
--rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2xml.py
--rwxr-xr-x   0        0        0      713 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/rstpep2html.py
--rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/twine
--rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/virtualenv
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/wheel
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/wheel-3.10
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/wheel3
--rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/migenv/bin/wheel3.10
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/clean_cruise.py
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/cleaner.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/migration_properties.py
--rw-r--r--   0        0        0     3991 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/migrator.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/start_migration.py
--rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/cruise_connection.py
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/cruise_db.py
--rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/mb_db.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/oracledb_pooled.py
--rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/query_builder.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/cache.py
--rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_decoder.py
--rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_filter.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_labeler.py
--rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_validator.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/paginator.py
--rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/parsed_data_file.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/survey_filter.py
--rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/const_initializer.py
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/data_file_consts.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/data_file_part_consts.py
--rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/dataset_type_consts.py
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/error_consts.py
--rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/file_format_consts.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/file_label_consts.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/file_type_consts.py
--rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/instrument_consts.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/log_level_consts.py
--rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/platform_type_consts.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/survey_blacklist.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/version_consts.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/version_description_consts.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py
--rw-r--r--   0        0        0    23188 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py
--rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/batch_error.py
--rw-r--r--   0        0        0    10344 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_log.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_logger.py
--rw-r--r--   0        0        0     6816 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_report.py
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_access_path.py
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_dataset.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_dataset_types.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_file_formats.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_file_types.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_files.py
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_instruments.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_parameter.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_parameter_details.py
--rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_platforms.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_projects.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_shape.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_surveys.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_version_descriptions.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/cruise_cargo.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/mb_cargo.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/migrating_survey.py
--rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/prefab.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/transfer.py
--rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_mbinfo_formats.py
--rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py
--rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_survey.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_survey_reference.py
--rw-r--r--   0        0        0    20861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/cruise_processor.py
--rw-r--r--   0        0        0     5615 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/mb_processor.py
--rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/prefab_factory.py
--rw-r--r--   0        0        0    37683 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/schema_mapper.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/transfer_station.py
--rw-r--r--   0        0        0    46440 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/services/cruise_service.py
--rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/services/mb_service.py
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/utility/common.py
--rw-r--r--   0        0        0     4184 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/utility/dataset.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/config_test.yaml
--rwxr-xr-x   0        0        0     1355 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/start-it.sh
--rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/stop-it.sh
--rw-r--r--   0        0        0     3153 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_batch_insert.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cleaner.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_configurable_survey_query.py
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_const_initializer.py
--rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_designator_resolver.py
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_instrument_resolver.py
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_processor.py
--rw-r--r--   0        0        0    17566 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_service_crud.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_service_mappings.py
--rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_end_to_end_it.py
--rw-r--r--   0        0        0    16704 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_mb_filters.py
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_mb_paginator.py
--rw-r--r--   0        0        0     2175 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_mb_processor.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_mb_service.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_mb_survey_blacklist.py
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_scratch.py
--rw-r--r--   0        0        0    36232 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_standard_mapping.py
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/test_survey_metadata_mapping.py
--rw-r--r--   0        0        0     9673 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/testutils.py
--rw-r--r--   0        0        0    53753 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/create_mb.sql
--rw-r--r--   0        0        0   213608 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/migrate_cruise.sql
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/setup-user.sql
--rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/setup_cruise.sh
--rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/setup_mb.sh
--rw-r--r--   0        0        0   683665 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1208.sql
--rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1208_lite.sql
--rw-r--r--   0        0        0   856973 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1570.sql
--rw-r--r--   0        0        0   584287 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW2176.sql
--rw-r--r--   0        0        0  2082204 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3020.sql
--rw-r--r--   0        0        0   688103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3106.sql
--rw-r--r--   0        0        0   222391 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3206.sql
--rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3370.sql
--rw-r--r--   0        0        0   828582 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3549.sql
--rw-r--r--   0        0        0   419998 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW523.sql
--rw-r--r--   0        0        0   352532 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/RR1808.sql
--rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/RR1808_lite.sql
--rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/test_blacklist.sql
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/LICENSE
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/README.md
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/pyproject.toml
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.0/PKG-INFO
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/config.yaml
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/requirements.txt
+-rwxr-xr-x   0        0        0      112 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/run.sh
+-rwxr-xr-x   0        0        0       90 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/start_background.sh
+-rwxr-xr-x   0        0        0      368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/stop_background.sh
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/.gitignore
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/pyvenv.cfg
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.csh
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.fish
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.nu
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.ps1
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate_this.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/deactivate.nu
+-rwxr-xr-x   0        0        0      261 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/docutils
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/futurize
+-rwxr-xr-x   0        0        0      255 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/keyring
+-rwxr-xr-x   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/markdown-it
+-rwxr-xr-x   0        0        0      289 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/normalizer
+-rwxr-xr-x   0        0        0      262 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pasteurize
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip3
+-rwxr-xr-x   0        0        0      266 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pip3.10
+-rwxr-xr-x   0        0        0      263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pkginfo
+-rwxr-xr-x   0        0        0      260 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pygmentize
+-rwxr-xr-x   0        0        0      270 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/pyproject-build
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python -> /opt/homebrew/bin/python3
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python3 -> python
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/python3.10 -> python
+-rwxr-xr-x   0        0        0      637 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html.py
+-rwxr-xr-x   0        0        0      759 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html4.py
+-rwxr-xr-x   0        0        0     1104 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html5.py
+-rwxr-xr-x   0        0        0      836 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2latex.py
+-rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2man.py
+-rwxr-xr-x   0        0        0      825 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt.py
+-rwxr-xr-x   0        0        0     1763 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0        0        0      644 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0        0        0      680 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2s5.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xetex.py
+-rwxr-xr-x   0        0        0      645 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xml.py
+-rwxr-xr-x   0        0        0      713 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/rstpep2html.py
+-rwxr-xr-x   0        0        0      258 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/twine
+-rwxr-xr-x   0        0        0      283 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/virtualenv
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel-3.10
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel3
+-rwxr-xr-x   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/migenv/bin/wheel3.10
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/clean_cruise.py
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/cleaner.py
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migration_properties.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migrator.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/start_migration.py
+-rw-r--r--   0        0        0     2421 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_connection.py
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_db.py
+-rw-r--r--   0        0        0     2674 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/mb_db.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/oracledb_pooled.py
+-rw-r--r--   0        0        0     3152 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/query_builder.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/cache.py
+-rw-r--r--   0        0        0     3529 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_decoder.py
+-rw-r--r--   0        0        0     2335 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_filter.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_labeler.py
+-rw-r--r--   0        0        0     3367 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_validator.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/paginator.py
+-rw-r--r--   0        0        0     4379 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/parsed_data_file.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/survey_filter.py
+-rw-r--r--   0        0        0     3843 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/const_initializer.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_consts.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_part_consts.py
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/dataset_type_consts.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/date_consts.py
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/error_consts.py
+-rw-r--r--   0        0        0     5002 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_format_consts.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_label_consts.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_type_consts.py
+-rw-r--r--   0        0        0     2340 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/instrument_consts.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/log_level_consts.py
+-rw-r--r--   0        0        0     5425 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/platform_type_consts.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/survey_blacklist.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/version_consts.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/version_description_consts.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py
+-rw-r--r--   0        0        0    23209 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py
+-rw-r--r--   0        0        0     3490 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/batch_error.py
+-rw-r--r--   0        0        0    10646 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_log.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_logger.py
+-rw-r--r--   0        0        0     8439 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_report.py
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_access_path.py
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset_types.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_file_formats.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_file_types.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_files.py
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_instruments.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter_details.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_platforms.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_projects.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_shape.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_surveys.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_version_descriptions.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/cruise_cargo.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/mb_cargo.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/migrating_survey.py
+-rw-r--r--   0        0        0     2704 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/prefab.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/transfer.py
+-rw-r--r--   0        0        0    15525 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_formats.py
+-rw-r--r--   0        0        0     5088 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py
+-rw-r--r--   0        0        0    11263 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey_reference.py
+-rw-r--r--   0        0        0    20861 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/cruise_processor.py
+-rw-r--r--   0        0        0     5675 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/mb_processor.py
+-rw-r--r--   0        0        0     4984 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/prefab_factory.py
+-rw-r--r--   0        0        0    37050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/schema_mapper.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/transfer_station.py
+-rw-r--r--   0        0        0    47113 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/cruise_service.py
+-rw-r--r--   0        0        0     3189 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/mb_service.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/common.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/dataset.py
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/config_test.yaml
+-rwxr-xr-x   0        0        0     1355 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/start-it.sh
+-rwxr-xr-x   0        0        0      169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/stop-it.sh
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_batch_insert.py
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cleaner.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_configurable_survey_query.py
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_const_initializer.py
+-rw-r--r--   0        0        0     2754 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_designator_resolver.py
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_instrument_resolver.py
+-rw-r--r--   0        0        0     8311 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_processor.py
+-rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_crud.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_mappings.py
+-rw-r--r--   0        0        0    20064 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_end_to_end_it.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_loggers.py
+-rw-r--r--   0        0        0    16438 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_filters.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_paginator.py
+-rw-r--r--   0        0        0     2169 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_processor.py
+-rw-r--r--   0        0        0     2850 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_service.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_mb_survey_blacklist.py
+-rw-r--r--   0        0        0     4555 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_provider_from_source.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_scratch.py
+-rw-r--r--   0        0        0    36368 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_standard_mapping.py
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/test_survey_metadata_mapping.py
+-rw-r--r--   0        0        0     9891 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/testutils.py
+-rw-r--r--   0        0        0    53753 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/create_mb.sql
+-rw-r--r--   0        0        0   213608 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/migrate_cruise.sql
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup-user.sql
+-rwxr-xr-x   0        0        0      149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup_cruise.sh
+-rwxr-xr-x   0        0        0      233 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/setup_mb.sh
+-rw-r--r--   0        0        0   683665 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208.sql
+-rw-r--r--   0        0        0     7149 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208_lite.sql
+-rw-r--r--   0        0        0   856973 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1570.sql
+-rw-r--r--   0        0        0   584287 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW2176.sql
+-rw-r--r--   0        0        0  2082204 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3020.sql
+-rw-r--r--   0        0        0   688103 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3106.sql
+-rw-r--r--   0        0        0   222391 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3206.sql
+-rw-r--r--   0        0        0    48250 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3370.sql
+-rw-r--r--   0        0        0    74691 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3403.sql
+-rw-r--r--   0        0        0   828582 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3549.sql
+-rw-r--r--   0        0        0   419998 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW523.sql
+-rw-r--r--   0        0        0   352532 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808.sql
+-rw-r--r--   0        0        0    10347 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808_lite.sql
+-rw-r--r--   0        0        0    18561 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/test_blacklist.sql
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/LICENSE
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/README.md
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/pyproject.toml
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 ci_cmg_mb_cruise_migration-1.1/PKG-INFO
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/config.yaml` & `ci_cmg_mb_cruise_migration-1.1/config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   service: ""
   sid: ""
   pooled: False
 
 log:
   log_root: ""
   log_dir: "log"
+  review_dir: "review"
   report_dir: "report"
   level: "info"
   log_size_mb: 10
 
 run_parameters:
   migrate_shapes: False
   max_queue_size: 10
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.csh` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.csh`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.fish` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.fish`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.nu` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.nu`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate.ps1` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate.ps1`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/activate_this.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/activate_this.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html4.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html4.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2html5.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2latex.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2latex.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2man.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2man.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2odt.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2odt_prepstyles.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2odt_prepstyles.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2pseudoxml.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2pseudoxml.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2s5.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2s5.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2xetex.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xetex.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rst2xml.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rst2xml.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/migenv/bin/rstpep2html.py` & `ci_cmg_mb_cruise_migration-1.1/migenv/bin/rstpep2html.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/cleaner.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/cleaner.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/migration_properties.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migration_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         super().__init__(config)
 
 
 class LogConfig(object):
     def __init__(self, config):
         self.log_root = config['log_root']
         self.log_path = config['log_dir']
+        self.review_path = config['review_dir']
         self.report_path = config['report_dir']
         self.level = config['level']
         self.log_size_mb = config['log_size_mb']
 
 
 class RunParameters(object):
     def __init__(self, config):
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/migrator.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/migrator.py`

 * *Files 14% similar despite different names*

```diff
@@ -95,14 +95,17 @@
         CruiseProcessor().ship(shipment)
 
     @staticmethod
     def end_migration():
         MigrationLog.log_end()
         MigrationReport.end = datetime.now()
         MigrationReport.migration_final_report()
+        MigrationReport.migration_successful_surveys_report()
+        MigrationReport.migration_skipped_surveys_report()
+        MigrationReport.migration_problem_surveys_report()
 
     @staticmethod
     def fail_migration(context, exception: Exception):
         MigrationReport.failure_message = f"Fatal failure occurred in {context}: \n\t{str(exception)}"
-        MigrationReport.success = False
+        MigrationReport.is_success = False
         # self.end_migration(success=False)
         # sys.exit(1)
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/cruise_connection.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_connection.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/cruise_db.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/cruise_db.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/mb_db.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/mb_db.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/oracledb_pooled.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/oracledb_pooled.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/db/query_builder.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/db/query_builder.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/cache.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/cache.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_decoder.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_decoder.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_filter.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_filter.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_labeler.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_labeler.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/file_validator.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/file_validator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/paginator.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/paginator.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/parsed_data_file.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/parsed_data_file.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/survey_filter.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/survey_filter.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/const_initializer.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/const_initializer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/data_file_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/data_file_part_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/data_file_part_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/dataset_type_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/dataset_type_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/error_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/error_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/file_format_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/file_format_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/instrument_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/instrument_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/parameter_detail_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/consts/platform_type_consts.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/consts/platform_type_consts.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/dataset_type_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_format_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/file_type_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/instrument_resolver.py`

 * *Files 0% similar despite different names*

```diff
@@ -141,15 +141,15 @@
             return InstrumentConsts.SEAMARCII
         if survey_instrument == "Odom Echotrac CV2 singlebeam":
             return InstrumentConsts.ODOMECHOTRACCV2SINGLEBEAM
         if survey_instrument == "Simrad EM950":
             return InstrumentConsts.SIMRADEM950
         if survey_instrument == "SeaBeam 3012":
             return InstrumentConsts.SEABEAM3012
-        if survey_instrument == "Reson 7125" or "Reson SeaBat 7125":
+        if survey_instrument == "Reson 7125" or survey_instrument == "Reson SeaBat 7125":
             return InstrumentConsts.RESON7125
         if survey_instrument == "Kongsberg EM712":
             return InstrumentConsts.KONGSBERGEM712
         if survey_instrument == "Kongsberg EM3002":
             return InstrumentConsts.KONGSBERGEM3002
         if survey_instrument == "Reson Seabat 7160":
             return InstrumentConsts.RESONSEABAT7160
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/platform_designator_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/framework/resolvers/version_description_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_log.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from src.mb_cruise_migration.logging.migration_logger import LoggerBuilder
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.models.cruise.cruise_files import CruiseFile
 from src.mb_cruise_migration.models.intermediary.cruise_cargo import CruiseCargo, CruiseSurveyCrate
 from src.mb_cruise_migration.models.intermediary.mb_cargo import MbFileCrate
 from src.mb_cruise_migration.models.intermediary.migrating_survey import MigratingSurvey
 from src.mb_cruise_migration.models.mb.mb_ngdcid_and_file import MbFile
+from src.mb_cruise_migration.models.mb.mb_survey import MbSurvey
 
 
 class LogConsts(object):
     START = "START"
     END = "END"
     SKIP = "SKIP"
     BEGIN = "BEGIN"
@@ -33,42 +34,41 @@
         self.__initialize_review()
 
     def __initialize_log(self):
         keyword = "migration_log"
 
         level = MigrationProperties.log_config.level
         log_size_mb = MigrationProperties.log_config.log_size_mb
-        handler = self.__get_log_handler(log_size_mb, keyword)
+        handler = self.__get_log_handler(log_size_mb, keyword, MigrationProperties.log_config.log_path)
         formatter = self.__get_log_formatter()
 
         builder = LoggerBuilder(keyword, level, handler, formatter)
         MigrationLog.log = builder.get_logger()
         self.__validate_level(MigrationLog.log, level)
 
     def __initialize_review(self):
-        keyword = "migration_review"
+        keyword = "review_log"
 
         level = MigrationProperties.log_config.level
         log_size_mb = MigrationProperties.log_config.log_size_mb
-        handler = self.__get_log_handler(log_size_mb, keyword)
+        handler = self.__get_log_handler(log_size_mb, keyword, MigrationProperties.log_config.review_path)
         formatter = self.__get_log_formatter()
 
         builder = LoggerBuilder(keyword, level, handler, formatter)
         MigrationLog.review = builder.get_logger()
         self.__validate_level(MigrationLog.review, level)
 
     @staticmethod
     def __pre_check():
         if not MigrationProperties.log_config:
             raise RuntimeError("Properties must be loaded prior to creating a logger")
 
     @staticmethod
-    def __get_log_handler(log_size_mb, keyword):
+    def __get_log_handler(log_size_mb, keyword, log_dir):
         log_root = MigrationProperties.log_config.log_root
-        log_dir = MigrationProperties.log_config.log_path
         log_path = LoggerBuilder.create_log_file_path(log_root, log_dir, keyword)
         log_size = int(log_size_mb)*1024*1024  # 10MB
         return logging.handlers.RotatingFileHandler(log_path, maxBytes=log_size, backupCount=10)
 
     @staticmethod
     def __get_log_formatter():
         return logging.Formatter('%(asctime)s %(levelname)-7s %(message)s', '%Y-%m-%d %H:%M:%S')
@@ -220,7 +220,11 @@
     def log_no_file_label_error(mb_file: MbFile):
         MigrationLog.log.error(f"no valid file label identified for file {mb_file.data_file} with ngdc_id {mb_file.ngdc_id}")
 
     @staticmethod
     def log_no_file_category_error(mb_file: MbFile):
         MigrationLog.log.error(f"no valid file category identified for file {mb_file.data_file} with ngdc_id {mb_file.ngdc_id}")
 
+    @staticmethod
+    def log_paged_surveys(surveys: [MbSurvey]):
+        survey_names = [survey.survey_name for survey in surveys]
+        MigrationLog.log.info("Surveys paged: " + ", ".join(survey_names))
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_logger.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_logger.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/logging/migration_report.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/logging/migration_report.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 
-from src.mb_cruise_migration.framework.consts.log_level_consts import LogLevels
 from src.mb_cruise_migration.logging.migration_logger import LoggerBuilder
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.models.intermediary.cruise_cargo import CruiseCargo
 from src.mb_cruise_migration.models.intermediary.mb_cargo import MbSurveyCrate
 
 
 class FailedSurvey(object):
@@ -15,39 +14,80 @@
 
 class ProblemSurvey(object):
     def __init__(self, survey, message):
         self.survey_name = survey
         self.message = message
 
 
-class MigrationReport(LoggerBuilder):
+class MigrationReport(object):
     report: logging.Logger = None
+    success: logging.Logger = None
+    skipped: logging.Logger = None
+    problem: logging.Logger = None
+
     start = None
     end = None
-    success = True
+    is_success = True
     failure_message = None
 
     migrated_surveys = []
     problem_surveys: [ProblemSurvey] = []
     skipped_surveys = []
     failed_surveys: [FailedSurvey] = []
 
     total_migrated_datasets = 0
     total_migrated_files = 0
     total_instrument_review_files = 0
 
     def __init__(self):
         self.__pre_check()
+        self.__initialize_report()
+        self.__initialize_success()
+        self.__initialize_skipped()
+        self.__initialize_problem()
 
+    def __initialize_report(self):
         keyword = "migration_report"
+
+        level = MigrationProperties.log_config.level
+        handler = self.__get_report_handler(keyword)
+        formatter = self.__get_report_formatter()
+
+        builder = LoggerBuilder(keyword, level, handler, formatter)
+        MigrationReport.report = builder.get_logger()
+
+    def __initialize_success(self):
+        keyword = "completed_surveys"
+
+        level = MigrationProperties.log_config.level
+        handler = self.__get_report_handler(keyword)
+        formatter = self.__get_report_formatter()
+
+        builder = LoggerBuilder(keyword, level, handler, formatter)
+        MigrationReport.success = builder.get_logger()
+
+    def __initialize_skipped(self):
+        keyword = "skipped_surveys"
+
+        level = MigrationProperties.log_config.level
+        handler = self.__get_report_handler(keyword)
+        formatter = self.__get_report_formatter()
+
+        builder = LoggerBuilder(keyword, level, handler, formatter)
+        MigrationReport.skipped = builder.get_logger()
+
+    def __initialize_problem(self):
+        keyword = "problem_surveys"
+
+        level = MigrationProperties.log_config.level
         handler = self.__get_report_handler(keyword)
-        formatter = self.get_report_formatter()
-        super(MigrationReport, self).__init__(keyword, LogLevels.INFO, handler, formatter)
+        formatter = self.__get_report_formatter()
 
-        MigrationReport.report = self.get_logger()
+        builder = LoggerBuilder(keyword, level, handler, formatter)
+        MigrationReport.problem = builder.get_logger()
 
     @staticmethod
     def __pre_check():
         if not MigrationProperties.log_config:
             raise RuntimeError("Properties must be loaded prior to creating a logger")
 
     @staticmethod
@@ -55,15 +95,15 @@
         log_root = MigrationProperties.log_config.log_root
         log_dir = MigrationProperties.log_config.report_path
         log_path = LoggerBuilder.create_log_file_path(log_root, log_dir, keyword)
 
         return logging.FileHandler(log_path, 'w')
 
     @staticmethod
-    def get_report_formatter():
+    def __get_report_formatter():
         return logging.Formatter('%(message)s')
 
     @staticmethod
     def add_migrated_dataset(cargo: CruiseCargo):
         MigrationReport.total_migrated_datasets += 1
         num_files = len(cargo.related_file_crates)
         MigrationReport.total_migrated_files += num_files
@@ -102,55 +142,67 @@
         logger = MigrationReport.report
         total_migrated_surveys = len(MigrationReport.migrated_surveys)
         total_failed_surveys = len(MigrationReport.failed_surveys)
         total_skipped_surveys = len(MigrationReport.skipped_surveys)
         total_problem_surveys = len(MigrationReport.problem_surveys)
         total_time = (MigrationReport.end - MigrationReport.start).total_seconds() / 60
 
-        logger.info(f"MIGRATION COMPLETED {'SUCCESSFULLY' if MigrationReport.success else 'UNSUCCESSFULLY'}")
-        if not MigrationReport.success:
+        logger.info(f"MIGRATION COMPLETED {'SUCCESSFULLY' if MigrationReport.is_success else 'UNSUCCESSFULLY'}")
+        if not MigrationReport.is_success:
             logger.info(f"\n{MigrationReport.failure_message}\n")
         logger.info(f'Elapsed time in minutes: {total_time}')
         logger.info(f"\r")
 
         logger.info(f'SUMMARY')
         logger.info(f"\tmigrated surveys: {total_migrated_surveys}")
         logger.info(f"\tfailed surveys: {total_failed_surveys}")
         logger.info(f"\tskipped surveys: {total_skipped_surveys}")
         logger.info(f"\tproblem surveys: {total_problem_surveys}")
         logger.info(f"\r")
         logger.info(f"\tmigrated datasets: {MigrationReport.total_migrated_datasets}")
         logger.info(f"\tmigrated files: {MigrationReport.total_migrated_files}")
-        reviewable_percent = int(MigrationReport.total_instrument_review_files / MigrationReport.total_migrated_files)
-        logger.info(f"\tfiles requiring instrument review: {MigrationReport.total_instrument_review_files} -- {reviewable_percent}% of total files")
-        logger.info(f"\r")
+        try:
+            reviewable_percent = int((MigrationReport.total_instrument_review_files / MigrationReport.total_migrated_files) * 100)
+            logger.info(f"\tfiles requiring instrument review: {MigrationReport.total_instrument_review_files} -- {reviewable_percent}% of total files")
+        except ZeroDivisionError:
+            logger.info("No files were migrated.")
         logger.info(f"\r")
+        print("MIGRATION COMPLETED: Elapsed time: ", total_time)
+
+    @staticmethod
+    def migration_successful_surveys_report():
+        logger = MigrationReport.success
 
-        logger.info(f'BREAKDOWN')
         logger.info(f"Migrated surveys (no problems flagged):")
         migrated_surveys = MigrationReport.get_successful_surveys_without_problems()
         for survey in migrated_surveys:
             logger.info(f"\t{survey}")
-        logger.info(f"\r")
+
+    @staticmethod
+    def migration_skipped_surveys_report():
+        logger = MigrationReport.skipped
+        logger.info(f"Skipped surveys (surveys explicitly omitted via migration config):")
+        for survey in MigrationReport.skipped_surveys:
+            logger.info(f"\t{survey}")
+
+    @staticmethod
+    def migration_problem_surveys_report():
+        logger = MigrationReport.problem
+
         logger.info(f"Problem surveys (surveys flagged for review during migration):")
         for survey in MigrationReport.problem_surveys:
             # logger.info(f"\t{survey.survey_name}; {survey.message}")
             logger.info(f"\t{survey.survey_name}")
         logger.info(f"\r")
-        logger.info(f"Skipped surveys (surveys explicitly omitted via migration config):")
-        for survey in MigrationReport.skipped_surveys:
-            logger.info(f"\t{survey}")
         logger.info(f"\r")
+
         logger.info(f"Failed surveys (migration was attempted, but an error occurred):")
         for survey in MigrationReport.failed_surveys:
             # logger.info(f"\t{survey.survey_name};\r{survey.error_message}\r")
             logger.info(f"\t{survey.survey_name}")
-        logger.info(f"\r")
-
-        print("MIGRATION COMPLETED: Elapsed time: ", total_time)
 
     @staticmethod
     def clean_final_report():
         logger = MigrationReport.report
         total_time = (MigrationReport.end - MigrationReport.start).total_seconds() / 60
 
         logger.info(f"DELETION OF MULTIBEAM DATA COMPLETED")
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_access_path.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_access_path.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_dataset.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_dataset.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_files.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_files.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_parameter.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_parameter.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_people_and_sources.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/cruise/cruise_surveys.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/cruise/cruise_surveys.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/cruise_cargo.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/cruise_cargo.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/migrating_survey.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/migrating_survey.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/prefab.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/prefab.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/intermediary/transfer.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/intermediary/transfer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_mbinfo_file_tsql.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_ngdcid_and_file.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_survey.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/models/mb/mb_survey_reference.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/models/mb/mb_survey_reference.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/cruise_processor.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/cruise_processor.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/mb_processor.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/mb_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,17 +29,18 @@
         return Paginator(self.survey_pagesize, number_of_surveys)
 
     def surveys_exhausted(self):
         return self.survey_paginator.done()
 
     def load(self) -> Optional[list[MbCargo]]:
         if not self.surveys_exhausted():
-            skip, next = self.survey_paginator.paginate()
+            skip, pagesize = self.survey_paginator.paginate()
 
-            surveys = self.mb_service.get_survey_page(skip, next)
+            surveys = self.mb_service.get_survey_page(skip, pagesize)
+            MigrationLog.log_paged_surveys(surveys)
             surveys = SurveyFilter.filter(surveys)
 
             surveys = strip_none([self.build_cargo(survey) for survey in surveys])
 
             if not surveys:
                 self.load()
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/prefab_factory.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/prefab_factory.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/schema_mapper.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/schema_mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,16 +184,16 @@
     @staticmethod
     def load_file_crates(files_context: [MbFileCrate], prefab: Prefab) -> [CruiseFileCrate]:
         cruise_files_crates = [SchemaMapper.load_cruise_file_crate(file, prefab) for file in files_context]
         return cruise_files_crates
 
     @staticmethod
     def load_cruise_survey(mb_survey: MbSurvey) -> CruiseSurvey:
-        start_time = mb_survey.start_time.strftime('%Y-%m-%dT%H:%M:%S') if mb_survey.start_time else None
-        end_time = mb_survey.end_time.strftime('%Y-%m-%dT%H:%M:%S') if mb_survey.end_time else None  # previously '%d-%b-%y'
+        start_time = mb_survey.start_time if mb_survey.start_time else None
+        end_time = mb_survey.end_time if mb_survey.end_time else None
 
         survey_name = mb_survey.survey_name        # MB.SURVEY.SURVEY_NAME
         parent = None                              # N/A
         platform_name = mb_survey.ship_name        # MB.SURVEY.SHIP_NAME
         start_date = start_time                    # MB.SURVEY.START_TIME
         end_date = end_time                        # MB.SURVEY.END_TIME-
         departure_port = mb_survey.departure_port  # MB.SURVEY.DEPARTURE_PORT
@@ -316,16 +316,15 @@
         mb_file = file_crate.mb_file
         file_type = prefab.files_type  # Derived: dataset type is derived from the data_file paths of files it contains, so file types of files within dataset are determined at dataset creation
 
         file_name = mb_file.data_file.split("/")[-1]  # derived from MB.NGDCID_AND_FILE.DATA_FILE
         raw_size = mb_file.filesize  # MB.NGDCID_AND_FILE.FILESIZE
         publish = "Y" if mb_file.publish.upper() == "yes".upper() else "N"  # derived directly from MB.NGDCID_AND_FILE.PUBLISH
         collection_date = mb_file.entry_date  # MB.NGDCID_AND_FILE.ENTRY_DATE
-        # collection_date = file_crate.mb_info.start_time.strftime('%d-%b-%y %H:%M:%S') if file_crate.mb_info and file_crate.mb_info.start_time else None
-        publish_date = mb_file.process_date  # MB.NGDCID_AND_FILE.PROCESS_DATE
+        publish_date = mb_file.entry_date  # MB.NGDCID_AND_FILE.ENTRY_DATE
         archive_date = mb_file.process_date  # MB.NGDCID_AND_FILE.PROCESS_DATE
         temp_id = None
         gzip_size = mb_file.filesize_gzip  # MB.NGDCID_AND_FILE.FILESIZE_GZIP
         type_id = FTLookup.get_id(file_type)
         format_id = FFLookup.get_id(FFLookup.get_name(mb_file.format_id))  # get format name from mb format id? mb_info.mbio_format_id
 
         version = None
@@ -370,21 +369,14 @@
 
         if mb_info.bathy_beams is not None:
             parameter = ParameterDetailConsts.MB_BATHY_BEAMS
             detail_id = PDLookup.get_id(parameter)
             file_parameters.append(
                 CruiseFileParameter(parameter_detail_name=parameter, parameter_detail_id=detail_id, value=mb_info.bathy_beams, xml=None, json=None)
             )  # MB.MBINFO_FILE_TSQL.BATHY_BEAMS
-
-        if mb_info.bathy_beams is not None:
-            parameter = ParameterDetailConsts.MB_BATHY_BEAMS
-            detail_id = PDLookup.get_id(parameter)
-            file_parameters.append(
-                CruiseFileParameter(parameter_detail_name=parameter, parameter_detail_id=detail_id, value=mb_info.bathy_beams, xml=None, json=None)
-            )  # MB.MBINFO_FILE_TSQL.BATHY_BEAMS
 
         if mb_info.bb_good is not None:
             parameter = ParameterDetailConsts.MB_GOOD_BATH_TOTAL
             detail_id = PDLookup.get_id(parameter)
             file_parameters.append(
                 CruiseFileParameter(parameter_detail_name=parameter, parameter_detail_id=detail_id, value=mb_info.bb_good, xml=None, json=None)
             )  # MB.MBINFO_FILE_TSQL.BB_GOOD
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/processors/transfer_station.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/processors/transfer_station.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/services/cruise_service.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/cruise_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import datetime
+
 from typing import Optional
 
 from oracledb import DatabaseError
 
 from src.mb_cruise_migration.db.cruise_connection import CruiseConnection
 
 from ncei_cruise_schema.entity.dataset_type import DatasetType
@@ -10,14 +12,15 @@
 from ncei_cruise_schema.entity.file_shape_mapping import FileShapeMapping
 from ncei_cruise_schema.entity.file_type import FileType
 from ncei_cruise_schema.entity.project_parameter import ProjectParameter
 from ncei_cruise_schema.entity.survey_shape_mapping import SurveyShapeMapping
 from ncei_cruise_schema.entity.version_description import VersionDescription
 
 from src.mb_cruise_migration.db.query_builder import QueryBuilder
+from src.mb_cruise_migration.framework.consts.date_consts import ORACLE_DATE_FORMAT
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
 from src.mb_cruise_migration.models.cruise.cruise_access_path import CruiseAccessPath
 from src.mb_cruise_migration.models.cruise.cruise_dataset import CruiseDataset
 from src.mb_cruise_migration.models.cruise.cruise_dataset_types import CruiseDatasetType
 from src.mb_cruise_migration.models.cruise.cruise_file_formats import CruiseFileFormat
 from src.mb_cruise_migration.models.cruise.cruise_file_types import CruiseFileType
 from src.mb_cruise_migration.models.cruise.cruise_files import CruiseFile
@@ -49,14 +52,15 @@
 from ncei_cruise_schema.entity.project import Project
 from ncei_cruise_schema.entity.shape import Shape
 from ncei_cruise_schema.orm.query import Where, Order, And
 from ncei_cruise_schema.entity.access_path import AccessPath
 from ncei_cruise_schema.entity.survey import Survey
 
 from src.mb_cruise_migration.models.cruise.cruise_version_descriptions import CruiseVersionDescription
+from src.mb_cruise_migration.utility.common import oracle_date_format
 
 
 def retry_on_disconnect(func):
     def wrap(self, *args, **kwargs):
         try:
             return func(self, *args, **kwargs)
         except DatabaseError:
@@ -298,15 +302,15 @@
     @staticmethod
     def from_model(model) -> ParameterDetail:
         return ParameterDetail(
             id=model.parameter_id,
             parameter=model.parameter,
             parameter_type=model.parameter_type,
             description=model.description,
-            last_update_date=model.last_update_date,
+            last_update_date=oracle_date_format(model.last_update_date, "cruise.parameter_detail.last_update_date"),
             last_updated_by=model.last_updated_by
         )
 
     @staticmethod
     def from_entity(entity: ParameterDetail) -> CruiseParameterDetail:
         return CruiseParameterDetail(
             id=entity.id,
@@ -431,19 +435,19 @@
     @staticmethod
     def from_model(model: CruiseSurvey) -> Survey:
         return Survey(
             id=model.id,
             name=model.survey_name,
             parent=model.parent,
             platform_name=model.platform_name,
-            start_date=model.start_date,
-            end_date=model.end_date,
+            start_date=oracle_date_format(model.start_date, "cruise.survey.start_date"),
+            end_date=oracle_date_format(model.end_date, "cruise.survey.end_date"),
             departure_port=model.departure_port,
             arrival_port=model.arrival_port,
-            last_update=model.last_update,
+            last_update=oracle_date_format(model.last_update, "cruise.survey.last_update"),
             creation_date=model.creation_date
         )
 
     @staticmethod
     def from_entity(entity: Survey) -> CruiseSurvey:
         return CruiseSurvey(
             id=entity.id,
@@ -521,16 +525,16 @@
             other_id=model.other_id,
             name=model.dataset_name,
             dataset_type_name=model.dataset_type_name,
             dataset_type_id=model.dataset_type_id,
             instruments=model.instruments,
             platforms=model.platforms,
             doi=model.doi,
-            archive_date=model.archive_date,
-            last_update=model.last_update,
+            archive_date=oracle_date_format(model.archive_date, "cruise.dataset.archive_date"),
+            last_update=oracle_date_format(model.last_update, "cruise.dataset.last_update"),
             surveys=model.surveys,
             projects=model.projects
         )
 
     @staticmethod
     def from_entity(entity: Dataset) -> CruiseDataset:
         return CruiseDataset(
@@ -958,21 +962,21 @@
     def from_model(model: CruiseFile) -> File:
         return File(
             id=model.id,
             dataset_id=model.dataset_id,
             name=model.file_name,
             raw_size=model.raw_size,
             publish=model.publish,
-            collection_date=model.collection_date,
-            publish_date=model.publish_date,
+            collection_date=oracle_date_format(model.collection_date, "cruise.file.collection_date"),
+            publish_date=oracle_date_format(model.publish_date, "cruise.file.publish_date"),
             version_id=model.version_id,
             type_id=model.type_id,
             format_id=model.format_id,
-            archive_date=model.archive_date,
-            last_update=model.last_update,
+            archive_date=oracle_date_format(model.archive_date, "cruise.file.archive_date"),
+            last_update=oracle_date_format(model.last_update, "cruise.file.last_update"),
             gzip_size=model.gzip_size
         )
 
     @staticmethod
     def from_entity(entity: File) -> CruiseFile:
         return CruiseFile(
             id=entity.id,
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/services/mb_service.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/services/mb_service.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/src/mb_cruise_migration/utility/dataset.py` & `ci_cmg_mb_cruise_migration-1.1/src/mb_cruise_migration/utility/dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -42,24 +42,35 @@
     if designator is not None:
         return " ".join([ship_name, "(" + designator + ")"])
 
     return ship_name
 
 
 def build_dataset_name(dataset_type, survey_name, instrument, provider):
-    if dataset_type == DatasetTypeConsts.MB_RAW or dataset_type == DatasetTypeConsts.MB_RAW_NONPUBLIC:
-        return "_".join([survey_name, instrument])
-    elif dataset_type == DatasetTypeConsts.MB_PRODUCT or dataset_type == DatasetTypeConsts.MB_PROCESSED:
-        return "_".join([survey_name, instrument, provider])
-    elif dataset_type == DatasetTypeConsts.MB_PRODUCT_NONPUBLIC or dataset_type == DatasetTypeConsts.MB_PROCESSED_NONPUBLIC:
-        return "_".join([survey_name, instrument, provider])
-    elif dataset_type == DatasetTypeConsts.METADATA or dataset_type == DatasetTypeConsts.METADATA_NONPUBLIC:
+
+    if dataset_type == DatasetTypeConsts.MB_RAW:
+        return "_".join([survey_name, "RAW", instrument])
+    elif dataset_type == DatasetTypeConsts.MB_RAW_NONPUBLIC:
+        return "_".join([survey_name, "RAW", instrument, "NONPUBLIC"])
+    elif dataset_type == DatasetTypeConsts.MB_PROCESSED:
+        return "_".join([survey_name, "PROCESSED", instrument, provider])
+    elif dataset_type == DatasetTypeConsts.MB_PROCESSED_NONPUBLIC:
+        return "_".join([survey_name, "PROCESSED", instrument, provider, "NONPUBLIC"])
+    elif dataset_type == DatasetTypeConsts.MB_PRODUCT:
+        return "_".join([survey_name, "PRODUCTS", provider])
+    elif dataset_type == DatasetTypeConsts.MB_PRODUCT_NONPUBLIC:
+        return "_".join([survey_name, "PRODUCTS", provider, "NONPUBLIC"])
+    elif dataset_type == DatasetTypeConsts.METADATA:
         return "_".join([survey_name, "METADATA"])
-    elif dataset_type == DatasetTypeConsts.ANCILLARY or dataset_type == DatasetTypeConsts.ANCILLARY_NONPUBLIC:
+    elif dataset_type == DatasetTypeConsts.METADATA_NONPUBLIC:
+        return "_".join([survey_name, "METADATA", "NONPUBLIC"])
+    elif dataset_type == DatasetTypeConsts.ANCILLARY:
         return "_".join([survey_name, "ANCILLARY"])
+    elif dataset_type == DatasetTypeConsts.ANCILLARY_NONPUBLIC:
+        return "_".join([survey_name, "ANCILLARY", "NONPUBLIC"])
     else:
         raise RuntimeError(ErrorConsts.BAD_DATASET_TYPE)
 
 
 def get_dataset_instrument(dataset_type: DatasetTypeConsts, mb_file: MbFileCrate, survey_instrument: str) -> Optional[str]:
     parsed_file = mb_file.mb_file.parsed_file
     if DatasetTypeConsts.dataset_has_associated_instrument(dataset_type):
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/config_test.yaml` & `ci_cmg_mb_cruise_migration-1.1/tests/config_test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
   sid: ""
   service: "XEPDB1"
   pooled: False
 
 log:
   log_root: ""
   log_dir: "log"
+  review_dir: "review"
   report_dir: "report"
   level: "info"
   log_size_mb: 10
 
 run_parameters:
   migrate_shapes: False
   max_queue_size: 10
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/start-it.sh` & `ci_cmg_mb_cruise_migration-1.1/tests/start-it.sh`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_batch_insert.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_batch_insert.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from src.mb_cruise_migration.db.cruise_db import CruiseDb
 from src.mb_cruise_migration.db.cruise_connection import CruiseConnection
 from src.mb_cruise_migration.framework.consts.dataset_type_consts import DatasetTypeConsts
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.models.cruise.cruise_dataset import CruiseDataset
 from src.mb_cruise_migration.models.cruise.cruise_files import CruiseFile
 from src.mb_cruise_migration.services.cruise_service import FileService, DatasetService
-from tests.testutils import get_file_parameters
+from testutils import get_file_parameters
 
 
 class TestBatchInsert(unittest.TestCase):
     MigrationProperties("config_test.yaml")
 
     def setUp(self) -> None:
         self.tearDown()
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_cleaner.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_cleaner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 
 from src.mb_cruise_migration.cleaner import Cleaner
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.migrator import Migrator
-from tests.testutils import load_test_mb_data, clean_cruise_db, \
+from testutils import load_test_mb_data, clean_cruise_db, \
     get_cruise_datasets, get_files, get_access_paths, get_dataset_projects, \
     get_dataset_platforms, get_dataset_instrument, get_dataset_surveys, \
     get_file_access_paths, get_dataset_parameters, get_file_parameters, clean_mb_db
 
 
 class TestCleaner(unittest.TestCase):
     MigrationProperties("config_test.yaml")
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_configurable_survey_query.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_configurable_survey_query.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_const_initializer.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_const_initializer.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_designator_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_designator_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_instrument_resolver.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_instrument_resolver.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_processor.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         ConstInitializer.initialize_consts()
 
         # build cargo
         file1 = create_test_file(
             file_name="/path/to/file/filename.mb.all",
             raw_size=52460436,
             publish="Y",
-            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5).isoformat(),
-            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13).isoformat(),
+            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5),
+            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13),
             temp_id=None,
             gzip_size=48460436,
             version_id=VDLookup.get_id_from_description("RAW"),
             format_id=FFLookup.get_id("MBF_SBSIOSWB"),
             type_id=FTLookup.get_id("MB RAW")
         )
         file1_access_path1 = create_test_access_path(path="/path", path_type="winding")
@@ -53,17 +53,17 @@
         file_crate1.file_parameters = [file1_parameter1, file1_parameter2]
         file_crate1.file_shape = file1_shape
 
         file2 = create_test_file(
             file_name="/path/to/file/filename.mb.all",
             raw_size=52460436,
             publish="Y",
-            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5).isoformat(),
-            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13).isoformat(),
+            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5),
+            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13),
             temp_id=None,
             gzip_size=48460436,
             version_id=VDLookup.get_id_from_description("PROCESSED"),
             format_id=FFLookup.get_id("ASCII_TEXT"),
             type_id=FTLookup.get_id("MB PRODUCT")
         )
         file2_access_path1 = create_test_access_path(path="/path", path_type="winding")
@@ -82,15 +82,15 @@
 
         dataset = create_test_dataset(
             other_id="02030057",
             dataset_name="KN159L5_SeaBeam2112",
             dataset_type_name="MB RAW",
             instruments="SeaBeam2112",
             platforms="Knorr",
-            archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat(),
+            archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3),
             surveys="KN159L5",
             projects="Project Manhattan",
             type_id=DTLookup.get_id("MB RAW")
         )
 
         dataset_parameter1 = create_test_parameter(parameter="DEPTH", value="infinite", detail_id=PDLookup.get_id("FILE_FORMAT_TYPE"))
         dataset_parameter2 = create_test_parameter(parameter="DIST", value="far", detail_id=PDLookup.get_id("MB_MAX_ALTITUDE"))
@@ -130,16 +130,16 @@
 
         cruise_survey = create_test_survey(
             name="Falkor999",
             parent=5,
             platform="popeye power",
             departure_port="hong kong",
             arrival_port="pearl harbor",
-            start_date=datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat(),
-            end_date=datetime.datetime(2020, 5, 20, 1, 2, 3).isoformat()
+            start_date=datetime.datetime(2020, 5, 19, 1, 2, 3),
+            end_date=datetime.datetime(2020, 5, 20, 1, 2, 3)
         )
         survey_parameter1 = create_test_parameter(parameter="METAL", value="tin", detail_id=PDLookup.get_id("DIRECTORY_STRUCTURE_TYPE"))
         survey_parameter2 = create_test_parameter(parameter="WOOD", value="oak", detail_id=PDLookup.get_id("NAV1"))
         survey_parameters = [survey_parameter1, survey_parameter2]
         survey_shape = create_test_shape(shape='POINT(0 0)', shape_type="survey", geom_type="geom_type",)
 
         survey_crate = CruiseSurveyCrate()
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_cruise_service_crud.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_cruise_service_crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import unittest
 import datetime
 
 from ncei_cruise_schema.entity.file import File
 
 from src.mb_cruise_migration.db.cruise_db import CruiseDb
+from src.mb_cruise_migration.framework.consts.date_consts import ORACLE_DATE_FORMAT
 from src.mb_cruise_migration.framework.resolvers.dataset_type_resolver import DTLookup, DatasetTypeConsts
 from src.mb_cruise_migration.framework.resolvers.file_format_resolver import FFLookup
 from src.mb_cruise_migration.framework.resolvers.file_type_resolver import FTLookup
 from src.mb_cruise_migration.framework.resolvers.version_description_resolver import VDLookup
 from src.mb_cruise_migration.framework.consts.const_initializer import ConstInitializer
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
 from src.mb_cruise_migration.migration_properties import MigrationProperties
@@ -28,15 +29,15 @@
 from src.mb_cruise_migration.models.cruise.cruise_projects import CruiseProject
 from src.mb_cruise_migration.models.cruise.cruise_surveys import CruiseSurvey
 from src.mb_cruise_migration.services.cruise_service import AccessPathService, SurveyService, \
     ShapeService, ProjectService, PlatformService, ParameterService, \
     InstrumentService, FileService, ContactService, DatasetService, \
     DatasetTypeService, FileFormatService, FileTypeService, \
     VersionDescriptionService, ParameterDetailService
-from tests.testutils import create_test_file, create_test_dataset, clean_cruise_db
+from testutils import create_test_file, create_test_dataset, clean_cruise_db
 
 
 class TestCruiseServiceCrud(unittest.TestCase):
     MigrationProperties("config_test.yaml")
     MigrationLog()
 
     def tearDown(self):
@@ -47,15 +48,15 @@
         ConstInitializer.initialize_consts()
 
         other_id = "02030057"
         dataset_name = "KN159L5_SeaBeam2112"
         dataset_type_name = "MB RAW"
         instruments = "SeaBeam2112"
         platforms = "Knorr"
-        archive_date = datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat()
+        archive_date = datetime.datetime(2020, 5, 19, 1, 2, 3)
         surveys = "KN159L5"
         projects = "Project Manhattan"
         dataset_type_id = DTLookup.get_id(DatasetTypeConsts.MB_RAW)
 
         model = CruiseDataset(
             other_id=other_id,
             dataset_name=dataset_name,
@@ -72,29 +73,29 @@
         saved = dataset_service.save_new_dataset(model)
 
         self.assertTrue(isinstance(saved, Dataset))
         self.assertEqual(saved.other_id, other_id)
         self.assertEqual(saved.dataset_type_name, dataset_type_name)
         self.assertEqual(saved.instruments, instruments)
         self.assertEqual(saved.platforms, platforms)
-        self.assertEqual(saved.archive_date, archive_date)
+        self.assertEqual(saved.archive_date, archive_date.strftime(ORACLE_DATE_FORMAT).upper())
         self.assertEqual(saved.surveys, surveys)
         self.assertEqual(saved.projects, projects)
         self.assertEqual(saved.dataset_type_id, dataset_type_id)
         self.assertIsNotNone(saved.id)
 
         # Find existing
         found = dataset_service.find_by_dataset_name(dataset_name)
 
         self.assertTrue(isinstance(found, Dataset))
         self.assertEqual(found.other_id, other_id)
         self.assertEqual(found.dataset_type_name, dataset_type_name)
         self.assertEqual(found.instruments, instruments)
         self.assertEqual(found.platforms, platforms)
-        self.assertEqual(found.archive_date, archive_date)
+        self.assertEqual(found.archive_date, archive_date.strftime(ORACLE_DATE_FORMAT).upper())
         self.assertEqual(found.surveys, surveys)
         self.assertEqual(found.projects, projects)
         self.assertEqual(found.dataset_type_id, dataset_type_id)
         self.assertIsNotNone(found.id)
         self.assertEqual(found.id, saved.id)
 
         found_by_id = dataset_service.find_by_id(found.id)
@@ -145,16 +146,16 @@
         self.survey_service = SurveyService(CruiseDb())
 
         name = "Falkor999"
         parent = 5
         platform = "popeye power"
         departure_port = "hong kong"
         arrival_port = "pearl harbor"
-        start_date = datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat()
-        end_date = datetime.datetime(2020, 5, 20, 1, 2, 3).isoformat()
+        start_date = datetime.datetime(2020, 5, 19, 1, 2, 3)
+        end_date = datetime.datetime(2020, 5, 20, 1, 2, 3)
 
         model = CruiseSurvey(
             survey_name=name,
             parent=parent,
             platform_name=platform,
             departure_port=departure_port,
             arrival_port=arrival_port,
@@ -167,28 +168,28 @@
 
         self.assertTrue(isinstance(saved, Survey))
         self.assertEqual(saved.name, name)
         self.assertEqual(saved.parent, parent)
         self.assertEqual(saved.platform_name, platform)
         self.assertEqual(saved.departure_port, departure_port)
         self.assertEqual(saved.arrival_port, arrival_port)
-        self.assertEqual(saved.start_date, start_date)
-        self.assertEqual(saved.end_date, end_date)
+        self.assertEqual(saved.start_date, start_date.strftime(ORACLE_DATE_FORMAT).upper())
+        self.assertEqual(saved.end_date, end_date.strftime(ORACLE_DATE_FORMAT).upper())
         self.assertIsNotNone(saved.id)
 
         # Find existing
         found = self.survey_service.find_by_survey_name(model.survey_name)
         self.assertTrue(isinstance(found, Survey))
         self.assertEqual(found.name, name)
         self.assertEqual(found.parent, parent)
         self.assertEqual(found.platform_name, platform)
         self.assertEqual(found.departure_port, departure_port)
         self.assertEqual(found.arrival_port, arrival_port)
-        self.assertEqual(found.start_date, start_date)
-        self.assertEqual(found.end_date, end_date)
+        self.assertEqual(found.start_date, start_date.strftime(ORACLE_DATE_FORMAT).upper())
+        self.assertEqual(found.end_date, end_date.strftime(ORACLE_DATE_FORMAT).upper())
         self.assertIsNotNone(found.id)
 
         # Delete
         self.survey_service.delete_survey(found)
         deleted = self.survey_service.find_by_survey_name(name)
         self.assertIsNone(deleted)
 
@@ -251,28 +252,28 @@
 
         dataset_model = create_test_dataset(
             other_id="02030057",
             dataset_name="KN159L5_SeaBeam2112",
             dataset_type_name="MB RAW",
             instruments="SeaBeam2112",
             platforms="Knorr",
-            archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat(),
+            archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3),
             surveys="KN159L5",
             projects="Project Manhattan",
             type_id=DTLookup.get_id(DatasetTypeConsts.MB_RAW)
         )
         dataset = dataset_service.save_new_dataset(dataset_model)
 
         model = create_test_file(
             file_name="/path/to/file/filename.mb.all",
             raw_size=52460436,
             publish="Y",
-            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5).isoformat(),
-            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13).isoformat(),
+            collection_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+            publish_date=datetime.datetime(2020, 5, 18, 1, 2, 5),
+            archive_date=datetime.datetime(2020, 5, 18, 11, 12, 13),
             temp_id=None,
             gzip_size=48460436,
             version_id=VDLookup.get_id_from_description("PROCESSED"),
             format_id=FFLookup.get_id("ASCII_TEXT"),
             type_id=FTLookup.get_id("MB PRODUCT")
         )
 
@@ -282,33 +283,33 @@
         saved = file_service.save_new_file(model)
 
         self.assertTrue(isinstance(saved, File))
 
         self.assertEqual(model.file_name, saved.name)
         self.assertEqual(model.raw_size, saved.raw_size)
         self.assertEqual(model.publish, saved.publish)
-        self.assertEqual(model.collection_date, saved.collection_date)
-        self.assertEqual(model.publish_date, saved.publish_date)
-        self.assertEqual(model.archive_date, saved.archive_date)
+        self.assertEqual(model.collection_date.strftime(ORACLE_DATE_FORMAT).upper(), saved.collection_date)
+        self.assertEqual(model.publish_date.strftime(ORACLE_DATE_FORMAT).upper(), saved.publish_date)
+        self.assertEqual(model.archive_date.strftime(ORACLE_DATE_FORMAT).upper(), saved.archive_date)
         self.assertEqual(model.temp_id, saved.temp_id)
         self.assertEqual(model.gzip_size, saved.gzip_size)
         self.assertEqual(model.version_id, saved.version_id)
         self.assertEqual(model.format_id, saved.format_id)
         self.assertEqual(model.type_id, saved.type_id)
 
         self.assertIsNotNone(saved.id)
 
         # Find existing
         found = file_service.find_by_file_name(model.file_name)
         self.assertEqual(model.file_name, found.name)
         self.assertEqual(model.raw_size, found.raw_size)
         self.assertEqual(model.publish, found.publish)
-        self.assertEqual(model.collection_date, found.collection_date)
-        self.assertEqual(model.publish_date, found.publish_date)
-        self.assertEqual(model.archive_date, found.archive_date)
+        self.assertEqual(model.collection_date.strftime(ORACLE_DATE_FORMAT).upper(), found.collection_date)
+        self.assertEqual(model.publish_date.strftime(ORACLE_DATE_FORMAT).upper(), found.publish_date)
+        self.assertEqual(model.archive_date.strftime(ORACLE_DATE_FORMAT).upper(), found.archive_date)
         self.assertEqual(model.temp_id, found.temp_id)
         self.assertEqual(model.gzip_size, found.gzip_size)
         self.assertEqual(model.version_id, found.version_id)
         self.assertEqual(model.format_id, found.format_id)
         self.assertEqual(model.type_id, found.type_id)
         self.assertIsNotNone(found.id)
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_end_to_end_it.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_end_to_end_it.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import unittest
-
 from src.mb_cruise_migration.migrator import Migrator
 from src.mb_cruise_migration.processors.cruise_processor import CruiseProcessor
 
-from tests.testutils import clean_mb_db, clean_cruise_db, reset_properties, \
+from testutils import clean_mb_db, clean_cruise_db, reset_properties, \
     get_cruise_surveys, get_cruise_datasets, get_files, get_platforms, \
     get_instruments, get_projects, get_people_and_sources, get_access_paths, \
     get_shapes, get_survey_parameters, get_project_parameters, \
     get_dataset_parameters, get_file_parameters, get_dataset_projects, \
     get_dataset_platforms, get_dataset_instrument, get_dataset_surveys, \
     get_scientists, get_sources, get_dataset_shapes, get_survey_shapes, \
-    get_file_shapes, get_file_access_paths, load_test_mb_data
+    get_file_shapes, get_file_access_paths, load_test_mb_data, delete_test_logs
 
 
 class TestEndToEndIntegration(unittest.TestCase):
 
     def setUp(self) -> None:
+        delete_test_logs()
         reset_properties()
         self.tearDown()
 
     def tearDown(self) -> None:
         self.migrator = Migrator("config_test.yaml")
         clean_mb_db()
         clean_cruise_db()
@@ -33,14 +33,16 @@
     def test_end_to_end_RR1808_lite(self):
         test_data_file = "RR1808_lite.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=2,
             num_datasets_with_instruments=1,
             num_instruments=1,
             num_scientists=1,
             num_files=8,
             num_mbinfo_records=2,
@@ -50,17 +52,19 @@
 
     @unittest.skip("Not implemented yet.")
     def test_end_to_end_NEW1208_lite(self):
         """a.k.a HE0302"""
         test_data_file = "NEW1208_lite.sql"
         load_test_mb_data(test_data_file)
 
-        migrator = Migrator()
+        migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=1,
             num_datasets_with_instruments=0,
             num_instruments=1,
             num_scientists=1,
             num_files=8,
             num_mbinfo_records=2,
@@ -92,14 +96,16 @@
     def test_end_to_end_RR1808(self):
         test_data_file = "RR1808.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=2,
             num_datasets_with_instruments=1,
             num_instruments=1,
             num_scientists=1,
             num_files=157,
             num_mbinfo_records=142,
@@ -116,14 +122,16 @@
 
         test_data_file = "NEW3020.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=5,
             num_datasets_with_instruments=3,
             num_instruments=1,
             num_scientists=2,
             num_files=989,
             num_mbinfo_records=811,
@@ -141,14 +149,16 @@
 
         test_data_file = "NEW3549.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=4,
             num_instruments=1,
             num_datasets_with_instruments=2,
             num_scientists=1,
             num_files=603,  # WCD file gets filtered out
             num_mbinfo_records=240,
@@ -165,40 +175,44 @@
         """
         test_data_file = "NEW1570.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         num_files = 450
 
         self.validate_structure_results(
             num_datasets=5,
             num_instruments=1,
             num_datasets_with_instruments=3,
             num_scientists=1,
             num_files=450,  # filters out WCD "file"
             num_access_paths=13,  # one less than normal due to no archive path for survey metadata
             num_survey_params=4,  # NAV1, Comments, Previous_State, Proprietary
             num_paths_per_file=1,
             num_file_access_paths=(num_files*2) - 1,  # survey metadata only has one access path, wcd file already "filtered" out of total
             num_file_parameters=1,
-            num_mbinfo_records=16345,  # not all mbinfo records fully populated. 194 have 14 null values. So, 16345 file parameters instead of normal 19061
+            num_mbinfo_records=15956,  # not all mbinfo records fully populated. 194 have 14 null values. 194 *
         )
 
     def test_end_to_end_NEW3206(self):
         """
         this one has two sources, R2R (version1) and MGDS (version2).  These should become separate datasets.
         """
         test_data_file = "NEW3206.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=3,
             num_datasets_with_instruments=2,
             num_instruments=1,
             num_scientists=1,
             num_files=103,
             num_mbinfo_records=91,
@@ -212,14 +226,16 @@
         """
         test_data_file = "NEW3370.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=3,
             num_datasets_with_instruments=2,
             num_instruments=2,
             num_scientists=1,
             num_files=25,
             num_mbinfo_records=18,
@@ -235,14 +251,16 @@
 
         test_data_file = "NEW1208.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=5,
             num_datasets_with_instruments=3,
             num_instruments=1,
             num_scientists=1,
             num_files=522,
             num_mbinfo_records=243,
@@ -262,14 +280,16 @@
 
         test_data_file = "NEW523.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+
         self.validate_structure_results(
             num_datasets=2,
             num_datasets_with_instruments=1,
             num_instruments=1,
             num_scientists=1,
             num_files=237,
             num_mbinfo_records=235,
@@ -289,14 +309,23 @@
 
         test_data_file = "NEW2176.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+        expected_instrument_name = "SB7101"
+        expected_instrument_long_name = "Reson SeaBat 7101"
+
+        with self.subTest(msg="instrument short name"):
+            self.assertEqual(expected_instrument_name, instruments[0][1])
+        with self.subTest(msg="instrument short name"):
+            self.assertEqual(expected_instrument_long_name, instruments[0][3])
+
         self.validate_structure_results(
             num_datasets=2,
             num_datasets_with_instruments=1,
             num_instruments=1,
             num_scientists=1,
             num_files=1048,
             num_mbinfo_records=0,
@@ -314,25 +343,55 @@
         """
         test_data_file = "NEW3106.sql"
         load_test_mb_data(test_data_file)
 
         migrator = Migrator("config_test.yaml")
         migrator.migrate()
 
+        instruments = get_instruments()
+        expected_instrument_name = "EM122"
+        expected_instrument_long_name = "Kongsberg EM122"
+
+        with self.subTest(msg="instrument short name"):
+            self.assertEqual(expected_instrument_name, instruments[0][1])
+        with self.subTest(msg="instrument short name"):
+            self.assertEqual(expected_instrument_long_name, instruments[0][3])
+
         self.validate_structure_results(
             num_datasets=3,
             num_datasets_with_instruments=1,
             num_instruments=1,
             num_scientists=0,
             num_files=285,
             num_mbinfo_records=283,
             num_access_paths=6,
             num_survey_params=4,  # NAV1, Horizontal_Datum, Previous_State, Proprietary
         )
 
+    def test_end_to_end_NEW3403(self):
+        """
+        AKA FSPT180004
+        submission from Fugro, one of our regular providers.  Should be straightforward.
+        One instrument, one level of processing, and one metadata record and some ancillary.
+        """
+        test_data_file = "NEW3403.sql"
+        load_test_mb_data(test_data_file)
+
+        migrator = Migrator("config_test.yaml")
+        migrator.migrate()
+
+        instruments = get_instruments()
+        expected_instrument_name = "EM124"
+        expected_instrument_long_name = "Kongsberg EM124"
+
+        with self.subTest(msg="validate instrument mapping"):
+            self.assertEqual(1, len(instruments))
+            self.assertEqual(expected_instrument_name, instruments[0][1])
+            self.assertEqual(expected_instrument_long_name, instruments[0][3])
+
     def test_end_to_end_all_at_once(self):
 
         load_test_mb_data("RR1808.sql")
         load_test_mb_data("NEW3020.sql")
         load_test_mb_data("NEW3549.sql")
         load_test_mb_data("NEW1570.sql")
         load_test_mb_data("NEW3206.sql")
@@ -390,15 +449,15 @@
             num_survey_params,
             num_shapes=0,
             num_survey_shapes=0,
             num_dataset_shapes=0,
             num_file_shapes=0,
             num_paths_per_file=2,
             num_dataset_parameters=6,
-            num_file_parameters=49,
+            num_file_parameters=48,
             num_dataset_platforms=1,
             num_file_access_paths=None
             ):
         if not num_file_access_paths:
             num_file_access_paths = (num_files * num_paths_per_file)
 
         surveys = get_cruise_surveys()
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_mb_filters.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,16 +21,16 @@
 
 class TestFileFilter(unittest.TestCase):
 
     file_standard = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/em122/0140_20180617_101452_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=32143468,
         filesize_gzip=15813031,
@@ -41,16 +41,16 @@
     )
     file_standard.parsed_file = ParsedFilePath(file_standard.data_file)
 
     file_standard_nonpublic = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/em122/nonpublic/0150_20180617_151453_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -61,16 +61,16 @@
     )
     file_standard_nonpublic.parsed_file = ParsedFilePath(file_standard_nonpublic.data_file)
 
     file_standard_no_instrument_dir = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/0140_20180617_101452_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=32143468,
         filesize_gzip=15813031,
@@ -81,16 +81,16 @@
     )
     file_standard_no_instrument_dir.parsed_file = ParsedFilePath(file_standard_no_instrument_dir.data_file)
 
     file_WCD = MbFile(
         ngdc_id='NEW2930',
         data_file='WCD',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -101,16 +101,16 @@
     )
     file_WCD.parsed_file = ParsedFilePath(file_WCD.data_file)
 
     file_singlebeam = MbFile(
         ngdc_id='NEW2930',
         data_file='singlebeam',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -121,16 +121,16 @@
     )
     file_singlebeam.parsed_file = ParsedFilePath(file_singlebeam.data_file)
 
     file_XTF = MbFile(
         ngdc_id='NEW2930',
         data_file='XTF',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -141,16 +141,16 @@
     )
     file_XTF.parsed_file = ParsedFilePath(file_XTF.data_file)
 
     file_Canadian = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/Canadian_Data/1999/1999Sidney/filename.ext',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -161,16 +161,16 @@
     )
     file_Canadian.parsed_file = ParsedFilePath(file_Canadian.data_file)
 
     file_legs = MbFile(
         ngdc_id='NEW2930',
         data_file='oocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/leg1/0140_20180617_101452_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -181,16 +181,16 @@
     )
     file_legs.parsed_file = ParsedFilePath(file_legs.data_file)
 
     file_region = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/kauai/0140_20180617_101452_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -201,16 +201,16 @@
     )
     file_region.parsed_file = ParsedFilePath(file_region.data_file)
 
     file_zone = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/ZONE_AGH/0140_20180617_101452_revelle.all.mb58.gz',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -221,16 +221,16 @@
     )
     file_zone.parsed_file = ParsedFilePath(file_zone.data_file)
 
     file_extraneous = MbFile(
         ngdc_id='NEW2930',
         data_file='ocean/ships/roger_revelle/RR1808/multibeam/data/version1/products/Backscatter/filename.ext',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -241,16 +241,16 @@
     )
     file_extraneous.parsed_file = ParsedFilePath(file_extraneous.data_file)
 
     file_survey_metadata = MbFile(
         ngdc_id='NEW2930',
         data_file='MGG/Multibeam/iso/xml/filename.file',
         format_id=58,
-        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
-        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4).isoformat(),
+        entry_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
+        process_date=datetime.datetime(2020, 5, 18, 1, 2, 4),
         status='arrgh matey',
         version=1,
         mostcurrent=1,
         version_id=0,
         process_notes='thar be dragons',
         filesize=23576814,
         filesize_gzip=13715710,
@@ -393,15 +393,15 @@
 
         survey_instrument = None
         result = FileFilter.filter_invalid_files(files)
         result, removed = FileFilter.filter_files_not_configured_for_migration(result)
         result = FileLabeler.label(result)
         result = [MbFileCrate(file, None, None) for file in result]
         result = FileDecoder.decode(result)
-        result = FileValidator.validate(result, survey_instrument)
+        result, end_count = FileValidator.validate(result, survey_instrument)
         self.assertEqual(1, len(result))
 
     def test_missing_file_instrument_and_multiple_values_in_survey_instrument(self):
         MigrationProperties("config_test.yaml")
         MigrationLog()
         config = MigrationProperties.migrate
         config.standard = True
@@ -420,13 +420,13 @@
 
         survey_instrument = "EM710; EM122"
         result = FileFilter.filter_invalid_files(files)
         result, removed = FileFilter.filter_files_not_configured_for_migration(result)
         result = FileLabeler.label(result)
         result = [MbFileCrate(file, None, None) for file in result]
         result = FileDecoder.decode(result)
-        result = FileValidator.validate(result, survey_instrument)
+        result, end_count = FileValidator.validate(result, survey_instrument)
         self.assertEqual(1, len(result))
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_mb_paginator.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 
         skip, limit = paginator.paginate()
         self.assertEqual(0, skip)
         self.assertEqual(10, limit)
 
         skip, limit = paginator.paginate()
         self.assertEqual(10, skip)
-        self.assertEqual(20, limit)
+        self.assertEqual(10, limit)
 
         paginator.paginate()
         paginator.paginate()
         paginator.paginate()
         paginator.paginate()
         paginator.paginate()
         paginator.paginate()
         paginator.paginate()
         skip, limit = paginator.paginate()
         self.assertEqual(90, skip)
-        self.assertEqual(99, limit)
+        self.assertEqual(9, limit)
 
         self.assertTrue(paginator.done())
         self.assertRaises(StopIteration, paginator.paginate)
 
     def test_edge_case_pagination(self):
 
         paginator = Paginator(pagesize=10, table_size=4)
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_mb_processor.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
 from src.mb_cruise_migration.models.intermediary.mb_cargo import MbCargo, MbSurveyCrate, MbFileCrate
 from src.mb_cruise_migration.processors.mb_processor import MbProcessor
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.services.mb_service import MbService
 from src.mb_cruise_migration.models.mb.mb_ngdcid_and_file import MbFile
 from src.mb_cruise_migration.models.mb.mb_mbinfo_file_tsql import MbInfo
-from tests.testutils import clean_mb_db, load_test_mb_data
+from testutils import clean_mb_db, load_test_mb_data
 
 
 class TestMbIntegration(unittest.TestCase):
     test_data_file = "RR1808_lite.sql"
 
     def setUp(self) -> None:
         MigrationProperties("config_test.yaml")  # load app configuration from file
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_mb_service.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.models.mb.mb_mbinfo_file_tsql import MbInfo
 from src.mb_cruise_migration.models.mb.mb_ngdcid_and_file import MbFile
 from src.mb_cruise_migration.models.mb.mb_survey import MbSurvey
 from src.mb_cruise_migration.models.mb.mb_survey_reference import SurveyReference
 from src.mb_cruise_migration.services.mb_service import MbService
-from tests.testutils import load_test_mb_data, clean_mb_db
+from testutils import load_test_mb_data, clean_mb_db
 
 
 class TestMbService(unittest.TestCase):
     MigrationProperties("config_test.yaml")  # load app configuration from file
     MigrationLog()
     mb_service: MbService = MbService()
     test_data_file = "RR1808_lite.sql"
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_mb_survey_blacklist.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_mb_survey_blacklist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import unittest
 
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.framework.consts.const_initializer import ConstInitializer
 from src.mb_cruise_migration.processors.mb_processor import MbProcessor
-from tests.testutils import load_test_mb_data, clean_mb_db
+from testutils import load_test_mb_data, clean_mb_db
 
 
 class TestSurveyBlacklist(unittest.TestCase):
     MigrationProperties("config_test.yaml")
     MigrationLog()
 
     def setUp(self) -> None:
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_standard_mapping.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_standard_mapping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import datetime
 import unittest
 
 from src.mb_cruise_migration.db.cruise_db import CruiseDb
+from src.mb_cruise_migration.framework.consts.date_consts import ORACLE_DATE_FORMAT
 from src.mb_cruise_migration.framework.parsed_data_file import ParsedFilePath
 from src.mb_cruise_migration.framework.file_decoder import FileDecoder
 from src.mb_cruise_migration.logging.migration_log import MigrationLog
-from tests.testutils import clean_cruise_db
+from testutils import clean_cruise_db
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 
 from src.mb_cruise_migration.framework.resolvers.dataset_type_resolver import DatasetTypeConsts, DTLookup
 from src.mb_cruise_migration.framework.consts.file_label_consts import FileLabels
 from src.mb_cruise_migration.framework.consts.platform_type_consts import PlatformTypeConsts
 from src.mb_cruise_migration.models.cruise.cruise_access_path import CruiseAccessPath
 from src.mb_cruise_migration.models.cruise.cruise_dataset import CruiseDataset
@@ -73,16 +74,16 @@
         # survey and survey related tables
         survey = cargo.related_survey_crate.cruise_survey
         self.assertTrue(isinstance(survey, CruiseSurvey))
         self.assertIsNone(survey.id)
         self.assertEqual("RR1808", survey.survey_name)
         self.assertIsNone(survey.parent)
         self.assertEqual("Roger Revelle", survey.platform_name)
-        self.assertEqual("2018-06-13T00:00:00", survey.start_date)
-        self.assertEqual("2018-06-17T00:00:00", survey.end_date)
+        self.assertEqual("13-JUN-18", survey.start_date.strftime(ORACLE_DATE_FORMAT).upper())
+        self.assertEqual("17-JUN-18", survey.end_date.strftime(ORACLE_DATE_FORMAT).upper())
         self.assertEqual("Newport, Oregon", survey.departure_port)
         self.assertEqual("Newport, Oregon", survey.arrival_port)
         self.assertIsNone(survey.creation_date)
         self.assertIsNone(survey.last_update)
 
         survey_parameters = cargo.related_survey_crate.survey_parameters
         self.assertEqual(9, len(survey_parameters))
@@ -128,15 +129,15 @@
         self.assertEqual("LINESTRING (30 10, 10 30, 40 40)", survey_shape.shape)  # TODO
         self.assertIsNone(survey_shape.id)
 
         # dataset and dataset related tables
         dataset = cargo.dataset_crate.dataset
         self.assertTrue(isinstance(dataset, CruiseDataset))
         self.assertEqual("NEW2930", dataset.other_id)
-        self.assertEqual("RR1808_EM122", dataset.dataset_name)
+        self.assertEqual("RR1808_RAW_EM122", dataset.dataset_name)
         self.assertEqual(DatasetTypeConsts.MB_RAW, dataset.dataset_type_name)
         self.assertEqual("EM122", dataset.instruments)
         self.assertEqual("Roger Revelle (RR)", dataset.platforms)
         self.assertEqual("04-SEP-19", dataset.archive_date)
         self.assertEqual("RR1808", dataset.surveys)
         self.assertEqual("Cascadia GPS-A", dataset.projects)
         self.assertEqual(DTLookup.get_id(DatasetTypeConsts.MB_RAW), dataset.dataset_type_id)
@@ -262,15 +263,15 @@
         for crate in file_crates:
             file = crate.file
             self.assertTrue(isinstance(file, CruiseFile))
             self.assertEqual("0140_20180617_101452_revelle.all.mb58.gz", file.file_name)
             self.assertEqual(32143468, file.raw_size)
             self.assertEqual("Y", file.publish)
             self.assertEqual("04-SEP-19", file.collection_date)
-            self.assertEqual("05-SEP-19", file.publish_date)
+            self.assertEqual("04-SEP-19", file.publish_date)
             self.assertEqual("05-SEP-19", file.archive_date)
             self.assertIsNone(file.temp_id)  # TODO verify this was created for old migration script only and is not used.
             self.assertEqual(15813031, file.gzip_size)
             self.assertIsNone(file.id)
             self.assertIsNone(file.dataset_id)
             self.assertEqual(1, file.version_id)
             self.assertEqual(1, file.type_id)
@@ -293,15 +294,15 @@
                     self.assertEqual("ocean/ships/roger_revelle/RR1808/multibeam/data/version1/MB/em122", access_path.path)  # MB.NGDCID_AND_FILE.DATA_FILE
                 elif access_path.path_type == "Stornext":
                     self.assertEqual("/stornext/ngdc/archive/insitu_ocean/trackline/roger_revelle/rr1808/multibeam/data/version1/MB/em122", access_path.path)  # MB.NGDCID_AND_FILE.ARCHIVE_PATH
                 else:
                     self.assertTrue(False)  # must be one of either stornext or disk path type
                 self.assertIsNone(access_path.id)
 
-            self.assertEqual(49, len(crate.file_parameters))
+            self.assertEqual(48, len(crate.file_parameters))
             file_parameters = crate.file_parameters
             for file_parameter in file_parameters:
                 self.assertTrue(isinstance(file_parameter, CruiseFileParameter))
                 self.assertIsNone(file_parameter.id)
                 self.assertIsNone(file_parameter.file_id)
                 if file_parameter.parameter_detail_name == 'MBIO_Format_ID':
                     self.assertEqual(58, file_parameter.value)  # MB.MBINFO_FILE_TSQL.MBIO_FORMAT_ID
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/test_survey_metadata_mapping.py` & `ci_cmg_mb_cruise_migration-1.1/tests/test_survey_metadata_mapping.py`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/testutils.py` & `ci_cmg_mb_cruise_migration-1.1/tests/testutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import datetime
 import os
+import shutil
 
 from src.mb_cruise_migration.db.cruise_db import CruiseDb
 from src.mb_cruise_migration.migration_properties import MigrationProperties
 from src.mb_cruise_migration.models.cruise.cruise_access_path import CruiseAccessPath
 from src.mb_cruise_migration.models.cruise.cruise_dataset import CruiseDataset
 from src.mb_cruise_migration.models.cruise.cruise_files import CruiseFile
 from src.mb_cruise_migration.models.cruise.cruise_instruments import CruiseInstrument
@@ -275,15 +276,15 @@
 def create_test_dataset(other_id, dataset_name, dataset_type_name, instruments, platforms, archive_date, surveys, projects, type_id):
     return CruiseDataset(
         other_id=other_id,
         dataset_name=dataset_name,
         dataset_type_name=dataset_type_name,
         instruments=instruments,
         platforms=platforms,
-        archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3).isoformat(),
+        archive_date=datetime.datetime(2020, 5, 19, 1, 2, 3),
         surveys=surveys,
         projects=projects,
         dataset_type_id=type_id
     )
 
 
 def create_test_source(organization):
@@ -314,7 +315,17 @@
 
 def create_test_shape(shape, shape_type, geom_type):
     return CruiseShape(
         shape=shape,
         shape_type=shape_type,
         geom_type=geom_type,
     )
+
+
+def delete_test_logs():
+
+    if os.path.exists("log"):
+        shutil.rmtree("log")
+    if os.path.exists("report"):
+        shutil.rmtree("report")
+    if os.path.exists("review"):
+        shutil.rmtree("review")
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/create_mb.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/create_mb.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/migrate_cruise.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/migrate_cruise.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1208.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1208_lite.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1208_lite.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW1570.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW1570.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW2176.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW2176.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3020.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3020.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3106.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3106.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3206.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3206.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3370.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3370.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW3549.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW3549.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/NEW523.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/NEW523.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/RR1808.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/RR1808_lite.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/RR1808_lite.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/tests/setup-files/test_data/test_blacklist.sql` & `ci_cmg_mb_cruise_migration-1.1/tests/setup-files/test_data/test_blacklist.sql`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/.gitignore` & `ci_cmg_mb_cruise_migration-1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 coverage.xml
 *.cover
 *.py,cover
 .hypothesis/
 .pytest_cache/
 log/
 report/
+review/
 
 # Translations
 *.mo
 *.pot
 
 # Django stuff:
 *.log
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/LICENSE` & `ci_cmg_mb_cruise_migration-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/README.md` & `ci_cmg_mb_cruise_migration-1.1/README.md`

 * *Files identical despite different names*

### Comparing `ci_cmg_mb_cruise_migration-1.0/pyproject.toml` & `ci_cmg_mb_cruise_migration-1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "oracledb", "pyyaml", "ci-cmg-cruise-schema-orm"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ci-cmg-mb-cruise-migration"
-version = "1.0"
+version = "1.1"
 description = "migrates multibeam metadata from mb schema to cruise schema"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ci_cmg_mb_cruise_migration-1.0/PKG-INFO` & `ci_cmg_mb_cruise_migration-1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ci-cmg-mb-cruise-migration
-Version: 1.0
+Version: 1.1
 Summary: migrates multibeam metadata from mb schema to cruise schema
 Project-URL: Github, https://github.com/CI-CMG/mb-cruise-migration
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
```

