# Comparing `tmp/datarobot_early_access-3.2.0.2023.7.3.tar.gz` & `tmp/datarobot_early_access-3.3.0.2023.7.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datarobot_early_access-3.2.0.2023.7.3.tar", last modified: Mon Jul  3 16:46:43 2023, max compression
+gzip compressed data, was "dist/datarobot_early_access-3.3.0.2023.7.17.tar", last modified: Mon Jul 17 16:49:35 2023, max compression
```

## Comparing `datarobot_early_access-3.2.0.2023.7.3.tar` & `datarobot_early_access-3.3.0.2023.7.17.tar`

### file list

```diff
@@ -1,174 +1,177 @@
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   179085 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/CHANGES.rst
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/LICENSE.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/MANIFEST.in
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/README.md
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5712 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/common_setup.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2332 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_compat.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      600 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/__init__.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/data_matching.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/documentai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/documentai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/documentai/document.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      927 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/idiomatic_project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4428 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model_lineage.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model_package.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/notebooks.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/retraining.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/analytics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21331 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/client.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/context.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26065 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/enums.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/errors.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/binary_data_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/eligibility_result.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/feature_discovery.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/image_utils.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/partitioning_methods.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/browser_mixin.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/update_attributes_mixin.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4140 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/advanced_tuning.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/anomaly_assessment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/api_object.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/application.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/automated_documentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19691 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_monitoring_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    66977 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_prediction_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/blueprint.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/calendar_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/change_request.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/cluster.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/cluster_insight.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/compliance_doc_template.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/connector.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13004 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/credential.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33089 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model_test.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59836 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task_version_dependency_build.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_engine_query_generator.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16994 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_slice.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18064 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_store.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    58746 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/datetime_trend_plots.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/accuracy.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/bias_and_fairness.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/data_drift.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94652 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/deployment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/mixins.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/service_stats.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/driver.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/execution_environment.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/execution_environment_version.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_baseline_validation.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_scores.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18187 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_effect.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7151 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/featurelist.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/imported_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21166 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5106 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/lift_chart.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/missing_report.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   278679 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/modeljob.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/pairwise_statistics.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/pareto_front.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/payoff_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/predict_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_explanations.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_server.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prime_file.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215251 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/project.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/project_options.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/rating_table.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/recommended_model.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/relationships_configuration.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5049 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/residuals.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/restore_discarded_features.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10126 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/roc_curve.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/ruleset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/secondary_dataset.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/segmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_impact.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_matrix.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_matrix_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7236 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/sharing.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4554 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/status_check_job.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/training_predictions.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/types.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24079 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/use_case.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12298 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/utils.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/models.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/trafarets.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/validators.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/augmentation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/images.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/insights.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/models/word_cloud.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/py.typed
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/rest.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/__init__.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/deprecation.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/logger.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/pagination.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/retry.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/source.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/sourcedata.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4061 2023-07-03 16:46:14.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/waiters.py
-drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4183 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/PKG-INFO
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5840 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/SOURCES.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/dependency_links.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1154 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/requires.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/top_level.txt
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-07-03 16:46:15.000000 datarobot_early_access-3.2.0.2023.7.3/pyproject.toml
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-07-03 16:46:43.000000 datarobot_early_access-3.2.0.2023.7.3/setup.cfg
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-07-03 16:46:15.000000 datarobot_early_access-3.2.0.2023.7.3/setup.py
--rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-07-03 16:46:15.000000 datarobot_early_access-3.2.0.2023.7.3/setup_weekly.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   179852 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/CHANGES.rst
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7555 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/LICENSE.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      421 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/MANIFEST.in
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8911 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/README.md
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5712 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/common_setup.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2332 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      687 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_compat.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      553 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/__init__.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15390 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/data_matching.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2742 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/dataset.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/documentai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/documentai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26523 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/documentai/document.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2346 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8693 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/idiomatic_project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4428 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21414 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model_lineage.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14822 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model_package.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9905 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/notebooks.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    54152 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9191 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/recipe_operations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8990 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/recipes.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7398 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/retraining.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      313 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5241 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/analytics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21331 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/client.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4664 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/context.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    26065 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/enums.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8984 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/errors.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    22432 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13002 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/binary_data_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1156 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/eligibility_result.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14350 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/feature_discovery.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8696 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/image_utils.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   101561 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/partitioning_methods.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1134 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/browser_mixin.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1112 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/update_attributes_mixin.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4140 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9166 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/advanced_tuning.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    27075 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/anomaly_assessment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2925 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/api_object.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8859 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/application.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15447 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/automated_documentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19691 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    37053 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_monitoring_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    66977 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_prediction_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11096 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/blueprint.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    23822 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/calendar_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13301 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/change_request.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3978 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/cluster.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7233 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/cluster_insight.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12910 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/compliance_doc_template.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4887 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6953 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/connector.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13004 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/credential.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    33397 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12413 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model_test.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59836 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15411 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21102 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2315 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task_version_dependency_build.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17613 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_engine_query_generator.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16994 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_slice.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    16402 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18064 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_store.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    59131 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    30524 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/datetime_trend_plots.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      387 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12535 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/accuracy.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5688 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/bias_and_fairness.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12650 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/data_drift.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    94652 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/deployment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1131 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/mixins.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10065 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/service_stats.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3450 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6583 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/driver.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     9411 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/execution_environment.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    11344 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/execution_environment_version.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5374 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_baseline_validation.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      355 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6403 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4915 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4523 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5208 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4521 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6789 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_scores.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    53938 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      237 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2600 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_featurelists.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     6177 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4753 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_matrix_details.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18187 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_effect.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7003 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    17463 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/featurelist.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7336 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/imported_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    21166 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5106 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/lift_chart.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5468 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/missing_report.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   281724 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7215 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/modeljob.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14320 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/pairwise_statistics.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5438 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/pareto_front.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8726 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/payoff_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7403 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/predict_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10218 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    34744 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_explanations.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2426 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_server.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15940 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2655 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prime_file.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)   215251 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/project.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    55519 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/project_options.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8774 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/rating_table.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4337 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/recommended_model.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19064 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/relationships_configuration.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5049 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/residuals.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4524 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/restore_discarded_features.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10126 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/roc_curve.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2927 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/ruleset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    19381 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/secondary_dataset.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    14217 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/segmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4070 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_impact.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7057 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_matrix.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2645 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_matrix_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     7236 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/sharing.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4683 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/status_check_job.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1431 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    28260 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/training_predictions.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1822 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/types.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      262 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    24079 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/use_case.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    12513 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/utils.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       49 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    69649 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/models.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     8758 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/trafarets.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2749 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/validators.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      226 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18528 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/augmentation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    10521 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/images.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    13615 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/insights.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4936 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/models/word_cloud.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/py.typed
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    18404 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/rest.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)    15618 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/__init__.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2997 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/deprecation.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      495 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/logger.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1200 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/pagination.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1461 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/retry.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1282 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/source.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4109 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/sourcedata.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4193 2023-07-17 16:49:07.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/waiters.py
+drwxrwxr-x   0 jenkins-slave  (1001) jenkins-slave  (1001)        0 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     4184 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/PKG-INFO
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     5976 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/SOURCES.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)        1 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/dependency_links.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     1154 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/requires.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)       10 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/top_level.txt
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     3066 2023-07-17 16:49:08.000000 datarobot_early_access-3.3.0.2023.7.17/pyproject.toml
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      123 2023-07-17 16:49:35.000000 datarobot_early_access-3.3.0.2023.7.17/setup.cfg
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)      965 2023-07-17 16:49:08.000000 datarobot_early_access-3.3.0.2023.7.17/setup.py
+-rw-rw-r--   0 jenkins-slave  (1001) jenkins-slave  (1001)     2403 2023-07-17 16:49:08.000000 datarobot_early_access-3.3.0.2023.7.17/setup_weekly.py
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/CHANGES.rst` & `datarobot_early_access-3.3.0.2023.7.17/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,24 @@
 #########
 Changelog
 #########
