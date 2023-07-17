# Comparing `tmp/torchrec_nightly-2023.7.15-py39-none-any.whl.zip` & `tmp/torchrec_nightly-2023.7.17-py39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,147 +1,150 @@
-Zip file size: 364208 bytes, number of entries: 145
--rw-r--r--  2.0 unx      811 b- defN 23-Jul-15 11:18 torchrec/__init__.py
--rw-r--r--  2.0 unx     1638 b- defN 23-Jul-15 11:18 torchrec/streamable.py
--rw-r--r--  2.0 unx      854 b- defN 23-Jul-15 11:18 torchrec/types.py
--rw-r--r--  2.0 unx     1153 b- defN 23-Jul-15 11:18 torchrec/datasets/__init__.py
--rw-r--r--  2.0 unx    41469 b- defN 23-Jul-15 11:18 torchrec/datasets/criteo.py
--rw-r--r--  2.0 unx     4548 b- defN 23-Jul-15 11:18 torchrec/datasets/movielens.py
--rw-r--r--  2.0 unx     6539 b- defN 23-Jul-15 11:18 torchrec/datasets/random.py
--rw-r--r--  2.0 unx    10909 b- defN 23-Jul-15 11:18 torchrec/datasets/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/datasets/scripts/__init__.py
--rw-r--r--  2.0 unx     2448 b- defN 23-Jul-15 11:18 torchrec/datasets/scripts/contiguous_preproc_criteo.py
--rw-r--r--  2.0 unx     2847 b- defN 23-Jul-15 11:18 torchrec/datasets/scripts/npy_preproc_criteo.py
--rw-r--r--  2.0 unx     3077 b- defN 23-Jul-15 11:18 torchrec/datasets/scripts/shuffle_preproc_criteo.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/datasets/test_utils/__init__.py
--rw-r--r--  2.0 unx     5308 b- defN 23-Jul-15 11:18 torchrec/datasets/test_utils/criteo_test_utils.py
--rw-r--r--  2.0 unx     1912 b- defN 23-Jul-15 11:18 torchrec/distributed/__init__.py
--rw-r--r--  2.0 unx    37307 b- defN 23-Jul-15 11:18 torchrec/distributed/batched_embedding_kernel.py
--rw-r--r--  2.0 unx     2069 b- defN 23-Jul-15 11:18 torchrec/distributed/collective_utils.py
--rw-r--r--  2.0 unx     4988 b- defN 23-Jul-15 11:18 torchrec/distributed/comm.py
--rw-r--r--  2.0 unx    55918 b- defN 23-Jul-15 11:18 torchrec/distributed/comm_ops.py
--rw-r--r--  2.0 unx    36967 b- defN 23-Jul-15 11:18 torchrec/distributed/dist_data.py
--rw-r--r--  2.0 unx    32295 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding.py
--rw-r--r--  2.0 unx     4947 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding_kernel.py
--rw-r--r--  2.0 unx    29185 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding_lookup.py
--rw-r--r--  2.0 unx    19035 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding_sharding.py
--rw-r--r--  2.0 unx    36853 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding_tower_sharding.py
--rw-r--r--  2.0 unx    15030 b- defN 23-Jul-15 11:18 torchrec/distributed/embedding_types.py
--rw-r--r--  2.0 unx    37214 b- defN 23-Jul-15 11:18 torchrec/distributed/embeddingbag.py
--rw-r--r--  2.0 unx     7373 b- defN 23-Jul-15 11:18 torchrec/distributed/fbgemm_qcomm_codec.py
--rw-r--r--  2.0 unx     6137 b- defN 23-Jul-15 11:18 torchrec/distributed/fp_embeddingbag.py
--rw-r--r--  2.0 unx     5243 b- defN 23-Jul-15 11:18 torchrec/distributed/fused_embedding.py
--rw-r--r--  2.0 unx     5080 b- defN 23-Jul-15 11:18 torchrec/distributed/fused_embeddingbag.py
--rw-r--r--  2.0 unx     2271 b- defN 23-Jul-15 11:18 torchrec/distributed/fused_params.py
--rw-r--r--  2.0 unx     3807 b- defN 23-Jul-15 11:18 torchrec/distributed/grouped_position_weighted.py
--rw-r--r--  2.0 unx    19750 b- defN 23-Jul-15 11:18 torchrec/distributed/model_parallel.py
--rw-r--r--  2.0 unx    20748 b- defN 23-Jul-15 11:18 torchrec/distributed/quant_embedding.py
--rw-r--r--  2.0 unx    15112 b- defN 23-Jul-15 11:18 torchrec/distributed/quant_embedding_kernel.py
--rw-r--r--  2.0 unx    12621 b- defN 23-Jul-15 11:18 torchrec/distributed/quant_embeddingbag.py
--rw-r--r--  2.0 unx    13928 b- defN 23-Jul-15 11:18 torchrec/distributed/quant_state.py
--rw-r--r--  2.0 unx     9261 b- defN 23-Jul-15 11:18 torchrec/distributed/shard.py
--rw-r--r--  2.0 unx    19646 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding_plan.py
--rw-r--r--  2.0 unx    32061 b- defN 23-Jul-15 11:18 torchrec/distributed/train_pipeline.py
--rw-r--r--  2.0 unx    27865 b- defN 23-Jul-15 11:18 torchrec/distributed/types.py
--rw-r--r--  2.0 unx    15470 b- defN 23-Jul-15 11:18 torchrec/distributed/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/distributed/composable/__init__.py
--rw-r--r--  2.0 unx     3207 b- defN 23-Jul-15 11:18 torchrec/distributed/composable/table_batched_embedding_slice.py
--rw-r--r--  2.0 unx     1025 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/__init__.py
--rw-r--r--  2.0 unx     3135 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/constants.py
--rw-r--r--  2.0 unx    11430 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/enumerators.py
--rw-r--r--  2.0 unx    12642 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/partitioners.py
--rw-r--r--  2.0 unx      835 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/perf_models.py
--rw-r--r--  2.0 unx    13530 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/planners.py
--rw-r--r--  2.0 unx    11236 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/proposers.py
--rw-r--r--  2.0 unx    41291 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/shard_estimators.py
--rw-r--r--  2.0 unx    23791 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/stats.py
--rw-r--r--  2.0 unx     9643 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/storage_reservations.py
--rw-r--r--  2.0 unx    14582 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/types.py
--rw-r--r--  2.0 unx     1119 b- defN 23-Jul-15 11:18 torchrec/distributed/planner/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/__init__.py
--rw-r--r--  2.0 unx     2479 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/cw_sequence_sharding.py
--rw-r--r--  2.0 unx    12945 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/cw_sharding.py
--rw-r--r--  2.0 unx     2802 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/dp_sequence_sharding.py
--rw-r--r--  2.0 unx     7681 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/dp_sharding.py
--rw-r--r--  2.0 unx     7640 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/rw_sequence_sharding.py
--rw-r--r--  2.0 unx    17911 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/rw_sharding.py
--rw-r--r--  2.0 unx     3627 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/sequence_sharding.py
--rw-r--r--  2.0 unx     7632 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/tw_sequence_sharding.py
--rw-r--r--  2.0 unx    16097 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/tw_sharding.py
--rw-r--r--  2.0 unx     1284 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/twcw_sharding.py
--rw-r--r--  2.0 unx    19871 b- defN 23-Jul-15 11:18 torchrec/distributed/sharding/twrw_sharding.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/__init__.py
--rw-r--r--  2.0 unx    11237 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/infer_utils.py
--rw-r--r--  2.0 unx     4868 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/multi_process.py
--rw-r--r--  2.0 unx    34091 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/test_model.py
--rw-r--r--  2.0 unx    11197 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/test_model_parallel.py
--rw-r--r--  2.0 unx    25310 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/test_model_parallel_base.py
--rw-r--r--  2.0 unx    15367 b- defN 23-Jul-15 11:18 torchrec/distributed/test_utils/test_sharding.py
--rw-r--r--  2.0 unx      422 b- defN 23-Jul-15 11:18 torchrec/fx/__init__.py
--rw-r--r--  2.0 unx     6451 b- defN 23-Jul-15 11:18 torchrec/fx/tracer.py
--rw-r--r--  2.0 unx     4524 b- defN 23-Jul-15 11:18 torchrec/fx/utils.py
--rw-r--r--  2.0 unx     1223 b- defN 23-Jul-15 11:18 torchrec/inference/__init__.py
--rw-r--r--  2.0 unx     3614 b- defN 23-Jul-15 11:18 torchrec/inference/client.py
--rw-r--r--  2.0 unx     3957 b- defN 23-Jul-15 11:18 torchrec/inference/model_packager.py
--rw-r--r--  2.0 unx     8068 b- defN 23-Jul-15 11:18 torchrec/inference/modules.py
--rw-r--r--  2.0 unx     3797 b- defN 23-Jul-15 11:18 torchrec/inference/state_dict_transform.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/metrics/__init__.py
--rw-r--r--  2.0 unx     4168 b- defN 23-Jul-15 11:18 torchrec/metrics/accuracy.py
--rw-r--r--  2.0 unx    12549 b- defN 23-Jul-15 11:18 torchrec/metrics/auc.py
--rw-r--r--  2.0 unx     3703 b- defN 23-Jul-15 11:18 torchrec/metrics/calibration.py
--rw-r--r--  2.0 unx     3465 b- defN 23-Jul-15 11:18 torchrec/metrics/ctr.py
--rw-r--r--  2.0 unx     3836 b- defN 23-Jul-15 11:18 torchrec/metrics/mae.py
--rw-r--r--  2.0 unx    17990 b- defN 23-Jul-15 11:18 torchrec/metrics/metric_module.py
--rw-r--r--  2.0 unx     6796 b- defN 23-Jul-15 11:18 torchrec/metrics/metrics_config.py
--rw-r--r--  2.0 unx     3731 b- defN 23-Jul-15 11:18 torchrec/metrics/metrics_namespace.py
--rw-r--r--  2.0 unx     3904 b- defN 23-Jul-15 11:18 torchrec/metrics/model_utils.py
--rw-r--r--  2.0 unx     4631 b- defN 23-Jul-15 11:18 torchrec/metrics/mse.py
--rw-r--r--  2.0 unx     5605 b- defN 23-Jul-15 11:18 torchrec/metrics/multiclass_recall.py
--rw-r--r--  2.0 unx     8735 b- defN 23-Jul-15 11:18 torchrec/metrics/ndcg.py
--rw-r--r--  2.0 unx     6811 b- defN 23-Jul-15 11:18 torchrec/metrics/ne.py
--rw-r--r--  2.0 unx    33554 b- defN 23-Jul-15 11:18 torchrec/metrics/rec_metric.py
--rw-r--r--  2.0 unx    10490 b- defN 23-Jul-15 11:18 torchrec/metrics/recall_session.py
--rw-r--r--  2.0 unx     6057 b- defN 23-Jul-15 11:18 torchrec/metrics/throughput.py
--rw-r--r--  2.0 unx    11160 b- defN 23-Jul-15 11:18 torchrec/metrics/tower_qps.py
--rw-r--r--  2.0 unx     2867 b- defN 23-Jul-15 11:18 torchrec/metrics/weighted_avg.py
--rw-r--r--  2.0 unx    16441 b- defN 23-Jul-15 11:18 torchrec/metrics/test_utils/__init__.py
--rw-r--r--  2.0 unx      913 b- defN 23-Jul-15 11:18 torchrec/models/__init__.py
--rw-r--r--  2.0 unx    11410 b- defN 23-Jul-15 11:18 torchrec/models/deepfm.py
--rw-r--r--  2.0 unx    29965 b- defN 23-Jul-15 11:18 torchrec/models/dlrm.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jul-15 11:18 torchrec/models/experimental/__init__.py
--rw-r--r--  2.0 unx     9825 b- defN 23-Jul-15 11:18 torchrec/models/experimental/test_transformerdlrm.py
--rw-r--r--  2.0 unx     7434 b- defN 23-Jul-15 11:18 torchrec/models/experimental/transformerdlrm.py
--rw-r--r--  2.0 unx     1179 b- defN 23-Jul-15 11:18 torchrec/modules/__init__.py
--rw-r--r--  2.0 unx     1456 b- defN 23-Jul-15 11:18 torchrec/modules/activation.py
--rw-r--r--  2.0 unx    14636 b- defN 23-Jul-15 11:18 torchrec/modules/crossnet.py
--rw-r--r--  2.0 unx     8415 b- defN 23-Jul-15 11:18 torchrec/modules/deepfm.py
--rw-r--r--  2.0 unx     6468 b- defN 23-Jul-15 11:18 torchrec/modules/embedding_configs.py
--rw-r--r--  2.0 unx    14021 b- defN 23-Jul-15 11:18 torchrec/modules/embedding_modules.py
--rw-r--r--  2.0 unx     4858 b- defN 23-Jul-15 11:18 torchrec/modules/embedding_tower.py
--rw-r--r--  2.0 unx    12360 b- defN 23-Jul-15 11:18 torchrec/modules/feature_processor.py
--rw-r--r--  2.0 unx     4832 b- defN 23-Jul-15 11:18 torchrec/modules/feature_processor_.py
--rw-r--r--  2.0 unx     4403 b- defN 23-Jul-15 11:18 torchrec/modules/fp_embedding_modules.py
--rw-r--r--  2.0 unx    31545 b- defN 23-Jul-15 11:18 torchrec/modules/fused_embedding_modules.py
--rw-r--r--  2.0 unx    10541 b- defN 23-Jul-15 11:18 torchrec/modules/lazy_extension.py
--rw-r--r--  2.0 unx     6309 b- defN 23-Jul-15 11:18 torchrec/modules/mlp.py
--rw-r--r--  2.0 unx     3897 b- defN 23-Jul-15 11:18 torchrec/modules/utils.py
--rw-r--r--  2.0 unx     1639 b- defN 23-Jul-15 11:18 torchrec/optim/__init__.py
--rw-r--r--  2.0 unx     2012 b- defN 23-Jul-15 11:18 torchrec/optim/apply_optimizer_in_backward.py
--rw-r--r--  2.0 unx     1569 b- defN 23-Jul-15 11:18 torchrec/optim/clipping.py
--rw-r--r--  2.0 unx     1353 b- defN 23-Jul-15 11:18 torchrec/optim/fused.py
--rw-r--r--  2.0 unx    16069 b- defN 23-Jul-15 11:18 torchrec/optim/keyed.py
--rw-r--r--  2.0 unx     4420 b- defN 23-Jul-15 11:18 torchrec/optim/optimizers.py
--rw-r--r--  2.0 unx     7405 b- defN 23-Jul-15 11:18 torchrec/optim/rowwise_adagrad.py
--rw-r--r--  2.0 unx     4865 b- defN 23-Jul-15 11:18 torchrec/optim/warmup.py
--rw-r--r--  2.0 unx      560 b- defN 23-Jul-15 11:18 torchrec/optim/test_utils/__init__.py
--rw-r--r--  2.0 unx     1140 b- defN 23-Jul-15 11:18 torchrec/quant/__init__.py
--rw-r--r--  2.0 unx    26618 b- defN 23-Jul-15 11:18 torchrec/quant/embedding_modules.py
--rw-r--r--  2.0 unx     4292 b- defN 23-Jul-15 11:18 torchrec/quant/utils.py
--rw-r--r--  2.0 unx     1163 b- defN 23-Jul-15 11:18 torchrec/sparse/__init__.py
--rw-r--r--  2.0 unx    56412 b- defN 23-Jul-15 11:18 torchrec/sparse/jagged_tensor.py
--rw-r--r--  2.0 unx     1430 b- defN 23-Jul-15 11:18 torchrec/sparse/test_utils/__init__.py
--rw-r--r--  2.0 unx     5661 b- defN 23-Jul-15 11:18 torchrec/test_utils/__init__.py
--rw-r--r--  2.0 unx     1530 b- defN 23-Jul-15 11:23 torchrec_nightly-2023.7.15.dist-info/LICENSE
--rw-r--r--  2.0 unx     5012 b- defN 23-Jul-15 11:23 torchrec_nightly-2023.7.15.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 23-Jul-15 11:23 torchrec_nightly-2023.7.15.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jul-15 11:23 torchrec_nightly-2023.7.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    13527 b- defN 23-Jul-15 11:23 torchrec_nightly-2023.7.15.dist-info/RECORD
-145 files, 1500994 bytes uncompressed, 342574 bytes compressed:  77.2%
+Zip file size: 369967 bytes, number of entries: 148
+-rw-r--r--  2.0 unx      811 b- defN 23-Jul-17 11:19 torchrec/__init__.py
+-rw-r--r--  2.0 unx     1638 b- defN 23-Jul-17 11:19 torchrec/streamable.py
+-rw-r--r--  2.0 unx      854 b- defN 23-Jul-17 11:19 torchrec/types.py
+-rw-r--r--  2.0 unx     1153 b- defN 23-Jul-17 11:19 torchrec/datasets/__init__.py
+-rw-r--r--  2.0 unx    41469 b- defN 23-Jul-17 11:19 torchrec/datasets/criteo.py
+-rw-r--r--  2.0 unx     4548 b- defN 23-Jul-17 11:19 torchrec/datasets/movielens.py
+-rw-r--r--  2.0 unx     6539 b- defN 23-Jul-17 11:19 torchrec/datasets/random.py
+-rw-r--r--  2.0 unx    10909 b- defN 23-Jul-17 11:19 torchrec/datasets/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/datasets/scripts/__init__.py
+-rw-r--r--  2.0 unx     2448 b- defN 23-Jul-17 11:19 torchrec/datasets/scripts/contiguous_preproc_criteo.py
+-rw-r--r--  2.0 unx     2847 b- defN 23-Jul-17 11:19 torchrec/datasets/scripts/npy_preproc_criteo.py
+-rw-r--r--  2.0 unx     3077 b- defN 23-Jul-17 11:19 torchrec/datasets/scripts/shuffle_preproc_criteo.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/datasets/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5308 b- defN 23-Jul-17 11:19 torchrec/datasets/test_utils/criteo_test_utils.py
+-rw-r--r--  2.0 unx     1912 b- defN 23-Jul-17 11:19 torchrec/distributed/__init__.py
+-rw-r--r--  2.0 unx    37307 b- defN 23-Jul-17 11:19 torchrec/distributed/batched_embedding_kernel.py
+-rw-r--r--  2.0 unx     2069 b- defN 23-Jul-17 11:19 torchrec/distributed/collective_utils.py
+-rw-r--r--  2.0 unx     4988 b- defN 23-Jul-17 11:19 torchrec/distributed/comm.py
+-rw-r--r--  2.0 unx    55918 b- defN 23-Jul-17 11:19 torchrec/distributed/comm_ops.py
+-rw-r--r--  2.0 unx    36967 b- defN 23-Jul-17 11:19 torchrec/distributed/dist_data.py
+-rw-r--r--  2.0 unx    32295 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding.py
+-rw-r--r--  2.0 unx     4947 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding_kernel.py
+-rw-r--r--  2.0 unx    29185 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding_lookup.py
+-rw-r--r--  2.0 unx    19035 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding_sharding.py
+-rw-r--r--  2.0 unx    36853 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding_tower_sharding.py
+-rw-r--r--  2.0 unx    15030 b- defN 23-Jul-17 11:19 torchrec/distributed/embedding_types.py
+-rw-r--r--  2.0 unx    37369 b- defN 23-Jul-17 11:19 torchrec/distributed/embeddingbag.py
+-rw-r--r--  2.0 unx     7373 b- defN 23-Jul-17 11:19 torchrec/distributed/fbgemm_qcomm_codec.py
+-rw-r--r--  2.0 unx     6137 b- defN 23-Jul-17 11:19 torchrec/distributed/fp_embeddingbag.py
+-rw-r--r--  2.0 unx     5243 b- defN 23-Jul-17 11:19 torchrec/distributed/fused_embedding.py
+-rw-r--r--  2.0 unx     5080 b- defN 23-Jul-17 11:19 torchrec/distributed/fused_embeddingbag.py
+-rw-r--r--  2.0 unx     2271 b- defN 23-Jul-17 11:19 torchrec/distributed/fused_params.py
+-rw-r--r--  2.0 unx     3807 b- defN 23-Jul-17 11:19 torchrec/distributed/grouped_position_weighted.py
+-rw-r--r--  2.0 unx    10997 b- defN 23-Jul-17 11:19 torchrec/distributed/mc_embeddingbag.py
+-rw-r--r--  2.0 unx    19750 b- defN 23-Jul-17 11:19 torchrec/distributed/model_parallel.py
+-rw-r--r--  2.0 unx    20748 b- defN 23-Jul-17 11:19 torchrec/distributed/quant_embedding.py
+-rw-r--r--  2.0 unx    15112 b- defN 23-Jul-17 11:19 torchrec/distributed/quant_embedding_kernel.py
+-rw-r--r--  2.0 unx    12621 b- defN 23-Jul-17 11:19 torchrec/distributed/quant_embeddingbag.py
+-rw-r--r--  2.0 unx    13928 b- defN 23-Jul-17 11:19 torchrec/distributed/quant_state.py
+-rw-r--r--  2.0 unx     9261 b- defN 23-Jul-17 11:19 torchrec/distributed/shard.py
+-rw-r--r--  2.0 unx    19646 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding_plan.py
+-rw-r--r--  2.0 unx    32061 b- defN 23-Jul-17 11:19 torchrec/distributed/train_pipeline.py
+-rw-r--r--  2.0 unx    27865 b- defN 23-Jul-17 11:19 torchrec/distributed/types.py
+-rw-r--r--  2.0 unx    15470 b- defN 23-Jul-17 11:19 torchrec/distributed/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/distributed/composable/__init__.py
+-rw-r--r--  2.0 unx     3207 b- defN 23-Jul-17 11:19 torchrec/distributed/composable/table_batched_embedding_slice.py
+-rw-r--r--  2.0 unx     1025 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/__init__.py
+-rw-r--r--  2.0 unx     3135 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/constants.py
+-rw-r--r--  2.0 unx    11430 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/enumerators.py
+-rw-r--r--  2.0 unx    12642 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/partitioners.py
+-rw-r--r--  2.0 unx      835 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/perf_models.py
+-rw-r--r--  2.0 unx    13530 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/planners.py
+-rw-r--r--  2.0 unx    11236 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/proposers.py
+-rw-r--r--  2.0 unx    41291 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/shard_estimators.py
+-rw-r--r--  2.0 unx    23791 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/stats.py
+-rw-r--r--  2.0 unx     9643 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/storage_reservations.py
+-rw-r--r--  2.0 unx    14582 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/types.py
+-rw-r--r--  2.0 unx     1119 b- defN 23-Jul-17 11:19 torchrec/distributed/planner/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/__init__.py
+-rw-r--r--  2.0 unx     2479 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/cw_sequence_sharding.py
+-rw-r--r--  2.0 unx    12945 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/cw_sharding.py
+-rw-r--r--  2.0 unx     2802 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/dp_sequence_sharding.py
+-rw-r--r--  2.0 unx     7681 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/dp_sharding.py
+-rw-r--r--  2.0 unx     7640 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/rw_sequence_sharding.py
+-rw-r--r--  2.0 unx    17911 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/rw_sharding.py
+-rw-r--r--  2.0 unx     3627 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/sequence_sharding.py
+-rw-r--r--  2.0 unx     7632 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/tw_sequence_sharding.py
+-rw-r--r--  2.0 unx    16097 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/tw_sharding.py
+-rw-r--r--  2.0 unx     1284 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/twcw_sharding.py
+-rw-r--r--  2.0 unx    19871 b- defN 23-Jul-17 11:19 torchrec/distributed/sharding/twrw_sharding.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/__init__.py
+-rw-r--r--  2.0 unx    11237 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/infer_utils.py
+-rw-r--r--  2.0 unx     4868 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/multi_process.py
+-rw-r--r--  2.0 unx    34091 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/test_model.py
+-rw-r--r--  2.0 unx    11197 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/test_model_parallel.py
+-rw-r--r--  2.0 unx    25310 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/test_model_parallel_base.py
+-rw-r--r--  2.0 unx    15367 b- defN 23-Jul-17 11:19 torchrec/distributed/test_utils/test_sharding.py
+-rw-r--r--  2.0 unx      422 b- defN 23-Jul-17 11:19 torchrec/fx/__init__.py
+-rw-r--r--  2.0 unx     6451 b- defN 23-Jul-17 11:19 torchrec/fx/tracer.py
+-rw-r--r--  2.0 unx     4524 b- defN 23-Jul-17 11:19 torchrec/fx/utils.py
+-rw-r--r--  2.0 unx     1223 b- defN 23-Jul-17 11:19 torchrec/inference/__init__.py
+-rw-r--r--  2.0 unx     3614 b- defN 23-Jul-17 11:19 torchrec/inference/client.py
+-rw-r--r--  2.0 unx     3957 b- defN 23-Jul-17 11:19 torchrec/inference/model_packager.py
+-rw-r--r--  2.0 unx     8068 b- defN 23-Jul-17 11:19 torchrec/inference/modules.py
+-rw-r--r--  2.0 unx     3797 b- defN 23-Jul-17 11:19 torchrec/inference/state_dict_transform.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/metrics/__init__.py
+-rw-r--r--  2.0 unx     4168 b- defN 23-Jul-17 11:19 torchrec/metrics/accuracy.py
+-rw-r--r--  2.0 unx    12549 b- defN 23-Jul-17 11:19 torchrec/metrics/auc.py
+-rw-r--r--  2.0 unx     3703 b- defN 23-Jul-17 11:19 torchrec/metrics/calibration.py
+-rw-r--r--  2.0 unx     3465 b- defN 23-Jul-17 11:19 torchrec/metrics/ctr.py
+-rw-r--r--  2.0 unx     3836 b- defN 23-Jul-17 11:19 torchrec/metrics/mae.py
+-rw-r--r--  2.0 unx    17990 b- defN 23-Jul-17 11:19 torchrec/metrics/metric_module.py
+-rw-r--r--  2.0 unx     6796 b- defN 23-Jul-17 11:19 torchrec/metrics/metrics_config.py
+-rw-r--r--  2.0 unx     3731 b- defN 23-Jul-17 11:19 torchrec/metrics/metrics_namespace.py
+-rw-r--r--  2.0 unx     3904 b- defN 23-Jul-17 11:19 torchrec/metrics/model_utils.py
+-rw-r--r--  2.0 unx     4631 b- defN 23-Jul-17 11:19 torchrec/metrics/mse.py
+-rw-r--r--  2.0 unx     5605 b- defN 23-Jul-17 11:19 torchrec/metrics/multiclass_recall.py
+-rw-r--r--  2.0 unx     8735 b- defN 23-Jul-17 11:19 torchrec/metrics/ndcg.py
+-rw-r--r--  2.0 unx     6811 b- defN 23-Jul-17 11:19 torchrec/metrics/ne.py
+-rw-r--r--  2.0 unx    33554 b- defN 23-Jul-17 11:19 torchrec/metrics/rec_metric.py
+-rw-r--r--  2.0 unx    10490 b- defN 23-Jul-17 11:19 torchrec/metrics/recall_session.py
+-rw-r--r--  2.0 unx     6057 b- defN 23-Jul-17 11:19 torchrec/metrics/throughput.py
+-rw-r--r--  2.0 unx    11160 b- defN 23-Jul-17 11:19 torchrec/metrics/tower_qps.py
+-rw-r--r--  2.0 unx     2867 b- defN 23-Jul-17 11:19 torchrec/metrics/weighted_avg.py
+-rw-r--r--  2.0 unx    16441 b- defN 23-Jul-17 11:19 torchrec/metrics/test_utils/__init__.py
+-rw-r--r--  2.0 unx      913 b- defN 23-Jul-17 11:19 torchrec/models/__init__.py
+-rw-r--r--  2.0 unx    11410 b- defN 23-Jul-17 11:19 torchrec/models/deepfm.py
+-rw-r--r--  2.0 unx    29965 b- defN 23-Jul-17 11:19 torchrec/models/dlrm.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-17 11:19 torchrec/models/experimental/__init__.py
+-rw-r--r--  2.0 unx     9825 b- defN 23-Jul-17 11:19 torchrec/models/experimental/test_transformerdlrm.py
+-rw-r--r--  2.0 unx     7434 b- defN 23-Jul-17 11:19 torchrec/models/experimental/transformerdlrm.py
+-rw-r--r--  2.0 unx     1179 b- defN 23-Jul-17 11:19 torchrec/modules/__init__.py
+-rw-r--r--  2.0 unx     1456 b- defN 23-Jul-17 11:19 torchrec/modules/activation.py
+-rw-r--r--  2.0 unx    14636 b- defN 23-Jul-17 11:19 torchrec/modules/crossnet.py
+-rw-r--r--  2.0 unx     8415 b- defN 23-Jul-17 11:19 torchrec/modules/deepfm.py
+-rw-r--r--  2.0 unx     6468 b- defN 23-Jul-17 11:19 torchrec/modules/embedding_configs.py
+-rw-r--r--  2.0 unx    14021 b- defN 23-Jul-17 11:19 torchrec/modules/embedding_modules.py
+-rw-r--r--  2.0 unx     4858 b- defN 23-Jul-17 11:19 torchrec/modules/embedding_tower.py
+-rw-r--r--  2.0 unx    12360 b- defN 23-Jul-17 11:19 torchrec/modules/feature_processor.py
+-rw-r--r--  2.0 unx     4832 b- defN 23-Jul-17 11:19 torchrec/modules/feature_processor_.py
+-rw-r--r--  2.0 unx     4403 b- defN 23-Jul-17 11:19 torchrec/modules/fp_embedding_modules.py
+-rw-r--r--  2.0 unx    31545 b- defN 23-Jul-17 11:19 torchrec/modules/fused_embedding_modules.py
+-rw-r--r--  2.0 unx    10541 b- defN 23-Jul-17 11:19 torchrec/modules/lazy_extension.py
+-rw-r--r--  2.0 unx     3143 b- defN 23-Jul-17 11:19 torchrec/modules/managed_collision_modules.py
+-rw-r--r--  2.0 unx     5124 b- defN 23-Jul-17 11:19 torchrec/modules/mc_embedding_modules.py
+-rw-r--r--  2.0 unx     6309 b- defN 23-Jul-17 11:19 torchrec/modules/mlp.py
+-rw-r--r--  2.0 unx     3897 b- defN 23-Jul-17 11:19 torchrec/modules/utils.py
+-rw-r--r--  2.0 unx     1639 b- defN 23-Jul-17 11:19 torchrec/optim/__init__.py
+-rw-r--r--  2.0 unx     2012 b- defN 23-Jul-17 11:19 torchrec/optim/apply_optimizer_in_backward.py
+-rw-r--r--  2.0 unx     1569 b- defN 23-Jul-17 11:19 torchrec/optim/clipping.py
+-rw-r--r--  2.0 unx     1353 b- defN 23-Jul-17 11:19 torchrec/optim/fused.py
+-rw-r--r--  2.0 unx    16069 b- defN 23-Jul-17 11:19 torchrec/optim/keyed.py
+-rw-r--r--  2.0 unx     4420 b- defN 23-Jul-17 11:19 torchrec/optim/optimizers.py
+-rw-r--r--  2.0 unx     7405 b- defN 23-Jul-17 11:19 torchrec/optim/rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4865 b- defN 23-Jul-17 11:19 torchrec/optim/warmup.py
+-rw-r--r--  2.0 unx      560 b- defN 23-Jul-17 11:19 torchrec/optim/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1140 b- defN 23-Jul-17 11:19 torchrec/quant/__init__.py
+-rw-r--r--  2.0 unx    26618 b- defN 23-Jul-17 11:19 torchrec/quant/embedding_modules.py
+-rw-r--r--  2.0 unx     4292 b- defN 23-Jul-17 11:19 torchrec/quant/utils.py
+-rw-r--r--  2.0 unx     1163 b- defN 23-Jul-17 11:19 torchrec/sparse/__init__.py
+-rw-r--r--  2.0 unx    56412 b- defN 23-Jul-17 11:19 torchrec/sparse/jagged_tensor.py
+-rw-r--r--  2.0 unx     1430 b- defN 23-Jul-17 11:19 torchrec/sparse/test_utils/__init__.py
+-rw-r--r--  2.0 unx     5661 b- defN 23-Jul-17 11:19 torchrec/test_utils/__init__.py
+-rw-r--r--  2.0 unx     1530 b- defN 23-Jul-17 11:24 torchrec_nightly-2023.7.17.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5012 b- defN 23-Jul-17 11:24 torchrec_nightly-2023.7.17.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 23-Jul-17 11:24 torchrec_nightly-2023.7.17.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jul-17 11:24 torchrec_nightly-2023.7.17.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    13823 b- defN 23-Jul-17 11:24 torchrec_nightly-2023.7.17.dist-info/RECORD
+148 files, 1520709 bytes uncompressed, 347857 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -93,14 +93,17 @@
 
 Filename: torchrec/distributed/fused_params.py
 Comment: 
 
 Filename: torchrec/distributed/grouped_position_weighted.py
 Comment: 
 
