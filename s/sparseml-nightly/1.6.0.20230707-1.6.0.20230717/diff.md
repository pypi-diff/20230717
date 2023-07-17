# Comparing `tmp/sparseml_nightly-1.6.0.20230707-py3-none-any.whl.zip` & `tmp/sparseml_nightly-1.6.0.20230717-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,377 +1,378 @@
-Zip file size: 966301 bytes, number of entries: 375
--rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-07 21:17 sparseml/__init__.py
--rw-rw-r--  2.0 unx      898 b- defN 23-Jul-07 21:17 sparseml/analytics.py
--rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-07 21:17 sparseml/base.py
--rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-07 21:17 sparseml/log.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-07 21:17 sparseml/version.py
--rw-rw-r--  2.0 unx      758 b- defN 23-Jul-07 21:17 sparseml/benchmark/__init__.py
--rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-07 21:17 sparseml/benchmark/info.py
--rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-07 21:17 sparseml/benchmark/serialization.py
--rw-rw-r--  2.0 unx      863 b- defN 23-Jul-07 21:17 sparseml/deepsparse/__init__.py
--rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-07 21:17 sparseml/deepsparse/base.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-07 21:17 sparseml/deepsparse/framework/__init__.py
--rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-07 21:17 sparseml/deepsparse/framework/info.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-07 21:17 sparseml/deepsparse/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-07 21:17 sparseml/deepsparse/sparsification/info.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/exporters/__init__.py
--rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-07 21:17 sparseml/exporters/base_exporter.py
--rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-07 21:17 sparseml/exporters/kv_cache_injector.py
--rw-rw-r--  2.0 unx     4783 b- defN 23-Jul-07 21:17 sparseml/exporters/onnx_to_deepsparse.py
--rw-rw-r--  2.0 unx     2276 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/__init__.py
--rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/base_transform.py
--rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/constants_to_initializers.py
--rw-rw-r--  2.0 unx     3866 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/conv_to_qlinearconv.py
--rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/delete_repeated_qdq.py
--rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
--rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/flatten_qparams.py
--rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_conv_div_bn.py
--rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_identity_initializers.py
--rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/fold_relu_quants.py
--rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/initializers_to_uint8.py
--rw-rw-r--  2.0 unx     4866 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
--rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
--rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
--rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/onnx_transform.py
--rw-rw-r--  2.0 unx     3398 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/propagate_embedding_quantization.py
--rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/quantize_qat_embedding.py
--rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/quantize_residuals.py
--rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
--rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
--rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/skip_input_quantize.py
--rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/unwrap_batchnorms.py
--rw-rw-r--  2.0 unx      909 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/__init__.py
--rw-rw-r--  2.0 unx    26599 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
--rw-rw-r--  2.0 unx     6192 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/configs.py
--rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
--rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
--rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
--rw-rw-r--  2.0 unx      730 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/__init__.py
--rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
--rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/helpers.py
--rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-07 21:17 sparseml/exporters/transforms/utils/matching.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-07 21:17 sparseml/framework/__init__.py
--rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-07 21:17 sparseml/framework/info.py
--rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-07 21:17 sparseml/keras/__init__.py
--rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-07 21:17 sparseml/keras/base.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/__init__.py
--rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/dataset.py
--rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/helpers.py
--rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/registry.py
--rw-rw-r--  2.0 unx      786 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-07 21:17 sparseml/keras/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      793 b- defN 23-Jul-07 21:17 sparseml/keras/framework/__init__.py
--rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-07 21:17 sparseml/keras/framework/info.py
--rw-rw-r--  2.0 unx      921 b- defN 23-Jul-07 21:17 sparseml/keras/models/__init__.py
--rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-07 21:17 sparseml/keras/models/registry.py
--rw-rw-r--  2.0 unx      656 b- defN 23-Jul-07 21:17 sparseml/keras/models/classification/__init__.py
--rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-07 21:17 sparseml/keras/models/classification/resnet.py
--rw-rw-r--  2.0 unx      768 b- defN 23-Jul-07 21:17 sparseml/keras/models/external/__init__.py
--rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-07 21:17 sparseml/keras/models/external/keras_applications.py
--rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-07 21:17 sparseml/keras/optim/__init__.py
--rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-07 21:17 sparseml/keras/optim/manager.py
--rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-07 21:17 sparseml/keras/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-07 21:17 sparseml/keras/optim/mask_pruning_creator.py
--rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier.py
--rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_params.py
--rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-07 21:17 sparseml/keras/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-07 21:17 sparseml/keras/optim/utils.py
--rw-rw-r--  2.0 unx      808 b- defN 23-Jul-07 21:17 sparseml/keras/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-07 21:17 sparseml/keras/sparsification/info.py
--rw-rw-r--  2.0 unx      962 b- defN 23-Jul-07 21:17 sparseml/keras/utils/__init__.py
--rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-07 21:17 sparseml/keras/utils/callbacks.py
--rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-07 21:17 sparseml/keras/utils/compat.py
--rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-07 21:17 sparseml/keras/utils/exporter.py
--rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-07 21:17 sparseml/keras/utils/logger.py
--rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-07 21:17 sparseml/keras/utils/model.py
--rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-07 21:17 sparseml/onnx/__init__.py
--rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-07 21:17 sparseml/onnx/base.py
--rw-rw-r--  2.0 unx      743 b- defN 23-Jul-07 21:17 sparseml/onnx/benchmark/__init__.py
--rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-07 21:17 sparseml/onnx/benchmark/info.py
--rw-rw-r--  2.0 unx      823 b- defN 23-Jul-07 21:17 sparseml/onnx/framework/__init__.py
--rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-07 21:17 sparseml/onnx/framework/info.py
--rw-rw-r--  2.0 unx      820 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/__init__.py
--rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/analyzer_model.py
--rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/structured_pruning.py
--rw-rw-r--  2.0 unx      815 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/calibration.py
--rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/quantize.py
--rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-07 21:17 sparseml/onnx/optim/quantization/quantize_model_post_training.py
--rw-rw-r--  2.0 unx      869 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/__init__.py
--rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/info.py
--rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-07 21:17 sparseml/onnx/sparsification/model_info.py
--rw-rw-r--  2.0 unx      867 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/__init__.py
--rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/data.py
--rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/graph_editor.py
--rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/graph_optimizer.py
--rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/helpers.py
--rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/loss.py
--rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/model.py
--rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-07 21:17 sparseml/onnx/utils/sparse_tensor.py
--rw-rw-r--  2.0 unx      931 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/__init__.py
--rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/export.py
--rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/train.py
--rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-07 21:17 sparseml/openpifpaf/trainer.py
--rw-rw-r--  2.0 unx      882 b- defN 23-Jul-07 21:17 sparseml/optim/__init__.py
--rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-07 21:17 sparseml/optim/analyzer.py
--rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-07 21:17 sparseml/optim/helpers.py
--rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-07 21:17 sparseml/optim/manager.py
--rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-07 21:17 sparseml/optim/modifier.py
--rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-07 21:17 sparseml/optim/sensitivity.py
--rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-07 21:17 sparseml/pytorch/__init__.py
--rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-07 21:17 sparseml/pytorch/base.py
--rw-rw-r--  2.0 unx      933 b- defN 23-Jul-07 21:17 sparseml/pytorch/opset.py
--rw-rw-r--  2.0 unx    10884 b- defN 23-Jul-07 21:17 sparseml/pytorch/torch_to_onnx_exporter.py
--rw-rw-r--  2.0 unx      998 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/__init__.py
--rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/generic.py
--rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/registry.py
--rw-rw-r--  2.0 unx      828 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx     4017 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/classification/mnist.py
--rw-rw-r--  2.0 unx      767 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/__init__.py
--rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/coco.py
--rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/helpers.py
--rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/detection/voc.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/image_classification/__init__.py
--rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
--rw-rw-r--  2.0 unx      684 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/recommendation/__init__.py
--rw-rw-r--  2.0 unx      693 b- defN 23-Jul-07 21:17 sparseml/pytorch/datasets/video/__init__.py
--rw-rw-r--  2.0 unx      814 b- defN 23-Jul-07 21:17 sparseml/pytorch/framework/__init__.py
--rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-07 21:17 sparseml/pytorch/framework/info.py
--rw-rw-r--  2.0 unx      753 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/__init__.py
--rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/export.py
--rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/lr_analysis.py
--rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/pr_sensitivity.py
--rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/train.py
--rw-rw-r--  2.0 unx      682 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/__init__.py
--rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/cli_helpers.py
--rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/constants.py
--rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/helpers.py
--rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-07 21:17 sparseml/pytorch/image_classification/utils/trainer.py
--rw-rw-r--  2.0 unx      976 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/__init__.py
--rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/registry.py
--rw-rw-r--  2.0 unx      901 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/__init__.py
--rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/darknet.py
--rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/efficientnet.py
--rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/inception_v3.py
--rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mnist.py
--rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/resnet.py
--rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/classification/vgg.py
--rw-rw-r--  2.0 unx      824 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/__init__.py
--rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd.py
--rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_lite.py
--rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_mobilenet.py
--rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/ssd_resnet.py
--rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/detection/yolo_v3.py
--rw-rw-r--  2.0 unx      763 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/external/__init__.py
--rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/external/torchvision.py
--rw-rw-r--  2.0 unx      676 b- defN 23-Jul-07 21:17 sparseml/pytorch/models/recommendation/__init__.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/__init__.py
--rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/activations.py
--rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/fatrelu.py
--rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/identity.py
--rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-07 21:17 sparseml/pytorch/nn/se.py
--rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/__init__.py
--rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_as.py
--rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/analyzer_pruning.py
--rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/manager.py
--rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/mask_pruning_scorer.py
--rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/optimizer.py
--rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_as.py
--rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_lr.py
--rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-07 21:17 sparseml/pytorch/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      633 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/cli.py
--rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/description.py
--rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-07 21:17 sparseml/pytorch/recipe_template/main.py
--rw-rw-r--  2.0 unx      992 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/info.py
--rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/modifier.py
--rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/modifier_thinning.py
--rw-rw-r--  2.0 unx      705 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/__init__.py
--rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
--rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
--rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
--rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/__init__.py
--rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/mask_creator.py
--rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/mask_params.py
--rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_as.py
--rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
--rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
--rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
--rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
--rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
--rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
--rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
--rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
--rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
--rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/pruning/scorer.py
--rw-rw-r--  2.0 unx      813 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/__init__.py
--rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/constants.py
--rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/helpers.py
--rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
--rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
--rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
--rw-rw-r--  2.0 unx    17905 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantize.py
--rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
--rw-rw-r--  2.0 unx      790 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/__init__.py
--rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_epoch.py
--rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_logging.py
--rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_lr.py
--rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_params.py
--rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-07 21:17 sparseml/pytorch/sparsification/training/modifier_regularizer.py
--rw-rw-r--  2.0 unx      943 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/__init__.py
--rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/export_onnx.py
--rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/presets.py
--rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/sampler.py
--rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/train.py
--rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/transforms.py
--rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-07 21:17 sparseml/pytorch/torchvision/utils.py
--rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/__init__.py
--rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/benchmarker.py
--rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/callbacks.py
--rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/distributed.py
--rw-rw-r--  2.0 unx    31098 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/exporter.py
--rw-rw-r--  2.0 unx    39284 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/helpers.py
--rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/log_sparsification_info.py
--rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/logger.py
--rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/loss.py
--rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/model.py
--rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/module.py
--rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification.py
--rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/ssd_helpers.py
--rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/yolo_helpers.py
--rw-rw-r--  2.0 unx      617 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/__init__.py
--rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/configs.py
--rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/helpers.py
--rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-07 21:17 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
--rw-rw-r--  2.0 unx      655 b- defN 23-Jul-07 21:17 sparseml/recipe_template/__init__.py
--rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-07 21:17 sparseml/recipe_template/utils.py
--rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-07 21:17 sparseml/sparsification/__init__.py
--rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-07 21:17 sparseml/sparsification/analyzer.py
--rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-07 21:17 sparseml/sparsification/info.py
--rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-07 21:17 sparseml/sparsification/model_info.py
--rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_epoch.py
--rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_lr.py
--rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_params.py
--rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-07 21:17 sparseml/sparsification/modifier_pruning.py
--rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-07 21:17 sparseml/sparsification/oracle.py
--rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-07 21:17 sparseml/sparsification/recipe_builder.py
--rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-07 21:17 sparseml/sparsification/recipe_editor.py
--rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-07 21:17 sparseml/sparsification/types.py
--rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/__init__.py
--rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/base.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/__init__.py
--rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/dataset.py
--rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/helpers.py
--rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/registry.py
--rw-rw-r--  2.0 unx      807 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/__init__.py
--rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/cifar.py
--rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
--rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagenet.py
--rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/datasets/classification/imagenette.py
--rw-rw-r--  2.0 unx      805 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/framework/__init__.py
--rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/framework/info.py
--rw-rw-r--  2.0 unx      925 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/__init__.py
--rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/estimator.py
--rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/registry.py
--rw-rw-r--  2.0 unx      822 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/__init__.py
--rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mnist.py
--rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mobilenet.py
--rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
--rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/resnet.py
--rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/models/classification/vgg.py
--rw-rw-r--  2.0 unx      865 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/nn/__init__.py
--rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/nn/layers.py
--rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/__init__.py
--rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/analyzer_module.py
--rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/manager.py
--rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
--rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/mask_pruning.py
--rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier.py
--rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_epoch.py
--rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_lr.py
--rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_params.py
--rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/modifier_pruning.py
--rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/schedule_lr.py
--rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
--rw-rw-r--  2.0 unx      801 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/sparsification/__init__.py
--rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/sparsification/info.py
--rw-rw-r--  2.0 unx      967 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/__init__.py
--rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/exporter.py
--rw-rw-r--  2.0 unx      996 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/helpers.py
--rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/loss.py
--rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/nets_utils.py
--rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/summary.py
--rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-07 21:17 sparseml/tensorflow_v1/utils/variable.py
--rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-07 21:17 sparseml/transformers/__init__.py
--rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-07 21:17 sparseml/transformers/export.py
--rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-07 21:17 sparseml/transformers/masked_language_modeling.py
--rw-rw-r--  2.0 unx    36557 b- defN 23-Jul-07 21:17 sparseml/transformers/question_answering.py
--rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-07 21:17 sparseml/transformers/text_classification.py
--rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-07 21:17 sparseml/transformers/token_classification.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/__init__.py
--rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/question_answering.py
--rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/trainer.py
--rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-07 21:17 sparseml/transformers/sparsification/training_args.py
--rw-rw-r--  2.0 unx      794 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/__init__.py
--rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/helpers.py
--rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/metrics.py
--rw-rw-r--  2.0 unx    17072 b- defN 23-Jul-07 21:17 sparseml/transformers/utils/model.py
--rw-rw-r--  2.0 unx      844 b- defN 23-Jul-07 21:17 sparseml/utils/__init__.py
--rw-rw-r--  2.0 unx      886 b- defN 23-Jul-07 21:17 sparseml/utils/frameworks.py
--rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-07 21:17 sparseml/utils/helpers.py
--rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-07 21:17 sparseml/utils/restricted_eval.py
--rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-07 21:17 sparseml/utils/singleton.py
--rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-07 21:17 sparseml/utils/worker.py
--rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-07 21:17 sparseml/utils/wrapper.py
--rw-rw-r--  2.0 unx      819 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/__init__.py
--rw-rw-r--  2.0 unx      833 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/cifar.py
--rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/coco.py
--rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/helpers.py
--rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/imagenet.py
--rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/imagenette.py
--rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-07 21:17 sparseml/utils/datasets/voc.py
--rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-07 21:17 sparseml/yolact/COCO.sh
--rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-07 21:17 sparseml/yolact/COCO_test.sh
--rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-07 21:17 sparseml/yolact/__init__.py
--rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-07 21:17 sparseml/yolact/scripts.py
--rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-07 21:17 sparseml/yolov5/__init__.py
--rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-07 21:17 sparseml/yolov5/helpers.py
--rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-07 21:17 sparseml/yolov5/scripts.py
--rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-07 21:17 sparseml/yolov5/yolov5.status.yaml
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jul-07 21:17 sparseml/yolov8/__init__.py
--rw-rw-r--  2.0 unx     5781 b- defN 23-Jul-07 21:17 sparseml/yolov8/default.yaml
--rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-07 21:17 sparseml/yolov8/export.py
--rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-07 21:17 sparseml/yolov8/modules.py
--rw-rw-r--  2.0 unx     7194 b- defN 23-Jul-07 21:17 sparseml/yolov8/train.py
--rw-rw-r--  2.0 unx    35999 b- defN 23-Jul-07 21:17 sparseml/yolov8/trainers.py
--rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-07 21:17 sparseml/yolov8/val.py
--rw-rw-r--  2.0 unx     8196 b- defN 23-Jul-07 21:17 sparseml/yolov8/validators.py
--rw-rw-r--  2.0 unx      685 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/__init__.py
--rw-rw-r--  2.0 unx     6172 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/export_samples.py
--rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-07 21:17 sparseml/yolov8/utils/helpers.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/LICENSE
--rw-rw-r--  2.0 unx    21782 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/METADATA
--rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/NOTICE
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/WHEEL
--rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx    37382 b- defN 23-Jul-07 21:20 sparseml_nightly-1.6.0.20230707.dist-info/RECORD
-375 files, 3494563 bytes uncompressed, 905753 bytes compressed:  74.1%
+Zip file size: 968624 bytes, number of entries: 376
+-rw-rw-r--  2.0 unx     1413 b- defN 23-Jul-17 15:00 sparseml/__init__.py
+-rw-rw-r--  2.0 unx      898 b- defN 23-Jul-17 15:00 sparseml/analytics.py
+-rw-rw-r--  2.0 unx    10284 b- defN 23-Jul-17 15:00 sparseml/base.py
+-rw-rw-r--  2.0 unx     2483 b- defN 23-Jul-17 15:00 sparseml/log.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-17 15:00 sparseml/version.py
+-rw-rw-r--  2.0 unx      758 b- defN 23-Jul-17 15:00 sparseml/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    17763 b- defN 23-Jul-17 15:00 sparseml/benchmark/info.py
+-rw-rw-r--  2.0 unx    10778 b- defN 23-Jul-17 15:00 sparseml/benchmark/serialization.py
+-rw-rw-r--  2.0 unx      863 b- defN 23-Jul-17 15:00 sparseml/deepsparse/__init__.py
+-rw-rw-r--  2.0 unx     3516 b- defN 23-Jul-17 15:00 sparseml/deepsparse/base.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-17 15:00 sparseml/deepsparse/framework/__init__.py
+-rw-rw-r--  2.0 unx     6032 b- defN 23-Jul-17 15:00 sparseml/deepsparse/framework/info.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-17 15:00 sparseml/deepsparse/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1348 b- defN 23-Jul-17 15:00 sparseml/deepsparse/sparsification/info.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-17 15:00 sparseml/exporters/__init__.py
+-rw-rw-r--  2.0 unx     1477 b- defN 23-Jul-17 15:00 sparseml/exporters/base_exporter.py
+-rw-rw-r--  2.0 unx     6325 b- defN 23-Jul-17 15:00 sparseml/exporters/kv_cache_injector.py
+-rw-rw-r--  2.0 unx     4847 b- defN 23-Jul-17 15:00 sparseml/exporters/onnx_to_deepsparse.py
+-rw-rw-r--  2.0 unx     2350 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/__init__.py
+-rw-rw-r--  2.0 unx     2333 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/base_transform.py
+-rw-rw-r--  2.0 unx     1388 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/constants_to_initializers.py
+-rw-rw-r--  2.0 unx     4630 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     5838 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/conv_to_qlinearconv.py
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/delete_repeated_qdq.py
+-rw-rw-r--  2.0 unx     1842 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/delete_trivial_onnx_adds.py
+-rw-rw-r--  2.0 unx     2181 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/flatten_qparams.py
+-rw-rw-r--  2.0 unx     3553 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/fold_conv_div_bn.py
+-rw-rw-r--  2.0 unx     1669 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/fold_identity_initializers.py
+-rw-rw-r--  2.0 unx     2070 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/fold_relu_quants.py
+-rw-rw-r--  2.0 unx     4418 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     7629 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     1645 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/initializers_to_uint8.py
+-rw-rw-r--  2.0 unx     6297 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py
+-rw-rw-r--  2.0 unx     4681 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py
+-rw-rw-r--  2.0 unx     4156 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
+-rw-rw-r--  2.0 unx     3724 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/onnx_transform.py
+-rw-rw-r--  2.0 unx     3433 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/propagate_dequant_through_split.py
+-rw-rw-r--  2.0 unx     4801 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/propagate_embedding_quantization.py
+-rw-rw-r--  2.0 unx     4464 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/quantize_qat_embedding.py
+-rw-rw-r--  2.0 unx     3869 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/quantize_residuals.py
+-rw-rw-r--  2.0 unx     3331 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py
+-rw-rw-r--  2.0 unx     3210 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/skip_input_quantize.py
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/unwrap_batchnorms.py
+-rw-rw-r--  2.0 unx      909 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/__init__.py
+-rw-rw-r--  2.0 unx    26610 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py
+-rw-rw-r--  2.0 unx     6523 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/configs.py
+-rw-rw-r--  2.0 unx     1660 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py
+-rw-rw-r--  2.0 unx     3377 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py
+-rw-rw-r--  2.0 unx     4951 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py
+-rw-rw-r--  2.0 unx      730 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/utils/__init__.py
+-rw-rw-r--  2.0 unx    10570 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py
+-rw-rw-r--  2.0 unx     6457 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/utils/helpers.py
+-rw-rw-r--  2.0 unx    14429 b- defN 23-Jul-17 15:00 sparseml/exporters/transforms/utils/matching.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-17 15:00 sparseml/framework/__init__.py
+-rw-rw-r--  2.0 unx     9479 b- defN 23-Jul-17 15:00 sparseml/framework/info.py
+-rw-rw-r--  2.0 unx     1144 b- defN 23-Jul-17 15:00 sparseml/keras/__init__.py
+-rw-rw-r--  2.0 unx     8054 b- defN 23-Jul-17 15:00 sparseml/keras/base.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/__init__.py
+-rw-rw-r--  2.0 unx     3297 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/dataset.py
+-rw-rw-r--  2.0 unx     2423 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2761 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/registry.py
+-rw-rw-r--  2.0 unx      786 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     8369 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4301 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     2727 b- defN 23-Jul-17 15:00 sparseml/keras/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      793 b- defN 23-Jul-17 15:00 sparseml/keras/framework/__init__.py
+-rw-rw-r--  2.0 unx     5906 b- defN 23-Jul-17 15:00 sparseml/keras/framework/info.py
+-rw-rw-r--  2.0 unx      921 b- defN 23-Jul-17 15:00 sparseml/keras/models/__init__.py
+-rw-rw-r--  2.0 unx    11814 b- defN 23-Jul-17 15:00 sparseml/keras/models/registry.py
+-rw-rw-r--  2.0 unx      656 b- defN 23-Jul-17 15:00 sparseml/keras/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    17932 b- defN 23-Jul-17 15:00 sparseml/keras/models/classification/resnet.py
+-rw-rw-r--  2.0 unx      768 b- defN 23-Jul-17 15:00 sparseml/keras/models/external/__init__.py
+-rw-rw-r--  2.0 unx     4402 b- defN 23-Jul-17 15:00 sparseml/keras/models/external/keras_applications.py
+-rw-rw-r--  2.0 unx     1166 b- defN 23-Jul-17 15:00 sparseml/keras/optim/__init__.py
+-rw-rw-r--  2.0 unx     5677 b- defN 23-Jul-17 15:00 sparseml/keras/optim/manager.py
+-rw-rw-r--  2.0 unx    14777 b- defN 23-Jul-17 15:00 sparseml/keras/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    19740 b- defN 23-Jul-17 15:00 sparseml/keras/optim/mask_pruning_creator.py
+-rw-rw-r--  2.0 unx     9183 b- defN 23-Jul-17 15:00 sparseml/keras/optim/modifier.py
+-rw-rw-r--  2.0 unx     1676 b- defN 23-Jul-17 15:00 sparseml/keras/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    14736 b- defN 23-Jul-17 15:00 sparseml/keras/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     5477 b- defN 23-Jul-17 15:00 sparseml/keras/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    24031 b- defN 23-Jul-17 15:00 sparseml/keras/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     1133 b- defN 23-Jul-17 15:00 sparseml/keras/optim/utils.py
+-rw-rw-r--  2.0 unx      808 b- defN 23-Jul-17 15:00 sparseml/keras/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1356 b- defN 23-Jul-17 15:00 sparseml/keras/sparsification/info.py
+-rw-rw-r--  2.0 unx      962 b- defN 23-Jul-17 15:00 sparseml/keras/utils/__init__.py
+-rw-rw-r--  2.0 unx     8202 b- defN 23-Jul-17 15:00 sparseml/keras/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-17 15:00 sparseml/keras/utils/compat.py
+-rw-rw-r--  2.0 unx     5737 b- defN 23-Jul-17 15:00 sparseml/keras/utils/exporter.py
+-rw-rw-r--  2.0 unx     6087 b- defN 23-Jul-17 15:00 sparseml/keras/utils/logger.py
+-rw-rw-r--  2.0 unx     1738 b- defN 23-Jul-17 15:00 sparseml/keras/utils/model.py
+-rw-rw-r--  2.0 unx     1036 b- defN 23-Jul-17 15:00 sparseml/onnx/__init__.py
+-rw-rw-r--  2.0 unx     6202 b- defN 23-Jul-17 15:00 sparseml/onnx/base.py
+-rw-rw-r--  2.0 unx      743 b- defN 23-Jul-17 15:00 sparseml/onnx/benchmark/__init__.py
+-rw-rw-r--  2.0 unx    15366 b- defN 23-Jul-17 15:00 sparseml/onnx/benchmark/info.py
+-rw-rw-r--  2.0 unx      823 b- defN 23-Jul-17 15:00 sparseml/onnx/framework/__init__.py
+-rw-rw-r--  2.0 unx     6116 b- defN 23-Jul-17 15:00 sparseml/onnx/framework/info.py
+-rw-rw-r--  2.0 unx      820 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/__init__.py
+-rw-rw-r--  2.0 unx    13285 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/analyzer_model.py
+-rw-rw-r--  2.0 unx    19639 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx     6470 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/structured_pruning.py
+-rw-rw-r--  2.0 unx      815 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/quantization/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/quantization/calibration.py
+-rw-rw-r--  2.0 unx    73551 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/quantization/quantize.py
+-rw-rw-r--  2.0 unx     4552 b- defN 23-Jul-17 15:00 sparseml/onnx/optim/quantization/quantize_model_post_training.py
+-rw-rw-r--  2.0 unx      869 b- defN 23-Jul-17 15:00 sparseml/onnx/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    10209 b- defN 23-Jul-17 15:00 sparseml/onnx/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     1363 b- defN 23-Jul-17 15:00 sparseml/onnx/sparsification/info.py
+-rw-rw-r--  2.0 unx     8009 b- defN 23-Jul-17 15:00 sparseml/onnx/sparsification/model_info.py
+-rw-rw-r--  2.0 unx      867 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/__init__.py
+-rw-rw-r--  2.0 unx    13013 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/data.py
+-rw-rw-r--  2.0 unx    18825 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/graph_editor.py
+-rw-rw-r--  2.0 unx     8133 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/graph_optimizer.py
+-rw-rw-r--  2.0 unx    40230 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/helpers.py
+-rw-rw-r--  2.0 unx     1958 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/loss.py
+-rw-rw-r--  2.0 unx    31591 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/model.py
+-rw-rw-r--  2.0 unx     5437 b- defN 23-Jul-17 15:00 sparseml/onnx/utils/sparse_tensor.py
+-rw-rw-r--  2.0 unx      931 b- defN 23-Jul-17 15:00 sparseml/openpifpaf/__init__.py
+-rw-rw-r--  2.0 unx     3713 b- defN 23-Jul-17 15:00 sparseml/openpifpaf/export.py
+-rw-rw-r--  2.0 unx    10950 b- defN 23-Jul-17 15:00 sparseml/openpifpaf/train.py
+-rw-rw-r--  2.0 unx     4211 b- defN 23-Jul-17 15:00 sparseml/openpifpaf/trainer.py
+-rw-rw-r--  2.0 unx      882 b- defN 23-Jul-17 15:00 sparseml/optim/__init__.py
+-rw-rw-r--  2.0 unx     6302 b- defN 23-Jul-17 15:00 sparseml/optim/analyzer.py
+-rw-rw-r--  2.0 unx    25563 b- defN 23-Jul-17 15:00 sparseml/optim/helpers.py
+-rw-rw-r--  2.0 unx    25984 b- defN 23-Jul-17 15:00 sparseml/optim/manager.py
+-rw-rw-r--  2.0 unx    30708 b- defN 23-Jul-17 15:00 sparseml/optim/modifier.py
+-rw-rw-r--  2.0 unx    26315 b- defN 23-Jul-17 15:00 sparseml/optim/sensitivity.py
+-rw-rw-r--  2.0 unx     2190 b- defN 23-Jul-17 15:00 sparseml/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     6155 b- defN 23-Jul-17 15:00 sparseml/pytorch/base.py
+-rw-rw-r--  2.0 unx      933 b- defN 23-Jul-17 15:00 sparseml/pytorch/opset.py
+-rw-rw-r--  2.0 unx    10884 b- defN 23-Jul-17 15:00 sparseml/pytorch/torch_to_onnx_exporter.py
+-rw-rw-r--  2.0 unx      998 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/__init__.py
+-rw-rw-r--  2.0 unx     4193 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/generic.py
+-rw-rw-r--  2.0 unx     3014 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/registry.py
+-rw-rw-r--  2.0 unx      828 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx     4457 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     3669 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     4000 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     6491 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx     2434 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/classification/mnist.py
+-rw-rw-r--  2.0 unx      767 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/detection/__init__.py
+-rw-rw-r--  2.0 unx    16159 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/detection/coco.py
+-rw-rw-r--  2.0 unx     5705 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/detection/helpers.py
+-rw-rw-r--  2.0 unx    10759 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/detection/voc.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/image_classification/__init__.py
+-rw-rw-r--  2.0 unx     9512 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/image_classification/ffcv_dataset.py
+-rw-rw-r--  2.0 unx      684 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      693 b- defN 23-Jul-17 15:00 sparseml/pytorch/datasets/video/__init__.py
+-rw-rw-r--  2.0 unx      814 b- defN 23-Jul-17 15:00 sparseml/pytorch/framework/__init__.py
+-rw-rw-r--  2.0 unx     5580 b- defN 23-Jul-17 15:00 sparseml/pytorch/framework/info.py
+-rw-rw-r--  2.0 unx      753 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/__init__.py
+-rw-rw-r--  2.0 unx    18265 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/export.py
+-rw-rw-r--  2.0 unx    15494 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/lr_analysis.py
+-rw-rw-r--  2.0 unx    14444 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/pr_sensitivity.py
+-rw-rw-r--  2.0 unx    29287 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/train.py
+-rw-rw-r--  2.0 unx      682 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/utils/__init__.py
+-rw-rw-r--  2.0 unx     4278 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/utils/cli_helpers.py
+-rw-rw-r--  2.0 unx     1257 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/utils/constants.py
+-rw-rw-r--  2.0 unx    21742 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/utils/helpers.py
+-rw-rw-r--  2.0 unx    12056 b- defN 23-Jul-17 15:00 sparseml/pytorch/image_classification/utils/trainer.py
+-rw-rw-r--  2.0 unx      976 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/__init__.py
+-rw-rw-r--  2.0 unx    14753 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/registry.py
+-rw-rw-r--  2.0 unx      901 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/__init__.py
+-rw-rw-r--  2.0 unx    11658 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/darknet.py
+-rw-rw-r--  2.0 unx    40293 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/efficientnet.py
+-rw-rw-r--  2.0 unx    16512 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/inception_v3.py
+-rw-rw-r--  2.0 unx     4164 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/mnist.py
+-rw-rw-r--  2.0 unx     9546 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    13014 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    40800 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    16649 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      824 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/__init__.py
+-rw-rw-r--  2.0 unx     6820 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/ssd.py
+-rw-rw-r--  2.0 unx     8116 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/ssd_lite.py
+-rw-rw-r--  2.0 unx     4046 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/ssd_mobilenet.py
+-rw-rw-r--  2.0 unx     9069 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/ssd_resnet.py
+-rw-rw-r--  2.0 unx    10188 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/detection/yolo_v3.py
+-rw-rw-r--  2.0 unx      763 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/external/__init__.py
+-rw-rw-r--  2.0 unx     6759 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/external/torchvision.py
+-rw-rw-r--  2.0 unx      676 b- defN 23-Jul-17 15:00 sparseml/pytorch/models/recommendation/__init__.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-17 15:00 sparseml/pytorch/nn/__init__.py
+-rw-rw-r--  2.0 unx     8673 b- defN 23-Jul-17 15:00 sparseml/pytorch/nn/activations.py
+-rw-rw-r--  2.0 unx    11854 b- defN 23-Jul-17 15:00 sparseml/pytorch/nn/fatrelu.py
+-rw-rw-r--  2.0 unx     1690 b- defN 23-Jul-17 15:00 sparseml/pytorch/nn/identity.py
+-rw-rw-r--  2.0 unx     2828 b- defN 23-Jul-17 15:00 sparseml/pytorch/nn/se.py
+-rw-rw-r--  2.0 unx     1243 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/__init__.py
+-rw-rw-r--  2.0 unx    13638 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/analyzer_as.py
+-rw-rw-r--  2.0 unx    17069 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     3955 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/analyzer_pruning.py
+-rw-rw-r--  2.0 unx    26838 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/manager.py
+-rw-rw-r--  2.0 unx    36844 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    23085 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    10449 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/mask_pruning_scorer.py
+-rw-rw-r--  2.0 unx     6605 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/optimizer.py
+-rw-rw-r--  2.0 unx    14879 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/sensitivity_as.py
+-rw-rw-r--  2.0 unx     6101 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/sensitivity_lr.py
+-rw-rw-r--  2.0 unx     9324 b- defN 23-Jul-17 15:00 sparseml/pytorch/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      633 b- defN 23-Jul-17 15:00 sparseml/pytorch/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4534 b- defN 23-Jul-17 15:00 sparseml/pytorch/recipe_template/cli.py
+-rw-rw-r--  2.0 unx     1559 b- defN 23-Jul-17 15:00 sparseml/pytorch/recipe_template/description.py
+-rw-rw-r--  2.0 unx    15943 b- defN 23-Jul-17 15:00 sparseml/pytorch/recipe_template/main.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1366 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/info.py
+-rw-rw-r--  2.0 unx    32014 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/modifier.py
+-rw-rw-r--  2.0 unx    18952 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/modifier_thinning.py
+-rw-rw-r--  2.0 unx      705 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/distillation/__init__.py
+-rw-rw-r--  2.0 unx     4741 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/distillation/modifier_distillation.py
+-rw-rw-r--  2.0 unx    14742 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/distillation/modifier_distillation_base.py
+-rw-rw-r--  2.0 unx    19177 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/distillation/modifier_per_layer.py
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/__init__.py
+-rw-rw-r--  2.0 unx    29250 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/mask_creator.py
+-rw-rw-r--  2.0 unx    22391 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/mask_params.py
+-rw-rw-r--  2.0 unx    13389 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_as.py
+-rw-rw-r--  2.0 unx    10455 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_acdc.py
+-rw-rw-r--  2.0 unx    33219 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_base.py
+-rw-rw-r--  2.0 unx     5757 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_constant.py
+-rw-rw-r--  2.0 unx     8860 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_layer.py
+-rw-rw-r--  2.0 unx    15595 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_magnitude.py
+-rw-rw-r--  2.0 unx    63519 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_mfac.py
+-rw-rw-r--  2.0 unx     8774 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_movement.py
+-rw-rw-r--  2.0 unx    24121 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_obs.py
+-rw-rw-r--  2.0 unx    18245 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/modifier_pruning_structured.py
+-rw-rw-r--  2.0 unx     4644 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/pruning/scorer.py
+-rw-rw-r--  2.0 unx      813 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/__init__.py
+-rw-rw-r--  2.0 unx     2220 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/constants.py
+-rw-rw-r--  2.0 unx    32271 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/helpers.py
+-rw-rw-r--  2.0 unx    33626 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py
+-rw-rw-r--  2.0 unx    26778 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/modifier_quantization.py
+-rw-rw-r--  2.0 unx    12558 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/quantization_scheme.py
+-rw-rw-r--  2.0 unx    18014 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/quantize.py
+-rw-rw-r--  2.0 unx    76796 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py
+-rw-rw-r--  2.0 unx      790 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/__init__.py
+-rw-rw-r--  2.0 unx     1778 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/modifier_epoch.py
+-rw-rw-r--  2.0 unx     2883 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/modifier_logging.py
+-rw-rw-r--  2.0 unx    24287 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/modifier_lr.py
+-rw-rw-r--  2.0 unx    21497 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/modifier_params.py
+-rw-rw-r--  2.0 unx     6690 b- defN 23-Jul-17 15:00 sparseml/pytorch/sparsification/training/modifier_regularizer.py
+-rw-rw-r--  2.0 unx      943 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/__init__.py
+-rw-rw-r--  2.0 unx     6490 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/export_onnx.py
+-rw-rw-r--  2.0 unx     2870 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/presets.py
+-rw-rw-r--  2.0 unx     2530 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/sampler.py
+-rw-rw-r--  2.0 unx    41409 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/train.py
+-rw-rw-r--  2.0 unx     7128 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/transforms.py
+-rw-rw-r--  2.0 unx    16675 b- defN 23-Jul-17 15:00 sparseml/pytorch/torchvision/utils.py
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/__init__.py
+-rw-rw-r--  2.0 unx     9706 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/benchmarker.py
+-rw-rw-r--  2.0 unx     2846 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/callbacks.py
+-rw-rw-r--  2.0 unx     1061 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/distributed.py
+-rw-rw-r--  2.0 unx    31098 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/exporter.py
+-rw-rw-r--  2.0 unx    39284 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/helpers.py
+-rw-rw-r--  2.0 unx     1663 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/log_sparsification_info.py
+-rw-rw-r--  2.0 unx    31374 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/logger.py
+-rw-rw-r--  2.0 unx    27048 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/loss.py
+-rw-rw-r--  2.0 unx    11754 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/model.py
+-rw-rw-r--  2.0 unx    39117 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/module.py
+-rw-rw-r--  2.0 unx     8809 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/sparsification.py
+-rw-rw-r--  2.0 unx    30059 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/ssd_helpers.py
+-rw-rw-r--  2.0 unx    12337 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/yolo_helpers.py
+-rw-rw-r--  2.0 unx      617 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/sparsification_info/__init__.py
+-rw-rw-r--  2.0 unx    10457 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/sparsification_info/configs.py
+-rw-rw-r--  2.0 unx     4309 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/sparsification_info/helpers.py
+-rw-rw-r--  2.0 unx     2946 b- defN 23-Jul-17 15:00 sparseml/pytorch/utils/sparsification_info/module_sparsification_info.py
+-rw-rw-r--  2.0 unx      655 b- defN 23-Jul-17 15:00 sparseml/recipe_template/__init__.py
+-rw-rw-r--  2.0 unx     4788 b- defN 23-Jul-17 15:00 sparseml/recipe_template/utils.py
+-rw-rw-r--  2.0 unx     1058 b- defN 23-Jul-17 15:00 sparseml/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     9387 b- defN 23-Jul-17 15:00 sparseml/sparsification/analyzer.py
+-rw-rw-r--  2.0 unx     9065 b- defN 23-Jul-17 15:00 sparseml/sparsification/info.py
+-rw-rw-r--  2.0 unx    15565 b- defN 23-Jul-17 15:00 sparseml/sparsification/model_info.py
+-rw-rw-r--  2.0 unx     2002 b- defN 23-Jul-17 15:00 sparseml/sparsification/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10117 b- defN 23-Jul-17 15:00 sparseml/sparsification/modifier_lr.py
+-rw-rw-r--  2.0 unx     5505 b- defN 23-Jul-17 15:00 sparseml/sparsification/modifier_params.py
+-rw-rw-r--  2.0 unx    12845 b- defN 23-Jul-17 15:00 sparseml/sparsification/modifier_pruning.py
+-rw-rw-r--  2.0 unx     3700 b- defN 23-Jul-17 15:00 sparseml/sparsification/oracle.py
+-rw-rw-r--  2.0 unx    18570 b- defN 23-Jul-17 15:00 sparseml/sparsification/recipe_builder.py
+-rw-rw-r--  2.0 unx    14413 b- defN 23-Jul-17 15:00 sparseml/sparsification/recipe_editor.py
+-rw-rw-r--  2.0 unx     1250 b- defN 23-Jul-17 15:00 sparseml/sparsification/types.py
+-rw-rw-r--  2.0 unx     1169 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/__init__.py
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/base.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/__init__.py
+-rw-rw-r--  2.0 unx     8121 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/dataset.py
+-rw-rw-r--  2.0 unx     5600 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/helpers.py
+-rw-rw-r--  2.0 unx     2768 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/registry.py
+-rw-rw-r--  2.0 unx      807 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/classification/__init__.py
+-rw-rw-r--  2.0 unx    12686 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/classification/cifar.py
+-rw-rw-r--  2.0 unx     8690 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/classification/imagefolder.py
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/classification/imagenet.py
+-rw-rw-r--  2.0 unx     4695 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/datasets/classification/imagenette.py
+-rw-rw-r--  2.0 unx      805 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/framework/__init__.py
+-rw-rw-r--  2.0 unx     5859 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/framework/info.py
+-rw-rw-r--  2.0 unx      925 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/__init__.py
+-rw-rw-r--  2.0 unx    19752 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/estimator.py
+-rw-rw-r--  2.0 unx    14774 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/registry.py
+-rw-rw-r--  2.0 unx      822 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/__init__.py
+-rw-rw-r--  2.0 unx     3540 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/mnist.py
+-rw-rw-r--  2.0 unx    11161 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/mobilenet.py
+-rw-rw-r--  2.0 unx    18359 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/mobilenet_v2.py
+-rw-rw-r--  2.0 unx    28103 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/resnet.py
+-rw-rw-r--  2.0 unx    26886 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/models/classification/vgg.py
+-rw-rw-r--  2.0 unx      865 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/nn/__init__.py
+-rw-rw-r--  2.0 unx    18670 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/nn/layers.py
+-rw-rw-r--  2.0 unx     1238 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/__init__.py
+-rw-rw-r--  2.0 unx     8607 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/analyzer_module.py
+-rw-rw-r--  2.0 unx     9591 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/manager.py
+-rw-rw-r--  2.0 unx    19683 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/mask_creator_pruning.py
+-rw-rw-r--  2.0 unx    33919 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/mask_pruning.py
+-rw-rw-r--  2.0 unx    15955 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/modifier.py
+-rw-rw-r--  2.0 unx     1715 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/modifier_epoch.py
+-rw-rw-r--  2.0 unx    10685 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/modifier_lr.py
+-rw-rw-r--  2.0 unx     7092 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/modifier_params.py
+-rw-rw-r--  2.0 unx    15702 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/modifier_pruning.py
+-rw-rw-r--  2.0 unx     5682 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/schedule_lr.py
+-rw-rw-r--  2.0 unx     9232 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/optim/sensitivity_pruning.py
+-rw-rw-r--  2.0 unx      801 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/sparsification/__init__.py
+-rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/sparsification/info.py
+-rw-rw-r--  2.0 unx      967 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/__init__.py
+-rw-rw-r--  2.0 unx    10913 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/exporter.py
+-rw-rw-r--  2.0 unx      996 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/helpers.py
+-rw-rw-r--  2.0 unx     1974 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/loss.py
+-rw-rw-r--  2.0 unx     8119 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/nets_utils.py
+-rw-rw-r--  2.0 unx     1327 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/summary.py
+-rw-rw-r--  2.0 unx    12536 b- defN 23-Jul-17 15:00 sparseml/tensorflow_v1/utils/variable.py
+-rw-rw-r--  2.0 unx     1511 b- defN 23-Jul-17 15:00 sparseml/transformers/__init__.py
+-rw-rw-r--  2.0 unx    22048 b- defN 23-Jul-17 15:00 sparseml/transformers/export.py
+-rw-rw-r--  2.0 unx    30756 b- defN 23-Jul-17 15:00 sparseml/transformers/masked_language_modeling.py
+-rw-rw-r--  2.0 unx    36976 b- defN 23-Jul-17 15:00 sparseml/transformers/question_answering.py
+-rw-rw-r--  2.0 unx    40299 b- defN 23-Jul-17 15:00 sparseml/transformers/text_classification.py
+-rw-rw-r--  2.0 unx    34350 b- defN 23-Jul-17 15:00 sparseml/transformers/token_classification.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-17 15:00 sparseml/transformers/sparsification/__init__.py
+-rw-rw-r--  2.0 unx    19529 b- defN 23-Jul-17 15:00 sparseml/transformers/sparsification/question_answering.py
+-rw-rw-r--  2.0 unx    44413 b- defN 23-Jul-17 15:00 sparseml/transformers/sparsification/trainer.py
+-rw-rw-r--  2.0 unx     1890 b- defN 23-Jul-17 15:00 sparseml/transformers/sparsification/training_args.py
+-rw-rw-r--  2.0 unx      794 b- defN 23-Jul-17 15:00 sparseml/transformers/utils/__init__.py
+-rw-rw-r--  2.0 unx     3090 b- defN 23-Jul-17 15:00 sparseml/transformers/utils/helpers.py
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Jul-17 15:00 sparseml/transformers/utils/metrics.py
+-rw-rw-r--  2.0 unx    17074 b- defN 23-Jul-17 15:00 sparseml/transformers/utils/model.py
+-rw-rw-r--  2.0 unx      844 b- defN 23-Jul-17 15:00 sparseml/utils/__init__.py
+-rw-rw-r--  2.0 unx      886 b- defN 23-Jul-17 15:00 sparseml/utils/frameworks.py
+-rw-rw-r--  2.0 unx    26562 b- defN 23-Jul-17 15:00 sparseml/utils/helpers.py
+-rw-rw-r--  2.0 unx     3983 b- defN 23-Jul-17 15:00 sparseml/utils/restricted_eval.py
+-rw-rw-r--  2.0 unx     1083 b- defN 23-Jul-17 15:00 sparseml/utils/singleton.py
+-rw-rw-r--  2.0 unx     6312 b- defN 23-Jul-17 15:00 sparseml/utils/worker.py
+-rw-rw-r--  2.0 unx     2952 b- defN 23-Jul-17 15:00 sparseml/utils/wrapper.py
+-rw-rw-r--  2.0 unx      819 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/__init__.py
+-rw-rw-r--  2.0 unx      833 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/cifar.py
+-rw-rw-r--  2.0 unx     3750 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/coco.py
+-rw-rw-r--  2.0 unx     1217 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/helpers.py
+-rw-rw-r--  2.0 unx    23366 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/imagenet.py
+-rw-rw-r--  2.0 unx     8967 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/imagenette.py
+-rw-rw-r--  2.0 unx     1009 b- defN 23-Jul-17 15:00 sparseml/utils/datasets/voc.py
+-rw-rw-r--  2.0 unx     1875 b- defN 23-Jul-17 15:00 sparseml/yolact/COCO.sh
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Jul-17 15:00 sparseml/yolact/COCO_test.sh
+-rw-rw-r--  2.0 unx     4020 b- defN 23-Jul-17 15:00 sparseml/yolact/__init__.py
+-rw-rw-r--  2.0 unx     1784 b- defN 23-Jul-17 15:00 sparseml/yolact/scripts.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jul-17 15:00 sparseml/yolov5/__init__.py
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Jul-17 15:00 sparseml/yolov5/helpers.py
+-rw-rw-r--  2.0 unx     1609 b- defN 23-Jul-17 15:00 sparseml/yolov5/scripts.py
+-rw-rw-r--  2.0 unx     1220 b- defN 23-Jul-17 15:00 sparseml/yolov5/yolov5.status.yaml
+-rw-rw-r--  2.0 unx     1115 b- defN 23-Jul-17 15:00 sparseml/yolov8/__init__.py
+-rw-rw-r--  2.0 unx     5781 b- defN 23-Jul-17 15:00 sparseml/yolov8/default.yaml
+-rw-rw-r--  2.0 unx     2502 b- defN 23-Jul-17 15:00 sparseml/yolov8/export.py
+-rw-rw-r--  2.0 unx     2259 b- defN 23-Jul-17 15:00 sparseml/yolov8/modules.py
+-rw-rw-r--  2.0 unx     7194 b- defN 23-Jul-17 15:00 sparseml/yolov8/train.py
+-rw-rw-r--  2.0 unx    35999 b- defN 23-Jul-17 15:00 sparseml/yolov8/trainers.py
+-rw-rw-r--  2.0 unx     2748 b- defN 23-Jul-17 15:00 sparseml/yolov8/val.py
+-rw-rw-r--  2.0 unx     8196 b- defN 23-Jul-17 15:00 sparseml/yolov8/validators.py
+-rw-rw-r--  2.0 unx      685 b- defN 23-Jul-17 15:00 sparseml/yolov8/utils/__init__.py
+-rw-rw-r--  2.0 unx     6247 b- defN 23-Jul-17 15:00 sparseml/yolov8/utils/export_samples.py
+-rw-rw-r--  2.0 unx     4041 b- defN 23-Jul-17 15:00 sparseml/yolov8/utils/helpers.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/LICENSE
+-rw-rw-r--  2.0 unx    21837 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/METADATA
+-rw-rw-r--  2.0 unx     2158 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/NOTICE
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/WHEEL
+-rw-rw-r--  2.0 unx     2326 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        9 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx    37503 b- defN 23-Jul-17 15:02 sparseml_nightly-1.6.0.20230717.dist-info/RECORD
+376 files, 3503295 bytes uncompressed, 907872 bytes compressed:  74.1%
```

## zipnote {}

```diff
@@ -102,14 +102,17 @@
 
 Filename: sparseml/exporters/transforms/matmul_to_qlinearmatmul.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/onnx_transform.py
 Comment: 
 
