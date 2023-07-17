# Comparing `tmp/wallaroo-2023.2.1rc1.tar.gz` & `tmp/wallaroo-2023.2.1rc2.tar.gz`

## Comparing `wallaroo-2023.2.1rc1.tar` & `wallaroo-2023.2.1rc2.tar`

### file list

```diff
@@ -1,1563 +1,1625 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/.DS_Store
--rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/.coverage
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/Dockerfile
--rw-r--r--   0        0        0     4732 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/Makefile
--rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/README.md
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/_version.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/mypy.ini
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/pytest.ini
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/requirements.txt
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/.gitignore
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/make.bat
--rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/autoscaling.ipynb
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/conf.py
--rw-r--r--   0        0        0    16542 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/core-abstractions.ipynb
--rw-r--r--   0        0        0    97557 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/email.png
--rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/experiments.ipynb
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/index.rst
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/jupyter.md
--rw-r--r--   0        0        0  1202751 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model-insights.ipynb
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion.rst
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_keras.ipynb
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_sklearn.ipynb
--rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_xgboost.ipynb
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/models.ipynb
--rw-r--r--   0        0        0    36022 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/monitoring.ipynb
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/overview.md
--rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/python-processing.ipynb
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/sdk.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/single-sign-on.md
--rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/standalone-mode.ipynb
--rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/workspaces.ipynb
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/BikeShareRegressor.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/demand_curve.pickle
--rw-r--r--   0        0        0    55124 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/isolet_xgboost_model.pickle
--rw-r--r--   0        0        0   339061 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt
--rw-r--r--   0        0        0    16201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/sentiment_model.zip
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/doc_app.py
--rw-r--r--   0        0        0    45048 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/ModelConversion.html
--rw-r--r--   0        0        0    37610 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/assay.html
--rw-r--r--   0        0        0    92157 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/assay_config.html
--rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/auth.html
--rw-r--r--   0        0        0    41365 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/checks.html
--rw-r--r--   0        0        0    86995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/client.html
--rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/comment.html
--rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/connection.html
--rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/datasizeunit.html
--rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/deployment.html
--rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/deployment_config.html
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/engine_config.html
--rw-r--r--   0        0        0    61794 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/explainability.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/expression.html
--rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/framework.html
--rw-r--r--   0        0        0    17152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/functions.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql.html
--rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/inference_decode.html
--rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/inference_result.html
--rw-r--r--   0        0        0    23071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/logs.html
--rw-r--r--   0        0        0    35292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/model.html
--rw-r--r--   0        0        0    25359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/model_config.html
--rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/models.html
--rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/notify.html
--rw-r--r--   0        0        0    39062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/object.html
--rw-r--r--   0        0        0    37539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/orchestration.html
--rw-r--r--   0        0        0    70395 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/pipeline.html
--rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/pipeline_config.html
--rw-r--r--   0        0        0    27690 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/pipeline_variant.html
--rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/queries.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records.html
--rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/standalone_client.html
--rw-r--r--   0        0        0    26746 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/tag.html
--rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/task.html
--rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/unwrap.html
--rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/user.html
--rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/user_type.html
--rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/utils.html
--rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/version.html
--rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/visibility.html
--rw-r--r--   0        0        0    30345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client.html
--rw-r--r--   0        0        0    30487 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/workspace.html
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/Assays.html
--rw-r--r--   0        0        0    17176 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/Workspaces.html
--rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/explainability.html
--rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/models.html
--rw-r--r--   0        0        0    17164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/orch.html
--rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/pipelines.html
--rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/graphql/tasks.html
--rw-r--r--   0        0        0    31550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/convert_keras_model.html
--rw-r--r--   0        0        0    17186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/graphql_queries.html
--rw-r--r--   0        0        0    42591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/telemetry_body.html
--rw-r--r--   0        0        0    22224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/telemetry_error.html
--rw-r--r--   0        0        0    30662 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/v1_metric_response.html
--rw-r--r--   0        0        0    22631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/records/v1_tls_response.html
--rw-r--r--   0        0        0    35762 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api.html
--rw-r--r--   0        0        0    91511 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/client.html
--rw-r--r--   0        0        0   251776 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models.html
--rw-r--r--   0        0        0    57883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/types.html
--rw-r--r--   0        0        0    34852 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html
--rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html
--rw-r--r--   0        0        0    35695 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html
--rw-r--r--   0        0        0    34792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html
--rw-r--r--   0        0        0    35222 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html
--rw-r--r--   0        0        0    34996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html
--rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html
--rw-r--r--   0        0        0    35099 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html
--rw-r--r--   0        0        0    34932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html
--rw-r--r--   0        0        0    35100 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html
--rw-r--r--   0        0        0   103915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html
--rw-r--r--   0        0        0   103903 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html
--rw-r--r--   0        0        0    96536 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html
--rw-r--r--   0        0        0    94546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html
--rw-r--r--   0        0        0    94354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html
--rw-r--r--   0        0        0   102532 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html
--rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html
--rw-r--r--   0        0        0    98489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html
--rw-r--r--   0        0        0   101224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html
--rw-r--r--   0        0        0   102809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html
--rw-r--r--   0        0        0    97798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html
--rw-r--r--   0        0        0   104246 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html
--rw-r--r--   0        0        0   105823 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html
--rw-r--r--   0        0        0   101555 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html
--rw-r--r--   0        0        0   101740 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html
--rw-r--r--   0        0        0   101327 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html
--rw-r--r--   0        0        0    90484 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html
--rw-r--r--   0        0        0    95036 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html
--rw-r--r--   0        0        0   106882 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html
--rw-r--r--   0        0        0   104529 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html
--rw-r--r--   0        0        0    77244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html
--rw-r--r--   0        0        0   101018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html
--rw-r--r--   0        0        0    96704 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html
--rw-r--r--   0        0        0    96492 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html
--rw-r--r--   0        0        0   100867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html
--rw-r--r--   0        0        0    97263 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html
--rw-r--r--   0        0        0   117840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html
--rw-r--r--   0        0        0    98796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html
--rw-r--r--   0        0        0    99321 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html
--rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html
--rw-r--r--   0        0        0    97607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html
--rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html
--rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html
--rw-r--r--   0        0        0   100741 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html
--rw-r--r--   0        0        0    98851 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html
--rw-r--r--   0        0        0    97387 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html
--rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html
--rw-r--r--   0        0        0   101796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html
--rw-r--r--   0        0        0    99500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html
--rw-r--r--   0        0        0    90132 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html
--rw-r--r--   0        0        0    97111 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html
--rw-r--r--   0        0        0    97527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html
--rw-r--r--   0        0        0    97283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html
--rw-r--r--   0        0        0    96571 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html
--rw-r--r--   0        0        0    98574 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html
--rw-r--r--   0        0        0    97932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html
--rw-r--r--   0        0        0    97500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html
--rw-r--r--   0        0        0   100083 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html
--rw-r--r--   0        0        0    99319 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html
--rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html
--rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html
--rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html
--rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html
--rw-r--r--   0        0        0   247398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html
--rw-r--r--   0        0        0    77057 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    76000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    76698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    89869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    76792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    90314 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   137892 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    47768 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    45477 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    81740 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    45501 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   108406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html
--rw-r--r--   0        0        0    72211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html
--rw-r--r--   0        0        0   116441 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html
--rw-r--r--   0        0        0    82564 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html
--rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html
--rw-r--r--   0        0        0   255712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html
--rw-r--r--   0        0        0    78641 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html
--rw-r--r--   0        0        0    77371 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    78282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html
--rw-r--r--   0        0        0    91786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    78376 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html
--rw-r--r--   0        0        0    92231 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   141854 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    48924 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48409 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   110939 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html
--rw-r--r--   0        0        0    87219 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html
--rw-r--r--   0        0        0   225352 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html
--rw-r--r--   0        0        0   179675 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    49043 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html
--rw-r--r--   0        0        0   146962 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49751 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46721 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46745 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   178307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    78631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html
--rw-r--r--   0        0        0   110252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html
--rw-r--r--   0        0        0    68384 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html
--rw-r--r--   0        0        0   104659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html
--rw-r--r--   0        0        0   220093 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html
--rw-r--r--   0        0        0   176239 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49288 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    48549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html
--rw-r--r--   0        0        0   144127 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50133 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46332 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    84522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   174871 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html
--rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html
--rw-r--r--   0        0        0    74300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html
--rw-r--r--   0        0        0   268583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html
--rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html
--rw-r--r--   0        0        0    76983 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    77834 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html
--rw-r--r--   0        0        0    91242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    77928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html
--rw-r--r--   0        0        0    91687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   140730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49541 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83006 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    45890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   110339 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html
--rw-r--r--   0        0        0   267313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html
--rw-r--r--   0        0        0    80673 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    79130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    80314 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    94247 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    80408 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    94692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   146937 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50623 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85772 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    46741 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   114192 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html
--rw-r--r--   0        0        0    69546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html
--rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html
--rw-r--r--   0        0        0   257261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html
--rw-r--r--   0        0        0    78865 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html
--rw-r--r--   0        0        0    77565 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html
--rw-r--r--   0        0        0    78506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html
--rw-r--r--   0        0        0    92058 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html
--rw-r--r--   0        0        0    78600 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html
--rw-r--r--   0        0        0    92503 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html
--rw-r--r--   0        0        0   142416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    49835 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    48500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46097 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html
--rw-r--r--   0        0        0    83756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html
--rw-r--r--   0        0        0    46121 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html
--rw-r--r--   0        0        0   111299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html
--rw-r--r--   0        0        0   224337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html
--rw-r--r--   0        0        0   178975 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html
--rw-r--r--   0        0        0    49652 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html
--rw-r--r--   0        0        0    48941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html
--rw-r--r--   0        0        0   146375 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html
--rw-r--r--   0        0        0    49656 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html
--rw-r--r--   0        0        0    50525 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html
--rw-r--r--   0        0        0    49141 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html
--rw-r--r--   0        0        0    46640 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html
--rw-r--r--   0        0        0    85522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html
--rw-r--r--   0        0        0    46664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html
--rw-r--r--   0        0        0   177607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html
--rw-r--r--   0        0        0    49470 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html
--rw-r--r--   0        0        0    76814 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html
--rw-r--r--   0        0        0    77468 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html
--rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html
--rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html
--rw-r--r--   0        0        0    79738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html
--rw-r--r--   0        0        0    69201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html
--rw-r--r--   0        0        0   159996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html
--rw-r--r--   0        0        0    96970 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html
--rw-r--r--   0        0        0    96196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html
--rw-r--r--   0        0        0    69367 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html
--rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html
--rw-r--r--   0        0        0    74075 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html
--rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html
--rw-r--r--   0        0        0    74305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html
--rw-r--r--   0        0        0    68869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html
--rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html
--rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html
--rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html
--rw-r--r--   0        0        0    74445 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html
--rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html
--rw-r--r--   0        0        0    76003 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html
--rw-r--r--   0        0        0    71398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html
--rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html
--rw-r--r--   0        0        0    69712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html
--rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html
--rw-r--r--   0        0        0    74738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html
--rw-r--r--   0        0        0    69878 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html
--rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html
--rw-r--r--   0        0        0    84036 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html
--rw-r--r--   0        0        0    68211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html
--rw-r--r--   0        0        0    70842 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html
--rw-r--r--   0        0        0   110748 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html
--rw-r--r--   0        0        0   114100 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html
--rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html
--rw-r--r--   0        0        0    71360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html
--rw-r--r--   0        0        0    81687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html
--rw-r--r--   0        0        0    99356 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html
--rw-r--r--   0        0        0    83498 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html
--rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html
--rw-r--r--   0        0        0   105405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html
--rw-r--r--   0        0        0    46114 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html
--rw-r--r--   0        0        0    86971 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html
--rw-r--r--   0        0        0    85711 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html
--rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html
--rw-r--r--   0        0        0    78923 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html
--rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html
--rw-r--r--   0        0        0    88601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html
--rw-r--r--   0        0        0    87371 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html
--rw-r--r--   0        0        0    90725 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html
--rw-r--r--   0        0        0    80112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html
--rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html
--rw-r--r--   0        0        0    45522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html
--rw-r--r--   0        0        0   119549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html
--rw-r--r--   0        0        0    70280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html
--rw-r--r--   0        0        0   107861 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html
--rw-r--r--   0        0        0    75696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html
--rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html
--rw-r--r--   0        0        0    96500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html
--rw-r--r--   0        0        0    68859 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html
--rw-r--r--   0        0        0    83809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html
--rw-r--r--   0        0        0   155198 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html
--rw-r--r--   0        0        0    69238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html
--rw-r--r--   0        0        0    83368 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html
--rw-r--r--   0        0        0    72567 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html
--rw-r--r--   0        0        0    83727 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html
--rw-r--r--   0        0        0    67694 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html
--rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html
--rw-r--r--   0        0        0    83009 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html
--rw-r--r--   0        0        0    75223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html
--rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html
--rw-r--r--   0        0        0    91489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html
--rw-r--r--   0        0        0    73642 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html
--rw-r--r--   0        0        0    72867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html
--rw-r--r--   0        0        0   146363 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html
--rw-r--r--   0        0        0    79269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html
--rw-r--r--   0        0        0   143833 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html
--rw-r--r--   0        0        0    48904 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html
--rw-r--r--   0        0        0    72317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html
--rw-r--r--   0        0        0    51426 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html
--rw-r--r--   0        0        0   122335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html
--rw-r--r--   0        0        0   142755 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html
--rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html
--rw-r--r--   0        0        0    71968 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html
--rw-r--r--   0        0        0    51212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html
--rw-r--r--   0        0        0    72505 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html
--rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html
--rw-r--r--   0        0        0    78096 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html
--rw-r--r--   0        0        0   141171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html
--rw-r--r--   0        0        0    48445 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html
--rw-r--r--   0        0        0    71464 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html
--rw-r--r--   0        0        0    50897 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html
--rw-r--r--   0        0        0    87540 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html
--rw-r--r--   0        0        0   143811 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html
--rw-r--r--   0        0        0    48900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html
--rw-r--r--   0        0        0    72304 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html
--rw-r--r--   0        0        0    51422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html
--rw-r--r--   0        0        0    47341 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html
--rw-r--r--   0        0        0    71728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html
--rw-r--r--   0        0        0    67391 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html
--rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html
--rw-r--r--   0        0        0    72120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html
--rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html
--rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html
--rw-r--r--   0        0        0    79001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html
--rw-r--r--   0        0        0    76665 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html
--rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html
--rw-r--r--   0        0        0    81109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html
--rw-r--r--   0        0        0    74260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html
--rw-r--r--   0        0        0    79975 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html
--rw-r--r--   0        0        0    70389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html
--rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html
--rw-r--r--   0        0        0    72475 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html
--rw-r--r--   0        0        0    88028 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html
--rw-r--r--   0        0        0   109802 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html
--rw-r--r--   0        0        0    71831 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html
--rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html
--rw-r--r--   0        0        0    72851 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html
--rw-r--r--   0        0        0   126961 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html
--rw-r--r--   0        0        0   110890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html
--rw-r--r--   0        0        0    72361 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html
--rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html
--rw-r--r--   0        0        0    71840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html
--rw-r--r--   0        0        0    75030 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html
--rw-r--r--   0        0        0   279449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html
--rw-r--r--   0        0        0   235836 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html
--rw-r--r--   0        0        0    72127 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html
--rw-r--r--   0        0        0    72293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html
--rw-r--r--   0        0        0    46678 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html
--rw-r--r--   0        0        0    46642 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html
--rw-r--r--   0        0        0    46786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html
--rw-r--r--   0        0        0    46726 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html
--rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html
--rw-r--r--   0        0        0    78265 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html
--rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html
--rw-r--r--   0        0        0    45429 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html
--rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html
--rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html
--rw-r--r--   0        0        0    45321 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html
--rw-r--r--   0        0        0    45465 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html
--rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html
--rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html
--rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html
--rw-r--r--   0        0        0    45455 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html
--rw-r--r--   0        0        0    45575 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html
--rw-r--r--   0        0        0    45491 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html
--rw-r--r--   0        0        0    75329 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html
--rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html
--rw-r--r--   0        0        0   169074 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html
--rw-r--r--   0        0        0    46366 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html
--rw-r--r--   0        0        0    46330 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html
--rw-r--r--   0        0        0    46474 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html
--rw-r--r--   0        0        0    46414 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html
--rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html
--rw-r--r--   0        0        0    77476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html
--rw-r--r--   0        0        0    87286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html
--rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html
--rw-r--r--   0        0        0    47034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    47058 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    79041 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html
--rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html
--rw-r--r--   0        0        0   154233 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html
--rw-r--r--   0        0        0    45434 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html
--rw-r--r--   0        0        0    45398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html
--rw-r--r--   0        0        0    45542 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html
--rw-r--r--   0        0        0    45482 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html
--rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html
--rw-r--r--   0        0        0    75122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html
--rw-r--r--   0        0        0    83570 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html
--rw-r--r--   0        0        0   123274 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html
--rw-r--r--   0        0        0    46102 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    46126 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    76687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html
--rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html
--rw-r--r--   0        0        0    73401 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html
--rw-r--r--   0        0        0    84383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html
--rw-r--r--   0        0        0   219068 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html
--rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html
--rw-r--r--   0        0        0    46357 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html
--rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html
--rw-r--r--   0        0        0    46285 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html
--rw-r--r--   0        0        0    46249 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html
--rw-r--r--   0        0        0    46393 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html
--rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html
--rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html
--rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html
--rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html
--rw-r--r--   0        0        0   129869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html
--rw-r--r--   0        0        0    69164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html
--rw-r--r--   0        0        0    68285 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html
--rw-r--r--   0        0        0    50899 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html
--rw-r--r--   0        0        0    74827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html
--rw-r--r--   0        0        0   164435 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html
--rw-r--r--   0        0        0    45272 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html
--rw-r--r--   0        0        0    45236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html
--rw-r--r--   0        0        0    45380 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html
--rw-r--r--   0        0        0    45320 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html
--rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html
--rw-r--r--   0        0        0    74708 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html
--rw-r--r--   0        0        0    76620 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html
--rw-r--r--   0        0        0   102591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html
--rw-r--r--   0        0        0    68109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html
--rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html
--rw-r--r--   0        0        0    72650 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html
--rw-r--r--   0        0        0    73154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html
--rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html
--rw-r--r--   0        0        0    74934 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html
--rw-r--r--   0        0        0    83034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html
--rw-r--r--   0        0        0   112145 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html
--rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html
--rw-r--r--   0        0        0    73182 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html
--rw-r--r--   0        0        0    84128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html
--rw-r--r--   0        0        0    83709 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html
--rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html
--rw-r--r--   0        0        0    88686 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html
--rw-r--r--   0        0        0    74176 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html
--rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html
--rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/pdoc_templates/frame.html.jinja2
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/pdoc_templates/module.html.jinja2
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/__init__.py
--rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/reusable_responders.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/status_samples.py
--rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_assay.py
--rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_assay_config.py
--rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_auth.py
--rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_checks.py
--rw-r--r--   0        0        0    49752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_client.py
--rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_comment.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_connection.py
--rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_deployment.py
--rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_deployment_config.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_engine_config.py
--rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_explainability.py
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_import.py
--rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_inference_result.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_log_entries.py
--rw-r--r--   0        0        0    20326 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_model.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_model_config.py
--rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_models.py
--rw-r--r--   0        0        0    23297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_pipeline.py
--rw-r--r--   0        0        0    34999 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_pipeline_config.py
--rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_pipeline_variant.py
--rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_tag.py
--rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/test_workspace.py
--rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/testutil.py
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/.DS_Store
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/ccfraud_output.json
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/day5_output.json
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.arrow
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.pandas.json
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.txt
--rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/lazyadam_output.json
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/pipeline_output.json
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_batched_inference_result.json
--rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.arrow
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.json
--rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.pandas.json
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_logged_inference_result.json
--rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/sample_logs.arrow
--rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/outputs/some_output.json
--rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json
--rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_model_drift/drift.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_model_drift/gauges.json
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_values_expression/gauges.json
--rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_values_expression/values.json
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/default_model_config.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/experiment_model_config.yaml
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/model_config.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/model_config.yaml
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_only_config.yaml
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_step_config.yaml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/post_model_config.yaml
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pre_model_config.yaml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/wl_model_config.yaml
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/challenger.yaml
--rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/control.yaml
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/control.yaml
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model2.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model3.yaml
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/model_config.yaml
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/pipeline_config.yaml
--rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/ModelConversion.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/__init__.py
--rw-r--r--   0        0        0    17522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/assay.py
--rw-r--r--   0        0        0    28077 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/assay_config.py
--rw-r--r--   0        0        0    27488 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/auth.py
--rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/checks.py
--rw-r--r--   0        0        0    84091 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/client.py
--rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/comment.py
--rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/connection.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/datasizeunit.py
--rw-r--r--   0        0        0    37000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/deployment.py
--rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/deployment_config.py
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/engine_config.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/explainability.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/expression.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/framework.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/functions.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/inference_decode.py
--rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/inference_result.py
--rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/logs.py
--rw-r--r--   0        0        0    17966 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/model.py
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/model_config.py
--rw-r--r--   0        0        0    14586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/model_registry.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/models.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/notify.py
--rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/object.py
--rw-r--r--   0        0        0    15260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/orchestration.py
--rw-r--r--   0        0        0    43650 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/pipeline.py
--rw-r--r--   0        0        0    26383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/pipeline_config.py
--rw-r--r--   0        0        0     8286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/pipeline_variant.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/queries.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/standalone_client.py
--rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/tag.py
--rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/task.py
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/task_run.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/unwrap.py
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/user.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/user_type.py
--rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/utils.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/version.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/visibility.py
--rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/workspace.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateConnection.graphql
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDeployment.graphql
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateTag.graphql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspace.graphql
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspaceBare.graphql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspaceConnection.graphql
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteConnection.graphql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteWorkspaceConnection.graphql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteWorkspaceUser.graphql
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConfiguredModelById.graphql
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConnection.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConnectionById.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetDeploymentForPipeline.graphql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModel.graphql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelById.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelByTaskId.graphql
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelConfigs.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelVersionById.graphql
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModels.graphql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineAndWorkspace.graphql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineByIdForCopying.graphql
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineByName.graphql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineVersion.graphql
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelinesForModels.graphql
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertConfiguredModel.graphql
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentModelConfig.graphql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModel.graphql
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModelConfig.graphql
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModelConfigFull.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertWorkspaceUser.graphql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListConnections.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListDeployments.graphql
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListModelConversions.graphql
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListModels.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListPipelines.graphql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListWorkspaces.graphql
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ModelByName.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/PipelineModels.graphql
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/PipelineVariantById.graphql
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/README.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Undeploy.graphql
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModel.graphql
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UserDefaultWorkspace.graphql
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceById.graphql
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceByName.graphql
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceListConnections.graphql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceNameById.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/AssaySetActive.graphql
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/CreateAssay.graphql
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/FilterAssays.graphql
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/GetAssayResults.graphql
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/ListAssays.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetLatestModelConfig.graphql
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModel.graphql
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModelVersions.graphql
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModels.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/GetOrchestration.graphql
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/InsertOrchestration.graphql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/ListOrchestrations.graphql
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/UpdateOrchestration.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/__init__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/AttachRegistryToWorkspace.graphql
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/CreateRegistry.graphql
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/GetRegistry.graphql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/ListRegistries.graphql
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/RemoveRegistryFromWorkspace.graphql
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetLogsForRun.graphql
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTaskById.graphql
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTaskRun.graphql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTasksByOrchSha.graphql
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/InsertTask.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/InsertTaskRun.graphql
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTaskRuns.graphql
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasks.graphql
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/README.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/SetTaskKilled.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/StartTaskRun.graphql
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTask.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTaskRun.graphql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/__init__.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/README.md
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/__init__.py
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/convert_keras_model.py
--rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/graphql_queries.py
--rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/telemetry_body.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/telemetry_error.py
--rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/v1_metric_response.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/records/v1_tls_response.py
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/__init__.py
--rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/client.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/errors.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/types.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/__init__.py
--rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py
--rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/__init__.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py
--rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py
--rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py
--rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py
--rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/__init__.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py
--rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py
--rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py
--rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py
--rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py
--rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/__init__.py
--rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py
--rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py
--rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py
--rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py
--rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py
--rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py
--rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py
--rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/__init__.py
--rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py
--rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/__init__.py
--rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/attach_registry_to_workspace.py
--rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/create_registry.py
--rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/get_model_version_by_id.py
--rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/get_registry.py
--rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registries.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registry_models.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py
--rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py
--rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py
--rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/remove_registry_from_workspace.py
--rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload1.py
--rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_and_convert.py
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_from_registry.py
--rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py
--rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/__init__.py
--rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py
--rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py
--rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/__init__.py
--rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py
--rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py
--rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py
--rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/__init__.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/get_publish_status.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/list_published_pipelines.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/publish_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/__init__.py
--rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py
--rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/__init__.py
--rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_logs_for_run.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_run_details.py
--rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_tasks_by_orch_sha.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py
--rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list_task_runs.py
--rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/__init__.py
--rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py
--rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py
--rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/__init__.py
--rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py
--rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py
--rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py
--rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py
--rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py
--rw-r--r--   0        0        0    61653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/arbex_status.py
--rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py
--rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py
--rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py
--rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.py
--rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py
--rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py
--rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py
--rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py
--rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py
--rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py
--rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py
--rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py
--rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py
--rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py
--rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py
--rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py
--rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.py
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.py
--rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py
--rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py
--rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.py
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_request.py
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response.py
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response_200.py
--rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py
--rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py
--rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_409.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py
--rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py
--rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py
--rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/conversion.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_request.py
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response.py
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response_200.py
--rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py
--rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py
--rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py
--rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py
--rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py
--rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py
--rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py
--rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py
--rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py
--rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py
--rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py
--rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py
--rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/file_info.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/framework.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_request.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response.py
--rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response_200.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_model_by_id_request.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py
--rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_request.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response.py
--rw-r--r--   0        0        0     3687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_200.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_workspace.py
--rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_request.py
--rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_response_200.py
--rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_request.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response_200.py
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_models.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_registries_request.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_registry_models_request.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_request.py
--rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request_status.py
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_response_task_runs.py
--rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py
--rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_id.py
--rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_registry.py
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_status.py
--rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_version.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py
--rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py
--rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py
--rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py
--rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py
--rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.py
--rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec_exec_type.py
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py
--rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration_status.py
--rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py
--rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py
--rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py
--rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py
--rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py
--rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py
--rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body_order.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_502.py
--rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py
--rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py
--rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py
--rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/publish_request.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/publish_response.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/python_version.py
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/registered_model.py
--rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/registered_model_version.py
--rw-r--r--   0        0        0     1808 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_request.py
--rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response.py
--rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response_200.py
--rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/search_registered_models_response.py
--rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py
--rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.py
--rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py
--rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py
--rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.py
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.py
--rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py
--rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py
--rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_request.py
--rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_run.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_status.py
--rw-r--r--   0        0        0     3832 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_request.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response_200.py
--rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc_1.py
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request_1.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response_1.py
--rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py
--rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py
--rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py
--rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py
--rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py
--rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py
--rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py
--rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py
--rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py
--rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateConnection.graphql
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDeployment.graphql
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateTag.graphql
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspace.graphql
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspaceBare.graphql
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/CreateWorkspaceConnection.graphql
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteConnection.graphql
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteWorkspaceConnection.graphql
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/DeleteWorkspaceUser.graphql
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConfiguredModelById.graphql
--rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConnection.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetConnectionById.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetDeploymentForPipeline.graphql
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModel.graphql
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelById.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelByTaskId.graphql
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelConfigs.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModelVersionById.graphql
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetModels.graphql
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineAndWorkspace.graphql
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineByIdForCopying.graphql
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineByName.graphql
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineVersion.graphql
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelinesForModels.graphql
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertConfiguredModel.graphql
--rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentModelConfig.graphql
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModel.graphql
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModelConfig.graphql
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModelConfigFull.graphql
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/InsertWorkspaceUser.graphql
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListConnections.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListDeployments.graphql
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListModelConversions.graphql
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListModels.graphql
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListPipelines.graphql
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ListWorkspaces.graphql
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/ModelByName.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/PipelineModels.graphql
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/PipelineVariantById.graphql
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/README.md
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Undeploy.graphql
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModel.graphql
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/UserDefaultWorkspace.graphql
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceById.graphql
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceByName.graphql
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceListConnections.graphql
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/WorkspaceNameById.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/AssaySetActive.graphql
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/CreateAssay.graphql
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/FilterAssays.graphql
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/GetAssayResults.graphql
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/ListAssays.graphql
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/__init__.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/Workspaces/__init__.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/__init__.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetLatestModelConfig.graphql
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModel.graphql
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModelVersions.graphql
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/GetModels.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/models/__init__.py
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/GetOrchestration.graphql
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/InsertOrchestration.graphql
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/ListOrchestrations.graphql
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/UpdateOrchestration.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/orch/__init__.py
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/__init__.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/AttachRegistryToWorkspace.graphql
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/CreateRegistry.graphql
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/GetRegistry.graphql
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/ListRegistries.graphql
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/registries/RemoveRegistryFromWorkspace.graphql
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetLogsForRun.graphql
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTaskById.graphql
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTaskRun.graphql
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/GetTasksByOrchSha.graphql
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/InsertTask.graphql
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/InsertTaskRun.graphql
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTaskRuns.graphql
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasks.graphql
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/README.md
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/SetTaskKilled.graphql
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/StartTaskRun.graphql
--rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTask.graphql
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTaskRun.graphql
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/__init__.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/.gitignore
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/public_README.md
--rw-r--r--   0        0        0     4704 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/pyproject.toml
--rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/.DS_Store
+-rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/.coverage
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/Dockerfile
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/Makefile
+-rw-r--r--   0        0        0     3030 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/README.md
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/_version.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mypy.ini
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/pytest.ini
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/requirements.txt
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/tensor_dropped_no_metadata.arrow
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/.gitignore
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/make.bat
+-rw-r--r--   0        0        0     2271 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/autoscaling.ipynb
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/conf.py
+-rw-r--r--   0        0        0    16542 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/core-abstractions.ipynb
+-rw-r--r--   0        0        0    97557 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/email.png
+-rw-r--r--   0        0        0    18932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/experiments.ipynb
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/index.rst
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/jupyter.md
+-rw-r--r--   0        0        0  1202751 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model-insights.ipynb
+-rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion.rst
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_keras.ipynb
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_sklearn.ipynb
+-rw-r--r--   0        0        0     3949 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_xgboost.ipynb
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/models.ipynb
+-rw-r--r--   0        0        0    36022 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/monitoring.ipynb
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/overview.md
+-rw-r--r--   0        0        0    13235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/python-processing.ipynb
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/sdk.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/single-sign-on.md
+-rw-r--r--   0        0        0    12444 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/standalone-mode.ipynb
+-rw-r--r--   0        0        0    16569 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/workspaces.ipynb
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/BikeShareRegressor.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/demand_curve.pickle
+-rw-r--r--   0        0        0    55124 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/isolet_xgboost_model.pickle
+-rw-r--r--   0        0        0   339061 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt
+-rw-r--r--   0        0        0    16201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/sentiment_model.zip
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/doc_app.py
+-rw-r--r--   0        0        0    45048 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/ModelConversion.html
+-rw-r--r--   0        0        0    37610 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/assay.html
+-rw-r--r--   0        0        0    92157 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/assay_config.html
+-rw-r--r--   0        0        0    31123 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/auth.html
+-rw-r--r--   0        0        0    41365 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/checks.html
+-rw-r--r--   0        0        0    86995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/client.html
+-rw-r--r--   0        0        0    25318 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/comment.html
+-rw-r--r--   0        0        0    28571 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/connection.html
+-rw-r--r--   0        0        0    20833 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/datasizeunit.html
+-rw-r--r--   0        0        0    43756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/deployment.html
+-rw-r--r--   0        0        0    33510 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/deployment_config.html
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/engine_config.html
+-rw-r--r--   0        0        0    61794 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/explainability.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/expression.html
+-rw-r--r--   0        0        0    33076 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/framework.html
+-rw-r--r--   0        0        0    17152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/functions.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql.html
+-rw-r--r--   0        0        0    25039 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/inference_decode.html
+-rw-r--r--   0        0        0    23185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/inference_result.html
+-rw-r--r--   0        0        0    23071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/logs.html
+-rw-r--r--   0        0        0    35292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/model.html
+-rw-r--r--   0        0        0    25359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/model_config.html
+-rw-r--r--   0        0        0    24148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/models.html
+-rw-r--r--   0        0        0    23083 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/notify.html
+-rw-r--r--   0        0        0    39062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/object.html
+-rw-r--r--   0        0        0    37539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/orchestration.html
+-rw-r--r--   0        0        0    70395 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/pipeline.html
+-rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/pipeline_config.html
+-rw-r--r--   0        0        0    27690 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/pipeline_variant.html
+-rw-r--r--   0        0        0    17657 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/queries.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records.html
+-rw-r--r--   0        0        0    22344 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/standalone_client.html
+-rw-r--r--   0        0        0    26746 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/tag.html
+-rw-r--r--   0        0        0    26135 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/task.html
+-rw-r--r--   0        0        0    17856 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/unwrap.html
+-rw-r--r--   0        0        0    22292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/user.html
+-rw-r--r--   0        0        0    23063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/user_type.html
+-rw-r--r--   0        0        0    24899 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/utils.html
+-rw-r--r--   0        0        0    17148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/version.html
+-rw-r--r--   0        0        0    17154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/visibility.html
+-rw-r--r--   0        0        0    30345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client.html
+-rw-r--r--   0        0        0    30487 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/workspace.html
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/Assays.html
+-rw-r--r--   0        0        0    17176 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/Workspaces.html
+-rw-r--r--   0        0        0    17184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/explainability.html
+-rw-r--r--   0        0        0    17168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/models.html
+-rw-r--r--   0        0        0    17164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/orch.html
+-rw-r--r--   0        0        0    17174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/pipelines.html
+-rw-r--r--   0        0        0    17166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/graphql/tasks.html
+-rw-r--r--   0        0        0    31550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/convert_keras_model.html
+-rw-r--r--   0        0        0    17186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/graphql_queries.html
+-rw-r--r--   0        0        0    42591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/telemetry_body.html
+-rw-r--r--   0        0        0    22224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/telemetry_error.html
+-rw-r--r--   0        0        0    30662 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/v1_metric_response.html
+-rw-r--r--   0        0        0    22631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/records/v1_tls_response.html
+-rw-r--r--   0        0        0    35762 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api.html
+-rw-r--r--   0        0        0    91511 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/client.html
+-rw-r--r--   0        0        0   251776 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models.html
+-rw-r--r--   0        0        0    57883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/types.html
+-rw-r--r--   0        0        0    34852 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html
+-rw-r--r--   0        0        0    35428 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html
+-rw-r--r--   0        0        0    35695 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html
+-rw-r--r--   0        0        0    34792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html
+-rw-r--r--   0        0        0    35222 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html
+-rw-r--r--   0        0        0    34996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html
+-rw-r--r--   0        0        0    34842 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html
+-rw-r--r--   0        0        0    35099 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html
+-rw-r--r--   0        0        0    34932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html
+-rw-r--r--   0        0        0    35100 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html
+-rw-r--r--   0        0        0   103915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html
+-rw-r--r--   0        0        0   103903 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html
+-rw-r--r--   0        0        0    96536 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html
+-rw-r--r--   0        0        0    94546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html
+-rw-r--r--   0        0        0    94354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html
+-rw-r--r--   0        0        0   102532 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html
+-rw-r--r--   0        0        0   100091 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html
+-rw-r--r--   0        0        0    98489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html
+-rw-r--r--   0        0        0   101224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html
+-rw-r--r--   0        0        0   102809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html
+-rw-r--r--   0        0        0    97798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html
+-rw-r--r--   0        0        0   104246 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html
+-rw-r--r--   0        0        0   105823 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html
+-rw-r--r--   0        0        0   101555 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html
+-rw-r--r--   0        0        0   101740 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html
+-rw-r--r--   0        0        0   101327 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html
+-rw-r--r--   0        0        0    90484 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html
+-rw-r--r--   0        0        0    95036 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html
+-rw-r--r--   0        0        0   106882 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html
+-rw-r--r--   0        0        0   104529 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html
+-rw-r--r--   0        0        0    77244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html
+-rw-r--r--   0        0        0   101018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html
+-rw-r--r--   0        0        0    96704 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html
+-rw-r--r--   0        0        0    96492 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html
+-rw-r--r--   0        0        0   100867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html
+-rw-r--r--   0        0        0    97263 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html
+-rw-r--r--   0        0        0   117840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html
+-rw-r--r--   0        0        0    98796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html
+-rw-r--r--   0        0        0    99321 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html
+-rw-r--r--   0        0        0    99309 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html
+-rw-r--r--   0        0        0    97607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html
+-rw-r--r--   0        0        0    97511 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html
+-rw-r--r--   0        0        0   101888 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html
+-rw-r--r--   0        0        0   100741 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html
+-rw-r--r--   0        0        0    98851 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html
+-rw-r--r--   0        0        0    97387 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html
+-rw-r--r--   0        0        0    98563 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html
+-rw-r--r--   0        0        0   101796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html
+-rw-r--r--   0        0        0    99500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html
+-rw-r--r--   0        0        0    90132 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html
+-rw-r--r--   0        0        0    97111 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html
+-rw-r--r--   0        0        0    97527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html
+-rw-r--r--   0        0        0    97283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html
+-rw-r--r--   0        0        0    96571 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html
+-rw-r--r--   0        0        0    98574 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html
+-rw-r--r--   0        0        0    97932 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html
+-rw-r--r--   0        0        0    97500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html
+-rw-r--r--   0        0        0   100083 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html
+-rw-r--r--   0        0        0    99319 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html
+-rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html
+-rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html
+-rw-r--r--   0        0        0    80018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html
+-rw-r--r--   0        0        0    75031 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html
+-rw-r--r--   0        0        0   247398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html
+-rw-r--r--   0        0        0    77057 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    76000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    76698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    89869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    76792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    90314 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   137892 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    48283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49047 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    47768 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    45477 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    81740 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    45501 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   108406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html
+-rw-r--r--   0        0        0    72211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html
+-rw-r--r--   0        0        0   116441 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html
+-rw-r--r--   0        0        0    82564 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html
+-rw-r--r--   0        0        0    45578 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html
+-rw-r--r--   0        0        0   255712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html
+-rw-r--r--   0        0        0    78641 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html
+-rw-r--r--   0        0        0    77371 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    78282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html
+-rw-r--r--   0        0        0    91786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    78376 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html
+-rw-r--r--   0        0        0    92231 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   141854 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    48924 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49737 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48409 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   110939 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html
+-rw-r--r--   0        0        0    87219 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html
+-rw-r--r--   0        0        0   225352 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html
+-rw-r--r--   0        0        0   179675 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    49043 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html
+-rw-r--r--   0        0        0   146962 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49751 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46721 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46745 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   178307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49565 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    78631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html
+-rw-r--r--   0        0        0   110252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html
+-rw-r--r--   0        0        0    68384 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html
+-rw-r--r--   0        0        0   104659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html
+-rw-r--r--   0        0        0   220093 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html
+-rw-r--r--   0        0        0   176239 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49288 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    48549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html
+-rw-r--r--   0        0        0   144127 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49292 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50133 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48777 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46332 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    84522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46356 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   174871 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html
+-rw-r--r--   0        0        0    77508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html
+-rw-r--r--   0        0        0    74300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html
+-rw-r--r--   0        0        0   268583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html
+-rw-r--r--   0        0        0    78193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html
+-rw-r--r--   0        0        0    76983 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    77834 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html
+-rw-r--r--   0        0        0    91242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    77928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html
+-rw-r--r--   0        0        0    91687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   140730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    48742 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49541 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    45866 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83006 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    45890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   110339 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html
+-rw-r--r--   0        0        0   267313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html
+-rw-r--r--   0        0        0    80673 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    79130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    80314 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    94247 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    80408 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    94692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   146937 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    49747 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50623 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85772 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    46741 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   114192 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html
+-rw-r--r--   0        0        0    69546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html
+-rw-r--r--   0        0        0    80185 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html
+-rw-r--r--   0        0        0   257261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html
+-rw-r--r--   0        0        0    78865 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html
+-rw-r--r--   0        0        0    77565 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html
+-rw-r--r--   0        0        0    78506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html
+-rw-r--r--   0        0        0    92058 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html
+-rw-r--r--   0        0        0    78600 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html
+-rw-r--r--   0        0        0    92503 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html
+-rw-r--r--   0        0        0   142416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    49835 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    48500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46097 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    83756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html
+-rw-r--r--   0        0        0    46121 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   111299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html
+-rw-r--r--   0        0        0   224337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html
+-rw-r--r--   0        0        0   178975 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html
+-rw-r--r--   0        0        0    49652 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html
+-rw-r--r--   0        0        0    48941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html
+-rw-r--r--   0        0        0   146375 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html
+-rw-r--r--   0        0        0    49656 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html
+-rw-r--r--   0        0        0    50525 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html
+-rw-r--r--   0        0        0    49141 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html
+-rw-r--r--   0        0        0    46640 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html
+-rw-r--r--   0        0        0    85522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html
+-rw-r--r--   0        0        0    46664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html
+-rw-r--r--   0        0        0   177607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html
+-rw-r--r--   0        0        0    49470 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html
+-rw-r--r--   0        0        0    76814 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html
+-rw-r--r--   0        0        0    77468 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html
+-rw-r--r--   0        0        0    77286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html
+-rw-r--r--   0        0        0   156808 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html
+-rw-r--r--   0        0        0    79738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html
+-rw-r--r--   0        0        0    69201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html
+-rw-r--r--   0        0        0   159996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html
+-rw-r--r--   0        0        0    96970 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html
+-rw-r--r--   0        0        0    96196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html
+-rw-r--r--   0        0        0    69367 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html
+-rw-r--r--   0        0        0    79950 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html
+-rw-r--r--   0        0        0    74075 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html
+-rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html
+-rw-r--r--   0        0        0    74305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html
+-rw-r--r--   0        0        0    68869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html
+-rw-r--r--   0        0        0    79284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html
+-rw-r--r--   0        0        0    74516 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html
+-rw-r--r--   0        0        0    68703 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html
+-rw-r--r--   0        0        0    74445 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html
+-rw-r--r--   0        0        0    79062 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html
+-rw-r--r--   0        0        0    76003 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html
+-rw-r--r--   0        0        0    71398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html
+-rw-r--r--   0        0        0    81752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html
+-rw-r--r--   0        0        0    69712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html
+-rw-r--r--   0        0        0    79506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html
+-rw-r--r--   0        0        0    74738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html
+-rw-r--r--   0        0        0    69878 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html
+-rw-r--r--   0        0        0    79728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html
+-rw-r--r--   0        0        0    84036 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html
+-rw-r--r--   0        0        0    68211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html
+-rw-r--r--   0        0        0    70842 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html
+-rw-r--r--   0        0        0   110748 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html
+-rw-r--r--   0        0        0   114100 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html
+-rw-r--r--   0        0        0    75941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html
+-rw-r--r--   0        0        0    71360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html
+-rw-r--r--   0        0        0    81687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html
+-rw-r--r--   0        0        0    99356 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html
+-rw-r--r--   0        0        0    83498 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html
+-rw-r--r--   0        0        0   115258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html
+-rw-r--r--   0        0        0   105405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html
+-rw-r--r--   0        0        0    46114 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html
+-rw-r--r--   0        0        0    86971 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html
+-rw-r--r--   0        0        0    85711 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html
+-rw-r--r--   0        0        0    89065 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html
+-rw-r--r--   0        0        0    78923 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html
+-rw-r--r--   0        0        0    76607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html
+-rw-r--r--   0        0        0    88601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html
+-rw-r--r--   0        0        0    87371 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html
+-rw-r--r--   0        0        0    90725 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html
+-rw-r--r--   0        0        0    80112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html
+-rw-r--r--   0        0        0    77952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html
+-rw-r--r--   0        0        0    45522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html
+-rw-r--r--   0        0        0   119549 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html
+-rw-r--r--   0        0        0    70280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html
+-rw-r--r--   0        0        0   107861 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html
+-rw-r--r--   0        0        0    75696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html
+-rw-r--r--   0        0        0    78618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html
+-rw-r--r--   0        0        0    96500 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html
+-rw-r--r--   0        0        0    68859 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html
+-rw-r--r--   0        0        0    83809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html
+-rw-r--r--   0        0        0   155198 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html
+-rw-r--r--   0        0        0    69238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html
+-rw-r--r--   0        0        0    83368 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html
+-rw-r--r--   0        0        0    72567 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html
+-rw-r--r--   0        0        0    83727 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html
+-rw-r--r--   0        0        0    67694 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html
+-rw-r--r--   0        0        0    77717 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html
+-rw-r--r--   0        0        0    83009 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html
+-rw-r--r--   0        0        0    75223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html
+-rw-r--r--   0        0        0    79976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html
+-rw-r--r--   0        0        0    91489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html
+-rw-r--r--   0        0        0    73642 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html
+-rw-r--r--   0        0        0    72867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html
+-rw-r--r--   0        0        0   146363 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html
+-rw-r--r--   0        0        0    79269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html
+-rw-r--r--   0        0        0   143833 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html
+-rw-r--r--   0        0        0    48904 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html
+-rw-r--r--   0        0        0    72317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html
+-rw-r--r--   0        0        0    51426 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html
+-rw-r--r--   0        0        0   122335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html
+-rw-r--r--   0        0        0   142755 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html
+-rw-r--r--   0        0        0    48718 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html
+-rw-r--r--   0        0        0    71968 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html
+-rw-r--r--   0        0        0    51212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html
+-rw-r--r--   0        0        0    72505 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html
+-rw-r--r--   0        0        0    73018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html
+-rw-r--r--   0        0        0    78096 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html
+-rw-r--r--   0        0        0   141171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html
+-rw-r--r--   0        0        0    48445 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html
+-rw-r--r--   0        0        0    71464 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html
+-rw-r--r--   0        0        0    50897 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html
+-rw-r--r--   0        0        0    87540 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html
+-rw-r--r--   0        0        0   143811 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html
+-rw-r--r--   0        0        0    48900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html
+-rw-r--r--   0        0        0    72304 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html
+-rw-r--r--   0        0        0    51422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html
+-rw-r--r--   0        0        0    47341 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html
+-rw-r--r--   0        0        0    71728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html
+-rw-r--r--   0        0        0    67391 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html
+-rw-r--r--   0        0        0    76829 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html
+-rw-r--r--   0        0        0    72120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html
+-rw-r--r--   0        0        0    67727 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html
+-rw-r--r--   0        0        0    77273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html
+-rw-r--r--   0        0        0    79001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html
+-rw-r--r--   0        0        0    76665 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html
+-rw-r--r--   0        0        0    76385 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html
+-rw-r--r--   0        0        0    81109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html
+-rw-r--r--   0        0        0    74260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html
+-rw-r--r--   0        0        0    79975 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html
+-rw-r--r--   0        0        0    70389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html
+-rw-r--r--   0        0        0    76163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html
+-rw-r--r--   0        0        0    72475 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html
+-rw-r--r--   0        0        0    88028 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html
+-rw-r--r--   0        0        0   109802 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html
+-rw-r--r--   0        0        0    71831 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html
+-rw-r--r--   0        0        0    77521 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html
+-rw-r--r--   0        0        0    72851 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html
+-rw-r--r--   0        0        0   126961 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html
+-rw-r--r--   0        0        0   110890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html
+-rw-r--r--   0        0        0    72361 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html
+-rw-r--r--   0        0        0    78213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html
+-rw-r--r--   0        0        0    71840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html
+-rw-r--r--   0        0        0    75030 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html
+-rw-r--r--   0        0        0   279449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html
+-rw-r--r--   0        0        0   235836 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html
+-rw-r--r--   0        0        0    72127 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html
+-rw-r--r--   0        0        0    72293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html
+-rw-r--r--   0        0        0    46678 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html
+-rw-r--r--   0        0        0    46642 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html
+-rw-r--r--   0        0        0    46786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html
+-rw-r--r--   0        0        0    46726 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html
+-rw-r--r--   0        0        0    46654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html
+-rw-r--r--   0        0        0    78265 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html
+-rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html
+-rw-r--r--   0        0        0    45429 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html
+-rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html
+-rw-r--r--   0        0        0    45357 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html
+-rw-r--r--   0        0        0    45321 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html
+-rw-r--r--   0        0        0    45465 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html
+-rw-r--r--   0        0        0    45405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html
+-rw-r--r--   0        0        0    45333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html
+-rw-r--r--   0        0        0    74928 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html
+-rw-r--r--   0        0        0    45455 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html
+-rw-r--r--   0        0        0    45575 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html
+-rw-r--r--   0        0        0    45491 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html
+-rw-r--r--   0        0        0    75329 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html
+-rw-r--r--   0        0        0    76868 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html
+-rw-r--r--   0        0        0   169074 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html
+-rw-r--r--   0        0        0    46366 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html
+-rw-r--r--   0        0        0    46330 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html
+-rw-r--r--   0        0        0    46474 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html
+-rw-r--r--   0        0        0    46414 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html
+-rw-r--r--   0        0        0    46342 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html
+-rw-r--r--   0        0        0    77476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html
+-rw-r--r--   0        0        0    87286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html
+-rw-r--r--   0        0        0   129638 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html
+-rw-r--r--   0        0        0    47034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    47058 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    79041 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html
+-rw-r--r--   0        0        0    80446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html
+-rw-r--r--   0        0        0   154233 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html
+-rw-r--r--   0        0        0    45434 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html
+-rw-r--r--   0        0        0    45398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html
+-rw-r--r--   0        0        0    45542 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html
+-rw-r--r--   0        0        0    45482 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html
+-rw-r--r--   0        0        0    45410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html
+-rw-r--r--   0        0        0    75122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html
+-rw-r--r--   0        0        0    83570 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html
+-rw-r--r--   0        0        0   123274 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html
+-rw-r--r--   0        0        0    46102 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    46126 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    76687 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html
+-rw-r--r--   0        0        0    77756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html
+-rw-r--r--   0        0        0    73401 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html
+-rw-r--r--   0        0        0    84383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html
+-rw-r--r--   0        0        0   219068 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html
+-rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html
+-rw-r--r--   0        0        0    46357 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html
+-rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html
+-rw-r--r--   0        0        0    46285 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html
+-rw-r--r--   0        0        0    46249 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html
+-rw-r--r--   0        0        0    46393 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html
+-rw-r--r--   0        0        0    46333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html
+-rw-r--r--   0        0        0    46261 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html
+-rw-r--r--   0        0        0    77269 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html
+-rw-r--r--   0        0        0    78422 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html
+-rw-r--r--   0        0        0   129869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html
+-rw-r--r--   0        0        0    69164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html
+-rw-r--r--   0        0        0    68285 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html
+-rw-r--r--   0        0        0    50899 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html
+-rw-r--r--   0        0        0    74827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html
+-rw-r--r--   0        0        0   164435 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html
+-rw-r--r--   0        0        0    45272 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html
+-rw-r--r--   0        0        0    45236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html
+-rw-r--r--   0        0        0    45380 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html
+-rw-r--r--   0        0        0    45320 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html
+-rw-r--r--   0        0        0    45248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html
+-rw-r--r--   0        0        0    74708 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html
+-rw-r--r--   0        0        0    76620 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html
+-rw-r--r--   0        0        0   102591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html
+-rw-r--r--   0        0        0    68109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html
+-rw-r--r--   0        0        0    77730 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html
+-rw-r--r--   0        0        0    72650 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html
+-rw-r--r--   0        0        0    73154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html
+-rw-r--r--   0        0        0    77495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html
+-rw-r--r--   0        0        0    74934 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html
+-rw-r--r--   0        0        0    83034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html
+-rw-r--r--   0        0        0   112145 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html
+-rw-r--r--   0        0        0    77051 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html
+-rw-r--r--   0        0        0    73182 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html
+-rw-r--r--   0        0        0    84128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html
+-rw-r--r--   0        0        0    83709 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html
+-rw-r--r--   0        0        0    78174 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html
+-rw-r--r--   0        0        0    88686 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html
+-rw-r--r--   0        0        0    74176 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html
+-rw-r--r--   0        0        0    78396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html
+-rw-r--r--   0        0        0     1281 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/pdoc_templates/frame.html.jinja2
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/pdoc_templates/module.html.jinja2
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/__init__.py
+-rw-r--r--   0        0        0     5469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/reusable_responders.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/status_samples.py
+-rw-r--r--   0        0        0     6448 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_assay.py
+-rw-r--r--   0        0        0     8186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_assay_config.py
+-rw-r--r--   0        0        0    26551 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_auth.py
+-rw-r--r--   0        0        0     2985 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_checks.py
+-rw-r--r--   0        0        0    51281 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_client.py
+-rw-r--r--   0        0        0     7933 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_comment.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_connection.py
+-rw-r--r--   0        0        0    31927 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_deployment.py
+-rw-r--r--   0        0        0    11118 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_deployment_config.py
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_engine_config.py
+-rw-r--r--   0        0        0     1238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_explainability.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_import.py
+-rw-r--r--   0        0        0    21694 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_inference_result.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_log_entries.py
+-rw-r--r--   0        0        0    20478 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_model.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_model_config.py
+-rw-r--r--   0        0        0     5140 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_models.py
+-rw-r--r--   0        0        0    24447 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_pipeline.py
+-rw-r--r--   0        0        0    34999 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_pipeline_config.py
+-rw-r--r--   0        0        0    14056 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_pipeline_variant.py
+-rw-r--r--   0        0        0     5439 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_tag.py
+-rw-r--r--   0        0        0    14900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/test_workspace.py
+-rw-r--r--   0        0        0     4053 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/testutil.py
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/.DS_Store
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/ccfraud_output.json
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/day5_output.json
+-rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.arrow
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.pandas.json
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.txt
+-rw-r--r--   0        0        0    17729 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/lazyadam_output.json
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/pipeline_output.json
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_batched_inference_result.json
+-rw-r--r--   0        0        0     2068 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.arrow
+-rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.json
+-rw-r--r--   0        0        0      900 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.pandas.json
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_logged_inference_result.json
+-rw-r--r--   0        0        0    32666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/sample_logs.arrow
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/some_output.json
+-rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/tensor_dropped_log_file.arrow
+-rw-r--r--   0        0        0    32122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/test_logs-1.arrow
+-rw-r--r--   0        0        0    32122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/outputs/logs/x-1.arrow
+-rw-r--r--   0        0        0     1344 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json
+-rw-r--r--   0        0        0      586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_model_drift/drift.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_model_drift/gauges.json
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_values_expression/gauges.json
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_values_expression/values.json
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/default_model_config.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/experiment_model_config.yaml
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_ab_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_batch_config_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0     2122 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mimo_pipeline/python_only_config.yaml
+-rw-r--r--   0        0        0     3543 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mimo_pipeline/python_step_config.yaml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_only_config.yaml
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_step_config.yaml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/post_model_config.yaml
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/pre_model_config.yaml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pipeline/wl_model_config.yaml
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/challenger.yaml
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/control.yaml
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_random_split_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/control.yaml
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model2.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/model3.yaml
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_shadow_deploy_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/model_config.yaml
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_simple_pipeline/pipeline_config.yaml
+-rw-r--r--   0        0        0      933 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/ModelConversion.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/__init__.py
+-rw-r--r--   0        0        0    17522 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/assay.py
+-rw-r--r--   0        0        0    28077 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/assay_config.py
+-rw-r--r--   0        0        0    27488 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/auth.py
+-rw-r--r--   0        0        0     7795 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/checks.py
+-rw-r--r--   0        0        0    85006 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/client.py
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/comment.py
+-rw-r--r--   0        0        0     8867 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/connection.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/datasizeunit.py
+-rw-r--r--   0        0        0    37000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/deployment.py
+-rw-r--r--   0        0        0     8837 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/deployment_config.py
+-rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/engine_config.py
+-rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/explainability.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/expression.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/framework.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/functions.py
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/inference_decode.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/inference_result.py
+-rw-r--r--   0        0        0     5635 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/logs.py
+-rw-r--r--   0        0        0    18773 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/model.py
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/model_config.py
+-rw-r--r--   0        0        0    16666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/model_registry.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/models.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/notify.py
+-rw-r--r--   0        0        0     7572 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/object.py
+-rw-r--r--   0        0        0    15260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/orchestration.py
+-rw-r--r--   0        0        0    45108 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/pipeline.py
+-rw-r--r--   0        0        0    26383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/pipeline_config.py
+-rw-r--r--   0        0        0     8286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/pipeline_variant.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/queries.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/standalone_client.py
+-rw-r--r--   0        0        0    10259 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/tag.py
+-rw-r--r--   0        0        0     9995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/task.py
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/task_run.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/unwrap.py
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/user.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/user_type.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/utils.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/version.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/visibility.py
+-rw-r--r--   0        0        0    10158 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/workspace.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateConnection.graphql
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDeployment.graphql
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateTag.graphql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspace.graphql
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspaceBare.graphql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteConnection.graphql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteWorkspaceUser.graphql
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConfiguredModelById.graphql
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConnection.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConnectionById.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetDeploymentForPipeline.graphql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModel.graphql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelById.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelByTaskId.graphql
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelConfigs.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelVersionById.graphql
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModels.graphql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineAndWorkspace.graphql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineByIdForCopying.graphql
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineByName.graphql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineVersion.graphql
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelinesForModels.graphql
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertConfiguredModel.graphql
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentModelConfig.graphql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModel.graphql
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModelConfig.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModelConfigFull.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertWorkspaceUser.graphql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListConnections.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListDeployments.graphql
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListModelConversions.graphql
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListModels.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListPipelines.graphql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListWorkspaces.graphql
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ModelByName.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/PipelineModels.graphql
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/PipelineVariantById.graphql
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/README.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Undeploy.graphql
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModel.graphql
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UserDefaultWorkspace.graphql
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceById.graphql
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceByName.graphql
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceListConnections.graphql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceNameById.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/AssaySetActive.graphql
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/CreateAssay.graphql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/FilterAssays.graphql
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/GetAssayResults.graphql
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/ListAssays.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetLatestModelConfig.graphql
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModel.graphql
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModelVersions.graphql
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModels.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/GetOrchestration.graphql
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/InsertOrchestration.graphql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/ListOrchestrations.graphql
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/UpdateOrchestration.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelineForPublish.graphql
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelinePublish.graphql
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/InsertPipelinePublish.graphql
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/SetPipelinePublishStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/AttachRegistryToWorkspace.graphql
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/CreateRegistry.graphql
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/GetRegistry.graphql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/ListRegistries.graphql
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/RemoveRegistryFromWorkspace.graphql
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetLogsForRun.graphql
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTaskById.graphql
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTaskRun.graphql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTasksByOrchSha.graphql
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/InsertTask.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/InsertTaskRun.graphql
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTaskRuns.graphql
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasks.graphql
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/README.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/SetTaskKilled.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/StartTaskRun.graphql
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTask.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTaskRun.graphql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/__init__.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/README.md
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/__init__.py
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/convert_keras_model.py
+-rw-r--r--   0        0        0     8639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/graphql_queries.py
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/telemetry_body.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/telemetry_error.py
+-rw-r--r--   0        0        0     3275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/v1_metric_response.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/records/v1_tls_response.py
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/__init__.py
+-rw-r--r--   0        0        0     2827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/client.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/errors.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/types.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/__init__.py
+-rw-r--r--   0        0        0     7661 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/__init__.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py
+-rw-r--r--   0        0        0     5808 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py
+-rw-r--r--   0        0        0     5938 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py
+-rw-r--r--   0        0        0     6086 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py
+-rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py
+-rw-r--r--   0        0        0     6395 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/__init__.py
+-rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py
+-rw-r--r--   0        0        0     6976 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py
+-rw-r--r--   0        0        0     6648 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py
+-rw-r--r--   0        0        0     7110 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py
+-rw-r--r--   0        0        0     6948 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/__init__.py
+-rw-r--r--   0        0        0     7749 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py
+-rw-r--r--   0        0        0     7982 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py
+-rw-r--r--   0        0        0     7211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py
+-rw-r--r--   0        0        0     7078 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py
+-rw-r--r--   0        0        0     6043 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py
+-rw-r--r--   0        0        0     6809 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py
+-rw-r--r--   0        0        0     8431 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py
+-rw-r--r--   0        0        0     7710 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/__init__.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py
+-rw-r--r--   0        0        0     7049 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/__init__.py
+-rw-r--r--   0        0        0     4806 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/attach_registry_to_workspace.py
+-rw-r--r--   0        0        0     4465 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/create_registry.py
+-rw-r--r--   0        0        0     2765 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/get_model_version_by_id.py
+-rw-r--r--   0        0        0     4310 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/get_registry.py
+-rw-r--r--   0        0        0     4514 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registries.py
+-rw-r--r--   0        0        0     5148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registry_model_version_artifacts.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registry_models.py
+-rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py
+-rw-r--r--   0        0        0     5997 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py
+-rw-r--r--   0        0        0     6923 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py
+-rw-r--r--   0        0        0     8104 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py
+-rw-r--r--   0        0        0     4924 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/remove_registry_from_workspace.py
+-rw-r--r--   0        0        0     4179 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload1.py
+-rw-r--r--   0        0        0     4197 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_and_convert.py
+-rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_from_registry.py
+-rw-r--r--   0        0        0     6625 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/__init__.py
+-rw-r--r--   0        0        0     4366 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py
+-rw-r--r--   0        0        0     4537 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py
+-rw-r--r--   0        0        0     4166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/__init__.py
+-rw-r--r--   0        0        0     6744 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py
+-rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py
+-rw-r--r--   0        0        0     6428 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py
+-rw-r--r--   0        0        0     6497 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py
+-rw-r--r--   0        0        0     7048 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/__init__.py
+-rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/get_publish_status.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/list_published_pipelines.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/publish_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/__init__.py
+-rw-r--r--   0        0        0     7165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py
+-rw-r--r--   0        0        0     6599 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/__init__.py
+-rw-r--r--   0        0        0     4090 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_logs_for_run.py
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_run_details.py
+-rw-r--r--   0        0        0     4333 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_tasks_by_orch_sha.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py
+-rw-r--r--   0        0        0     4543 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list_task_runs.py
+-rw-r--r--   0        0        0     4071 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/__init__.py
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py
+-rw-r--r--   0        0        0     6257 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py
+-rw-r--r--   0        0        0     6025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py
+-rw-r--r--   0        0        0     6349 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py
+-rw-r--r--   0        0        0     6305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py
+-rw-r--r--   0        0        0     6729 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py
+-rw-r--r--   0        0        0     6757 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py
+-rw-r--r--   0        0        0    61955 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/arbex_status.py
+-rw-r--r--   0        0        0    10956 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py
+-rw-r--r--   0        0        0     2019 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     1924 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4605 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py
+-rw-r--r--   0        0        0     1503 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py
+-rw-r--r--   0        0        0     3681 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.py
+-rw-r--r--   0        0        0    11372 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py
+-rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py
+-rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2922 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py
+-rw-r--r--   0        0        0     1958 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py
+-rw-r--r--   0        0        0     9367 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.py
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py
+-rw-r--r--   0        0        0     4113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py
+-rw-r--r--   0        0        0    12777 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py
+-rw-r--r--   0        0        0     2084 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1955 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py
+-rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py
+-rw-r--r--   0        0        0    11996 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2020 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      214 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py
+-rw-r--r--   0        0        0     1682 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py
+-rw-r--r--   0        0        0    11489 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py
+-rw-r--r--   0        0        0     2049 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py
+-rw-r--r--   0        0        0     4813 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py
+-rw-r--r--   0        0        0     9311 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py
+-rw-r--r--   0        0        0     5001 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.py
+-rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.py
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.py
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_request.py
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response_200.py
+-rw-r--r--   0        0        0     1905 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py
+-rw-r--r--   0        0        0     2775 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_409.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py
+-rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py
+-rw-r--r--   0        0        0     1383 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py
+-rw-r--r--   0        0        0     1941 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/conversion.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_request.py
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response.py
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response_200.py
+-rw-r--r--   0        0        0     4163 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py
+-rw-r--r--   0        0        0     1224 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py
+-rw-r--r--   0        0        0     2034 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/dbfs_list_response_file.py
+-rw-r--r--   0        0        0     2397 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/dbfs_list_response_file_with_full_path.py
+-rw-r--r--   0        0        0     3676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py
+-rw-r--r--   0        0        0     1242 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py
+-rw-r--r--   0        0        0     5860 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py
+-rw-r--r--   0        0        0     6373 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py
+-rw-r--r--   0        0        0     2411 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py
+-rw-r--r--   0        0        0     1327 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py
+-rw-r--r--   0        0        0     1312 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py
+-rw-r--r--   0        0        0     1345 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/file_info.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/framework.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_request.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response.py
+-rw-r--r--   0        0        0     1454 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response_200.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_model_by_id_request.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py
+-rw-r--r--   0        0        0     3846 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_request.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response.py
+-rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_200.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_workspace.py
+-rw-r--r--   0        0        0     1550 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_request.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_response_200.py
+-rw-r--r--   0        0        0     1696 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_request.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response.py
+-rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response_200.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_models.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_registries_request.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_registry_model_version_artifacts_request.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_registry_models_request.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_request.py
+-rw-r--r--   0        0        0     2576 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request_status.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_response_task_runs.py
+-rw-r--r--   0        0        0     2326 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py
+-rw-r--r--   0        0        0     1297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_id.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_registry.py
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_status.py
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_version.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py
+-rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py
+-rw-r--r--   0        0        0     2146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py
+-rw-r--r--   0        0        0     2621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py
+-rw-r--r--   0        0        0     2047 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py
+-rw-r--r--   0        0        0     3499 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py
+-rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py
+-rw-r--r--   0        0        0     2539 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.py
+-rw-r--r--   0        0        0     4563 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec.py
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec_exec_type.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py
+-rw-r--r--   0        0        0     4653 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration_status.py
+-rw-r--r--   0        0        0     4042 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py
+-rw-r--r--   0        0        0     1387 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py
+-rw-r--r--   0        0        0     2337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py
+-rw-r--r--   0        0        0     1440 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py
+-rw-r--r--   0        0        0     3449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body_order.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_502.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py
+-rw-r--r--   0        0        0     1340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py
+-rw-r--r--   0        0        0     2012 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py
+-rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/publish_request.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/python_version.py
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/registered_model.py
+-rw-r--r--   0        0        0     3666 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/registered_model_version.py
+-rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_request.py
+-rw-r--r--   0        0        0     1754 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response.py
+-rw-r--r--   0        0        0     1772 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response_200.py
+-rw-r--r--   0        0        0     2660 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/search_registered_models_response.py
+-rw-r--r--   0        0        0     1483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py
+-rw-r--r--   0        0        0     4878 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.py
+-rw-r--r--   0        0        0     4879 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py
+-rw-r--r--   0        0        0     4827 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py
+-rw-r--r--   0        0        0     4761 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.py
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py
+-rw-r--r--   0        0        0     4871 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.py
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_request.py
+-rw-r--r--   0        0        0     3974 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_run.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_status.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_request.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response_200.py
+-rw-r--r--   0        0        0     2389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc_1.py
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request_1.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response_1.py
+-rw-r--r--   0        0        0     1463 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py
+-rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py
+-rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py
+-rw-r--r--   0        0        0     1363 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py
+-rw-r--r--   0        0        0     3557 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py
+-rw-r--r--   0        0        0     1469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py
+-rw-r--r--   0        0        0     3605 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py
+-rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py
+-rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py
+-rw-r--r--   0        0        0     1580 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py
+-rw-r--r--   0        0        0     2215 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateConnection.graphql
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDeployment.graphql
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateTag.graphql
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspace.graphql
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspaceBare.graphql
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/CreateWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteConnection.graphql
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteWorkspaceConnection.graphql
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/DeleteWorkspaceUser.graphql
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConfiguredModelById.graphql
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConfiguredModelByTaskId.graphql
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConnection.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetConnectionById.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetDeploymentForPipeline.graphql
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModel.graphql
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelById.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelByTaskId.graphql
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelConfigs.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModelVersionById.graphql
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetModels.graphql
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineAndWorkspace.graphql
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineByIdForCopying.graphql
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineByName.graphql
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineVersion.graphql
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineVersionDeploymentDetails.graphql
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelinesForModels.graphql
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertConfiguredModel.graphql
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentModelConfig.graphql
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentModelConfigMultiple.graphql
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModel.graphql
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModelConfig.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModelConfigFull.graphql
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/InsertWorkspaceUser.graphql
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListConnections.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListDeployments.graphql
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListModelConversions.graphql
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListModels.graphql
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListPipelines.graphql
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ListWorkspaces.graphql
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/ModelByName.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/PipelineModels.graphql
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/PipelineVariantById.graphql
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/README.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Undeploy.graphql
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModel.graphql
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/UserDefaultWorkspace.graphql
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceById.graphql
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceByName.graphql
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceListConnections.graphql
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/WorkspaceNameById.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/AssaySetActive.graphql
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/CreateAssay.graphql
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/FilterAssays.graphql
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/GetAssayResults.graphql
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/ListAssays.graphql
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/ListAssaysWithPipeline.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/__init__.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/DeleteUsersFromWorkspace.graphql
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/GetUserWorkspacePermission.graphql
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/ListWorkspaceUsers.graphql
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/ListWorkspacesByUser.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/Workspaces/__init__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetDeploymentPipelineVersion.graphql
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityConfig.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityConfigByReferencePipelineVersion.graphql
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetExplainabilityRequest.graphql
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetPipelineByPipelineVersion.graphql
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/GetPipelineVersionVersion.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityConfigs.graphql
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityConfigsByPipeline.graphql
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/ListExplainabilityRequests.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/__init__.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetLatestModelConfig.graphql
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModel.graphql
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModelVersions.graphql
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/GetModels.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/models/__init__.py
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/GetOrchestration.graphql
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/GetOrchestrationByTaskId.graphql
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/InsertOrchestration.graphql
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/ListOrchestrations.graphql
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/UpdateOrchestration.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/orch/__init__.py
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelineDefinitionByNameAndVersion.graphql
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelineForPublish.graphql
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/GetPipelinePublish.graphql
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/InsertPipelinePublish.graphql
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/PipelineModelsFlat.graphql
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/SetPipelinePublishStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/__init__.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/AttachRegistryToWorkspace.graphql
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/CreateRegistry.graphql
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/GetRegistry.graphql
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/ListRegistries.graphql
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/registries/RemoveRegistryFromWorkspace.graphql
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetLogsForRun.graphql
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTaskById.graphql
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTaskRun.graphql
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/GetTasksByOrchSha.graphql
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/InsertTask.graphql
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/InsertTaskRun.graphql
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTaskRuns.graphql
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasks.graphql
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/README.md
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/SetTaskKilled.graphql
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/StartTaskRun.graphql
+-rw-r--r--   0        0        0      579 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTask.graphql
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTaskRun.graphql
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTaskStatus.graphql
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/__init__.py
+-rw-r--r--   0        0        0      857 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/cli.py
+-rw-r--r--   0        0        0     4093 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/exceptions.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/types.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/inference/__init__.py
+-rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/inference/custom_inference_config.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/inference/inference_config.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/service/__init__.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/service/inference_service_config.py
+-rw-r--r--   0        0        0     2018 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/config/service/mlflow_service_config.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/entrypoints/__init__.py
+-rw-r--r--   0        0        0     5662 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/entrypoints/serving.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/__init__.py
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/inference.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/streamlined_dl_inference.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/streamlined_inference.py
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/streamlined_ml_inference.py
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/creation/__init__.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/inference/creation/inference_builder.py
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_processing/__init__.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_processing/base_preprocessor.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_processing/postprocessor.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_processing/preprocessor.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_validation/__init__.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_validation/ascending_keys_validator.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_validation/data_validator.py
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/data_validation/keys_validator.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/file_loading/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/file_loading/file_loader.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/file_loading/json_loader.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/io/file_loading/pickle_loader.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/__init__.py
+-rw-r--r--   0        0        0     1856 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/inference_service.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/wsgi_server_options.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/creation/__init__.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/creation/inference_service_factory.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/mlflow/__init__.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/mlflow/mlflow_adapter.py
+-rw-r--r--   0        0        0     6161 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/service/mlflow/mlflow_service.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/utils/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/utils/abstract_factory.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/utils/gunicorn_app.py
+-rw-r--r--   0        0        0     8694 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/mac/utils/helpers.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/.gitignore
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/public_README.md
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/pyproject.toml
+-rw-r--r--   0        0        0     3106 2020-02-02 00:00:00.000000 wallaroo-2023.2.1rc2/PKG-INFO
```

