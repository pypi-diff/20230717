# Comparing `tmp/bittensor-5.3.0.tar.gz` & `tmp/bittensor-5.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bittensor-5.3.0.tar", last modified: Tue Jul  4 23:20:43 2023, max compression
+gzip compressed data, was "bittensor-5.3.1.tar", last modified: Mon Jul 17 20:03:22 2023, max compression
```

## Comparing `bittensor-5.3.0.tar` & `bittensor-5.3.1.tar`

### file list

```diff
@@ -1,116 +1,146 @@
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.300383 bittensor-5.3.0/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1087 2023-06-28 18:47:57.000000 bittensor-5.3.0/LICENSE
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    23569 2023-07-04 23:20:43.300169 bittensor-5.3.0/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    22543 2023-07-04 20:54:21.000000 bittensor-5.3.0/README.md
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.282407 bittensor-5.3.0/bin/
--rwxr-xr-x   0 cameronfairchild   (501) staff       (20)     1297 2023-07-04 19:38:51.000000 bittensor-5.3.0/bin/btcli
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.282673 bittensor-5.3.0/bittensor/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    15302 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.283833 bittensor-5.3.0/bittensor/_axon/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    17038 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_axon/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.283992 bittensor-5.3.0/bittensor/_blacklist/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4759 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_blacklist/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.284466 bittensor-5.3.0/bittensor/_cli/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7377 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4431 2023-07-04 19:41:43.000000 bittensor-5.3.0/bittensor/_cli/cli_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.287676 bittensor-5.3.0/bittensor/_cli/commands/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      739 2023-07-04 19:41:43.000000 bittensor-5.3.0/bittensor/_cli/commands/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    24532 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/delegates.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7982 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/inspect.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3900 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/list.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7371 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/metagraph.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5572 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/misc.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    16284 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/overview.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7397 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/register.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    17951 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/senate.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10872 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/stake.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4285 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/transfer.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11002 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/unstake.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7692 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_cli/commands/utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    17326 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_cli/commands/wallets.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.288569 bittensor-5.3.0/bittensor/_dataset/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    11200 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_dataset/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    26660 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dataset/dataset_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5443 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dataset/dataset_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3581 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dataset/thread_queue.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.288916 bittensor-5.3.0/bittensor/_dendrite/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dendrite/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10132 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_dendrite/dendrite.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.289351 bittensor-5.3.0/bittensor/_dendrite/text_prompting/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dendrite/text_prompting/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7861 2023-07-04 21:03:21.000000 bittensor-5.3.0/bittensor/_dendrite/text_prompting/dendrite.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5215 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_dendrite/text_prompting/dendrite_pool.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.289669 bittensor-5.3.0/bittensor/_ipfs/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-06-28 18:47:57.000000 bittensor-5.3.0/bittensor/_ipfs/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2890 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_ipfs/ipfs_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.289845 bittensor-5.3.0/bittensor/_logging/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13313 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_logging/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.290011 bittensor-5.3.0/bittensor/_metagraph/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    12895 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_metagraph/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.290888 bittensor-5.3.0/bittensor/_neuron/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_neuron/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5752 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_neuron/base_huggingface_miner.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10128 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_neuron/base_miner_neuron.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3186 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_neuron/base_prompting_miner.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.291145 bittensor-5.3.0/bittensor/_priority/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3529 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_priority/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.291383 bittensor-5.3.0/bittensor/_prometheus/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8337 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_prometheus/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.291889 bittensor-5.3.0/bittensor/_proto/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-06-28 18:47:57.000000 bittensor-5.3.0/bittensor/_proto/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    28340 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_proto/bittensor_pb2.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4422 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_proto/bittensor_pb2_grpc.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.292244 bittensor-5.3.0/bittensor/_serializer/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6062 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_serializer/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10739 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_serializer/serializer_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.293456 bittensor-5.3.0/bittensor/_subtensor/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    13873 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    26055 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/chain_data.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2467 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/errors.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.296037 bittensor-5.3.0/bittensor/_subtensor/extrinsics/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1119 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    14116 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/delegation.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    26886 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/log_utilities.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5736 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/prometheus.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    12590 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/registration.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    10609 2023-07-04 19:41:43.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/senate.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9835 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/serving.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5624 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/set_weights.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    17833 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/staking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6109 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/transfer.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    14947 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/extrinsics/unstaking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    69604 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/subtensor_impl.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    52059 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/subtensor_mock.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     1505 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_subtensor/types.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.296334 bittensor-5.3.0/bittensor/_synapse/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_synapse/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6959 2023-07-04 19:41:43.000000 bittensor-5.3.0/bittensor/_synapse/synapse.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.296772 bittensor-5.3.0/bittensor/_synapse/text_prompting/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_synapse/text_prompting/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     5329 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_synapse/text_prompting/synapse.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.297041 bittensor-5.3.0/bittensor/_threadpool/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4730 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/_threadpool/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8594 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_threadpool/priority_thread_pool_impl.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.297338 bittensor-5.3.0/bittensor/_tokenizer/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     2485 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/_tokenizer/__init__.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.299927 bittensor-5.3.0/bittensor/utils/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     6492 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/utils/__init__.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3443 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/_register_cuda.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     8699 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/balance.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     4445 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/codes.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      518 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/formatting.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     7999 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/networking.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    37871 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/utils/registration.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    33019 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/utils/registratrion_old.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3351 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/stats.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      630 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/test_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    75481 2023-07-04 19:38:51.000000 bittensor-5.3.0/bittensor/utils/tokenizer_utils.py
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     9966 2023-07-04 20:54:21.000000 bittensor-5.3.0/bittensor/utils/weight_utils.py
-drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-04 23:20:43.283683 bittensor-5.3.0/bittensor.egg-info/
--rw-r--r--   0 cameronfairchild   (501) staff       (20)    23569 2023-07-04 23:20:43.000000 bittensor-5.3.0/bittensor.egg-info/PKG-INFO
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3028 2023-07-04 23:20:43.000000 bittensor-5.3.0/bittensor.egg-info/SOURCES.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-04 23:20:43.000000 bittensor-5.3.0/bittensor.egg-info/dependency_links.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)      908 2023-07-04 23:20:43.000000 bittensor-5.3.0/bittensor.egg-info/requires.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       10 2023-07-04 23:20:43.000000 bittensor-5.3.0/bittensor.egg-info/top_level.txt
--rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-04 23:20:43.300456 bittensor-5.3.0/setup.cfg
--rw-r--r--   0 cameronfairchild   (501) staff       (20)     3429 2023-07-04 19:38:51.000000 bittensor-5.3.0/setup.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.113470 bittensor-5.3.1/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1087 2023-07-13 19:44:57.000000 bittensor-5.3.1/LICENSE
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    23565 2023-07-17 20:03:22.113257 bittensor-5.3.1/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    22539 2023-07-13 19:50:20.000000 bittensor-5.3.1/README.md
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.081961 bittensor-5.3.1/bin/
+-rwxr-xr-x   0 cameronfairchild   (501) staff       (20)     1297 2023-07-13 19:44:57.000000 bittensor-5.3.1/bin/btcli
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.082223 bittensor-5.3.1/bittensor/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    15302 2023-07-13 19:50:20.000000 bittensor-5.3.1/bittensor/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.083581 bittensor-5.3.1/bittensor/_axon/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    17038 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_axon/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.083779 bittensor-5.3.1/bittensor/_blacklist/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4770 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_blacklist/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.084117 bittensor-5.3.1/bittensor/_cli/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7377 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4431 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/cli_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.091877 bittensor-5.3.1/bittensor/_cli/commands/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      739 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    24532 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/delegates.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7982 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/inspect.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3900 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/list.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7371 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/metagraph.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5572 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/misc.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    16284 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/overview.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7397 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/register.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    17951 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/senate.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10872 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/stake.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4285 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/transfer.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    11002 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/unstake.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7692 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    17326 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_cli/commands/wallets.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.093243 bittensor-5.3.1/bittensor/_dataset/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    11200 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dataset/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    26660 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dataset/dataset_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5443 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dataset/dataset_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3581 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dataset/thread_queue.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.094160 bittensor-5.3.1/bittensor/_dendrite/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dendrite/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10132 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dendrite/dendrite.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.095682 bittensor-5.3.1/bittensor/_dendrite/text_prompting/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dendrite/text_prompting/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7861 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dendrite/text_prompting/dendrite.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5215 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_dendrite/text_prompting/dendrite_pool.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.096551 bittensor-5.3.1/bittensor/_ipfs/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_ipfs/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2890 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_ipfs/ipfs_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.096989 bittensor-5.3.1/bittensor/_logging/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13313 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_logging/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.097456 bittensor-5.3.1/bittensor/_metagraph/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12895 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_metagraph/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.099523 bittensor-5.3.1/bittensor/_neuron/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_neuron/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5752 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_neuron/base_huggingface_miner.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10128 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_neuron/base_miner_neuron.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3186 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_neuron/base_prompting_miner.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.099689 bittensor-5.3.1/bittensor/_priority/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3529 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_priority/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.099841 bittensor-5.3.1/bittensor/_prometheus/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8337 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_prometheus/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.100400 bittensor-5.3.1/bittensor/_proto/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_proto/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    28340 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_proto/bittensor_pb2.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4422 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_proto/bittensor_pb2_grpc.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.100738 bittensor-5.3.1/bittensor/_serializer/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6062 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_serializer/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10739 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_serializer/serializer_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.102339 bittensor-5.3.1/bittensor/_subtensor/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13873 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    26055 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/chain_data.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2467 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/errors.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.104582 bittensor-5.3.1/bittensor/_subtensor/extrinsics/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1119 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    14116 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/delegation.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    26886 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/log_utilities.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5736 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/prometheus.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12590 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/registration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    10609 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/senate.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     9835 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/serving.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5624 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/set_weights.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    17833 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/staking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6109 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/transfer.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    14947 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/extrinsics/unstaking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    69611 2023-07-13 19:50:20.000000 bittensor-5.3.1/bittensor/_subtensor/subtensor_impl.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    52059 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/subtensor_mock.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1505 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_subtensor/types.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.104859 bittensor-5.3.1/bittensor/_synapse/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_synapse/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6959 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_synapse/synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.105142 bittensor-5.3.1/bittensor/_synapse/text_prompting/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_synapse/text_prompting/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5329 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_synapse/text_prompting/synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.105702 bittensor-5.3.1/bittensor/_threadpool/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4730 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_threadpool/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8594 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_threadpool/priority_thread_pool_impl.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.105961 bittensor-5.3.1/bittensor/_tokenizer/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2485 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/_tokenizer/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.108136 bittensor-5.3.1/bittensor/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     6492 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3443 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/_register_cuda.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     8699 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/balance.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4445 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/codes.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      518 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/formatting.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7999 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/networking.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    37871 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/registration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    33019 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/registratrion_old.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3351 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/stats.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      630 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/test_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    75481 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/tokenizer_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     9966 2023-07-13 19:44:57.000000 bittensor-5.3.1/bittensor/utils/weight_utils.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.083376 bittensor-5.3.1/bittensor.egg-info/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    23565 2023-07-17 20:03:22.000000 bittensor-5.3.1/bittensor.egg-info/PKG-INFO
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4105 2023-07-17 20:03:22.000000 bittensor-5.3.1/bittensor.egg-info/SOURCES.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        1 2023-07-17 20:03:22.000000 bittensor-5.3.1/bittensor.egg-info/dependency_links.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      908 2023-07-17 20:03:22.000000 bittensor-5.3.1/bittensor.egg-info/requires.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       16 2023-07-17 20:03:22.000000 bittensor-5.3.1/bittensor.egg-info/top_level.txt
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)       38 2023-07-17 20:03:22.113535 bittensor-5.3.1/setup.cfg
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3429 2023-07-13 19:44:57.000000 bittensor-5.3.1/setup.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.108298 bittensor-5.3.1/tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1197 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.108551 bittensor-5.3.1/tests/helpers/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1246 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/helpers/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     5671 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/helpers/helpers.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.109754 bittensor-5.3.1/tests/integration_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/integration_tests/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    81518 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/integration_tests/test_cli.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    37492 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/integration_tests/test_cli_no_network.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)      920 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/integration_tests/test_ipfs.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     3474 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/integration_tests/test_metagraph_integration.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1645 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/integration_tests/test_priority_thread_pool.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1331 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/integration_tests/test_prometheus.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    23570 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/integration_tests/test_subtensor_integration.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.109997 bittensor-5.3.1/tests/unit_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/__init__.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.111553 bittensor-5.3.1/tests/unit_tests/bittensor_tests/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    13529 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_axon.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    15160 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_balance.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4331 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_config.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     1761 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_metagraph.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    12319 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_serialization.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     7098 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_subtensor.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4886 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/test_synapse.py
+drwxr-xr-x   0 cameronfairchild   (501) staff       (20)        0 2023-07-17 20:03:22.112938 bittensor-5.3.1/tests/unit_tests/bittensor_tests/utils/
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)        0 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/utils/__init__.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     4916 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/utils/test_network_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)    34082 2023-07-13 19:50:20.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/utils/test_utils.py
+-rw-r--r--   0 cameronfairchild   (501) staff       (20)     2931 2023-07-13 19:44:57.000000 bittensor-5.3.1/tests/unit_tests/bittensor_tests/utils/test_weight_utils.py
```

### Comparing `bittensor-5.3.0/LICENSE` & `bittensor-5.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/PKG-INFO` & `bittensor-5.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 5.3.0
+Version: 5.3.1
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 
 ---
 
 ### Internet-scale Neural Networks <!-- omit in toc -->
 