-3.2.0b0
-========
+3.3.0b0
+=======
+
+New Features
+************
+
+Enhancements
+************
+
+Bugfixes
+********
+
+3.2.0
+=====
 
 New Features
 ************
 - Added new methods to trigger batch monitoring jobs without providing a job definition.
   :meth:`BatchMonitoringJob.run <datarobot.models.BatchMonitoringJob.run>`
   :meth:`BatchMonitoringJob.get_status <datarobot.models.BatchMonitoringJob.get_status>`
   :meth:`BatchMonitoringJob.cancel <datarobot.models.BatchMonitoringJob.cancel>`
@@ -90,14 +102,16 @@
   :meth:`Model.get_all_lift_charts <datarobot.models.Model.get_all_lift_charts>`
   :meth:`Model.get_residuals_chart <datarobot.models.Model.get_residuals_chart>`
   :meth:`Model.get_all_residuals_charts <datarobot.models.Model.get_all_residuals_charts>`
   :meth:`Model.request_lift_chart <datarobot.models.Model.request_lift_chart>`
   :meth:`Model.request_residuals_chart <datarobot.models.Model.request_residuals_chart>`
   :meth:`Model.get_roc_curve<datarobot.models.Model.get_roc_curve>`
   :meth:`Model.get_feature_impact <datarobot.models.Model.get_feature_impact>`
+  :meth:`Model.request_feature_impact <datarobot.models.Model.request_feature_impact>`
+  :meth:`Model.get_or_request_feature_impact <datarobot.models.Model.get_or_request_feature_impact>`
 - Added support for :class:`SharingRole <datarobot.models.sharing.SharingRole>` to the following methods:
   - :meth:`DataStore.share <datarobot.DataStore.share>`
 - Added new methods for retrieving :class:`SharingRole <datarobot.models.sharing.SharingRole>` information for the following classes:
   - :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>`
 - Added new method for calculating sliced roc curve :meth:`Model.request_roc_curve <datarobot.models.Model.request_roc_curve>`
 - Added new :class:`DataSlice <datarobot.models.data_slice.DataSlice>` to support the following slices methods:
   :meth:`DataSlice.list <datarobot.models.data_slice.DataSlice.list>` to retrieve all data slices in a project.
@@ -132,16 +146,16 @@
     The parameters added to both APIs are:
         - `training_dataset_id`
         - `partition_column`
         - `holdout_dataset_id`
         - `keep_training_holdout_data`
         - `max_wait`
 
-- Extended :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.create>` and :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.update>`
-  with `is_training_data_for_versions_permanently_enabled` parameter.
+- Extended :meth:`CustomInferenceModel.create <datarobot.CustomInferenceModel.create>` and :meth:`CustomInferenceModel.update <datarobot.CustomInferenceModel.update>`
+  with the parameter `is_training_data_for_versions_permanently_enabled`.
 
 - Added value `DR_API_ACCESS` to the `NETWORK_EGRESS_POLICY` enum.
 
 - Added new parameter `low_memory` to :meth:`Dataset.get_as_dataframe <datarobot.models.Dataset.get_as_dataframe>` to allow a low memory mode for larger datasets
 
 Bugfixes
 ********
@@ -171,14 +185,16 @@
   Use :meth:`Model.get_or_request_feature_effect <datarobot.models.Model.get_or_request_feature_effect>` instead.
 - ``DatetimeModel.get_or_request_feature_fit`` has been removed.
   Use :meth:`DatetimeModel.get_or_request_feature_effect <datarobot.models.DatetimeModel.get_or_request_feature_effect>` instead.
 - Deprecated the use of :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` in favor of :class:`SharingRole <datarobot.models.sharing.SharingRole>` for sharing in the following classes:
   - :meth:`DataStore.share <datarobot.DataStore.share>`
 - Deprecated the following methods for retrieving :class:`SharingAccess <datarobot.models.sharing.SharingAccess>` information.
   - :meth:`DataStore.get_access_list <datarobot.DataStore.get_access_list>`. Please use :meth:`DataStore.get_shared_roles <datarobot.DataStore.get_shared_roles>` instead.
+- :meth:`CustomInferenceModel.assign_training_data <datarobot.CustomInferenceModel.assign_training_data>` was marked as deprecated and will be removed in v3.4.
+  Use :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>` and :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>` instead.
 
 Configuration Changes
 *********************
 - Pins dependency on package `urllib3 <https://pypi.org/project/urllib3/>`_  to be less than version 2.0.0.
 
 Deprecation Summary
 *******************
@@ -206,14 +222,18 @@
 
 - Changed behavior for methods that search for the closest data points in :class:`DataMatching <datarobot._experimental.models.data_matching.DataMatching>`. If the index is missing, instead of throwing the error, methods try to create the index and then query it. This is enabled by default, but if this is not the intended behavior it can be changed by passing `False` to the new `build_index` parameter added to the methods:
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_model>`
     - :meth:`DataMatching.get_closest_data <datarobot._experimental.models.data_matching.DataMatching.get_closest_data_for_featurelist>`
 - Added a new class :class:`Notebook <datarobot._experimental.models.notebooks.Notebook>` for retrieving DataRobot Notebooks available to the user.
 
+- Added experimental support for data wrangling:
+
+  - :class:`Recipe <datarobot._experimental.models.recipes.Recipe>`
+
 
 3.1.1
 =====
 
 Configuration Changes
 *********************
 - Removes dependency on package `contextlib2 <https://pypi.org/project/contextlib2/>`_  since the package is Python 3.7+.