+Filename: torchrec/distributed/mc_embeddingbag.py
+Comment: 
+
 Filename: torchrec/distributed/model_parallel.py
 Comment: 
 
 Filename: torchrec/distributed/quant_embedding.py
 Comment: 
 
 Filename: torchrec/distributed/quant_embedding_kernel.py
@@ -360,14 +363,20 @@
 
 Filename: torchrec/modules/fused_embedding_modules.py
 Comment: 
 
 Filename: torchrec/modules/lazy_extension.py
 Comment: 
 
+Filename: torchrec/modules/managed_collision_modules.py
+Comment: 
+
+Filename: torchrec/modules/mc_embedding_modules.py
+Comment: 
+
 Filename: torchrec/modules/mlp.py
 Comment: 
 
 Filename: torchrec/modules/utils.py
 Comment: 
 
 Filename: torchrec/optim/__init__.py
@@ -414,23 +423,23 @@
 
 Filename: torchrec/sparse/test_utils/__init__.py
 Comment: 
 
 Filename: torchrec/test_utils/__init__.py
 Comment: 
 
-Filename: torchrec_nightly-2023.7.15.dist-info/LICENSE
+Filename: torchrec_nightly-2023.7.17.dist-info/LICENSE
 Comment: 
 
-Filename: torchrec_nightly-2023.7.15.dist-info/METADATA
+Filename: torchrec_nightly-2023.7.17.dist-info/METADATA
 Comment: 
 