### Comparing `wallaroo-2023.2.1rc1/.DS_Store` & `wallaroo-2023.2.1rc2/.DS_Store`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/.coverage` & `wallaroo-2023.2.1rc2/.coverage`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/Dockerfile` & `wallaroo-2023.2.1rc2/Dockerfile`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/Makefile` & `wallaroo-2023.2.1rc2/Makefile`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 	python3 -m pip install hatch==1.7.0
 
 # This is a convenience for unit tests that will symlink into the SDK and need its dependencies.
 install-sdk-requirements: ensure_hatch
 	python3 -m hatch -e default dep show requirements | xargs python3 -m pip install
 
 build-sdk: clean generate-openapi ensure_hatch
-	SETUPTOOLS_SCM_PRETEND_VERSION="2023.2.1rc1" python3 -m hatch build
+	SETUPTOOLS_SCM_PRETEND_VERSION="${SDK_VERSION}rc2" python3 -m hatch build
 
 image: build-sdk
 	$(DOCKER) build \
 	-t $(SDK_IMAGE):$(TAG) -t $(SDK_IMAGE):latest \
 	--cache-to=type=registry,ref=$(SDK_IMAGE):cache,mode=max \
 	--cache-from=type=registry,ref=$(SDK_IMAGE):cache \
 	--label "org.opencontainers.image.revision=$(REVISION)" \
