# Comparing `tmp/canals-0.3.1.tar.gz` & `tmp/canals-0.3.2.tar.gz`

## Comparing `canals-0.3.1.tar` & `canals-0.3.2.tar`

### file list

```diff
@@ -1,78 +1,78 @@
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.3.1/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 canals-0.3.1/.github/workflows/tests.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.3.1/canals/__about__.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.3.1/canals/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 canals-0.3.1/canals/errors.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/__init__.py
--rw-r--r--   0        0        0    14157 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/component.py
--rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 canals-0.3.1/canals/component/input_output.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/__init__.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/draw.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/graphviz.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 canals-0.3.1/canals/draw/mermaid.py
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/__init__.py
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/connections.py
--rw-r--r--   0        0        0    31560 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/save_load.py
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/sockets.py
--rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 canals-0.3.1/canals/pipeline/validation.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.1/canals/testing/__init__.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.3.1/canals/testing/test_component.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.1/docs/index.md
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/component.md
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/draw.md
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.3.1/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/components.md
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/concepts.md
--rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 canals-0.3.1/docs/concepts/pipelines.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.3.1/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.3.1/images/canals-logo-light.png
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/__init__.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.1/test/_helpers.py
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.1/test/conftest.py
--rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_save_load.py
--rw-r--r--   0        0        0     5063 2020-02-02 00:00:00.000000 canals-0.3.1/test/component/test_component.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/__init__.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_complex_pipeline.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_double_loop_pipeline.py
--rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_decision_pipeline.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_fixed_merging_pipeline.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_linear_pipeline.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_looping_pipeline.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_decision_pipeline.py
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/integration/test_variable_merging_pipeline.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/__init__.py
--rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_connections.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_draw.py
--rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_input_sockets.py
--rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_output_sockets.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_pipeline.py
--rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 canals-0.3.1/test/pipelines/unit/test_validation_pipeline_io.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/__init__.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_accumulate.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_add_value.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_concatenate.py
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_double.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_greet.py
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_merge_loop.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_parity.py
--rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_remainder.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_repeat.py
--rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_subtract.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_sum.py
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 canals-0.3.1/test/sample_components/test_threshold.py
--rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_files/mermaid_mock/test_response.png
--rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 canals-0.3.1/test/test_files/pipeline_draw/pygraphviz.jpg
--rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.3.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.3.1/LICENSE
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 canals-0.3.1/README.md
--rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 canals-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 canals-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.3.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.3.2/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 canals-0.3.2/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 canals-0.3.2/canals/__about__.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 canals-0.3.2/canals/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 canals-0.3.2/canals/errors.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/__init__.py
+-rw-r--r--   0        0        0    14156 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/component.py
+-rw-r--r--   0        0        0     4818 2020-02-02 00:00:00.000000 canals-0.3.2/canals/component/input_output.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/draw.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 canals-0.3.2/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/connections.py
+-rw-r--r--   0        0        0    31560 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     6668 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/sockets.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 canals-0.3.2/canals/pipeline/validation.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 canals-0.3.2/canals/testing/__init__.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 canals-0.3.2/canals/testing/test_component.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.2/docs/index.md
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.3.2/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     6408 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/components.md
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     6902 2020-02-02 00:00:00.000000 canals-0.3.2/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.3.2/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.3.2/images/canals-logo-light.png
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/__init__.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.2/test/_helpers.py
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 canals-0.3.2/test/conftest.py
+-rw-r--r--   0        0        0     6615 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_save_load.py
+-rw-r--r--   0        0        0     6630 2020-02-02 00:00:00.000000 canals-0.3.2/test/component/test_component.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_double_loop_pipeline.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0    22518 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_connections.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_draw.py
+-rw-r--r--   0        0        0     8999 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_input_sockets.py
+-rw-r--r--   0        0        0     9130 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_output_sockets.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_pipeline.py
+-rw-r--r--   0        0        0     6533 2020-02-02 00:00:00.000000 canals-0.3.2/test/pipelines/unit/test_validation_pipeline_io.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/__init__.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_accumulate.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_add_value.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_concatenate.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_double.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_greet.py
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_parity.py
+-rw-r--r--   0        0        0     2097 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_remainder.py
+-rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_repeat.py
+-rw-r--r--   0        0        0     1291 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_subtract.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_sum.py
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 canals-0.3.2/test/sample_components/test_threshold.py
+-rw-r--r--   0        0        0     2976 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_files/mermaid_mock/test_response.png
+-rw-r--r--   0        0        0     9327 2020-02-02 00:00:00.000000 canals-0.3.2/test/test_files/pipeline_draw/pygraphviz.jpg
+-rw-r--r--   0        0        0     1843 2020-02-02 00:00:00.000000 canals-0.3.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.3.2/LICENSE
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 canals-0.3.2/README.md
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 canals-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 canals-0.3.2/PKG-INFO
```