-Filename: torchrec_nightly-2023.7.15.dist-info/WHEEL
+Filename: torchrec_nightly-2023.7.17.dist-info/WHEEL
 Comment: 
 
-Filename: torchrec_nightly-2023.7.15.dist-info/top_level.txt
+Filename: torchrec_nightly-2023.7.17.dist-info/top_level.txt
 Comment: 
 
-Filename: torchrec_nightly-2023.7.15.dist-info/RECORD
+Filename: torchrec_nightly-2023.7.17.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchrec/distributed/embeddingbag.py

```diff
@@ -352,14 +352,18 @@
         self._embedding_bag_configs: List[
             EmbeddingBagConfig
         ] = module.embedding_bag_configs()
         self._table_names: List[str] = [
             config.name for config in self._embedding_bag_configs
         ]
 
+        self._table_name_to_config: Dict[str, EmbeddingBagConfig] = {
+            config.name: config for config in self._embedding_bag_configs
+        }
+
         self.module_sharding_plan: EmbeddingModuleShardingPlan = cast(
             EmbeddingModuleShardingPlan,
             {
                 table_name: parameter_sharding
                 for table_name, parameter_sharding in table_name_to_parameter_sharding.items()
                 if table_name in self._table_names
             },
```

## Comparing `torchrec_nightly-2023.7.15.dist-info/LICENSE` & `torchrec_nightly-2023.7.17.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torchrec_nightly-2023.7.15.dist-info/METADATA` & `torchrec_nightly-2023.7.17.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchrec-nightly
-Version: 2023.7.15
+Version: 2023.7.17
 Summary: Pytorch domain library for recommendation systems
 Home-page: https://github.com/pytorch/torchrec
 Author: TorchRec Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: pytorch,recommendation systems,sharding
 Classifier: Development Status :: 4 - Beta