@@ -1144,15 +1164,15 @@
 API Changes
 ***********
 - Remove `desired_memory` param from the following classes: :class:`datarobot.CustomInferenceModel`,
   :class:`datarobot.CustomModelVersion`, :class:`datarobot.CustomModelTest`
 - Remove ``desired_memory`` param from the following methods:
   :meth:`CustomInferenceModel.create <datarobot.CustomInferenceModel.create>`,
   :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_clean>`,
-  :meth:`CustomModelVersion.create_clean <datarobot.CustomModelVersion.create_from_previous>`,
+  :meth:`CustomModelVersion.create_from_previous <datarobot.CustomModelVersion.create_from_previous>`,
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>` and
   :meth:`CustomModelTest.create <datarobot.CustomModelTest.create>`
 
 
 Deprecation Summary
 *******************
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/LICENSE.txt` & `datarobot_early_access-3.3.0.2023.7.17/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/PKG-INFO` & `datarobot_early_access-3.3.0.2023.7.17/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot_early_access
-Version: 3.2.0.2023.7.3
+Version: 3.3.0.2023.7.17
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/README.md` & `datarobot_early_access-3.3.0.2023.7.17/README.md`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/common_setup.py` & `datarobot_early_access-3.3.0.2023.7.17/common_setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/__init__.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_compat.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_compat.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/__init__.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # flake8: noqa
 # because the unused imports are on purpose
 
 import logging
 
-from .models.enums import UnsupervisedTypeEnum
 from .models.idiomatic_project import IdiomaticProject
 from .models.model import DatetimeModel, Model
 
 logger = logging.getLogger(__package__)
 
 experimental_warning = (
     "You have imported from the _experimental directory.\n"
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/data_matching.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/data_matching.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/documentai/document.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/documentai/document.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/idiomatic_project.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/idiomatic_project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model_lineage.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model_lineage.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/model_package.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/model_package.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/notebooks.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/notebooks.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/project_options.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/_experimental/models/retraining.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/_experimental/models/retraining.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/analytics.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/analytics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/client.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/client.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/context.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/context.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/enums.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/enums.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/errors.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/errors.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/__init__.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/binary_data_utils.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/binary_data_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/eligibility_result.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/eligibility_result.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/feature_discovery.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/feature_discovery.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/image_utils.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/image_utils.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/helpers/partitioning_methods.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/helpers/partitioning_methods.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/browser_mixin.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/browser_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/mixins/update_attributes_mixin.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/mixins/update_attributes_mixin.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/__init__.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/advanced_tuning.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/advanced_tuning.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/anomaly_assessment.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/anomaly_assessment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/api_object.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/api_object.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/application.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/application.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/automated_documentation.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/automated_documentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_monitoring_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_monitoring_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/batch_prediction_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/batch_prediction_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/blueprint.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/blueprint.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/calendar_file.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/calendar_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/change_request.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/change_request.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/cluster.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/cluster.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/cluster_insight.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/cluster_insight.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/compliance_doc_template.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/compliance_doc_template.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/confusion_chart.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/connector.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/connector.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/credential.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/credential.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     DEFAULT_MAX_WAIT,
     NETWORK_EGRESS_POLICY,
     TARGET_TYPE,
 )
 from datarobot.errors import ClientError
 from datarobot.models.api_object import APIObject
 from datarobot.models.custom_model_version import CustomModelVersion
+from datarobot.utils import deprecated
 from datarobot.utils.pagination import unpaginate
 from datarobot.utils.waiters import wait_for_async_resolution
 
 T_CustomModelBase = TypeVar("T_CustomModelBase", bound="_CustomModelBase")
 
 
 class _CustomModelBase(APIObject):  # pylint: disable=missing-class-docstring
@@ -814,14 +815,20 @@
         datarobot.errors.ClientError
             If the server responded with 4xx status.
         datarobot.errors.ServerError
             If the server responded with 5xx status.
         """
         super().delete()
 
+    @deprecated(
+        deprecated_since_version="v3.2",
+        will_remove_version="v3.4",
+        message="Please use training data assignment on the model version level: "
+        "CustomModelVersion.create_from_previous or CustomModelVersion.create_clean",
+    )
     def assign_training_data(
         self,
         dataset_id: str,
         partition_column: Optional[str] = None,
         max_wait: int = DEFAULT_MAX_WAIT,
     ) -> None:
         """Assign training data to the custom inference model.
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model_test.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model_test.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_model_version.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_model_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task_version.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/custom_task_version_dependency_build.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/custom_task_version_dependency_build.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_engine_query_generator.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_engine_query_generator.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_slice.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_slice.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_source.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/data_store.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/data_store.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/dataset.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,28 +122,30 @@
         is_latest_version: bool,
         is_snapshot: bool,
         processing_state: str,
         created_by: Optional[str] = None,
         data_persisted: Optional[bool] = None,
         size: Optional[int] = None,
         row_count: Optional[int] = None,
+        recipe_id: Optional[str] = None,
     ) -> None:
         self.id = dataset_id
         self.version_id = version_id
         self.name = name
         self.data_persisted = data_persisted
         self.categories = categories[:]
         self.created_at = created_at
         self.created_by = created_by
         self.is_data_engine_eligible = is_data_engine_eligible
         self.is_latest_version = is_latest_version
         self.is_snapshot = is_snapshot
         self.size = size
         self.row_count = row_count
         self.processing_state = processing_state
+        self.recipe_id = recipe_id
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(name={self.name!r}, id={self.id!r})"
 
     def get_uri(self) -> str:
         """
         Returns
@@ -1437,14 +1439,16 @@
             t.Key("feature_count_by_type", optional=True): t.List(
                 t.Call(lambda d: FeatureTypeCount(**d))
             ),
             t.Key("last_modification_date"): t.Call(dateutil.parser.parse),
             t.Key("last_modifier_full_name"): String,
             t.Key("tags", optional=True): t.List(String),
             t.Key("uri"): String,
+            t.Key("recipe_id", optional=True): String,
+            t.Key("is_wrangling_eligible", optional=True): bool,
         }
     )
 
     _converter = _safe_merge(_extra_fields, _base_dataset_schema).allow_extra("*")
 
     _path = "datasets/"
 
@@ -1472,14 +1476,16 @@
         eda1_modification_date: Optional[str] = None,
         eda1_modifier_full_name: Optional[str] = None,
         feature_count: Optional[int] = None,
         feature_count_by_type: Optional[List[FeatureTypeCount]] = None,
         row_count: Optional[int] = None,
         size: Optional[int] = None,
         tags: Optional[List[str]] = None,
+        recipe_id: Optional[str] = None,
+        is_wrangling_eligible: Optional[bool] = None,
     ):
         self.dataset_id = dataset_id
         self.version_id = version_id
         self.categories = categories
         self.created_by = created_by
         self.created_at = created_at
         self.data_source_type = data_source_type
@@ -1499,14 +1505,16 @@
         self.eda1_modifier_full_name = eda1_modifier_full_name
         self.feature_count = feature_count
         self.feature_count_by_type = feature_count_by_type
         self.processing_state = processing_state
         self.row_count = row_count
         self.size = size
         self.tags = tags
+        self.recipe_id = recipe_id
+        self.is_wrangling_eligible = is_wrangling_eligible
 
     @classmethod
     def get(cls: Type[TDatasetDetails], dataset_id: str) -> TDatasetDetails:
         """
         Get details for a Dataset from the server
 
         Parameters
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/datetime_trend_plots.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/datetime_trend_plots.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/accuracy.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/accuracy.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/bias_and_fairness.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/bias_and_fairness.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/data_drift.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/data_drift.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/deployment.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/mixins.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/mixins.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/service_stats.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/service_stats.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/deployment/sharing.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/deployment/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/driver.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/driver.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/execution_environment.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/execution_environment.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/execution_environment_version.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/execution_environment_version.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_baseline_validation.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_baseline_validation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_confusion_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_dataset_residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_multiclass_lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_roc_curve.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/external_dataset_scores_insights/external_scores.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/external_dataset_scores_insights/external_scores.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_featurelists.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_featurelists.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_matrix.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_association_matrix/feature_association_matrix_details.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_association_matrix/feature_association_matrix_details.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_effect.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_effect.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/feature_impact.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/feature_impact.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 )
 
 
 class FeatureImpactData(TypedDict):
     feature_name: str
     impact_normalized: float
     impact_unnormalized: float
-    adjusted_feature_impact: Optional[List[str]]
     redundant_with: Optional[str]
 
 
 class FeatureImpactsData(TypedDict):
     feature_impacts: List[FeatureImpactData]
     ran_redundancy_detection: bool
     row_count: Optional[int]
@@ -141,15 +140,14 @@
            "dataSliceId": None,
            "data": {
               "featureImpacts": [
                  {
                     "featureName": "readmitted",
                     "impactNormalized": 1.0,
                     "impactUnnormalized": 16.468279209120773,
-                    "adjustedFeatureImpact": None,
                     "redundantWith": None,
                  },
               ],
               "ranRedundancyDetection": True,
               "rowCount": 2500,
            }
         }
@@ -160,15 +158,14 @@
         {
            "count": 1,
            "featureImpacts": [
               {
                  "featureName": "readmitted",
                  "impactNormalized": 1.0,
                  "impactUnnormalized": 16.468279209120773,
-                 "adjustedFeatureImpact": None,
                  "redundantWith": None,
               },
            ],
            "ranRedundancyDetection": True,
            "shapBased": False,
            "rowCount": 2500,
            "backtest": None,
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/featurelist.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/featurelist.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/imported_model.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/imported_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/lift_chart.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/lift_chart.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/missing_report.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/missing_report.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/model.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #
 # Released under the terms of DataRobot Tool and Utility Agreement.
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
 from datetime import datetime
 from io import IOBase, StringIO
-from typing import Any, cast, Dict, List, NoReturn, Optional, Tuple, TYPE_CHECKING, Union
+from typing import Any, cast, Dict, List, NoReturn, Optional, Set, Tuple, TYPE_CHECKING, Union
 from urllib.parse import urljoin
 import warnings
 
 import pandas as pd
 import trafaret as t
 
 from datarobot._compat import Int, String
@@ -73,14 +73,15 @@
     DATETIME_TREND_PLOTS_STATUS,
     DEFAULT_MAX_WAIT,
     MONOTONICITY_FEATURELIST_DEFAULT,
     SOURCE_TYPE,
     TARGET_TYPE,
 )
 from ..utils import from_api, get_id_from_response, parse_time
+from ..utils.waiters import wait_for_async_resolution
 from .advanced_tuning import AdvancedTuningSession
 from .api_object import APIObject
 from .feature_impact import FeatureImpact
 
 if TYPE_CHECKING:
     from mypy_extensions import TypedDict
 
@@ -1022,25 +1023,14 @@
         if self.id is None:
             # This check is why this is a method instead of an attribute. Once we stop creating
             # models without model id's in the tests, we can make this an attribute we set in the
             # constructor.
             raise ValueError("Sorry, id attribute is None so I can't make the url to this model.")
         return f"insights/{insight_name}/models/{self.id}"
 
-    def _get_data_slice_params(self, data_slice_id: str, unsliced_only: bool) -> Dict[str, str]:
-        """Validate user input, raise an exception or return a valid data slice params dict"""
-        # TODO: remove this function entirely and use _data_slice_to_query_params instead
-
-        if data_slice_id:
-            if unsliced_only:
-                raise ValueError("Do not specify unsliced_only=true and data_slice_id together")
-
-            return {"dataSliceId": data_slice_id}
-        return {"unslicedOnly": "true"} if unsliced_only else {}
-
     def _data_slice_to_query_params(self, data_slice_filter: DataSlice = None) -> Dict[str, str]:
         """Convert a DataSlice object to the query params needed to request insights with a matching
         DataSlice.  Passing in data_slice_filter = None will set params to return all insights"""
         params = {}
         if data_slice_filter:
             if data_slice_filter.id is None:
                 # since we can't pass None to the endpoint, setting unslicedOnly = True
@@ -1050,14 +1040,24 @@
                 params["dataSliceId"] = data_slice_filter.id
         else:
             # this is default, but just being explicit here
             params["unslicedOnly"] = False
 
         return params
 
+    def _validate_data_slice_filter(self, data_slice_filter: DataSlice | None) -> None:
+        """This method to validate data_slice_filter is not None for:
+        get_feature_impact, get_residuals_chart, get_lift_chart and get_roc_curve.
+        if data_slice_filter is None, the insights API fetch call won't filter insights,
+        this potentially will return a list of charts. The methods listed above expect to return
+        only a single chart sliced or unsliced insight.
+        """
+        if data_slice_filter is None:
+            raise ValueError("Invalid data_slice_filter value. Please specify `DataSlice` filter")
+
     def _get_feature_impact_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureImpact/"
 
     def get_feature_impact(
         self,
         with_metadata: bool = False,
@@ -1087,15 +1087,15 @@
         Parameters
         ----------
         with_metadata : bool
             The flag indicating if the result should include the metadata as well.
         data_slice_filter : DataSlice, optional
             A dataslice used to filter the return values based on the dataslice.id. By default, this function will
             use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
-            then no data_slice filtering will be applied when requesting the roc_curve.
+            then get_feature_impact will raise a ValueError.
 
         Returns
         -------
         list or dict
             The feature impact data response depends on the with_metadata parameter. The response is
             either a dict with metadata and a list with actual data or just a list with that data.
 
@@ -1116,15 +1116,20 @@
                     logic, without specifying the rowCount, we return None here.
               - ``count`` - An integer with the number of features under the ``featureImpacts``.
 
         Raises
         ------
         ClientError (404)
             If the feature impacts have not been computed.
+        ValueError
+            If data_slice_filter passed as None
         """
+
+        self._validate_data_slice_filter(data_slice_filter)
+
         if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
             data_slice_filter = DataSlice(id=None)
 
         insight_name = "featureImpact"
         params = self._data_slice_to_query_params(data_slice_filter)
 
         try:
@@ -1165,15 +1170,15 @@
             A dataslice used to filter the return values based on the dataslice.id. By default, this function will
             use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
             then no data_slice filtering will be applied when requesting the roc_curve.
 
         Returns
         -------
         list of dicts
-            Data for all available model feature impacts.
+            Data for all available model feature impacts. Or an empty list if not data found.
 
         Examples
         --------
         .. code-block:: python
 
             model = datarobot.Model(id='model-id', project_id='project-id')
 
@@ -1234,41 +1239,65 @@
             If the multiclass feature impacts have not been computed.
         """
         url = self._get_model_url() + "multiclassFeatureImpact/"
         data = self._client.get(url).json()
         data = multiclass_feature_impact_trafaret.check(data)
         return data["classFeatureImpacts"]
 
-    def request_feature_impact(self, row_count: Optional[int] = None, with_metadata: bool = False):
+    def request_feature_impact(
+        self,
+        row_count: Optional[int] = None,
+        with_metadata: bool = False,
+        data_slice_id: Optional[str] = None,
+    ):
         """
         Request feature impacts to be computed for the model.
 
         See :meth:`get_feature_impact <datarobot.models.Model.get_feature_impact>` for more
         information on the result of the job.
 
         Parameters
         ----------
-        row_count : int
+        row_count : int, optional
             The sample size (specified in rows) to use for Feature Impact computation. This is not
-            supported for unsupervised, multi-class (that has a separate method) and time series
+            supported for unsupervised, multiclass (which has a separate method), and time series
             projects.
+        with_metadata : bool, optional
+            Flag indicating whether the result should include the metadata.
+            If true, metadata is included.
+        data_slice_id : str, optional
+            ID for the data slice used in the request. If None, request unsliced insight data.
 
         Returns
         -------
-         job : Job
-            A Job representing the feature impact computation. To get the completed feature impact
+         job : Job or status_id
+            Job representing the Feature Impact computation. To retrieve the completed Feature Impact
             data, use `job.get_result` or `job.get_result_when_complete`.
 
         Raises
         ------
         JobAlreadyRequested (422)
             If the feature impacts have already been requested.
         """
         from .job import FeatureImpactJob  # pylint: disable=import-outside-toplevel,cyclic-import
 
+        if data_slice_id:
+            route = self._post_insights_url("featureImpact")
+            payload = {
+                "source": "training",
+                "dataSliceId": data_slice_id,
+                "entityType": "datarobotModel",
+                "entityId": self.id,
+                "rowCount": row_count,
+            }
+            response = self._client.post(route, data=payload)
+            # `/insights/featureImpact/` returns `status_id`, so there is no `job_id`
+            # to build a FeatureImpactJob object
+            return get_id_from_response(response)
+
         route = self._get_feature_impact_url()
         payload = {"row_count": row_count} if row_count is not None else {}
         response = self._client.post(route, data=payload)
         job_id = get_id_from_response(response)
         return FeatureImpactJob.get(self.project_id, job_id, with_metadata=with_metadata)
 
     def request_external_test(self, dataset_id: str, actual_value_column: Optional[str] = None):
@@ -1308,33 +1337,38 @@
         -------
          feature_impacts : list or dict
             The feature impact data. See
             :meth:`get_feature_impact <datarobot.models.Model.get_feature_impact>` for the exact
             schema.
         """
         try:
-            feature_impact_job = self.request_feature_impact(**kwargs)
+            feature_impact_response = self.request_feature_impact(**kwargs)
         except JobAlreadyRequested as e:
             # If already requested it may be still running. Check and get the job id in that case.
             qid = e.json["jobId"]
             if qid is None:
                 # There are rare cases, when existing (old) job can not be retrieved.
                 # Last resort: optimistically try to return an existing result.
                 return self.get_feature_impact(**kwargs)
 
             from .job import (  # pylint: disable=import-outside-toplevel,cyclic-import
                 FeatureImpactJob,
             )
 
             with_metadata = kwargs.get("with_metadata", False)
-            feature_impact_job = FeatureImpactJob.get(
+            feature_impact_response = FeatureImpactJob.get(
                 self.project_id, qid, with_metadata=with_metadata
             )
+        if kwargs.get("data_slice_id"):
+            wait_for_async_resolution(self._client, f"status/{feature_impact_response}/", max_wait)
+            data_slice = DataSlice(id=kwargs["data_slice_id"])
+
+            return self.get_feature_impact(data_slice_filter=data_slice, with_metadata=True)
 
-        return feature_impact_job.get_result_when_complete(max_wait=max_wait)
+        return feature_impact_response.get_result_when_complete(max_wait=max_wait)
 
     def _get_feature_effect_metadata_url(self) -> str:
         # This is a method (rather than attribute) for the same reason as _get_model_url.
         return self._get_model_url() + "featureEffectsMetadata/"
 
     def get_feature_effect_metadata(self):
         """
@@ -2033,45 +2067,57 @@
         fallback_to_parent_insights: bool optional
             The default value of False makes this function a no-op.  If True, execute this function.
 
         Returns
         -------
         insight data: dict
             This is the list of all insight data including both what was found associated with the
-            original model and additional insights found in parent model if fallback_to_parent_insights == True.
+            original model and additional insights found in parent model if the model is frozen and
+            fallback_to_parent_insights == True.
+
+        Raises
+        ------
+        ClientError (404)
+            If the insight is not available for this model
         """
 
-        if not fallback_to_parent_insights:
-            return response_data["data"]
+        if self.is_frozen and fallback_to_parent_insights:
 
-        sources = [item["source"] for item in response_data["data"]]
-        source_types = [
-            CHART_DATA_SOURCE.VALIDATION,
-            CHART_DATA_SOURCE.CROSSVALIDATION,
-            CHART_DATA_SOURCE.HOLDOUT,
-        ]
-        if self.is_frozen and any(source_type not in sources for source_type in source_types):
-            frozen_model = FrozenModel.get(self.project_id, self.id)
-            parent_model_id = frozen_model.parent_model_id
-            parent_model = Model(id=parent_model_id, project_id=self.project_id)
-            url = parent_model._get_insights_url(insight_type)
-            warning_message = (
-                "{} is not available for all sources for model {}. "
-                "Falling back to parent model {} for missing sources".format(
-                    insight_type, self.id, parent_model_id
+            response_items: Set[Tuple[str, str]] = {
+                (item["source"], item["dataSliceId"]) for item in response_data["data"]
+            }
+
+            source_types = [
+                CHART_DATA_SOURCE.VALIDATION,
+                CHART_DATA_SOURCE.CROSSVALIDATION,
+                CHART_DATA_SOURCE.HOLDOUT,
+            ]
+            sources: Set[str] = {item[0] for item in response_items}
+            if self.is_frozen and any(source_type not in sources for source_type in source_types):
+                frozen_model = FrozenModel.get(self.project_id, self.id)
+                parent_model_id = frozen_model.parent_model_id
+                parent_model = Model(id=parent_model_id, project_id=self.project_id)
+                url = parent_model._get_insights_url(insight_type)
+                warning_message = (
+                    "{} is not available for all sources for model {}. "
+                    "Falling back to parent model {} for missing sources".format(
+                        insight_type, self.id, parent_model_id
+                    )
                 )
-            )
-            warnings.warn(warning_message, ParentModelInsightFallbackWarning, stacklevel=3)
-            parent_data = self._client.get(url, params=params).json()
-            # keep data for sources found on model, and add additional data for sources in parent
-            # but not in original model
-            for data in parent_data.get("data", {}):
-                if data.get("source") and data["source"] not in sources:
-                    response_data["data"].append(data)
-            return response_data["data"]
+                warnings.warn(warning_message, ParentModelInsightFallbackWarning, stacklevel=3)
+                parent_data = self._client.get(url, params=params).json()
+                # keep data for sources/slice_id combination found on model, and add additional data in the parent
+                # but not in original model
+                for parent_record in parent_data.get("data"):
+                    parent_source = parent_record.get("source")
+                    parent_data_slice_id = parent_record.get("dataSliceId")
+                    if (parent_source, parent_data_slice_id) not in response_items:
+                        response_data["data"].append(parent_record)
+
+        return response_data["data"]
 
     def _format_residuals_chart(self, response_data):
         """Reformat the residuals chart API data to match the standard used by
         the Lift and ROC charts
         """
         if list(response_data) == ["charts"]:
             # already been reformatted, so nothing to do
@@ -2113,52 +2159,67 @@
         response = self._client.post(route, data=params)
         return StatusCheckJob.from_response(response)
 
     def get_lift_chart(
         self,
         source: str,
         fallback_to_parent_insights: Optional[bool] = False,
-        data_slice_id: Optional[str] = None,
+        data_slice_filter: Optional[DataSlice] = DATA_SLICE_WITH_ID_NONE,
     ):
         """Retrieve the model Lift chart for the specified source.
 
         Parameters
         ----------
         source : str
             Lift chart data source. Check datarobot.enums.CHART_DATA_SOURCE for possible values.
             (New in version v2.23) For time series and OTV models, also accepts values `backtest_2`,
             `backtest_3`, ..., up to the number of backtests in the model.
         fallback_to_parent_insights : bool
             (New in version v2.14) Optional, if True, this will return lift chart data for this
             model's parent if the lift chart is not available for this model and the model has a
             defined parent model. If omitted or False, or there is no parent model, will not
             attempt to return insight data from this model's parent.
-        data_slice_id : string, optional
-            ID for the data slice used in the request. If None, retrieve unsliced insight data.
+        data_slice_filter : DataSlice, optional
+            A dataslice used to filter the return values based on the dataslice.id. By default this function will
+            use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
+            then get_lift_chart will raise a ValueError.
 
         Returns
         -------
         LiftChart
             Model lift chart data
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
+        ValueError
+            If data_slice_filter passed as None
         """
         insight_name = "liftChart"
-        params = {"source": source}
-        if data_slice_id:
-            params["dataSliceId"] = data_slice_id
-        else:
-            params["unslicedOnly"] = "true"
+
+        self._validate_data_slice_filter(data_slice_filter)
+
+        if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
+            data_slice_filter = DataSlice(id=None)
+
+        params = self._data_slice_to_query_params(data_slice_filter)
+        params["source"] = source
+
         try:
             insights_lift_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_lift_url, params=params).json()
-            response_data = paginated_response["data"][0]
+            response_data = self._get_sliced_insight_from_parent(
+                paginated_response, insight_name, params, fallback_to_parent_insights
+            )
+
+            if len(response_data) == 0:
+                raise ClientError("Requested insight does not exist.", 404)
+
+            response_data = response_data[0]
             use_insights_format = True
         except ClientError as e:
             self._raise_if_not_slice_forbidden_error(e)
             url_template = "projects/{}/models/{}/liftChart/{}/"
             response_data = self._get_insight(
                 url_template,
                 source,
@@ -2197,41 +2258,33 @@
         response = self._client.post(route, data=params)
 
         return StatusCheckJob.from_response(response)
 
     def get_all_lift_charts(
         self,
         fallback_to_parent_insights: Optional[bool] = False,
-        data_slice_id: Optional[str] = None,
-        unsliced_only: Optional[bool] = False,
+        data_slice_filter: Optional[DataSlice] = None,
     ):
         """Retrieve a list of all Lift charts available for the model.
 
         Parameters
         ----------
         fallback_to_parent_insights : bool, optional
             (New in version v2.14) Optional, if True, this will return lift chart data for this
             model's parent for any source that is not available for this model and if this model
             has a defined parent model. If omitted or False, or this model has no parent,
             this will not attempt to retrieve any data from this model's parent.
-        data_slice_id : string, optional
-            ID for the data slice used in the request.
-        unsliced_only: bool
-            Optional, defaults to False.
-            If True return unsliced insight data.
+        data_slice_filter : DataSlice, optional
+            Filters the returned lift chart by data_slice_filter.id.
+            If None (the default) applies no filter based on data_slice_id.
 
         Returns
         -------
         list of LiftChart
-            Data for all available model lift charts.
-
-        Raises
-        ------
-        ClientError
-            If the insight is not available for this model
+            Data for all available model lift charts. Or an empty list if no data found.
 
         Examples
         --------
         .. code-block:: python
 
             model = datarobot.Model.get('project-id', 'model-id')
 
@@ -2242,20 +2295,22 @@
             unsliced_lift_charts = model.get_all_lift_charts(unsliced_only=True)
 
             # Get all lift chart insights
             all_lift_charts = model.get_all_lift_charts()
 
         """
         insight_name = "liftChart"
-        params = self._get_data_slice_params(data_slice_id, unsliced_only)
+        params = self._data_slice_to_query_params(data_slice_filter)
 
         try:
             insights_lift_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_lift_url, params=params).json()
-            response_data = paginated_response["data"]
+            response_data = self._get_sliced_insight_from_parent(
+                paginated_response, insight_name, params, fallback_to_parent_insights
+            )
             use_insights_format = True
         except ClientError as e:
             self._raise_if_not_slice_forbidden_error(e)
             url_template = "projects/{}/models/{}/liftChart/"
             data = self._get_all_source_insight(
                 url_template, "Lift Chart", fallback_to_parent_insights=fallback_to_parent_insights
             )
@@ -2319,19 +2374,14 @@
             has a defined parent model. If omitted or False, or this model has no parent,
             this will not attempt to retrieve any data from this model's parent.
 
         Returns
         -------
         list of LiftChart
             Data for all available model lift charts.
-
-        Raises
-        ------
-        ClientError
-            If the insight is not available for this model
         """
         url_template = "projects/{}/models/{}/multiclassLiftChart/"
         response_data = self._get_all_source_insight(
             url_template,
             "Multiclass Lift Chart",
             fallback_to_parent_insights=fallback_to_parent_insights,
         )
@@ -2410,41 +2460,49 @@
             Optional, if True, this will return residuals chart data for this model's parent if
             the residuals chart is not available for this model and the model has a defined parent
             model. If omitted or False, or there is no parent model, will not attempt to return
             residuals data from this model's parent.
         data_slice_filter : DataSlice, optional
             A dataslice used to filter the return values based on the dataslice.id. By default this function will
             use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
-            then no data_slice filtering will be applied when requesting the residuals chart.
+            then get_residuals_chart will raise a ValueError.
 
         Returns
         -------
         ResidualsChart
             Model residuals chart data
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
+        ValueError
+            If data_slice_filter passed as None
         """
 
         insight_name = "residuals"
 
+        self._validate_data_slice_filter(data_slice_filter)
+
         if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
             data_slice_filter = DataSlice(id=None)
 
         params = self._data_slice_to_query_params(data_slice_filter)
         params["source"] = source
 
         try:
             insights_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_url, params=params).json()
             response_data = self._get_sliced_insight_from_parent(
                 paginated_response, insight_name, params, fallback_to_parent_insights
             )
+
+            if len(response_data) == 0:
+                raise ClientError("Requested insight does not exist.", 404)
+
             response_data = response_data[0]
             use_insights_format = True
         except ClientError as e:
             self._raise_if_not_slice_forbidden_error(e)
             url_template = "projects/{}/models/{}/residuals/{}/"
             response_data = self._get_insight(
                 url_template,
@@ -2656,48 +2714,56 @@
             (New in version v2.14) Optional, if True, this will return ROC curve data for this
             model's parent if the ROC curve is not available for this model and the model has a
             defined parent model. If omitted or False, or there is no parent model, will not
             attempt to return data from this model's parent.
         data_slice_filter : DataSlice, optional
             A dataslice used to filter the return values based on the dataslice.id. By default this function will
             use data_slice_filter.id == None which returns an unsliced insight. If data_slice_filter is None
-            then no data_slice filtering will be applied when requesting the roc_curve.
+            then get_roc_curve will raise a ValueError.
 
         Returns
         -------
         RocCurve
             Model ROC curve data
 
         Raises
         ------
         ClientError
             If the insight is not available for this model
         (New in version v3.0) TypeError
             If the underlying project type is multilabel
+        ValueError
+            If data_slice_filter passed as None
         """
         if self.project.target_type == TARGET_TYPE.MULTILABEL:
             error_message = (
                 "Model.get_roc_curve should be used for binary projects. "
                 "Please use Model.get_labelwise_roc_curves API for multilabel models."
             )
             raise TypeError(error_message)
 
+        self._validate_data_slice_filter(data_slice_filter)
+
         if data_slice_filter is DATA_SLICE_WITH_ID_NONE:
             data_slice_filter = DataSlice(id=None)
 
         insight_name = "rocCurve"
         params = self._data_slice_to_query_params(data_slice_filter)
         params["source"] = source
 
         try:
             insights_url = self._get_insights_url(insight_name)
             paginated_response = self._client.get(insights_url, params=params).json()
             response_data = self._get_sliced_insight_from_parent(
                 paginated_response, insight_name, params, fallback_to_parent_insights
             )
+
+            if len(response_data) == 0:
+                raise ClientError("Requested insight does not exist.", 404)
+
             response_data = response_data[0]
             use_insights_format = True
         except ClientError as e:
             self._raise_if_not_slice_forbidden_error(e)
             url_template = "projects/{}/models/{}/rocCurve/{}/"
 
             response_data = self._get_insight(
@@ -2726,20 +2792,15 @@
         data_slice_filter : DataSlice, optional
             filters the returned roc_curve by data_slice_filter.id.  If None (the default) applies no filter based on
             data_slice_id.
 
         Returns
         -------
         list of RocCurve
-            Data for all available model ROC curves.
-
-        Raises
-        ------
-        ClientError
-            If the insight is not available for this model.
+            Data for all available model ROC curves. Or an empty list if no RocCurves are found.
 
         Examples
         --------
         .. code-block:: python
 
             model = datarobot.Model.get('project-id', 'model-id')
             ds_filter=DataSlice(id='data-slice-id')
@@ -5914,15 +5975,17 @@
             )
         from .job import (  # pylint: disable=import-outside-toplevel,cyclic-import
             filter_feature_impact_result,
         )
 
         return filter_feature_impact_result(valid_vata, with_metadata=with_metadata)
 
-    def request_feature_impact(self, row_count=None, with_metadata=False, backtest=None):
+    def request_feature_impact(
+        self, row_count=None, with_metadata=False, backtest=None
+    ):  # pylint: disable=arguments-renamed
         """
         Request feature impacts to be computed for the model.
 
         See :meth:`get_feature_impact <datarobot.models.Model.get_feature_impact>` for more
         information on the result of the job.
 
         Parameters
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/modeljob.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/modeljob.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/pairwise_statistics.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/pairwise_statistics.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/pareto_front.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/pareto_front.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/payoff_matrix.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/payoff_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/predict_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/predict_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_dataset.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_explanations.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_explanations.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prediction_server.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prediction_server.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/predictions.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/prime_file.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/prime_file.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/project.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/project.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/project_options.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/project_options.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/rating_table.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/rating_table.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/recommended_model.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/recommended_model.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/relationships_configuration.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/relationships_configuration.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/residuals.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/residuals.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/restore_discarded_features.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/restore_discarded_features.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/roc_curve.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/roc_curve.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/ruleset.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/ruleset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/secondary_dataset.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/secondary_dataset.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/segmentation.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/segmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_impact.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_impact.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_matrix.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_matrix.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/shap_matrix_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/shap_matrix_job.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/sharing.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/sharing.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/status_check_job.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/status_check_job.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
 
         safe_data = self.converter.check(from_api(data))
 
         return JobStatusResult(
             status=safe_data.get("status"),
             status_id=safe_data.get("statusId"),
             completed_resource_url=completed_resource_url,
+            message=safe_data.get("message"),
         )
 
     @classmethod
     def _job_path(cls, job_id: str) -> str:
         return f"status/{job_id}/"
 
     def _this_job_path(self) -> str:
@@ -101,16 +102,18 @@
         Returns
         -------
         status : JobStatusResult
             Returns the current status of the job.
         """
         try:
             wait_for_async_resolution(self._client, self._this_job_path(), max_wait=max_wait)
-        except (AsyncFailureError, AsyncProcessUnsuccessfulError):
-            return self.status_from_response(data={"status": ASYNC_PROCESS_STATUS.ERROR})
+        except (AsyncFailureError, AsyncProcessUnsuccessfulError) as ex:
+            return self.status_from_response(
+                data={"status": ASYNC_PROCESS_STATUS.ERROR, "message": str(ex)}
+            )
         except AsyncTimeoutError:
             pass  # just return current status to user
 
         return self.get_status()
 
     def get_status(self) -> JobStatusResult:
         """
@@ -136,7 +139,8 @@
     """
     This class represents a result of status check for submitted async jobs.
     """
 
     status: Optional[str]
     status_id: Optional[str]
     completed_resource_url: Optional[str]
+    message: Optional[str]
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/trafarets.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/training_predictions.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/training_predictions.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/types.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/types.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/use_case.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/use_case.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/use_cases/utils.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/use_cases/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,16 +112,22 @@
 
 
 def add_to_use_case(
     allow_multiple: bool,
 ) -> Callable[[Callable[P, T]], Callable[..., T]]:
     """
     A decorator to mark functions as adding the return value to a given Use Case. When implemented,
-    the decorator will add a `use_cases` keyword-only argument to the decorated function or method that
-    will automatically add the returned object to a Use Case.
+    the decorator will:
+
+    1. add a `use_cases` keyword-only argument to the decorated function or method,
+    2. add logic to automatically add the returned object to a Use Case, AFTER the decorated function
+       has finished executing.
+
+    This invokes the UseCase API and does NOT require the underlying route / SmartController to
+    consume a use_case_id as an argument.
 
     Parameters
     ----------
     allow_multiple : bool
         Whether the function should be decorated to permit adding to multiple use cases. Default is False.
 
     Examples
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/models.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/models.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/user_blueprints/trafarets.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/user_blueprints/trafarets.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/validators.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/validators.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/augmentation.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/augmentation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/images.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/images.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/visualai/insights.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/visualai/insights.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/models/word_cloud.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/models/word_cloud.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/rest.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/rest.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/__init__.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/deprecation.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/pagination.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/retry.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/retry.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/source.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/source.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/sourcedata.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/sourcedata.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot/utils/waiters.py` & `datarobot_early_access-3.3.0.2023.7.17/datarobot/utils/waiters.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     """
     start_time = time.time()
 
     join_endpoint = not url.startswith("http")  # Accept full qualified and relative urls
 
     response = client.get(url, allow_redirects=False, join_endpoint=join_endpoint)
     while time.time() < start_time + max_wait:
-        if response.status_code not in (200, 303):
+        if response.status_code not in (200, 303, 307):
             e_template = "The server gave an unexpected response. Status Code {}: {}"
             raise errors.AsyncFailureError(e_template.format(response.status_code, response.text))
         is_successful = success_fn(response)
 
         if is_successful:
             return is_successful
 
@@ -112,14 +112,16 @@
     AsyncProcessUnsuccessfulError
         If the job being waited for has failed or has been cancelled.
     AsyncTimeoutError
         If the resource did not resolve in time
     """
 
     def async_resolved(response: Response) -> Any:
+        if response.status_code == 307:
+            response = client.get(response.headers["Location"], allow_redirects=False)
         if response.status_code == 303:
             return response.headers["Location"]
         data = response.json()
         if data["status"].lower()[:5] in ["error", "abort"]:
             e_template = "The job did not complete successfully. Job Data: {}"
             raise errors.AsyncProcessUnsuccessfulError(e_template.format(data))
         if data["status"].lower() == "completed":
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/PKG-INFO` & `datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datarobot-early-access
-Version: 3.2.0.2023.7.3
+Version: 3.3.0.2023.7.17
 Summary: This client library is designed to support the DataRobot API.
 Home-page: https://datarobot.com
 Author: datarobot
 Author-email: support@datarobot.com
 Maintainer: datarobot
 Maintainer-email: info@datarobot.com
 License: DataRobot Tool and Utility Agreement
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/SOURCES.txt` & `datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,24 @@
 datarobot/enums.py
 datarobot/errors.py
 datarobot/py.typed
 datarobot/rest.py
 datarobot/_experimental/__init__.py
 datarobot/_experimental/models/__init__.py
 datarobot/_experimental/models/data_matching.py
+datarobot/_experimental/models/dataset.py
 datarobot/_experimental/models/enums.py
 datarobot/_experimental/models/idiomatic_project.py
 datarobot/_experimental/models/model.py
 datarobot/_experimental/models/model_lineage.py
 datarobot/_experimental/models/model_package.py
 datarobot/_experimental/models/notebooks.py
 datarobot/_experimental/models/project_options.py
+datarobot/_experimental/models/recipe_operations.py
+datarobot/_experimental/models/recipes.py
 datarobot/_experimental/models/retraining.py
 datarobot/_experimental/models/documentai/__init__.py
 datarobot/_experimental/models/documentai/document.py
 datarobot/helpers/__init__.py
 datarobot/helpers/binary_data_utils.py
 datarobot/helpers/eligibility_result.py
 datarobot/helpers/feature_discovery.py
```

### Comparing `datarobot_early_access-3.2.0.2023.7.3/datarobot_early_access.egg-info/requires.txt` & `datarobot_early_access-3.3.0.2023.7.17/datarobot_early_access.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/pyproject.toml` & `datarobot_early_access-3.3.0.2023.7.17/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/setup.py` & `datarobot_early_access-3.3.0.2023.7.17/setup.py`

 * *Files identical despite different names*

### Comparing `datarobot_early_access-3.2.0.2023.7.3/setup_weekly.py` & `datarobot_early_access-3.3.0.2023.7.17/setup_weekly.py`

 * *Files identical despite different names*

