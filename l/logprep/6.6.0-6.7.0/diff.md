# Comparing `tmp/logprep-6.6.0.tar.gz` & `tmp/logprep-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logprep-6.6.0.tar", last modified: Mon Jul  3 12:51:55 2023, max compression
+gzip compressed data, was "logprep-6.7.0.tar", last modified: Mon Jul 17 09:06:39 2023, max compression
```

## Comparing `logprep-6.6.0.tar` & `logprep-6.7.0.tar`

### file list

```diff
@@ -1,537 +1,537 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-03 12:51:51.000000 logprep-6.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-03 12:51:51.000000 logprep-6.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-03 12:51:55.490977 logprep-6.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-07-03 12:51:51.000000 logprep-6.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.494977 logprep-6.6.0/logprep/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-03 12:51:55.494977 logprep-6.6.0/logprep/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/abc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/output.py
--rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/abc/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/confluent_kafka/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/confluent_kafka/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/console/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/console/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/dummy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/dummy/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/elasticsearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/elasticsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13487 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/elasticsearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/file/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/http/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/http/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/json/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/json/input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/jsonl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/jsonl/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/opensearch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/opensearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/opensearch/output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/connector/s3/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/connector/s3/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/factory_error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep/filter/expression/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/expression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/expression/filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/filter/lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/framework/rule_tree/rule_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/metrics/metric_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/amides/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/base/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/fourFn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/calculator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/concatenator/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/datetime_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/deleter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.462977 logprep-6.6.0/logprep/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9759 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dissector/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_label_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/domain_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/dropper/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/field_manager/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/mysql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_adder/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/generic_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/geoip_enricher/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/grokker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/hyperscan_resolver/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/ip_informer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/key_checker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/key_checker/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/labeling_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/labeler/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/list_comparison/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/normalizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.466977 logprep-6.6.0/logprep/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pre_detector/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/pseudonymizer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/requester/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/selective_extractor/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/string_splitter/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/template_replacer/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamp_differ/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/processor/timestamper/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/aggregating_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.470977 logprep-6.6.0/logprep/util/auto_rule_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/getter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9006 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/grok.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.454977 logprep-6.6.0/logprep/util/grok/patterns/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/aws
--rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bind
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/exim
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/java
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/maven
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/rails
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/redis
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/squid
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/zeek
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/logprep/util/grok/patterns/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/aws
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bacula
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bind
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/bro
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/exim
--rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/firewalls
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/grok-patterns
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/haproxy
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/httpd
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/java
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/junos
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/linux-syslog
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/maven
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mcollective
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mcollective-patterns
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/mongodb
--rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/nagios
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/postgresql
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/rails
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/redis
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/ruby
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok/patterns/legacy/squid
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9641 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/json_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/multiprocessing_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/pipeline_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/pre_detector_rule_matching_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-03 12:51:51.000000 logprep-6.6.0/logprep/util/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.458977 logprep-6.6.0/logprep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-03 12:51:55.000000 logprep-6.6.0/logprep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-03 12:51:51.000000 logprep-6.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-03 12:51:55.494977 logprep-6.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-03 12:51:51.000000 logprep-6.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.474977 logprep-6.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_config_refresh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_file_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_full_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_multiple_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_pre_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/test_wineventlog_pseudonymization.py
--rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/acceptance/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/runner-image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/ci/runner-image/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/ci/runner-image/scripts/compare_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/ConfigurationForTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/FilledTempFile.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/ruledata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/testdata/unit/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/testdata/unit/clusterer/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.478977 logprep-6.6.0/tests/unit/component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/component/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/connector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_confluent_kafka_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_console_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_dummy_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_dummy_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9100 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_elasticsearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_default_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_not_tailing_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_file_input_start_at_end_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_http_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_json_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_jsonl_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_jsonl_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_opensearch_output.py
--rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/connector/test_s3_output.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/exceptions/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/exceptions/processor/test_processing_warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/filter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/test_filter_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/filter/test_lucene_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/framework/rule_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/framework/test_pipeline_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metric_exposer.py
--rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metric_targets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/metrics/test_metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/amides/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_amides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_amides_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_normalize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/amides/test_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/calculator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/test_calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/calculator/test_calculator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/clusterer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/concatenator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/datetime_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.482977 logprep-6.6.0/tests/unit/processor/deleter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/test_deleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/deleter/test_deleter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/dissector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/test_dissector.py
--rw-r--r--   0 runner    (1001) docker     (123)    17960 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dissector/test_dissector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/domain_label_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/domain_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/dropper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/test_dropper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/dropper/test_dropper_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/field_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/generic_adder/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/generic_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/geoip_enricher/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/grokker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grok.py
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grokker.py
--rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/grokker/test_grokker_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/ip_informer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/labeler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeler_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/labeler/test_labeling_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/list_comparison/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.486977 logprep-6.6.0/tests/unit/processor/normalizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38341 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/pre_detector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_ip_alerter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/pseudonymizer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_encrypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/requester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/test_requester.py
--rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/requester/test_requester_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/selective_extractor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/string_splitter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/template_replacer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/template_replacer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/template_replacer/test_template_replacer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/test_processor_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/test_processor_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/timestamp_differ/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
--rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/processor/timestamper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10055 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_run_logprep.py
--rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/test_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/unit/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19327 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_auto_rule_corpus_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_auto_rule_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_grok_pattern.py
--rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_grok_pattern_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_hasher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_helper_add_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_log_aggregator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_processor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_prometheus_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_rule_dry_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_schema_and_rule_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_time_measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/test_validators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/unit/util/tests_json_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:55.490977 logprep-6.6.0/tests/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-03 12:51:51.000000 logprep-6.6.0/tests/util/testhelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-07-03 12:51:51.000000 logprep-6.6.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    26526 2023-07-17 09:06:25.000000 logprep-6.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-17 09:06:25.000000 logprep-6.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-17 09:06:39.496904 logprep-6.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16888 2023-07-17 09:06:25.000000 logprep-6.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/logprep/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 09:06:39.496904 logprep-6.7.0/logprep/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/abc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16580 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12111 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/abc/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/confluent_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13345 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8002 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/confluent_kafka/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/console/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/console/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/dummy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/dummy/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/elasticsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/elasticsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17783 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/elasticsearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13765 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/file/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/http/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/json/input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.448904 logprep-6.7.0/logprep/connector/jsonl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/jsonl/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/connector/opensearch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/opensearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/opensearch/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/connector/s3/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/connector/s3/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/factory_error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/filter/expression/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/expression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11694 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/expression/filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14990 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/filter/lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22836 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/framework/rule_tree/rule_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/metrics/metric_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.452904 logprep-6.7.0/logprep/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5277 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11390 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/amides/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/base/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/fourFn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/calculator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4418 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/rules/rule_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6672 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/clusterer/signature_calculation/signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/concatenator/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/datetime_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.456904 logprep-6.7.0/logprep/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/deleter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dissector/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_label_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/domain_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/dropper/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7506 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/field_manager/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/mysql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10887 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_adder/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5616 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/generic_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/geoip_enricher/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4630 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/grokker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7441 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/hyperscan_resolver/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/ip_informer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.460904 logprep-6.7.0/logprep/processor/key_checker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/key_checker/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6943 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/labeling_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/labeler/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/list_comparison/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16233 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28757 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/normalizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5099 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pre_detector/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16361 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/pseudonymizer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/requester/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/selective_extractor/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/string_splitter/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6064 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/template_replacer/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamp_differ/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.464904 logprep-6.7.0/logprep/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/processor/timestamper/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4985 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8561 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11023 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/aggregating_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/auto_rule_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19103 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26980 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19307 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/getter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.468904 logprep-6.7.0/logprep/util/grok/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9075 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/grok.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.436904 logprep-6.7.0/logprep/util/grok/patterns/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/maven
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/zeek
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/logprep/util/grok/patterns/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/aws
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bacula
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bind
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/bro
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/exim
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/firewalls
+-rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/grok-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/haproxy
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/httpd
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/java
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/junos
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/linux-syslog
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/maven
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mcollective
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mcollective-patterns
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/mongodb
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/nagios
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/postgresql
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/rails
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/redis
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/ruby
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok/patterns/legacy/squid
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10188 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/json_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/multiprocessing_log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/pipeline_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12543 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/pre_detector_rule_matching_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4442 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6602 2023-07-17 09:06:25.000000 logprep-6.7.0/logprep/util/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.444904 logprep-6.7.0/logprep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17607 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-17 09:06:39.000000 logprep-6.7.0/logprep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-17 09:06:25.000000 logprep-6.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-17 09:06:39.496904 logprep-6.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-07-17 09:06:25.000000 logprep-6.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.472904 logprep-6.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_config_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_file_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9180 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_full_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_multiple_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19060 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_pre_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/test_wineventlog_pseudonymization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10368 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/acceptance/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/runner-image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/ci/runner-image/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/ci/runner-image/scripts/compare_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/ConfigurationForTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/FilledTempFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/ruledata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/testdata/unit/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12733 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/testdata/unit/clusterer/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.476904 logprep-6.7.0/tests/unit/component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/component/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21616 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7315 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_confluent_kafka_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_console_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_dummy_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_dummy_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13404 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_elasticsearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9926 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_default_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_not_tailing_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_file_input_start_at_end_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_http_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_json_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_jsonl_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_jsonl_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_opensearch_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10265 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/connector/test_s3_output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/exceptions/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/exceptions/processor/test_processing_warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22185 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/test_filter_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20548 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/filter/test_lucene_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/framework/rule_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31631 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19943 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39696 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9032 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/framework/test_pipeline_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8285 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metric_exposer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22279 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metric_targets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5612 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/metrics/test_metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.480904 logprep-6.7.0/tests/unit/processor/amides/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_amides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_amides_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_normalize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/amides/test_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/calculator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/test_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/calculator/test_calculator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/clusterer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7217 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/concatenator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6963 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11216 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/datetime_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6723 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/deleter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/test_deleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/deleter/test_deleter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/dissector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23629 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/test_dissector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17940 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dissector/test_dissector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/domain_label_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/domain_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12825 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/dropper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/test_dropper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/dropper/test_dropper_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/field_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19047 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/generic_adder/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29997 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/generic_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14079 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.484904 logprep-6.7.0/tests/unit/processor/geoip_enricher/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16002 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/grokker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grok.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grokker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11691 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/grokker/test_grokker_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23145 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/ip_informer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/labeler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9177 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9016 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeler_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/labeler/test_labeling_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/list_comparison/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11202 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3623 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/normalizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38350 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/pre_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_ip_alerter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13887 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/pseudonymizer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_encrypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/requester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12431 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/test_requester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8142 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/requester/test_requester_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.488904 logprep-6.7.0/tests/unit/processor/selective_extractor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/string_splitter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/template_replacer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/template_replacer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/template_replacer/test_template_replacer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/test_processor_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8157 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/test_processor_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/timestamp_differ/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16573 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4283 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.492905 logprep-6.7.0/tests/unit/processor/timestamper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10064 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11779 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_run_logprep.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18858 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/test_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/tests/unit/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20761 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_auto_rule_corpus_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_auto_rule_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39375 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16243 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_grok_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3995 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_grok_pattern_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_hasher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7897 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_helper_add_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_log_aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_processor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_prometheus_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7288 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_rule_dry_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_schema_and_rule_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4103 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_time_measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16746 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/test_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/unit/util/tests_json_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:39.496904 logprep-6.7.0/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-07-17 09:06:25.000000 logprep-6.7.0/tests/util/testhelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81000 2023-07-17 09:06:25.000000 logprep-6.7.0/versioneer.py
```

### Comparing `logprep-6.6.0/LICENSE` & `logprep-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/PKG-INFO` & `logprep-6.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.6.0
+Version: 6.7.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.6.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.7.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.6.0/README.md` & `logprep-6.7.0/README.md`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/component.py` & `logprep-6.7.0/logprep/abc/component.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/connector.py` & `logprep-6.7.0/logprep/abc/connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/getter.py` & `logprep-6.7.0/logprep/abc/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/input.py` & `logprep-6.7.0/logprep/abc/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/output.py` & `logprep-6.7.0/logprep/abc/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/abc/processor.py` & `logprep-6.7.0/logprep/abc/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/configuration.py` & `logprep-6.7.0/logprep/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/confluent_kafka/input.py` & `logprep-6.7.0/logprep/connector/confluent_kafka/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/confluent_kafka/output.py` & `logprep-6.7.0/logprep/connector/confluent_kafka/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/console/output.py` & `logprep-6.7.0/logprep/connector/console/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/dummy/input.py` & `logprep-6.7.0/logprep/connector/dummy/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/dummy/output.py` & `logprep-6.7.0/logprep/connector/dummy/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/elasticsearch/output.py` & `logprep-6.7.0/logprep/connector/elasticsearch/output.py`

 * *Files 24% similar despite different names*

