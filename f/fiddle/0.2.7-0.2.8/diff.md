# Comparing `tmp/fiddle-0.2.7.tar.gz` & `tmp/fiddle-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiddle-0.2.7.tar", last modified: Fri Jun 30 20:02:14 2023, max compression
+gzip compressed data, was "fiddle-0.2.8.tar", last modified: Mon Jul 17 18:56:16 2023, max compression
```

## Comparing `fiddle-0.2.7.tar` & `fiddle-0.2.8.tar`

### file list

```diff
@@ -1,218 +1,212 @@
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.7/LICENSE
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-06-30 20:02:14.370883 fiddle-0.2.7/PKG-INFO
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-06-30 20:02:00.000000 fiddle-0.2.7/README.md
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.350883 fiddle-0.2.7/fiddle/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.354883 fiddle-0.2.7/fiddle/_src/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.354883 fiddle-0.2.7/fiddle/_src/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    21439 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/flags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/absl_flags/sample_module_for_flags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/arg_factory_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/building.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/building_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.358883 fiddle-0.2.7/fiddle/_src/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6997 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2212 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9800 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4499 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2940 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7694 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5162 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7708 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6819 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6743 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8402 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2322 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4052 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11018 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3467 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5499 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/auto_config/test_fixtures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17067 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/formatting_utilities.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/import_manager.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/import_manager_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/mini_ast.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/namespace.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/namespace_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/new_codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/new_codegen_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4057 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5783 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/special_value_codegen.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_submodule/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/codegen/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    49485 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    52963 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    26463 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_extensions.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_extensions_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20078 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/daglish_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/diffing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/diffing_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42932 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config_policy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43562 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/auto_config_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.362883 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7228 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14396 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dataclasses_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/dict_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2069 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/fixture_node.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2970 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/fixture_node_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/namespace_config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30108 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2767 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/tied_value.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6335 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/tied_value_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/transform_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/with_tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/with_tags_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3089 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5119 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/flax_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/seqio_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/extensions/tf_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1633 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/field_metadata.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/graphviz_custom_object.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/history_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/materialize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/materialize_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3111 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/module_reflection_test_module.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/mutate_buildable.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/mutate_buildable_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/printing_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/reraised_exception.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/reraised_exception_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9305 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11178 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/selectors_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/signatures_test_helper.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14083 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/tagging_test_module.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/autotest.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/_src/testing/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      925 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/demo_configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/fake_encoder_decoder.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/example/person_friend_toy.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/nested_values.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/nested_values_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/_src/testing/test_util_test.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/absl_flags/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/absl_flags/example/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/business_logic.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/configs.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/example.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/absl_flags/example/tags.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/arg_factory.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/building.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/codegen/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/codegen/auto_config/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/auto_config/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/auto_config/experimental_top_level_api.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      961 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/codegen.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/codegen_diff.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/codegen/py_val_to_cst_converter.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1052 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/config_test.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/daglish.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/diffing.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/examples/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/examples/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/examples/colabs/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/examples/colabs/__init__.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/experimental/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1658 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/auto_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/auto_config_policy.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.366883 fiddle-0.2.7/fiddle/experimental/autobuilders/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/autobuilders/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/configurator.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1523 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/dataclasses.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/dict_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1059 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/fixture_node.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/namespace_config.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/serialization.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      901 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/tied_value.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/transform.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/visualize.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/experimental/yaml_serialization.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/fiddle/extensions/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/jax.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/seqio.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/extensions/tf.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/graphviz.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/history.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/printing.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/selectors.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/signatures.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/tag_type.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/tagging.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.370883 fiddle-0.2.7/fiddle/testing/
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/__init__.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/autotest.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/testing/test_util.py
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-06-30 20:02:01.000000 fiddle-0.2.7/fiddle/version.py
-drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-06-30 20:02:14.350883 fiddle-0.2.7/fiddle.egg-info/
--rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/PKG-INFO
--rw-r-----   0 dhr      (201437) primarygroup (89939)     7188 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/SOURCES.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/dependency_links.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/requires.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-06-30 20:02:14.000000 fiddle-0.2.7/fiddle.egg-info/top_level.txt
--rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-06-30 20:02:14.370883 fiddle-0.2.7/setup.cfg
--rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-06-30 20:02:01.000000 fiddle-0.2.7/setup.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11357 2022-02-19 00:33:27.000000 fiddle-0.2.8/LICENSE
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-17 18:56:16.484165 fiddle-0.2.8/PKG-INFO
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      603 2023-07-17 18:55:59.000000 fiddle-0.2.8/README.md
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.464165 fiddle-0.2.8/fiddle/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1610 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      907 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    21439 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/flags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1021 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/absl_flags/sample_module_for_flags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16567 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15484 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/arg_factory_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5939 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/building.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2483 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/building_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.472165 fiddle-0.2.8/fiddle/_src/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.476165 fiddle-0.2.8/fiddle/_src/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7956 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2506 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5371 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4327 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8540 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9988 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2445 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2187 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1605 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1181 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5242 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3942 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7921 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6294 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8328 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7507 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6743 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8402 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4183 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2322 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4027 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3586 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2047 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2335 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11043 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3467 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5759 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/auto_config/test_fixtures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    17419 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1951 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/formatting_utilities.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     8776 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/import_manager.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5074 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/import_manager_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11220 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9134 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4206 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/mini_ast.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3471 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/namespace.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2204 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/namespace_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5207 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/new_codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3653 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/new_codegen_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4537 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6544 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    15928 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6189 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3500 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/special_value_codegen.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.476165 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      810 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_submodule/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/codegen/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    51137 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    53885 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    27540 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5349 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_extensions.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3241 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_extensions_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    20247 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/daglish_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    41201 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/diffing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    45929 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/diffing_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    42854 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5668 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config_policy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    43562 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/auto_config_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11256 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6512 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      922 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3585 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12374 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    16195 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7228 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14396 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dataclasses_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1173 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2706 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/dict_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1264 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2678 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/namespace_config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    30108 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3228 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4743 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/transform_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11539 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2338 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/with_tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2169 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/with_tags_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2804 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4422 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1324 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/flax_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5458 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1408 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1479 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/seqio_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3433 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4583 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/extensions/tf_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1633 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/field_metadata.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    36979 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2133 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/graphviz_custom_object.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9437 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5216 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/history_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2380 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/materialize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1760 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/materialize_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3459 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2768 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1420 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/module_reflection_test_module.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1795 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/mutate_buildable.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1615 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/mutate_buildable_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    12318 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14648 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/printing_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2879 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/reraised_exception.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2235 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/reraised_exception_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    10408 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    11289 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/selectors_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4274 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     6539 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/signatures_test_helper.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     4267 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     7368 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)    14083 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1275 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/tagging_test_module.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5543 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/autotest.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/_src/testing/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1871 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/demo_configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2533 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/fake_encoder_decoder.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1235 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/example/person_friend_toy.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     5419 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/nested_values.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3155 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/nested_values_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9562 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     9805 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/_src/testing/test_util_test.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/absl_flags/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      967 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.480165 fiddle-0.2.8/fiddle/absl_flags/example/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1342 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/business_logic.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3451 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/configs.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1444 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/example.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      906 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/absl_flags/example/tags.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3528 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/arg_factory.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      792 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/building.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/codegen/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/codegen/auto_config/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      606 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/auto_config/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1828 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/auto_config/experimental_top_level_api.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1076 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/codegen.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/codegen_diff.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1296 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/codegen/py_val_to_cst_converter.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1011 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1002 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/config_test.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2119 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/daglish.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1705 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/diffing.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/examples/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/examples/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/examples/colabs/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/examples/colabs/__init__.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/experimental/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1658 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/auto_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1210 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/auto_config_policy.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/experimental/autobuilders/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1019 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/autobuilders/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1025 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/configurator.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1523 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/dataclasses.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      763 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/dict_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      781 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/namespace_config.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1910 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/serialization.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      860 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/transform.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1327 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/visualize.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1043 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/experimental/yaml_serialization.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/extensions/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      607 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      824 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/jax.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      868 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/seqio.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      840 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/extensions/tf.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      942 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/graphviz.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1184 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/history.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      812 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/printing.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1049 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/selectors.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      866 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/signatures.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      847 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/tag_type.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     2682 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/tagging.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.484165 fiddle-0.2.8/fiddle/testing/
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      801 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/__init__.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     1300 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/autotest.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      762 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/testing/test_util.py
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)      676 2023-07-17 18:56:00.000000 fiddle-0.2.8/fiddle/version.py
+drwxr-x---   0 dhr      (201437) primarygroup (89939)        0 2023-07-17 18:56:16.468165 fiddle-0.2.8/fiddle.egg-info/
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     1631 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/PKG-INFO
+-rw-r-----   0 dhr      (201437) primarygroup (89939)     6948 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/SOURCES.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        1 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/dependency_links.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)      151 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/requires.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)        7 2023-07-17 18:56:16.000000 fiddle-0.2.8/fiddle.egg-info/top_level.txt
+-rw-r-----   0 dhr      (201437) primarygroup (89939)       38 2023-07-17 18:56:16.484165 fiddle-0.2.8/setup.cfg
+-rw-rw-r--   0 dhr      (201437) primarygroup (89939)     3554 2023-07-17 18:56:00.000000 fiddle-0.2.8/setup.py
```

### Comparing `fiddle-0.2.7/LICENSE` & `fiddle-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/PKG-INFO` & `fiddle-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.7
+Version: 0.2.8
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.7/README.md` & `fiddle-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/__init__.py` & `fiddle-0.2.8/fiddle/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/__init__.py` & `fiddle-0.2.8/fiddle/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/absl_flags/__init__.py` & `fiddle-0.2.8/fiddle/_src/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/absl_flags/flags.py` & `fiddle-0.2.8/fiddle/_src/absl_flags/flags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/absl_flags/sample_module_for_flags_test.py` & `fiddle-0.2.8/fiddle/_src/absl_flags/sample_module_for_flags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/arg_factory.py` & `fiddle-0.2.8/fiddle/_src/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/arg_factory_test.py` & `fiddle-0.2.8/fiddle/_src/arg_factory_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/building.py` & `fiddle-0.2.8/fiddle/_src/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/building_test.py` & `fiddle-0.2.8/fiddle/_src/building_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/__init__.py` & `fiddle-0.2.8/fiddle/_src/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/__init__.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir.py`

 * *Files 14% similar despite different names*

```diff
@@ -89,25 +89,48 @@
 @dataclasses.dataclass
 class Parameter(CodegenNode):
   name: Name
   value_type: Optional[Type[Any]] = None
 
 
 @dataclasses.dataclass
-class VariableReference(CodegenNode):
-  """Reference to a variable or parameter."""
+class BaseNameReference(CodegenNode):
+  """Reference to a named symbol (mostly a base class for the below)."""
 
   name: Name
 
 
 @dataclasses.dataclass
-class SymbolReference(CodegenNode):
-  """Reference to a library symbol, like MyEncoderLayer."""
+class VariableReference(BaseNameReference):
+  """Reference to a variable or parameter."""
 