```

## Comparing `torchrec_nightly-2023.7.15.dist-info/RECORD` & `torchrec_nightly-2023.7.17.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -20,21 +20,22 @@
 torchrec/distributed/dist_data.py,sha256=mpmO_oiZKCebKbYkXHu9CGwSHWLo-5w4cDj-tYvQ6kU,36967
 torchrec/distributed/embedding.py,sha256=ctrHHtWFq5ITPOucAbO2UQ2cRdeDPKRFyHd04lhYmPo,32295
 torchrec/distributed/embedding_kernel.py,sha256=9OA5PDofQZ-ZRORNR4Ca1pJoEZk5Oj2gE6axYwcXIds,4947
 torchrec/distributed/embedding_lookup.py,sha256=-rExTGufuH2qcRzeR2FSSdB9TfqsnVXdz-lghXceVZs,29185
 torchrec/distributed/embedding_sharding.py,sha256=X088TGuzLb3ou2LQWokn3MNYvo3bNpZT5RzdT1bz9JI,19035
 torchrec/distributed/embedding_tower_sharding.py,sha256=eDHPHzjCstJJRJlE-n8a9lC54lCDsi1iAt4SmkLfza0,36853
 torchrec/distributed/embedding_types.py,sha256=QbDVqeT2wb1RpnGZxrFtFdHYDsOHKW7SH8fLWmN_d0E,15030