```diff
@@ -31,24 +31,25 @@
 """
 
 import json
 import re
 import ssl
 from functools import cached_property
 from logging import Logger
-from typing import List, Optional
+from typing import List, Optional, Tuple, Union, Pattern
 
 import elasticsearch as search
 from attr import define, field
 from attrs import validators
 from elasticsearch import ElasticsearchException, helpers
 from opensearchpy import OpenSearchException
 from urllib3.exceptions import TimeoutError
 
 from logprep.abc.output import FatalOutputError, Output
+from logprep.util.helper import get_dict_size_in_byte
 from logprep.util.time import TimeParser
 
 
 class ElasticsearchOutput(Output):
     """An Elasticsearch output connector."""
 
     @define(kw_only=True, slots=False)
@@ -69,35 +70,49 @@
         """Default index to write to if no index was set in the document or the document could not
         be indexed. The document will be transformed into a string to prevent rejections by the
         default index."""
         error_index: str = field(validator=validators.instance_of(str))
         """Index to write documents to that could not be processed."""
         message_backlog_size: int = field(validator=validators.instance_of(int))
         """Amount of documents to store before sending them."""
+        maximum_message_size_mb: Optional[Union[float, int]] = field(
+            validator=validators.optional(validators.instance_of((float, int))),
+            converter=(lambda x: x * 10**6 if x else None),
+            default=None,
+        )
+        """(Optional) Maximum estimated size of a document in MB before discarding it if it causes 
+        an error."""
         timeout: int = field(validator=validators.instance_of(int), default=500)
         """(Optional) Timeout for the connection (default is 500ms)."""
         max_retries: int = field(validator=validators.instance_of(int), default=0)
         """(Optional) Maximum number of retries for documents rejected with code 429 (default is 0).
         Increases backoff time by 2 seconds per try, but never exceeds 600 seconds."""
         user: Optional[str] = field(validator=validators.instance_of(str), default="")
         """(Optional) User used for authentication."""
         secret: Optional[str] = field(validator=validators.instance_of(str), default="")
         """(Optional) Secret used for authentication."""
         ca_cert: Optional[str] = field(validator=validators.instance_of(str), default="")
         """(Optional) Path to a SSL ca certificate to verify the ssl context."""
         flush_timeout: Optional[int] = field(validator=validators.instance_of(int), default=60)
-        """(Optional) Timout after :code:`message_backlog` is flushed if :code:`message_backlog_size` is not reached."""
+        """(Optional) Timout after :code:`message_backlog` is flushed if 
+        :code:`message_backlog_size` is not reached."""
 
-    __slots__ = ["_message_backlog"]
+    __slots__ = ["_message_backlog", "_size_error_pattern"]
 
     _message_backlog: List
 
+    _size_error_pattern: Pattern[str]
+
     def __init__(self, name: str, configuration: "ElasticsearchOutput.Config", logger: Logger):
         super().__init__(name, configuration, logger)
         self._message_backlog = []
+        self._size_error_pattern = re.compile(
+            r".*coordinating_operation_bytes=(?P<size>\d+), "
+            r"max_coordinating_and_primary_bytes=(?P<max_size>\d+).*"
+        )
 
     @cached_property
     def ssl_context(self) -> ssl.SSLContext:
         """Returns the ssl context
 
         Returns
         -------
@@ -165,14 +180,106 @@
         elasticsearch_output : ElasticsearchOutput
             Acts as output connector for Elasticsearch.
 
         """
         base_description = super().describe()
         return f"{base_description} - ElasticSearch Output: {self._config.hosts}"
 
+    def setup(self):
+        super().setup()
+        flush_timeout = self._config.flush_timeout
+        self._schedule_task(task=self._write_backlog, seconds=flush_timeout)
+        try:
+            self._search_context.info()
+        except (ElasticsearchException, OpenSearchException, TimeoutError) as error:
+            raise FatalOutputError(self, error) from error
+
+    def store(self, document: dict):
+        """Store a document in the index.
+
+        Parameters
+        ----------
+        document : dict
+           Document to store.
+
+        Returns
+        -------
+        Returns True to inform the pipeline to call the batch_finished_callback method in the
+        configured input
+        """
+        if document.get("_index") is None:
+            document = self._build_failed_index_document(document, "Missing index in document")
+
+        self._add_dates(document)
+        self.metrics.number_of_processed_events += 1
+        self._write_to_search_context(document)
+
+    def store_custom(self, document: dict, target: str):
+        """Write document to Elasticsearch into the target index.
+
+        Parameters
+        ----------
+        document : dict
+            Document to be stored into the target index.
+        target : str
+            Index to store the document in.
+        Raises
+        ------
+        CriticalOutputError
+            Raises if any error except a BufferError occurs while writing into elasticsearch.
+
+        """
+        document["_index"] = target
+        self._add_dates(document)
+        self.metrics.number_of_processed_events += 1
+        self._write_to_search_context(document)
+
+    def store_failed(self, error_message: str, document_received: dict, document_processed: dict):
+        """Write errors into error topic for documents that failed processing.
+
+        Parameters
+        ----------
+        error_message : str
+           Error message to write into Kafka document.
+        document_received : dict
+            Document as it was before processing.
+        document_processed : dict
+            Document after processing until an error occurred.
+
+        """
+        error_document = {
+            "error": error_message,
+            "original": document_received,
+            "processed": document_processed,
+            "@timestamp": TimeParser.now().isoformat(),
+            "_index": self._config.error_index,
+        }
+        self._add_dates(error_document)
+        self._write_to_search_context(error_document)
+
+    def _build_failed_index_document(self, message_document: dict, reason: str):
+        document = {
+            "reason": reason,
+            "@timestamp": TimeParser.now().isoformat(),
+            "_index": self._config.default_index,
+        }
+        try:
+            document["message"] = json.dumps(message_document)
+        except TypeError:
+            document["message"] = str(message_document)
+        return document
+
+    def _add_dates(self, document):
+        date_format_matches = self._replace_pattern.findall(document["_index"])
+        if date_format_matches:
+            now = TimeParser.now()
+            for date_format_match in date_format_matches:
+                formatted_date = now.strftime(date_format_match[2:-1])
+                document["_index"] = re.sub(date_format_match, formatted_date, document["_index"])
+
     def _write_to_search_context(self, document):
         """Writes documents from a buffer into Elasticsearch indices.
 
         Writes documents in a bulk if the document buffer limit has been reached.
         This reduces connections to Elasticsearch.
         The target index is determined per document by the value of the meta field '_index'.
         A configured default index is used if '_index' hasn't been set.
@@ -199,175 +306,173 @@
             self._search_context,
             self._message_backlog,
             max_retries=self._config.max_retries,
             chunk_size=len(self._message_backlog),
         )
         self._message_backlog.clear()
 
-    def _handle_bulk_index_error(self, error: helpers.BulkIndexError):
-        """Handle bulk indexing error for elasticsearch bulk indexing.
-
-        Documents that could not be sent to elastiscsearch due to index errors are collected and
-        sent into an error index that should always accept all documents.
-        This can lead to a rebuild of the pipeline if this causes another exception.
-
-        Parameters
-        ----------
-        error : BulkIndexError
-           BulkIndexError to collect IndexErrors from.
-
-        """
-        error_documents = []
-        for bulk_error in error.errors:
-            _, error_info = bulk_error.popitem()
-            data = error_info.get("data") if "data" in error_info else None
-            error_type = error_info.get("error").get("type")
-            error_reason = error_info.get("error").get("reason")
-            reason = f"{error_type}: {error_reason}"
-            error_document = self._build_failed_index_document(data, reason)
-            self._add_dates(error_document)
-            error_documents.append(error_document)
-        self._bulk(self._search_context, error_documents)
-
     def _bulk(self, *args, **kwargs):
         try:
             helpers.bulk(*args, **kwargs)
         except search.SerializationError as error:
             self._handle_serialization_error(error)
         except search.ConnectionError as error:
             self._handle_connection_error(error)
         except helpers.BulkIndexError as error:
             self._handle_bulk_index_error(error)
+        except search.exceptions.TransportError as error:
+            self._handle_transport_error(error)
         if self.input_connector:
             self.input_connector.batch_finished_callback()
 
-    def _handle_connection_error(self, error: search.ConnectionError):
-        """Handle connection error for elasticsearch bulk indexing.
+    def _handle_serialization_error(self, error: search.SerializationError):
+        """Handle serialization error for elasticsearch bulk indexing.
 
-        No documents will be sent if there is no connection to begin with.
+        If at least one document in a chunk can't be serialized, no events will be sent.
+        The chunk size is thus set to be the same size as the message backlog size.
         Therefore, it won't result in duplicates once the the data is resent.
-        If the connection is lost during indexing, duplicate documents could be sent.
 
         Parameters
         ----------
-        error : ConnectionError
-           ConnectionError for the error message.
+        error : SerializationError
+           SerializationError for the error message.
 
         Raises
         ------
         FatalOutputError
             This causes a pipeline rebuild and gives an appropriate error log message.
 
         """
-        raise FatalOutputError(self, error.error)
+        raise FatalOutputError(self, f"{error.args[1]} in document {error.args[0]}")
 
-    def _handle_serialization_error(self, error: search.SerializationError):
-        """Handle serialization error for elasticsearch bulk indexing.
+    def _handle_connection_error(self, error: search.ConnectionError):
+        """Handle connection error for elasticsearch bulk indexing.
 
-        If at least one document in a chunk can't be serialized, no events will be sent.
-        The chunk size is thus set to be the same size as the message backlog size.
+        No documents will be sent if there is no connection to begin with.
         Therefore, it won't result in duplicates once the the data is resent.
+        If the connection is lost during indexing, duplicate documents could be sent.
 
         Parameters
         ----------
-        error : SerializationError
-           SerializationError for the error message.
+        error : ConnectionError
+           ConnectionError for the error message.
 
         Raises
         ------
         FatalOutputError
             This causes a pipeline rebuild and gives an appropriate error log message.
 
         """
-        raise FatalOutputError(self, f"{error.args[1]} in document {error.args[0]}")
+        raise FatalOutputError(self, error.error)
 
-    def store(self, document: dict) -> bool:
-        """Store a document in the index.
+    def _handle_bulk_index_error(self, error: helpers.BulkIndexError):
+        """Handle bulk indexing error for elasticsearch bulk indexing.
+
+        Documents that could not be sent to elastiscsearch due to index errors are collected and
+        sent into an error index that should always accept all documents.
+        This can lead to a rebuild of the pipeline if this causes another exception.
 
         Parameters
         ----------
-        document : dict
-           Document to store.
+        error : BulkIndexError
+           BulkIndexError to collect IndexErrors from.
 
-        Returns
-        -------
-        Returns True to inform the pipeline to call the batch_finished_callback method in the
-        configured input
         """
-        if document.get("_index") is None:
-            document = self._build_failed_index_document(document, "Missing index in document")
+        error_documents = []
+        for bulk_error in error.errors:
+            _, error_info = bulk_error.popitem()
+            data = error_info.get("data") if "data" in error_info else None
+            error_type = error_info.get("error").get("type")
+            error_reason = error_info.get("error").get("reason")
+            reason = f"{error_type}: {error_reason}"
+            error_document = self._build_failed_index_document(data, reason)
+            self._add_dates(error_document)
+            error_documents.append(error_document)
+        self._bulk(self._search_context, error_documents)
 
-        self._add_dates(document)
-        self.metrics.number_of_processed_events += 1
-        self._write_to_search_context(document)
+    def _handle_transport_error(self, error: search.exceptions.TransportError):
+        """Handle transport error for elasticsearch bulk indexing.
 
-    def _build_failed_index_document(self, message_document: dict, reason: str):
-        document = {
-            "reason": reason,
-            "@timestamp": TimeParser.now().isoformat(),
-            "_index": self._config.default_index,
-        }
-        try:
-            document["message"] = json.dumps(message_document)
-        except TypeError:
-            document["message"] = str(message_document)
-        return document
-
-    def store_custom(self, document: dict, target: str):
-        """Write document to Elasticsearch into the target index.
+        Discard messages that exceed the maximum size if they caused an error.
 
         Parameters
         ----------
-        document : dict
-            Document to be stored into the target index.
-        target : str
-            Index to store the document in.
-        Raises
-        ------
-        CriticalOutputError
-            Raises if any error except a BufferError occurs while writing into elasticsearch.
+        error : TransportError
+           TransportError for the error message.
 
         """
-        document["_index"] = target
-        self._add_dates(document)
-        self.metrics.number_of_processed_events += 1
-        self._write_to_search_context(document)
+        if self._config.maximum_message_size_mb is None:
+            raise error
 
-    def store_failed(self, error_message: str, document_received: dict, document_processed: dict):
-        """Write errors into error topic for documents that failed processing.
+        if self._message_exceeds_max_size_error(error):
+            (
+                messages_under_size_limit,
+                messages_over_size_limit,
+            ) = self._split_message_backlog_by_size_limit()
+
+            if len(messages_over_size_limit) == 0:
+                raise error
+
+            error_documents = self._build_messages_for_large_error_documents(
+                messages_over_size_limit
+            )
+            self._message_backlog = error_documents + messages_under_size_limit
+            self._bulk(self._search_context, self._message_backlog)
+        else:
+            raise error
+
+    def _message_exceeds_max_size_error(self, error):
+        if error.status_code == 429:
+            if error.error == "circuit_breaking_exception":
+                return True
+
+            if error.error == "rejected_execution_exception":
+                reason = error.info.get("error", {}).get("reason", {})
+                match = self._size_error_pattern.match(reason)
+                if match and int(match.group("size")) >= int(match.group("max_size")):
+                    return True
+        return False
+
+    def _split_message_backlog_by_size_limit(self):
+        messages_under_size_limit = []
+        messages_over_size_limit = []
+        total_size = 0
+        for message in self._message_backlog:
+            message_size = get_dict_size_in_byte(message)
+            if message_size < self._config.maximum_message_size_mb:
+                messages_under_size_limit.append(message)
+                total_size += message_size
+            else:
+                messages_over_size_limit.append((message, message_size))
+        return messages_under_size_limit, messages_over_size_limit
+
+    def _build_messages_for_large_error_documents(
+        self, messages_over_size_limit: List[Tuple[dict, int]]
+    ) -> List[dict]:
+        """Build error message for messages that were larger than the allowed size limit.
+
+        Only a snipped of the message is stored in the error document, since the original message
+        was too large to be written in the first place.
 
         Parameters
         ----------
-        error_message : str
-           Error message to write into Kafka document.
-        document_received : dict
-            Document as it was before processing.
-        document_processed : dict
-            Document after processing until an error occurred.
+        messages_over_size_limit : List[Tuple[dict, int]]
+           Messages that were too large with their corresponding sizes in byte.
 
         """
-        error_document = {
-            "error": error_message,
-            "original": document_received,
-            "processed": document_processed,
-            "@timestamp": TimeParser.now().isoformat(),
-            "_index": self._config.error_index,
-        }
-        self._add_dates(error_document)
-        self._write_to_search_context(error_document)
-
-    def _add_dates(self, document):
-        date_format_matches = self._replace_pattern.findall(document["_index"])
-        if date_format_matches:
-            now = TimeParser.now()
-            for date_format_match in date_format_matches:
-                formatted_date = now.strftime(date_format_match[2:-1])
-                document["_index"] = re.sub(date_format_match, formatted_date, document["_index"])
-
-    def setup(self):
-        super().setup()
-        flush_timeout = self._config.flush_timeout
-        self._schedule_task(task=self._write_backlog, seconds=flush_timeout)
-        try:
-            self._search_context.info()
-        except (ElasticsearchException, OpenSearchException, TimeoutError) as error:
-            raise FatalOutputError(self, error) from error
+        error_documents = []
+        for message, size in messages_over_size_limit:
+            error_message = (
+                f"Discarded message that is larger than the allowed size limit "
+                f"({size / 10 ** 6} MB/{self._config.maximum_message_size_mb} MB)"
+            )
+            self._logger.warning(error_message)
+
+            error_document = {
+                "processed_snipped": f'{self._encoder.encode(message).decode("utf-8")[:1000]} ...',
+                "error": error_message,
+                "@timestamp": TimeParser.now().isoformat(),
+                "_index": self._config.error_index,
+            }
+            self._add_dates(error_document)
+            error_documents.append(error_document)
+        return error_documents
```