-  expression: str
+
+@dataclasses.dataclass
+class ModuleReference(BaseNameReference):
+  """Reference to an imported module."""
+
+
+@dataclasses.dataclass
+class FixtureReference(BaseNameReference):
+  """Reference to another fixture."""
+
+
+@dataclasses.dataclass
+class AttributeExpression(CodegenNode):
+  """Reference to an attribute of another expression."""
+
+  base: Any  # Wrapped expression, can involve VariableReference's
+  attribute: str
+
+  def __hash__(self):
+    # Currently, some Pax (https://github.com/google/paxml) codegen involves
+    # having AttributeExpression's as dict keys, as those keys are rewritten to
+    # expressions. This function allows for that, but one shouldn't generally
+    # assume equality as object identity here.
+    return id(self)
 
 
 @dataclasses.dataclass
 class ArgFactoryExpr(CodegenNode):
   """Represents a factory that should be interpreted as an argument factory.
 
   Inside Fiddle configs, we represent arg factories with fdl.ArgFactory, e.g.
@@ -137,22 +160,29 @@
   per_field: Dict[str, str] = dataclasses.field(default_factory=dict)
 
 
 @dataclasses.dataclass
 class SymbolOrFixtureCall(CodegenNode):
   """Reference to a call of a library symbol/fixture, like MyEncoderLayer()."""
 
-  symbol_expression: str
+  symbol_expression: Any
   # Values for args can involve VariableReference's, Calls, etc.
   positional_arg_expressions: List[Any]
   arg_expressions: Dict[str, Any]
   history_comments: HistoryComments = dataclasses.field(
       default_factory=HistoryComments
   )
 
+  def __post_init__(self):
+    if isinstance(self.symbol_expression, str):
+      raise TypeError(
+          "Strings are no longer allowed in `symbol_expression`, please wrap"
+          " with a name!"
+      )
+
 
 @dataclasses.dataclass
 class WithTagsCall(CodegenNode):
   """Represents a call to auto_config.with_tags()."""
 
   tag_symbol_expressions: List[str]
   item_to_tag: Any
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/code_ir_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/code_ir_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,14 +37,22 @@
     self.assertEqual(name.previous.value, "foo_1")
     self.assertTrue(name.is_generated)
     self.assertTrue(name.previous.is_generated)
 
 
 class CodegenNodeTest(parameterized.TestCase):
 
+  def test_symbol_expression_string_raises(self):
+    with self.assertRaisesRegex(TypeError, "Strings are no longer allowed.*"):
+      code_ir.FunctoolsPartialCall(
+          symbol_expression="functools.partial",
+          positional_arg_expressions=[],
+          arg_expressions={},
+      )
+
   def test_daglish_iteration(self):
     fn = code_ir.FixtureFunction(
         name=code_ir.Name("foo"),
         parameters=[],
         variables=[],
         output_value=fdl.Config(foo, x=2),
     )
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/complex_to_variables_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/complex_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/experimental_top_level_api_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,20 +185,22 @@
                   "fake_encoder": config.encoder,
                   "fake_decoder": config.decoder,
               },
           ).code
 
         # Choose an arbitrary split point and check that there are more lines
         # when we add more intermediate variables. This is just to ensure that
-        # the MoveComplexNodesToVariables pass is run.
+        # the MoveComplexNodesToVariables pass is run. (We don't currently wrap
+        # lines, so there will be fewer when not extracting variables.)
+        max_lines_when_no_variables = 22
         num_lines = len(code.splitlines())
         if complexity is None:
-          self.assertLessEqual(num_lines, 25)
+          self.assertLessEqual(num_lines, max_lines_when_no_variables)
         else:
-          self.assertGreater(num_lines, 25)
+          self.assertGreater(num_lines, max_lines_when_no_variables)
 
         matches = re.findall(r"def\ (?P<name>[\w_]+)\(", code)
         self.assertEqual(
             matches, ["config_fixture", "fake_encoder", "fake_decoder"]
         )
         module = self._load_code_as_module(code)
         generated_config = module.config_fixture.as_buildable()
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/get_history_comments_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/get_history_comments_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/init_task_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/init_task_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_printer.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_printer.py`

 * *Files 17% similar despite different names*

```diff
@@ -75,22 +75,41 @@
     elif isinstance(value, dict):
       value = state.map_children(value)
       return (
           "{"
           + ", ".join(f'"{key}": {value}' for key, value in value.items())
           + "}"
       )
-    elif isinstance(value, code_ir.VariableReference):
+    elif isinstance(value, code_ir.BaseNameReference):
       return value.name.value
+    elif isinstance(value, code_ir.AttributeExpression):
+      base_obj = state.call(value.base, daglish.Attr("base"))
+      return f"{base_obj}.{value.attribute}"
     elif isinstance(value, code_ir.ArgFactoryExpr):
       sub_value = state.map_children(value).expression
       return f"ArgFactoryExpr[{sub_value}]"
     elif isinstance(value, code_ir.WithTagsCall):
       sub_value = state.map_children(value).expression
       return f"WithTagsCall[{sub_value}]"
+    elif isinstance(value, code_ir.SymbolOrFixtureCall):
+      symbol_expression = state.call(
+          value.symbol_expression, daglish.Attr("symbol_expression")
+      )
+      positional_arg_expressions = state.call(
+          value.positional_arg_expressions,
+          daglish.Attr("positional_arg_expressions"),
+      )
+      arg_expressions = state.call(
+          value.arg_expressions, daglish.Attr("arg_expressions")
+      )
+      return (
+          f"call:<{symbol_expression}"
+          f"(*[{positional_arg_expressions}],"
+          f" **{arg_expressions})>"
+      )
     elif isinstance(value, code_ir.Name):
       return value.value
     elif isinstance(value, type):
       return value.__name__
     elif value in typing_consts or type(value) in typing_consts:
       return str(value)
     else:
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/ir_to_cst.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 **kwargs,
             )
         )
       return args
 
     if isinstance(value, config_lib.Buildable):
       raise ValueError(
-          "Internal Fiddle error: you must run the make_symbolic_reference "
+          "Internal Fiddle error: you must run the make_symbolic_references "
           "passes before CST generation."
       )
     elif isinstance(value, (list, tuple)):
       value = state.map_children(value)
       if isinstance(value, list):
         cst_cls = cst.List
       else:
@@ -92,16 +92,19 @@
     elif isinstance(value, dict):
       elements = []
       for key, sub_value in value.items():
         key_node = state.call(key, daglish.Key(f"__key_{key}"))
         sub_value_node = state.call(sub_value, daglish.Attr(key))
         elements.append(cst.DictElement(key_node, sub_value_node))
       return cst.Dict(elements)
-    elif isinstance(value, code_ir.VariableReference):
+    elif isinstance(value, code_ir.BaseNameReference):
       return cst.Name(value.name.value)
+    elif isinstance(value, code_ir.AttributeExpression):
+      base = state.call(value.base, daglish.Attr("base"))
+      return cst.Attribute(value=base, attr=cst.Name(value.attribute))
     elif isinstance(value, code_ir.SymbolOrFixtureCall):
       attr = daglish.Attr("arg_expressions")
       args = []
       for i, arg_value in enumerate(value.positional_arg_expressions):
         arg_value = state.call(arg_value, attr, daglish.Key(i))
         args.append(cst.Arg(arg_value))
 
@@ -120,41 +123,42 @@
         whitespace_before_args = cst.ParenthesizedWhitespace(
             first_line=cst.TrailingWhitespace(newline=cst.Newline()),
             last_line=cst.SimpleWhitespace(" " * 6),
         )
       else:
         whitespace_before_args = cst.SimpleWhitespace("")
       return cst.Call(
-          cst.parse_expression(value.symbol_expression),
+          state.call(
+              value.symbol_expression, daglish.Attr("symbol_expression")
+          ),
           args=args,
           whitespace_before_args=whitespace_before_args,
       )
     elif isinstance(value, code_ir.WithTagsCall):
       attr = daglish.Attr("item_to_tag")
       item_to_tag = state.call(value.item_to_tag, attr)
       call_args = [cst.Arg(item_to_tag)]
       sorted_tags = sorted([tag for tag in value.tag_symbol_expressions])
       for tag in sorted_tags:
         tag_name = cst.parse_expression(tag)
         call_args.append(cst.Arg(tag_name))
       with_tags = cst.parse_expression("auto_config.with_tags")
       return cst.Call(with_tags, args=call_args)
-    elif isinstance(value, code_ir.SymbolReference):
-      return cst.parse_expression(value.expression)
     elif state.is_traversable(value):
       raise NotImplementedError(
           f"Expression generation is not implemented for {value!r}"
       )
     else:
       # Convert primitives with existing logic.
       try:
         return py_val_to_cst_converter.convert_py_val_to_cst(value)
       except:
         print(f"\n\nERROR CONVERTING: {value!r}")
         print(f"\n\nTYPE: {type(value)}")
+        print(f"\n\nPATH: {daglish.path_str(state.current_path)}")
         raise
 
   return daglish.MemoizedTraversal.run(traverse, expr)
 
 
 def code_for_fn(
     fn: code_ir.FixtureFunction, *, task: code_ir.CodegenTask
@@ -191,15 +195,15 @@
       body=[
           *variable_lines,
           cst.SimpleStatementLine(
               body=[cst.Return(code_for_expr(fn.output_value))]
           ),
       ]
   )
-  if fn.parameters:
+  if fn.parameters and len(fn.parameters) > 1:
     whitespace_before_params = cst.ParenthesizedWhitespace(
         cst.TrailingWhitespace(),
         indent=True,
         last_line=cst.SimpleWhitespace("  "),
     )
   else:
     whitespace_before_params = cst.SimpleWhitespace("")
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/ir_to_cst_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/new_codegen.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,129 +9,133 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Tests for ir_to_cst."""
+"""Generates Fiddle code with the auto_config codegen codebase.
 
-import inspect
+Currently this API is under development; please do not depend on it.
+"""
 