-torchrec/distributed/embeddingbag.py,sha256=ddy1uo1Sg2TWISw03bvlp_kaHHvpqkztUm-8pegEq2c,37214
+torchrec/distributed/embeddingbag.py,sha256=3r_m4bnmyNWPI82_QDZ6vuZVuXnn8siPTDdMmhpX68o,37369
 torchrec/distributed/fbgemm_qcomm_codec.py,sha256=StYltKC6Eq6SE_YiX6GsVW3ZF0VyqTcGHXuCYmPAFlU,7373
 torchrec/distributed/fp_embeddingbag.py,sha256=sC7ZIECzJtwn5LNRrUzf0OH7phI3kQHqQ6wBPaGGvPQ,6137
 torchrec/distributed/fused_embedding.py,sha256=1VJeW5Dl7EFMvyOfhBvDKZlp39GYucBo8vNFJY2alFI,5243
 torchrec/distributed/fused_embeddingbag.py,sha256=tG_BrUlCdsek87jgHPKbxg3-z13sAgSWPNRBArf2_ss,5080
 torchrec/distributed/fused_params.py,sha256=YEbH5KUphcSWkwLi-JzXUR9SRDm2OykFxP46CJj6nTM,2271
 torchrec/distributed/grouped_position_weighted.py,sha256=q-QE0U306BiPkXIAlJGIQ80EUDZj-FXTbWwjz3EyvLI,3807
