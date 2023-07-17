# Comparing `tmp/deepspeed-0.9.4.tar.gz` & `tmp/deepspeed-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepspeed-0.9.4.tar", last modified: Fri Jun  9 18:43:47 2023, max compression
+gzip compressed data, was "deepspeed-0.9.5.tar", last modified: Thu Jun 22 17:19:29 2023, max compression
```

## Comparing `deepspeed-0.9.4.tar` & `deepspeed-0.9.5.tar`

### file list

```diff
@@ -1,638 +1,636 @@
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.806864 deepspeed-0.9.4/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.4/LICENSE
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.4/MANIFEST.in
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27751 2023-06-09 18:43:47.806864 deepspeed-0.9.4/PKG-INFO
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    26821 2023-06-09 18:33:23.000000 deepspeed-0.9.4/README.md
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/cpu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/accelerator/npu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.4/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/bin/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/deepspeed
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/deepspeed.pt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.4/bin/ds_bench
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.4/bin/ds_elastic
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds_report
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/ds_ssh
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.4/bin/dsr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:46.000000 deepspeed-0.9.4/build.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.254364 deepspeed-0.9.4/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.276030 deepspeed-0.9.4/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.286864 deepspeed-0.9.4/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/cpu/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.297697 deepspeed-0.9.4/csrc/cpu/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/cpu/comm/ccl.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.330197 deepspeed-0.9.4/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.4/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.341030 deepspeed-0.9.4/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.341030 deepspeed-0.9.4/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.351863 deepspeed-0.9.4/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.373530 deepspeed-0.9.4/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.4/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.4/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.243530 deepspeed-0.9.4/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.384364 deepspeed-0.9.4/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/pointwise_ops.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/rms_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.4/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed/accelerator/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/accelerator/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/abstract_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/cpu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/cuda_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/accelerator/npu_accelerator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/accelerator/real_accelerator.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.406030 deepspeed-0.9.4/deepspeed/autotuning/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54184 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/autotuner.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.406030 deepspeed-0.9.4/deepspeed/autotuning/config_templates/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero0.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero1.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero2.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.4/deepspeed/autotuning/config_templates/template_zero3.json
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5943 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.416864 deepspeed-0.9.4/deepspeed/autotuning/tuner/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2754 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/base_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/cost_model.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/index_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/model_based_tuner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/autotuning/tuner/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15053 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/autotuning/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.427697 deepspeed-0.9.4/deepspeed/checkpoint/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/checkpoint/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12012 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/checkpoint/deepspeed_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_3d_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_meg_2d.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/reshape_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/universal_checkpoint.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2534 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/checkpoint/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/checkpoint/zero_checkpoint.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.438530 deepspeed-0.9.4/deepspeed/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/comm/backend.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2248 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/ccl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27788 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/comm/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1276 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      259 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/comm/reduce_op.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13416 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/comm/torch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/comm/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.460197 deepspeed-0.9.4/deepspeed/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36033 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11886 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/compress.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25067 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5569 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14637 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8161 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7818 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/compression/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.460197 deepspeed-0.9.4/deepspeed/elasticity/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4703 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/elasticity/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2454 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/elasticity/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/elastic_agent.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/elasticity.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/elasticity/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/env_report.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/git_version_info.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      790 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed/git_version_info_installed.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9501 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/inference/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    31552 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/inference/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/launcher/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/launcher/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      375 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/launcher/constants.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14654 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/launcher/launch.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16568 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/launcher/multinode_runner.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24146 2023-06-09 18:38:25.000000 deepspeed-0.9.4/deepspeed/launcher/runner.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.471030 deepspeed-0.9.4/deepspeed/model_implementations/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.481864 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/diffusers/vae.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.481864 deepspeed-0.9.4/deepspeed/model_implementations/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/features/cuda_graph.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.492697 deepspeed-0.9.4/deepspeed/model_implementations/transformers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/clip_encoder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8247 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.503530 deepspeed-0.9.4/deepspeed/module_inject/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4998 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/auto_tp.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.514364 deepspeed-0.9.4/deepspeed/module_inject/containers/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      893 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13091 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/base_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3690 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/bert.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5289 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/bloom.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2822 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/clip.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3109 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/distil_bert.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/module_inject/containers/features/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      275 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4788 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/gated_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7273 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4129 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1200 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/megatron.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2930 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/meta_tensor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7136 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/features/split_qkv.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2221 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gpt2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4768 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptj.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5002 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptneo.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5571 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/gptneox.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5797 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/llama.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5017 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3936 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6599 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/opt.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/unet.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/containers/vae.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/inject.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4592 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/layers.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14597 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/load_checkpoint.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/module_inject/module_quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8259 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    44312 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/replace_module.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      989 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/replace_policy.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1762 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/module_inject/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/moe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/experts.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/mappings.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/sharded_moe.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/moe/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.525197 deepspeed-0.9.4/deepspeed/monitor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2485 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/monitor/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/csv_monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/monitor.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/tensorboard.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/monitor/wandb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/nebula/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/nebula/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/nebula/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/nebula/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/ops/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.536030 deepspeed-0.9.4/deepspeed/ops/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adagrad/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adagrad/cpu_adagrad.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/adam/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adam/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8544 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/adam/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8767 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/adam/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/adam/multi_tensor_apply.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/aio/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/aio/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/adam/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/cpu_adam.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/aio/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.546864 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_test/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_test/single_process_config.json
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/common/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.557697 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/ccl.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.568530 deepspeed-0.9.4/deepspeed/ops/csrc/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/StopWatch.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/Timer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/compat.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6957 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/conversion_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adagrad.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adam.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/custom_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/dequantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/dropout.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_kernel_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/feed_forward.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/gelu.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/gemm_test.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/general_kernels.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/memory_access_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/normalize_layer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantizer.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/reduction_utils.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/simd.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/softmax.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/strided_batch_gemm.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/includes/type_shim.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.568530 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/fake_quantizer.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/quantization/quantize.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/token_sort.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/utils.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/dropout_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/gelu_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/general_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.265197 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.579364 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85817 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10280 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/normalize_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/softmax_kernels.cu
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/transformer/transform_kernels.cu
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/csrc/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.590197 deepspeed-0.9.4/deepspeed/ops/lamb/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/lamb/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/lamb/fused_lamb.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.601030 deepspeed-0.9.4/deepspeed/ops/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/builder.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/no_impl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/quantizer/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/quantizer/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/quantizer/quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.611864 deepspeed-0.9.4/deepspeed/ops/random_ltd/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/random_ltd/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4902 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/random_ltd/dropping_utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.622697 deepspeed-0.9.4/deepspeed/ops/sparse_attention/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/matmul.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_attention_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_self_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42463 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparsity_config.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.633530 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/matmul.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.633530 deepspeed-0.9.4/deepspeed/ops/transformer/
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.644364 deepspeed-0.9.4/deepspeed/ops/transformer/inference/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/bias_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5725 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9830 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4853 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13853 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_attention.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6212 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_mlp.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18454 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/moe_inference.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      536 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/base.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1496 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1404 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/linear.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4472 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3129 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2660 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/residual_add.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2460 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2131 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1447 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/inference/triton_ops.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/ops/transformer/transformer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/pipe/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/profiling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/profiling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1959 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1243 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.655197 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47248 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/profiling/flops_profiler/profiler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.687697 deepspeed-0.9.4/deepspeed/runtime/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/__init__.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.698530 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/checkpointing.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18559 2023-04-21 00:47:36.000000 deepspeed-0.9.4/deepspeed/runtime/bf16_optimizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.698530 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      653 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4975 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/comm/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/coalesced_collectives.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/mpi.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/comm/nccl.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/compression/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/compression/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/compression/cupy.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39863 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/config.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/config_utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12971 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/constants.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.709364 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.720197 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/helper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.720197 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25023 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/dataloader.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/eigenvalue.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   155219 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/engine.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.731030 deepspeed-0.9.4/deepspeed/runtime/fp16/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/__init__.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/fused_optimizer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11492 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/loss_scaler.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.741864 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/zoadam.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/fp16/unfused_optimizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21045 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/hybrid_engine.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/lr_schedules.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.752697 deepspeed-0.9.4/deepspeed/runtime/pipe/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56845 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/engine.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/module.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/p2p.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/schedule.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/pipe/topology.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/progressive_layer_drop.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/quantize.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/sparse_tensor.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/state_dict_factory.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.763530 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/aio_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/async_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/constants.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/optimizer_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/swap_tensor/utils.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35805 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/weight_quantizer.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.785197 deepspeed-0.9.4/deepspeed/runtime/zero/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/contiguous_memory_allocator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/linear.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21984 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/mics.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/mics_utils.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/offload_config.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22194 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/zero/parameter_offload.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    73213 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/partition_parameters.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22674 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/partitioned_param_coordinator.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)   115761 2023-06-09 18:33:23.000000 deepspeed-0.9.4/deepspeed/runtime/zero/stage3.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110843 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/runtime/zero/stage_1_and_2.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/test.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/runtime/zero/tiling.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/runtime/zero/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/deepspeed/utils/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      751 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/comms_logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/debug.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/exceptions.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/groups.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/init_on_device.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/logging.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/mixed_precision_linkage.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5158 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/numa.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/nvtx.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.4/deepspeed/utils/tensor_fragment.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     9477 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/timer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      434 2023-06-02 22:08:07.000000 deepspeed-0.9.4/deepspeed/utils/types.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.4/deepspeed/utils/zero_to_fp32.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.395197 deepspeed-0.9.4/deepspeed.egg-info/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27751 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/PKG-INFO
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21258 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/SOURCES.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/dependency_links.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/entry_points.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1146 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/requires.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-06-09 18:43:46.000000 deepspeed-0.9.4/deepspeed.egg-info/top_level.txt
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/op_builder/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/all_ops.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/async_io.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.4/op_builder/builder.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.796030 deepspeed-0.9.4/op_builder/cpu/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/__init__.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.4/op_builder/cpu/builder.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/comm.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/cpu/no_impl.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/cpu_adagrad.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/cpu_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/fused_adam.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/fused_lamb.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/quantizer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/random_ltd.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.4/op_builder/sparse_attn.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/spatial_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/stochastic_transformer.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/transformer.py
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.4/op_builder/transformer_inference.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      431 2023-04-11 17:18:49.000000 deepspeed-0.9.4/op_builder/utils.py
-drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-09 18:43:47.806864 deepspeed-0.9.4/requirements/
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-1bit-mpi.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-autotuning-ml.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-autotuning.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       28 2023-06-02 22:08:07.000000 deepspeed-0.9.4/requirements/requirements-cpu.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.4/requirements/requirements-dev.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.4/requirements/requirements-inf.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.4/requirements/requirements-readthedocs.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.4/requirements/requirements-sd.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.4/requirements/requirements-sparse_attn.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       25 2023-06-02 22:08:07.000000 deepspeed-0.9.4/requirements/requirements-sparse_pruning.txt
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.4/requirements/requirements.txt
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-06-09 18:43:47.806864 deepspeed-0.9.4/setup.cfg
--rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11424 2023-06-02 22:08:07.000000 deepspeed-0.9.4/setup.py
--rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-06-02 22:13:07.000000 deepspeed-0.9.4/version.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.835791 deepspeed-0.9.5/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11357 2023-04-11 17:18:49.000000 deepspeed-0.9.5/LICENSE
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      290 2023-02-28 00:54:52.000000 deepspeed-0.9.5/MANIFEST.in
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28217 2023-06-22 17:19:29.835791 deepspeed-0.9.5/PKG-INFO
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    27287 2023-06-22 17:11:08.000000 deepspeed-0.9.5/README.md
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.629958 deepspeed-0.9.5/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.5/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.5/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.5/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.5/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.5/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.5/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.629958 deepspeed-0.9.5/bin/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/deepspeed
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/deepspeed.pt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      106 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/ds
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      757 2022-08-05 18:43:48.000000 deepspeed-0.9.5/bin/ds_bench
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1869 2023-04-11 17:18:49.000000 deepspeed-0.9.5/bin/ds_elastic
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/ds_report
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      680 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/ds_ssh
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      109 2022-07-06 20:47:37.000000 deepspeed-0.9.5/bin/dsr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.000000 deepspeed-0.9.5/build.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.597458 deepspeed-0.9.5/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.629958 deepspeed-0.9.5/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.640791 deepspeed-0.9.5/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.597458 deepspeed-0.9.5/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.640791 deepspeed-0.9.5/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.640791 deepspeed-0.9.5/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.640791 deepspeed-0.9.5/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.597458 deepspeed-0.9.5/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.640791 deepspeed-0.9.5/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.651624 deepspeed-0.9.5/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7207 2023-06-20 00:07:13.000000 deepspeed-0.9.5/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.5/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.5/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.5/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.5/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.5/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.651624 deepspeed-0.9.5/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.5/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.597458 deepspeed-0.9.5/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.5/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.5/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.5/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.5/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.597458 deepspeed-0.9.5/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85902 2023-06-20 00:07:13.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10531 2023-06-20 00:07:13.000000 deepspeed-0.9.5/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.5/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.5/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.662458 deepspeed-0.9.5/deepspeed/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14304 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.673291 deepspeed-0.9.5/deepspeed/accelerator/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      214 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/accelerator/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4607 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/accelerator/abstract_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7140 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/accelerator/cpu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8389 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/accelerator/cuda_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6893 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/accelerator/npu_accelerator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6791 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/accelerator/real_accelerator.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.673291 deepspeed-0.9.5/deepspeed/autotuning/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      129 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    54187 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/autotuning/autotuner.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4633 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.673291 deepspeed-0.9.5/deepspeed/autotuning/config_templates/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       48 2022-07-06 20:47:37.000000 deepspeed-0.9.5/deepspeed/autotuning/config_templates/template_zero0.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      113 2022-07-06 20:47:37.000000 deepspeed-0.9.5/deepspeed/autotuning/config_templates/template_zero1.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      237 2022-07-06 20:47:37.000000 deepspeed-0.9.5/deepspeed/autotuning/config_templates/template_zero2.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      485 2022-07-06 20:47:37.000000 deepspeed-0.9.5/deepspeed/autotuning/config_templates/template_zero3.json
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5943 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/autotuning/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    15644 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.673291 deepspeed-0.9.5/deepspeed/autotuning/tuner/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      235 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2754 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/base_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1820 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/cost_model.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1158 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/index_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5614 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/model_based_tuner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2329 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/autotuning/tuner/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15053 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/autotuning/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.684124 deepspeed-0.9.5/deepspeed/checkpoint/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      561 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2429 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/checkpoint/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12012 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/checkpoint/deepspeed_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4674 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/reshape_3d_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7885 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/reshape_meg_2d.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2888 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/reshape_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4888 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/universal_checkpoint.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2534 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/checkpoint/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5316 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/checkpoint/zero_checkpoint.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.684124 deepspeed-0.9.5/deepspeed/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      137 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1416 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/comm/backend.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2248 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/comm/ccl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27798 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/comm/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      855 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/comm/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1276 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/comm/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      259 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/comm/reduce_op.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13416 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/comm/torch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3684 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/comm/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.684124 deepspeed-0.9.5/deepspeed/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      243 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    36033 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11886 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/compress.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25067 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5569 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14637 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8161 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7818 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/compression/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      733 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/elasticity/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      383 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/elasticity/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4703 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/elasticity/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2454 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/elasticity/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7762 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/elasticity/elastic_agent.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17374 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/elasticity/elasticity.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      459 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/elasticity/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/env_report.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      756 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/git_version_info.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      759 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed/git_version_info_installed.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9501 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/inference/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    31552 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/inference/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/launcher/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/launcher/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      375 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/launcher/constants.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    14654 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/launcher/launch.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    16568 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/launcher/multinode_runner.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    24146 2023-06-09 18:38:25.000000 deepspeed-0.9.5/deepspeed/launcher/runner.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/model_implementations/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      220 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/model_implementations/diffusers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/diffusers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2792 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/diffusers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6025 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/diffusers/vae.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.694958 deepspeed-0.9.5/deepspeed/model_implementations/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      563 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/features/cuda_graph.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.705791 deepspeed-0.9.5/deepspeed/model_implementations/transformers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3045 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/clip_encoder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      388 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      667 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      669 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      682 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      665 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8247 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.705791 deepspeed-0.9.5/deepspeed/module_inject/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      444 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4998 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/auto_tp.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.716624 deepspeed-0.9.5/deepspeed/module_inject/containers/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      893 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13091 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5756 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/base_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3690 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/bert.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5289 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/bloom.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2822 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/clip.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3109 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/distil_bert.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.716624 deepspeed-0.9.5/deepspeed/module_inject/containers/features/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      275 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4804 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/gated_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7281 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/hybrid_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4129 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/hybrid_megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1200 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/megatron.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2930 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/meta_tensor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7136 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/features/split_qkv.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2221 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/gpt2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4768 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/gptj.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5002 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/gptneo.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5571 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/gptneox.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5797 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/llama.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5017 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/megatron_gpt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3936 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/megatron_gpt_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6599 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/opt.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1732 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/unet.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1163 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/containers/vae.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     4719 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/inject.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4592 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/layers.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14597 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/load_checkpoint.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3107 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/module_inject/module_quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8259 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    44312 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/replace_module.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      989 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/replace_policy.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1762 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/module_inject/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.716624 deepspeed-0.9.5/deepspeed/moe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1223 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/experts.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6082 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3529 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/mappings.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20621 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/sharded_moe.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5214 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/moe/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.716624 deepspeed-0.9.5/deepspeed/monitor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2485 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/monitor/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2907 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/csv_monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1604 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/monitor.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2227 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/tensorboard.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      754 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1150 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/monitor/wandb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.716624 deepspeed-0.9.5/deepspeed/nebula/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/nebula/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1764 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/nebula/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2786 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/nebula/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      477 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      141 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/adagrad/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5089 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/adagrad/cpu_adagrad.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/adam/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      169 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/adam/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8544 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/adam/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8767 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/adam/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      429 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/adam/multi_tensor_apply.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/aio/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      136 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/aio/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.619124 deepspeed-0.9.5/deepspeed/ops/csrc/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/adagrad/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8438 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/adam/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10428 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/adam/cpu_adam.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      880 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6573 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/adam/multi_tensor_adam.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5595 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.608291 deepspeed-0.9.5/deepspeed/ops/csrc/aio/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13040 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1364 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2033 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1402 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4330 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2086 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2707 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1427 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1240 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      722 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4326 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1052 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2459 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4422 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1246 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1805 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_test/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      359 2021-08-17 18:54:40.000000 deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_test/single_process_config.json
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/common/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1278 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/common/custom_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.608291 deepspeed-0.9.5/deepspeed/ops/csrc/cpu/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.727457 deepspeed-0.9.5/deepspeed/ops/csrc/cpu/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7446 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/cpu/comm/ccl.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.738291 deepspeed-0.9.5/deepspeed/ops/csrc/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1981 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/StopWatch.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/Timer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      336 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/compat.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7207 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12402 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/conversion_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5615 2023-04-13 15:29:56.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/cpu_adagrad.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8137 2023-04-13 15:29:56.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/cpu_adam.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3277 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13156 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/custom_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7301 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2195 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/dropout.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1155 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/ds_kernel_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6164 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/ds_transformer_cuda.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3189 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/feed_forward.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1018 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/gelu.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10326 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/gemm_test.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1507 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/general_kernels.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    33966 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7089 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/normalize_layer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2293 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/quantization.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17370 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/quantization_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      346 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/quantizer.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18641 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/reduction_utils.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4526 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/simd.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1642 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/softmax.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6807 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/strided_batch_gemm.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6388 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/includes/type_shim.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.738291 deepspeed-0.9.5/deepspeed/ops/csrc/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4002 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15291 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.738291 deepspeed-0.9.5/deepspeed/ops/csrc/quantization/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3302 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/quantization/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    37581 2023-04-13 15:29:56.000000 deepspeed-0.9.5/deepspeed/ops/csrc/quantization/fake_quantizer.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5784 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6988 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/quantization/quantize.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.738291 deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8408 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/gather_scatter.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9590 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5076 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/token_sort.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.749124 deepspeed-0.9.5/deepspeed/ops/csrc/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4523 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/sparse_attention/utils.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.619124 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.749124 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6273 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3863 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.749124 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      915 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.749124 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17572 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/cublas_wrappers.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29835 2023-04-13 15:29:56.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/dropout_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    47589 2023-04-13 15:29:56.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12191 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/gelu_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    14520 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/general_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.619124 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.759957 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7781 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5009 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28641 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20883 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2476 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    85902 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2318 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10251 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27245 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    30233 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.759957 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10531 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18517 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     8904 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    74900 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/normalize_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    26758 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/softmax_kernels.cu
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22709 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/transformer/transform_kernels.cu
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.759957 deepspeed-0.9.5/deepspeed/ops/csrc/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      788 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/csrc/utils/flatten_unflatten.cpp
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.759957 deepspeed-0.9.5/deepspeed/ops/lamb/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      130 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/lamb/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7815 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/lamb/fused_lamb.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/op_builder/transformer_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/quantizer/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      132 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/quantizer/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1193 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/quantizer/quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/random_ltd/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      191 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/random_ltd/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4902 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/random_ltd/dropping_utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/sparse_attention/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      467 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3463 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    32948 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/matmul.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11322 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    12300 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparse_attention_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6746 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparse_self_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    42463 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparsity_config.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1032 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6628 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/matmul.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1923 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4047 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.770791 deepspeed-0.9.5/deepspeed/ops/transformer/
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)      413 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.781624 deepspeed-0.9.5/deepspeed/ops/transformer/inference/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      315 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      876 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/bias_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5725 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      236 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/diffusers_2d_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9830 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/diffusers_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4853 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/diffusers_transformer_block.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    13853 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/ds_attention.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6212 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/ds_mlp.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18454 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/moe_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.781624 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      382 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      536 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/base.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1496 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1404 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/linear.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4472 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3129 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2704 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/residual_add.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2460 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/softmax.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2131 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/softmax_context.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1447 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4434 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/inference/triton_ops.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20600 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/ops/transformer/transformer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.781624 deepspeed-0.9.5/deepspeed/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      164 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/pipe/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.781624 deepspeed-0.9.5/deepspeed/profiling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/profiling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1959 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/profiling/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1243 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/profiling/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.781624 deepspeed-0.9.5/deepspeed/profiling/flops_profiler/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      120 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/profiling/flops_profiler/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    51515 2023-06-22 17:11:08.000000 deepspeed-0.9.5/deepspeed/profiling/flops_profiler/profiler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      192 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/__init__.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    32764 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/checkpointing.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3987 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18534 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/runtime/bf16_optimizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      653 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4975 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1060 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/comm/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/comm/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3698 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/comm/coalesced_collectives.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10062 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/comm/mpi.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7712 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/comm/nccl.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/compression/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/compression/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      701 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/compression/cupy.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    39863 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/config.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     8199 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/config_utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    12971 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/constants.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6081 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4701 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10025 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/curriculum_scheduler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5638 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1282 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/helper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4638 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/scheduler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      955 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.792457 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    25023 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19160 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    20614 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1756 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6977 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/dataloader.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     5625 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/eigenvalue.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   155150 2023-06-22 17:19:05.000000 deepspeed-0.9.5/deepspeed/runtime/engine.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.803291 deepspeed-0.9.5/deepspeed/runtime/fp16/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      140 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/__init__.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    20052 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/fused_optimizer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11492 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/loss_scaler.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.803291 deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      186 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15258 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    23085 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    19112 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/zoadam.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18076 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/fp16/unfused_optimizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21045 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/hybrid_engine.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    33557 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/lr_schedules.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.803291 deepspeed-0.9.5/deepspeed/runtime/pipe/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      195 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    56845 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/engine.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    27186 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/module.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5477 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/p2p.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15546 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/schedule.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17167 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/pipe/topology.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     1353 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/progressive_layer_drop.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     7699 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/quantize.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2416 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/sparse_tensor.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    18177 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/state_dict_factory.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.814124 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       95 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1172 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/aio_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6282 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/async_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      596 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/constants.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    18967 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/optimizer_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     9654 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    17684 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10793 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7734 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/swap_tensor/utils.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    35805 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7027 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/weight_quantizer.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.824957 deepspeed-0.9.5/deepspeed/runtime/zero/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      452 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/runtime/zero/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10113 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/runtime/zero/config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    10926 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/zero/contiguous_memory_allocator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7403 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/runtime/zero/linear.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    21984 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/runtime/zero/mics.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7500 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/runtime/zero/mics_utils.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2931 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/zero/offload_config.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22194 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/runtime/zero/parameter_offload.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    73213 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/runtime/zero/partition_parameters.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    22674 2023-06-09 18:33:23.000000 deepspeed-0.9.5/deepspeed/runtime/zero/partitioned_param_coordinator.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)   115736 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/runtime/zero/stage3.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)   110818 2023-06-20 00:07:13.000000 deepspeed-0.9.5/deepspeed/runtime/zero/stage_1_and_2.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2727 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/zero/test.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    11727 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/runtime/zero/tiling.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     3033 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/runtime/zero/utils.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.824957 deepspeed-0.9.5/deepspeed/utils/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      751 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/utils/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     6096 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/comms_logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4370 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/debug.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      144 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/exceptions.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    15606 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/groups.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3004 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/init_on_device.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     4375 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/logging.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2041 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/mixed_precision_linkage.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     5158 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/utils/numa.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      499 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/nvtx.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     7997 2023-04-11 17:18:49.000000 deepspeed-0.9.5/deepspeed/utils/tensor_fragment.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     9477 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/utils/timer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      434 2023-06-02 22:08:07.000000 deepspeed-0.9.5/deepspeed/utils/types.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    23607 2023-05-03 17:31:31.000000 deepspeed-0.9.5/deepspeed/utils/zero_to_fp32.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.673291 deepspeed-0.9.5/deepspeed.egg-info/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    28217 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/PKG-INFO
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    21204 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/SOURCES.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        1 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/dependency_links.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       85 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/entry_points.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1146 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/requires.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       10 2023-06-22 17:19:29.000000 deepspeed-0.9.5/deepspeed.egg-info/top_level.txt
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.835791 deepspeed-0.9.5/op_builder/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1990 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1180 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/all_ops.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     3333 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/async_io.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)    29637 2023-06-09 18:33:23.000000 deepspeed-0.9.5/op_builder/builder.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.835791 deepspeed-0.9.5/op_builder/cpu/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      217 2023-06-02 22:08:07.000000 deepspeed-0.9.5/op_builder/cpu/__init__.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1224 2023-06-09 18:33:23.000000 deepspeed-0.9.5/op_builder/cpu/builder.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1225 2023-06-02 22:08:07.000000 deepspeed-0.9.5/op_builder/cpu/comm.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      616 2023-06-02 22:08:07.000000 deepspeed-0.9.5/op_builder/cpu/no_impl.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1420 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/cpu_adagrad.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1397 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/cpu_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1044 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/fused_adam.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1216 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/fused_lamb.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      805 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/quantizer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1079 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/random_ltd.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     2994 2023-04-21 00:47:36.000000 deepspeed-0.9.5/op_builder/sparse_attn.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1534 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/spatial_inference.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      565 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/stochastic_transformer.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)     1294 2023-04-11 17:18:49.000000 deepspeed-0.9.5/op_builder/transformer.py
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)     2745 2023-06-02 22:08:07.000000 deepspeed-0.9.5/op_builder/transformer_inference.py
+drwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        0 2023-06-22 17:19:29.835791 deepspeed-0.9.5/requirements/
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        7 2022-07-06 20:47:37.000000 deepspeed-0.9.5/requirements/requirements-1bit-mpi.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       23 2022-07-06 20:47:37.000000 deepspeed-0.9.5/requirements/requirements-autotuning-ml.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)        9 2022-07-06 20:47:37.000000 deepspeed-0.9.5/requirements/requirements-autotuning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       28 2023-06-02 22:08:07.000000 deepspeed-0.9.5/requirements/requirements-cpu.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      213 2023-05-03 17:31:31.000000 deepspeed-0.9.5/requirements/requirements-dev.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       72 2023-02-28 00:54:52.000000 deepspeed-0.9.5/requirements/requirements-inf.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       97 2023-04-21 00:47:36.000000 deepspeed-0.9.5/requirements/requirements-readthedocs.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)       36 2023-04-11 17:18:49.000000 deepspeed-0.9.5/requirements/requirements-sd.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       14 2022-07-06 20:47:37.000000 deepspeed-0.9.5/requirements/requirements-sparse_attn.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       25 2023-06-02 22:08:07.000000 deepspeed-0.9.5/requirements/requirements-sparse_pruning.txt
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)       78 2023-04-21 00:47:36.000000 deepspeed-0.9.5/requirements/requirements.txt
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)      148 2023-06-22 17:19:29.835791 deepspeed-0.9.5/setup.cfg
+-rwxr-xr-x   0 jerasley  (1000) jerasley  (1000)    11424 2023-06-02 22:08:07.000000 deepspeed-0.9.5/setup.py
+-rw-r--r--   0 jerasley  (1000) jerasley  (1000)        6 2023-06-09 18:44:10.000000 deepspeed-0.9.5/version.txt
```

### Comparing `deepspeed-0.9.4/LICENSE` & `deepspeed-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/PKG-INFO` & `deepspeed-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.4
+Version: 0.9.5
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -29,14 +29,16 @@
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
 [![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
+[![Japanese Twitter](https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9ETwitter-%40MSFTDeepSpeedJP-blue)](https://twitter.com/MSFTDeepSpeedJP)
+[![Chinese Zhihu](https://img.shields.io/badge/%E7%9F%A5%E4%B9%8E-%E5%BE%AE%E8%BD%AFDeepSpeed-blue)](https://www.zhihu.com/people/deepspeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -133,15 +135,15 @@
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
 | ----------- | ------ |
-| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
+| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-h100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
 | AMD | [![amd-mi100](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml) [![amd-mi200](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml) |
 | CPU | [![nv-torch-latest-cpu](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml) |
 | PyTorch Nightly | [![nv-torch-nightly-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml) |
 | Integrations | [![nv-transformers-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml) [![nv-lightning-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml) [![nv-accelerate-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml)[![nv-megatron](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml)[![nv-mii](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml) |
 | Misc | [![Formatting](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml) [![pages-build-deployment](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment) [![Documentation Status](https://readthedocs.org/projects/deepspeed/badge/?version=latest)](https://deepspeed.readthedocs.io/en/latest/?badge=latest)[![python](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml) |
 
 # Installation
```

### Comparing `deepspeed-0.9.4/README.md` & `deepspeed-0.9.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
 [![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
+[![Japanese Twitter](https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9ETwitter-%40MSFTDeepSpeedJP-blue)](https://twitter.com/MSFTDeepSpeedJP)
+[![Chinese Zhihu](https://img.shields.io/badge/%E7%9F%A5%E4%B9%8E-%E5%BE%AE%E8%BD%AFDeepSpeed-blue)](https://www.zhihu.com/people/deepspeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -103,15 +105,15 @@
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
 | ----------- | ------ |
-| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
+| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-h100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
 | AMD | [![amd-mi100](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml) [![amd-mi200](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml) |
 | CPU | [![nv-torch-latest-cpu](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml) |
 | PyTorch Nightly | [![nv-torch-nightly-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml) |
 | Integrations | [![nv-transformers-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml) [![nv-lightning-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml) [![nv-accelerate-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml)[![nv-megatron](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml)[![nv-mii](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml) |
 | Misc | [![Formatting](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml) [![pages-build-deployment](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment) [![Documentation Status](https://readthedocs.org/projects/deepspeed/badge/?version=latest)](https://deepspeed.readthedocs.io/en/latest/?badge=latest)[![python](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml) |
 
 # Installation
```

### Comparing `deepspeed-0.9.4/accelerator/abstract_accelerator.py` & `deepspeed-0.9.5/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/accelerator/cpu_accelerator.py` & `deepspeed-0.9.5/accelerator/cpu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/accelerator/cuda_accelerator.py` & `deepspeed-0.9.5/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/accelerator/npu_accelerator.py` & `deepspeed-0.9.5/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/accelerator/real_accelerator.py` & `deepspeed-0.9.5/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/bin/ds_bench` & `deepspeed-0.9.5/bin/ds_bench`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/bin/ds_elastic` & `deepspeed-0.9.5/bin/ds_elastic`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/bin/ds_ssh` & `deepspeed-0.9.5/bin/ds_ssh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.5/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.5/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.5/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.5/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.5/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.5/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.5/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.5/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.5/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/cpu/comm/ccl.cpp` & `deepspeed-0.9.5/csrc/cpu/comm/ccl.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/StopWatch.h` & `deepspeed-0.9.5/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/Timer.h` & `deepspeed-0.9.5/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/context.h` & `deepspeed-0.9.5/csrc/includes/context.h`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,20 @@
 
 class TrainingContext {
 public:
     TrainingContext() : _workspace(nullptr), _seed(42), _curr_offset(0)
     {
         curandCreateGenerator(&_gen, CURAND_RNG_PSEUDO_DEFAULT);
         curandSetPseudoRandomGeneratorSeed(_gen, 123);
-        if (cublasCreate(&_cublasHandle) != CUBLAS_STATUS_SUCCESS) {
-            auto message = std::string("Fail to create cublas handle.");
+        cublasStatus_t stat = cublasCreate(&_cublasHandle);
+        if (stat != CUBLAS_STATUS_SUCCESS) {
+            // It would be nice to use cublasGetStatusName and
+            // cublasGetStatusString, but they were only added in CUDA 11.4.2.
+            auto message = std::string("Failed to create cublas handle: cublasStatus_t was ") +
+                           std::to_string(stat);
             std::cerr << message << std::endl;
             throw std::runtime_error(message);
         }
     }
 
     virtual ~TrainingContext()
     {
```

### Comparing `deepspeed-0.9.4/csrc/includes/conversion_utils.h` & `deepspeed-0.9.5/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.5/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/cpu_adam.h` & `deepspeed-0.9.5/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.5/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.5/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.5/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/dropout.h` & `deepspeed-0.9.5/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.5/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.5/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/feed_forward.h` & `deepspeed-0.9.5/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/gelu.h` & `deepspeed-0.9.5/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/gemm_test.h` & `deepspeed-0.9.5/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/general_kernels.h` & `deepspeed-0.9.5/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.5/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/normalize_layer.h` & `deepspeed-0.9.5/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/quantization.h` & `deepspeed-0.9.5/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/quantization_utils.h` & `deepspeed-0.9.5/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/reduction_utils.h` & `deepspeed-0.9.5/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/simd.h` & `deepspeed-0.9.5/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/softmax.h` & `deepspeed-0.9.5/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.5/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/includes/type_shim.h` & `deepspeed-0.9.5/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.5/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.5/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/quantization/dequantize.cu` & `deepspeed-0.9.5/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.5/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.5/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/quantization/quantize.cu` & `deepspeed-0.9.5/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.5/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.5/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.5/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.5/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.5/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.5/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.5/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.5/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.5/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.5/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/pointwise_ops.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/pointwise_ops.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1105,16 +1105,17 @@
                        .dtype(input_cont.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
     int head_size = input_cont.size(2) / num_heads;
     int bsz = input.size(0) * input.size(1);
+    int out_size = transposed_mode ? weight.size(0) : weight.size(1);
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
-    auto output = at::from_blob(workspace, {input.size(0), input.size(1), weight.size(1)}, options);
+    auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
 
     float alpha = (T)1.0;
     float gemm_beta = (T)0.0;
     cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
                     InferenceContext::Instance().GetCurrentStream());
 
     cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
@@ -1309,15 +1310,15 @@
                             bool transposed_mode)
 {
     auto options = at::TensorOptions()
                        .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
-    int out_size = q_int8 ? weight.size(0) : weight.size(1);
+    int out_size = (q_int8 || transposed_mode) ? weight.size(0) : weight.size(1);
     int bsz = input.size(0) * input.size(1);
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
     if (q_int8) {
         quantized_gemm<T>(output.data_ptr(),
                           (T*)input.data_ptr(),
```

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/rms_norm.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.5/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.5/csrc/transformer/inference/includes/inference_context.h`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,21 @@
           _free_memory_size(0),
           _num_tokens(1),
           _attention_unfused_workspace_offset(0),
           _workSpaceSize(0)
     {
         _workSpaceSize = 0;
         _workspace = 0;
-        if (cublasCreate(&_cublasHandle) != CUBLAS_STATUS_SUCCESS) {
-            auto message = std::string("Fail to create cublas handle.");
+
+        cublasStatus_t stat = cublasCreate(&_cublasHandle);
+        if (stat != CUBLAS_STATUS_SUCCESS) {
+            // It would be nice to use cublasGetStatusName and
+            // cublasGetStatusString, but they were only added in CUDA 11.4.2.
+            auto message = std::string("Failed to create cublas handle: cublasStatus_t was ") +
+                           std::to_string(stat);
             std::cerr << message << std::endl;
             throw std::runtime_error(message);
         }
 #ifndef __HIP_PLATFORM_HCC__
         cublasSetMathMode(_cublasHandle, CUBLAS_TENSOR_OP_MATH);
 #endif
         cudaEventCreate(&_comp1_event);
```

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.5/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.5/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.5/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.5/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/__init__.py` & `deepspeed-0.9.5/deepspeed/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/accelerator/abstract_accelerator.py` & `deepspeed-0.9.5/deepspeed/accelerator/abstract_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/accelerator/cpu_accelerator.py` & `deepspeed-0.9.5/deepspeed/accelerator/cpu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/accelerator/cuda_accelerator.py` & `deepspeed-0.9.5/deepspeed/accelerator/cuda_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/accelerator/npu_accelerator.py` & `deepspeed-0.9.5/deepspeed/accelerator/npu_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/accelerator/real_accelerator.py` & `deepspeed-0.9.5/deepspeed/accelerator/real_accelerator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/autotuner.py` & `deepspeed-0.9.5/deepspeed/autotuning/autotuner.py`

 * *Files 0% similar despite different names*

```diff
@@ -981,15 +981,15 @@
     def get_gas_from_user_config(self):
         gas = 1
         if GRADIENT_ACCUMULATION_STEPS in self.user_config:
             gas_in_config = self.user_config[GRADIENT_ACCUMULATION_STEPS]
             if isinstance(gas_in_config, int):
                 gas = gas_in_config
             elif gas_in_config == "auto":  # GRADIENT_ACCUMULATION_STEPS: "auto"
-                val = self.get_val_from_config(GRADIENT_ACCUMULATION_STEPS)
+                val = self.get_val_from_user_args(GRADIENT_ACCUMULATION_STEPS)
                 if val:
                     gas = int(val)
             elif isinstance(gas_in_config, list):
                 logger.info(
                     f"Specifying a list of {GRADIENT_ACCUMULATION_STEPS} to tune is not supported. 1 would be used.")
         assert gas > 0, "Gradient accumulation steps must be positive."
         return gas
```

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/config.py` & `deepspeed-0.9.5/deepspeed/autotuning/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/constants.py` & `deepspeed-0.9.5/deepspeed/autotuning/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/scheduler.py` & `deepspeed-0.9.5/deepspeed/autotuning/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/tuner/base_tuner.py` & `deepspeed-0.9.5/deepspeed/autotuning/tuner/base_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/tuner/cost_model.py` & `deepspeed-0.9.5/deepspeed/autotuning/tuner/cost_model.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/tuner/index_based_tuner.py` & `deepspeed-0.9.5/deepspeed/autotuning/tuner/index_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/tuner/model_based_tuner.py` & `deepspeed-0.9.5/deepspeed/autotuning/tuner/model_based_tuner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/tuner/utils.py` & `deepspeed-0.9.5/deepspeed/autotuning/tuner/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/autotuning/utils.py` & `deepspeed-0.9.5/deepspeed/autotuning/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/__init__.py` & `deepspeed-0.9.5/deepspeed/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/constants.py` & `deepspeed-0.9.5/deepspeed/checkpoint/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/deepspeed_checkpoint.py` & `deepspeed-0.9.5/deepspeed/checkpoint/deepspeed_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/reshape_3d_utils.py` & `deepspeed-0.9.5/deepspeed/checkpoint/reshape_3d_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/reshape_meg_2d.py` & `deepspeed-0.9.5/deepspeed/checkpoint/reshape_meg_2d.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/reshape_utils.py` & `deepspeed-0.9.5/deepspeed/checkpoint/reshape_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/universal_checkpoint.py` & `deepspeed-0.9.5/deepspeed/checkpoint/universal_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/utils.py` & `deepspeed-0.9.5/deepspeed/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/checkpoint/zero_checkpoint.py` & `deepspeed-0.9.5/deepspeed/checkpoint/zero_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/comm/backend.py` & `deepspeed-0.9.5/deepspeed/comm/backend.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/comm/ccl.py` & `deepspeed-0.9.5/deepspeed/comm/ccl.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     print(f'DeepSpeed {builder.absolute_name()} built successfully')
     return ccl_cpp_module
 
 
 class CCLBackend(TorchBackend):
 
     def __init__(self, name='ccl', rank=-1, world_size=-1, mpu=None, timeout=None, init_method=None):
+        self.ccl_comm_op = build_ccl_op()
+        if self.ccl_comm_op == None:
+            # set CCLBackend to uninitialized state if CCLCommBuilder cannot be loaded
+            self.initialized = False
+            return
         super(CCLBackend, self).__init__(backend='ccl',
                                          name='torch',
                                          rank=rank,
                                          world_size=world_size,
                                          timeout=timeout,
                                          init_method=init_method)
         self.name = 'ccl'
-        self.ccl_comm_op = build_ccl_op()
-        if self.ccl_comm_op == None:
-            # set CCLBackend to uninitialized state if CCLCommBuilder cannot be loaded
-            self.initialized = False
-            return
         size = self.get_world_size()
         rank = self.get_rank()
         main_kvs = self.ccl_comm_op.get_kvs_addr(rank)
         main_kvs = torch.tensor(main_kvs).to(torch.uint8)
         super(CCLBackend, self).broadcast(main_kvs, 0)
         self.ccl_comm_op.initialize(size, rank, main_kvs)
         self.initialized = True
```

### Comparing `deepspeed-0.9.4/deepspeed/comm/comm.py` & `deepspeed-0.9.5/deepspeed/comm/comm.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,16 +141,16 @@
 # UNUSED: Future helper function to initialize DS backends
 def init_deepspeed_backend(ds_backend, timeout, init_method):
     global cdb
     global nccl_backend
     global mpi_backend
     global ccl_backend
 
-    rank = int(os.environ["RANK"])
-    size = int(os.environ["WORLD_SIZE"])
+    rank = int(os.getenv('RANK', '-1'))
+    size = int(os.getenv('WORLD_SIZE', '-1'))
 
     if ds_backend == NCCL_BACKEND:
         utils.logger.warn("NCCL backend in DeepSpeed not yet implemented")
     elif ds_backend == MPI_BACKEND:
         utils.logger.warn("MPI backend in DeepSpeed not yet implemented")
     elif ds_backend == GLOO_BACKEND:
         utils.logger.warn("Gloo backend in DeepSpeed not yet implemented")
```

### Comparing `deepspeed-0.9.4/deepspeed/comm/config.py` & `deepspeed-0.9.5/deepspeed/comm/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/comm/constants.py` & `deepspeed-0.9.5/deepspeed/comm/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/comm/torch.py` & `deepspeed-0.9.5/deepspeed/comm/torch.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/comm/utils.py` & `deepspeed-0.9.5/deepspeed/comm/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/basic_layer.py` & `deepspeed-0.9.5/deepspeed/compression/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/compress.py` & `deepspeed-0.9.5/deepspeed/compression/compress.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/config.py` & `deepspeed-0.9.5/deepspeed/compression/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/constants.py` & `deepspeed-0.9.5/deepspeed/compression/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/helper.py` & `deepspeed-0.9.5/deepspeed/compression/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/scheduler.py` & `deepspeed-0.9.5/deepspeed/compression/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/compression/utils.py` & `deepspeed-0.9.5/deepspeed/compression/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/constants.py` & `deepspeed-0.9.5/deepspeed/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/elasticity/config.py` & `deepspeed-0.9.5/deepspeed/elasticity/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/elasticity/constants.py` & `deepspeed-0.9.5/deepspeed/elasticity/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/elasticity/elastic_agent.py` & `deepspeed-0.9.5/deepspeed/elasticity/elastic_agent.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/elasticity/elasticity.py` & `deepspeed-0.9.5/deepspeed/elasticity/elasticity.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/env_report.py` & `deepspeed-0.9.5/deepspeed/env_report.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/git_version_info.py` & `deepspeed-0.9.5/deepspeed/git_version_info.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/git_version_info_installed.py` & `deepspeed-0.9.5/deepspeed/git_version_info_installed.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-version='0.9.4'
+version='0.9.5'
 git_hash='unknown'
 git_branch='unknown'
-installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False, 'utils': False}
-compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True, 'utils': True}
+installed_ops={'async_io': False, 'cpu_adagrad': False, 'cpu_adam': False, 'fused_adam': False, 'fused_lamb': False, 'quantizer': False, 'random_ltd': False, 'sparse_attn': False, 'spatial_inference': False, 'transformer': False, 'stochastic_transformer': False, 'transformer_inference': False}
+compatible_ops={'async_io': False, 'cpu_adagrad': True, 'cpu_adam': True, 'fused_adam': True, 'fused_lamb': True, 'quantizer': True, 'random_ltd': True, 'sparse_attn': False, 'spatial_inference': True, 'transformer': True, 'stochastic_transformer': True, 'transformer_inference': True}
 torch_info={'version': '1.9', 'bf16_support': False, 'cuda_version': '10.2', 'nccl_version': '2.7', 'hip_version': '0.0'}
```

### Comparing `deepspeed-0.9.4/deepspeed/inference/config.py` & `deepspeed-0.9.5/deepspeed/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/inference/engine.py` & `deepspeed-0.9.5/deepspeed/inference/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/launcher/launch.py` & `deepspeed-0.9.5/deepspeed/launcher/launch.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/launcher/multinode_runner.py` & `deepspeed-0.9.5/deepspeed/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/launcher/runner.py` & `deepspeed-0.9.5/deepspeed/launcher/runner.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/diffusers/unet.py` & `deepspeed-0.9.5/deepspeed/model_implementations/diffusers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/diffusers/vae.py` & `deepspeed-0.9.5/deepspeed/model_implementations/diffusers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/features/cuda_graph.py` & `deepspeed-0.9.5/deepspeed/model_implementations/features/cuda_graph.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/clip_encoder.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/clip_encoder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bert.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_bloom.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_gpt.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_megatron_gpt.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_opt.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/model_implementations/transformers/ds_transformer.py` & `deepspeed-0.9.5/deepspeed/model_implementations/transformers/ds_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/auto_tp.py` & `deepspeed-0.9.5/deepspeed/module_inject/auto_tp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/__init__.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/base.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/base_moe.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/base_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/bert.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/bloom.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/bloom.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/clip.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/clip.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/distil_bert.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/distil_bert.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/gated_mlp.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/gated_mlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,16 @@
             self.inter_up_w.data = self._h4h_w[:self.inter_up_w.shape[0], :]
             self.inter_gate_w.data = self._h4h_w[self.inter_up_w.shape[0]:, :]
 
             if self.inter_up_b is not None:
                 self.inter_up_b.data = self._h4h_b[:self.inter_up_w.shape[0]] if self._h4h_b is not None else None
                 self.inter_gate_b.data = self._h4h_b[self.inter_up_w.shape[0]:] if self._h4h_b is not None else None
         else:
-            self.module.inter_up_w = self.inter_up_w
-            self.module.inter_up_b = self.inter_up_b
-            self.module.inter_gate_w = self.inter_gate_w
-            self.module.inter_gate_b = self.inter_gate_b
+            self.module.mlp.inter_up_w = self.inter_up_w
+            self.module.mlp.inter_up_b = self.inter_up_b
+            self.module.mlp.inter_gate_w = self.inter_gate_w
+            self.module.mlp.inter_gate_b = self.inter_gate_b
 
     def get_mlp_params(self):
         params = super().get_mlp_params()
         params.extend([self.inter_up_w, self.inter_up_b, self.inter_gate_w, self.inter_gate_b])
         return params
```

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_engine.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/hybrid_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         Delete module parameters if they exist and point them back to the container. The primary
         purpose of this is for TP-inference with ZeRO-3. In this scenario, we need to delete the
         parameters we've created for inference to free their memory.
         """
         general_params = [
             (self.module.attention.attn_ow, self.dense_w),
             (self.module.attention.attn_ob, self.dense_b),
-            (self.module.attn_nw, self.attn_nw),
-            (self.module.attn_nb, self.attn_nb),
+            (self.module.mlp.attn_nw, self.attn_nw),
+            (self.module.mlp.attn_nb, self.attn_nb),
             (self.module.norm_w, self.input_nw),
             (self.module.norm_b, self.input_nb),
         ]
 
         self._release_params(general_params)
 
         self.release_qkv()
```

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/hybrid_megatron.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/hybrid_megatron.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/megatron.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/megatron.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/meta_tensor.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/features/split_qkv.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/features/split_qkv.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/gpt2.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/gpt2.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/gptj.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/gptj.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/gptneo.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/gptneo.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/gptneox.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/gptneox.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/llama.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/llama.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/megatron_gpt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/megatron_gpt_moe.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/megatron_gpt_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/opt.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/opt.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/unet.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/unet.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/containers/vae.py` & `deepspeed-0.9.5/deepspeed/module_inject/containers/vae.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/inject.py` & `deepspeed-0.9.5/deepspeed/module_inject/inject.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/layers.py` & `deepspeed-0.9.5/deepspeed/module_inject/layers.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/load_checkpoint.py` & `deepspeed-0.9.5/deepspeed/module_inject/load_checkpoint.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/module_quantize.py` & `deepspeed-0.9.5/deepspeed/module_inject/module_quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/policy.py` & `deepspeed-0.9.5/deepspeed/module_inject/policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/replace_module.py` & `deepspeed-0.9.5/deepspeed/module_inject/replace_module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/replace_policy.py` & `deepspeed-0.9.5/deepspeed/module_inject/replace_policy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/module_inject/utils.py` & `deepspeed-0.9.5/deepspeed/module_inject/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/moe/experts.py` & `deepspeed-0.9.5/deepspeed/moe/experts.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/moe/layer.py` & `deepspeed-0.9.5/deepspeed/moe/layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/moe/mappings.py` & `deepspeed-0.9.5/deepspeed/moe/mappings.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/moe/sharded_moe.py` & `deepspeed-0.9.5/deepspeed/moe/sharded_moe.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/moe/utils.py` & `deepspeed-0.9.5/deepspeed/moe/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/config.py` & `deepspeed-0.9.5/deepspeed/monitor/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/csv_monitor.py` & `deepspeed-0.9.5/deepspeed/monitor/csv_monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/monitor.py` & `deepspeed-0.9.5/deepspeed/monitor/monitor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/tensorboard.py` & `deepspeed-0.9.5/deepspeed/monitor/tensorboard.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/utils.py` & `deepspeed-0.9.5/deepspeed/monitor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/monitor/wandb.py` & `deepspeed-0.9.5/deepspeed/monitor/wandb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/nebula/config.py` & `deepspeed-0.9.5/deepspeed/nebula/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/nebula/constants.py` & `deepspeed-0.9.5/deepspeed/nebula/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/adagrad/cpu_adagrad.py` & `deepspeed-0.9.5/deepspeed/ops/adagrad/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/adam/cpu_adam.py` & `deepspeed-0.9.5/deepspeed/ops/adam/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/adam/fused_adam.py` & `deepspeed-0.9.5/deepspeed/ops/adam/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/adagrad/cpu_adagrad.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/adam/cpu_adam.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/adam/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/adam/fused_adam_frontend.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_adam.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/adam/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh` & `deepspeed-0.9.5/deepspeed/ops/csrc/adam/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_common.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_types.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/common/deepspeed_aio_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_aio_thread.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_pin_tensor.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_aio_handle.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/deepspeed_py_copy.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/aio/py_lib/py_ds_aio.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/common/custom_cuda_kernel.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/common/custom_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/cpu/comm/ccl.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/cpu/comm/ccl.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/StopWatch.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/StopWatch.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/Timer.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/Timer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/context.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/context.h`

 * *Files 3% similar despite different names*

```diff
@@ -46,16 +46,20 @@
 
 class TrainingContext {
 public:
     TrainingContext() : _workspace(nullptr), _seed(42), _curr_offset(0)
     {
         curandCreateGenerator(&_gen, CURAND_RNG_PSEUDO_DEFAULT);
         curandSetPseudoRandomGeneratorSeed(_gen, 123);
-        if (cublasCreate(&_cublasHandle) != CUBLAS_STATUS_SUCCESS) {
-            auto message = std::string("Fail to create cublas handle.");
+        cublasStatus_t stat = cublasCreate(&_cublasHandle);
+        if (stat != CUBLAS_STATUS_SUCCESS) {
+            // It would be nice to use cublasGetStatusName and
+            // cublasGetStatusString, but they were only added in CUDA 11.4.2.
+            auto message = std::string("Failed to create cublas handle: cublasStatus_t was ") +
+                           std::to_string(stat);
             std::cerr << message << std::endl;
             throw std::runtime_error(message);
         }
     }
 
     virtual ~TrainingContext()
     {
```

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/conversion_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/conversion_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adagrad.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/cpu_adagrad.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cpu_adam.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/cublas_wrappers.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/custom_cuda_layers.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/custom_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/dequantization_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/dequantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/dropout.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/dropout.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_kernel_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/ds_kernel_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/ds_transformer_cuda.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/ds_transformer_cuda.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/feed_forward.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/feed_forward.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/gelu.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/gelu.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/gemm_test.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/gemm_test.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/general_kernels.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/general_kernels.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/memory_access_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/memory_access_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/normalize_layer.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/quantization.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/quantization_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/quantization_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/reduction_utils.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/reduction_utils.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/simd.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/simd.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/softmax.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/softmax.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/strided_batch_gemm.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/includes/type_shim.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/includes/type_shim.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/lamb/fused_lamb_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/lamb/fused_lamb_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/dequantize.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/quantization/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/fake_quantizer.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/quantization/fake_quantizer.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/pt_binding.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/quantization/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/quantization/quantize.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/quantization/quantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/gather_scatter.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/gather_scatter.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/pt_binding.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/slice_attn_masks.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/random_ltd/token_sort.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/random_ltd/token_sort.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/sparse_attention/utils.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/sparse_attention/utils.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/spatial/csrc/opt_bias_add.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/spatial/csrc/pt_binding.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/spatial/includes/spatial_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/cublas_wrappers.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/dropout_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/ds_transformer_cuda.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/gelu_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/gelu_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/general_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/apply_rotary_pos_emb.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/dequantize.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/gelu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/layer_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/pointwise_ops.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/pt_binding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1105,16 +1105,17 @@
                        .dtype(input_cont.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
 
     int head_size = input_cont.size(2) / num_heads;
     int bsz = input.size(0) * input.size(1);
+    int out_size = transposed_mode ? weight.size(0) : weight.size(1);
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
-    auto output = at::from_blob(workspace, {input.size(0), input.size(1), weight.size(1)}, options);
+    auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
 
     float alpha = (T)1.0;
     float gemm_beta = (T)0.0;
     cublasSetStream(InferenceContext::Instance().GetCublasHandle(),
                     InferenceContext::Instance().GetCurrentStream());
 
     cublas_gemm_ex(InferenceContext::Instance().GetCublasHandle(),
@@ -1309,15 +1310,15 @@
                             bool transposed_mode)
 {
     auto options = at::TensorOptions()
                        .dtype(input.options().dtype())
                        .layout(at::kStrided)
                        .device(at::kCUDA)
                        .requires_grad(false);
-    int out_size = q_int8 ? weight.size(0) : weight.size(1);
+    int out_size = (q_int8 || transposed_mode) ? weight.size(0) : weight.size(1);
     int bsz = input.size(0) * input.size(1);
 
     T* workspace = (T*)InferenceContext::Instance().GetWorkSpace();
     auto output = at::from_blob(workspace, {input.size(0), input.size(1), out_size}, options);
     if (q_int8) {
         quantized_gemm<T>(output.data_ptr(),
                           (T*)input.data_ptr(),
```

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/relu.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/rms_norm.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/softmax.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/csrc/transform.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_context.h`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,21 @@
           _free_memory_size(0),
           _num_tokens(1),
           _attention_unfused_workspace_offset(0),
           _workSpaceSize(0)
     {
         _workSpaceSize = 0;
         _workspace = 0;
-        if (cublasCreate(&_cublasHandle) != CUBLAS_STATUS_SUCCESS) {
-            auto message = std::string("Fail to create cublas handle.");
+
+        cublasStatus_t stat = cublasCreate(&_cublasHandle);
+        if (stat != CUBLAS_STATUS_SUCCESS) {
+            // It would be nice to use cublasGetStatusName and
+            // cublasGetStatusString, but they were only added in CUDA 11.4.2.
+            auto message = std::string("Failed to create cublas handle: cublasStatus_t was ") +
+                           std::to_string(stat);
             std::cerr << message << std::endl;
             throw std::runtime_error(message);
         }
 #ifndef __HIP_PLATFORM_HCC__
         cublasSetMathMode(_cublasHandle, CUBLAS_TENSOR_OP_MATH);
 #endif
         cudaEventCreate(&_comp1_event);
```

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/inference/includes/inference_cuda_layers.h`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/normalize_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/softmax_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/transformer/transform_kernels.cu` & `deepspeed-0.9.5/deepspeed/ops/csrc/transformer/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/csrc/utils/flatten_unflatten.cpp` & `deepspeed-0.9.5/deepspeed/ops/csrc/utils/flatten_unflatten.cpp`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/lamb/fused_lamb.py` & `deepspeed-0.9.5/deepspeed/ops/lamb/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/__init__.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/all_ops.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/async_io.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/builder.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/builder.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/comm.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu/no_impl.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/cpu/no_impl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adagrad.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/cpu_adam.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/fused_adam.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/fused_lamb.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/quantizer.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/random_ltd.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/sparse_attn.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/spatial_inference.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/stochastic_transformer.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/transformer.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/op_builder/transformer_inference.py` & `deepspeed-0.9.5/deepspeed/ops/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/quantizer/quantizer.py` & `deepspeed-0.9.5/deepspeed/ops/quantizer/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/random_ltd/dropping_utils.py` & `deepspeed-0.9.5/deepspeed/ops/random_ltd/dropping_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/bert_sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/matmul.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/softmax.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_attention_utils.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparse_attention_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparse_self_attention.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparse_self_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/sparsity_config.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/sparsity_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/__init__.py` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/matmul.tr` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/matmul.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/softmax_bwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr` & `deepspeed-0.9.5/deepspeed/ops/sparse_attention/trsrc/softmax_fwd.tr`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/bias_add.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/bias_add.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/config.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_attention.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/diffusers_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/diffusers_transformer_block.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/diffusers_transformer_block.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_attention.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/ds_attention.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/ds_mlp.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/ds_mlp.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/moe_inference.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/moe_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/base.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/base.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/gelu_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/linear.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/mlp_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/qkv_gemm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/residual_add.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/residual_add.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,19 @@
         try:
             if self.config.dtype in [torch.float16, torch.int8]:
                 self.residual_add_func = self.inference_module.residual_add_bias_fp16
             elif self.config.dtype == torch.bfloat16:
                 self.residual_add_func = self.inference_module.residual_add_bias_bf16
             else:
                 self.residual_add_func = self.inference_module.residual_add_bias_fp32
-            self._vector_add = self.inference_module._vector_add
         except AttributeError:
             self.residual_add_func = None
+        try:
+            self._vector_add = self.inference_module._vector_add
+        except AttributeError:
             self._vector_add = None
 
     def forward(self,
                 hidden_state: torch.Tensor,
                 residual: torch.Tensor,
                 add_bias: bool,
                 attention_output: Optional[torch.Tensor] = None,
```

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/softmax.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/softmax_context.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/softmax_context.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/op_binding/vector_matmul.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/inference/triton_ops.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/inference/triton_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/ops/transformer/transformer.py` & `deepspeed-0.9.5/deepspeed/ops/transformer/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/profiling/config.py` & `deepspeed-0.9.5/deepspeed/profiling/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/profiling/constants.py` & `deepspeed-0.9.5/deepspeed/profiling/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/profiling/flops_profiler/profiler.py` & `deepspeed-0.9.5/deepspeed/profiling/flops_profiler/profiler.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import torch.nn as nn
 import torch.nn.functional as F
 from functools import partial
 from typing import List, Optional
 from collections import OrderedDict
 import numpy as np
 from deepspeed.accelerator import get_accelerator
+from deepspeed.moe.layer import MoE
 
 Tensor = torch.Tensor
 
 module_flop_count = []
 module_mac_count = []
 old_functions = {}
 
@@ -153,18 +154,39 @@
 
     def reset_profile(self):
         """Resets the profiling.
 
         Adds or resets the extra attributes.
         """
 
+        def get_param_count_and_ep(param):
+            """
+            Return the number of parameters in the layer, whether the layer is an MoE layer,
+            and its expert parallelism size if so
+            """
+            prefix = 'ep_size_'
+            offset = len(prefix)
+            expert_parallelism = 0
+            if getattr(param, "group_name", "").startswith(prefix):
+                try:
+                    expert_parallelism = int(param.group_name[offset:])
+                except ValueError:
+                    pass
+            is_moe = expert_parallelism > 0
+            return param.numel(), is_moe, expert_parallelism
+
         def add_or_reset_attrs(module):
+            parameters = [get_param_count_and_ep(p) for p in module.parameters()]
             module.__flops__ = 0
             module.__macs__ = 0
-            module.__params__ = sum(p.numel() for p in module.parameters())
+            module.__params__ = sum(count for count, is_expert, _ in parameters if not is_expert)
+            module.__expert_params__ = sum(count for count, is_expert, _ in parameters if is_expert)
+            # number of expert parameters taking into account other expert parallel groups
+            module.__model_expert_params__ = sum(count * expert_parallelism
+                                                 for count, is_expert, expert_parallelism in parameters if is_expert)
             module.__start_time__ = 0
             module.__duration__ = 0
 
         self.model.apply(add_or_reset_attrs)
 
     def end_profile(self):
         """Ends profiling.
@@ -179,14 +201,18 @@
         def remove_profile_attrs(module):
             if hasattr(module, "__flops__"):
                 del module.__flops__
             if hasattr(module, "__macs__"):
                 del module.__macs__
             if hasattr(module, "__params__"):
                 del module.__params__
+            if hasattr(module, "__expert_params__"):
+                del module.__expert_params__
+            if hasattr(module, "__model_expert_params__"):
+                del module.__model_expert_params__
             if hasattr(module, "__start_time__"):
                 del module.__start_time__
             if hasattr(module, "__duration__"):
                 del module.__duration__
 
         self.model.apply(remove_profile_attrs)
 
@@ -223,23 +249,30 @@
         Returns:
             The latency of the model forward pass.
         """
         total_duration = get_module_duration(self.model)
         return duration_to_string(total_duration) if as_string else total_duration
 
     def get_total_params(self, as_string=False):
-        """Returns the total parameters of the model.
+        """Returns the total number of parameters stored per rank.
 
         Args:
             as_string (bool, optional): whether to output the parameters as string. Defaults to False.
 
         Returns:
-            The number of parameters in the model.
+            The total number of parameters stored per rank.
         """
-        return params_to_string(self.model.__params__) if as_string else self.model.__params__
+        total_params = self.model.__expert_params__ + self.model.__params__
+        return params_to_string(total_params) if as_string else total_params
+
+    def is_expert_tensor_parallelism_enabled(self):
+        for _, module in self.model.named_modules():
+            if isinstance(module, MoE) and hasattr(module, 'enable_expert_tensor_parallelism'):
+                return module.enable_expert_tensor_parallelism
+        return False
 
     def print_model_profile(self, profile_step=1, module_depth=-1, top_modules=1, detailed=True, output_file=None):
         """Prints the model graph with the measured profile attached to each module.
 
         Args:
             profile_step (int, optional): The global training step at which to profile. Note that warm up steps are needed for accurate time measurement.
             module_depth (int, optional): The depth of the model to which to print the aggregated module information. When set to -1, it prints information from the top to the innermost modules (the maximum depth).
@@ -261,14 +294,22 @@
             f = open(output_file, "w")
             sys.stdout = f
 
         total_flops = self.get_total_flops()
         total_macs = self.get_total_macs()
         total_duration = self.get_total_duration()
         total_params = self.get_total_params()
+        expert_tensor_parallelism = None  # silence the linters
+        total_model_expert_params = total_model_nonexpert_params = 0
+        if self.ds_engine:
+            total_model_nonexpert_params = self.model.__params__ * self.ds_engine.mp_world_size
+            if self.ds_engine.has_moe_layers:
+                expert_tensor_parallelism = self.is_expert_tensor_parallelism_enabled()
+                total_model_expert_params = self.model.__model_expert_params__ * (self.ds_engine.mp_world_size
+                                                                                  if expert_tensor_parallelism else 1)
 
         self.flops = total_flops
         self.macs = total_macs
         self.params = total_params
 
         print("\n-------------------------- DeepSpeed Flops Profiler --------------------------")
         print(f'Profile Summary at step {profile_step}:')
@@ -276,19 +317,27 @@
             "Notations:\ndata parallel size (dp_size), model parallel size(mp_size),\nnumber of parameters (params), number of multiply-accumulate operations(MACs),\nnumber of floating-point operations (flops), floating-point operations per second (FLOPS),\nfwd latency (forward propagation latency), bwd latency (backward propagation latency),\nstep (weights update latency), iter latency (sum of fwd, bwd and step latency)\n"
         )
         if self.ds_engine:
             print('{:<60}  {:<8}'.format('world size: ', self.ds_engine.world_size))
             print('{:<60}  {:<8}'.format('data parallel size: ', self.ds_engine.dp_world_size))
             print('{:<60}  {:<8}'.format('model parallel size: ', self.ds_engine.mp_world_size))
             print('{:<60}  {:<8}'.format('batch size per GPU: ', self.ds_engine.train_micro_batch_size_per_gpu()))
+            if self.ds_engine.has_moe_layers:
+                print('{:<60}  {:<8}'.format('expert tensor parallelism enabled: ', expert_tensor_parallelism))
 
         print('{:<60}  {:<8}'.format('params per gpu: ', params_to_string(total_params)))
-        print('{:<60}  {:<8}'.format(
-            'params of model = params per GPU * mp_size: ',
-            params_to_string(total_params * ((self.ds_engine.mp_world_size) if self.ds_engine else 1))))
+        if total_model_expert_params > 0:
+            print('{:<60}  {:<8}'.format('params of model: ',
+                                         params_to_string(total_model_nonexpert_params + total_model_expert_params)))
+            print('{:<60}  {:<8}'.format('   non-expert params of model: ',
+                                         params_to_string(total_model_nonexpert_params)))
+            print('{:<60}  {:<8}'.format('   expert params of model: ', params_to_string(total_model_expert_params)))
+        else:
+            print('{:<60}  {:<8}'.format('params of model = params per GPU * mp_size: ',
+                                         params_to_string(total_model_nonexpert_params)))
 
         print('{:<60}  {:<8}'.format('fwd MACs per GPU: ', macs_to_string(total_macs)))
 
         print('{:<60}  {:<8}'.format('fwd flops per GPU: ', num_to_string(total_flops)))
 
         print('{:<60}  {:<8}'.format(
             'fwd flops of model = fwd flops per GPU * mp_size: ',
@@ -319,15 +368,15 @@
             print('{:<60}  {:<8}'.format(f'FLOPS per GPU = {bwd_factor+1} * fwd flops per GPU / iter latency: ',
                                          flops_to_string((bwd_factor + 1) * total_flops / iter_latency)))
 
             samples_per_iter = self.ds_engine.train_micro_batch_size_per_gpu() * self.ds_engine.world_size
             print('{:<60}  {:<8.2f}'.format('samples/second: ', samples_per_iter / iter_latency))
 
         def flops_repr(module):
-            params = module.__params__
+            params = module.__params__ + module.__expert_params__
             flops = get_module_flops(module)
             macs = get_module_macs(module)
             items = [
                 params_to_string(params),
                 "{:.2%} Params".format(params / total_params if total_params else 0),
                 macs_to_string(macs),
                 "{:.2%} MACs".format(0.0 if total_macs == 0 else macs / total_macs),
@@ -393,15 +442,15 @@
             if module.__class__.__name__ not in info[curr_depth]:
                 info[curr_depth][module.__class__.__name__] = [
                     0,
                     0,
                     0,
                 ]  # macs, params, time
             info[curr_depth][module.__class__.__name__][0] += get_module_macs(module)
-            info[curr_depth][module.__class__.__name__][1] += module.__params__
+            info[curr_depth][module.__class__.__name__][1] += module.__params__ + module.__expert_params__
             info[curr_depth][module.__class__.__name__][2] += get_module_duration(module)
             has_children = len(module._modules.items()) != 0
             if has_children:
                 for child in module.children():
                     walk_module(child, curr_depth + 1, info)
 
         walk_module(self.model, 0, info)
@@ -494,17 +543,28 @@
     in_channels = input.shape[1]
     out_channels = weight.shape[0]
     kernel_dims = list(weight.shape[2:])
     input_dims = list(input.shape[2:])
 
     length = len(input_dims)
 
-    paddings = padding if type(padding) is tuple else (padding, ) * length
     strides = stride if type(stride) is tuple else (stride, ) * length
     dilations = dilation if type(dilation) is tuple else (dilation, ) * length
+    if isinstance(padding, str):
+        if padding == 'valid':
+            paddings = (0, ) * length
+        elif padding == 'same':
+            paddings = ()
+            for d, k in zip(dilations, kernel_dims):
+                total_padding = d * (k - 1)
+                paddings += (total_padding // 2, )
+    elif isinstance(padding, tuple):
+        paddings = padding
+    else:
+        paddings = (padding, ) * length
 
     output_dims = []
     for idx, input_dim in enumerate(input_dims):
         output_dim = (input_dim + 2 * paddings[idx] - (dilations[idx] *
                                                        (kernel_dims[idx] - 1) + 1)) // strides[idx] + 1
         output_dims.append(output_dim)
 
@@ -618,23 +678,31 @@
     eps: float = 1e-5,
 ):
     has_affine = weight is not None
     # estimation
     return input.numel() * (5 if has_affine else 4), 0
 
 
-def _upsample_flops_compute(input, **kwargs):
+def _upsample_flops_compute(*args, **kwargs):
+    input = args[0]
     size = kwargs.get('size', None)
+    if size is None and len(args) > 1:
+        size = args[1]
+
     if size is not None:
         if isinstance(size, tuple) or isinstance(size, list):
             return int(_prod(size)), 0
         else:
             return int(size), 0
+
     scale_factor = kwargs.get('scale_factor', None)
+    if scale_factor is None and len(args) > 2:
+        scale_factor = args[2]
     assert scale_factor is not None, "either size or scale_factor should be defined"
+
     flops = input.numel()
     if isinstance(scale_factor, tuple) and len(scale_factor) == len(input):
         flops * int(_prod(scale_factor))
     else:
         flops * scale_factor**len(input)
     return flops, 0
 
@@ -1108,28 +1176,27 @@
     duration = module.__duration__
     if duration == 0:  # e.g. ModuleList
         for m in module.children():
             duration += m.__duration__
     return duration
 
 
-def get_model_profile(
-    model,
-    input_shape=None,
-    args=[],
-    kwargs={},
-    print_profile=True,
-    detailed=True,
-    module_depth=-1,
-    top_modules=1,
-    warm_up=1,
-    as_string=True,
-    output_file=None,
-    ignore_modules=None,
-):
+def get_model_profile(model,
+                      input_shape=None,
+                      args=[],
+                      kwargs={},
+                      print_profile=True,
+                      detailed=True,
+                      module_depth=-1,
+                      top_modules=1,
+                      warm_up=1,
+                      as_string=True,
+                      output_file=None,
+                      ignore_modules=None,
+                      mode='forward'):
     """Returns the total floating-point operations, MACs, and parameters of a model.
 
     Example:
 
     .. code-block:: python
 
         model = torchvision.models.alexnet()
@@ -1167,26 +1234,37 @@
                 device=next(model.parameters()).device,
             )
         except StopIteration:
             input = torch.ones(()).new_empty((*input_shape, ))
 
         args = [input]
     assert (len(args) > 0) or (len(kwargs) > 0), "args and/or kwargs must be specified if input_shape is None"
-
     for _ in range(warm_up):
         if kwargs:
-            _ = model(*args, **kwargs)
+            if mode == 'forward':
+                _ = model(*args, **kwargs)
+            if mode == 'generate':
+                _ = model.generate(*args, **kwargs)
         else:
-            _ = model(*args)
+            if mode == 'forward':
+                _ = model(*args)
+            if mode == 'generate':
+                _ = model.generate(*args)
     prof.start_profile(ignore_list=ignore_modules)
 
     if kwargs:
-        _ = model(*args, **kwargs)
+        if mode == 'forward':
+            _ = model(*args, **kwargs)
+        if mode == 'generate':
+            _ = model.generate(*args, **kwargs)
     else:
-        _ = model(*args)
+        if mode == 'forward':
+            _ = model(*args)
+        if mode == 'generate':
+            _ = model.generate(*args)
 
     flops = prof.get_total_flops()
     macs = prof.get_total_macs()
     params = prof.get_total_params()
     if print_profile:
         prof.print_model_profile(profile_step=warm_up,
                                  module_depth=module_depth,
```

### Comparing `deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/checkpointing.py` & `deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/checkpointing.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/activation_checkpointing/config.py` & `deepspeed-0.9.5/deepspeed/runtime/activation_checkpointing/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/bf16_optimizer.py` & `deepspeed-0.9.5/deepspeed/runtime/bf16_optimizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 # DeepSpeed Team
 
 from collections import OrderedDict
 import torch
 import sys
 import os
+from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 from deepspeed import comm as dist
 from deepspeed.runtime.constants import PIPE_REPLICATED
-from deepspeed.ops.op_builder import UtilsBuilder
 from deepspeed.runtime import ZeROOptimizer
 from packaging import version as pkg_version
 
 from deepspeed.git_version_info import version
 from deepspeed.runtime.utils import (get_global_norm_of_tensors, clip_tensors_by_global_norm, DummyOptim,
                                      align_dense_tensors, all_gather_dp_groups, bwc_tensor_model_parallel_rank,
                                      is_model_parallel_parameter, see_memory_usage)
@@ -49,18 +49,17 @@
         self.norm_type = norm_type
         self.mpu = mpu
         self.allgather_bucket_size = int(allgather_bucket_size)
         self.dp_process_group = dp_process_group
         self.dp_rank = dist.get_rank(group=self.dp_process_group)
         self.real_dp_process_group = [dp_process_group for i in range(len(self.optimizer.param_groups))]
 
-        # Load pre-built or JIT compile (un)flatten ops
-        util_ops = UtilsBuilder().load()
-        self.flatten = util_ops.flatten
-        self.unflatten = util_ops.unflatten
+        # Use torch (un)flatten ops
+        self.flatten = _flatten_dense_tensors
+        self.unflatten = _unflatten_dense_tensors
 
         #align nccl all-gather send buffers to 4-bye boundary
         self.nccl_start_alignment_factor = 2  # 4-byte alignment/sizeof(fp16) = 2
 
         # Build BF16/FP32 groups
         self.bf16_groups = []
         self.bf16_groups_flat = []
```

### Comparing `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py` & `deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py` & `deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/nebula_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py` & `deepspeed-0.9.5/deepspeed/runtime/checkpoint_engine/torch_checkpoint_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/comm/coalesced_collectives.py` & `deepspeed-0.9.5/deepspeed/runtime/comm/coalesced_collectives.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/comm/mpi.py` & `deepspeed-0.9.5/deepspeed/runtime/comm/mpi.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/comm/nccl.py` & `deepspeed-0.9.5/deepspeed/runtime/comm/nccl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/compression/cupy.py` & `deepspeed-0.9.5/deepspeed/runtime/compression/cupy.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/config.py` & `deepspeed-0.9.5/deepspeed/runtime/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/config_utils.py` & `deepspeed-0.9.5/deepspeed/runtime/config_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/constants.py` & `deepspeed-0.9.5/deepspeed/runtime/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/config.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/constants.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/curriculum_scheduler.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/curriculum_scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/basic_layer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/helper.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/helper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/scheduler.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/scheduler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_routing/utils.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_routing/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/data_analyzer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/data_sampler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/indexed_dataset.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/data_pipeline/data_sampling/utils.py` & `deepspeed-0.9.5/deepspeed/runtime/data_pipeline/data_sampling/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/dataloader.py` & `deepspeed-0.9.5/deepspeed/runtime/dataloader.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/eigenvalue.py` & `deepspeed-0.9.5/deepspeed/runtime/eigenvalue.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/engine.py` & `deepspeed-0.9.5/deepspeed/runtime/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from shutil import copyfile
 import gc
 
 from torch.nn.modules import Module
 from torch.nn.parameter import Parameter
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
+from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 
 from typing import Callable, Dict, Union, Iterable
 
 import deepspeed
 
 from deepspeed import comm as dist
 from deepspeed.runtime.utils import see_memory_usage, DummyOptim
@@ -89,15 +90,14 @@
 from ..moe.utils import is_moe_param
 from ..git_version_info import version
 
 from deepspeed.profiling.flops_profiler.profiler import FlopsProfiler
 from deepspeed.utils.logging import print_json_dist, print_configuration
 
 from deepspeed.accelerator import get_accelerator
-from deepspeed.ops.op_builder import UtilsBuilder
 
 from deepspeed.runtime.config import DtypeEnum
 
 MEMORY_OPT_ALLREDUCE_SIZE = 500000000
 
 DeepSpeedOptimizerCallable = \
     Callable[[Union[Iterable[Parameter], Dict[str, Iterable]]], Optimizer]
@@ -356,18 +356,17 @@
                                           or self.flops_profiler_enabled())
 
         if self.global_rank == 0:
             self._config.print("DeepSpeedEngine configuration")
             if self.dump_state():
                 print_configuration(self, "DeepSpeedEngine")
 
-        # Load pre-installed or JIT compile (un)flatten ops
-        util_ops = UtilsBuilder().load()
-        self.flatten = util_ops.flatten
-        self.unflatten = util_ops.unflatten
+        # Use torch (un)flatten ops
+        self.flatten = _flatten_dense_tensors
+        self.unflatten = _unflatten_dense_tensors
 
     def destroy(self):
         if self.optimizer is not None and hasattr(self.optimizer, 'destroy'):
             self.optimizer.destroy()
 
     def _get_model_parameters(self):
         if self.autotuning_profile_model_info():
@@ -1041,15 +1040,15 @@
             if is_zero3_model:
                 self.__check_params(self.module, torch.bfloat16)
             self.module.bfloat16()
         else:
             self.__check_params(self.module, torch.float)
 
         # zero.Init() handles device placement of model
-        if not (self.dont_change_device or is_zero3_model):
+        if not self.dont_change_device:
             self.module.to(self.device)
 
         # MoE related initialization
         for _, module in self.module.named_modules():
             if isinstance(module, MoE):
                 self.has_moe_layers = True
                 self.num_experts.append(module.num_experts)
@@ -1077,15 +1076,15 @@
         # Query the groups module to get information about various parallel groups
         self.data_parallel_group = groups._get_data_parallel_group()
         self.dp_world_size = groups._get_data_parallel_world_size()
         self.mp_world_size = groups._get_model_parallel_world_size()
         self.expert_parallel_group = groups._get_expert_parallel_group_dict()
         self.expert_data_parallel_group = groups._get_expert_data_parallel_group_dict()
 
-        if not (self.amp_enabled() or is_zero3_model):
+        if not self.amp_enabled():
             self._broadcast_model()
 
     # check if parameters are duplicated in optimizer param_groups
     def _check_for_duplicates(self, optimizer):
         for name, param in self.module.named_parameters():
             param_id = id(param)
```

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/fused_optimizer.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/fused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/loss_scaler.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/loss_scaler.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/adam.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/lamb.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/onebit/zoadam.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/onebit/zoadam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/fp16/unfused_optimizer.py` & `deepspeed-0.9.5/deepspeed/runtime/fp16/unfused_optimizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/hybrid_engine.py` & `deepspeed-0.9.5/deepspeed/runtime/hybrid_engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/lr_schedules.py` & `deepspeed-0.9.5/deepspeed/runtime/lr_schedules.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/pipe/engine.py` & `deepspeed-0.9.5/deepspeed/runtime/pipe/engine.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/pipe/module.py` & `deepspeed-0.9.5/deepspeed/runtime/pipe/module.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/pipe/p2p.py` & `deepspeed-0.9.5/deepspeed/runtime/pipe/p2p.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/pipe/schedule.py` & `deepspeed-0.9.5/deepspeed/runtime/pipe/schedule.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/pipe/topology.py` & `deepspeed-0.9.5/deepspeed/runtime/pipe/topology.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/progressive_layer_drop.py` & `deepspeed-0.9.5/deepspeed/runtime/progressive_layer_drop.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/quantize.py` & `deepspeed-0.9.5/deepspeed/runtime/quantize.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/sparse_tensor.py` & `deepspeed-0.9.5/deepspeed/runtime/sparse_tensor.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/state_dict_factory.py` & `deepspeed-0.9.5/deepspeed/runtime/state_dict_factory.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/aio_config.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/aio_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/async_swapper.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/async_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/constants.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/constants.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/optimizer_utils.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/optimizer_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/partitioned_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/partitioned_param_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/pipelined_optimizer_swapper.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/swap_tensor/utils.py` & `deepspeed-0.9.5/deepspeed/runtime/swap_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/utils.py` & `deepspeed-0.9.5/deepspeed/runtime/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/weight_quantizer.py` & `deepspeed-0.9.5/deepspeed/runtime/weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/config.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/contiguous_memory_allocator.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/contiguous_memory_allocator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/linear.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/linear.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/mics.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/mics.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/mics_utils.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/mics_utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/offload_config.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/offload_config.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/parameter_offload.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/parameter_offload.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/partition_parameters.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/partition_parameters.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/partitioned_param_coordinator.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/partitioned_param_coordinator.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/stage3.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/stage3.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # DeepSpeed Team
 
 import sys
 import gc
 import collections
 from typing import Deque, Dict, Tuple
 
+from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 from deepspeed.runtime import ZeROOptimizer
 from deepspeed.utils import logger
 from deepspeed.runtime.fp16.loss_scaler import CreateLossScaler
 from deepspeed.runtime.comm.coalesced_collectives import reduce_scatter_coalesced
 from deepspeed.runtime.utils import inf, get_global_norm, is_model_parallel_parameter
 from deepspeed.runtime.zero.partition_parameters import *
 from deepspeed.runtime.zero.config import ZeroStageEnum
@@ -19,15 +20,14 @@
 from deepspeed.runtime.zero.parameter_offload import DeepSpeedZeRoOffload
 from deepspeed.ops.adam import DeepSpeedCPUAdam
 from deepspeed.runtime.swap_tensor.partitioned_param_swapper import PartitionedParamStatus
 from deepspeed.runtime.swap_tensor.partitioned_optimizer_swapper import PartitionedOptimizerSwapper
 from deepspeed.runtime.swap_tensor.pipelined_optimizer_swapper import PipelinedOptimizerSwapper
 from deepspeed.checkpoint.constants import OPTIMIZER_STATE_DICT, FP32_FLAT_GROUPS, PARTITION_COUNT, ZERO_STAGE
 from deepspeed.accelerator import get_accelerator
-from deepspeed.ops.op_builder import UtilsBuilder
 
 # Toggle this to true to enable correctness test
 # with gradient partitioning and without
 pg_correctness_test = False
 
 
 def print_rank_0(message, debug=False, force=False):
@@ -122,18 +122,17 @@
         # - flat by groups, not keeping state. TODO: remove state explicitly?
         # - master grad and unflat master weight never exist. TODO: a way to save out unflat master?
         if not get_accelerator().is_available():
             raise SystemError("Cannot use fp16 without accelerator.")
 
         self.optimizer = init_optimizer
 
-        # Load pre-built or JIT compile (un)flatten ops
-        util_ops = UtilsBuilder().load()
-        self.flatten = util_ops.flatten
-        self.unflatten = util_ops.unflatten
+        # Use torch (un)flatten ops
+        self.flatten = _flatten_dense_tensors
+        self.unflatten = _unflatten_dense_tensors
         self.dtype = self.optimizer.param_groups[0]['params'][0].dtype
         self._global_grad_norm = 0.
 
         self.custom_loss_scaler = False
         self.external_loss_scale = None
 
         self.optimizer_swapper = None
```

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/stage_1_and_2.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/stage_1_and_2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 # DeepSpeed Team
 
 import torch
 import os
 from deepspeed import comm as dist
 from packaging import version as pkg_version
 from collections import OrderedDict
+from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
 
 from deepspeed.runtime import ZeROOptimizer
 from deepspeed.runtime.fp16.loss_scaler import CreateLossScaler
 from deepspeed.runtime.utils import (bwc_tensor_model_parallel_rank, get_global_norm, empty_cache, see_memory_usage,
                                      inf, is_model_parallel_parameter, align_dense_tensors, all_gather_dp_groups)
 
 from deepspeed.runtime.zero.config import ZeroStageEnum
@@ -19,15 +20,14 @@
 from deepspeed.ops.adam import DeepSpeedCPUAdam
 from deepspeed.utils import logger
 from deepspeed.moe.utils import is_moe_param
 from deepspeed.git_version_info import version
 
 from deepspeed.runtime.constants import PIPE_REPLICATED
 from deepspeed.accelerator import get_accelerator
-from deepspeed.ops.op_builder import UtilsBuilder
 
 from deepspeed.checkpoint.constants import (DS_VERSION, GROUP_PADDINGS, PARTITION_COUNT,
                                             SINGLE_PARTITION_OF_FP32_GROUPS, BASE_OPTIMIZER_STATE, CLIP_GRAD,
                                             ZERO_STAGE, PARAM_SLICE_MAPPINGS)
 from deepspeed.utils import link_hp_params
 from deepspeed.checkpoint import enable_universal_checkpoint
 
@@ -146,18 +146,17 @@
         # - assume all params requires grad
         # - flat by groups, not keeping state. TODO: remove state explicitly?
         # - master grad and unflat master weight never exist. TODO: a way to save out unflat master?
         if not get_accelerator().is_available():
             raise SystemError("Cannot use fp16 without accelerator.")
         self.optimizer = init_optimizer
 
-        # Load pre-built or JIT compile (un)flatten ops
-        util_ops = UtilsBuilder().load()
-        self.flatten = util_ops.flatten
-        self.unflatten = util_ops.unflatten
+        # Use torch (un)flatten ops
+        self.flatten = _flatten_dense_tensors
+        self.unflatten = _unflatten_dense_tensors
 
         # ZeRO stage 1 (False) or 2 (True)
         self.partition_gradients = partition_grads
         self.zero_stage_string = "ZeRO-2" if partition_grads else "ZeRO-1"
 
         self.timers = timers
```

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/test.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/test.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/tiling.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/tiling.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/runtime/zero/utils.py` & `deepspeed-0.9.5/deepspeed/runtime/zero/utils.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/__init__.py` & `deepspeed-0.9.5/deepspeed/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/comms_logging.py` & `deepspeed-0.9.5/deepspeed/utils/comms_logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/debug.py` & `deepspeed-0.9.5/deepspeed/utils/debug.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/groups.py` & `deepspeed-0.9.5/deepspeed/utils/groups.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/init_on_device.py` & `deepspeed-0.9.5/deepspeed/utils/init_on_device.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/logging.py` & `deepspeed-0.9.5/deepspeed/utils/logging.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/mixed_precision_linkage.py` & `deepspeed-0.9.5/deepspeed/utils/mixed_precision_linkage.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/numa.py` & `deepspeed-0.9.5/deepspeed/utils/numa.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/tensor_fragment.py` & `deepspeed-0.9.5/deepspeed/utils/tensor_fragment.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/timer.py` & `deepspeed-0.9.5/deepspeed/utils/timer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed/utils/zero_to_fp32.py` & `deepspeed-0.9.5/deepspeed/utils/zero_to_fp32.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/deepspeed.egg-info/PKG-INFO` & `deepspeed-0.9.5/deepspeed.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepspeed
-Version: 0.9.4
+Version: 0.9.5
 Summary: DeepSpeed library
 Home-page: http://deepspeed.ai
 Author: DeepSpeed Team
 Author-email: deepspeed-info@microsoft.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://deepspeed.readthedocs.io
 Project-URL: Source, https://github.com/microsoft/DeepSpeed
@@ -29,14 +29,16 @@
 License-File: LICENSE
 
 [![License Apache 2.0](https://badgen.net/badge/license/apache2.0/blue)](https://github.com/Microsoft/DeepSpeed/blob/master/LICENSE)
 [![PyPI version](https://badge.fury.io/py/deepspeed.svg)](https://pypi.org/project/deepspeed/)
 [![Downloads](https://pepy.tech/badge/deepspeed)](https://pepy.tech/project/deepspeed)
 [![Build](https://badgen.net/badge/build/check-status/blue)](#build-pipeline-status)
 [![Twitter](https://img.shields.io/twitter/follow/MSFTDeepSpeed)](https://twitter.com/intent/follow?screen_name=MSFTDeepSpeed)
+[![Japanese Twitter](https://img.shields.io/badge/%E6%97%A5%E6%9C%AC%E8%AA%9ETwitter-%40MSFTDeepSpeedJP-blue)](https://twitter.com/MSFTDeepSpeedJP)
+[![Chinese Zhihu](https://img.shields.io/badge/%E7%9F%A5%E4%B9%8E-%E5%BE%AE%E8%BD%AFDeepSpeed-blue)](https://www.zhihu.com/people/deepspeed)
 
 
 <div align="center">
  <img src="docs/assets/images/DeepSpeed_light.svg#gh-light-mode-only" width="400px">
  <img src="docs/assets/images/DeepSpeed_dark_transparent.svg#gh-dark-mode-only" width="400px">
 </div>
 
@@ -133,15 +135,15 @@
 
 ---
 
 # Build Pipeline Status
 
 | Description | Status |
 | ----------- | ------ |
-| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
+| NVIDIA | [![nv-torch19-p40](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-p40.yml) [![nv-torch19-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch19-v100.yml) [![nv-torch-latest-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-v100.yml) [![nv-h100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-h100.yml) [![nv-inference](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-inference.yml) [![nv-nightly](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-nightly.yml) |
 | AMD | [![amd-mi100](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi100.yml) [![amd-mi200](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/amd-mi200.yml) |
 | CPU | [![nv-torch-latest-cpu](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-latest-cpu.yml) |
 | PyTorch Nightly | [![nv-torch-nightly-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-torch-nightly-v100.yml) |
 | Integrations | [![nv-transformers-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-transformers-v100.yml) [![nv-lightning-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-lightning-v100.yml) [![nv-accelerate-v100](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-accelerate-v100.yml)[![nv-megatron](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-megatron.yml)[![nv-mii](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/nv-mii.yml) |
 | Misc | [![Formatting](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/formatting.yml) [![pages-build-deployment](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/microsoft/DeepSpeed/actions/workflows/pages/pages-build-deployment) [![Documentation Status](https://readthedocs.org/projects/deepspeed/badge/?version=latest)](https://deepspeed.readthedocs.io/en/latest/?badge=latest)[![python](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml/badge.svg?branch=master)](https://github.com/microsoft/DeepSpeed/actions/workflows/python.yml) |
 
 # Installation
```

### Comparing `deepspeed-0.9.4/deepspeed.egg-info/SOURCES.txt` & `deepspeed-0.9.5/deepspeed.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -353,15 +353,14 @@
 deepspeed/ops/op_builder/quantizer.py
 deepspeed/ops/op_builder/random_ltd.py
 deepspeed/ops/op_builder/sparse_attn.py
 deepspeed/ops/op_builder/spatial_inference.py
 deepspeed/ops/op_builder/stochastic_transformer.py
 deepspeed/ops/op_builder/transformer.py
 deepspeed/ops/op_builder/transformer_inference.py
-deepspeed/ops/op_builder/utils.py
 deepspeed/ops/op_builder/cpu/__init__.py
 deepspeed/ops/op_builder/cpu/builder.py
 deepspeed/ops/op_builder/cpu/comm.py
 deepspeed/ops/op_builder/cpu/no_impl.py
 deepspeed/ops/quantizer/__init__.py
 deepspeed/ops/quantizer/quantizer.py
 deepspeed/ops/random_ltd/__init__.py
@@ -511,15 +510,14 @@
 op_builder/quantizer.py
 op_builder/random_ltd.py
 op_builder/sparse_attn.py
 op_builder/spatial_inference.py
 op_builder/stochastic_transformer.py
 op_builder/transformer.py
 op_builder/transformer_inference.py
-op_builder/utils.py
 op_builder/cpu/__init__.py
 op_builder/cpu/builder.py
 op_builder/cpu/comm.py
 op_builder/cpu/no_impl.py
 requirements/requirements-1bit-mpi.txt
 requirements/requirements-autotuning-ml.txt
 requirements/requirements-autotuning.txt
```

### Comparing `deepspeed-0.9.4/deepspeed.egg-info/requires.txt` & `deepspeed-0.9.5/deepspeed.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -10,49 +10,49 @@
 
 [1bit]
 
 [1bit_mpi]
 mpi4py
 
 [all]
+google
+recommonmark
+packaging
+pytest-randomly
+psutil
+docutils<0.18
+neural-compressor==2.1.0
+hjson
 mpi4py
-transformers[sentencepiece]
-tabulate
-sphinx
-sphinx-rtd-theme
-future
+triton==1.0.0
+protobuf
 autodoc_pydantic<2.0.0
+torchvision
+pytest
+wandb
+pre-commit>=2.20.0
+tensorboard
+lm-eval==0.3.0
+torch
+future
+tqdm
+tabulate
+pytest-forked
+transformers[sentencepiece]
 diffusers
+pydantic<2.0.0
+sphinx
 transformers
 pytest-xdist
-torch
-docutils<0.18
-pytest-forked
-tensorboard
-psutil
+triton==2.0.0.dev20221202
 xgboost
 py-cpuinfo
-tqdm
-triton==2.0.0.dev20221202
+sphinx-rtd-theme
 clang-format==16.0.2
 importlib-metadata>=4
-pytest-randomly
-protobuf
-lm-eval==0.3.0
-pre-commit>=2.20.0
-wandb
-packaging
-pytest
-pydantic<2.0.0
-triton==1.0.0
-google
-neural-compressor==2.1.0
-hjson
-recommonmark
-torchvision
 
 [autotuning]
 tabulate
 
 [autotuning_ml]
 hjson
 tabulate
```

### Comparing `deepspeed-0.9.4/op_builder/__init__.py` & `deepspeed-0.9.5/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/all_ops.py` & `deepspeed-0.9.5/op_builder/all_ops.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/async_io.py` & `deepspeed-0.9.5/op_builder/async_io.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/builder.py` & `deepspeed-0.9.5/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/cpu/builder.py` & `deepspeed-0.9.5/op_builder/cpu/builder.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/cpu/comm.py` & `deepspeed-0.9.5/op_builder/cpu/comm.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/cpu/no_impl.py` & `deepspeed-0.9.5/op_builder/cpu/no_impl.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/cpu_adagrad.py` & `deepspeed-0.9.5/op_builder/cpu_adagrad.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/cpu_adam.py` & `deepspeed-0.9.5/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/fused_adam.py` & `deepspeed-0.9.5/op_builder/fused_adam.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/fused_lamb.py` & `deepspeed-0.9.5/op_builder/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/quantizer.py` & `deepspeed-0.9.5/op_builder/quantizer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/random_ltd.py` & `deepspeed-0.9.5/op_builder/random_ltd.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/sparse_attn.py` & `deepspeed-0.9.5/op_builder/sparse_attn.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/spatial_inference.py` & `deepspeed-0.9.5/op_builder/spatial_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/stochastic_transformer.py` & `deepspeed-0.9.5/op_builder/stochastic_transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/transformer.py` & `deepspeed-0.9.5/op_builder/transformer.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/op_builder/transformer_inference.py` & `deepspeed-0.9.5/op_builder/transformer_inference.py`

 * *Files identical despite different names*

### Comparing `deepspeed-0.9.4/setup.py` & `deepspeed-0.9.5/setup.py`

 * *Files identical despite different names*