-from absl.testing import absltest
-from fiddle._src.codegen.auto_config import get_history_comments
-from fiddle._src.codegen.auto_config import init_task
-from fiddle._src.codegen.auto_config import ir_to_cst
-from fiddle._src.codegen.auto_config import make_symbolic_references
-from fiddle._src.codegen.auto_config import shared_to_variables
-from fiddle._src.codegen.auto_config import test_fixtures
-
-
-class IrToCstTest(absltest.TestCase):
-
-  def test_basic_ir(self):
-    task = test_fixtures.simple_ir()
-    make_symbolic_references.import_symbols(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
-    code = ir_to_cst.code_for_task(task).code
-    expected = """
-    from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle.experimental import auto_config
-
-
-    @auto_config.auto_config
-    def simple_ir_fixture():
-        return test_fixtures.foo(x=4)
-    """
-    self.assertEqual(code.split(), expected.split(), msg=code)
-
-  def test_two_shared_config(self):
-    task = test_fixtures.unprocessed_two_shared_config()
-    make_symbolic_references.import_symbols(task)
-    shared_to_variables.move_shared_nodes_to_variables(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(
-        task, format_history=get_history_comments.format_history_for_buildable
-    )
-    code = ir_to_cst.code_for_task(task).code
-    (base_line,) = (
-        i
-        for i, line in enumerate(inspect.getsource(test_fixtures).splitlines())
-        if "def unprocessed_two_shared_config(" in line
-    )
-    line = base_line + 11  # Feel free to adjust if the test fixture is changed.
-    expected = f"""
-    from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle.experimental import auto_config
-
-
-    @auto_config.auto_config
-    def unprocessed_two_shared_fixture():
-      foo = test_fixtures.foo(
-        x=3,  # Set in .../auto_config/test_fixtures.py:{line}:unprocessed_two_shared_config
-        )
-      shared_type = test_fixtures.SharedType(
-        x=foo,  # Set in .../auto_config/test_fixtures.py:{line + 1}:unprocessed_two_shared_config
-        z=7.0,  # Set in .../auto_config/test_fixtures.py:{line + 1}:unprocessed_two_shared_config
-        )
-      return [shared_type, shared_type, foo]
-    """
-    self.assertEqual(code.split(), expected.split(), msg=code)
-
-  def test_complex_dict_node_generation(self):
-    # These kinds of dictionaries aren't really supported by other passes, so
-    # please don't actually put them in your configs.
-    #
-    # Also sets are not supported by daglish by default, so they are only
-    # generated for primitive values here thanks to py_val_to_cst_converter.
-    config = {7.2: ("hi", {3, 4})}
-    task = init_task.init_task(config)
-    code = ir_to_cst.code_for_task(task).code
-    expected = """
-    from fiddle.experimental import auto_config
-
-
-    @auto_config.auto_config
-    def config_fixture():
-        return {7.2: ('hi', {3, 4})}
-    """
-    self.assertEqual(code.split(), expected.split(), msg=code)
-
-  def test_tags_generation_config(self):
-    task = test_fixtures.simple_ir_with_tags()
-    make_symbolic_references.import_symbols(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
-    code = ir_to_cst.code_for_task(task).code
-    expected = """
-    from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle.experimental import auto_config
-
-
-    @auto_config.auto_config
-    def config_fixture():
-        return test_fixtures.bar(x=auto_config.with_tags(1,
-          test_fixtures.ATag),
-          y=auto_config.with_tags(2, test_fixtures.ATag, test_fixtures.BTag))
-    """
-    self.assertEqual(code.split(), expected.split(), msg=code)
-
-  def test_tags_generation_partial(self):
-    task = test_fixtures.simple_partial_ir_with_tags()
-    make_symbolic_references.import_symbols(task)
-    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
-    code = ir_to_cst.code_for_task(task).code
-    expected = """
-    from fiddle._src.codegen.auto_config import test_fixtures
-    from fiddle.experimental import auto_config
-    import functools
-
-
-    @auto_config.auto_config
-    def config_fixture():
-        return functools.partial(test_fixtures.bar,
-            x=auto_config.with_tags(1, test_fixtures.ATag),
-            y=auto_config.with_tags(2, test_fixtures.ATag, test_fixtures.BTag))
-    """
-    self.assertEqual(code.split(), expected.split(), msg=code)
+import dataclasses
+from typing import Any, Callable, Dict, Optional, Type
 
-
-if __name__ == "__main__":
-  absltest.main()
+import fiddle as fdl
+from fiddle._src.codegen import newcg_symbolic_references
+from fiddle._src.codegen.auto_config import code_ir
+from fiddle._src.codegen.auto_config import experimental_top_level_api
+from fiddle._src.codegen.auto_config import make_symbolic_references as old_symbolic_references
+from fiddle._src.experimental import auto_config
+
+
+@dataclasses.dataclass(frozen=True)
+class RemoveAutoConfigFn(experimental_top_level_api.CodegenPass):
+
+  def __call__(self, value: Any) -> Any:
+    assert isinstance(value, code_ir.CodegenTask)
+    value.auto_config_fn = None
+    return value
+
+
+@dataclasses.dataclass(frozen=True)
+class ImportSymbols(experimental_top_level_api.MutationCodegenPass):
+  """Preprocessing step to import symbols, for better naming."""
+
+  fn: Callable[..., Any] = newcg_symbolic_references.import_symbols
+
+
+@dataclasses.dataclass(frozen=True)
+class MakeSymbolicReferences(experimental_top_level_api.MutationCodegenPass):
+  """Converts Buildable sub-objects to IR nodes representing function calls.
+
+  In this case, we emit fdl.Config(), fdl.Partial(), and fdl.ArgFactory() calls,
+  instead of calls to the configured functions/classes.
+  """
+
+  fn: Callable[..., Any] = (
+      newcg_symbolic_references.replace_callables_and_configs_with_symbols
+  )
+  format_history: Callable[..., Any] = (
+      old_symbolic_references.noop_history_comments
+  )
+
+
+def _get_pass_idx(
+    codegen_config: fdl.Config[experimental_top_level_api.Codegen],
+    cls: Type[experimental_top_level_api.CodegenPass],
+) -> int:
+  for i, codegen_pass in enumerate(codegen_config.passes):
+    if issubclass(fdl.get_callable(codegen_pass), cls):
+      return i
+  raise ValueError(f"Could not find codegen pass {cls}")
+
+
+@auto_config.auto_unconfig
+def code_generator(
+    top_level_fixture_name: str = "config_fixture",
+    max_expression_complexity: Optional[int] = None,
+    include_history: bool = False,
+    debug_print: bool = False,
+) -> experimental_top_level_api.Codegen:
+  """Returns a low-level Codegen instance; see experimental_top_level_api."""
+  config = experimental_top_level_api.code_generator.as_buildable(
+      top_level_fixture_name=top_level_fixture_name,
+      max_expression_complexity=max_expression_complexity,
+      include_history=include_history,
+      debug_print=debug_print,
+  )
+
+  # Unset auto_config right after initialization.
+  config.passes.insert(1, fdl.Config(RemoveAutoConfigFn))
+
+  # Remove LowerArgFactories
+  idx = _get_pass_idx(config, experimental_top_level_api.LowerArgFactories)
+  config.passes.pop(idx)
+
+  # Replace ImportSymbols
+  idx = _get_pass_idx(config, experimental_top_level_api.ImportSymbols)
+  fdl.update_callable(config.passes[idx], ImportSymbols)
+
+  # Replace MakeSymbolicReferences
+  idx = _get_pass_idx(config, experimental_top_level_api.MakeSymbolicReferences)
+  fdl.update_callable(config.passes[idx], MakeSymbolicReferences)
+  return config
+
+
+def new_codegen(
+    config,
+    *,
+    top_level_fixture_name: str = "config_fixture",
+    sub_fixtures: Optional[Dict[str, Any]] = None,
+    max_expression_complexity: Optional[int] = None,
+    include_history: bool = False,
+    debug_print: bool = False,
+) -> str:
+  """Generates code for an auto_config fixture.
+
+  Args:
+    config: Configuration to generate auto_config code for.
+    top_level_fixture_name: Name of the top-level fixture. When its as_buildable
+      path is called, e.g. `config_fixture.as_buildable()`, this should return a
+      config equivalent to `config`.
+    sub_fixtures: Dictionary from function name to sub-configuration object,
+      declaring sub-functions to create. This helps manage complexity of huge
+      configurations.
+    max_expression_complexity: Breaks complex expressions into variables for
+      readability.
+    include_history: Whether history should be included. These currently appear
+      as trailing comments in the field of Buildable's.
+    debug_print: Whether to use the IR printer to print intermediate
+      representations as various passes run to generate code.
+
+  Returns:
+    Python module code.
+  """
+  codegen_obj: experimental_top_level_api.Codegen = code_generator(
+      top_level_fixture_name=top_level_fixture_name,
+      max_expression_complexity=max_expression_complexity,
+      include_history=include_history,
+      debug_print=debug_print,
+  )
+  return codegen_obj(config, sub_fixtures=sub_fixtures).code
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 """Changes callables to symbol references."""
 
 import enum
 import functools
 import inspect
+import typing
 from typing import Any, Callable
 
 from fiddle import arg_factory
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen.auto_config import code_ir
 
@@ -62,14 +63,24 @@
       task.import_manager.add(value)
 
 
 def noop_history_comments(unused_buildable):
   return code_ir.HistoryComments()
 
 
+def _name_to_attribute_expression(name: str) -> code_ir.AttributeExpression:
+  if "." not in name:
+    raise ValueError(f"Could not parse symbol import {name}")
+  base, *parts = name.split(".")
+  value = code_ir.ModuleReference(code_ir.Name(base))
+  for part in parts:
+    value = code_ir.AttributeExpression(value, part)
+  return typing.cast(code_ir.AttributeExpression, value)
+
+
 def replace_callables_and_configs_with_symbols(
     task: code_ir.CodegenTask,
     *,
     format_history: Callable[
         ..., code_ir.HistoryComments
     ] = noop_history_comments,
 ) -> None:
@@ -81,19 +92,19 @@
       get_history_comments.format_history_for_buildable (or a functools.partial
       variant) to populate histories.
   """
 
   fn_name = None
 
   def _handle_partial(
-      value: config_lib.Partial, state: daglish.State, symbol: str
+      value: config_lib.Partial,
+      state: daglish.State,
+      ir_for_symbol: code_ir.AttributeExpression,
   ):
     """Split-out helper method to handle Partial() nodes."""
-    symbol_ref = code_ir.SymbolReference(symbol)
-
     arguments = config_lib.ordered_arguments(value)
     all_tags = value.__argument_tags__
 
     # Arguments which were config_lib.ArgFactory arguments; these need to be
     # turned into regular calls.
     arg_factory_args = {}
 
@@ -116,49 +127,57 @@
           dict_of_args[arg] = code_ir.WithTagsCall(
               tag_symbol_expressions=tags_expr,
               item_to_tag=dict_of_args[arg],
           )
 
     def _arg_factory_partial():
       return code_ir.SymbolOrFixtureCall(
-          task.import_manager.add(arg_factory.partial),
-          positional_arg_expressions=[symbol_ref],
+          _name_to_attribute_expression(
+              task.import_manager.add(arg_factory.partial)
+          ),
+          positional_arg_expressions=[ir_for_symbol],
           arg_expressions=arg_factory_args,
           history_comments=format_history(value),
       )
 
     if not arg_factory_args:
       # The common case: there are no arg_factory's, so just emit a functools
       # partial. We currently emit a functools partial even if there are no
       # arguments, because this will mean there's a fdl.Partial when we call
       # the auto_config fixture's as_buildable() method. If we got rid of the
       # functools.partial, then we couldn't configure any attributes.
       return code_ir.SymbolOrFixtureCall(
-          task.import_manager.add(functools.partial),
-          positional_arg_expressions=[symbol_ref],
+          _name_to_attribute_expression(
+              task.import_manager.add(functools.partial)
+          ),
+          positional_arg_expressions=[ir_for_symbol],
           arg_expressions=regular_args,
           history_comments=format_history(value),
       )
     elif not regular_args:
       # There are only arg_factory args, so we can emit an arg_factory.partial.
       return _arg_factory_partial()
     else:
       # We have both functools.partial and arg_factory args. It doesn't matter
       # which order, but we need to emit both decorators. Go with functools
       # on the outer level.
       return code_ir.SymbolOrFixtureCall(
-          task.import_manager.add(functools.partial),
+          _name_to_attribute_expression(
+              task.import_manager.add(functools.partial)
+          ),
           positional_arg_expressions=[_arg_factory_partial()],
           arg_expressions=regular_args,
           history_comments=format_history(value),
       )
 
   def traverse(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
-      symbol = task.import_manager.add(config_lib.get_callable(value))
+      ir_for_symbol = _name_to_attribute_expression(
+          task.import_manager.add(config_lib.get_callable(value))
+      )
       if isinstance(value, config_lib.Config):
         all_tags = value.__argument_tags__
         value = state.map_children(value)
         for arg, arg_tags in all_tags.items():
           tag_expr = [task.import_manager.add(tag) for tag in arg_tags]
           if arg not in value.__arguments__:
             raise ValueError(
@@ -169,21 +188,21 @@
                 " config, for example using `fdl.clear_tags`."
             )
           value.__arguments__[arg] = code_ir.WithTagsCall(
               tag_symbol_expressions=tag_expr,
               item_to_tag=value.__arguments__[arg],
           )
         return code_ir.SymbolOrFixtureCall(
-            symbol_expression=symbol,
+            symbol_expression=ir_for_symbol,
             positional_arg_expressions=[],
             arg_expressions=config_lib.ordered_arguments(value),
             history_comments=format_history(value),
         )
       elif isinstance(value, config_lib.Partial):
-        return _handle_partial(value, state, symbol)
+        return _handle_partial(value, state, ir_for_symbol)
       elif isinstance(value, config_lib.ArgFactory):
         paths = " , ".join(
             daglish.path_str(path) for path in state.get_all_paths()
         )
         raise TypeError(
             "fdl.ArgFactory instances should be inside fdl.Partial's, and "
             "appropriately lowered with the split_arg_factories pass. Either "
@@ -191,15 +210,14 @@
             f"an error. Path to misformed object in codegen DAG: {paths}.\n\n("
             f"in function definition {fn_name}; `.output_value` "
             "indicates the value in the `return` statement.)"
         )
       else:
         raise TypeError(f"Unsupported Buildable {type(value)}")
     elif is_plain_symbol_or_enum_value(value):
-      symbol = task.import_manager.add(value)
-      return code_ir.SymbolReference(symbol)
+      return _name_to_attribute_expression(task.import_manager.add(value))
     else:
       return state.map_children(value)
 
   for fn in task.top_level_call.all_fixture_functions():
     fn_name = fn.name.value
     fn.replace_with(daglish.MemoizedTraversal.run(traverse, fn))
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/make_symbolic_references_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,18 @@
         code_ir.FixtureFunction(
             name=code_ir.Name(
                 value='simple_ir_fixture', is_generated=False, previous=None
             ),
             parameters=[],
             variables=[],
             output_value=code_ir.SymbolOrFixtureCall(
-                symbol_expression='test_fixtures.foo',
+                symbol_expression=code_ir.AttributeExpression(
+                    code_ir.ModuleReference(code_ir.Name('test_fixtures')),
+                    'foo',
+                ),
                 positional_arg_expressions=[],
                 arg_expressions={'x': 4},
                 history_comments=code_ir.HistoryComments(
                     per_field={
                         '__fn_or_cls__': (
                             f'Set in .../auto_config/test_fixtures.py:{line}'
                             ':simple_ir'
@@ -172,10 +175,26 @@
         initializer = functools.partial(test_fixtures.initializer,
             name='const', dtype='float32')
         return arg_factory.partial(test_fixtures.Attention,
             kernel_init=initializer)
     """
     self.assertEqual(code.split(), expected.split(), msg=code)
 
+  def test_bare_symbols(self):
+    task = test_fixtures.bare_symbol_reference_config()
+    make_symbolic_references.import_symbols(task)
+    make_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    code = ir_to_cst.code_for_task(task).code
+    expected = """
+    from fiddle._src.codegen.auto_config import test_fixtures
+    from fiddle.experimental import auto_config
+
+
+    @auto_config.auto_config
+    def config_fixture():
+        return test_fixtures.Attention
+    """
+    self.assertEqual(code.split(), expected.split(), msg=code)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/naming_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/naming_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/parents_first_traversal_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     # Object IDs of values to extract into variables.
     to_extract_ids = set()
 
     def find_to_extract(value, parent_results: Any) -> Any:
       """Processes a node in a function definition."""
       if isinstance(
           value,
-          (code_ir.VariableReference, code_ir.SymbolReference, code_ir.Name),
+          (code_ir.BaseNameReference, code_ir.Name),
       ):
         # Don't double-extract variables, and repeated symbol references are
         # fine.
         return
       elif len(parent_results) > 1:
         to_extract_ids.add(id(value))
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/shared_to_variables_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/shared_to_variables_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/split_arg_factories_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/split_arg_factories_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,15 +229,15 @@
           name=name, parameters=params, variables=[], output_value=value
       )
       new_fixtures.append(fixture_fn)
       args = {}
       for param in params:
         args[param.name.value] = code_ir.VariableReference(name=param.name)
       return code_ir.SymbolOrFixtureCall(
-          symbol_expression=name.value,
+          symbol_expression=code_ir.FixtureReference(name=name),
           positional_arg_expressions=[],
           arg_expressions=args,
       )
     else:
       return value
 
   value = task.top_level_call.fn.output_value
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/sub_fixture_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/sub_fixture_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/auto_config/test_fixtures.py` & `fiddle-0.2.8/fiddle/_src/codegen/auto_config/test_fixtures.py`

 * *Files 3% similar despite different names*

```diff
@@ -201,14 +201,23 @@
   shared = fdl.Config(SharedType, foo_call, 7.0)
   config = [shared, shared, foo_call]
   return init_task.init_task(
       config, top_level_fixture_name="unprocessed_two_shared_fixture"
   )
 
 
+def bare_symbol_reference_config() -> code_ir.CodegenTask:
+  """Returns a task for a config that is a bare symbol reference.
+
+  i.e. a symbol reference not wrapped in a fdl.Partial or the like.
+  """
+  config = Attention
+  return init_task.init_task(config)
+
+
 def parameters_for_testcases():
   """Returns parameters for absl's parameterized test cases."""
   return [
       {
           "testcase_name": "simple_ir",
           "task": simple_ir(),
       },
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/codegen_diff.py` & `fiddle-0.2.8/fiddle/_src/codegen/codegen_diff.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,30 +15,33 @@
 
 """Library for converting generating fiddlers from diffs."""
 
 import collections
 import functools
 import re
 import types
-from typing import Any, Callable, Dict, List, Set, Tuple
+from typing import Any, Callable, Dict, List, Optional, Set, Tuple
 
 from fiddle import daglish
 from fiddle import diffing
 from fiddle._src import config as config_lib
 from fiddle._src.codegen import import_manager as import_manager_lib
 from fiddle._src.codegen import namespace as namespace_lib
 from fiddle._src.codegen import py_val_to_cst_converter
 from fiddle._src.experimental import daglish_legacy
 import libcst as cst
 
 
-def fiddler_from_diff(diff: diffing.Diff,
-                      old: Any = None,
-                      func_name: str = 'fiddler',
-                      param_name: str = 'cfg'):
+def fiddler_from_diff(
+    diff: diffing.Diff,
+    old: Any = None,
+    func_name: str = 'fiddler',
+    param_name: str = 'cfg',
+    import_manager: Optional[import_manager_lib.ImportManager] = None,
+):
   """Returns the CST for a fiddler function that applies the changes in `diff`.
 
   The returned `cst.Module` consists of a set of `import` statements for any
   necessary imports, followed by a function definition for a function whose
   name is `func_name`, which takes a single parameter named `param_name`
   containing a `fdl.Config` (or other `Buildable` or structure), and mutates
   that `Config` in-place as described by `diff`.
@@ -62,26 +65,34 @@
       this is used when creating aliases for values in the input `Config` to
       determine which paths need to have aliases created.  (In particular, it is
       used to determine which paths are aliases for one another.)  If not
       specified, then pessimistically assume that aliases must be created for
       all referenced paths.
     func_name: The name for the fiddler function.
     param_name: The name for the parameter to the fiddler function.
+    import_manager: Existing import manager. Usually set to None, but if you are
+      integrating this with other code generation tasks, it can be nice to
+      share.
 
   Returns:
     An `cst.Module` object.  You can convert this to a string using
     `result.code`.
   """
-  # Create a namespace to keep track of variables that we add.  Reserve the
-  # names of the param & func.
-  namespace = namespace_lib.Namespace()
-  namespace.add(param_name)
-  namespace.add(func_name)
-
-  import_manager = import_manager_lib.ImportManager(namespace)
+  if import_manager is None:
+    # Create a namespace to keep track of variables that we add.  Reserve the
+    # names of the param & func.
+    namespace = namespace_lib.Namespace()
+    namespace.add(param_name)
+    namespace.add(func_name)
+
+    import_manager = import_manager_lib.ImportManager(namespace)
+  else:
+    namespace = import_manager.namespace
+    namespace.add(param_name)
+    namespace.add(func_name)
 
   # Get a list of paths that are referenced by the diff.
   used_paths = _find_used_paths(diff)
 
   # Add variables for any used paths where the value (or any of the value's
   # ancestors) will be replaced by a change in the diff.  If we don't have an
   # `old` structure, then we pessimistically assume that we need to create
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/formatting_utilities.py` & `fiddle-0.2.8/fiddle/_src/codegen/formatting_utilities.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/import_manager.py` & `fiddle-0.2.8/fiddle/_src/codegen/import_manager.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/import_manager_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/import_manager_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen.py` & `fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/legacy_codegen_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/legacy_codegen_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/mini_ast.py` & `fiddle-0.2.8/fiddle/_src/codegen/mini_ast.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/namespace.py` & `fiddle-0.2.8/fiddle/_src/codegen/namespace.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/namespace_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/namespace_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/new_codegen_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/new_codegen_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references.py` & `fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 # limitations under the License.
 
 """Changes callables to symbol references for non-auto_config codegen.
 
 N.B. Please see codegen/auto_config for the auto_config version!!
 """
 
+import typing
 from typing import Callable
 
 from fiddle import daglish
 from fiddle._src import config as config_lib
 from fiddle._src.codegen.auto_config import code_ir
 from fiddle._src.codegen.auto_config import make_symbolic_references as ac_make_symbolic_references
 
@@ -51,14 +52,24 @@
       for arg_tags in value.__argument_tags__.values():
         for tag in arg_tags:
           task.import_manager.add(tag)
     elif is_plain_symbol_or_enum_value(value):
       task.import_manager.add(value)
 
 
+def _name_to_attribute_expression(name: str) -> code_ir.AttributeExpression:
+  if "." not in name:
+    raise ValueError(f"Could not parse symbol import {name}")
+  base, *parts = name.split(".")
+  value = code_ir.ModuleReference(code_ir.Name(base))
+  for part in parts:
+    value = code_ir.AttributeExpression(value, part)
+  return typing.cast(code_ir.AttributeExpression, value)
+
+
 def replace_callables_and_configs_with_symbols(
     task: code_ir.CodegenTask,
     *,
     format_history: Callable[
         ..., code_ir.HistoryComments
     ] = noop_history_comments,
 ) -> None:
@@ -69,16 +80,20 @@
     format_history: Function used to format history for a buildable. Set to
       get_history_comments.format_history_for_buildable (or a functools.partial
       variant) to populate histories.
   """
 
   def traverse(value, state: daglish.State):
     if isinstance(value, config_lib.Buildable):
-      buildable_type = task.import_manager.add(type(value))
-      symbol = task.import_manager.add(config_lib.get_callable(value))
+      ir_for_buildable_type = _name_to_attribute_expression(
+          task.import_manager.add(type(value))
+      )
+      ir_for_symbol = _name_to_attribute_expression(
+          task.import_manager.add(config_lib.get_callable(value))
+      )
       all_tags = value.__argument_tags__
       value = state.map_children(value)
       for arg, arg_tags in all_tags.items():
         tag_expr = [task.import_manager.add(tag) for tag in arg_tags]
         if arg not in value.__arguments__:
           raise ValueError(
               f"Tagged field '{arg}' of {value!r} is not found in its"
@@ -88,20 +103,19 @@
               " config, for example using `fdl.clear_tags`."
           )
         value.__arguments__[arg] = code_ir.WithTagsCall(
             tag_symbol_expressions=tag_expr,
             item_to_tag=value.__arguments__[arg],
         )
       return code_ir.SymbolOrFixtureCall(
-          symbol_expression=buildable_type,
-          positional_arg_expressions=[code_ir.SymbolReference(symbol)],
+          symbol_expression=ir_for_buildable_type,
+          positional_arg_expressions=[ir_for_symbol],
           arg_expressions=config_lib.ordered_arguments(value),
           history_comments=format_history(value),
       )
     elif is_plain_symbol_or_enum_value(value):
-      symbol = task.import_manager.add(value)
-      return code_ir.SymbolReference(symbol)
+      return _name_to_attribute_expression(task.import_manager.add(value))
     else:
       return state.map_children(value)
 
   for fn in task.top_level_call.all_fixture_functions():
     fn.replace_with(daglish.MemoizedTraversal.run(traverse, fn))
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/newcg_symbolic_references_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/newcg_symbolic_references_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,23 @@
         code_ir.FixtureFunction(
             name=code_ir.Name(
                 value='simple_ir_fixture', is_generated=False, previous=None
             ),
             parameters=[],
             variables=[],
             output_value=code_ir.SymbolOrFixtureCall(
-                symbol_expression='fdl.Config',
+                symbol_expression=code_ir.AttributeExpression(
+                    code_ir.ModuleReference(code_ir.Name('fdl')),
+                    'Config',
+                ),
                 positional_arg_expressions=[
-                    code_ir.SymbolReference('test_fixtures.foo')
+                    code_ir.AttributeExpression(
+                        code_ir.ModuleReference(code_ir.Name('test_fixtures')),
+                        'foo',
+                    )
                 ],
                 arg_expressions={'x': 4},
                 history_comments=code_ir.HistoryComments(
                     per_field={
                         '__fn_or_cls__': (
                             f'Set in .../auto_config/test_fixtures.py:{line}'
                             ':simple_ir'
@@ -149,10 +155,25 @@
     def config_fixture():
         initializer = fdl.ArgFactory(test_fixtures.initializer,
             name='const', dtype='float32')
         return fdl.Partial(test_fixtures.Attention, kernel_init=initializer)
     """
     self.assertEqual(code.split(), expected.split(), msg=code)
 
+  def test_bare_symbols(self):
+    task = test_fixtures.bare_symbol_reference_config()
+    task.auto_config_fn = None
+    newcg_symbolic_references.import_symbols(task)
+    newcg_symbolic_references.replace_callables_and_configs_with_symbols(task)
+    code = ir_to_cst.code_for_task(task).code
+    expected = """
+    from fiddle._src.codegen.auto_config import test_fixtures
+
+
+    def config_fixture():
+        return test_fixtures.Attention
+    """
+    self.assertEqual(code.split(), expected.split(), msg=code)
+
 
 if __name__ == '__main__':
   absltest.main()
```

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/py_val_to_cst_converter_test.py` & `fiddle-0.2.8/fiddle/_src/codegen/py_val_to_cst_converter_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/special_value_codegen.py` & `fiddle-0.2.8/fiddle/_src/codegen/special_value_codegen.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/test_submodule/__init__.py` & `fiddle-0.2.8/fiddle/_src/codegen/test_submodule/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/test_submodule/test_util.py` & `fiddle-0.2.8/fiddle/_src/codegen/test_submodule/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/codegen/test_util.py` & `fiddle-0.2.8/fiddle/_src/codegen/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/config.py` & `fiddle-0.2.8/fiddle/_src/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,128 @@
 
 # Unique object instance that should never be used by end-users, and can thus
 # be used to differentiate between unset values and user-set values that are
 # None or other commonly-used sentinel.
 _UNSET_SENTINEL = object()
 
 
+_defaults_aware_traverser_registry = daglish.NodeTraverserRegistry(
+    use_fallback=True
+)
+
+
+def _buildable_flatten(
+    buildable: Buildable, include_defaults: bool = False
+) -> Tuple[Tuple[Any, ...], BuildableTraverserMetadata]:
+  """Implement Buildable.__flatten__ method."""
+  arguments = ordered_arguments(buildable, include_defaults=include_defaults)
+  keys = tuple(arguments.keys())
+  values = tuple(arguments.values())
+  argument_tags = {
+      name: frozenset(tags)
+      for name, tags in buildable.__argument_tags__.items()
+      if tags  # Don't include empty sets.
+  }
+  argument_history = {
+      name: tuple(entries)
+      for name, entries in buildable.__argument_history__.items()
+  }
+  metadata = BuildableTraverserMetadata(
+      fn_or_cls=buildable.__fn_or_cls__,
+      argument_names=keys,
+      argument_tags=argument_tags,
+      argument_history=argument_history,
+  )
+  return values, metadata
+
+
+def _buildable_path_elements(
+    buildable: Buildable, include_defaults: bool = False
+) -> Tuple[daglish.Attr]:
+  """Implement Buildable.__path_elements__ method."""
+  return tuple(
+      daglish.Attr(name)
+      for name in ordered_arguments(
+          buildable, include_defaults=include_defaults
+      ).keys()
+  )
+
+
+def _register_buildable_defaults_aware_traversers(cls: Type[Buildable]):
+  """Registers defaults aware traversal routines for buildable subclasses."""
+  _defaults_aware_traverser_registry.register_node_traverser(
+      cls,
+      flatten_fn=functools.partial(_buildable_flatten, include_defaults=True),
+      unflatten_fn=cls.__unflatten__,
+      path_elements_fn=functools.partial(
+          _buildable_path_elements, include_defaults=True
+      ),
+  )
+
+
+def _compare_buildable(x: Buildable, y: Buildable, check_dag: bool = False):
+  """Compare if two Buildables are equal, including DAG structure."""
+  assert isinstance(x, Buildable)
+  if type(x) is not type(y):
+    return False
+  if x.__fn_or_cls__ != y.__fn_or_cls__:
+    return False
+  assert x._has_var_keyword == y._has_var_keyword, (  # pylint: disable=protected-access
+      'Internal invariant violated: has_var_keyword should be the same if '
+      "__fn_or_cls__'s are the same."
+  )
+
+  missing = object()
+  for key in set(x.__arguments__) | set(y.__arguments__):
+    v1 = getattr(x, key, missing)
+    v2 = getattr(y, key, missing)
+    assert not (v1 is missing and v2 is missing)
+    if v1 is missing or v2 is missing:
+      return False
+    if isinstance(v1, Buildable) and isinstance(v2, Buildable):
+      if not _compare_buildable(v1, v2, check_dag=False):
+        return False
+    if v1 != v2:
+      return False
+
+  # Compare the DAG structure.
+  # The DAG stracture comparison must traverse the whole DAG and sort the
+  # result by path, which is expensive. Thus, we compare values first so
+  # that most unequal cases will not reach the expensive DAG compare step.
+  if check_dag:
+    x_elements = list(
+        daglish.iterate(
+            x,
+            memoized=True,
+            # Not to memorize internables during traversal, as they might
+            # be equal in value but have different object ids.
+            memoize_internables=False,
+            registry=_defaults_aware_traverser_registry,
+        )
+    )
+    y_elements = list(
+        daglish.iterate(
+            y,
+            memoized=True,
+            memoize_internables=False,
+            registry=_defaults_aware_traverser_registry,
+        )
+    )
+    x_paths = sorted([elt[1] for elt in x_elements])
+    y_paths = sorted([elt[1] for elt in y_elements])
+
+    if len(x_paths) != len(y_paths):
+      return False
+    for x_path, y_path in zip(x_paths, y_paths):
+      if x_path != y_path:
+        return False
+
+  return True
+
+
 class BuildableTraverserMetadata(NamedTuple):
   """Metadata for a Buildable.
 
   This separate class is used for DAG traversals.
   """
 
   fn_or_cls: Callable[..., Any]
@@ -188,63 +302,42 @@
   def __init_subclass__(cls):
     daglish.register_node_traverser(
         cls,
         flatten_fn=lambda x: x.__flatten__(),
         unflatten_fn=cls.__unflatten__,
         path_elements_fn=lambda x: x.__path_elements__(),
     )
+    _register_buildable_defaults_aware_traversers(cls)
 
   @abc.abstractmethod
   def __build__(self, *args, **kwargs):
     """Builds output for this instance; see subclasses for details."""
     raise NotImplementedError()
 
   def __flatten__(self) -> Tuple[Tuple[Any, ...], BuildableTraverserMetadata]:
-    arguments = ordered_arguments(self)
-    keys = tuple(arguments.keys())
-    values = tuple(arguments.values())
-    argument_tags = {
-        name: frozenset(tags)
-        for name, tags in self.__argument_tags__.items()
-        if tags  # Don't include empty sets.
-    }
-    argument_history = {
-        name: tuple(entries)
-        for name, entries in self.__argument_history__.items()
-    }
-    metadata = BuildableTraverserMetadata(
-        fn_or_cls=self.__fn_or_cls__,
-        argument_names=keys,
-        argument_tags=argument_tags,
-        argument_history=argument_history,
-    )
-    return values, metadata
+    return _buildable_flatten(self, include_defaults=False)
 
   @classmethod
   def __unflatten__(
       cls, values: Iterable[Any], metadata: BuildableTraverserMetadata
   ):
     rebuilt = cls.__new__(cls)
     rebuilt.__init_callable__(metadata.fn_or_cls)
     object.__setattr__(rebuilt, '__argument_tags__', metadata.tags())
     object.__setattr__(rebuilt, '__argument_history__', metadata.history())
     object.__setattr__(rebuilt, '__arguments__', metadata.arguments(values))
     return rebuilt
 
-  def __path_elements__(self):
-    return tuple(daglish.Attr(name) for name in ordered_arguments(self).keys())
+  def __path_elements__(self) -> Tuple[daglish.Attr]:
+    return _buildable_path_elements(self, include_defaults=False)
 
   def __getattr__(self, name: str):
     """Get parameter with given ``name``."""
     value = self.__arguments__.get(name, _UNSET_SENTINEL)
 
-    # Replace tied values with their contents.
-    if isinstance(value, TiedValue):
-      value = value.value
-
     if value is not _UNSET_SENTINEL:
       return value
     if dataclasses.is_dataclass(
         self.__fn_or_cls__
     ) and _field_uses_default_factory(self.__fn_or_cls__, name):
       raise ValueError(
           "Can't get default value for dataclass field "
@@ -309,28 +402,19 @@
       tags = value.__argument_tags__.get('value', ())
       if tags:
         self.__argument_tags__[name].update(tags)
         self.__argument_history__.add_updated_tags(
             name, self.__argument_tags__[name]
         )
       if 'value' in value.__arguments__:
-        # Must pull from underlying dictionary to preserve TiedValue's.
         value = value.__arguments__['value']
       else:
         return
 
-    # Actually set the value, handling TiedValue's as a special case.
-    current = self.__arguments__.get(name)
-    if isinstance(current, TiedValue) and not isinstance(value, TiedValue):
-      # This will create a history entry in the TiedValue as well. (Seems
-      # reasonable, but not clear what's best?)
-      current.value = value
-    else:
-      self.__arguments__[name] = value
-
+    self.__arguments__[name] = value
     self.__argument_history__.add_new_value(name, value)
 
   def __delattr__(self, name):
     """Unsets parameter ``name``."""
     try:
       del self.__arguments__[name]
       self.__argument_history__.add_deleted_value(name)
@@ -442,30 +526,15 @@
 
     Args:
       other: The other value to compare ``self`` to.
 
     Returns:
       ``True`` if ``self`` equals ``other``, ``False`` if not.
     """
-    if type(self) is not type(other):
-      return False
-    if self.__fn_or_cls__ != other.__fn_or_cls__:
-      return False
-    assert self._has_var_keyword == other._has_var_keyword, (
-        'Internal invariant violated: has_var_keyword should be the same if '
-        "__fn_or_cls__'s are the same."
-    )
-
-    missing = object()
-    for key in set(self.__arguments__) | set(other.__arguments__):
-      v1 = getattr(self, key, missing)
-      v2 = getattr(other, key, missing)
-      if (v1 is not missing or v2 is not missing) and v1 != v2:
-        return False
-    return True
+    return _compare_buildable(self, other, check_dag=True)
 
   def __getstate__(self):
     """Gets pickle serialization state, removing some fields.
 
     For now, we discard the ``__signature__`` (which can be recalculated) and
     ``__argument_history__``, because these tend to contain values which cannot
     be serialized.
@@ -782,30 +851,14 @@
       raise RuntimeError(
           'Unexpected __fn_or_cls__ in TaggedValueCls; found:'
           f'{self.__fn_or_cls__}'
       )
     return self.__fn_or_cls__(tags=self.tags, *args, **kwargs)
 
 
-class TiedValue(Generic[T], Config[T]):
-  """Class implementing tied values.
-
-  The implementation/declaration is here, so that we can write __getattr__ and
-  __setattr__ buildable hooks to eliminate the extra ``.value`` when it is a
-  field attribute, but please use ``experimental/tied_value.py`` for the public
-  API.
-  """
-
-  # NOTE(b/201159339): We currently need to repeat these annotations for pytype.
-  __fn_or_cls__: TypeOrCallableProducingT[T]
-  __signature__: inspect.Signature
-
-  value: T
-
-
 @dataclasses.dataclass(frozen=True)
 class _BuiltArgFactory:
   """The result of building an ``ArgFactory``.
 
   This wrapper is returned by ``ArgFactory.__build__``, and then consumed by the
   ``__build__`` method of the containing ``Partial`` or ``ArgFactory`` object.
   """
```

### Comparing `fiddle-0.2.7/fiddle/_src/config_test.py` & `fiddle-0.2.8/fiddle/_src/config_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 import copy
 import dataclasses
 import functools
 import pickle
 import threading
 from typing import Any, Callable, Dict, Generic, TypeVar
-
 from absl.testing import absltest
 from absl.testing import parameterized
 import fiddle as fdl
 from fiddle import arg_factory
 from fiddle import daglish
 from fiddle import history
 from fiddle._src import config as config_lib
 from fiddle._src.experimental import daglish_legacy
+from fiddle._src.testing.example import demo_configs
 import pytype_extensions
 from typing_extensions import Annotated
 
 
 class Tag1(fdl.Tag):
   """One tag."""
 
@@ -513,14 +513,40 @@
 
     cfg = fdl.Config(fn_with_non_comparable_default)
     cfg.value1 = ClassWithDisabledEquality()
     value1, value2 = fdl.build(cfg)
     self.assertIsInstance(value1, ClassWithDisabledEquality)
     self.assertIsInstance(value2, ClassWithDisabledEquality)
 
+  def test_config_dag_structure_comparison(self):
+    a = fdl.Config(SampleClass, 1, 2)
+    b = fdl.Config(SampleClass, 1, 2)
+    with self.subTest('python_list'):
+      x = [a, a]
+      y = [a, b]
+      self.assertEqual(x, y)
+
+    with self.subTest('node_sharing_detection'):
+      x = fdl.Config(SampleClass, a, b)
+      y = fdl.Config(SampleClass, a, a)
+      self.assertNotEqual(x, y)
+
+    with self.subTest('node_sharing_difference'):
+      x = fdl.Config(SampleClass, a, b, b)
+      y = fdl.Config(SampleClass, a, a, b)
+      self.assertNotEqual(x, y)
+
+  def test_config_internables_comparison(self):
+    x, y = demo_configs.get_equal_but_not_object_identical_string_configs()
+    self.assertEqual(x, y)
+
+  def test_dict_with_different_order_comparison(self):
+    x, y = demo_configs.get_equal_but_not_object_identical_string_configs()
+    self.assertEqual(x, y)
+
   def test_unsetting_argument(self):
     fn_config = fdl.Config(basic_fn)
     fn_config.arg1 = 3
     fn_config.arg2 = 4
 
     del fn_config.arg1
```

### Comparing `fiddle-0.2.7/fiddle/_src/daglish.py` & `fiddle-0.2.8/fiddle/_src/daglish.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,53 +33,80 @@
     """Generates code for accessing this path."""
     raise NotImplementedError()
 
   @abc.abstractmethod
   def follow(self, container) -> Any:
     """Returns the element of `container` specified by this path element."""
 
+  def __lt__(self, other: PathElement) -> bool:
+    """Define the less than relation for PathElement."""
+    if type(self) is not type(other):
+      return str(type(self)) < str(type(other))
+    else:
+      raise NotImplementedError(
+          "__lt__ relation should be handled by subclasses of PathElement."
+      )
+
 
 @dataclasses.dataclass(frozen=True)
 class Index(PathElement):
   """An index into a sequence (list or tuple)."""
   index: int
 
   @property
   def code(self) -> str:
     return f"[{self.index}]"
 
   def follow(self, container: Union[List[Any], Tuple[Any, ...]]) -> Any:
     return container[self.index]
 
+  def __lt__(self, other: PathElement) -> bool:
+    if type(self) is type(other):
+      return self.index < other.index
+    else:
+      return super().__lt__(other)
+
 
 @dataclasses.dataclass(frozen=True)
 class Key(PathElement):
   """A key of a mapping (e.g., dict)."""
   key: Any
 
   @property
   def code(self) -> str:
     return f"[{self.key!r}]"
 
   def follow(self, container: Dict[Any, Any]) -> Any:
     return container[self.key]
 
+  def __lt__(self, other: PathElement) -> bool:
+    if type(self) is type(other):
+      return self.key < other.key
+    else:
+      return super().__lt__(other)
+
 
 @dataclasses.dataclass(frozen=True)
 class Attr(PathElement):
   """An attribute of an object."""
   name: str
 
   @property
   def code(self) -> str:
     return f".{self.name}"
 
   def follow(self, container: Any) -> Any:
     return getattr(container, self.name)
 
+  def __lt__(self, other: PathElement) -> bool:
+    if type(self) is type(other):
+      return self.name < other.name
+    else:
+      return super().__lt__(other)
+
 
 class BuildableAttr(Attr):
   """An attribute of a Buildable."""
 
 
 @dataclasses.dataclass(frozen=True)
 class BuildableFnOrCls(Attr):
@@ -723,14 +750,15 @@
   traverse(structure, traversal.initial_state())
   return paths_by_id
 
 
 def iterate(
     value: Any,
     memoized: bool = True,
+    memoize_internables: bool = True,
     registry: NodeTraverserRegistry = _default_traverser_registry,
 ) -> Iterable[Tuple[Any, Path]]:
   """Iterates through values in a DAG.
 
   This API is suitable for read-only access and small/reasonable edits to a
   configuration DAG. If a transformation seeks to change the type of nodes, then
   we recommend using the functional traversal API.
@@ -739,23 +767,32 @@
   API is not discouraged for modifying configuration.
 
   Args:
     value: fdl.Buildable or collection of buildables.
     memoized: Whether to yield shared nodes only once. Defaults to True. With
       this setting, you will only see one path (which is somewhat arbitrary) to
       shared nodes.
+    memoize_internables: Whether to memoize Python internable values. Check the
+      docstring of MemoizedTraversal for details.
     registry: Override to the NodeTraverserRegistry; this is a low-level setting
       for traversing into custom data types.
 
   Returns:
     Iterable of (value, path) tuples.
   """
 
   def _traverse(node, state: State):
     yield node, state.current_path
     if state.is_traversable(node):
       for sub_result in state.flattened_map_children(node).values:
         yield from sub_result
 
-  traversal_cls = MemoizedTraversal if memoized else BasicTraversal
-  traversal: Traversal = traversal_cls(_traverse, value, registry=registry)
+  if memoized:
+    traversal = MemoizedTraversal(
+        _traverse,
+        value,
+        registry=registry,
+        memoize_internables=memoize_internables,
+    )
+  else:
+    traversal = BasicTraversal(_traverse, value, registry=registry)
   return _traverse(value, traversal.initial_state())
```

### Comparing `fiddle-0.2.7/fiddle/_src/daglish_extensions.py` & `fiddle-0.2.8/fiddle/_src/daglish_extensions.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/daglish_extensions_test.py` & `fiddle-0.2.8/fiddle/_src/daglish_extensions_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/daglish_test.py` & `fiddle-0.2.8/fiddle/_src/daglish_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,14 +196,21 @@
 
     bad_path_3 = (daglish.Index(1), daglish.Key("a"), daglish.Attr("bam"))
     with self.assertRaisesRegex(
         ValueError, r"Attr\(name='bam'\) is not compatible "
         r"with root\[1\]\['a'\]=.*"):
       daglish.follow_path(root, bad_path_3)
 
+  def test_path_elements_order(self):
+    a = daglish.Attr("bar")
+    b = daglish.Index(1)
+    c = daglish.Key("a")
+    self.assertLess(a, b)
+    self.assertLess(b, c)
+
 
 class TraverserRegistryTest(parameterized.TestCase):
 
   @parameterized.named_parameters([
       ("config", fdl.Config(Foo, bar=1, baz=2)),
       ("tagged_value", SampleTag.new()),
       ("namedtuple", SampleNamedTuple("a", "b")),
```

### Comparing `fiddle-0.2.7/fiddle/_src/diffing.py` & `fiddle-0.2.8/fiddle/_src/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/diffing_test.py` & `fiddle-0.2.8/fiddle/_src/diffing_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/__init__.py` & `fiddle-0.2.8/fiddle/_src/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/auto_config.py` & `fiddle-0.2.8/fiddle/_src/experimental/auto_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -573,19 +573,18 @@
     config if called inside an auto_config function.
   """
   return AutoConfig(
       func=fn_or_cls, buildable_func=fn_or_cls, always_inline=True
   )
 
 
-# TODO(b/286559744): Change allow_dataclass_attribute_access default as False.
 def auto_config(
     fn=None,
     *,
-    experimental_allow_dataclass_attribute_access=True,
+    experimental_allow_dataclass_attribute_access=False,
     experimental_allow_control_flow: bool = False,
     experimental_always_inline: Optional[bool] = None,
     experimental_exemption_policy: Optional[auto_config_policy.Policy] = None,
     experimental_config_cls=config.Config,
     experimental_result_must_contain_buildable: bool = True,
 ) -> Any:  # TODO(b/272377821): More precise return type.
   """Rewrites the given function to make it generate a ``Config``.
```

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/auto_config_policy.py` & `fiddle-0.2.8/fiddle/_src/experimental/auto_config_policy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/auto_config_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/auto_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/__init__.py` & `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders.py` & `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py` & `fiddle-0.2.8/fiddle/_src/experimental/autobuilders/autobuilders_test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/configurator.py` & `fiddle-0.2.8/fiddle/_src/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy.py` & `fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/daglish_legacy_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/daglish_legacy_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/dataclasses.py` & `fiddle-0.2.8/fiddle/_src/experimental/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/dataclasses_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/dataclasses_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/dict_config.py` & `fiddle-0.2.8/fiddle/_src/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/dict_config_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/dict_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/namespace_config.py` & `fiddle-0.2.8/fiddle/_src/experimental/namespace_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/namespace_config_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/namespace_config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/serialization.py` & `fiddle-0.2.8/fiddle/_src/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/transform.py` & `fiddle-0.2.8/fiddle/_src/experimental/transform.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/transform_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/transform_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/visualize.py` & `fiddle-0.2.8/fiddle/_src/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/with_tags.py` & `fiddle-0.2.8/fiddle/_src/experimental/with_tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/with_tags_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/with_tags_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization.py` & `fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization.py`

 * *Files 21% similar despite different names*

```diff
@@ -23,65 +23,65 @@
 
 import collections
 import inspect
 from typing import Any
 
 from fiddle._src import config as config_lib
 from fiddle._src import tagging
-from fiddle._src.experimental import fixture_node
 import yaml
 
 
 def _defaultdict_representer(dumper, data):
   return dumper.represent_dict(data)
 
 
-yaml.SafeDumper.add_representer(collections.defaultdict,
-                                _defaultdict_representer)
+yaml.SafeDumper.add_representer(
+    collections.defaultdict, _defaultdict_representer
+)
 
 
 def _config_representer(dumper, data, type_name="fdl.Config"):
   """Returns a YAML representation of `data`."""
   value = dict(data.__arguments__)
 
   # We put __fn_or_cls__ into __arguments__, so "__fn_or_cls__" must be a new
   # key that doesn't exist in __arguments__. It would be pretty rare for this
   # to be an issue.
   if "__fn_or_cls__" in value:
-    raise ValueError("It is not supported to dump objects of functions/classes "
-                     "that have a __fn_or_cls__ parameter.")
+    raise ValueError(
+        "It is not supported to dump objects of functions/classes "
+        "that have a __fn_or_cls__ parameter."
+    )
 
   value["__fn_or_cls__"] = {
       "module": inspect.getmodule(config_lib.get_callable(data)).__name__,
       "name": config_lib.get_callable(data).__qualname__,
   }
   return dumper.represent_mapping(f"!{type_name}", value)
 
 
 def _partial_representer(dumper, data):
   return _config_representer(dumper, data, type_name="fdl.Partial")
 
 
-def _fixture_representer(dumper, data):
-  return _config_representer(
-      dumper, data, type_name="fiddle.experimental.Fixture")
-
-
 def _taggedvalue_representer(dumper, data):
-  return dumper.represent_mapping("!fdl.TaggedValue", {
-      "tags": [tag.name for tag in data.tags],
-      "value": data.value,
-  })
+  return dumper.represent_mapping(
+      "!fdl.TaggedValue",
+      {
+          "tags": [tag.name for tag in data.tags],
+          "value": data.value,
+      },
+  )
 
 
 yaml.SafeDumper.add_representer(config_lib.Config, _config_representer)
 yaml.SafeDumper.add_representer(config_lib.Partial, _partial_representer)
-yaml.SafeDumper.add_representer(fixture_node.FixtureNode, _fixture_representer)
-yaml.SafeDumper.add_representer(tagging.TaggedValueCls,
-                                _taggedvalue_representer)
+yaml.SafeDumper.add_representer(
+    tagging.TaggedValueCls, _taggedvalue_representer
+)
 
 
 def dump_yaml(value: Any) -> str:
   """Returns the YAML serialization of `value`.
 
   Args:
     value: The value to serialize.
```

### Comparing `fiddle-0.2.7/fiddle/_src/experimental/yaml_serialization_test.py` & `fiddle-0.2.8/fiddle/_src/experimental/yaml_serialization_test.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 """Tests for yaml_serialization."""
 import dataclasses
 import pathlib
 from typing import Any
 
 from absl.testing import absltest
 import fiddle as fdl
-from fiddle._src.experimental import fixture_node
 from fiddle._src.experimental import serialization
 from fiddle._src.experimental import yaml_serialization
 from fiddle._src.testing import test_util
 import yaml
 
 
 def _testdata_dir():
@@ -45,18 +44,14 @@
   return fdl.Config(fn_or_cls, **arguments)
 
 
 def _partial_constructor(loader, node):
   return fdl.cast(fdl.Partial, _config_constructor(loader, node))
 
 
-def _fixture_constructor(loader, node):
-  return fdl.cast(fixture_node.FixtureNode, _config_constructor(loader, node))
-
-
 class SemiSafeLoader(yaml.SafeLoader):
   """Intermediate class that can load Fiddle configs."""
 
 
 def load_yaml_test_only(serialized: str) -> Any:
   """Test-only method that returns a Fiddle configuration from YAML.
 
@@ -69,30 +64,24 @@
     serialized: Serialized configuration.
 
   Returns:
     Loaded object.
   """
   SemiSafeLoader.add_constructor("!fdl.Config", _config_constructor)
   SemiSafeLoader.add_constructor("!fdl.Partial", _partial_constructor)
-  SemiSafeLoader.add_constructor("!fiddle.experimental.Fixture",
-                                 _fixture_constructor)
   return yaml.load(serialized, Loader=SemiSafeLoader)
 
 
 @dataclasses.dataclass
 class Foo:
   a: int
   b: str
   c: Any
 
 
-def my_fixture(template):
-  return template
-
-
 class FakeTag(fdl.Tag):
   """Fake/test tag class."""
 
 
 def _normalize_expected_config(config_str: str):
   return config_str.replace("fiddle._src.experimental.yaml_serialization_test",
                             "__main__")
@@ -126,22 +115,14 @@
   def test_dump_yaml_partial(self):
     config = fdl.Partial(
         Foo, a=1, b="hi", c=fdl.Config(Foo, a=2, b="bye", c=None))
     serialized = yaml_serialization.dump_yaml(value=config)
     loaded = load_yaml_test_only(serialized)
     self.assertEqual(loaded, config)
 
-  def test_dump_fixture(self):
-    config = fixture_node.FixtureNode(my_fixture,
-                                      fdl.Config(Foo, a=1, b="hi", c=None))
-    serialized = yaml_serialization.dump_yaml(value=config)
-    loaded = load_yaml_test_only(serialized)
-    self.assertIsInstance(loaded, fixture_node.FixtureNode)
-    self.assertEqual(loaded, config)
-
   def test_dump_tagged_value(self):
     self.assertRegex(
         yaml_serialization.dump_yaml(value=FakeTag.new(2)).strip(),
         r"""!fdl\.TaggedValue
 tags:
 - [\w\d_\.]+\.FakeTag
 value: 2""")
```

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/__init__.py` & `fiddle-0.2.8/fiddle/_src/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/flax_test.py` & `fiddle-0.2.8/fiddle/_src/extensions/flax_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/jax.py` & `fiddle-0.2.8/fiddle/_src/extensions/jax.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/seqio.py` & `fiddle-0.2.8/fiddle/_src/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/seqio_test.py` & `fiddle-0.2.8/fiddle/_src/extensions/seqio_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/tf.py` & `fiddle-0.2.8/fiddle/_src/extensions/tf.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/extensions/tf_test.py` & `fiddle-0.2.8/fiddle/_src/extensions/tf_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/field_metadata.py` & `fiddle-0.2.8/fiddle/_src/field_metadata.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/graphviz.py` & `fiddle-0.2.8/fiddle/_src/graphviz.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/graphviz_custom_object.py` & `fiddle-0.2.8/fiddle/_src/graphviz_custom_object.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/history.py` & `fiddle-0.2.8/fiddle/_src/history.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/history_test.py` & `fiddle-0.2.8/fiddle/_src/history_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/materialize.py` & `fiddle-0.2.8/fiddle/_src/materialize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/materialize_test.py` & `fiddle-0.2.8/fiddle/_src/materialize_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/module_reflection.py` & `fiddle-0.2.8/fiddle/_src/module_reflection.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """A collection of Fiddle-internal tools to reflect over modules."""
 
 import inspect
 import logging
+import typing
 from typing import Any, List
+from fiddle._src import config as config_lib
 
 
 def find_fiddler_like_things(source_module: Any) -> List[str]:
   """Returns a list of names that look like fiddlers.
 
   A fiddler is a 1-ary function that mutates a config (and returns None).
 
@@ -70,17 +72,25 @@
     A list of attributes on `source_module` that appear to be base
     config-producing functions.
   """
   available_base_names = []
   for name in dir(source_module):
     if name.startswith('__'):
       continue
+    if name in dir(typing):
+      continue
     try:
       sig = inspect.signature(getattr(source_module, name))
 
+      # Exclude functions that do not return a single config.
+      return_type = sig.return_annotation
+      origin = typing.get_origin(return_type)
+      if origin is not None and not issubclass(origin, config_lib.Buildable):
+        continue
+
       def is_required_arg(name: str) -> bool:
         param = sig.parameters[name]  # pylint: disable=cell-var-from-loop
         return ((param.kind == param.POSITIONAL_ONLY or
                  param.kind == param.POSITIONAL_OR_KEYWORD) and
                 param.default is param.empty)
 
       if not any(filter(is_required_arg, sig.parameters)):
```

### Comparing `fiddle-0.2.7/fiddle/_src/module_reflection_test.py` & `fiddle-0.2.8/fiddle/_src/module_reflection_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/module_reflection_test_module.py` & `fiddle-0.2.8/fiddle/_src/module_reflection_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/mutate_buildable.py` & `fiddle-0.2.8/fiddle/_src/mutate_buildable.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/mutate_buildable_test.py` & `fiddle-0.2.8/fiddle/_src/mutate_buildable_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/printing.py` & `fiddle-0.2.8/fiddle/_src/printing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/printing_test.py` & `fiddle-0.2.8/fiddle/_src/printing_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/reraised_exception.py` & `fiddle-0.2.8/fiddle/_src/reraised_exception.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/reraised_exception_test.py` & `fiddle-0.2.8/fiddle/_src/reraised_exception_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/selectors.py` & `fiddle-0.2.8/fiddle/_src/selectors.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,22 @@
 of base configuration, and these APIs allow such overrides to take place
 imperatively.
 """
 
 import abc
 import copy
 import dataclasses
+import logging
 from typing import Any, Callable, Iterator, Optional, Type, Union
 
 from fiddle._src import config as config_lib
 from fiddle._src import daglish
 from fiddle._src import mutate_buildable
 from fiddle._src import tag_type
+from fiddle._src import tagging
 
 
 # Maybe DRY up with type declaration in autobuilders.py?
 FnOrClass = Union[Callable[..., Any], Type[Any]]
 
 
 class Selection(metaclass=abc.ABCMeta):
@@ -132,14 +134,22 @@
     Nodes that are reachable via multiple paths are yielded only once.
     """
 
     for value in _memoized_walk_leaves_first(self.cfg):
       if self._matches(value):
         yield value
 
+  def __str__(self) -> str:
+    return (
+        f"NodeSelection(cfg, fn_or_cls={self.fn_or_cls},"
+        f" match_subclasses={self.match_subclasses})"
+    )
+
+  __repr__ = __str__
+
   def replace(self, value: Any, deepcopy: bool = True) -> None:
     if self._matches(self.cfg):
       raise ValueError(
           "NodeSelection.replace() is not supported on selections that "
           "match the root Buildable, because select() is primarily a "
           "mutation-based API that does not return new/replacement configs.")
 
@@ -194,15 +204,15 @@
   def __iter__(self) -> Iterator[Any]:
     """Yields all values for the selected tag."""
 
     for value in _memoized_walk_leaves_first(self.cfg):
       if isinstance(value, config_lib.Buildable):
         for name, tags in value.__argument_tags__.items():
           if any(issubclass(tag, self.tag) for tag in tags):
-            yield getattr(value, name)
+            yield getattr(value, name, tagging.NO_VALUE)
 
   def replace(self, value: Any, deepcopy: bool = True) -> None:
 
     for node_value in _memoized_walk_leaves_first(self.cfg):
       if isinstance(node_value, config_lib.Buildable):
         for name, tags in node_value.__argument_tags__.items():
           if any(issubclass(tag, self.tag) for tag in tags):
@@ -215,22 +225,30 @@
         "of get().")
 
   def set(self, **kwargs) -> None:
     raise NotImplementedError(
         "You can't set named attributes on tagged values, you can only replace "
         "them. Please call replace() instead of set().")
 
+_missing = object()
+
+
+def _is_empty(selection: Selection) -> bool:
+  """Returns whether a selection is empty."""
+  return next(iter(selection), _missing) is _missing
+
 
 def select(
     cfg: config_lib.Buildable,
     fn_or_cls: Optional[FnOrClass] = None,
     *,
     tag: Optional[tag_type.TagType] = None,
     match_subclasses: bool = True,
     buildable_type: Type[config_lib.Buildable] = config_lib.Buildable,
+    check_nonempty: Optional[bool] = None,
 ) -> Selection:
   """Selects sub-buildables or fields within a configuration DAG.
 
   Example configuring attention classes::
 
     select(my_config, MyDenseAttention).set(num_heads=12, head_dim=512)
 
@@ -243,26 +261,43 @@
     fn_or_cls: Select by a given function or class that is being configured.
     tag: If set, selects all attributes tagged by `tag`. This will return a
       TagSelection instead of a Selection, which has a slightly different API.
     match_subclasses: If fn_or_cls is provided and a class, then also match
       subclasses of `fn_or_cls`.
     buildable_type: Restrict the selection to a particular buildable type. Not
       valid for tag selections.
+    check_nonempty: Whether to raise an error on empty selections. This will be
+      true in the future.
 
   Returns:
     A Selection, which is a TagSelection if `tag` is set, and a NodeSelection
     otherwise.
   """
   if tag is not None:
     if fn_or_cls is not None:
       raise NotImplementedError(
           "Selecting by tag and fn_or_cls is not supported yet.")
     if not match_subclasses:
       raise NotImplementedError(
           "match_subclasses is ignored when selecting by tag.")
-    return TagSelection(cfg, tag)
+    selection = TagSelection(cfg, tag)
   else:
-    return NodeSelection(
+    if fn_or_cls is None:
+      raise ValueError("Either tag or fn_or_cls must be provided.")
+    selection = NodeSelection(
         cfg,
         fn_or_cls,
         match_subclasses=match_subclasses,
-        buildable_type=buildable_type)
+        buildable_type=buildable_type,
+    )
+
+  if check_nonempty and _is_empty(selection):
+    raise ValueError(
+        f"Selection {selection} is empty! If this is OK, please call"
+        " select(..., check_nonempty=False)"
+    )
+  elif check_nonempty is None and _is_empty(selection):
+    logging.warning(
+        "Your selection was empty. In the future, this will be "
+        "an error. Please set check_nonempty=False if this is intended."
+    )
+  return selection
```

### Comparing `fiddle-0.2.7/fiddle/_src/selectors_test.py` & `fiddle-0.2.8/fiddle/_src/selectors_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -170,25 +170,14 @@
       selectors.select(cfg, fn_or_cls=Attention, tag=ActivationDType)
     with self.assertRaises(NotImplementedError):
       selectors.select(cfg, tag=ActivationDType, match_subclasses=False)
 
 
 class NodeSelectionTest(absltest.TestCase):
 
-  def test_matches_everything(self):
-    cfg = encoder_decoder_config()
-    sel = typing.cast(selectors.NodeSelection, selectors.select(cfg))
-    self.assertTrue(sel._matches(cfg.encoder))
-    self.assertTrue(sel._matches(cfg.encoder.attention))
-    self.assertTrue(sel._matches(cfg.encoder.mlp))
-    self.assertTrue(sel._matches(cfg.decoder))
-    self.assertTrue(sel._matches(cfg.decoder.self_attention))
-    self.assertTrue(sel._matches(cfg.decoder.encoder_decoder_attention))
-    self.assertTrue(sel._matches(cfg.decoder.mlp))
-
   def test_matches_based_on_type(self):
     cfg = encoder_decoder_config()
     sel = typing.cast(selectors.NodeSelection, selectors.select(cfg, Attention))
     self.assertFalse(sel._matches(cfg.encoder))
     self.assertTrue(sel._matches(cfg.encoder.attention))
     self.assertFalse(sel._matches(cfg.encoder.mlp))
 
@@ -290,14 +279,19 @@
     selectors.select(cfg, Attention).set(
         dtype="override_dtype", kernel_init="override_init")
     self.assertEqual(cfg.encoder.attention.dtype, "override_dtype")
     self.assertEqual(cfg.decoder.self_attention.dtype, "override_dtype")
     self.assertEqual(cfg.encoder.attention.kernel_init, "override_init")
     self.assertEqual(cfg.decoder.self_attention.kernel_init, "override_init")
 
+  def test_check_nonempty(self):
+    cfg = encoder_decoder_config()
+    with self.assertRaisesRegex(ValueError, "Selection.*fcn.*is empty"):
+      selectors.select(cfg, fcn, check_nonempty=True)
+
   def test_debug_get(self):
     cfg = encoder_decoder_config()
     attention_kernels = list(
         selectors.select(cfg, Attention).get("kernel_init"))
     self.assertCountEqual(["kernel1", "kernel1", "kernel2"], attention_kernels)
 
 
@@ -344,10 +338,23 @@
     config.bias_init = 2
 
     selectors.select(
         config, tag=KernelInitializerTag).replace(
             value=KernelInitializerTag.new("actual_value"))
     self.assertEqual(fdl.build(config), Attention("float32", "actual_value", 2))
 
+  def test_iterate_no_values(self):
+    config = fdl.Config(Attention, dtype="float32")
+    fdl.add_tag(config, "kernel_init", KernelInitializerTag)
+    fdl.add_tag(config, "bias_init", BiasInitializerTag)
+
+    self.assertEqual(
+        list(selectors.select(config, tag=KernelInitializerTag)), [fdl.NO_VALUE]
+    )
+    self.assertEqual(
+        list(selectors.select(config, tag=AnyInitializerTag)),
+        [fdl.NO_VALUE, fdl.NO_VALUE],
+    )
+
 
 if __name__ == "__main__":
   absltest.main()
```

### Comparing `fiddle-0.2.7/fiddle/_src/signatures.py` & `fiddle-0.2.8/fiddle/_src/signatures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/signatures_test.py` & `fiddle-0.2.8/fiddle/_src/signatures_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/signatures_test_helper.py` & `fiddle-0.2.8/fiddle/_src/signatures_test_helper.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/tag_type.py` & `fiddle-0.2.8/fiddle/_src/tag_type.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/tagging.py` & `fiddle-0.2.8/fiddle/_src/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/tagging_test.py` & `fiddle-0.2.8/fiddle/_src/tagging_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/tagging_test_module.py` & `fiddle-0.2.8/fiddle/_src/tagging_test_module.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/__init__.py` & `fiddle-0.2.8/fiddle/_src/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/autotest.py` & `fiddle-0.2.8/fiddle/_src/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/example/__init__.py` & `fiddle-0.2.8/fiddle/_src/testing/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/example/demo_configs.py` & `fiddle-0.2.8/fiddle/extensions/tf.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,26 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Sample configs to use to validate the testing infrastructure."""
+"""Fiddle extensions to handle TensorFlow code more elegantly.
 
-import dataclasses
-import fiddle as fdl
+Currently this affects codegen, graphviz, serialization, and other
+debugging functions.
+"""
 
-
-@dataclasses.dataclass
-class Simple:
-  x: int
-  y: str = 'why?'
-
-
-def base() -> fdl.Config:
-  return fdl.Config(Simple, x=1)
-
-
-def simple_fiddler(cfg: fdl.Config):
-  cfg.x += 1
-  cfg.y *= 3  # Lots of why's!
+# pylint: disable=unused-import
+from fiddle._src.extensions.tf import enable
```

### Comparing `fiddle-0.2.7/fiddle/_src/testing/example/fake_encoder_decoder.py` & `fiddle-0.2.8/fiddle/_src/testing/example/fake_encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/example/person_friend_toy.py` & `fiddle-0.2.8/fiddle/_src/testing/example/person_friend_toy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/nested_values.py` & `fiddle-0.2.8/fiddle/_src/testing/nested_values.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/nested_values_test.py` & `fiddle-0.2.8/fiddle/_src/testing/nested_values_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/test_util.py` & `fiddle-0.2.8/fiddle/_src/testing/test_util.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/_src/testing/test_util_test.py` & `fiddle-0.2.8/fiddle/_src/testing/test_util_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/__init__.py` & `fiddle-0.2.8/fiddle/absl_flags/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/example/__init__.py` & `fiddle-0.2.8/fiddle/absl_flags/example/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/example/business_logic.py` & `fiddle-0.2.8/fiddle/absl_flags/example/business_logic.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/example/configs.py` & `fiddle-0.2.8/fiddle/absl_flags/example/configs.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/example/example.py` & `fiddle-0.2.8/fiddle/absl_flags/example/example.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/absl_flags/example/tags.py` & `fiddle-0.2.8/fiddle/absl_flags/example/tags.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/arg_factory.py` & `fiddle-0.2.8/fiddle/arg_factory.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/building.py` & `fiddle-0.2.8/fiddle/building.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/codegen/__init__.py` & `fiddle-0.2.8/fiddle/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/codegen/auto_config/__init__.py` & `fiddle-0.2.8/fiddle/codegen/auto_config/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/codegen/auto_config/experimental_top_level_api.py` & `fiddle-0.2.8/fiddle/codegen/auto_config/experimental_top_level_api.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/codegen/codegen.py` & `fiddle-0.2.8/fiddle/codegen/codegen.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,7 +16,9 @@
 """Library for generating code from a Config or Partial object."""
 
 # pylint: disable=unused-import
 from fiddle._src.codegen.legacy_codegen import assignment_path
 from fiddle._src.codegen.legacy_codegen import codegen_dot_syntax
 from fiddle._src.codegen.legacy_codegen import mini_ast
 from fiddle._src.codegen.legacy_codegen import SharedBuildableManager
+from fiddle._src.codegen.new_codegen import code_generator
+from fiddle._src.codegen.new_codegen import new_codegen
```

### Comparing `fiddle-0.2.7/fiddle/codegen/codegen_diff.py` & `fiddle-0.2.8/fiddle/codegen/codegen_diff.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/codegen/py_val_to_cst_converter.py` & `fiddle-0.2.8/fiddle/codegen/py_val_to_cst_converter.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/config.py` & `fiddle-0.2.8/fiddle/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,8 +20,7 @@
 from fiddle._src.config import ArgFactory
 from fiddle._src.config import Buildable
 from fiddle._src.config import BuildableTraverserMetadata
 from fiddle._src.config import Config
 from fiddle._src.config import NO_VALUE
 from fiddle._src.config import NoValue
 from fiddle._src.config import Partial
-from fiddle._src.config import TiedValue
```

### Comparing `fiddle-0.2.7/fiddle/config_test.py` & `fiddle-0.2.8/fiddle/config_test.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/daglish.py` & `fiddle-0.2.8/fiddle/daglish.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/diffing.py` & `fiddle-0.2.8/fiddle/diffing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/examples/__init__.py` & `fiddle-0.2.8/fiddle/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/examples/colabs/__init__.py` & `fiddle-0.2.8/fiddle/examples/colabs/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/__init__.py` & `fiddle-0.2.8/fiddle/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/auto_config.py` & `fiddle-0.2.8/fiddle/experimental/auto_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/auto_config_policy.py` & `fiddle-0.2.8/fiddle/experimental/auto_config_policy.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/autobuilders/__init__.py` & `fiddle-0.2.8/fiddle/experimental/autobuilders/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/configurator.py` & `fiddle-0.2.8/fiddle/experimental/configurator.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/dataclasses.py` & `fiddle-0.2.8/fiddle/experimental/dataclasses.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/dict_config.py` & `fiddle-0.2.8/fiddle/experimental/dict_config.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/fixture_node.py` & `fiddle-0.2.8/fiddle/experimental/namespace_config.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,17 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Declares a fixture node, which allows two-stage configuration.
-
-By delegating implementation of the fixture to the user, we sidestep questions
-of what sub-configuation DAGs should be shared, how to replicate them, etc.,
-which are hard questions to answer well at the Fiddle library level.
-"""
+"""A Config that builds a `types.SimpleNamespace` from any argument."""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.fixture_node import FixtureNode
-from fiddle._src.experimental.fixture_node import materialize
+from fiddle._src.experimental.namespace_config import NamespaceConfig
```

### Comparing `fiddle-0.2.7/fiddle/experimental/namespace_config.py` & `fiddle-0.2.8/fiddle/experimental/transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,11 +9,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""A Config that builds a `types.SimpleNamespace` from any argument."""
+"""Transformation functions for Fiddle buildables."""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.namespace_config import NamespaceConfig
+from fiddle._src.experimental.transform import replace_unconfigured_partials_with_callables
+from fiddle._src.experimental.transform import unintern_tuples_of_literals
```

### Comparing `fiddle-0.2.7/fiddle/experimental/serialization.py` & `fiddle-0.2.8/fiddle/experimental/serialization.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/tied_value.py` & `fiddle-0.2.8/fiddle/testing/test_util.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,11 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Public API for tied values."""
+"""Utility functions for tests that use fiddle.experimental.daglish."""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.tied_value import get_tied
-from fiddle._src.experimental.tied_value import tied_value
-from fiddle._src.experimental.tied_value import TiedValue
-from fiddle._src.experimental.tied_value import untie
+from fiddle._src.testing.test_util import TestCase
```

### Comparing `fiddle-0.2.7/fiddle/experimental/transform.py` & `fiddle-0.2.8/fiddle/experimental/yaml_serialization.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,12 +9,17 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Transformation functions for Fiddle buildables."""
+"""Serialization helper that writes YAML output.
+
+Note: This API is highly experimental, and primarily intended for dumping
+objects in a medium-easy-to-read format, using indentation/spaces instead of
+`printing.py`'s dot-separated paths. Please use `serialization.py` whenever
+you need to serialize Fiddle objects in a robust manner.
+"""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.transform import replace_unconfigured_partials_with_callables
-from fiddle._src.experimental.transform import unintern_tuples_of_literals
+from fiddle._src.experimental.yaml_serialization import dump_yaml
```

### Comparing `fiddle-0.2.7/fiddle/experimental/visualize.py` & `fiddle-0.2.8/fiddle/experimental/visualize.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/experimental/yaml_serialization.py` & `fiddle-0.2.8/fiddle/graphviz.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Serialization helper that writes YAML output.
-
-Note: This API is highly experimental, and primarily intended for dumping
-objects in a medium-easy-to-read format, using indentation/spaces instead of
-`printing.py`'s dot-separated paths. Please use `serialization.py` whenever
-you need to serialize Fiddle objects in a robust manner.
-"""
+"""Provides a renderer to visualize a DAG of `fdl.Buildable`s via Graphviz."""
 
 # pylint: disable=unused-import
-from fiddle._src.experimental.yaml_serialization import dump_yaml
+
+from fiddle._src.graphviz import render
+from fiddle._src.graphviz import render_diff
+from fiddle._src.graphviz_custom_object import CustomGraphvizBuildable
+from fiddle._src.graphviz_custom_object import GraphvizRendererApi
```

### Comparing `fiddle-0.2.7/fiddle/extensions/__init__.py` & `fiddle-0.2.8/fiddle/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/extensions/jax.py` & `fiddle-0.2.8/fiddle/extensions/jax.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/extensions/seqio.py` & `fiddle-0.2.8/fiddle/extensions/seqio.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/extensions/tf.py` & `fiddle-0.2.8/fiddle/tag_type.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Fiddle extensions to handle TensorFlow code more elegantly.
+"""Defines the core dataclasses for tagging.
 
-Currently this affects codegen, graphviz, serialization, and other
-debugging functions.
+Please see tagging.py for information about tagging APIs.
 """
 
 # pylint: disable=unused-import
-from fiddle._src.extensions.tf import enable
+from fiddle._src.tag_type import TaggedValueNotFilledError
+from fiddle._src.tag_type import TagType
```

### Comparing `fiddle-0.2.7/fiddle/history.py` & `fiddle-0.2.8/fiddle/history.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/printing.py` & `fiddle-0.2.8/fiddle/printing.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/selectors.py` & `fiddle-0.2.8/fiddle/selectors.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/signatures.py` & `fiddle-0.2.8/fiddle/signatures.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/tagging.py` & `fiddle-0.2.8/fiddle/tagging.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/testing/__init__.py` & `fiddle-0.2.8/fiddle/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/testing/autotest.py` & `fiddle-0.2.8/fiddle/testing/autotest.py`

 * *Files identical despite different names*

### Comparing `fiddle-0.2.7/fiddle/version.py` & `fiddle-0.2.8/fiddle/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Current Fiddle version at head on Github."""
-__version__ = "0.2.7"
+__version__ = "0.2.8"
```

### Comparing `fiddle-0.2.7/fiddle.egg-info/PKG-INFO` & `fiddle-0.2.8/fiddle.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiddle
-Version: 0.2.7
+Version: 0.2.8
 Summary: Fiddle: A Python-first configuration library
 Home-page: https://github.com/google/fiddle
 Author: The Fiddle Team
 Author-email: noreply@google.com
 License: Apache 2.0
 Project-URL: Documentation, https://github.com/google/fiddle/docs
 Project-URL: Bug Reports, https://github.com/google/fiddle/issues
```

### Comparing `fiddle-0.2.7/fiddle.egg-info/SOURCES.txt` & `fiddle-0.2.8/fiddle.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -117,21 +117,17 @@
 fiddle/_src/experimental/configurator.py
 fiddle/_src/experimental/daglish_legacy.py
 fiddle/_src/experimental/daglish_legacy_test.py
 fiddle/_src/experimental/dataclasses.py
 fiddle/_src/experimental/dataclasses_test.py
 fiddle/_src/experimental/dict_config.py
 fiddle/_src/experimental/dict_config_test.py
-fiddle/_src/experimental/fixture_node.py
-fiddle/_src/experimental/fixture_node_test.py
 fiddle/_src/experimental/namespace_config.py
 fiddle/_src/experimental/namespace_config_test.py
 fiddle/_src/experimental/serialization.py
-fiddle/_src/experimental/tied_value.py
-fiddle/_src/experimental/tied_value_test.py
 fiddle/_src/experimental/transform.py
 fiddle/_src/experimental/transform_test.py
 fiddle/_src/experimental/visualize.py
 fiddle/_src/experimental/with_tags.py
 fiddle/_src/experimental/with_tags_test.py
 fiddle/_src/experimental/yaml_serialization.py
 fiddle/_src/experimental/yaml_serialization_test.py
@@ -172,18 +168,16 @@
 fiddle/examples/colabs/__init__.py
 fiddle/experimental/__init__.py
 fiddle/experimental/auto_config.py
 fiddle/experimental/auto_config_policy.py
 fiddle/experimental/configurator.py
 fiddle/experimental/dataclasses.py
 fiddle/experimental/dict_config.py
-fiddle/experimental/fixture_node.py
 fiddle/experimental/namespace_config.py
 fiddle/experimental/serialization.py
-fiddle/experimental/tied_value.py
 fiddle/experimental/transform.py
 fiddle/experimental/visualize.py
 fiddle/experimental/yaml_serialization.py
 fiddle/experimental/autobuilders/__init__.py
 fiddle/extensions/__init__.py
 fiddle/extensions/jax.py
 fiddle/extensions/seqio.py
```

### Comparing `fiddle-0.2.7/setup.py` & `fiddle-0.2.8/setup.py`

 * *Files identical despite different names*