### Comparing `canals-0.3.1/.pre-commit-config.yaml` & `canals-0.3.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/mkdocs.yml` & `canals-0.3.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/.github/workflows/tests.yml` & `canals-0.3.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/errors.py` & `canals-0.3.2/canals/errors.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/component/component.py` & `canals-0.3.2/canals/component/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     """
     inputs_found = []
     outputs_found = []
 
     # Get all properties of class_
     properties = inspect.getmembers(class_, predicate=lambda m: isinstance(m, property))
     for _, prop in properties:
-        if not hasattr(prop, "fget") and not hasattr(prop.fget, "__canals_connection__"):
+        if not hasattr(prop, "fget") or not hasattr(prop.fget, "__canals_connection__"):
             continue
 
         # Field __canals_connection__ is set by _input and _output decorators
         if prop.fget.__canals_connection__ == Connection.INPUT:
             inputs_found.append(prop)
         elif prop.fget.__canals_connection__ == Connection.OUTPUT:
             outputs_found.append(prop)
```

### Comparing `canals-0.3.1/canals/component/input_output.py` & `canals-0.3.2/canals/component/input_output.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/draw/draw.py` & `canals-0.3.2/canals/draw/draw.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/draw/graphviz.py` & `canals-0.3.2/canals/draw/graphviz.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/draw/mermaid.py` & `canals-0.3.2/canals/draw/mermaid.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/pipeline/connections.py` & `canals-0.3.2/canals/pipeline/connections.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/pipeline/pipeline.py` & `canals-0.3.2/canals/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/pipeline/save_load.py` & `canals-0.3.2/canals/pipeline/save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/pipeline/sockets.py` & `canals-0.3.2/canals/pipeline/sockets.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/pipeline/validation.py` & `canals-0.3.2/canals/pipeline/validation.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/canals/testing/test_component.py` & `canals-0.3.2/canals/testing/test_component.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/docs/index.md` & `canals-0.3.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/docs/concepts/components.md` & `canals-0.3.2/docs/concepts/components.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/docs/concepts/concepts.md` & `canals-0.3.2/docs/concepts/concepts.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/docs/concepts/pipelines.md` & `canals-0.3.2/docs/concepts/pipelines.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/images/canals-logo-dark.png` & `canals-0.3.2/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/images/canals-logo-light.png` & `canals-0.3.2/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/_helpers.py` & `canals-0.3.2/test/_helpers.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/conftest.py` & `canals-0.3.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/test_save_load.py` & `canals-0.3.2/test/test_save_load.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/component/test_component.py` & `canals-0.3.2/test/component/test_component.py`

 * *Files 21% similar despite different names*

```diff
@@ -25,14 +25,79 @@
             return self.output(output_value=1)
 
     # Verifies also instantiation works with no issues
     assert MockComponent()
     assert component.registry["MockComponent"] == MockComponent
 
 