+torchrec/distributed/mc_embeddingbag.py,sha256=3_cm7HF53Lj12DJ271yfN1cbjbdxxYRpBCQUWySNsWc,10997
 torchrec/distributed/model_parallel.py,sha256=VV9Vsyas0VKNHr8sX9pq1iT_xJ2b9xjenY3pYAY5HYw,19750
 torchrec/distributed/quant_embedding.py,sha256=9hTS4oUYkoCEHInYO7r0IQjfAJi4fsw5WNiTOHGUJuM,20748
 torchrec/distributed/quant_embedding_kernel.py,sha256=VsROr4bXBkYysS0H7NnlZzF7IvGgZFtgws5jsnPf6g4,15112
 torchrec/distributed/quant_embeddingbag.py,sha256=SJPY-nL95LKozfT8iR4SHt1BNLx4OcoAfFvqKzy1Gf4,12621
 torchrec/distributed/quant_state.py,sha256=PDQ7qUwhFt-q1WvTkoSbWE3rotiFOYyKNFsQ5vJQ36U,13928
 torchrec/distributed/shard.py,sha256=4Dr5ixWCoMEFEuL5WN4fL2gIdl9wmSUjZWsiF-kdCdQ,9261
 torchrec/distributed/sharding_plan.py,sha256=DftThfyzPvfFzg7SvqsNo7X5n-1rxWhp1RlcQCcpq2o,19646