```

### Comparing `wallaroo-2023.2.1rc1/README.md` & `wallaroo-2023.2.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/mypy.ini` & `wallaroo-2023.2.1rc2/mypy.ini`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/requirements.txt` & `wallaroo-2023.2.1rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/Makefile` & `wallaroo-2023.2.1rc2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/make.bat` & `wallaroo-2023.2.1rc2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/autoscaling.ipynb` & `wallaroo-2023.2.1rc2/docs/source/autoscaling.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/conf.py` & `wallaroo-2023.2.1rc2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/core-abstractions.ipynb` & `wallaroo-2023.2.1rc2/docs/source/core-abstractions.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/email.png` & `wallaroo-2023.2.1rc2/docs/source/email.png`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/experiments.ipynb` & `wallaroo-2023.2.1rc2/docs/source/experiments.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/index.rst` & `wallaroo-2023.2.1rc2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/jupyter.md` & `wallaroo-2023.2.1rc2/docs/source/jupyter.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model-insights.ipynb` & `wallaroo-2023.2.1rc2/docs/source/model-insights.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion.rst` & `wallaroo-2023.2.1rc2/docs/source/model_conversion.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_keras.ipynb` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_keras.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_sklearn.ipynb` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_sklearn.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_xgboost.ipynb` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_xgboost.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/models.ipynb` & `wallaroo-2023.2.1rc2/docs/source/models.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/monitoring.ipynb` & `wallaroo-2023.2.1rc2/docs/source/monitoring.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/python-processing.ipynb` & `wallaroo-2023.2.1rc2/docs/source/python-processing.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/sdk.rst` & `wallaroo-2023.2.1rc2/docs/source/sdk.rst`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/standalone-mode.ipynb` & `wallaroo-2023.2.1rc2/docs/source/standalone-mode.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/workspaces.ipynb` & `wallaroo-2023.2.1rc2/docs/source/workspaces.ipynb`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/BikeShareRegressor.py` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/BikeShareRegressor.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/isolet_xgboost_model.pickle` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/isolet_xgboost_model.pickle`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/pytorch_bikesharingmodel.pt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/docs/source/model_conversion_resources/sentiment_model.zip` & `wallaroo-2023.2.1rc2/docs/source/model_conversion_resources/sentiment_model.zip`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/ModelConversion.html` & `wallaroo-2023.2.1rc2/html/wallaroo/ModelConversion.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/assay.html` & `wallaroo-2023.2.1rc2/html/wallaroo/assay.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/assay_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/assay_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/auth.html` & `wallaroo-2023.2.1rc2/html/wallaroo/auth.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/checks.html` & `wallaroo-2023.2.1rc2/html/wallaroo/checks.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/client.html` & `wallaroo-2023.2.1rc2/html/wallaroo/client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/comment.html` & `wallaroo-2023.2.1rc2/html/wallaroo/comment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/connection.html` & `wallaroo-2023.2.1rc2/html/wallaroo/connection.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/datasizeunit.html` & `wallaroo-2023.2.1rc2/html/wallaroo/datasizeunit.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/deployment.html` & `wallaroo-2023.2.1rc2/html/wallaroo/deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/deployment_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/deployment_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/engine_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/explainability.html` & `wallaroo-2023.2.1rc2/html/wallaroo/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/expression.html` & `wallaroo-2023.2.1rc2/html/wallaroo/expression.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/framework.html` & `wallaroo-2023.2.1rc2/html/wallaroo/framework.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/functions.html` & `wallaroo-2023.2.1rc2/html/wallaroo/functions.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/inference_decode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/inference_decode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/inference_result.html` & `wallaroo-2023.2.1rc2/html/wallaroo/inference_result.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/logs.html` & `wallaroo-2023.2.1rc2/html/wallaroo/logs.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/model.html` & `wallaroo-2023.2.1rc2/html/wallaroo/model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/model_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/models.html` & `wallaroo-2023.2.1rc2/html/wallaroo/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/notify.html` & `wallaroo-2023.2.1rc2/html/wallaroo/notify.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/object.html` & `wallaroo-2023.2.1rc2/html/wallaroo/object.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/orchestration.html` & `wallaroo-2023.2.1rc2/html/wallaroo/orchestration.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/pipeline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/pipeline_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/pipeline_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/pipeline_variant.html` & `wallaroo-2023.2.1rc2/html/wallaroo/pipeline_variant.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/queries.html` & `wallaroo-2023.2.1rc2/html/wallaroo/queries.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/standalone_client.html` & `wallaroo-2023.2.1rc2/html/wallaroo/standalone_client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/tag.html` & `wallaroo-2023.2.1rc2/html/wallaroo/tag.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/task.html` & `wallaroo-2023.2.1rc2/html/wallaroo/task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/unwrap.html` & `wallaroo-2023.2.1rc2/html/wallaroo/unwrap.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/user.html` & `wallaroo-2023.2.1rc2/html/wallaroo/user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/user_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/user_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/utils.html` & `wallaroo-2023.2.1rc2/html/wallaroo/utils.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/version.html` & `wallaroo-2023.2.1rc2/html/wallaroo/version.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/visibility.html` & `wallaroo-2023.2.1rc2/html/wallaroo/visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/workspace.html` & `wallaroo-2023.2.1rc2/html/wallaroo/workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/Assays.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/Assays.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/Workspaces.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/Workspaces.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/explainability.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/models.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/orch.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/orch.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/pipelines.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/pipelines.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/graphql/tasks.html` & `wallaroo-2023.2.1rc2/html/wallaroo/graphql/tasks.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/convert_keras_model.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/convert_keras_model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/graphql_queries.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/graphql_queries.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/telemetry_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/telemetry_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/telemetry_error.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/telemetry_error.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/v1_metric_response.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/v1_metric_response.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/records/v1_tls_response.html` & `wallaroo-2023.2.1rc2/html/wallaroo/records/v1_tls_response.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/client.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/client.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/types.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/types.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_results.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_id.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_status_and_workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_get_by_workspace.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/task/v1_task_update.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_sort_by.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_results_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_bin_mode.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_metric.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1_type.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary_aggregation.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_multipart_data_visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_200_insert_models_returning_item_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_visibility.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_health.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_error_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_output_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_attempt_output_item_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_200_task_task_type_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_id_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_json_body_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_and_workspace_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_json_body_task_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_status_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_flavor_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_200_tasks_item_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_get_by_workspace_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_additional_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_error_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_json_body_status.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_0.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_1.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_2.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_3.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_4.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_5.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_6.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_200_data_status_type_7.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/v1_task_update_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html` & `wallaroo-2023.2.1rc2/html/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.html`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/pdoc_templates/frame.html.jinja2` & `wallaroo-2023.2.1rc2/pdoc_templates/frame.html.jinja2`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/reusable_responders.py` & `wallaroo-2023.2.1rc2/unit_tests/reusable_responders.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/status_samples.py` & `wallaroo-2023.2.1rc2/unit_tests/status_samples.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_assay.py` & `wallaroo-2023.2.1rc2/unit_tests/test_assay.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_assay_config.py` & `wallaroo-2023.2.1rc2/unit_tests/test_assay_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_auth.py` & `wallaroo-2023.2.1rc2/unit_tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_checks.py` & `wallaroo-2023.2.1rc2/unit_tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_client.py` & `wallaroo-2023.2.1rc2/unit_tests/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -661,56 +661,99 @@
             f"{self.test_client.api_endpoint}/v1/api/models/upload_and_convert",
             status=200,
             json={"insert_models": {"returning": [{"models": [{"id": 1}]}]}},
         )
         self.add_get_configured_model()
         self.add_default_workspace_responder()
 
+        responses.add(
+            responses.POST,
+            f"{self.test_client.api_endpoint}/v1/graphql",
+            status=200,
+            match=[testutil.query_name_matcher("ModelById")],
+            json={
+                "data": {
+                    "model_by_pk": {
+                        "id": 1,
+                        "sha": "adsfadsf",
+                        "model_id": "some_model_name",
+                        "model_version": "some_model_variant_name",
+                        "status": "ready",
+                        "file_name": "some_model_file.onnx",
+                        "updated_at": self.now.isoformat(),
+                        "visibility": "private",
+                    },
+                },
+            },
+        )
+
         with tempfile.NamedTemporaryFile() as f:
             f.write(b"model_data")
 
             variant = self.test_client.upload_model(
                 name="foo",
                 path=f.name,
                 framework=Framework.KERAS,
                 convert_wait=True,
                 input_schema=pa.schema([]),
                 output_schema=pa.schema([]),
             )
 
         self.assertEqual(1, variant.id())
         self.assertEqual("ready", variant.status())
-        self.assertEqual(3, len(responses.calls))
+        self.assertEqual(5, len(responses.calls))
 
     @responses.activate
     @mock.patch.dict(os.environ, {"MODELS_ENABLED": "true"})
     def test_upload_model_and_wait_for_convert_timedout(self):
         responses.add(
             responses.POST,
             f"{self.test_client.api_endpoint}/v1/api/models/upload_and_convert",
             status=200,
             json={"insert_models": {"returning": [{"models": [{"id": 1}]}]}},
         )
         self.add_get_configured_model("pendingconversion")
         self.add_default_workspace_responder()
         wallaroo.client.DEFAULT_MODEL_CONVERSION_TIMEOUT = 0.1
+
+        responses.add(
+            responses.POST,
+            f"{self.test_client.api_endpoint}/v1/graphql",
+            status=200,
+            match=[testutil.query_name_matcher("ModelById")],
+            json={
+                "data": {
+                    "model_by_pk": {
+                        "id": 1,
+                        "sha": "adsfadsf",
+                        "model_id": "some_model_name",
+                        "model_version": "some_model_variant_name",
+                        "status": "pendingconversion",
+                        "file_name": "some_model_file.onnx",
+                        "updated_at": self.now.isoformat(),
+                        "visibility": "private",
+                    },
+                },
+            },
+        )
+
         with tempfile.NamedTemporaryFile() as f:
             f.write(b"model_data")
 
             with self.assertRaises(ModelConversionTimeoutError):
                 self.test_client.upload_model(
                     name="foo",
                     path=f.name,
                     framework=Framework.KERAS,
                     convert_wait=True,
                     input_schema=pa.schema([]),
                     output_schema=pa.schema([]),
                 )
 
-        self.assertEqual(3, len(responses.calls))
+        self.assertEqual(4, len(responses.calls))
 
     @responses.activate
     @mock.patch.dict(os.environ, {"MODELS_ENABLED": "true"})
     def test_upload_model_and_convert(self):
         responses.add(
             responses.POST,
             f"{self.test_client.api_endpoint}/v1/api/models/upload_and_convert",
```

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_comment.py` & `wallaroo-2023.2.1rc2/unit_tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_connection.py` & `wallaroo-2023.2.1rc2/unit_tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_deployment.py` & `wallaroo-2023.2.1rc2/unit_tests/test_deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_deployment_config.py` & `wallaroo-2023.2.1rc2/unit_tests/test_deployment_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_engine_config.py` & `wallaroo-2023.2.1rc2/unit_tests/test_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_explainability.py` & `wallaroo-2023.2.1rc2/unit_tests/test_explainability.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_inference_result.py` & `wallaroo-2023.2.1rc2/unit_tests/test_inference_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_log_entries.py` & `wallaroo-2023.2.1rc2/unit_tests/test_log_entries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_model.py` & `wallaroo-2023.2.1rc2/unit_tests/test_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,14 @@
                 "updated_at": self.now.isoformat(),
                 "visibility": "private",
             },
         )
 
     @responses.activate
     def test_init_full_dict(self):