-[Discord](https://discord.gg/realbittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
+[Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
 
 </div>
 
 This repository contains Bittensor's Python API, which can be used for the following purposes:
 
 1. Querying the Bittensor network as a client.
 2. Running and building Bittensor miners.  (Validators are now at [openvalidators](https://github.com/opentensor/validators)).
```

### Comparing `bittensor-5.3.0/README.md` & `bittensor-5.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 
 ---
 
 ### Internet-scale Neural Networks <!-- omit in toc -->
 
-[Discord](https://discord.gg/realbittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
+[Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
 
 </div>
 
 This repository contains Bittensor's Python API, which can be used for the following purposes:
 
 1. Querying the Bittensor network as a client.
 2. Running and building Bittensor miners.  (Validators are now at [openvalidators](https://github.com/opentensor/validators)).
```

### Comparing `bittensor-5.3.0/bin/btcli` & `bittensor-5.3.1/bin/btcli`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/__init__.py` & `bittensor-5.3.1/bittensor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from langchain.llms.base import LLM
 from typing import Optional, List, Mapping, Any, Tuple
 
 import nest_asyncio
 nest_asyncio.apply()
 
 # Bittensor code and protocol version.
-__version__ = '5.3.0'
+__version__ = '5.3.1'
 version_split = __version__.split(".")
 __version_as_int__ = (100 * int(version_split[0])) + (10 * int(version_split[1])) + (1 * int(version_split[2]))
 __new_signature_version__ = 360
 
 # Turn off rich console locals trace.
 from rich.traceback import install
 install(show_locals=False)
```

### Comparing `bittensor-5.3.0/bittensor/_axon/__init__.py` & `bittensor-5.3.1/bittensor/_axon/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_blacklist/__init__.py` & `bittensor-5.3.1/bittensor/_blacklist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,16 +55,16 @@
             nargs = '*', 
             action = 'store',
             help = 'List of ss58 addresses which are always allowed pass through.', default=[]
         )
         parser.add_argument(
             '--' + prefix_str + 'blacklist.allow_non_registered',
             action = 'store_true',
-            help = 'If True, the miner will allow non-registered hotkeys to mine.',
-            default = True
+            help = 'If True, the miner will allow non-registered hotkeys to pass blacklist.',
+            default = False
         )
         parser.add_argument(
             '--' + prefix_str + 'blacklist.min_allowed_stake',
             type = float,
             help = 'Minimum stake required to pass blacklist.',
             default = 0.0
         )
```

### Comparing `bittensor-5.3.0/bittensor/_cli/__init__.py` & `bittensor-5.3.1/bittensor/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/cli_impl.py` & `bittensor-5.3.1/bittensor/_cli/cli_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/__init__.py` & `bittensor-5.3.1/bittensor/_cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/delegates.py` & `bittensor-5.3.1/bittensor/_cli/commands/delegates.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/inspect.py` & `bittensor-5.3.1/bittensor/_cli/commands/inspect.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/list.py` & `bittensor-5.3.1/bittensor/_cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/metagraph.py` & `bittensor-5.3.1/bittensor/_cli/commands/metagraph.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/misc.py` & `bittensor-5.3.1/bittensor/_cli/commands/misc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/overview.py` & `bittensor-5.3.1/bittensor/_cli/commands/overview.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/register.py` & `bittensor-5.3.1/bittensor/_cli/commands/register.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/senate.py` & `bittensor-5.3.1/bittensor/_cli/commands/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/stake.py` & `bittensor-5.3.1/bittensor/_cli/commands/stake.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/transfer.py` & `bittensor-5.3.1/bittensor/_cli/commands/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/unstake.py` & `bittensor-5.3.1/bittensor/_cli/commands/unstake.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/utils.py` & `bittensor-5.3.1/bittensor/_cli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_cli/commands/wallets.py` & `bittensor-5.3.1/bittensor/_cli/commands/wallets.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dataset/__init__.py` & `bittensor-5.3.1/bittensor/_dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dataset/dataset_impl.py` & `bittensor-5.3.1/bittensor/_dataset/dataset_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dataset/dataset_mock.py` & `bittensor-5.3.1/bittensor/_dataset/dataset_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dataset/thread_queue.py` & `bittensor-5.3.1/bittensor/_dataset/thread_queue.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dendrite/dendrite.py` & `bittensor-5.3.1/bittensor/_dendrite/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dendrite/text_prompting/dendrite.py` & `bittensor-5.3.1/bittensor/_dendrite/text_prompting/dendrite.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_dendrite/text_prompting/dendrite_pool.py` & `bittensor-5.3.1/bittensor/_dendrite/text_prompting/dendrite_pool.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_ipfs/ipfs_impl.py` & `bittensor-5.3.1/bittensor/_ipfs/ipfs_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_logging/__init__.py` & `bittensor-5.3.1/bittensor/_logging/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_metagraph/__init__.py` & `bittensor-5.3.1/bittensor/_metagraph/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_neuron/base_huggingface_miner.py` & `bittensor-5.3.1/bittensor/_neuron/base_huggingface_miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_neuron/base_miner_neuron.py` & `bittensor-5.3.1/bittensor/_neuron/base_miner_neuron.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_neuron/base_prompting_miner.py` & `bittensor-5.3.1/bittensor/_neuron/base_prompting_miner.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_priority/__init__.py` & `bittensor-5.3.1/bittensor/_priority/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_prometheus/__init__.py` & `bittensor-5.3.1/bittensor/_prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_proto/bittensor_pb2.py` & `bittensor-5.3.1/bittensor/_proto/bittensor_pb2.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_proto/bittensor_pb2_grpc.py` & `bittensor-5.3.1/bittensor/_proto/bittensor_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_serializer/__init__.py` & `bittensor-5.3.1/bittensor/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_serializer/serializer_impl.py` & `bittensor-5.3.1/bittensor/_serializer/serializer_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/__init__.py` & `bittensor-5.3.1/bittensor/_subtensor/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/chain_data.py` & `bittensor-5.3.1/bittensor/_subtensor/chain_data.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/errors.py` & `bittensor-5.3.1/bittensor/_subtensor/errors.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/__init__.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/delegation.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/delegation.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/log_utilities.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/log_utilities.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/prometheus.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/prometheus.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/registration.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/senate.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/senate.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/serving.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/serving.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/set_weights.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/set_weights.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/staking.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/staking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/transfer.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/transfer.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/extrinsics/unstaking.py` & `bittensor-5.3.1/bittensor/_subtensor/extrinsics/unstaking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/subtensor_impl.py` & `bittensor-5.3.1/bittensor/_subtensor/subtensor_impl.py`

 * *Files 0% similar despite different names*

```diff
@@ -732,15 +732,15 @@
         return vote_senate_extrinsic( self, wallet, proposal_hash, proposal_idx, vote, wait_for_inclusion, wait_for_finalization, prompt )
     
     def is_senate_member(
         self,
         hotkey_ss58: str,
         block: Optional[int] = None,
     ) -> bool:
-        senate_members = self.query_module(module="Senate", name="Members", block=block ).serialize()
+        senate_members = self.query_module(module="SenateMembers", name="Members", block=block ).serialize()
         return senate_members.count( hotkey_ss58 ) > 0
     
     def get_vote_data(
         self,
         proposal_hash: str,
         block: Optional[int] = None,
     ) -> Optional[ProposalVoteData]:
```

### Comparing `bittensor-5.3.0/bittensor/_subtensor/subtensor_mock.py` & `bittensor-5.3.1/bittensor/_subtensor/subtensor_mock.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_subtensor/types.py` & `bittensor-5.3.1/bittensor/_subtensor/types.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_synapse/synapse.py` & `bittensor-5.3.1/bittensor/_synapse/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_synapse/text_prompting/synapse.py` & `bittensor-5.3.1/bittensor/_synapse/text_prompting/synapse.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_threadpool/__init__.py` & `bittensor-5.3.1/bittensor/_threadpool/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_threadpool/priority_thread_pool_impl.py` & `bittensor-5.3.1/bittensor/_threadpool/priority_thread_pool_impl.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/_tokenizer/__init__.py` & `bittensor-5.3.1/bittensor/_tokenizer/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/__init__.py` & `bittensor-5.3.1/bittensor/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/_register_cuda.py` & `bittensor-5.3.1/bittensor/utils/_register_cuda.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/balance.py` & `bittensor-5.3.1/bittensor/utils/balance.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/codes.py` & `bittensor-5.3.1/bittensor/utils/codes.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/formatting.py` & `bittensor-5.3.1/bittensor/utils/formatting.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/networking.py` & `bittensor-5.3.1/bittensor/utils/networking.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/registration.py` & `bittensor-5.3.1/bittensor/utils/registration.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/registratrion_old.py` & `bittensor-5.3.1/bittensor/utils/registratrion_old.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/stats.py` & `bittensor-5.3.1/bittensor/utils/stats.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/test_utils.py` & `bittensor-5.3.1/bittensor/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/tokenizer_utils.py` & `bittensor-5.3.1/bittensor/utils/tokenizer_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor/utils/weight_utils.py` & `bittensor-5.3.1/bittensor/utils/weight_utils.py`

 * *Files identical despite different names*

### Comparing `bittensor-5.3.0/bittensor.egg-info/PKG-INFO` & `bittensor-5.3.1/bittensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bittensor
-Version: 5.3.0
+Version: 5.3.1
 Summary: bittensor
 Home-page: https://github.com/opentensor/bittensor
 Author: bittensor.com
 Author-email: 
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
@@ -32,15 +32,15 @@
 [![PyPI version](https://badge.fury.io/py/bittensor.svg)](https://badge.fury.io/py/bittensor)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT) 
 
 ---
 
 ### Internet-scale Neural Networks <!-- omit in toc -->
 
-[Discord](https://discord.gg/realbittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
+[Discord](https://discord.gg/bittensor) • [Network](https://taostats.io/) • [Research](https://drive.google.com/file/d/1VnsobL6lIAAqcA1_Tbm8AYIQscfJV4KU)
 
 </div>
 
 This repository contains Bittensor's Python API, which can be used for the following purposes:
 
 1. Querying the Bittensor network as a client.
 2. Running and building Bittensor miners.  (Validators are now at [openvalidators](https://github.com/opentensor/validators)).
```

### Comparing `bittensor-5.3.0/bittensor.egg-info/requires.txt` & `bittensor-5.3.1/bittensor.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ansible_vault==2.1
 argparse==1.4.0
 base58==2.0.1
 backoff==2.1.0
 bittensor-config==0.0.0
-bittensor-wallet==0.0.1
-cryptography==39.0.0
+bittensor-wallet==0.0.4
+cryptography==41.0.0
 datasets==2.12.0
 fuzzywuzzy==0.18.0
 grpcio==1.42.0
 grpcio-tools==1.42.0
 hypothesis==6.47.4
 idna<3,>=2.5
 jsonschema[format-nongpl]<=4.17.0,>=4.14.0
```

### Comparing `bittensor-5.3.0/setup.py` & `bittensor-5.3.1/setup.py`

 * *Files identical despite different names*