### Comparing `logprep-6.6.0/logprep/connector/file/input.py` & `logprep-6.7.0/logprep/connector/file/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/http/input.py` & `logprep-6.7.0/logprep/connector/http/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/json/input.py` & `logprep-6.7.0/logprep/connector/json/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/jsonl/input.py` & `logprep-6.7.0/logprep/connector/jsonl/input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/jsonl/output.py` & `logprep-6.7.0/logprep/connector/jsonl/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/connector/opensearch/output.py` & `logprep-6.7.0/logprep/connector/opensearch/output.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,9 +72,11 @@
             helpers.bulk(*args, **kwargs)
         except search.SerializationError as error:
             self._handle_serialization_error(error)
         except search.ConnectionError as error:
             self._handle_connection_error(error)
         except helpers.BulkIndexError as error:
             self._handle_bulk_index_error(error)
+        except search.exceptions.TransportError as error:
+            self._handle_transport_error(error)
         if self.input_connector:
             self.input_connector.batch_finished_callback()
```

### Comparing `logprep-6.6.0/logprep/connector/s3/output.py` & `logprep-6.7.0/logprep/connector/s3/output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/factory.py` & `logprep-6.7.0/logprep/factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/factory_error.py` & `logprep-6.7.0/logprep/factory_error.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/filter/expression/filter_expression.py` & `logprep-6.7.0/logprep/filter/expression/filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/filter/lucene_filter.py` & `logprep-6.7.0/logprep/filter/lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/framework/pipeline.py` & `logprep-6.7.0/logprep/framework/pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/framework/pipeline_manager.py` & `logprep-6.7.0/logprep/framework/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/framework/rule_tree/node.py` & `logprep-6.7.0/logprep/framework/rule_tree/node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/framework/rule_tree/rule_parser.py` & `logprep-6.7.0/logprep/framework/rule_tree/rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/framework/rule_tree/rule_tree.py` & `logprep-6.7.0/logprep/framework/rule_tree/rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/metrics/metric.py` & `logprep-6.7.0/logprep/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/metrics/metric_exposer.py` & `logprep-6.7.0/logprep/metrics/metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/metrics/metric_targets.py` & `logprep-6.7.0/logprep/metrics/metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/amides/detection.py` & `logprep-6.7.0/logprep/processor/amides/detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/amides/features.py` & `logprep-6.7.0/logprep/processor/amides/features.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/amides/normalize.py` & `logprep-6.7.0/logprep/processor/amides/normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/amides/processor.py` & `logprep-6.7.0/logprep/processor/amides/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/amides/rule.py` & `logprep-6.7.0/logprep/processor/amides/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/base/exceptions.py` & `logprep-6.7.0/logprep/processor/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/base/rule.py` & `logprep-6.7.0/logprep/processor/base/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/calculator/fourFn.py` & `logprep-6.7.0/logprep/processor/calculator/fourFn.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/calculator/processor.py` & `logprep-6.7.0/logprep/processor/calculator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/calculator/rule.py` & `logprep-6.7.0/logprep/processor/calculator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/clusterer/processor.py` & `logprep-6.7.0/logprep/processor/clusterer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/clusterer/rule.py` & `logprep-6.7.0/logprep/processor/clusterer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/clusterer/signature_calculation/signature_phase.py` & `logprep-6.7.0/logprep/processor/clusterer/signature_calculation/signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/concatenator/processor.py` & `logprep-6.7.0/logprep/processor/concatenator/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/concatenator/rule.py` & `logprep-6.7.0/logprep/processor/concatenator/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/datetime_extractor/processor.py` & `logprep-6.7.0/logprep/processor/datetime_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/datetime_extractor/rule.py` & `logprep-6.7.0/logprep/processor/datetime_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/deleter/processor.py` & `logprep-6.7.0/logprep/processor/deleter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/deleter/rule.py` & `logprep-6.7.0/logprep/processor/deleter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/dissector/processor.py` & `logprep-6.7.0/logprep/processor/dissector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/dissector/rule.py` & `logprep-6.7.0/logprep/processor/dissector/rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
 STRIP_CHAR = r"(-\((?P<strip>.)\))?"
 SEPERATOR = r"(\((?P<separator>\\\)|[^)]+)\))?"
 TARGET_FIELD = r"(?P<target_field>[^\/\|-]*)"
 POSITION = r"(\/(?P<position>\d*))?"
 DATATYPE = r"(\|(?P<datatype>int|float|bool))?"
 SECTION_MATCH = rf"{START}{ACTION}{SEPERATOR}{TARGET_FIELD}{STRIP_CHAR}{POSITION}{DATATYPE}{END}(?P<delimiter>.*)"
 