-
         variant = Model(
             client=self.test_client,
             data={
                 "id": 1,
                 "model_id": "some_model_name",
                 "model_version": "some_model_variant_name",
                 "file_name": "some_model_file.onnx",
@@ -320,15 +319,18 @@
                         },
                     },
                 )
 
                 variant = Model(client=self.test_client, data={"id": 1})
 
                 self.assertEqual(want_value, getattr(variant, method_name)())
-                self.assertEqual(1, len(responses.calls))
+                if method_name == "status":
+                    self.assertEqual(2, len(responses.calls))
+                else:
+                    self.assertEqual(1, len(responses.calls))
                 responses.reset()
 
     @responses.activate
     def test_configure(self):
         responses.add(
             responses.POST,
             "http://api-lb/v1/graphql",
@@ -533,15 +535,14 @@
             },
         )
 
         self.assertEqual(len(variant.logs(20)), 1)
 
     @responses.activate
     def test_pipeline_tags(self):
-
         tag_1 = Tag(client=self.test_client, data={"id": 1, "tag": "bartag314"})
         tag_2 = Tag(client=self.test_client, data={"id": 2, "tag": "footag123"})
 
         responses.add(
             responses.POST,
             "http://api-lb/v1/graphql",
             status=200,
@@ -562,8 +563,10 @@
                         ],
                     },
                 },
             },
         )
 
         variant = Model(client=self.test_client, data={"id": 1})