+def test_correct_declaration_with_additional_readonly_property():
+    @component
+    class MockComponent:
+        @component.input
+        def input(self):
+            class Input:
+                input_value: int
+
+            return Input
+
+        @component.output
+        def output(self):
+            class Output:
+                output_value: int
+
+            return Output
+
+        @property
+        def store(self):
+            return "test_store"
+
+        def run(self, data):
+            return self.output(output_value=1)
+
+    # Verifies that instantiation works with no issues
+    assert MockComponent()
+    assert component.registry["MockComponent"] == MockComponent
+    assert MockComponent().store == "test_store"
+
+
+def test_correct_declaration_with_additional_writable_property():
+    @component
+    class MockComponent:
+        @component.input
+        def input(self):
+            class Input:
+                input_value: int
+
+            return Input
+
+        @component.output
+        def output(self):
+            class Output:
+                output_value: int
+
+            return Output
+
+        @property
+        def store(self):
+            return self._store
+
+        @store.setter
+        def store(self, value):
+            self._store = value
+
+        def run(self, data):
+            return self.output(output_value=1)
+
+    # Verifies that instantiation works with no issues
+    assert component.registry["MockComponent"] == MockComponent
+    comp = MockComponent()
+    comp.store = "test_store"
+    assert comp.store == "test_store"
+
+
 def test_input_required():
     with pytest.raises(
         ComponentError,
         match="No input definition found in Component MockComponent. "
         "Create a method that returns a dataclass defining the input and "
         "decorate it with @component.input\(\) to fix the error.",
     ):
```

### Comparing `canals-0.3.1/test/pipelines/integration/test_complex_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_complex_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_double_loop_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_double_loop_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_fixed_decision_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_fixed_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_fixed_merging_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_fixed_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_linear_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_linear_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_looping_and_merge_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_looping_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_looping_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_parallel_branches_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_parallel_branches_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_variable_decision_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/integration/test_variable_merging_pipeline.py` & `canals-0.3.2/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_connections.py` & `canals-0.3.2/test/pipelines/unit/test_connections.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_draw.py` & `canals-0.3.2/test/pipelines/unit/test_draw.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_input_sockets.py` & `canals-0.3.2/test/pipelines/unit/test_input_sockets.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_output_sockets.py` & `canals-0.3.2/test/pipelines/unit/test_output_sockets.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_pipeline.py` & `canals-0.3.2/test/pipelines/unit/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/pipelines/unit/test_validation_pipeline_io.py` & `canals-0.3.2/test/pipelines/unit/test_validation_pipeline_io.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/__init__.py` & `canals-0.3.2/test/sample_components/__init__.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_accumulate.py` & `canals-0.3.2/test/sample_components/test_accumulate.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_add_value.py` & `canals-0.3.2/test/sample_components/test_add_value.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_concatenate.py` & `canals-0.3.2/test/sample_components/test_concatenate.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_double.py` & `canals-0.3.2/test/sample_components/test_double.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_greet.py` & `canals-0.3.2/test/sample_components/test_greet.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_merge_loop.py` & `canals-0.3.2/test/sample_components/test_merge_loop.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_parity.py` & `canals-0.3.2/test/sample_components/test_parity.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_remainder.py` & `canals-0.3.2/test/sample_components/test_remainder.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_repeat.py` & `canals-0.3.2/test/sample_components/test_repeat.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_subtract.py` & `canals-0.3.2/test/sample_components/test_subtract.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_sum.py` & `canals-0.3.2/test/sample_components/test_sum.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/sample_components/test_threshold.py` & `canals-0.3.2/test/sample_components/test_threshold.py`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/test_files/mermaid_mock/test_response.png` & `canals-0.3.2/test/test_files/mermaid_mock/test_response.png`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/test/test_files/pipeline_draw/pygraphviz.jpg` & `canals-0.3.2/test/test_files/pipeline_draw/pygraphviz.jpg`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/.gitignore` & `canals-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/LICENSE` & `canals-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/README.md` & `canals-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/pyproject.toml` & `canals-0.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `canals-0.3.1/PKG-INFO` & `canals-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.3.1
+Version: 0.3.2
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: canals Version: 0.3.1 Summary: A component
+Metadata-Version: 2.1 Name: canals Version: 0.3.2 Summary: A component
 orchestration engine for Haystack Project-URL: Documentation, https://
 github.com/deepset-ai/canals#readme Project-URL: Issues, https://github.com/
 deepset-ai/canals/issues Project-URL: Source, https://github.com/deepset-ai/
 canals Author-email: ZanSara
 zanzottera@deepset.ai> License-Expression: Apache-2.0 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha Classifier: License :: Freely
 Distributable Classifier: License :: OSI Approved :: Apache Software License
```