-MAPPING_VALIDATION_REGEX = re.compile(rf"^({DELIMITER})?({DISSECT}{DELIMITER})+({DISSECT})?$")
+MAPPING_VALIDATION_REGEX = re.compile(rf"^({DELIMITER})?({DISSECT}({DELIMITER})?)+({DISSECT})?$")
 
 
 def _do_nothing(*_):
     return
 
 
 def str_to_bool(input_str: str) -> bool:
```

### Comparing `logprep-6.6.0/logprep/processor/domain_label_extractor/processor.py` & `logprep-6.7.0/logprep/processor/domain_label_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/domain_label_extractor/rule.py` & `logprep-6.7.0/logprep/processor/domain_label_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/domain_resolver/processor.py` & `logprep-6.7.0/logprep/processor/domain_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/domain_resolver/rule.py` & `logprep-6.7.0/logprep/processor/domain_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/dropper/processor.py` & `logprep-6.7.0/logprep/processor/dropper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/dropper/rule.py` & `logprep-6.7.0/logprep/processor/dropper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/field_manager/processor.py` & `logprep-6.7.0/logprep/processor/field_manager/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/field_manager/rule.py` & `logprep-6.7.0/logprep/processor/field_manager/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/generic_adder/mysql_connector.py` & `logprep-6.7.0/logprep/processor/generic_adder/mysql_connector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/generic_adder/processor.py` & `logprep-6.7.0/logprep/processor/generic_adder/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/generic_adder/rule.py` & `logprep-6.7.0/logprep/processor/generic_adder/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/generic_resolver/processor.py` & `logprep-6.7.0/logprep/processor/generic_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/generic_resolver/rule.py` & `logprep-6.7.0/logprep/processor/generic_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/geoip_enricher/processor.py` & `logprep-6.7.0/logprep/processor/geoip_enricher/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/geoip_enricher/rule.py` & `logprep-6.7.0/logprep/processor/geoip_enricher/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/grokker/processor.py` & `logprep-6.7.0/logprep/processor/grokker/processor.py`

 * *Files 11% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import re
 from pathlib import Path
 from zipfile import ZipFile
 
 from attrs import define, field, validators
 
 from logprep.abc.processor import Processor
-from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning
+from logprep.processor.base.exceptions import FieldExistsWarning, ProcessingWarning, ProcessingError
 from logprep.processor.grokker.rule import GrokkerRule
 from logprep.util.getter import GetterFactory
 from logprep.util.helper import add_field_to, get_dotted_field_value
 
 
 class Grokker(Processor):
     """A processor that dissects a message by grok patterns"""
@@ -65,15 +65,22 @@
         matches = []
         for dotted_field, grok in rule.actions.items():
             field_value = get_dotted_field_value(event, dotted_field)
             if field_value is None:
                 error = BaseException(f"{self.name}: missing source_field: '{dotted_field}'")
                 self._handle_warning_error(event=event, rule=rule, error=error)
                 continue
-            result = grok.match(field_value)
+            try:
+                result = grok.match(field_value)
+            except TimeoutError as error:
+                raise ProcessingError(
+                    self,
+                    f"Grok pattern timeout for source field: '{dotted_field}' in rule '{rule}', "
+                    f"the grok pattern might be too complex.",
+                ) from error
             if result is None or result == {}:
                 continue
             matches.append(True)
             for dotted_field, value in result.items():
                 if value is None:
                     continue
                 success = add_field_to(
```

### Comparing `logprep-6.6.0/logprep/processor/grokker/rule.py` & `logprep-6.7.0/logprep/processor/grokker/rule.py`

 * *Files 8% similar despite different names*

```diff
@@ -114,14 +114,17 @@
         The value can be a list of search patterns or a single search pattern.
         Lists of search pattern will be checked in the order of the list until the first matching
         pattern.
         It is possible to use `oniguruma` regex pattern with or without grok patterns in the
         patterns part. When defining an `oniguruma` there is a limitation of three nested
         parentheses inside the pattern. Applying more nested parentheses is not possible.  
         Logstashs ecs conform grok patterns are used to resolve the here used grok patterns.
+        When writing patterns it is advised to be careful as the underlying regex can become complex
+        fast. If the execution and the resolving of the pattern takes more than one second a
+        matching timeout will be raised.
         """
         patterns: dict = field(
             validator=[
                 validators.instance_of(dict),
                 validators.deep_mapping(
                     key_validator=validators.instance_of(str),
                     value_validator=validators.instance_of(str),
```

### Comparing `logprep-6.6.0/logprep/processor/hyperscan_resolver/processor.py` & `logprep-6.7.0/logprep/processor/hyperscan_resolver/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/hyperscan_resolver/rule.py` & `logprep-6.7.0/logprep/processor/hyperscan_resolver/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/ip_informer/processor.py` & `logprep-6.7.0/logprep/processor/ip_informer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/ip_informer/rule.py` & `logprep-6.7.0/logprep/processor/ip_informer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/key_checker/processor.py` & `logprep-6.7.0/logprep/processor/key_checker/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/key_checker/rule.py` & `logprep-6.7.0/logprep/processor/key_checker/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/labeler/labeling_schema.py` & `logprep-6.7.0/logprep/processor/labeler/labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/labeler/processor.py` & `logprep-6.7.0/logprep/processor/labeler/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/labeler/rule.py` & `logprep-6.7.0/logprep/processor/labeler/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/list_comparison/processor.py` & `logprep-6.7.0/logprep/processor/list_comparison/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/list_comparison/rule.py` & `logprep-6.7.0/logprep/processor/list_comparison/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/normalizer/processor.py` & `logprep-6.7.0/logprep/processor/normalizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/normalizer/rule.py` & `logprep-6.7.0/logprep/processor/normalizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pre_detector/ip_alerter.py` & `logprep-6.7.0/logprep/processor/pre_detector/ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pre_detector/processor.py` & `logprep-6.7.0/logprep/processor/pre_detector/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pre_detector/rule.py` & `logprep-6.7.0/logprep/processor/pre_detector/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/processor_strategy.py` & `logprep-6.7.0/logprep/processor/processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pseudonymizer/encrypter.py` & `logprep-6.7.0/logprep/processor/pseudonymizer/encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pseudonymizer/processor.py` & `logprep-6.7.0/logprep/processor/pseudonymizer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/pseudonymizer/rule.py` & `logprep-6.7.0/logprep/processor/pseudonymizer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/requester/processor.py` & `logprep-6.7.0/logprep/processor/requester/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/requester/rule.py` & `logprep-6.7.0/logprep/processor/requester/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/selective_extractor/processor.py` & `logprep-6.7.0/logprep/processor/selective_extractor/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/selective_extractor/rule.py` & `logprep-6.7.0/logprep/processor/selective_extractor/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/string_splitter/processor.py` & `logprep-6.7.0/logprep/processor/string_splitter/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/string_splitter/rule.py` & `logprep-6.7.0/logprep/processor/string_splitter/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/template_replacer/processor.py` & `logprep-6.7.0/logprep/processor/template_replacer/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/template_replacer/rule.py` & `logprep-6.7.0/logprep/processor/template_replacer/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/timestamp_differ/processor.py` & `logprep-6.7.0/logprep/processor/timestamp_differ/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/timestamp_differ/rule.py` & `logprep-6.7.0/logprep/processor/timestamp_differ/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/timestamper/processor.py` & `logprep-6.7.0/logprep/processor/timestamper/processor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/processor/timestamper/rule.py` & `logprep-6.7.0/logprep/processor/timestamper/rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/registry.py` & `logprep-6.7.0/logprep/registry.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/run_logprep.py` & `logprep-6.7.0/logprep/run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/runner.py` & `logprep-6.7.0/logprep/runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/aggregating_logger.py` & `logprep-6.7.0/logprep/util/aggregating_logger.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py` & `logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_corpus_tester.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,17 +74,20 @@
 
 If during the test run logprep has an error or warning it logs it to the console as well, which will
 be printed inside the test cases summary and before the summary result of the test, which created
 the log message.
 
 If one or more test cases fail this tester ends with an exit code of 1, otherwise 0.
 """
+import io
+
 # pylint: enable=anomalous-backslash-in-string
 # pylint: disable=protected-access
 import json
+import logging
 import os
 import re
 import shutil
 import sys
 import tempfile
 from functools import cached_property
 from json import JSONDecodeError
@@ -140,18 +143,20 @@
         input_document: dict = field(validator=validators.instance_of(dict), default={})
         expected_output: dict = field(validator=validators.instance_of(dict), default={})
         expected_extra_output: dict = field(validator=validators.instance_of(list), default=[])
         generated_output: dict = field(validator=validators.instance_of(dict), default={})
         generated_extra_output: dict = field(validator=validators.instance_of(list), default=[])
         failed: bool = field(validator=validators.instance_of(bool), default=False)
         report: List = Factory(list)
+        warnings: str = field(default="")
 
     def __init__(self, config_path, input_test_data_path):
         self._original_config_path = config_path
         self._input_test_data_path = input_test_data_path
+        self.log_capture_string = None
 
     @cached_property
     def _tmp_dir(self):
         return tempfile.mkdtemp()
 
     @cached_property
     def _test_cases(self):
@@ -165,25 +170,37 @@
             raise ValueError(f"Following parsing errors were found: {parsing_errors}")
         no_input_files = [case for case in test_cases if not test_cases[case].input_document]
         if no_input_files:
             raise ValueError(f"The following TestCases have no input documents: {no_input_files}")
         return dict(sorted(test_cases.items()))
 
     @cached_property
+    def _logprep_logger(self):
+        logprep_logger = getLogger("logprep-rule-corpus-tester")
+        logprep_logger.propagate = False
+        logprep_logger.setLevel(logging.WARNING)
+        self.log_capture_string = io.StringIO()
+        self.stream_handler = logging.StreamHandler(self.log_capture_string)
+        self.stream_handler.setLevel(logging.WARNING)
+        logprep_logger.addHandler(self.stream_handler)
+        return logprep_logger
+
+    @cached_property
     def _pipeline(self):
         merged_input_file_path = Path(self._tmp_dir) / "input.json"
         inputs = [test_case.input_document for test_case in self._test_cases.values()]
         merged_input_file_path.write_text(json.dumps(inputs), encoding="utf8")
         path_to_patched_config = Configuration.patch_yaml_with_json_connectors(
             self._original_config_path, self._tmp_dir, str(merged_input_file_path)
         )
         config = Configuration.create_from_yaml(path_to_patched_config)
         config.verify_pipeline_without_processor_outputs(getLogger("logprep"))
         del config["output"]
         pipeline = Pipeline(config=config)
+        pipeline.logger = self._logprep_logger
         return pipeline
 
     def run(self):
         """
         Starts the test routine by reading all input files, patching the logprep pipline, executing
         the pipeline for each input event, comparing the generated output with the expected output
         and printing out the test results.