+Filename: sparseml/exporters/transforms/propagate_dequant_through_split.py
+Comment: 
+
 Filename: sparseml/exporters/transforms/propagate_embedding_quantization.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/quantize_qat_embedding.py
 Comment: 
 
 Filename: sparseml/exporters/transforms/quantize_residuals.py
@@ -1098,29 +1101,29 @@
 
 Filename: sparseml/yolov8/utils/export_samples.py
 Comment: 
 
 Filename: sparseml/yolov8/utils/helpers.py
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/LICENSE
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/LICENSE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/METADATA
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/METADATA
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/NOTICE
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/NOTICE
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/WHEEL
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/WHEEL
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/entry_points.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/top_level.txt
 Comment: 
 
-Filename: sparseml_nightly-1.6.0.20230707.dist-info/RECORD
+Filename: sparseml_nightly-1.6.0.20230717.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sparseml/exporters/onnx_to_deepsparse.py

```diff
@@ -71,14 +71,15 @@
             sparseml_transforms.FoldIdentityInitializers(),
             sparseml_transforms.InitializersToUint8(),
             sparseml_transforms.FlattenQParams(),
             sparseml_transforms.FoldConvDivBn(),
             sparseml_transforms.DeleteRepeatedQdq(),
             sparseml_transforms.QuantizeQATEmbedding(),
             sparseml_transforms.PropagateEmbeddingQuantization(),
+            sparseml_transforms.PropagateDequantThroughSplit(),
             sparseml_transforms.MatMulToQLinearMatMul(),
             sparseml_transforms.MatMulAddToMatMulIntegerAddCastMul(),
             sparseml_transforms.MatMulToMatMulIntegerCastMul(),
             sparseml_transforms.FoldReLUQuants(),
             sparseml_transforms.ConvToQLinearConv()
             if use_qlinear_conv
             else sparseml_transforms.ConvToConvIntegerAddCastMul(),
```