-        self.assertListEqual(list(map(vars, [tag_1, tag_2])), list(map(vars, variant.tags())))
+        self.assertListEqual(
+            list(map(vars, [tag_1, tag_2])), list(map(vars, variant.tags()))
+        )
```

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_model_config.py` & `wallaroo-2023.2.1rc2/unit_tests/test_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_models.py` & `wallaroo-2023.2.1rc2/unit_tests/test_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_pipeline.py` & `wallaroo-2023.2.1rc2/unit_tests/test_pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,20 +32,29 @@
 
 sink = pa.BufferOutputStream()
 with pa.ipc.open_file("unit_tests/outputs/sample_logs.arrow") as reader:
     arrow_logs = reader.read_all()
     with pa.ipc.new_file(sink, arrow_logs.schema) as arrow_ipc:
         arrow_ipc.write(arrow_logs)
         arrow_ipc.close()
+
+dropped_log_sink = pa.BufferOutputStream()
+with pa.ipc.open_file("unit_tests/outputs/tensor_dropped_log_file.arrow") as tdl_reader:
+    tensor_dropped_logs = tdl_reader.read_all()
+    with pa.ipc.new_file(dropped_log_sink, tensor_dropped_logs.schema) as tdl_ipc:
+        tdl_ipc.write(tensor_dropped_logs)
+        tdl_ipc.close()
+
 SAMPLE_ARROW_LOGS_RESPONSE = sink.getvalue()
 SAMPLE_PANDAS_RECORDS_INFERENCE_RESPONSE = json.load(
     open('unit_tests/outputs/sample_inference_result.pandas.json', 'rb'))
 with open("unit_tests/outputs/dev_smoke_test.pandas.json", "r") as fp:
     SAMPLE_PANDAS_RECORDS_JSON = pd.read_json(fp)
 
+
 def logged_inference():
     with open("unit_tests/outputs/sample_logged_inference_result.json", "r") as fp:
         return json.loads(fp.read())
 
 
 class TestPipeline(unittest.TestCase):
     def setUp(self):
@@ -217,14 +226,27 @@
             match=[responses.matchers.query_param_matcher(
                 params
             )
             ],
         )
 
     @staticmethod
+    def add_get_tensor_dropped_records_responder(params):
+        responses.add(
+            responses.POST,
+            f"http://api-lb:8080/v1/logs/topic/workspace-1-pipeline-x-inference/records",
+            status=200,
+            body=dropped_log_sink.getvalue(),
+            match=[responses.matchers.query_param_matcher(
+                params
+            )
+            ],
+        )
+
+    @staticmethod
     def add_user_workspace_responder():
         responses.add(
             responses.POST,
             "http://api-lb:8080/v1/graphql",
             status=200,
             match=[testutil.query_name_matcher("UserDefaultWorkspace")],
             json={
@@ -362,34 +384,48 @@
 
     @responses.activate
     def test_logs_with_arrow(self):
         params = {
                     "page_size": 100,
                     "order": "desc",
                     "dataset[]": "*",
-                    "dataset.exclude[]": "metadata",
                     "dataset.separator": ".",
                 }
         self.add_get_topic_name_responder()
         self.add_user_workspace_responder()
         self.add_get_records_responder(params)
         log_table = self.pipeline.logs(limit=100, arrow=True)
         
         self.assertIsInstance(log_table, pa.Table)
         log_table.equals(arrow_logs)
 
     @responses.activate
+    def test_tensor_dropped_logs_with_arrow(self):
+        params = {
+            "page_size": 100,
+            "order": "desc",
+            "dataset[]": "*",
+            "dataset.separator": ".",
+        }
+        self.add_get_topic_name_responder()
+        self.add_user_workspace_responder()
+        self.add_get_tensor_dropped_records_responder(params)
+        log_table_df = self.pipeline.logs(limit=100)
+        self.assertIsInstance(log_table_df, pd.DataFrame)
+        self.assertIsNone(log_table_df["in.tensor"][0]) # tensor dropped
+
+    @responses.activate
     def test_export_logs_to_arrow_file(self):
         start_datetime = datetime.datetime.utcnow()
         end_datetime = datetime.datetime.utcnow()
         params = {
             "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "dataset[]": "*",
-            "dataset.exclude[]": "metadata",
+            "dataset[]": "*",
             "dataset.separator": ".",
         }
         self.add_get_topic_name_responder()
         self.add_get_records_responder(params)
 
         self.pipeline.export_logs(directory="unit_tests/outputs", file_prefix="test_logs", start_datetime=start_datetime,
                                   end_datetime=end_datetime, arrow=True)
@@ -401,15 +437,14 @@
     def test_export_logs_without_user_provided_filepath(self):
         start_datetime = datetime.datetime.utcnow()
         end_datetime = datetime.datetime.utcnow()
         params = {
             "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "dataset[]": "*",
-            "dataset.exclude[]": "metadata",
             "dataset.separator": ".",
         }
         self.add_get_topic_name_responder()
         self.add_get_records_responder(params)
         cwd = os.getcwd()
         # we don't want to be writing test related files outside this directory
         os.chdir("unit_tests/outputs")
@@ -423,15 +458,14 @@
     def test_get_pipeline_logs_by_time(self):
         start_datetime = datetime.datetime.utcnow()
         end_datetime = datetime.datetime.utcnow()
         params = {
             "time.start": start_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "time.end": end_datetime.astimezone(tz=datetime.timezone.utc).isoformat(),
             "dataset[]": "*",
-            "dataset.exclude[]": "metadata",
             "dataset.separator": ".",
         }
         self.add_get_topic_name_responder()
         self.add_user_workspace_responder()
         self.add_get_records_responder(params)
 
         log_table = self.pipeline.logs(start_datetime=start_datetime, end_datetime=end_datetime, arrow=True)
```

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_pipeline_config.py` & `wallaroo-2023.2.1rc2/unit_tests/test_pipeline_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_pipeline_variant.py` & `wallaroo-2023.2.1rc2/unit_tests/test_pipeline_variant.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_tag.py` & `wallaroo-2023.2.1rc2/unit_tests/test_tag.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/test_workspace.py` & `wallaroo-2023.2.1rc2/unit_tests/test_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/testutil.py` & `wallaroo-2023.2.1rc2/unit_tests/testutil.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/.DS_Store` & `wallaroo-2023.2.1rc2/unit_tests/outputs/.DS_Store`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/ccfraud_output.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/ccfraud_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/day5_output.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/day5_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.arrow` & `wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.pandas.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.pandas.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/dev_smoke_test.txt` & `wallaroo-2023.2.1rc2/unit_tests/outputs/dev_smoke_test.txt`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/lazyadam_output.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/lazyadam_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/pipeline_output.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/pipeline_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_batched_inference_result.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_batched_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.arrow` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_inference_result.pandas.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_inference_result.pandas.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_logged_inference_result.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_logged_inference_result.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/sample_logs.arrow` & `wallaroo-2023.2.1rc2/unit_tests/outputs/sample_logs.arrow`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/outputs/some_output.json` & `wallaroo-2023.2.1rc2/unit_tests/outputs/some_output.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_aggregate_function/aggregate.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_bounds_expression/bounds.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_bounds_expression/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_model_drift/drift.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_model_drift/drift.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_model_drift/gauges.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_model_drift/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_values_expression/gauges.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_values_expression/gauges.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_checks/test_values_expression/values.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_checks/test_values_expression/values.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_demandgen_mlflow_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/model_config.yaml` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_multidim_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_mlflow_variable_pipeline/model_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_step_config.yaml` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_py_pandas_pipeline/python_step_config.yaml`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_single_alert/alert.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_single_validation/single_validation.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_validate/single_validation.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json` & `wallaroo-2023.2.1rc2/unit_tests/snapshots/test_pipeline_config/test_validation_placement/checked_pipeline.json`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/ModelConversion.py` & `wallaroo-2023.2.1rc2/wallaroo/ModelConversion.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/assay.py` & `wallaroo-2023.2.1rc2/wallaroo/assay.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/assay_config.py` & `wallaroo-2023.2.1rc2/wallaroo/assay_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/auth.py` & `wallaroo-2023.2.1rc2/wallaroo/auth.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/checks.py` & `wallaroo-2023.2.1rc2/wallaroo/checks.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/client.py` & `wallaroo-2023.2.1rc2/wallaroo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import re
 import sys
 import time
 from datetime import datetime, timedelta, timezone
 from functools import partial
 from itertools import chain, repeat
 from typing import Any, Dict, List, NewType, Optional, TextIO, Tuple, Union, cast
-from urllib.parse import quote_plus
+from urllib.parse import quote_plus, urlparse
 
 import gql  # type: ignore
 import pandas as pd
 import pyarrow as pa  # type: ignore
 import requests
 from gql.transport.requests import RequestsHTTPTransport
 from wallaroo.model_registry import ModelRegistriesList, ModelRegistry
@@ -1295,24 +1295,17 @@
                 params["time.start"] = start_str  # type: ignore
                 end_str = end_datetime.astimezone(tz=timezone.utc).isoformat()
                 params["time.end"] = end_str  # type: ignore
             else:
                 raise Exception(
                     "Please provide both start datetime and end datetime together."
                 )
-            default_dataset_exclude = ["metadata"]
-            if dataset is not None:
-                if "metadata" in dataset:
-                    default_dataset_exclude = []
             params["dataset[]"] = dataset or ["*"]  # type: ignore