@@ -202,21 +219,32 @@
         For each test case the logprep connector files are rewritten (only the current test case
         will be added to the input file), the pipline is run and the outputs are compared.
         """
         print(Style.BRIGHT + "# Test Cases Summary:" + Style.RESET_ALL)
         for test_case_id, test_case in self._test_cases.items():
             _ = [processor.setup() for processor in self._pipeline._pipeline]
             parsed_event, extra_outputs = self._pipeline.process_pipeline()
+            test_case.warnings = self._retrieve_log_capture()
             extra_outputs = align_extra_output_formats(extra_outputs)
             test_case.generated_output = parsed_event
             test_case.generated_extra_output = extra_outputs
             self._compare_logprep_outputs(test_case_id, parsed_event)
             self._compare_extra_data_output(test_case_id, extra_outputs)
             self._print_pass_fail_statements(test_case_id)
 
+    def _retrieve_log_capture(self):
+        log_capture = self.log_capture_string.getvalue()
+        # set new log_capture to clear previous entries
+        self.log_capture_string = io.StringIO()
+        self.stream_handler = logging.StreamHandler(self.log_capture_string)
+        self.stream_handler.setLevel(logging.WARNING)
+        self._logprep_logger.handlers.clear()
+        self._logprep_logger.addHandler(self.stream_handler)
+        return log_capture
+
     def _compare_logprep_outputs(self, test_case_id, logprep_output):
         test_case = self._test_cases.get(test_case_id, {})
         if test_case.expected_output:
             diff = self._compare_events(logprep_output, test_case.expected_output)
             self._extract_print_statements_from_diff(test_case_id, diff)
 
     def _compare_extra_data_output(self, test_case_id, logprep_extra_outputs):
@@ -315,37 +343,49 @@
     def _print_pass_fail_statements(self, test_case_id):
         test_case = self._test_cases.get(test_case_id, {})
         status = f"{Style.BRIGHT}{Fore.GREEN} PASSED"
         if not test_case.expected_output:
             status = f"{Style.BRIGHT}{Fore.RESET} SKIPPED - (no expected output given)"
         elif len(test_case.report) > 0:
             status = f"{Style.BRIGHT}{Fore.RED} FAILED"
+        elif test_case.warnings:
+            status = f"{Style.BRIGHT}{Fore.YELLOW} PASSED - (with warnings)"
+
         print(f"{Fore.BLUE} Test Case: {Fore.CYAN}{test_case_id} {status}{Style.RESET_ALL}")
 
     def _print_test_reports(self):
         if not any(case.failed for case in self._test_cases.values()):
             return
         print(Style.BRIGHT + "# Test Cases Detailed Reports:" + Style.RESET_ALL)
         for test_case_id, test_case in self._test_cases.items():
-            if test_case.report and test_case.expected_output:
+            if (test_case.warnings or test_case.report) and test_case.expected_output:
                 self._print_long_test_result(test_case_id, test_case)
                 print()
 
     def _print_long_test_result(self, test_case_id, test_case):
         report_title = f"test report for '{test_case_id}'"
         print(f"{Fore.RED}{Style.BRIGHT}↓ {report_title} ↓ {Style.RESET_ALL}")
+        print_logprep_output = True
+        if test_case.warnings and not test_case.report:
+            print(Fore.GREEN + "Test passed, but with following warnings:" + Fore.RESET)
+            print(test_case.warnings)
+            print_logprep_output = False
+        if test_case.warnings and test_case.report:
+            print(Fore.RED + "Logprep Warnings:" + Fore.RESET)
+            print(test_case.warnings)
         for statement in test_case.report:
             if isinstance(statement, (dict, list)):
                 pprint(statement)
             else:
                 print(statement)
-        print(Fore.RED + "Logprep Event Output:" + Fore.RESET)
-        pprint(test_case.generated_output)
-        print(Fore.RED + "Logprep Extra Data Output:" + Fore.RESET)
-        pprint(test_case.generated_extra_output)
+        if print_logprep_output:
+            print(Fore.RED + "Logprep Event Output:" + Fore.RESET)
+            pprint(test_case.generated_output)
+            print(Fore.RED + "Logprep Extra Data Output:" + Fore.RESET)
+            pprint(test_case.generated_extra_output)
         print(f"{Fore.RED}{Style.BRIGHT}↑ {report_title} ↑ {Style.RESET_ALL}")
 
     def _print_test_summary(self):
         print(Fore.RESET + Style.BRIGHT + "# Test Overview" + Style.RESET_ALL)
         total_cases = len(self._test_cases)
         failed_cases = sum(case.failed for case in self._test_cases.values())
         print(f"Failed tests: {failed_cases}")
```

### Comparing `logprep-6.6.0/logprep/util/auto_rule_tester/auto_rule_tester.py` & `logprep-6.7.0/logprep/util/auto_rule_tester/auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py` & `logprep-6.7.0/logprep/util/auto_rule_tester/grok_pattern_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/cache.py` & `logprep-6.7.0/logprep/util/cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/configuration.py` & `logprep-6.7.0/logprep/util/configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/decorators.py` & `logprep-6.7.0/logprep/util/decorators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/getter.py` & `logprep-6.7.0/logprep/util/getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/grok.py` & `logprep-6.7.0/logprep/util/grok/grok.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,16 @@
 from pathlib import Path
 from re import error
 
 import numpy as np
 import pkg_resources
 from attrs import define, field, validators
 
+from logprep.util.decorators import timeout
+
 if sys.version_info.minor < 11:
     # because needed possessive quantifiers and atomic grouping
     # added to re module in python 3.11
     import regex as re  # pylint: disable=shadowed-import
 
 DEFAULT_PATTERNS_DIRS = [pkg_resources.resource_filename(__name__, "patterns/ecs-v1")]
 
@@ -76,14 +78,15 @@
             custom_pats[pat_name] = Pattern(pat_name, regex_str)
 
         if len(custom_pats) > 0:
             self.predefined_patterns.update(custom_pats)
 
         self._load_search_pattern()
 
+    @timeout(seconds=1)
     def match(self, text):
         """If text is matched with pattern, return variable names
         specified(%{pattern:variable name}) in pattern and their
         corresponding values. If not matched, return None.
         custom patterns can be passed in by
         custom_patterns(pattern name, pattern regular expression pair)
         or custom_patterns_dir.
```

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/aws` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bacula` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bind` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bind`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/bro` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/exim` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/firewalls` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/grok-patterns` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/haproxy` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/httpd` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/java` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/java`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/junos` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/linux-syslog` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/mongodb` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/nagios` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/rails` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/squid` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/squid`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/ecs-v1/zeek` & `logprep-6.7.0/logprep/util/grok/patterns/ecs-v1/zeek`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/aws` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/aws`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/bacula` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/bacula`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/bro` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/bro`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/exim` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/exim`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/firewalls` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/firewalls`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/grok-patterns` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/grok-patterns`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/haproxy` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/haproxy`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/httpd` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/httpd`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/java` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/java`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/junos` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/junos`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/linux-syslog` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/linux-syslog`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/mongodb` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/mongodb`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/nagios` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/nagios`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok/patterns/legacy/rails` & `logprep-6.7.0/logprep/util/grok/patterns/legacy/rails`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/grok_pattern_loader.py` & `logprep-6.7.0/logprep/util/grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/hasher.py` & `logprep-6.7.0/logprep/util/hasher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/helper.py` & `logprep-6.7.0/logprep/util/helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """This module contains helper functions that are shared by different modules."""
 import re
+import sys
 from functools import lru_cache, partial, reduce
 from os import remove
 from typing import Optional, Union
 
 from colorama import Back, Fore
 from colorama.ansi import AnsiBack, AnsiFore
 
@@ -290,7 +291,20 @@
 
 def get_source_fields_dict(event, rule):
     """returns a dict with dotted fields as keys and target values as values"""
     source_fields = rule.source_fields
     source_field_values = map(partial(get_dotted_field_value, event), source_fields)
     source_field_dict = dict(zip(source_fields, source_field_values))
     return source_field_dict
+
+
+def get_dict_size_in_byte(dictionary: dict) -> int:
+    """returns the size of a nested dictionary in bytes"""
+    size = sys.getsizeof(dictionary)
+    if isinstance(dictionary, dict):
+        keys_size = sum(map(get_dict_size_in_byte, dictionary.keys()))
+        values_size = sum(map(get_dict_size_in_byte, dictionary.values()))
+        return size + keys_size + values_size
+    if isinstance(dictionary, list):
+        elements_size = sum(map(get_dict_size_in_byte, dictionary))
+        return size + elements_size
+    return size
```

### Comparing `logprep-6.6.0/logprep/util/json_handling.py` & `logprep-6.7.0/logprep/util/json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/log_aggregator.py` & `logprep-6.7.0/logprep/util/log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/multiprocessing_log_handler.py` & `logprep-6.7.0/logprep/util/multiprocessing_log_handler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/pipeline_profiler.py` & `logprep-6.7.0/logprep/util/pipeline_profiler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/pre_detector_rule_matching_tester.py` & `logprep-6.7.0/logprep/util/pre_detector_rule_matching_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/processor_generator.py` & `logprep-6.7.0/logprep/util/processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/prometheus_exporter.py` & `logprep-6.7.0/logprep/util/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/rule_dry_runner.py` & `logprep-6.7.0/logprep/util/rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/schema_and_rule_checker.py` & `logprep-6.7.0/logprep/util/schema_and_rule_checker.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/time.py` & `logprep-6.7.0/logprep/util/time.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,33 @@
     """exception class for time parsing"""
 
 
 class TimeParser:
     """encapsulation of time related methods"""
 
     @classmethod
-    def from_string(cls, source: str) -> datetime:
+    def from_string(cls, source: str, set_missing_utc: bool = True) -> datetime:
         """parses input string to datetime object
 
         Parameters
         ----------
         source : str
             input string
+        set_missing_utc : bool
+            Set timezone to utc if it is missing and this is true
 
         Returns
         -------
         datetime
             datetime object
         """
         try:
             time_object = ciso8601.parse_datetime(source)  # pylint: disable=c-extension-no-member