## sparseml/exporters/transforms/__init__.py

```diff
@@ -37,13 +37,14 @@
 from .fold_relu_quants import FoldReLUQuants
 from .gemm_to_matmulinteger_add_cast_mul import GemmToMatMulIntegerAddCastMul
 from .gemm_to_qlinearmatmul import GemmToQLinearMatMul
 from .initializers_to_uint8 import InitializersToUint8
 from .matmul_add_to_matmulinteger_add_cast_mul import MatMulAddToMatMulIntegerAddCastMul
 from .matmul_to_matmulinteger_cast_mul import MatMulToMatMulIntegerCastMul
 from .propagate_embedding_quantization import PropagateEmbeddingQuantization
+from .propagate_dequant_through_split import PropagateDequantThroughSplit
 from .quantize_qat_embedding import QuantizeQATEmbedding
 from .quantize_residuals import QuantizeResiduals
 from .remove_duplicate_qconv_weights import RemoveDuplicateQConvWeights
 from .remove_duplicate_quantize_ops import RemoveDuplicateQuantizeOps
 from .skip_input_quantize import SkipInputQuantize
 from .kv_cache import *
```

## sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py

```diff
@@ -62,40 +62,72 @@
     |     |
     | Mul (Rescale from bias scale)
     ```
     """
 
     def transform(self, model: ModelProto) -> ModelProto:
         graph = ONNXGraph(model)
-        matches = get_structural_matches(
+
+        # Nodes with bias
+        matches_bias = get_structural_matches(
             graph,
             parent_ops=[
-                ["QuantizeLinear", "DequantizeLinear"],
+                ["DequantizeLinear"],
                 [
                     # weight should be initializer
                     INITIALIZER_MATCH,
                     "QuantizeLinear",
                     "DequantizeLinear",
                 ],
                 [
                     # bias should be initializer
-                    INITIALIZER_MATCH
+                    INITIALIZER_MATCH,
+                ],
+            ],
+            op_type="Conv",
+        )
+
+        # Nodes without bias
+        matches_no_bias = get_structural_matches(
+            graph,
+            parent_ops=[
+                ["DequantizeLinear"],
+                [
+                    # weight should be initializer
+                    INITIALIZER_MATCH,
+                    "QuantizeLinear",
+                    "DequantizeLinear",
                 ],
             ],
             op_type="Conv",
         )
+
+        matches = matches_bias
+        matches_names = [m.node.name for m in matches]
+        for match in matches_no_bias:
+            if match.node.name not in matches_names:
+                matches.append(match)
+
         for match in matches:
             self.log_match(match)
             self._transform_match(graph, model, match)
         return model
 
-    def _transform_match(self, graph: ONNXGraph, model: ModelProto, match: MatchResult):
-        input_quant, input_dequant = match.parents[0]
+    def _transform_match(
+        self,
+        graph: ONNXGraph,
+        model: ModelProto,
+        match: MatchResult,
+    ):
+        (input_dequant,) = match.parents[0]
         weight_init, weight_quantize_node, weight_dequantize_node = match.parents[1]
-        (bias_init,) = match.parents[2]
+        if len(match.parents) == 3:
+            (bias_init,) = match.parents[2]
+        else:
+            bias_init = None
 
         model = add_quantized_conv_matmul_add_ops(
             model=model,
             node=match.node,
             input_quantize_node=input_dequant,
             weight_quantize_node=weight_quantize_node,
             input_quantize_params=get_quantization_params(
```

## sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py

```diff
@@ -63,14 +63,45 @@
     |     |
     | Mul (Rescale from bias scale)
     ```
     """
 
     def transform(self, model: ModelProto) -> ModelProto:
         graph = ONNXGraph(model)