@@ -116,14 +117,16 @@
 torchrec/modules/embedding_modules.py,sha256=ezRcQ2BqgEEdDF-86Aeribm44YHtaA21NrgOvfr_KYM,14021
 torchrec/modules/embedding_tower.py,sha256=rHiMEUUMoMZUxIPKBE2HyI7I5uNthGQsZIxH038TmoI,4858
 torchrec/modules/feature_processor.py,sha256=UqDELZQ7cRpAQb_6LyxwVByJDdM5NPDfAyEk4qYQmKM,12360
 torchrec/modules/feature_processor_.py,sha256=y6OSfvgmNSvhe00Xwy69Yqu5mwkF24nO2I4G5iu_ONc,4832
 torchrec/modules/fp_embedding_modules.py,sha256=AdUxhEODvE-h0FbqQoD0o-haLBgMRhXl2O0gvcstxI0,4403
 torchrec/modules/fused_embedding_modules.py,sha256=4nyD7aJYasPXqQElg8u3Wmh1n_t-BSe3rd2qxN4WO-k,31545
 torchrec/modules/lazy_extension.py,sha256=bulbZhpIB5QMDy4I7SlE3lLNO0lovKxj5BmqRWfVMpA,10541
+torchrec/modules/managed_collision_modules.py,sha256=Au4LOxNEanXBtbOzlEi-xOnHKlj7NccZB9y7sHELRRM,3143
+torchrec/modules/mc_embedding_modules.py,sha256=z7l0cXKE9uy4GeDYsDCsdfJcPWJK5C4KMTRTUeLW37o,5124
 torchrec/modules/mlp.py,sha256=lV3vCEmNLI1kDtF4eGlCaGvtG3FQ8UEMs4Hcc6Nf3pM,6309
 torchrec/modules/utils.py,sha256=4xCBc_dTQ8CFNLdGtJcCa3Ei0zScfkZCSmnSxOq51vk,3897
 torchrec/optim/__init__.py,sha256=4-nuv6JsmuWBtzyUvCKJ0b9-m7oFi8QB2b3krFF0KgQ,1639
 torchrec/optim/apply_optimizer_in_backward.py,sha256=0wjamGai9i0rXvIf4GNYNhCz7NtkH_9expuepk1qcbI,2012
 torchrec/optim/clipping.py,sha256=sDotlb8Sf4D7-lbBxhzRDFHoiO_DVx34F1J8vOEWq8I,1569
 torchrec/optim/fused.py,sha256=J4u2PWaHD65PIEdg0wTWoK_riZCoSKAVKYPGuZtfKLY,1353
 torchrec/optim/keyed.py,sha256=5QASHSkw2oYwu3OVHU5JJ2mm5tQaSCOQ3z_vBVRLPtk,16069