-            time_object = cls._set_utc_if_timezone_is_missing(time_object)
+            if set_missing_utc:
+                time_object = cls._set_utc_if_timezone_is_missing(time_object)
             return time_object
         except ValueError as error:
             raise TimeParserException(str(error)) from error
 
     @classmethod
     def from_timestamp(cls, timestamp: Union[int, float]) -> datetime:
         """get datetime from unix timestamp
@@ -64,50 +67,53 @@
             current date and time as datetime
         """
         time_object = datetime.now()
         time_object = cls._set_utc_if_timezone_is_missing(time_object)
         return time_object
 
     @classmethod
-    def from_format(cls, source: str, format_str: str) -> datetime:
+    def from_format(cls, source: str, format_str: str, set_missing_utc: bool = True) -> datetime:
         """parse date from format
 
         Parameters
         ----------
         source : str
             the date string
         format_str : str
             the format string
+        set_missing_utc : bool
+            Set timezone to utc if it is missing and this is true
 
         Returns
         -------
         datetime
             the datetime object
 
         Raises
         ------
         TimeParserException
             raised if something could not be parsed
         """
         try:
             time_object = datetime.strptime(source, format_str)
-            time_object = cls._set_utc_if_timezone_is_missing(time_object)
+            if set_missing_utc:
+                time_object = cls._set_utc_if_timezone_is_missing(time_object)
             return time_object
         except ValueError as error:
             raise TimeParserException(str(error)) from error
 
     @classmethod
     def _set_utc_if_timezone_is_missing(cls, time_object):
         if time_object.tzinfo is None:
             time_object = time_object.replace(tzinfo=UTC)
         return time_object
 
     @classmethod
     def parse_datetime(
-        cls, timestamp: str, source_format: str, source_timezone: [str, tzinfo]
+        cls, timestamp: str, source_format: str, source_timezone: Union[str, tzinfo]
     ) -> datetime:
         """
         Parses a timestamp based on different formats, besides a format string 'ISO8601' and
         'UNIX' are allowed formats.
 
         Parameters
         ----------
@@ -120,15 +126,21 @@
 
 
         Returns
         -------
         datetime
             The parsed timestamp as datetime object.
         """
-        if source_format == "ISO8601":
-            parsed_datetime = cls.from_string(timestamp).astimezone(source_timezone)
-        elif source_format == "UNIX":
+        if source_format == "UNIX":
             parsed_datetime = int(timestamp) if len(timestamp) <= 10 else int(timestamp) / 1000
-            parsed_datetime = cls.from_timestamp(parsed_datetime).astimezone(source_timezone)
+            parsed_datetime = cls.from_timestamp(parsed_datetime)
+        elif source_format == "ISO8601":
+            parsed_datetime = cls.from_string(timestamp, set_missing_utc=False)
         else:
-            parsed_datetime = cls.from_format(timestamp, source_format).astimezone(source_timezone)
+            parsed_datetime = cls.from_format(timestamp, source_format, set_missing_utc=False)
+            if parsed_datetime.year == 1900:
+                parsed_datetime = parsed_datetime.replace(year=datetime.now().year)
+
+        if parsed_datetime.tzinfo is None:
+            parsed_datetime = parsed_datetime.replace(tzinfo=source_timezone)
+
         return parsed_datetime
```

### Comparing `logprep-6.6.0/logprep/util/time_measurement.py` & `logprep-6.7.0/logprep/util/time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep/util/validators.py` & `logprep-6.7.0/logprep/util/validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/logprep.egg-info/PKG-INFO` & `logprep-6.7.0/logprep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logprep
-Version: 6.6.0
+Version: 6.7.0
 Summary: Logprep allows to collect, process and forward log messages from various data sources.
 Home-page: https://github.com/fkie-cad/Logprep
 Author: Logprep Team
 License: LGPL-2.1 license
 Project-URL: Homepage, https://github.com/fkie-cad/Logprep
 Project-URL: Documentation, https://logprep.readthedocs.io/en/latest/
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: logprep Version: 6.6.0 Summary: Logprep allows to
+Metadata-Version: 2.1 Name: logprep Version: 6.7.0 Summary: Logprep allows to
 collect, process and forward log messages from various data sources. Home-page:
 https://github.com/fkie-cad/Logprep Author: Logprep Team License: LGPL-2.1
 license Project-URL: Homepage, https://github.com/fkie-cad/Logprep Project-URL:
 Documentation, https://logprep.readthedocs.io/en/latest/ Platform: UNKNOWN
 Classifier: Programming Language :: Python Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

### Comparing `logprep-6.6.0/logprep.egg-info/SOURCES.txt` & `logprep-6.7.0/logprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/setup.py` & `logprep-6.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_amides.py` & `logprep-6.7.0/tests/acceptance/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_config_refresh.py` & `logprep-6.7.0/tests/acceptance/test_config_refresh.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_file_input.py` & `logprep-6.7.0/tests/acceptance/test_file_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_full_configuration.py` & `logprep-6.7.0/tests/acceptance/test_full_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_http_input.py` & `logprep-6.7.0/tests/acceptance/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_multiple_outputs.py` & `logprep-6.7.0/tests/acceptance/test_multiple_outputs.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_pre_detection.py` & `logprep-6.7.0/tests/acceptance/test_pre_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_preprocessing.py` & `logprep-6.7.0/tests/acceptance/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py` & `logprep-6.7.0/tests/acceptance/test_selective_extractor_full_pipeline_pass.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_wineventlog_normalization.py` & `logprep-6.7.0/tests/acceptance/test_wineventlog_normalization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_wineventlog_processing.py` & `logprep-6.7.0/tests/acceptance/test_wineventlog_processing.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/test_wineventlog_pseudonymization.py` & `logprep-6.7.0/tests/acceptance/test_wineventlog_pseudonymization.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/acceptance/util.py` & `logprep-6.7.0/tests/acceptance/util.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/ci/runner-image/scripts/compare_json.py` & `logprep-6.7.0/tests/ci/runner-image/scripts/compare_json.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/testdata/ConfigurationForTest.py` & `logprep-6.7.0/tests/testdata/ConfigurationForTest.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/testdata/FilledTempFile.py` & `logprep-6.7.0/tests/testdata/FilledTempFile.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/testdata/metadata.py` & `logprep-6.7.0/tests/testdata/metadata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/testdata/ruledata.py` & `logprep-6.7.0/tests/testdata/ruledata.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/testdata/unit/clusterer/test_data.py` & `logprep-6.7.0/tests/testdata/unit/clusterer/test_data.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/component/base.py` & `logprep-6.7.0/tests/unit/component/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/base.py` & `logprep-6.7.0/tests/unit/connector/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_common.py` & `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_common.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_input.py` & `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_confluent_kafka_output.py` & `logprep-6.7.0/tests/unit/connector/test_confluent_kafka_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_console_output.py` & `logprep-6.7.0/tests/unit/connector/test_console_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_dummy_input.py` & `logprep-6.7.0/tests/unit/connector/test_dummy_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_dummy_output.py` & `logprep-6.7.0/tests/unit/connector/test_dummy_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_elasticsearch_output.py` & `logprep-6.7.0/tests/unit/connector/test_elasticsearch_output.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # pylint: disable=attribute-defined-outside-init
-# pylint: disable=no-self-use
+# pylint: disable=too-many-arguments
 import json
 import re
 from datetime import datetime
 from math import isclose
 from unittest import mock
 
 import elasticsearch as search
@@ -158,15 +158,15 @@
     def test_write_to_search_context_calls_handle_bulk_index_error_if_bulk_index_error(self, _):
         self.object._config.message_backlog_size = 1
         self.object._handle_bulk_index_error = mock.MagicMock()
         self.object._write_to_search_context({"dummy": "event"})
         self.object._handle_bulk_index_error.assert_called()
 
     @mock.patch("elasticsearch.helpers.bulk")
-    def test__handle_bulk_index_error_calls_bulk(self, fake_bulk):
+    def test_handle_bulk_index_error_calls_bulk(self, fake_bulk):
         mock_bulk_index_error = mock.MagicMock()
         mock_bulk_index_error.errors = [
             {
                 "index": {
                     "data": {"my": "document"},
                     "error": {"type": "myerrortype", "reason": "myreason"},
                 }
@@ -192,14 +192,139 @@
         assert "reason" in error_document
         assert "@timestamp" in error_document
         assert "_index" in error_document
         assert "message" in error_document
         assert error_document.get("reason") == "myerrortype: myreason"
         assert error_document.get("message") == json.dumps({"my": "document"})
 
+    @pytest.mark.parametrize(
+        "status_code, error, error_info, messages, discarded_cnt, exception",
+        [
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "bar"}, {"bar": "baz"}],
+                0,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}, {"bar": "baz"}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}, {"bar": "*" * 500}],
+                2,
+                None,
+            ),
+            (
+                123,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "wrong_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {"invalid": "error"},
+                [{"foo": "*" * 500}],
+                1,
+                TypeError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {"error": {"reason": "wrong_reason"}},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {
+                    "error": {
+                        "reason": "... "
+                        "coordinating_operation_bytes=9, max_coordinating_and_primary_bytes=1 "
+                        "..."
+                    }
+                },
+                [{"foo": "*" * 500}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {
+                    "error": {
+                        "reason": "... "
+                        "coordinating_operation_bytes=1, max_coordinating_and_primary_bytes=9 "
+                        "..."
+                    }
+                },
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+        ],
+    )
+    def test_handle_transport_error_calls_bulk_with_error_documents(
+        self, status_code, error, error_info, messages, discarded_cnt, exception
+    ):
+        self.object._config.maximum_message_size_mb = 5 * 10**-4
+
+        mock_transport_error = search.exceptions.TransportError(status_code, error, error_info)
+
+        if exception:
+            with pytest.raises(exception):
+                self.object._handle_transport_error(mock_transport_error)
+        else:
+            self.object._message_backlog = messages
+            self.object._handle_transport_error(mock_transport_error)
+            above_limit = []
+            under_limit = []
+            for message in self.object._message_backlog:
+                if message.get("_index") == "error_index":
+                    assert message.get("error", "").startswith(
+                        "Discarded message that is larger than the allowed size limit"
+                    )
+                    assert len(message.get("processed_snipped", "")) <= 1000
+                    assert message.get("processed_snipped", "").endswith(" ...")
+                    above_limit.append(message)
+                else:
+                    under_limit.append(message)
+            assert len(above_limit) == discarded_cnt
+            assert len(above_limit) + len(under_limit) == len(self.object._message_backlog)
+
     def test_handle_connection_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_connection_error(mock.MagicMock())
 
     def test_handle_serialization_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_serialization_error(mock.MagicMock())