+
+        # Weight on input 0
+        matches = get_structural_matches(
+            graph,
+            op_type="MatMul",
+            parent_ops=[
+                [
+                    # weight should be initializer
+                    INITIALIZER_MATCH,
+                    "QuantizeLinear",
+                    "DequantizeLinear",
+                    optional_node("Transpose"),
+                ],
+                [any_of("QuantizeLinear", "DequantizeLinear")],
+            ],
+            children_ops=[[optional_node("Add")]],
+        )
+        for match in matches:
+            add_node = match.children[0][0]
+            bias_init = None
+            if add_node:
+                # NOTE: bias could be either input 0 or 1 of add node
+                # if add does not have a bias initializer,
+                # still do conversion, but do not fold the bias add to rescale
+                bias_init = graph.get_init_by_name(match.children[0][0].input[1])
+                if bias_init is None:
+                    bias_init = graph.get_init_by_name(match.children[0][0].input[0])
+            self.log_match(match)
+            self._transform_match(graph, model, match, bias_init, 0)
+
+        # Weight on input 1
         matches = get_structural_matches(
             graph,
             op_type="MatMul",
             parent_ops=[
                 [any_of("QuantizeLinear", "DequantizeLinear")],
                 [
                     # weight should be initializer
@@ -89,27 +120,33 @@
                 # NOTE: bias could be either input 0 or 1 of add node
                 # if add does not have a bias initializer,
                 # still do conversion, but do not fold the bias add to rescale
                 bias_init = graph.get_init_by_name(match.children[0][0].input[1])
                 if bias_init is None:
                     bias_init = graph.get_init_by_name(match.children[0][0].input[0])
             self.log_match(match)
-            self._transform_match(graph, model, match, bias_init)
+            self._transform_match(graph, model, match, bias_init, 1)
+
         return model
 
     def _transform_match(
         self,
         graph: ONNXGraph,
         model: ModelProto,
         match: MatchResult,
         bias_init: TensorProto,
+        weight_parent: int,
     ):
         matmul = match.node
-        (input_quant,) = match.parents[0]
-        weight_init, weight_quant, weight_dequant, opt_transpose = match.parents[1]
+        if weight_parent == 0:
+            (input_quant,) = match.parents[1]
+            weight_init, weight_quant, weight_dequant, opt_transpose = match.parents[0]
+        else:
+            (input_quant,) = match.parents[0]
+            weight_init, weight_quant, weight_dequant, opt_transpose = match.parents[1]
         (add,) = match.children[0]
 
         input_quantize_params = get_quantization_params(
             model, input_quant, include_target=False
         )
         weight_quantize_params = get_quantization_params(
             model, weight_quant, include_target=True
```

## sparseml/exporters/transforms/propagate_embedding_quantization.py

```diff
@@ -11,14 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
 
 import numpy
+import onnx.numpy_helper
 from onnx import ModelProto, numpy_helper
 
 from sparseml.exporters.transforms.onnx_transform import OnnxTransform
 from sparseml.exporters.transforms.utils.matching import get_structural_matches
 from sparseml.onnx.utils.graph_editor import ONNXGraph
 
 
@@ -75,35 +76,65 @@
                 ["Slice", "Pad", "Concat"],
                 ["Slice", "Pad", "Concat"],
                 # NOTE: since the other two branch also send output to concat,
                 #       the actual concat branch will be last in a sorted graph.
                 ["Concat"],
             ],
         )
+
+        initializer_dict = {i.name: i for i in model.graph.initializer}
+
         for match in matches:
             (gather,) = match.parents[0]
             dequant = match.node
-            slice1, _, concat1 = match.children[0]
-            slice2, _, concat2 = match.children[1]
+            slice1, pad1, concat1 = match.children[0]
+            slice2, pad2, concat2 = match.children[1]
             (concat,) = match.children[2]
 
             # check for uint8 initializer
             indices = graph.get_init_by_name(gather.input[0])
-            if indices is None or numpy_helper.to_array(indices).dtype != numpy.uint8:
+            if indices is None or numpy_helper.to_array(indices).dtype not in [
+                numpy.uint8,
+                numpy.int8,
+            ]:
                 continue
 
             # check that all concats are the same
             if concat.name != concat1.name or concat.name != concat2.name:
                 continue
 
             self.log_match(match)
 
-            assert concat.input[2] == dequant.output[0]
-            concat.input[2] = gather.output[0]
+            for id, input_name in enumerate(concat.input):
+                if input_name == dequant.output[0]:
+                    break
+
+            concat.input[id] = gather.output[0]
             slice1.input[0] = gather.output[0]
             slice2.input[0] = gather.output[0]
 
+            zero_point_initializer = initializer_dict[match.node.input[2]]
+            zero_point = onnx.numpy_helper.to_array(zero_point_initializer)
+
+            pad1_value_initializer = initializer_dict[pad1.input[2]]
+            pad1_value = onnx.numpy_helper.to_array(pad1_value_initializer)
+            pad1_value = pad1_value.astype(zero_point.dtype) + zero_point
+            new_pad1_value_initializer = numpy_helper.from_array(
+                pad1_value, name=pad1_value_initializer.name
+            )
+            model.graph.initializer.remove(pad1_value_initializer)
+            model.graph.initializer.append(new_pad1_value_initializer)
+
+            pad2_value_initializer = initializer_dict[pad2.input[2]]
+            pad2_value = onnx.numpy_helper.to_array(pad2_value_initializer)
+            pad2_value = pad2_value.astype(zero_point.dtype) + zero_point
+            new_pad2_value_initializer = numpy_helper.from_array(
+                pad2_value, name=pad2_value_initializer.name
+            )
+            model.graph.initializer.remove(pad2_value_initializer)
+            model.graph.initializer.append(new_pad2_value_initializer)
+
             tmp = concat.output[0]
             concat.output[0] = dequant.output[0]
             dequant.output[0] = tmp
             dequant.input[0] = concat.output[0]
         return model
```

## sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py

```diff
@@ -25,15 +25,15 @@
 
 
 __all__ = ["CacheKeysAndValues"]
 
 
 _LOGGER = logging.getLogger(__name__)
 
-ALLOWED_NODES_BEFORE_SOFTMAX = ["Cast"]
+ALLOWED_NODES_BEFORE_SOFTMAX = ["Cast", "Reshape"]
 OUTPUT_CACHE_NAME = """present.{attention_layer_idx}.{cache_type}"""
 INPUT_CACHE_NAME = """past_key_values.{attention_layer_idx}.{cache_type}"""
 
 
 class CacheKeysAndValues(OnnxTransform):
     """
     Inject the key and value caches into the graph for the attention layers.
```

## sparseml/exporters/transforms/kv_cache/configs.py

```diff
@@ -98,17 +98,28 @@
     key_num_attention_heads="n_head",
     key_num_embedding_hidden_size="n_embd",
     transpose_value_input=(0, 2, 1, 3),
     transpose_key_input=None,
     multiply_batch_by_num_att_heads=False,
 )
 
+BLOOM_CONFIG = KeyValueCacheConfig(
+    model_name="bloom",
+    positional_embedding_transform=None,
+    key_num_attention_heads="num_attention_heads",
+    key_num_embedding_hidden_size="n_embed",
+    transpose_value_input=None,
+    transpose_key_input=(0, 1, 3, 2),
+    multiply_batch_by_num_att_heads=True,
+)
+
 
 def get_kv_cache_config(
-    model_path: str, supported_configs: List[BaseModel] = [OPT_CONFIG, CODEGEN_CONFIG]
+    model_path: str,
+    supported_configs: List[BaseModel] = [OPT_CONFIG, CODEGEN_CONFIG, BLOOM_CONFIG],
 ) -> KeyValueCacheConfig:
     """
     Get the kv cache config for the model at the given path.
 
     :param model_path: The path to the directory containing
         the transformers model. It is assumed that
         the `config.json` file (as supplied by the
```

## sparseml/pytorch/datasets/classification/cifar.py

```diff
@@ -14,14 +14,17 @@
 
 """
 CIFAR dataset implementations for the image classification field in computer vision.
 More info for the dataset can be found
 `here <https://www.cs.toronto.edu/~kriz/cifar.html>`__.
 """
 
+import logging
+
+
 try:
     from torchvision import transforms
     from torchvision.datasets import CIFAR10, CIFAR100
 
     torchvision_import_error = None
 except Exception as torchvision_error:
     CIFAR10 = object  # default for constructor
@@ -32,14 +35,16 @@
 from sparseml.pytorch.datasets.registry import DatasetRegistry
 from sparseml.utils.datasets import default_dataset_path
 
 
 __all__ = ["CIFAR10Dataset", "CIFAR100Dataset"]
 
 
+_LOGGER = logging.getLogger(__file__)
+
 _CIFAR10_RGB_MEANS = [0.491, 0.482, 0.447]
 _CIFAR10_RGB_STDS = [0.247, 0.243, 0.262]
 
 
 @DatasetRegistry.register(
     key=["cifar10", "cifar_10"],
     attributes={
@@ -60,15 +65,20 @@
     """
 
     def __init__(
         self,
         root: str = default_dataset_path("cifar10"),
         train: bool = True,
         rand_trans: bool = False,
+        image_size: None = None,
     ):
+        if image_size is not None:
+            _LOGGER.warning(
+                "image_size not supported for CIFAR dataset, using default size"
+            )
         if torchvision_import_error is not None:
             raise torchvision_import_error
 
         if rand_trans:
             trans = [
                 transforms.RandomCrop(32, padding=4),
                 transforms.RandomHorizontalFlip(),
@@ -110,15 +120,20 @@
     """
 
     def __init__(
         self,
         root: str = default_dataset_path("cifar100"),
         train: bool = True,
         rand_trans: bool = False,
+        image_size: None = None,
     ):
+        if image_size is not None:
+            _LOGGER.warning(
+                "image_size not supported for CIFAR dataset, using default size"
+            )
         normalize = transforms.Normalize(
             mean=_CIFAR100_RGB_MEANS, std=_CIFAR100_RGB_STDS
         )
         trans = (
             [transforms.RandomCrop(32, padding=4), transforms.RandomHorizontalFlip()]
             if rand_trans
             else []
```

## sparseml/pytorch/sparsification/quantization/quantize.py

```diff
@@ -358,16 +358,15 @@
 ) -> Optional[str]:
     # match preferences:
     #   1. match module type name
     #   2. match the submodule prefix (longest first)
     submodule_match = ""
     for name_or_type in names_or_types:
         name_to_compare = submodule_name[:]
-        if name_to_compare.startswith("module."):
-            name_to_compare = name_to_compare[7:]
+        name_to_compare = _maybe_discard_prefix(name_to_compare)
         if name_or_type == submodule.__class__.__name__:
             # type match, return type name
             return name_or_type
         if name_to_compare.startswith(name_or_type) and (
             len(name_or_type) > len(submodule_match)
         ):
             # match to most specific submodule name
@@ -422,16 +421,15 @@
 ):
     def _get_unmatched_types_or_names(types_or_names):
         unmatched = []
         for type_or_name in types_or_names:
             matched = False
             for submodule_name, submodule in model.named_modules():
                 name_to_compare = submodule_name[:]
-                if name_to_compare.startswith("module."):
-                    name_to_compare = name_to_compare[7:]
+                name_to_compare = _maybe_discard_prefix(name_to_compare)
                 if name_to_compare.startswith(type_or_name) or (
                     submodule.__class__.__name__ == type_or_name
                 ):
                     matched = True
                     break
             if not matched:
                 unmatched.append(type_or_name)
@@ -449,7 +447,14 @@
         raise ValueError(
             _build_error_str("scheme_overrides", unmatched_scheme_overrides)
         )
 
     unmatched_ignore = _get_unmatched_types_or_names(ignore)
     if unmatched_ignore:
         raise ValueError(_build_error_str("ignore", unmatched_ignore))
+
+
+def _maybe_discard_prefix(name: str) -> str:
+    for prefix in ["module.", "model."]:
+        if name.startswith(prefix):
+            name = name.replace(prefix, "", 1)
+    return name
```

## sparseml/transformers/question_answering.py

```diff
@@ -16,18 +16,15 @@
 
 # Adapted from https://github.com/huggingface/transformers
 # neuralmagic: no copyright
 
 """
 Fine-tuning the library models for question answering integrated with sparseml
 """
-
-# You can also adapt this script on your own question answering task.
-# Pointers for this are left as comments.
-
+import json
 import logging
 import os
 import sys
 from contextlib import nullcontext
 from dataclasses import dataclass, field
 from typing import Optional
 
@@ -52,14 +49,18 @@
     QuestionAnsweringTrainer,
     TrainingArguments,
     postprocess_qa_predictions,
 )
 from sparseml.transformers.utils import SparseAutoModel, get_shared_tokenizer_src
 
 
+# You can also adapt this script on your own question answering task.
+# Pointers for this are left as comments.
+
+
 require_version(
     "datasets>=1.18.0",
     "To fix: pip install -r examples/pytorch/question-answering/requirements.txt",
 )
 
 
 _LOGGER = logging.getLogger(__name__)
@@ -909,20 +910,30 @@
 
         if data_args.validation_file is not None:
             data_files["validation"] = data_args.validation_file
             extension = data_args.validation_file.split(".")[-1]
         if data_args.test_file is not None:
             data_files["test"] = data_args.test_file
             extension = data_args.test_file.split(".")[-1]
-        raw_datasets = load_dataset(
-            extension,
-            data_files=data_files,
-            field="data",
-            cache_dir=cache_dir,
-        )
+
+        try:
+            raw_datasets = load_dataset(
+                extension,
+                data_files=data_files,
+                field="data",
+                cache_dir=cache_dir,
+            )
+        except (json.JSONDecodeError, datasets.builder.DatasetGenerationError):
+            # run without `field="data"` - JSONL files will not always have each
+            # line nested under a top level field
+            raw_datasets = load_dataset(
+                extension,
+                data_files=data_files,
+                cache_dir=cache_dir,
+            )
     # See more about loading any type of standard or custom dataset
     # (from files, python dict, pandas DataFrame, etc) at
     # https://huggingface.co/docs/datasets/loading_datasets.html.
     return raw_datasets
 
 
 def _mp_fn(index):
```

## sparseml/transformers/utils/model.py

```diff
@@ -403,15 +403,15 @@
             return None, False
 
         _LOGGER.warning(
             "QAT state detected, ignore any loading errors, weights will reload "
             f"after SparseML recipes have been applied {model_name_or_path}"
         )
 
-        return {}, True
+        return None, True
 
     @staticmethod
     def _check_tf(model_name_or_path: str):
         if ".ckpt" in model_name_or_path:
             raise ValueError(
                 "PyTorch is the only supported model type currently for SparseML "
                 "HuggingFace Transformers integration. "
```

## sparseml/yolov8/utils/export_samples.py

```diff
@@ -159,23 +159,24 @@
     sample_out_dir: str,
     file_idx: str,
 ):
 
     # Run model to get onnxruntime outputs
     ort_inputs = {session.get_inputs()[0].name: image}
     ort_outs = session.run(None, ort_inputs)
-    preds = ort_outs
+    preds = numpy.squeeze(ort_outs, axis=0)
+    preds = numpy.squeeze(preds, axis=0)
 
     sample_output_filename = os.path.join(sample_out_dir, f"out-{file_idx}.npz")
     numpy.savez(sample_output_filename, preds)
 
 
 def _export_inputs(image: torch.Tensor, sample_in_dir: str, file_idx: str):
 
-    sample_in = image.detach().to("cpu")
+    sample_in = image.detach().to("cpu").squeeze(0)
 
     sample_input_filename = os.path.join(sample_in_dir, f"inp-{file_idx}.npz")
     numpy.savez(sample_input_filename, sample_in)
 
 
 def _graph_has_uint8_inputs(onnx_path: str) -> bool:
     """
```

## Comparing `sparseml_nightly-1.6.0.20230707.dist-info/LICENSE` & `sparseml_nightly-1.6.0.20230717.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230707.dist-info/METADATA` & `sparseml_nightly-1.6.0.20230717.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sparseml-nightly
-Version: 1.6.0.20230707
+Version: 1.6.0.20230717
 Summary: Libraries for applying sparsification recipes to neural networks with a few lines of code, enabling faster and smaller models
 Home-page: https://github.com/neuralmagic/sparseml
 Author: Neuralmagic, Inc.
 Author-email: support@neuralmagic.com
 License: Apache
 Keywords: inference,machine learning,neural network,computer vision,nlp,cv,deep learning,torch,pytorch,tensorflow,keras,sparsity,pruning,deep learning libraries,onnx,quantization,automl
 Platform: UNKNOWN
@@ -40,15 +40,15 @@
 Requires-Dist: pydantic (<2.0.0,>=1.8.2)
 Requires-Dist: requests (>=2.0.0)
 Requires-Dist: scikit-image (>=0.15.0)
 Requires-Dist: scikit-learn (>=0.24.2)
 Requires-Dist: tqdm (>=4.0.0)
 Requires-Dist: toposort (>=1.0)
 Requires-Dist: GPUtil (>=1.4.0)
-Requires-Dist: protobuf (>=3.12.2)
+Requires-Dist: protobuf (<=3.20.3,>=3.12.2)
 Requires-Dist: click (!=8.0.0,>=7.1.2)
 Requires-Dist: scipy (<1.9.2,>=1.8) ; python_version <= "3.9"
 Requires-Dist: scipy (>=1.0.0) ; python_version > "3.9"
 Provides-Extra: clip
 Requires-Dist: open-clip-torch (==2.20.0) ; extra == 'clip'
 Provides-Extra: deepsparse
 Requires-Dist: deepsparse-nightly (~=1.6.0) ; extra == 'deepsparse'
@@ -105,17 +105,18 @@
 Requires-Dist: gputils ; extra == 'torchvision'
 Requires-Dist: torchvision (<=0.15.1,>=0.3.0) ; extra == 'torchvision'
 Requires-Dist: opencv-python (<=4.6.0.66) ; extra == 'torchvision'
 Provides-Extra: transformers
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'transformers'
 Requires-Dist: gputils ; extra == 'transformers'
 Requires-Dist: nm-transformers-nightly (~=1.6.0) ; extra == 'transformers'
-Requires-Dist: datasets (<=1.18.4) ; extra == 'transformers'
+Requires-Dist: datasets (<=2.11) ; extra == 'transformers'
 Requires-Dist: scikit-learn ; extra == 'transformers'
 Requires-Dist: seqeval ; extra == 'transformers'
+Requires-Dist: einops ; extra == 'transformers'
 Requires-Dist: accelerate (>=0.20.3) ; extra == 'transformers'
 Provides-Extra: ultralytics
 Requires-Dist: ultralytics (==8.0.30) ; extra == 'ultralytics'
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'ultralytics'
 Provides-Extra: yolov5
 Requires-Dist: torch (<=2.0,>=1.7.0) ; extra == 'yolov5'
 Requires-Dist: gputils ; extra == 'yolov5'
```

## Comparing `sparseml_nightly-1.6.0.20230707.dist-info/NOTICE` & `sparseml_nightly-1.6.0.20230717.dist-info/NOTICE`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt` & `sparseml_nightly-1.6.0.20230717.dist-info/entry_points.txt`

 * *Files identical despite different names*

## Comparing `sparseml_nightly-1.6.0.20230707.dist-info/RECORD` & `sparseml_nightly-1.6.0.20230717.dist-info/RECORD`

 * *Files 1% similar despite different names*

```diff
@@ -11,43 +11,44 @@
 sparseml/deepsparse/framework/__init__.py,sha256=ZHrXXM3AMH78zKcF8Y40IBuy38UFy4fLrvytozw_bNY,801
 sparseml/deepsparse/framework/info.py,sha256=HVDPHFXggFeDqbpM20PkByf1nBccwKnjpTWh0EfrVas,6032
 sparseml/deepsparse/sparsification/__init__.py,sha256=re_2FtHWvO-iQQwRRJZDKz3l_pFZuwe266-4ZFxQqbY,813
 sparseml/deepsparse/sparsification/info.py,sha256=O5FJg5KMJvj-HcJn9W9iiKGZ6Z7_1SavOX-TstXRr6Q,1348
 sparseml/exporters/__init__.py,sha256=fH6rjBYAxuwrTzBTlTjTgCYNyh6TCvCqajCz4Im4YrA,617
 sparseml/exporters/base_exporter.py,sha256=M1HEe9GNf51uYx1z-qxWjIYo5iGZ_Ish8uZ3mj6OZR8,1477
 sparseml/exporters/kv_cache_injector.py,sha256=P14Ma0IRvLUJ7bdKmxWTHwHmTIxJaPYn2z0E8P2aa4U,6325
-sparseml/exporters/onnx_to_deepsparse.py,sha256=OO7WosKj8jtd-pSoh7RzaJh-ScWPHV7d-F75gOvJu08,4783
-sparseml/exporters/transforms/__init__.py,sha256=x0mpqLIbsRXjVVot0MH7ebFBmJwV_oZdOp7LhUEydI4,2276
+sparseml/exporters/onnx_to_deepsparse.py,sha256=XBCXBuJKzxZnQBegZuPU4ZC23VTI8MEXDJI3mWXzfXo,4847
+sparseml/exporters/transforms/__init__.py,sha256=0SMdBqAFpcoDTWDklE2nSk9G4sZOAUyUfeWUJSlRAD0,2350
 sparseml/exporters/transforms/base_transform.py,sha256=IpvdUdEADl2SfqHawcp6-lcNgz-R3L0zpS05WaWF5h8,2333
 sparseml/exporters/transforms/constants_to_initializers.py,sha256=_PX3y16OC-q85d-6DeOOVpKAAMNIU1m5BdYTZlFV_tk,1388
-sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=9z2HRqJAM68HPiSfu2RMyrn93dr8HCTpMcMrh_1-x2w,3866
+sparseml/exporters/transforms/conv_to_convinteger_add_cast_mul.py,sha256=x_Y8i9izPyIxX59P3i6rd324yA-o__FWdmwMIuU0_Ng,4630
 sparseml/exporters/transforms/conv_to_qlinearconv.py,sha256=CwCXtIBCOQ1qX5Z2JZhsdXSDk683wRCIBILF_1vd0GI,5838
 sparseml/exporters/transforms/delete_repeated_qdq.py,sha256=YiIOrvKqrxYboOA4A8YTbQIQ4s4MDdmqeLNYHPP4kjs,2440
 sparseml/exporters/transforms/delete_trivial_onnx_adds.py,sha256=St3-PQP8tPXYoyQTFn8fvJi7JF3LoX9Vb9nc-Zbx4Wg,1842
 sparseml/exporters/transforms/flatten_qparams.py,sha256=u0POagPJ_sqaS-DMe2x1Fd40RdlS9nYlLFZqHdsXx4Y,2181
 sparseml/exporters/transforms/fold_conv_div_bn.py,sha256=ckYdMKO2Z31NKRxQk4C4EbMWlVrsuhUDtyeMTMTErE4,3553
 sparseml/exporters/transforms/fold_identity_initializers.py,sha256=Yfv46MvL_vMxNGmUYSvlbucbrWIIDnjWnifmFCzyILA,1669
 sparseml/exporters/transforms/fold_relu_quants.py,sha256=qDGl-6aGmaQ8lAii3v0NvqkjbqtZB1UgHEkd3RzvjXQ,2070
 sparseml/exporters/transforms/gemm_to_matmulinteger_add_cast_mul.py,sha256=r1oVnnu-U0mISkqBJrebXO1o-cmbkSMbo1X4xA0l-t4,4418
 sparseml/exporters/transforms/gemm_to_qlinearmatmul.py,sha256=ccrB80ymufz6c9znwIGz0rxvM6U-vmKqiCa7l0vKYfE,7629
 sparseml/exporters/transforms/initializers_to_uint8.py,sha256=GxveAKe1xSNBZh1hjUx61veL6LTf9Msnx663Mrhvtxg,1645
-sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=Fry6n_u6KMG6mwnrekP5nj5eHYL-T-SPFcjz6E6LUU4,4866
+sparseml/exporters/transforms/matmul_add_to_matmulinteger_add_cast_mul.py,sha256=Oy-SVeqb1ZCZGhH8WAt7GPu2ivGoi9KigSbn71sb9JY,6297
 sparseml/exporters/transforms/matmul_to_matmulinteger_cast_mul.py,sha256=5vPDFN9YHC5-0LYhv5_GI4ZBBRwYfPMhgv3MZEIUBqE,4681
 sparseml/exporters/transforms/matmul_to_qlinearmatmul.py,sha256=Siii4mZ3LtqWY1blD1KT7ePVJud1oyLDrcr21YosU7E,4156
 sparseml/exporters/transforms/onnx_transform.py,sha256=vqlJJTjqZx9IUV3woHjKnWQMl2w-iurZK2eGABhYX9M,3724
-sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=XTEiUTX5nzLUtndGs_0t7nTgjIad-FyjuNc0O4f6Xro,3398
+sparseml/exporters/transforms/propagate_dequant_through_split.py,sha256=PVRL5ZG03axXrTyGDhmcA1Lx8nXkAj8HK3Sx1W1tMKE,3433
+sparseml/exporters/transforms/propagate_embedding_quantization.py,sha256=MlTJOOM7yDvqy-UTa3y5aFTCjCFmEloDkTA-5Xc_xak,4801
 sparseml/exporters/transforms/quantize_qat_embedding.py,sha256=_v1dEEt5vCSaMF6dJkg9fVGof145-_Lmo0DMjpXsnUE,4464
 sparseml/exporters/transforms/quantize_residuals.py,sha256=f3kNF930ymHI5CmCA0OmYW7vDKvEm9sYhN0UX0UC1EQ,3869
 sparseml/exporters/transforms/remove_duplicate_qconv_weights.py,sha256=mod-7bnlkg20LjerZ7tKKmp_7XyO3FKo13BtIZkDsmM,3331
 sparseml/exporters/transforms/remove_duplicate_quantize_ops.py,sha256=2FSXzaY3jdxOgj3xBaUOUqtk-hzg4kwhheELhoOKpS8,2545
 sparseml/exporters/transforms/skip_input_quantize.py,sha256=ANiYDwSos9gPW4960fMwmGubTDgpAcqFVSIHKf_ffYw,3210
 sparseml/exporters/transforms/unwrap_batchnorms.py,sha256=ly7GHCXN_2r8Gnk8PABWCqcoS-NL3GMfquEK0hRlFCs,1373
 sparseml/exporters/transforms/kv_cache/__init__.py,sha256=6wiIglqacQ56SO_4i5zemLL3VcUfTfJA-AMc5gOHmOE,909
-sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=PEN6NU9huZEgPkWpN-hpmYq-mfRDkbRWyoN8ozklsaY,26599
-sparseml/exporters/transforms/kv_cache/configs.py,sha256=yLIZpF2d90hoeXo-lqPlmSe7wuxXeq1DhroQ_BGOxZQ,6192
+sparseml/exporters/transforms/kv_cache/cache_keys_and_values.py,sha256=e6DEXx7Sm5kLxtapuGDFt7YfQt4-9rT0Wei8iXVxerQ,26610
+sparseml/exporters/transforms/kv_cache/configs.py,sha256=kxNTtjPW66S3rG6WkUvZ4NdneT2eTt0gvHX64pWVO1w,6523
 sparseml/exporters/transforms/kv_cache/positions_adjustment_base.py,sha256=bSiZF-U4LRoBxJfnSGXLlaG1pL5MzNPXlzmbDvAXtFw,1660
 sparseml/exporters/transforms/kv_cache/positions_adjustment_codegen.py,sha256=1FSG9npk_R0UK56fap-yRvSjNs5RWRejXJI4fYFD3lk,3377
 sparseml/exporters/transforms/kv_cache/positions_adjustment_opt.py,sha256=d3xqHqbxdRbLIEi5ebXaRwPauvsMjdLPLuRpYyx_DsM,4951
 sparseml/exporters/transforms/utils/__init__.py,sha256=tXSSUnzdyIc_H73xQ5dYhHb1Gj4Nb7GLLDVwJds8c_s,730
 sparseml/exporters/transforms/utils/add_quantized_conv_matmul_add_ops.py,sha256=I6kugQ0J9yHxCz7Yx3TlxQTUxcaAko4XkBDsQD7v5eo,10570
 sparseml/exporters/transforms/utils/helpers.py,sha256=vkEYL2Bdp_YNXlPg_TGd82Q2ef1EYEr11LVgmORQDiY,6457
 sparseml/exporters/transforms/utils/matching.py,sha256=CnVJLbJARBJwvFjoKh9vwYt6dLP4WXG3p7nCY5VUFaE,14429
@@ -129,15 +130,15 @@
 sparseml/pytorch/base.py,sha256=8HUpCMuP7gg6s4nvJVHU15AksGH5yhWLfeAMW6XvW18,6155
 sparseml/pytorch/opset.py,sha256=-BsKarkkKfq09HYJLZfxt_AEHEfuENpRDZF_J2va1Ck,933
 sparseml/pytorch/torch_to_onnx_exporter.py,sha256=HHgmXDopADURZcO50F5pX2wNffQGykWkwy0aTYw2H0U,10884
 sparseml/pytorch/datasets/__init__.py,sha256=2xoH_fCMojldFY1RCWSkt9pGfa8SzHAxU5em-_ZiwV8,998
 sparseml/pytorch/datasets/generic.py,sha256=nl-fFlpd7u5sNswe1AORZvQUne3sqrrPWnNgOUp6_Fc,4193
 sparseml/pytorch/datasets/registry.py,sha256=Ju8hAl3qkaplvkjZgt6WvpKmujgv0qJ690Buo1ekipg,3014
 sparseml/pytorch/datasets/classification/__init__.py,sha256=GMKhziJkRwSC7E_1Nox8FxnxhPFozZ6MxQWUWi1BN_Y,828
-sparseml/pytorch/datasets/classification/cifar.py,sha256=k32Z552YrrJv7IlshH8AWylaRKCOUC8KSrzRLLTHTag,4017
+sparseml/pytorch/datasets/classification/cifar.py,sha256=o6KRltIr6tSjaxy0BXsc0QosjMdCmx0sxfxocBEMEhw,4457
 sparseml/pytorch/datasets/classification/imagefolder.py,sha256=rOvwqy2Zp89VkT7zat2hQxRmgPyvCpSAhZ4mWEsL9JI,3669
 sparseml/pytorch/datasets/classification/imagenet.py,sha256=CHzsckzsSsUCLR-oxaxJ8NH7j4WBqg_Wg5ge27bPk5Q,4000
 sparseml/pytorch/datasets/classification/imagenette.py,sha256=cac2poejwyNyVUsxw4odSTmmrEkJ0AoIkDqDapAINnQ,6491
 sparseml/pytorch/datasets/classification/mnist.py,sha256=hDmxt2oCugMIuhtUPn8m4f811t-BdZx9cxjPiarZuxo,2434
 sparseml/pytorch/datasets/detection/__init__.py,sha256=RgS6mZ9-uAgaJ9GAgt40QI-kKl-gpLJf96MTrMUnd74,767
 sparseml/pytorch/datasets/detection/coco.py,sha256=s9dL59xBIkKH3lvXDmTD-9SKCtTt3i6lgFgbLl26N0I,16159
 sparseml/pytorch/datasets/detection/helpers.py,sha256=geEPIIsy1PuVxQRZi9xTopvSVAgLwSg9xSmYK1iucvs,5705
@@ -223,15 +224,15 @@
 sparseml/pytorch/sparsification/pruning/scorer.py,sha256=8gyYSv611GOJwmpQeD7FsWVrLxF8jeM_f59zhQlC6f8,4644
 sparseml/pytorch/sparsification/quantization/__init__.py,sha256=OjbeCzzhoeFJEJQvLmXZc89pghO83sLRhmvNF7_q_oQ,813
 sparseml/pytorch/sparsification/quantization/constants.py,sha256=sla-j0QwLFq92AbDZkHkNLxugpGrNEQJIuLWoWqV3Ks,2220
 sparseml/pytorch/sparsification/quantization/helpers.py,sha256=MmY5iOMlBUBEMrotPyj3H5drzpXhf13v4FJjb1N2aaw,32271
 sparseml/pytorch/sparsification/quantization/legacy_modifier_quantization.py,sha256=TToI4dGYZZEzB1q61m1YVg0THlvH7Ew1CZ2y-ajpTts,33626
 sparseml/pytorch/sparsification/quantization/modifier_quantization.py,sha256=LkHNB1IsiFlZugUecB4-LZMjWuoboFYf_PXPx6uPl1g,26778
 sparseml/pytorch/sparsification/quantization/quantization_scheme.py,sha256=10KNttNCHqUTNq706kPB6k7u6mvvfV0WTvx5D5Uqd-Y,12558
-sparseml/pytorch/sparsification/quantization/quantize.py,sha256=bqqH2qBEWYHfea5jzAHmz52uPddfRdmP3TFaCKgQqjM,17905
+sparseml/pytorch/sparsification/quantization/quantize.py,sha256=5vM57jjD2HuQjsYT7P1ayfpLJbXRthrI_Frlh1BELZQ,18014
 sparseml/pytorch/sparsification/quantization/quantize_qat_export.py,sha256=6JLbd3NUy9J0_pygSypJZsPtfxLlY8ZFJfK7kJSRrSY,76796
 sparseml/pytorch/sparsification/training/__init__.py,sha256=4GGhQf6KVSOYwtr_WL9Xcvx4mR-k8yKMVI_zuTBHGO4,790
 sparseml/pytorch/sparsification/training/modifier_epoch.py,sha256=_5p1EZk2qbwTnWsMXbVan3vRj1IRyIM4wYYZdLGA5GE,1778
 sparseml/pytorch/sparsification/training/modifier_logging.py,sha256=K1NMqhea5EBPko6yim8CThShbiSJKN5P_ca_TCyZXto,2883
 sparseml/pytorch/sparsification/training/modifier_lr.py,sha256=m_tCydo_BHiXCHMUKZu6iqKLAP24acAT8-NLjH9RIlE,24287
 sparseml/pytorch/sparsification/training/modifier_params.py,sha256=G_0eVqu0Cup8WNLFhkfPmYnKtJlNrxcJt0FcOOdq9tA,21497
 sparseml/pytorch/sparsification/training/modifier_regularizer.py,sha256=ezHbcwI8ITgq4vwkzsWXgnq_ls6NONW_D8jEN-YR7u8,6690
@@ -318,25 +319,25 @@
 sparseml/tensorflow_v1/utils/loss.py,sha256=4AsXh70fjp1dDcxBUzgjjpLgndwVa1CBiMG1sYi5Was,1974
 sparseml/tensorflow_v1/utils/nets_utils.py,sha256=cOTKgw7PVPEjRVU-bvcsNLdBJGTi-A7djJaUaZQwsT4,8119
 sparseml/tensorflow_v1/utils/summary.py,sha256=A2ub7KDwzsaindIuCHa7N3cRpCU6d7QbD5uNHV-R6H8,1327
 sparseml/tensorflow_v1/utils/variable.py,sha256=6ziLaNOLnxQrSPWJ2RaINqg4w-4NK9reVJWH-weK3-k,12536
 sparseml/transformers/__init__.py,sha256=8J1vljjZiybTTdNXN9e9senxvZUmKXKHAB5-H4D_4nY,1511
 sparseml/transformers/export.py,sha256=A0f4AhzegFco-rHJ0ySO51MrNpzQhsrtMR_IXs-i1_0,22048
 sparseml/transformers/masked_language_modeling.py,sha256=xV1H7jyWCWMKTiow501cI498I5ouNC68nF7g-QNuzjw,30756
-sparseml/transformers/question_answering.py,sha256=E_Ljec9bNDrZ2KD3unTlbcRxEpyYU6C9asuEynhh4AQ,36557
+sparseml/transformers/question_answering.py,sha256=AZnC7mlibBPijps7yCbqVPj8voJOCQJ4rECt29FIZwg,36976
 sparseml/transformers/text_classification.py,sha256=UYCpgSGTkmeGOeePQF5Idd8uY4GHQc-ShZK5SFOlP7E,40299
 sparseml/transformers/token_classification.py,sha256=6RUe1CmXQv7dHsE35aTg-xLW1g4BGakRp6pn0un2_mE,34350
 sparseml/transformers/sparsification/__init__.py,sha256=22XZNePvLFXNxp5NrcUIXzjgynCZm6jvQOErpRGlQNY,833
 sparseml/transformers/sparsification/question_answering.py,sha256=FAXhtQ8MW_2ar1dix2tQ1x1RXZuSWMLHZbVHToNWwmo,19529
 sparseml/transformers/sparsification/trainer.py,sha256=d_jRopQvHB0n-3uskpTHbqbnYFCiO7GocJ4iiujUW8s,44413
 sparseml/transformers/sparsification/training_args.py,sha256=gGivIDchLi__PZMNQRmzDOaQcQLkUVFystq3LaVko3Y,1890
 sparseml/transformers/utils/__init__.py,sha256=dxyg6b2XznhBzOsduHdOalgTmoX1JC32Rb4AHns6rVk,794
 sparseml/transformers/utils/helpers.py,sha256=pgxtf0ygP7qJEVPse_dGxm7UpWSJ9JVebA_ex1c8Muw,3090
 sparseml/transformers/utils/metrics.py,sha256=ciZsxgdrzlSMnyzbgKOFE3spWsKql0z82BiYFRXiVOU,2536
-sparseml/transformers/utils/model.py,sha256=JRq-p0CqKlWLdbhD9e8V2YkFtSZ6xLE9B512TTR8d2M,17072
+sparseml/transformers/utils/model.py,sha256=HxS1pMag21A4CHPwgcDHZIysA6LvY_RQwIQe0J7hOZ8,17074
 sparseml/utils/__init__.py,sha256=-WKBN4DERhw7rTJkarilkyAM9pw4rW8qkXGRPSEJ8SM,844
 sparseml/utils/frameworks.py,sha256=S-cGkbVc6DoWfI6Hu5AkIqF0Vi1PyxKX5GfhwRfpv_E,886
 sparseml/utils/helpers.py,sha256=qaooDtSTHgwLTjyfavDR7xPyS2mi26fGzla9VcHWJZg,26562
 sparseml/utils/restricted_eval.py,sha256=bBScMel61Cl3OcXs1TvxQgao1P2cJgmeDHeLSHF5Cqg,3983
 sparseml/utils/singleton.py,sha256=SbOoiw_CW7d9TEYIcvfb_ueaAD4iKbURZiTlBfM173g,1083
 sparseml/utils/worker.py,sha256=swoPegdTmV8nYbyie2WUytLLdwaK9skjx4RejHD3cww,6312
 sparseml/utils/wrapper.py,sha256=xrhPKRrXajQtDGIS--ZZxLsvnVTnnP0vlcnt_Tyd--g,2952
@@ -360,16 +361,16 @@
 sparseml/yolov8/export.py,sha256=BN4KFsrYYEfpU8e7icW4rQr4uR4lioNXlY3MII9ecKw,2502
 sparseml/yolov8/modules.py,sha256=j-8TGWMY5-pnEDt-uj1akERLt5zcjK11aN6Bnh1Clrg,2259
 sparseml/yolov8/train.py,sha256=DeZMrZ_moAc3fIojJloq3IvQqiPC_cgPgTjYFSOoG7E,7194
 sparseml/yolov8/trainers.py,sha256=6jr1v056lTlZy8DmPstQosAAIq6-Wj39gdHUoQABzQk,35999
 sparseml/yolov8/val.py,sha256=hlFImvknSpV1nONOxA3ivYgvzm64EmK0_Lh-JHLbOsw,2748
 sparseml/yolov8/validators.py,sha256=ytG7g_LOXvKFmxLPmQloT-wNf78convSoRRXVTYCR0Y,8196
 sparseml/yolov8/utils/__init__.py,sha256=6JekgnibQP-8p8Dm1dGiIEGCGdBOAkSOnEds0BMSYhQ,685
-sparseml/yolov8/utils/export_samples.py,sha256=CF4pF4FnQndQQgidfE_CNIRhR4hPoF_fZuPW6R2LLnk,6172
+sparseml/yolov8/utils/export_samples.py,sha256=Zy26etoYraN7k6IInS_i0j3RfoIzeeoK6JD-xFjkRk4,6247
 sparseml/yolov8/utils/helpers.py,sha256=8JZNaTT1zPKiZaOccmMtQu5mXCSMGkq8BDEgUqaPVIs,4041
-sparseml_nightly-1.6.0.20230707.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-sparseml_nightly-1.6.0.20230707.dist-info/METADATA,sha256=lTlIbYrG8hPbO5uEj5jN5BvuM_eQ0nRGU7smwv8xoe8,21782
-sparseml_nightly-1.6.0.20230707.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
-sparseml_nightly-1.6.0.20230707.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
-sparseml_nightly-1.6.0.20230707.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
-sparseml_nightly-1.6.0.20230707.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
-sparseml_nightly-1.6.0.20230707.dist-info/RECORD,,
+sparseml_nightly-1.6.0.20230717.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+sparseml_nightly-1.6.0.20230717.dist-info/METADATA,sha256=Lrgw8ijKNfD_rsKdBbKL71l2seM9wlusXtkCxwQ-TrE,21837
+sparseml_nightly-1.6.0.20230717.dist-info/NOTICE,sha256=4XaU0pCaSBt7sTZ5qA0WEn0jzOHUEL4FR52UEea4G3w,2158
+sparseml_nightly-1.6.0.20230717.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+sparseml_nightly-1.6.0.20230717.dist-info/entry_points.txt,sha256=UzbZv_wFWQuS0zGUhVxcLWzT_T2Ef9_brFWIy9POI-0,2326
+sparseml_nightly-1.6.0.20230717.dist-info/top_level.txt,sha256=JOOlWKgkyuJBScnty7pC1SQ58fOo1ONbslvMdxB6L2M,9
+sparseml_nightly-1.6.0.20230717.dist-info/RECORD,,
```