-            params["dataset.exclude[]"] = (
-                [*dataset_exclude, *default_dataset_exclude]  # type: ignore
-                if dataset_exclude
-                else default_dataset_exclude
-            )
+            if dataset_exclude is not None:
+                params["dataset.exclude[]"] = dataset_exclude  # type: ignore
             params["dataset.separator"] = dataset_separator or "."  # type: ignore
         else:
             params["limit"] = limit if limit is not None else DEFAULT_RECORDS_LIMIT  # type: ignore
             headers.update({"Accept": JSON_CONTENT_TYPE})
         return headers, params
 
     def _get_next_records(
@@ -1455,29 +1448,40 @@
         data_size_limit_in_bytes = data_unit.calculate_bytes(data_size)
 
         rows_written = 0
         writer = None
         file_num = 0
         schema = None
         schema_changed = False
+        columns_dropped = False
         end_time = None
         previous_end_time = None
         data_size_exceeded = False
         total_data_size = 0
-
+        dropped_columns = []
         while iterator is not None:
             response = self._get_next_records(params, iterator, headers, base)
             logs_table, iterator, status = self._extract_logs_from_response(response)
             if logs_table.num_rows == 0:
                 break
             if schema is not None and schema != logs_table.schema:
                 schema_changed = True
                 writer.close()
                 writer = None
-
+            if "metadata.dropped" in logs_table.column_names:
+                flattened_metadata = logs_table["metadata.dropped"].flatten()
+                if len(flattened_metadata[0][0]) > 0:
+                    columns_dropped = True
+                    dropped_columns = flattened_metadata[0][0]
+            if "metadata" not in params["dataset[]"]:
+                metadata_columns_to_drop = []
+                for column_name in logs_table.column_names:
+                    if column_name.startswith("metadata."):
+                        metadata_columns_to_drop.append(column_name)
+                logs_table = logs_table.drop(metadata_columns_to_drop)
             if writer is None:
                 schema = logs_table.schema
                 file_num += 1
                 writer = create_new_file(
                     directory, file_num, file_prefix, schema, arrow
                 )
 
@@ -1511,14 +1515,22 @@
                 writer.close()
                 break
         if schema_changed:
             sys.stderr.write(
                 f"Note: The logs with different schemas are "
                 f"written to separate files in the provided directory."
             )
+        if columns_dropped:
+            sys.stderr.write(
+                f"Warning: The inference log is above the allowable limit and the following columns may have"
+                f" been suppressed for various rows in the logs: {dropped_columns}."
+                f" To review the dropped columns for an individual inference’s suppressed data,"
+                f' include dataset=["metadata"] in the log request.'
+                f"\n"
+            )
         return None
 
     def get_logs(
         self,
         topic: str,
         limit: Optional[int] = None,
         start_datetime: Optional[datetime] = None,
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/comment.py` & `wallaroo-2023.2.1rc2/wallaroo/comment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/connection.py` & `wallaroo-2023.2.1rc2/wallaroo/connection.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/datasizeunit.py` & `wallaroo-2023.2.1rc2/wallaroo/datasizeunit.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/deployment.py` & `wallaroo-2023.2.1rc2/wallaroo/deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/deployment_config.py` & `wallaroo-2023.2.1rc2/wallaroo/deployment_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/engine_config.py` & `wallaroo-2023.2.1rc2/wallaroo/engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/explainability.py` & `wallaroo-2023.2.1rc2/wallaroo/explainability.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/framework.py` & `wallaroo-2023.2.1rc2/wallaroo/framework.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/inference_decode.py` & `wallaroo-2023.2.1rc2/wallaroo/inference_decode.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/inference_result.py` & `wallaroo-2023.2.1rc2/wallaroo/inference_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/logs.py` & `wallaroo-2023.2.1rc2/wallaroo/logs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/model.py` & `wallaroo-2023.2.1rc2/wallaroo/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,48 @@
                 "version": self.version(),
                 "file_name": self.file_name(),
                 "image_path": self.image_path(),
                 "last_update_time": self.last_update_time(),
             }
         )
 
+    def _repr_html_(self):
+        self._rehydrate()
+        fmt = self.client._time_format
+        return f"""<table>
+        <tr>
+          <td>Name</td>
+          <td>{self._name}</td>
+        </tr>
+        <tr>
+          <td>Version</td>
+          <td>{self._version}</td>
+        </tr>
+        <tr>
+          <td>File Name</td>
+          <td>{self._file_name}</td>
+        </tr>
+        <tr>
+          <td>SHA</td>
+          <td>{self._sha}</td>
+        </tr>
+        <tr>
+          <td>Status</td>
+          <td>{self._status}</td>
+        </tr>
+        <tr>
+          <td>Image Path</td>
+          <td>{self._image_path}</td>
+        </tr>
+        <tr>
+          <td>Updated At</td>
+          <td>{self._last_update_time.strftime(fmt)}</td>
+        </tr>
+      </table>"""
+
     @staticmethod
     def as_standalone(name: str, version: str, file_name: str) -> "Model":
         """Creates a Model intended for use in generating standalone configurations"""
         constructor_dict = {
             "model_id": name,
             "model_version": version,
             "file_name": file_name,
@@ -158,14 +192,15 @@
 
     @rehydrate("_sha")
     def sha(self) -> str:
         return cast(str, self._sha)
 
     @rehydrate("_status")
     def status(self) -> str:
+        self._rehydrate()
         return cast(str, self._status)
 
     @rehydrate("_file_name")
     def file_name(self) -> str:
         return cast(str, self._file_name)
 
     @rehydrate("_image_path")
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/model_config.py` & `wallaroo-2023.2.1rc2/wallaroo/model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/model_registry.py` & `wallaroo-2023.2.1rc2/wallaroo/model_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from __future__ import annotations
+import base64
 from datetime import datetime
 from typing import TYPE_CHECKING, Any, Dict, List, Optional
 from wallaroo.framework import Framework
 from wallaroo.model import Model
+import pyarrow as pa  # type: ignore
 
 from wallaroo.task import Task, TaskList
 from wallaroo.wallaroo_ml_ops_api_client.models import registered_model_version
 from .object import (
     DehydratedValue,
     Object,
     RequiredAttributeMissing,
@@ -156,54 +158,67 @@
                 RegisteredModel(client=self.client, data=m, registry_id=self._id)
                 for m in ret.registered_models
             ]
         )
 
     def upload_model(
         self,
-        model_name: str,
-        model_version: str,
+        name: str,
+        path: str,
         framework: Framework,
+        input_schema: pa.Schema,
+        output_schema: pa.Schema,
         requirements: List[str] = [],
     ) -> Model:
         """
+        :param: name str A descriptive name to set
+        :param: path str The DBFS path to the artifact file to upload.
         :param: framework Framework The ML framework that this model uses (ex. Framework.ONNX).
         :param: requirements List[str] An optional list of python requirements needed to run this model.
+        :param: input_schema pa.Schema A PyArrow schema describing inputs to this model.
+        :param: output_schema pa.Schema A PyArrow schema describing the outputs of this model.
         :return: Model An instance of the Wallaroo model that is being created.
         """
-        from .wallaroo_ml_ops_api_client.api.model.upload_from_registry import sync
+        from .wallaroo_ml_ops_api_client.api.model.upload_from_registry import (
+            sync,
+        )
         from .wallaroo_ml_ops_api_client.models.upload_from_registry_request import (
             UploadFromRegistryRequest,
-            Conversion,
         )
+        from .wallaroo_ml_ops_api_client.models.conversion import Conversion
+
+        i_s = base64.b64encode(bytes(input_schema.serialize())).decode("utf8")
+        o_s = base64.b64encode(bytes(output_schema.serialize())).decode("utf8")
 
         ret = sync(
             client=self.client.mlops(),
             json_body=UploadFromRegistryRequest(
-                Conversion(
+                path=path,
+                name=name,
+                registry_id=self._id,
+                conversion=Conversion(
                     framework=framework._to_openapi_framework(),
                     requirements=requirements,
                 ),
-                model_name,
-                self._id,
-                model_version,
-                "private",
-                self.client.get_current_workspace()._id,
+                input_schema=i_s,
+                output_schema=o_s,
+                visibility="private",
+                workspace_id=self.client.get_current_workspace()._id,
             ),
         )
 
         if ret is None:
             raise Exception("Failed to start upload.")
 
         return Model(client=self.client, data={"id": ret.model_id})
 
     def _repr_html_(self):
         self._rehydrate()
         fmt = self.client._time_format
-        workspace_list = ", ".join([w.name for w in self._workspaces])
+        workspace_list = ", ".join([w.get("name") for w in self._workspaces])
         return f"""<table>
           <tr>
             <th>Field</th>
             <th>Value</th>
           </tr>
           <tr>
             <td>Name</td><td>{self._name}</td>
@@ -249,15 +264,15 @@
                 + f"<td>{updated_at}</td>"
                 # + f"<td>{registry.workspace_names()}</td>"
                 + "</tr>"
             )
 
         fields = [
             "name",
-            "registry type",
+            "registry url",
             "created at",
             "updated at",
             # "linked workspaces",
         ]
 
         if self == []:
             return "(no registrys)"
@@ -279,26 +294,28 @@
         data: registered_model_version.RegisteredModelVersion,
         registry_id: str,
     ):
         super().__init__(**data.to_dict())
         self._client = client
         self.registry_id = registry_id
 
+    # Deprecated code.
+    """
     def upload(self, framework: Framework, requirements: List[str] = []):
-        """Uploads this Model's source code to your Wallaroo instance.
+        # Uploads this Model's source code to your Wallaroo instance.
 
-        :param: framework Framework The ML framework that this model uses (ex. Framework.ONNX).
-        :param: requirements List[str] An optional list of python requirements needed to run this model.
-        :return: Model An instance of the Wallaroo model that is being created.
-        """
+        #:param: framework Framework The ML framework that this model uses (ex. Framework.ONNX).
+        #:param: requirements List[str] An optional list of python requirements needed to run this model.
+        #:return: Model An instance of the Wallaroo model that is being created.
+        #
         from .wallaroo_ml_ops_api_client.api.model.upload_from_registry import sync
         from .wallaroo_ml_ops_api_client.models.upload_from_registry_request import (
             UploadFromRegistryRequest,
-            Conversion,
         )
+        from .wallaroo_ml_ops_api_client.models.conversion import Conversion
 
         ret = sync(
             client=self._client.mlops(),
             json_body=UploadFromRegistryRequest(
                 Conversion(
                     framework=framework._to_openapi_framework(),
                     requirements=requirements,
@@ -311,14 +328,37 @@
             ),
         )
 
         if ret is None:
             raise Exception("Failed to start upload.")
 
         return Model(client=self._client, data={"id": ret.model_id})
+      """
+
+    def list_artifacts(self):
+        from .wallaroo_ml_ops_api_client.api.model.list_registry_model_version_artifacts import (
+            sync_detailed,
+        )
+        from .wallaroo_ml_ops_api_client.models.list_registry_model_version_artifacts_request import (
+            ListRegistryModelVersionArtifactsRequest,
+        )
+
+        ret = sync_detailed(
+            client=self._client.mlops(),
+            json_body=ListRegistryModelVersionArtifactsRequest(
+                self.name, self.registry_id, self.version
+            ),
+        )
+
+        if ret.parsed is None:
+            raise Exception(
+                f"Failed to list artifacts from remote registry: {ret.content}"
+            )
+
+        return DbfsFileList(ret.parsed)
 
     def _repr_html_(self):
         return f"""
           <table>
             <tr>
               <td>Name</td><td>{self.name}</td>
             </tr>
@@ -340,14 +380,44 @@
             <tr>
               <td>Registry Status</td><td>{self.status}</td>
             </tr>
           </table>
         """
 
 
+from .wallaroo_ml_ops_api_client.models.dbfs_list_response_file_with_full_path import (
+    DbfsListResponseFileWithFullPath,
+)
+
+
+class DbfsFileList(List[DbfsListResponseFileWithFullPath]):
+    def _repr_html_(self):
+        def row(file: DbfsListResponseFileWithFullPath):
+            [_, file_name] = file.path.rsplit("/", 1)
+
+            return f"""
+            <tr>
+              <td>{file_name}</td>
+              <td>{file.file_size}B</td>
+              <td>{file.full_path}</td>
+            </tr>
+            """
+
+        return f"""
+          <table>
+            <tr>
+              <th>File Name</th>
+              <th>File Size</th>
+              <th>Full Path</th>
+            </tr>
+            {"".join(row(file) for file in self)}
+          </table>
+        """
+
+
 class RegisteredModelVersionsList(List[RegisteredModelVersion]):
     """Wraps a list of Model Registries for display in a display-aware environment like Jupyter."""
 
     def _repr_html_(self) -> str:
         def row(vers: RegisteredModelVersion):
             return f"""
             <tr>
@@ -395,22 +465,20 @@
         self.versions = RegisteredModelVersionsList(
             [
                 RegisteredModelVersion(client, vers, registry_id=self.registry_id)
                 for vers in latest_versions
             ]
         )
 
-    def upload(self, framework: Framework, requirements: List[str] = []) -> Model:
-        """Upload the most recent version of this model to Wallaroo.
-
-        :param: framework Framework The ML framework that this model uses (ex. Framework.ONNX).
-        :param: requirements List[str] An optional list of python requirements needed to run this model.
-        :return: Model An instance of the Wallaroo model that is being created.
-        """
-        return self.versions[0].upload(framework=framework, requirements=requirements)
+    def list_artifacts(self):
+        recent_version = self.versions[0]
+        print(
+            f"Listing artifacts for the most recent version ({recent_version.version})"
+        )
+        return recent_version.list_artifacts()
 
     def _repr_html_(self):
         fmt = self._client._time_format
         return f"""
         <table>
           <tr>
             <td>Name</td>
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/models.py` & `wallaroo-2023.2.1rc2/wallaroo/models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/notify.py` & `wallaroo-2023.2.1rc2/wallaroo/notify.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/object.py` & `wallaroo-2023.2.1rc2/wallaroo/object.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/orchestration.py` & `wallaroo-2023.2.1rc2/wallaroo/orchestration.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/pipeline.py` & `wallaroo-2023.2.1rc2/wallaroo/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,14 +333,37 @@
         if data is None:
             raise Exception("Failed to get pipeline version")
         if not isinstance(data, PipelinesGetVersionResponse200):
             raise Exception(data.msg)
         # TODO: Get pipeline version id and return PipelineVariant?
         return data.to_dict()
 
+    @staticmethod
+    def _write_metadata_warning(log_table):
+        if "metadata.dropped" in log_table.column_names:
+            flattened_metadata = log_table["metadata.dropped"].flatten()
+            if len(flattened_metadata[0][0]) > 0:
+                dropped_columns = flattened_metadata[0][0]
+                sys.stderr.write(
+                    f"Warning: The inference log is above the allowable limit and the following columns may have"
+                    f" been suppressed for various rows in the logs: {dropped_columns}."
+                    f" To review the dropped columns for an individual inference’s suppressed data,"
+                    f' include dataset=["metadata"] in the log request.'
+                    f"\n"
+                )
+
+    @staticmethod
+    def _drop_metadata_columns(dataset, log_table):
+        columns_to_drop = []
+        if dataset is None or "metadata" not in dataset:
+            for column_name in log_table.column_names:
+                if column_name.startswith("metadata"):
+                    columns_to_drop.append(column_name)
+        return log_table.drop(columns_to_drop)
+
     def logs(
         self,
         limit: Optional[int] = None,
         start_datetime: Optional[datetime.datetime] = None,
         end_datetime: Optional[datetime.datetime] = None,
         valid: Optional[bool] = None,
         dataset: Optional[List[str]] = None,
@@ -412,15 +435,22 @@
                     if start_datetime is not None and end_datetime is not None
                     else "newest"
                 )
                 sys.stderr.write(
                     f"Pipeline log schema has changed over the logs requested {entries.num_rows}"
                     f" {chronological_order} records retrieved successfully, {chronological_order}"
                     f" record seen was at <datetime>. Please request additional records separately"
+                    f"\n"
                 )
+
+            self._write_metadata_warning(entries)
+            entries = self._drop_metadata_columns(dataset, entries)
+            with pa.OSFile("tensor_dropped_no_metadata.arrow", "wb") as f:
+                with pa.ipc.new_file(f, entries.schema) as writer:
+                    writer.write(entries)
             if not arrow:
                 entries = entries.to_pandas()
         else:
             if self._last_infer_time is not None:
                 for ix in range(5):
                     if entries and self._last_infer_time <= max(
                         e.timestamp for e in entries
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/pipeline_config.py` & `wallaroo-2023.2.1rc2/wallaroo/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/pipeline_variant.py` & `wallaroo-2023.2.1rc2/wallaroo/pipeline_variant.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/queries.py` & `wallaroo-2023.2.1rc2/wallaroo/queries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/standalone_client.py` & `wallaroo-2023.2.1rc2/wallaroo/standalone_client.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/tag.py` & `wallaroo-2023.2.1rc2/wallaroo/tag.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/task.py` & `wallaroo-2023.2.1rc2/wallaroo/task.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/task_run.py` & `wallaroo-2023.2.1rc2/wallaroo/task_run.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/user.py` & `wallaroo-2023.2.1rc2/wallaroo/user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/utils.py` & `wallaroo-2023.2.1rc2/wallaroo/utils.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDefaultUserWorkspace.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDefaultUserWorkspace.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/CreateDeployment.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/CreateDeployment.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/CreatePipelineWithDefinition.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/CreatePipelineWithDefinition.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/GetPipelineByName.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/GetPipelineByName.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/InsertConfiguredModel.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/InsertConfiguredModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModel.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/InsertModelConfigFull.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/InsertModelConfigFull.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/PipelineVariantById.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/PipelineVariantById.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModel.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModel.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/UpdateModelConversionMetaData.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/UpdateModelConversionMetaData.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/CreateAssay.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/CreateAssay.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/Assays/ListAssays.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/Assays/ListAssays.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityConfig.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/explainability/CreateExplainabilityRequest.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/pipelines/ListPublishedPipelines.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/InsertTask.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/InsertTask.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasks.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasks.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/ListTasksByOrchSha.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/README.md` & `wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/graphql/tasks/UpdateTask.graphql` & `wallaroo-2023.2.1rc2/wallaroo/graphql/tasks/UpdateTask.graphql`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/README.md` & `wallaroo-2023.2.1rc2/wallaroo/records/README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/convert_keras_model.py` & `wallaroo-2023.2.1rc2/wallaroo/records/convert_keras_model.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/graphql_queries.py` & `wallaroo-2023.2.1rc2/wallaroo/records/graphql_queries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/telemetry_body.py` & `wallaroo-2023.2.1rc2/wallaroo/records/telemetry_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/telemetry_error.py` & `wallaroo-2023.2.1rc2/wallaroo/records/telemetry_error.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/v1_metric_response.py` & `wallaroo-2023.2.1rc2/wallaroo/records/v1_metric_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/records/v1_tls_response.py` & `wallaroo-2023.2.1rc2/wallaroo/records/v1_tls_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/client.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/client.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/types.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/types.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_external_url.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/admin/admin_get_pipeline_internal_url.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_filter.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_assay_results.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_get_baseline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_run_interactive_baseline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/assay/assays_set_active.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_add_to_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_delete.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_get_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/connection/connections_remove_from_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_create_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_result.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_get_status.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_configs_by_pipeline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/explainability/explainability_list_requests.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/features_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/misc/status_get_deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/attach_registry_to_workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/attach_registry_to_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/create_registry.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/create_registry.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/get_model_version_by_id.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/get_model_version_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/get_registry.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/get_registry.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     *,
     client: Client,
     json_body: GetRegistryRequest,
 
 ) -> Response[GetRegistryResponse200]:
     """ 
     Args:
-        json_body (GetRegistryRequest): Payload for the List Registries call.
+        json_body (GetRegistryRequest): Payload for the Get Registry call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetRegistryResponse200]
@@ -103,15 +103,15 @@
     *,
     client: Client,
     json_body: GetRegistryRequest,
 
 ) -> Optional[GetRegistryResponse200]:
     """ 
     Args:
-        json_body (GetRegistryRequest): Payload for the List Registries call.
+        json_body (GetRegistryRequest): Payload for the Get Registry call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetRegistryResponse200
@@ -128,15 +128,15 @@
     *,
     client: Client,
     json_body: GetRegistryRequest,
 
 ) -> Response[GetRegistryResponse200]:
     """ 
     Args:
-        json_body (GetRegistryRequest): Payload for the List Registries call.
+        json_body (GetRegistryRequest): Payload for the Get Registry call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetRegistryResponse200]
@@ -160,15 +160,15 @@
     *,
     client: Client,
     json_body: GetRegistryRequest,
 
 ) -> Optional[GetRegistryResponse200]:
     """ 
     Args:
-        json_body (GetRegistryRequest): Payload for the List Registries call.
+        json_body (GetRegistryRequest): Payload for the Get Registry call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetRegistryResponse200
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registries.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registries.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registry_models.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/list_registry_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     *,
     client: Client,
     json_body: ListRegistryModelsRequest,
 
 ) -> Response[SearchRegisteredModelsResponse]:
     """ 
     Args:
-        json_body (ListRegistryModelsRequest): Payload for the List Registries call.
+        json_body (ListRegistryModelsRequest): Payload for the List Registry Models call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SearchRegisteredModelsResponse]
@@ -104,15 +104,15 @@
     *,
     client: Client,
     json_body: ListRegistryModelsRequest,
 
 ) -> Optional[SearchRegisteredModelsResponse]:
     """ 
     Args:
-        json_body (ListRegistryModelsRequest): Payload for the List Registries call.
+        json_body (ListRegistryModelsRequest): Payload for the List Registry Models call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         SearchRegisteredModelsResponse
@@ -129,15 +129,15 @@
     *,
     client: Client,
     json_body: ListRegistryModelsRequest,
 
 ) -> Response[SearchRegisteredModelsResponse]:
     """ 
     Args:
-        json_body (ListRegistryModelsRequest): Payload for the List Registries call.
+        json_body (ListRegistryModelsRequest): Payload for the List Registry Models call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SearchRegisteredModelsResponse]
@@ -161,15 +161,15 @@
     *,
     client: Client,
     json_body: ListRegistryModelsRequest,
 
 ) -> Optional[SearchRegisteredModelsResponse]:
     """ 
     Args:
-        json_body (ListRegistryModelsRequest): Payload for the List Registries call.
+        json_body (ListRegistryModelsRequest): Payload for the List Registry Models call.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         SearchRegisteredModelsResponse
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_get.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_list_versions.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/models_upload_stream.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/remove_registry_from_workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/remove_registry_from_workspace.py`

 * *Files 9% similar despite different names*

```diff
@@ -73,16 +73,16 @@
     *,
     client: Client,
     json_body: RemoveRegistryFromWorkspaceRequest,
 
 ) -> Response[RemoveRegistryFromWorkspaceResponse200]:
     """ 
     Args:
-        json_body (RemoveRegistryFromWorkspaceRequest): The required information for creating a
-            Model Registry
+        json_body (RemoveRegistryFromWorkspaceRequest): The required information for removing a
+            Model Registry from a workspace
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RemoveRegistryFromWorkspaceResponse200]
@@ -106,16 +106,16 @@
     *,
     client: Client,
     json_body: RemoveRegistryFromWorkspaceRequest,
 
 ) -> Optional[RemoveRegistryFromWorkspaceResponse200]:
     """ 
     Args:
-        json_body (RemoveRegistryFromWorkspaceRequest): The required information for creating a
-            Model Registry
+        json_body (RemoveRegistryFromWorkspaceRequest): The required information for removing a
+            Model Registry from a workspace
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         RemoveRegistryFromWorkspaceResponse200
@@ -132,16 +132,16 @@
     *,
     client: Client,
     json_body: RemoveRegistryFromWorkspaceRequest,
 
 ) -> Response[RemoveRegistryFromWorkspaceResponse200]:
     """ 
     Args:
-        json_body (RemoveRegistryFromWorkspaceRequest): The required information for creating a
-            Model Registry
+        json_body (RemoveRegistryFromWorkspaceRequest): The required information for removing a
+            Model Registry from a workspace
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RemoveRegistryFromWorkspaceResponse200]
@@ -165,16 +165,16 @@
     *,
     client: Client,
     json_body: RemoveRegistryFromWorkspaceRequest,
 
 ) -> Optional[RemoveRegistryFromWorkspaceResponse200]:
     """ 
     Args:
-        json_body (RemoveRegistryFromWorkspaceRequest): The required information for creating a
-            Model Registry
+        json_body (RemoveRegistryFromWorkspaceRequest): The required information for removing a
+            Model Registry from a workspace
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         RemoveRegistryFromWorkspaceResponse200
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_and_convert.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_and_convert.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_from_registry.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/upload_from_registry.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/model/v1_model_get_model_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/get_by_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/list_.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/orchestration/upload.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_copy_pipeline.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_deploy.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_logs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_get_version.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipeline/pipelines_undeploy.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/get_publish_status.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/get_publish_status.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/list_published_pipelines.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/list_published_pipelines.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/pipelines/publish_pipeline.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.publish_request import PublishRequest
-from ...models.publish_response import PublishResponse
+from ...models.get_by_id_1_response_200 import GetById1Response200
+from ...models.get_task_by_id_request import GetTaskByIdRequest
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: PublishRequest,
+    json_body: GetTaskByIdRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/api/pipeline/publish".format(
+    url = "{}/v1/api/task/get_by_id".format(
         client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
@@ -41,55 +41,52 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[PublishResponse]:
-    if response.status_code == HTTPStatus.ACCEPTED:
-        response_202 = PublishResponse.from_dict(response.json())
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetById1Response200]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = GetById1Response200.from_dict(response.json())
 
 
 
-        return response_202
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[PublishResponse]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetById1Response200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: PublishRequest,
-
-) -> Response[PublishResponse]:
-    """ Publishes a given pipeline for deployment on the edge.
-
-     Publishes a given pipeline for deployment on the edge.
+    json_body: GetTaskByIdRequest,
 
+) -> Response[GetById1Response200]:
+    """ 
     Args:
-        json_body (PublishRequest): Request to publish a pipeline.
+        json_body (GetTaskByIdRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PublishResponse]
+        Response[GetById1Response200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -101,58 +98,52 @@
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: PublishRequest,
-
-) -> Optional[PublishResponse]:
-    """ Publishes a given pipeline for deployment on the edge.
-
-     Publishes a given pipeline for deployment on the edge.
+    json_body: GetTaskByIdRequest,
 
+) -> Optional[GetById1Response200]:
+    """ 
     Args:
-        json_body (PublishRequest): Request to publish a pipeline.
+        json_body (GetTaskByIdRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PublishResponse
+        GetById1Response200
      """
 
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: PublishRequest,
-
-) -> Response[PublishResponse]:
-    """ Publishes a given pipeline for deployment on the edge.
-
-     Publishes a given pipeline for deployment on the edge.
+    json_body: GetTaskByIdRequest,
 
+) -> Response[GetById1Response200]:
+    """ 
     Args:
-        json_body (PublishRequest): Request to publish a pipeline.
+        json_body (GetTaskByIdRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[PublishResponse]
+        Response[GetById1Response200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -164,30 +155,27 @@
         )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: PublishRequest,
-
-) -> Optional[PublishResponse]:
-    """ Publishes a given pipeline for deployment on the edge.
-
-     Publishes a given pipeline for deployment on the edge.
+    json_body: GetTaskByIdRequest,
 
+) -> Optional[GetById1Response200]:
+    """ 
     Args:
-        json_body (PublishRequest): Request to publish a pipeline.
+        json_body (GetTaskByIdRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        PublishResponse
+        GetById1Response200
      """
 
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_pipeline_topic_name.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/plateau/plateau_get_topic_name.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/cron_job.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_by_id1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_logs_for_run.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_by_id_1_response_200 import GetById1Response200
-from ...models.get_task_by_id_request import GetTaskByIdRequest
+from ...models.get_logs_for_run_request import GetLogsForRunRequest
+from ...models.get_logs_for_run_response_200 import GetLogsForRunResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: GetTaskByIdRequest,
+    json_body: GetLogsForRunRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/api/task/get_by_id".format(
+    url = "{}/v1/api/task/get_logs_for_run".format(
         client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
@@ -41,52 +41,52 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetById1Response200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetLogsForRunResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetById1Response200.from_dict(response.json())
+        response_200 = GetLogsForRunResponse200.from_dict(response.json())
 
 
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetById1Response200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetLogsForRunResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: GetTaskByIdRequest,
+    json_body: GetLogsForRunRequest,
 
-) -> Response[GetById1Response200]:
+) -> Response[GetLogsForRunResponse200]:
     """ 
     Args:
-        json_body (GetTaskByIdRequest):
+        json_body (GetLogsForRunRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetById1Response200]
+        Response[GetLogsForRunResponse200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -98,52 +98,52 @@
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: GetTaskByIdRequest,
+    json_body: GetLogsForRunRequest,
 
-) -> Optional[GetById1Response200]:
+) -> Optional[GetLogsForRunResponse200]:
     """ 
     Args:
-        json_body (GetTaskByIdRequest):
+        json_body (GetLogsForRunRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetById1Response200
+        GetLogsForRunResponse200
      """
 
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: GetTaskByIdRequest,
+    json_body: GetLogsForRunRequest,
 
-) -> Response[GetById1Response200]:
+) -> Response[GetLogsForRunResponse200]:
     """ 
     Args:
-        json_body (GetTaskByIdRequest):
+        json_body (GetLogsForRunRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetById1Response200]
+        Response[GetLogsForRunResponse200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -155,27 +155,27 @@
         )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: GetTaskByIdRequest,
+    json_body: GetLogsForRunRequest,
 
-) -> Optional[GetById1Response200]:
+) -> Optional[GetLogsForRunResponse200]:
     """ 
     Args:
-        json_body (GetTaskByIdRequest):
+        json_body (GetLogsForRunRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetById1Response200
+        GetLogsForRunResponse200
      """
 
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_logs_for_run.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_tasks_by_orch_sha.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_logs_for_run_request import GetLogsForRunRequest
-from ...models.get_logs_for_run_response_200 import GetLogsForRunResponse200
+from ...models.get_tasks_by_orch_sha_request import GetTasksByOrchShaRequest
+from ...models.get_tasks_by_orch_sha_response_200 import \
+    GetTasksByOrchShaResponse200
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: GetLogsForRunRequest,
+    json_body: GetTasksByOrchShaRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/api/task/get_logs_for_run".format(
+    url = "{}/v1/api/task/get_tasks_by_orch_sha".format(
         client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
@@ -41,52 +42,52 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetLogsForRunResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetTasksByOrchShaResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetLogsForRunResponse200.from_dict(response.json())
+        response_200 = GetTasksByOrchShaResponse200.from_dict(response.json())
 
 
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetLogsForRunResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[GetTasksByOrchShaResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: GetLogsForRunRequest,
+    json_body: GetTasksByOrchShaRequest,
 
-) -> Response[GetLogsForRunResponse200]:
+) -> Response[GetTasksByOrchShaResponse200]:
     """ 
     Args:
-        json_body (GetLogsForRunRequest):
+        json_body (GetTasksByOrchShaRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetLogsForRunResponse200]
+        Response[GetTasksByOrchShaResponse200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -98,52 +99,52 @@
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: GetLogsForRunRequest,
+    json_body: GetTasksByOrchShaRequest,
 
-) -> Optional[GetLogsForRunResponse200]:
+) -> Optional[GetTasksByOrchShaResponse200]:
     """ 
     Args:
-        json_body (GetLogsForRunRequest):
+        json_body (GetTasksByOrchShaRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetLogsForRunResponse200
+        GetTasksByOrchShaResponse200
      """
 
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: GetLogsForRunRequest,
+    json_body: GetTasksByOrchShaRequest,
 
-) -> Response[GetLogsForRunResponse200]:
+) -> Response[GetTasksByOrchShaResponse200]:
     """ 
     Args:
-        json_body (GetLogsForRunRequest):
+        json_body (GetTasksByOrchShaRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetLogsForRunResponse200]
+        Response[GetTasksByOrchShaResponse200]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -155,27 +156,27 @@
         )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: GetLogsForRunRequest,
+    json_body: GetTasksByOrchShaRequest,
 
-) -> Optional[GetLogsForRunResponse200]:
+) -> Optional[GetTasksByOrchShaResponse200]:
     """ 
     Args:
-        json_body (GetLogsForRunRequest):
+        json_body (GetTasksByOrchShaRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetLogsForRunResponse200
+        GetTasksByOrchShaResponse200
      """
 
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_run_details.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/get_run_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/get_tasks_by_orch_sha.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list_task_runs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from http import HTTPStatus
-from typing import Any, Dict, Optional
+from typing import Any, Dict, List, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.get_tasks_by_orch_sha_request import GetTasksByOrchShaRequest
-from ...models.get_tasks_by_orch_sha_response_200 import \
-    GetTasksByOrchShaResponse200
+from ...models.list_task_runs_request import ListTaskRunsRequest
+from ...models.list_task_runs_response_task_runs import \
+    ListTaskRunsResponseTaskRuns
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: GetTasksByOrchShaRequest,
+    json_body: ListTaskRunsRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/api/task/get_tasks_by_orch_sha".format(
+    url = "{}/v1/api/task/list_task_runs".format(
         client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
@@ -42,52 +42,57 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[GetTasksByOrchShaResponse200]:
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetTasksByOrchShaResponse200.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in (_response_200):
+            response_200_item = ListTaskRunsResponseTaskRuns.from_dict(response_200_item_data)
 
 
 
+            response_200.append(response_200_item)
+
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[GetTasksByOrchShaResponse200]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[List['ListTaskRunsResponseTaskRuns']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: GetTasksByOrchShaRequest,
+    json_body: ListTaskRunsRequest,
 
-) -> Response[GetTasksByOrchShaResponse200]:
+) -> Response[List['ListTaskRunsResponseTaskRuns']]:
     """ 
     Args:
-        json_body (GetTasksByOrchShaRequest):
+        json_body (ListTaskRunsRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetTasksByOrchShaResponse200]
+        Response[List['ListTaskRunsResponseTaskRuns']]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -99,52 +104,52 @@
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: GetTasksByOrchShaRequest,
+    json_body: ListTaskRunsRequest,
 
-) -> Optional[GetTasksByOrchShaResponse200]:
+) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
     """ 
     Args:
-        json_body (GetTasksByOrchShaRequest):
+        json_body (ListTaskRunsRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetTasksByOrchShaResponse200
+        List['ListTaskRunsResponseTaskRuns']
      """
 
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: GetTasksByOrchShaRequest,
+    json_body: ListTaskRunsRequest,
 
-) -> Response[GetTasksByOrchShaResponse200]:
+) -> Response[List['ListTaskRunsResponseTaskRuns']]:
     """ 
     Args:
-        json_body (GetTasksByOrchShaRequest):
+        json_body (ListTaskRunsRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetTasksByOrchShaResponse200]
+        Response[List['ListTaskRunsResponseTaskRuns']]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -156,27 +161,27 @@
         )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: GetTasksByOrchShaRequest,
+    json_body: ListTaskRunsRequest,
 
-) -> Optional[GetTasksByOrchShaResponse200]:
+) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
     """ 
     Args:
-        json_body (GetTasksByOrchShaRequest):
+        json_body (ListTaskRunsRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetTasksByOrchShaResponse200
+        List['ListTaskRunsResponseTaskRuns']
      """
 
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/kill.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/list1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/task/list_task_runs.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/task/oneshot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from http import HTTPStatus
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import Client
-from ...models.list_task_runs_request import ListTaskRunsRequest
-from ...models.list_task_runs_response_task_runs import \
-    ListTaskRunsResponseTaskRuns
+from ...models.oneshot_request import OneshotRequest
+from ...models.oneshot_response_201 import OneshotResponse201
 from ...types import Response
 
 
 def _get_kwargs(
     *,
     client: Client,
-    json_body: ListTaskRunsRequest,
+    json_body: OneshotRequest,
 
 ) -> Dict[str, Any]:
-    url = "{}/v1/api/task/list_task_runs".format(
+    url = "{}/v1/api/task/run_once".format(
         client.base_url)
 
     headers: Dict[str, str] = client.get_headers()
     cookies: Dict[str, Any] = client.get_cookies()
 
     
 
@@ -42,57 +41,52 @@
         "cookies": cookies,
         "timeout": client.get_timeout(),
         "follow_redirects": client.follow_redirects,
         "json": json_json_body,
     }
 
 
-def _parse_response(*, client: Client, response: httpx.Response) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
-    if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in (_response_200):
-            response_200_item = ListTaskRunsResponseTaskRuns.from_dict(response_200_item_data)
+def _parse_response(*, client: Client, response: httpx.Response) -> Optional[OneshotResponse201]:
+    if response.status_code == HTTPStatus.CREATED:
+        response_201 = OneshotResponse201.from_dict(response.json())
 
 
 
-            response_200.append(response_200_item)
-
-        return response_200
+        return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Client, response: httpx.Response) -> Response[List['ListTaskRunsResponseTaskRuns']]:
+def _build_response(*, client: Client, response: httpx.Response) -> Response[OneshotResponse201]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
     client: Client,
-    json_body: ListTaskRunsRequest,
+    json_body: OneshotRequest,
 
-) -> Response[List['ListTaskRunsResponseTaskRuns']]:
+) -> Response[OneshotResponse201]:
     """ 
     Args:
-        json_body (ListTaskRunsRequest):
+        json_body (OneshotRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ListTaskRunsResponseTaskRuns']]
+        Response[OneshotResponse201]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -104,52 +98,52 @@
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     *,
     client: Client,
-    json_body: ListTaskRunsRequest,
+    json_body: OneshotRequest,
 
-) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
+) -> Optional[OneshotResponse201]:
     """ 
     Args:
-        json_body (ListTaskRunsRequest):
+        json_body (OneshotRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ListTaskRunsResponseTaskRuns']
+        OneshotResponse201
      """
 
 
     return sync_detailed(
         client=client,
 json_body=json_body,
 
     ).parsed
 
 async def asyncio_detailed(
     *,
     client: Client,
-    json_body: ListTaskRunsRequest,
+    json_body: OneshotRequest,
 
-) -> Response[List['ListTaskRunsResponseTaskRuns']]:
+) -> Response[OneshotResponse201]:
     """ 
     Args:
-        json_body (ListTaskRunsRequest):
+        json_body (OneshotRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['ListTaskRunsResponseTaskRuns']]
+        Response[OneshotResponse201]
      """
 
 
     kwargs = _get_kwargs(
         client=client,
 json_body=json_body,
 
@@ -161,27 +155,27 @@
         )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     *,
     client: Client,
-    json_body: ListTaskRunsRequest,
+    json_body: OneshotRequest,
 