```

### Comparing `logprep-6.6.0/tests/unit/connector/test_file_input_default_config.py` & `logprep-6.7.0/tests/unit/connector/test_file_input_default_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_file_input_not_tailing_config.py` & `logprep-6.7.0/tests/unit/connector/test_file_input_not_tailing_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_file_input_start_at_end_config.py` & `logprep-6.7.0/tests/unit/connector/test_file_input_start_at_end_config.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_http_input.py` & `logprep-6.7.0/tests/unit/connector/test_http_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_json_input.py` & `logprep-6.7.0/tests/unit/connector/test_json_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_jsonl_input.py` & `logprep-6.7.0/tests/unit/connector/test_jsonl_input.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_jsonl_output.py` & `logprep-6.7.0/tests/unit/connector/test_jsonl_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/connector/test_opensearch_output.py` & `logprep-6.7.0/tests/unit/connector/test_opensearch_output.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=wrong-import-position
 # pylint: disable=wrong-import-order
 # pylint: disable=attribute-defined-outside-init
-# pylint: disable=no-self-use
+# pylint: disable=too-many-arguments
 import json
 import re
 from datetime import datetime
 from math import isclose
 from unittest import mock
 
 import opensearchpy as search
@@ -198,14 +198,139 @@
         assert "reason" in error_document
         assert "@timestamp" in error_document
         assert "_index" in error_document
         assert "message" in error_document
         assert error_document.get("reason") == "myerrortype: myreason"
         assert error_document.get("message") == json.dumps({"my": "document"})
 
+    @pytest.mark.parametrize(
+        "status_code, error, error_info, messages, discarded_cnt, exception",
+        [
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "bar"}, {"bar": "baz"}],
+                0,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}, {"bar": "baz"}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}, {"bar": "*" * 500}],
+                2,
+                None,
+            ),
+            (
+                123,
+                "circuit_breaking_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "wrong_exception",
+                {"anything": "anything"},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {"invalid": "error"},
+                [{"foo": "*" * 500}],
+                1,
+                TypeError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {"error": {"reason": "wrong_reason"}},
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {
+                    "error": {
+                        "reason": "... "
+                        "coordinating_operation_bytes=9, max_coordinating_and_primary_bytes=1 "
+                        "..."
+                    }
+                },
+                [{"foo": "*" * 500}],
+                1,
+                None,
+            ),
+            (
+                429,
+                "rejected_execution_exception",
+                {
+                    "error": {
+                        "reason": "... "
+                        "coordinating_operation_bytes=1, max_coordinating_and_primary_bytes=9 "
+                        "..."
+                    }
+                },
+                [{"foo": "*" * 500}],
+                1,
+                search.exceptions.TransportError,
+            ),
+        ],
+    )
+    def test_handle_transport_error_calls_bulk_with_error_documents(
+        self, status_code, error, error_info, messages, discarded_cnt, exception
+    ):
+        self.object._config.maximum_message_size_mb = 5 * 10**-4
+
+        mock_transport_error = search.exceptions.TransportError(status_code, error, error_info)
+
+        if exception:
+            with pytest.raises(exception):
+                self.object._handle_transport_error(mock_transport_error)
+        else:
+            self.object._message_backlog = messages
+            self.object._handle_transport_error(mock_transport_error)
+            above_limit = []
+            under_limit = []
+            for message in self.object._message_backlog:
+                if message.get("_index") == "error_index":
+                    assert message.get("error", "").startswith(
+                        "Discarded message that is larger than the allowed size limit"
+                    )
+                    assert len(message.get("processed_snipped", "")) <= 1000
+                    assert message.get("processed_snipped", "").endswith(" ...")
+                    above_limit.append(message)
+                else:
+                    under_limit.append(message)
+            assert len(above_limit) == discarded_cnt
+            assert len(above_limit) + len(under_limit) == len(self.object._message_backlog)
+
     def test_handle_connection_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_connection_error(mock.MagicMock())
 
     def test_handle_serialization_error_raises_fatal_output_error(self):
         with pytest.raises(FatalOutputError):
             self.object._handle_serialization_error(mock.MagicMock())
```

### Comparing `logprep-6.6.0/tests/unit/connector/test_s3_output.py` & `logprep-6.7.0/tests/unit/connector/test_s3_output.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/exceptions/processor/test_processing_warning.py` & `logprep-6.7.0/tests/unit/exceptions/processor/test_processing_warning.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/filter/test_filter_expression.py` & `logprep-6.7.0/tests/unit/filter/test_filter_expression.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/filter/test_lucene_filter.py` & `logprep-6.7.0/tests/unit/filter/test_lucene_filter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/framework/rule_tree/test_node.py` & `logprep-6.7.0/tests/unit/framework/rule_tree/test_node.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_parser.py` & `logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_parser.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/framework/rule_tree/test_rule_tree.py` & `logprep-6.7.0/tests/unit/framework/rule_tree/test_rule_tree.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/framework/test_pipeline.py` & `logprep-6.7.0/tests/unit/framework/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/framework/test_pipeline_manager.py` & `logprep-6.7.0/tests/unit/framework/test_pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/metrics/test_metric_exposer.py` & `logprep-6.7.0/tests/unit/metrics/test_metric_exposer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/metrics/test_metric_targets.py` & `logprep-6.7.0/tests/unit/metrics/test_metric_targets.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/metrics/test_metrics.py` & `logprep-6.7.0/tests/unit/metrics/test_metrics.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/amides/test_amides.py` & `logprep-6.7.0/tests/unit/processor/amides/test_amides.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/amides/test_amides_rule.py` & `logprep-6.7.0/tests/unit/processor/amides/test_amides_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/amides/test_detection.py` & `logprep-6.7.0/tests/unit/processor/amides/test_detection.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/amides/test_normalize.py` & `logprep-6.7.0/tests/unit/processor/amides/test_normalize.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/amides/test_tokenizer.py` & `logprep-6.7.0/tests/unit/processor/amides/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/base.py` & `logprep-6.7.0/tests/unit/processor/base.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/calculator/test_calculator.py` & `logprep-6.7.0/tests/unit/processor/calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/calculator/test_calculator_rule.py` & `logprep-6.7.0/tests/unit/processor/calculator/test_calculator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer.py` & `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_rule.py` & `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py` & `logprep-6.7.0/tests/unit/processor/clusterer/test_clusterer_signature_phase.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator.py` & `logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/concatenator/test_concatenator_rule.py` & `logprep-6.7.0/tests/unit/processor/concatenator/test_concatenator_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py` & `logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py` & `logprep-6.7.0/tests/unit/processor/datetime_extractor/test_datetime_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/deleter/test_deleter.py` & `logprep-6.7.0/tests/unit/processor/deleter/test_deleter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/deleter/test_deleter_rule.py` & `logprep-6.7.0/tests/unit/processor/deleter/test_deleter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/dissector/test_dissector.py` & `logprep-6.7.0/tests/unit/processor/dissector/test_dissector.py`

 * *Files 1% similar despite different names*

```diff
@@ -592,14 +592,38 @@
                     "message": "this is %{field1-(#)|int} message and this is %{field2-(#)|bool}"
                 }
             },
         },
         {"message": "this is 42#### message and this is 0##"},
         {"message": "this is 42#### message and this is 0##", "field1": 42, "field2": False},
     ),