@@ -134,12 +137,12 @@
 torchrec/quant/__init__.py,sha256=A6NIA6ztq6iP1JTLRLNzlgnCcd-LaN8efnxGub3Ii4A,1140
 torchrec/quant/embedding_modules.py,sha256=-_5_HaoNpt3AmL7fapO2Wj2r6WPjbq2VvATNmGhrai0,26618
 torchrec/quant/utils.py,sha256=rcyo5LDcLK49VLs6ZFxOHeutblWZunDAM_T-0NsraDE,4292
 torchrec/sparse/__init__.py,sha256=dLqSye4Jo6obnNNTUKdPDxPQb9sL2U4weemSn-DjpYk,1163
 torchrec/sparse/jagged_tensor.py,sha256=__iBD2tBQE9ZZpxcOn8RVmDF9gognnyUlmMjedHxJ4E,56412
 torchrec/sparse/test_utils/__init__.py,sha256=BLxfGKJvwjjCiQM64O5wGAA_Cea0sG-buw9lTDWuqug,1430
 torchrec/test_utils/__init__.py,sha256=JncJcXS4N3gI7-fsizQ2-qiWM6MhIrpvskF_9gDf0Go,5661
-torchrec_nightly-2023.7.15.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
-torchrec_nightly-2023.7.15.dist-info/METADATA,sha256=vGshEgrBFSyBpfcXHJUESHjfpjRFoQZVS2XZ1scaRXk,5012
-torchrec_nightly-2023.7.15.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
-torchrec_nightly-2023.7.15.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
-torchrec_nightly-2023.7.15.dist-info/RECORD,,
+torchrec_nightly-2023.7.17.dist-info/LICENSE,sha256=e0Eotbf_rHOYPuEUlppIbvwy4SN98CZnl_hqwvbDA4Q,1530
+torchrec_nightly-2023.7.17.dist-info/METADATA,sha256=Qf8CBt6ds4gZyzV54EiF4CJ8OX5k4hVYWELWPal4gLE,5012
+torchrec_nightly-2023.7.17.dist-info/WHEEL,sha256=ns_9KNZvwSNZtRgVV_clzMUG_fXjGc5Z8Tx4hxQ0gkw,93
+torchrec_nightly-2023.7.17.dist-info/top_level.txt,sha256=LoLcTAPLj_7x62AuyYmhEVBcx2WJ1Z1Nrknv0Jnk_gQ,9
+torchrec_nightly-2023.7.17.dist-info/RECORD,,
```