-) -> Optional[List['ListTaskRunsResponseTaskRuns']]:
+) -> Optional[OneshotResponse201]:
     """ 
     Args:
-        json_body (ListTaskRunsRequest):
+        json_body (OneshotRequest):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['ListTaskRunsResponseTaskRuns']
+        OneshotResponse201
      """
 
 
     return (await asyncio_detailed(
         client=client,
 json_body=json_body,
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_activate.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_deactivate.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_invite.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/user/users_query.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_add_user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_create.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_list_users.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/api/workspace/workspaces_remove_user.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,17 @@
 from .create_registry_response_200 import CreateRegistryResponse200
 from .cron_job_exec import CronJobExec
 from .cron_job_json_body import CronJobJsonBody
 from .cron_job_json_body_json import CronJobJsonBodyJson
 from .cron_job_request import CronJobRequest
 from .cron_job_request_json import CronJobRequestJson
 from .cron_job_response_201 import CronJobResponse201
+from .dbfs_list_response_file import DbfsListResponseFile
+from .dbfs_list_response_file_with_full_path import \
+    DbfsListResponseFileWithFullPath
 from .event_base import EventBase
 from .event_base_extra_env_vars import EventBaseExtraEnvVars
 from .explainability_create_config_json_body import \
     ExplainabilityCreateConfigJsonBody
 from .explainability_create_config_json_body_feature_bounds import \
     ExplainabilityCreateConfigJsonBodyFeatureBounds
 from .explainability_create_config_response_200 import \
@@ -449,14 +452,16 @@
 from .insert_models import InsertModels
 from .insert_task_response import InsertTaskResponse
 from .kill_request import KillRequest
 from .kill_response_202 import KillResponse202
 from .kill_response_202_input_data import KillResponse202InputData
 from .list_orchestrations_request import ListOrchestrationsRequest
 from .list_registries_request import ListRegistriesRequest
+from .list_registry_model_version_artifacts_request import \
+    ListRegistryModelVersionArtifactsRequest
 from .list_registry_models_request import ListRegistryModelsRequest
 from .list_request import ListRequest
 from .list_task_runs_request import ListTaskRunsRequest
 from .list_task_runs_request_status import ListTaskRunsRequestStatus
 from .list_task_runs_response_task_runs import ListTaskRunsResponseTaskRuns
 from .list_tasks_request import ListTasksRequest
 from .model_id import ModelId
@@ -561,15 +566,14 @@
     PlateauGetPipelineTopicNameResponse500
 from .plateau_get_topic_name_json_body import PlateauGetTopicNameJsonBody
 from .plateau_get_topic_name_response_200 import PlateauGetTopicNameResponse200
 from .plateau_get_topic_name_response_400 import PlateauGetTopicNameResponse400
 from .plateau_get_topic_name_response_401 import PlateauGetTopicNameResponse401
 from .plateau_get_topic_name_response_500 import PlateauGetTopicNameResponse500
 from .publish_request import PublishRequest
-from .publish_response import PublishResponse
 from .python_version import PythonVersion
 from .registered_model import RegisteredModel
 from .registered_model_version import RegisteredModelVersion
 from .remove_registry_from_workspace_request import \
     RemoveRegistryFromWorkspaceRequest
 from .remove_registry_from_workspace_response import \
     RemoveRegistryFromWorkspaceResponse
@@ -914,14 +918,16 @@
     "CreateRegistryResponse200",
     "CronJobExec",
     "CronJobJsonBody",
     "CronJobJsonBodyJson",
     "CronJobRequest",
     "CronJobRequestJson",
     "CronJobResponse201",
+    "DbfsListResponseFile",
+    "DbfsListResponseFileWithFullPath",
     "EventBase",
     "EventBaseExtraEnvVars",
     "ExplainabilityCreateConfigJsonBody",
     "ExplainabilityCreateConfigJsonBodyFeatureBounds",
     "ExplainabilityCreateConfigResponse200",
     "ExplainabilityCreateConfigResponse400",
     "ExplainabilityCreateConfigResponse401",
@@ -992,14 +998,15 @@
     "InsertTaskResponse",
     "KillRequest",
     "KillResponse202",
     "KillResponse202InputData",
     "ListOrchestrationsRequest",
     "ListRegistriesRequest",
     "ListRegistryModelsRequest",
+    "ListRegistryModelVersionArtifactsRequest",
     "ListRequest",
     "ListTaskRunsRequest",
     "ListTaskRunsRequestStatus",
     "ListTaskRunsResponseTaskRuns",
     "ListTasksRequest",
     "ModelId",
     "ModelRegistry",
@@ -1083,15 +1090,14 @@
     "PlateauGetPipelineTopicNameResponse500",
     "PlateauGetTopicNameJsonBody",
     "PlateauGetTopicNameResponse200",
     "PlateauGetTopicNameResponse400",
     "PlateauGetTopicNameResponse401",
     "PlateauGetTopicNameResponse500",
     "PublishRequest",
-    "PublishResponse",
     "PythonVersion",
     "RegisteredModel",
     "RegisteredModelVersion",
     "RemoveRegistryFromWorkspaceRequest",
     "RemoveRegistryFromWorkspaceResponse",
     "RemoveRegistryFromWorkspaceResponse200",
     "SearchRegisteredModelsResponse",
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_external_url_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/admin_get_pipeline_internal_url_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_json_body_drift_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_200_item_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_filter_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_baseline_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_200_item_window_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_assay_results_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_json_body_next.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_get_baseline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_200_item_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_baseline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_0_user_provided.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_1_fixed.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_baseline_type_2_sliding.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_json_body_window.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_baseline_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_0.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_summarizer_type_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_200_item_window_summary.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_run_interactive_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/assays_set_active_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/attach_registry_to_workspace_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_add_to_workspace_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_json_body_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_409.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_409.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_delete_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_200_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_404.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_by_id_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_200_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_404.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_get_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_200_connections_item_details.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/connections_remove_from_workspace_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/conversion.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/conversion.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/create_registry_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_exec.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_json_body_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_request_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/cron_job_response_201.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/event_base_extra_env_vars.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_json_body_feature_bounds.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_reference_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_json_body_window_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_create_request_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_request_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_result_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_get_status_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_by_pipeline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_configs_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/explainability_list_requests_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/features_list_response_200_features.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/file_info.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/file_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/framework.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/framework.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_by_id_1_response_200_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_logs_for_run_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_model_by_id_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_model_by_id_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_orchestration_by_id_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 T = TypeVar("T", bound="GetRegistryRequest")
 
 
 @attr.s(auto_attribs=True)
 class GetRegistryRequest:
-    """ Payload for the List Registries call.
+    """ Payload for the Get Registry call.
 
         Attributes:
             registry_id (str):
      """
 
     registry_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 T = TypeVar("T", bound="GetRegistryResponse")
 
 
 @attr.s(auto_attribs=True)
 class GetRegistryResponse:
-    """ Response object for the List Registries call.
+    """ Response object for the Get Registry call.
 
         Attributes:
             created_at (datetime.datetime):
             name (str): A descriptive name for this registry
             token (str): A user token with access to the Registry.
                 Tokens must be in base64 format.
             updated_at (datetime.datetime):
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_200.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 T = TypeVar("T", bound="GetRegistryResponse200")
 
 
 @attr.s(auto_attribs=True)
 class GetRegistryResponse200:
-    """ Response object for the List Registries call.
+    """ Response object for the Get Registry call.
 
         Attributes:
             created_at (datetime.datetime):
             name (str): A descriptive name for this registry
             token (str): A user token with access to the Registry.
                 Tokens must be in base64 format.
             updated_at (datetime.datetime):
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_workspace.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_registry_response_workspace.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_run_details_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_task_by_id_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/get_tasks_by_orch_sha_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_models.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/insert_task_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/kill_response_202_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_orchestrations_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_registries_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_registries_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_registry_models_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_registry_models_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 T = TypeVar("T", bound="ListRegistryModelsRequest")
 
 
 @attr.s(auto_attribs=True)
 class ListRegistryModelsRequest:
-    """ Payload for the List Registries call.
+    """ Payload for the List Registry Models call.
 
         Attributes:
             registry_id (str):
      """
 
     registry_id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_response_task_runs.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_task_runs_response_task_runs.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/list_tasks_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_id.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_id.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_registry.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_registry.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/model_version.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/model_version.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_200_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_get_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_200_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_200_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_list_versions_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_200_insert_models_returning_item_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/models_upload_stream_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/network_service_exec.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec_exec_type.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_exec_exec_type.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_request_json.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/oneshot_response_201.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/orchestration.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_json_body_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_200_deployment.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_copy_pipeline_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_json_body_definition.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_engine_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_json_body_models_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_deploy_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_502.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_logs_response_502.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_200_definition.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_get_version_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/pipelines_undeploy_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_pipeline_topic_name_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/plateau_get_topic_name_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/publish_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/publish_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,34 +5,42 @@
 T = TypeVar("T", bound="PublishRequest")
 
 
 @attr.s(auto_attribs=True)
 class PublishRequest:
     """ Request to publish a pipeline.
 
+        Attributes:
+            pipeline_id (int):
      """
 
+    pipeline_id: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        
+        pipeline_id = self.pipeline_id
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
+            "pipeline_id": pipeline_id,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        pipeline_id = d.pop("pipeline_id")
+
         publish_request = cls(
+            pipeline_id=pipeline_id,
         )
 
         publish_request.additional_properties = d
         return publish_request
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/publish_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="PublishResponse")
+T = TypeVar("T", bound="StatusRequest")
 
 
 @attr.s(auto_attribs=True)
-class PublishResponse:
-    """ Response with published pipeline id.
+class StatusRequest:
+    """ Request to fetch a pipeline publish status.
 
         Attributes:
-            id (str): published pipeline id
+            id (int): The ID of the pipeline publish
      """
 
-    id: str
+    id: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         field_dict: Dict[str, Any] = {}
@@ -31,20 +31,20 @@
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
-        publish_response = cls(
+        status_request = cls(
             id=id,
         )
 
-        publish_response.additional_properties = d
-        return publish_response
+        status_request.additional_properties = d
+        return status_request
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/registered_model.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/registered_model.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/registered_model_version.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/registered_model_version.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import attr
 
 T = TypeVar("T", bound="RemoveRegistryFromWorkspaceRequest")
 
 
 @attr.s(auto_attribs=True)
 class RemoveRegistryFromWorkspaceRequest:
-    """ The required information for creating a Model Registry
+    """ The required information for removing a Model Registry from a workspace
 
         Attributes:
             registry_id (str):
             workspace_id (int):
      """
 
     registry_id: str
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/remove_registry_from_workspace_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/search_registered_models_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/search_registered_models_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engine_lbs_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_model_statuses.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_engines_item_pipeline_statuses.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_helm_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_200_sidekicks_item_info_labels.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/status_get_deployment_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/status_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="StatusRequest")
+T = TypeVar("T", bound="UploadResponse")
 
 
 @attr.s(auto_attribs=True)
-class StatusRequest:
-    """ Request to fetch a pipeline publish status.
-
+class UploadResponse:
+    """ 
         Attributes:
-            id (str): pipeline id
+            id (str):
      """
 
     id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
@@ -31,20 +30,20 @@
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
-        status_request = cls(
+        upload_response = cls(
             id=id,
         )
 
-        status_request.additional_properties = d
-        return status_request
+        upload_response.additional_properties = d
+        return upload_response
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_input_data.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/task_run.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/task_run.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,55 +16,55 @@
 
 @attr.s(auto_attribs=True)
 class UploadFromRegistryRequest:
     """ Payload for the List Registries call.
 
         Attributes:
             conversion (Conversion):
-            name (str): The name of the model in the remote Model Registry.
+            name (str): A descriptive, DNS-safe name for this model in the Wallaroo system.
+            path (str): The path to the model file in the remote Model Registry.
             registry_id (str): The unique identifier of the Model Registry in the Wallaroo system.
-            version (str): The version of the model in the remote Model Registry
             visibility (str):
             workspace_id (int):
             image_path (Union[Unset, None, str]):
             input_schema (Union[Unset, None, str]):
             output_schema (Union[Unset, None, str]):
      """
 
     conversion: 'Conversion'
     name: str
+    path: str
     registry_id: str
-    version: str
     visibility: str
     workspace_id: int
     image_path: Union[Unset, None, str] = UNSET
     input_schema: Union[Unset, None, str] = UNSET
     output_schema: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         conversion = self.conversion.to_dict()
 
         name = self.name
+        path = self.path
         registry_id = self.registry_id
-        version = self.version
         visibility = self.visibility
         workspace_id = self.workspace_id
         image_path = self.image_path
         input_schema = self.input_schema
         output_schema = self.output_schema
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "conversion": conversion,
             "name": name,
+            "path": path,
             "registry_id": registry_id,
-            "version": version,
             "visibility": visibility,
             "workspace_id": workspace_id,
         })
         if image_path is not UNSET:
             field_dict["image_path"] = image_path
         if input_schema is not UNSET:
             field_dict["input_schema"] = input_schema
@@ -82,33 +82,33 @@
         conversion = Conversion.from_dict(d.pop("conversion"))
 
 
 
 
         name = d.pop("name")
 
-        registry_id = d.pop("registry_id")
+        path = d.pop("path")
 
-        version = d.pop("version")
+        registry_id = d.pop("registry_id")
 
         visibility = d.pop("visibility")
 
         workspace_id = d.pop("workspace_id")
 
         image_path = d.pop("image_path", UNSET)
 
         input_schema = d.pop("input_schema", UNSET)
 
         output_schema = d.pop("output_schema", UNSET)
 
         upload_from_registry_request = cls(
             conversion=conversion,
             name=name,
+            path=path,
             registry_id=registry_id,
-            version=version,
             visibility=visibility,
             workspace_id=workspace_id,
             image_path=image_path,
             input_schema=input_schema,
             output_schema=output_schema,
         )
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_from_registry_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_payload_doc_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_request_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_request_1.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,35 +21,39 @@
             conversion (Conversion):
             name (str):
             visibility (str):
             workspace_id (int):
             image_path (Union[Unset, None, str]):
             input_schema (Union[Unset, None, str]):
             output_schema (Union[Unset, None, str]):
+            registry_id (Union[Unset, None, str]): The unique identifier for a Registry
+                Not compatible with file uploads, only used with `registry_uri` uploads
      """
 
     conversion: 'Conversion'
     name: str
     visibility: str
     workspace_id: int
     image_path: Union[Unset, None, str] = UNSET
     input_schema: Union[Unset, None, str] = UNSET
     output_schema: Union[Unset, None, str] = UNSET
+    registry_id: Union[Unset, None, str] = UNSET
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
         conversion = self.conversion.to_dict()
 
         name = self.name
         visibility = self.visibility
         workspace_id = self.workspace_id
         image_path = self.image_path
         input_schema = self.input_schema
         output_schema = self.output_schema
+        registry_id = self.registry_id
 
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
             "conversion": conversion,
             "name": name,
             "visibility": visibility,
@@ -57,14 +61,16 @@
         })
         if image_path is not UNSET:
             field_dict["image_path"] = image_path
         if input_schema is not UNSET:
             field_dict["input_schema"] = input_schema
         if output_schema is not UNSET:
             field_dict["output_schema"] = output_schema
+        if registry_id is not UNSET:
+            field_dict["registry_id"] = registry_id
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
@@ -83,22 +89,25 @@
 
         image_path = d.pop("image_path", UNSET)
 
         input_schema = d.pop("input_schema", UNSET)
 
         output_schema = d.pop("output_schema", UNSET)
 
+        registry_id = d.pop("registry_id", UNSET)
+
         upload_request_1 = cls(
             conversion=conversion,
             name=name,
             visibility=visibility,
             workspace_id=workspace_id,
             image_path=image_path,
             input_schema=input_schema,
             output_schema=output_schema,
+            registry_id=registry_id,
         )
 
         upload_request_1.additional_properties = d
         return upload_request_1
 
     @property
     def additional_keys(self) -> List[str]:
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,42 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="UploadResponse")
+T = TypeVar("T", bound="WorkspacesAddUserResponse200")
 
 
 @attr.s(auto_attribs=True)
-class UploadResponse:
-    """ 
-        Attributes:
-            id (str):
+class WorkspacesAddUserResponse200:
+    """  Successful response to adding a user to workspace.
+
      """
 
-    id: str
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        id = self.id
-
+        
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
-            "id": id,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        id = d.pop("id")
-
-        upload_response = cls(
-            id=id,
+        workspaces_add_user_response_200 = cls(
         )
 
-        upload_response.additional_properties = d
-        return upload_response
+        workspaces_add_user_response_200.additional_properties = d
+        return workspaces_add_user_response_200
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/upload_response_1.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/upload_response_1.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_activate_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_deactivate_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_invite_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_200_users_additional_property.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/users_query_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_200_model_config_tensor_fields.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_config_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_200_model_config_tensor_fields.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/v1_model_get_model_by_id_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,42 +1,57 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="WorkspacesAddUserResponse200")
+T = TypeVar("T", bound="WorkspacesListResponse401")
 
 
 @attr.s(auto_attribs=True)
-class WorkspacesAddUserResponse200:
-    """  Successful response to adding a user to workspace.
+class WorkspacesListResponse401:
+    """  Error response.
 
+        Attributes:
+            msg (str):  Error message.
+            code (int):  Status code for the error.
      """
 
+    msg: str
+    code: int
     additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        
+        msg = self.msg
+        code = self.code
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
         field_dict.update({
+            "msg": msg,
+            "code": code,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        workspaces_add_user_response_200 = cls(
+        msg = d.pop("msg")
+
+        code = d.pop("code")
+
+        workspaces_list_response_401 = cls(
+            msg=msg,
+            code=code,
         )
 
-        workspaces_add_user_response_200.additional_properties = d
-        return workspaces_add_user_response_200
+        workspaces_list_response_401.additional_properties = d
+        return workspaces_list_response_401
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_add_user_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_create_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_200_workspaces_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="WorkspacesListResponse401")
+T = TypeVar("T", bound="WorkspacesRemoveUserResponse400")
 
 
 @attr.s(auto_attribs=True)
-class WorkspacesListResponse401:
+class WorkspacesRemoveUserResponse400:
     """  Error response.
 
         Attributes:
             msg (str):  Error message.
             code (int):  Status code for the error.
      """
 
@@ -37,21 +37,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         msg = d.pop("msg")
 
         code = d.pop("code")
 
-        workspaces_list_response_401 = cls(
+        workspaces_remove_user_response_400 = cls(
             msg=msg,
             code=code,
         )
 
-        workspaces_list_response_401.additional_properties = d
-        return workspaces_list_response_401
+        workspaces_remove_user_response_400.additional_properties = d
+        return workspaces_remove_user_response_400
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_200_users_item.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_400.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_list_users_response_500.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_json_body.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_200.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_400.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_500.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from typing import Any, Dict, List, Type, TypeVar
 
 import attr
 
-T = TypeVar("T", bound="WorkspacesRemoveUserResponse400")
+T = TypeVar("T", bound="WorkspacesRemoveUserResponse500")
 
 
 @attr.s(auto_attribs=True)
-class WorkspacesRemoveUserResponse400:
+class WorkspacesRemoveUserResponse500:
     """  Error response.
 
         Attributes:
             msg (str):  Error message.
             code (int):  Status code for the error.
      """
 
@@ -37,21 +37,21 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         msg = d.pop("msg")
 
         code = d.pop("code")
 
-        workspaces_remove_user_response_400 = cls(
+        workspaces_remove_user_response_500 = cls(
             msg=msg,
             code=code,
         )
 
-        workspaces_remove_user_response_400.additional_properties = d
-        return workspaces_remove_user_response_400
+        workspaces_remove_user_response_500.additional_properties = d
+        return workspaces_remove_user_response_500
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `wallaroo-2023.2.1rc1/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py` & `wallaroo-2023.2.1rc2/wallaroo/wallaroo_ml_ops_api_client/models/workspaces_remove_user_response_401.py`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/public_README.md` & `wallaroo-2023.2.1rc2/public_README.md`

 * *Files identical despite different names*

### Comparing `wallaroo-2023.2.1rc1/pyproject.toml` & `wallaroo-2023.2.1rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -63,14 +63,18 @@
 [tool.hatch.build]
 ignore-vcs = true
 exclude = ["wallaroo/graphql"]
 artifacts = ["./wallaroo/wallaroo_ml_ops_api_client"]
 
 [tool.hatch.build.force-include]
 "../api/graphql" = "wallaroo/graphql"
+"../conductor/model-auto-conversion/mac/mac" = "wallaroo/mac"
+
+[tool.hatch.build.sources]
+"wallaroo/mac" = "mac"
 
 [tool.hatch.envs.test]
 dependencies = [
   "aioresponses == 0.7.2",
   "httpx == 0.23.0",
   "pytest == 6.2.4",
   "pytest-snapshot==0.6.1",
```

### Comparing `wallaroo-2023.2.1rc1/PKG-INFO` & `wallaroo-2023.2.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wallaroo
-Version: 2023.2.1rc1
+Version: 2023.2.1rc2
 Summary: Wallaroo.ai model management API client
 Project-URL: Homepage, https://www.wallaroo.ai/
 Author-email: "Wallaroo.ai" <hello@wallaroo.ai>
 License: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
```