+    (
+        "extract end of string",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "system_%{type}"}},
+        },
+        {"message": "system_monitor"},
+        {
+            "message": "system_monitor",
+            "type": "monitor",
+        },
+    ),
+    (
+        "copy field - dissect without separator",
+        {
+            "filter": "message",
+            "dissector": {"mapping": {"message": "%{sys_type}"}},
+        },
+        {"message": "system_monitor"},
+        {
+            "message": "system_monitor",
+            "sys_type": "system_monitor",
+        },
+    ),
 ]
 failure_test_cases = [  # testcase, rule, event, expected
     (
         "Tags failure if convert is not possible",
         {
             "filter": "message",
             "dissector": {
```

### Comparing `logprep-6.6.0/tests/unit/processor/dissector/test_dissector_rule.py` & `logprep-6.7.0/tests/unit/processor/dissector/test_dissector_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,16 +70,16 @@
                 "must match regex",
             ),
             (
                 {
                     "filter": "message",
                     "dissector": {"mapping": {"field": "%{ts}"}},
                 },
-                ValueError,
-                "must match regex",
+                None,
+                None,
             ),
             (
                 {
                     "filter": "message",
                     "dissector": {"mapping": {"field": "%{ts}:"}},
                 },
                 None,
```

### Comparing `logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py` & `logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py` & `logprep-6.7.0/tests/unit/processor/domain_label_extractor/test_domain_label_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver.py` & `logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py` & `logprep-6.7.0/tests/unit/processor/domain_resolver/test_domain_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/dropper/test_dropper.py` & `logprep-6.7.0/tests/unit/processor/dropper/test_dropper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/dropper/test_dropper_rule.py` & `logprep-6.7.0/tests/unit/processor/dropper/test_dropper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager.py` & `logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/field_manager/test_field_manager_rule.py` & `logprep-6.7.0/tests/unit/processor/field_manager/test_field_manager_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder.py` & `logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py` & `logprep-6.7.0/tests/unit/processor/generic_adder/test_generic_adder_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver.py` & `logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py` & `logprep-6.7.0/tests/unit/processor/generic_resolver/test_generic_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py` & `logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py` & `logprep-6.7.0/tests/unit/processor/geoip_enricher/test_geoip_enricher_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/grokker/test_grok.py` & `logprep-6.7.0/tests/unit/processor/grokker/test_grok.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/grokker/test_grokker.py` & `logprep-6.7.0/tests/unit/processor/grokker/test_grokker.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 from copy import deepcopy
 from unittest import mock
 
 import pytest
 
 from logprep.factory import Factory
+from logprep.processor.base.exceptions import ProcessingCriticalError
 from logprep.util.getter import GetterFactory
 from tests.unit.processor.base import BaseProcessorTestCase
 
 test_cases = [  # testcase, rule, event, expected
     (
         "matches simple grok pattern",
         {"filter": "message", "grokker": {"mapping": {"message": "this is the %{USER:userfield}"}}},
@@ -347,14 +348,28 @@
                 "event_id": 123456789,
                 "event_data": {"normalize me!": "foo 123.123.123.123 1234 bar"},
             },
             "tags": ["_grokker_failure"],
         },
         "no grok pattern matched",
     ),
+    (
+        "grok pattern timeout",
+        {
+            "filter": "url",
+            "grokker": {
+                "mapping": {
+                    "url": "^(%{URIPROTO:[network][protocol]}://)?%{IPORHOST:[url][domain]}(?::%{POSINT:[url][port]})?(?:%{URIPATHPARAM:[url][path]})?$"
+                }
+            },
+        },
+        {"url": "is-ascdwa-fv458.sdcfvfdaq.ascg:316"},
+        {"url": "is-ascdwa-fv458.sdcfvfdaq.ascg:316"},
+        ProcessingCriticalError,
+    ),
 ]  # testcase, rule, event, expected
 
 
 class TestGrokker(BaseProcessorTestCase):
     CONFIG: dict = {
         "type": "grokker",
         "specific_rules": ["tests/testdata/unit/grokker/specific_rules"],
@@ -364,24 +379,26 @@
     @pytest.mark.parametrize("testcase, rule, event, expected", test_cases)
     def test_testcases(self, testcase, rule, event, expected):
         self._load_specific_rule(rule)
         self.object.setup()
         self.object.process(event)
         assert event == expected, testcase
 
-    @pytest.mark.parametrize("testcase, rule, event, expected, error_message", failure_test_cases)
-    def test_testcases_failure_handling(
-        self, caplog, testcase, rule, event, expected, error_message
-    ):
+    @pytest.mark.parametrize("testcase, rule, event, expected, error", failure_test_cases)
+    def test_testcases_failure_handling(self, caplog, testcase, rule, event, expected, error):
         self._load_specific_rule(rule)
         self.object.setup()
-        with caplog.at_level(logging.WARNING):
-            self.object.process(event)
-            assert re.match(rf".*{error_message}", caplog.text)
-        assert event == expected, testcase
+        if isinstance(error, str):
+            with caplog.at_level(logging.WARNING):
+                self.object.process(event)
+                assert re.match(rf".*{error}", caplog.text)
+                assert event == expected, testcase
+        else:
+            with pytest.raises(error):
+                self.object.process(event)
 
     def test_load_custom_patterns_from_http_as_zip_file(self):
         rule = {
             "filter": "message",
             "grokker": {"mapping": {"message": "this is %{ID:userfield}"}},
         }
```

### Comparing `logprep-6.6.0/tests/unit/processor/grokker/test_grokker_rule.py` & `logprep-6.7.0/tests/unit/processor/grokker/test_grokker_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py` & `logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py` & `logprep-6.7.0/tests/unit/processor/hyperscan_resolver/test_hyperscan_resolver_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer.py` & `logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py` & `logprep-6.7.0/tests/unit/processor/ip_informer/test_ip_informer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/labeler/test_labeler.py` & `logprep-6.7.0/tests/unit/processor/labeler/test_labeler.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/labeler/test_labeler_rule.py` & `logprep-6.7.0/tests/unit/processor/labeler/test_labeler_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/labeler/test_labeling_schema.py` & `logprep-6.7.0/tests/unit/processor/labeler/test_labeling_schema.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison.py` & `logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py` & `logprep-6.7.0/tests/unit/processor/list_comparison/test_list_comparison_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer.py` & `logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
         }
 
         with pytest.raises(InvalidGrokDefinition):
             self._load_specific_rule(rule)
 
     def test_normalization_from_timestamp_berlin_to_utc(self):
         expected = {
-            "@timestamp": "1999-12-12T12:12:22Z",
+            "@timestamp": "1999-12-12T11:12:22Z",
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
                 "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
             },
         }
 
@@ -996,35 +996,35 @@
         with caplog.at_level(logging.WARNING):
             self.object.process(event)
         assert re.match(".*NormalizerError.*", caplog.text)
         assert event == expected
 
     def test_normalization_from_timestamp_with_collision(self):
         expected = {
-            "@timestamp": "1999-12-12T12:12:22Z",
+            "@timestamp": "1999-12-12T11:12:22Z",
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
-                "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
+                "event_data": {"some_timestamp_berlin": "1999 12 12 - 12:12:22"},
             },
         }
 
         event = {
             "@timestamp": "2200-02-01T16:19:22Z",
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
-                "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
+                "event_data": {"some_timestamp_berlin": "1999 12 12 - 12:12:22"},
             },
         }
 
         rule = {
             "filter": "winlog.event_id: 123456789",
             "normalize": {
-                "winlog.event_data.some_timestamp_utc": {
+                "winlog.event_data.some_timestamp_berlin": {
                     "timestamp": {
                         "destination": "@timestamp",
                         "source_formats": ["%Y", "%Y %m %d - %H:%M:%S"],
                         "source_timezone": "Europe/Berlin",
                         "destination_timezone": "UTC",
                     }
                 }
```

### Comparing `logprep-6.6.0/tests/unit/processor/normalizer/test_normalizer_rule.py` & `logprep-6.7.0/tests/unit/processor/normalizer/test_normalizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pre_detector/test_ip_alerter.py` & `logprep-6.7.0/tests/unit/processor/pre_detector/test_ip_alerter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector.py` & `logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py` & `logprep-6.7.0/tests/unit/processor/pre_detector/test_pre_detector_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_encrypter.py` & `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_encrypter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py` & `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py` & `logprep-6.7.0/tests/unit/processor/pseudonymizer/test_pseudonymizer_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/requester/test_requester.py` & `logprep-6.7.0/tests/unit/processor/requester/test_requester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/requester/test_requester_rule.py` & `logprep-6.7.0/tests/unit/processor/requester/test_requester_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor.py` & `logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py` & `logprep-6.7.0/tests/unit/processor/selective_extractor/test_selective_extractor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter.py` & `logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py` & `logprep-6.7.0/tests/unit/processor/string_splitter/test_string_splitter_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/template_replacer/test_template_replacer.py` & `logprep-6.7.0/tests/unit/processor/template_replacer/test_template_replacer.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/test_processor_rule.py` & `logprep-6.7.0/tests/unit/processor/test_processor_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/test_processor_strategy.py` & `logprep-6.7.0/tests/unit/processor/test_processor_strategy.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py` & `logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py` & `logprep-6.7.0/tests/unit/processor/timestamp_differ/test_timestamp_differ_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper.py` & `logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,34 +83,34 @@
         },
     ),
     (
         "normalization from timestamp berlin to utc",
         {
             "filter": "winlog.event_id: 123456789",
             "timestamper": {
-                "source_fields": ["winlog.event_data.some_timestamp_utc"],
+                "source_fields": ["winlog.event_data.some_timestamp_berlin"],
                 "target_field": "@timestamp",
                 "source_format": "%Y %m %d - %H:%M:%S",
                 "source_timezone": "Europe/Berlin",
                 "target_timezone": "UTC",
             },
         },
         {
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
-                "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
+                "event_data": {"some_timestamp_berlin": "1999 12 12 - 12:12:22"},
             }
         },
         {
-            "@timestamp": "1999-12-12T12:12:22Z",
+            "@timestamp": "1999-12-12T11:12:22Z",
             "winlog": {
                 "api": "wineventlog",
                 "event_id": 123456789,
-                "event_data": {"some_timestamp_utc": "1999 12 12 - 12:12:22"},
+                "event_data": {"some_timestamp_berlin": "1999 12 12 - 12:12:22"},
             },
         },
     ),
     (
         "normalization from timestamp same timezone",
         {
             "filter": "winlog.event_id: 123456789",
```

### Comparing `logprep-6.6.0/tests/unit/processor/timestamper/test_timestamper_rule.py` & `logprep-6.7.0/tests/unit/processor/timestamper/test_timestamper_rule.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/test_configuration.py` & `logprep-6.7.0/tests/unit/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/test_factory.py` & `logprep-6.7.0/tests/unit/test_factory.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/test_run_logprep.py` & `logprep-6.7.0/tests/unit/test_run_logprep.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/test_runner.py` & `logprep-6.7.0/tests/unit/test_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_auto_rule_corpus_tester.py` & `logprep-6.7.0/tests/unit/util/test_auto_rule_corpus_tester.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pylint: disable=missing-docstring
 # pylint: disable=protected-access
 # pylint: disable=too-many-arguments
 import json
 import os
+import re
 from json import JSONDecodeError
 from unittest import mock
 
 import pytest
 
 from logprep.util.auto_rule_tester.auto_rule_corpus_tester import RuleCorpusTester
 from logprep.util.getter import GetterFactory
@@ -461,7 +462,36 @@
             "PASSED",
             "Total test cases: 2",
             "Success rate: 100.00%",
         ]
         for expected_print in expected_prints:
             assert expected_print in console_output
         mock_exit.assert_called_with(0)
+
+    @mock.patch("logprep.util.auto_rule_tester.auto_rule_corpus_tester.sys.exit")
+    def test_warnings_are_printed_inside_the_detailed_reports(self, mock_exit, tmp_path, capsys):
+        test_case_data = {
+            "input": {
+                "winlog": {"event_id": "2222", "event_data": {"Test1": 1, "Test2": 2}},
+                "test_normalized": "exists already",
+            },
+            "expected_output": {
+                "winlog": {"event_id": "2222", "event_data": {"Test1": 1, "Test2": 2}},
+                "test_normalized": {"test": {"field1": 1, "field2": 2}},
+            },
+            "expected_extra_output": [],
+        }
+        test_data_dir = tmp_path / "test_data"
+        os.makedirs(test_data_dir, exist_ok=True)
+        write_test_case_data_tmp_files(test_data_dir, "test_case_one", test_case_data)
+        config_path = "tests/testdata/config/config.yml"
+        corpus_tester = RuleCorpusTester(config_path, test_data_dir)
+        corpus_tester.run()
+        console_output, console_error = capsys.readouterr()
+        assert console_error == ""
+        warnings_inside_details_pattern = (
+            r".*Test Cases Detailed Reports.*test_case_one.*"
+            r"Logprep Warnings.*FieldExistsWarning.*test_case_one.*"
+            r"Test Overview"
+        )
+        assert re.match(warnings_inside_details_pattern, console_output, flags=re.DOTALL)
+        mock_exit.assert_called_with(1)
```

### Comparing `logprep-6.6.0/tests/unit/util/test_auto_rule_tester.py` & `logprep-6.7.0/tests/unit/util/test_auto_rule_tester.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_cache.py` & `logprep-6.7.0/tests/unit/util/test_cache.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_configuration.py` & `logprep-6.7.0/tests/unit/util/test_configuration.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_getter.py` & `logprep-6.7.0/tests/unit/util/test_getter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_grok_pattern.py` & `logprep-6.7.0/tests/unit/util/test_grok_pattern.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_grok_pattern_loader.py` & `logprep-6.7.0/tests/unit/util/test_grok_pattern_loader.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_helper.py` & `logprep-6.7.0/tests/unit/util/test_helper.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_helper_add_field.py` & `logprep-6.7.0/tests/unit/util/test_helper_add_field.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_log_aggregator.py` & `logprep-6.7.0/tests/unit/util/test_log_aggregator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_processor_generator.py` & `logprep-6.7.0/tests/unit/util/test_processor_generator.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_prometheus_exporter.py` & `logprep-6.7.0/tests/unit/util/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_rule_dry_runner.py` & `logprep-6.7.0/tests/unit/util/test_rule_dry_runner.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_time_measurement.py` & `logprep-6.7.0/tests/unit/util/test_time_measurement.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/test_validators.py` & `logprep-6.7.0/tests/unit/util/test_validators.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/unit/util/tests_json_handling.py` & `logprep-6.7.0/tests/unit/util/tests_json_handling.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/tests/util/testhelpers.py` & `logprep-6.7.0/tests/util/testhelpers.py`

 * *Files identical despite different names*

### Comparing `logprep-6.6.0/versioneer.py` & `logprep-6.7.0/versioneer.py`

 * *Files identical despite different names*

