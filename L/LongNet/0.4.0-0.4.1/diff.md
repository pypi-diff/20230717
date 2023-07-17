# Comparing `tmp/LongNet-0.4.0.tar.gz` & `tmp/LongNet-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LongNet-0.4.0.tar", last modified: Fri Jul 14 20:16:25 2023, max compression
+gzip compressed data, was "LongNet-0.4.1.tar", last modified: Mon Jul 17 19:55:20 2023, max compression
```

## Comparing `LongNet-0.4.0.tar` & `LongNet-0.4.1.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 20:16:14.000000 LongNet-0.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.602744 LongNet-0.4.0/LongNet/
--rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/Transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/attention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/iterations/
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/BlocksparseDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DilatedAttentionOP.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DilatedAttentionOld.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DistributedDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/DynamicDilatedAttention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/MultiModal.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/iterations/topk.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/torchscale/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.606744 LongNet-0.4.0/LongNet/torchscale/architecture/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/encoder_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/architecture/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/component/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/droppath.py
--rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/feedforward_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/multiway_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/relative_position_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/component/xmoe/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/global_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/moe_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xmoe/routing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/component/xpos_relative_position.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/LongNet/torchscale/model/
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/model/BEiT3.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/torchscale/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-14 20:16:14.000000 LongNet-0.4.0/LongNet/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.602744 LongNet-0.4.0/LongNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-14 20:16:25.000000 LongNet-0.4.0/LongNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-14 20:16:25.610744 LongNet-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-14 20:16:14.000000 LongNet-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 20:16:25.610744 LongNet-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-14 20:16:14.000000 LongNet-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 20:16:25.610744 LongNet-0.4.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-14 20:16:14.000000 LongNet-0.4.0/test/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 19:55:10.000000 LongNet-0.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/
+-rw-r--r--   0 runner    (1001) docker     (123)    13815 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/Transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/attention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/iterations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/BlocksparseDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionOP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionOld.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionV2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DilatedAttentionv5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DistributedDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/DynamicDilatedAttention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/MultiModal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/iterations/topk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/torchscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet/torchscale/architecture/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10698 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13806 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/encoder_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/architecture/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/component/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/droppath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3640 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/feedforward_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/multiway_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/relative_position_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/component/xmoe/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/global_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/moe_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18530 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xmoe/routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/component/xpos_relative_position.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/LongNet/torchscale/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/model/BEiT3.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/torchscale/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23040 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-17 19:55:10.000000 LongNet-0.4.1/LongNet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.957530 LongNet-0.4.1/LongNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 19:55:20.000000 LongNet-0.4.1/LongNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-17 19:55:20.961530 LongNet-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-17 19:55:10.000000 LongNet-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 19:55:20.961530 LongNet-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-17 19:55:10.000000 LongNet-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 19:55:20.961530 LongNet-0.4.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-07-17 19:55:10.000000 LongNet-0.4.1/test/test.py
```

### Comparing `LongNet-0.4.0/LICENSE` & `LongNet-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/Transformer.py` & `LongNet-0.4.1/LongNet/Transformer.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
         ff_dropout = 0.,
         ff_mult = 4,
         dilation_rate = 1,  # additional parameter for DilatedAttention
         segment_size = 1,  # additional parameter for DilatedAttention
         casual = False,  # additional parameter for DilatedAttention
         use_xpos = False,  # additional parameter for DilatedAttention
         use_rel_pos_bias = False,  # additional parameter for DilatedAttention
-        distributed = False,  # additional parameter for DilatedAttention
+        # distributed = False,  # additional parameter for DilatedAttention
         rel_pos = True,
         flash_attn = False
     ):
         super().__init__()
 
         self.rotary_emb = RotaryEmbedding(dim_head) if rel_pos else None
         self.layers = nn.ModuleList([])
@@ -151,15 +151,15 @@
                     num_heads=heads, 
                     dilation_rate=dilation_rate, 
                     segment_size=segment_size, 
                     dropout=attn_dropout, 
                     casual=casual, 
                     use_xpos=use_xpos, 
                     use_rel_pos_bias=use_rel_pos_bias, 
-                    distributed=distributed
+                    # distributed=distributed
                 ), 
                 FeedForward(dim = dim, mult = ff_mult, dropout = ff_dropout)
             ]))
 
         self.norm = RMSNorm(dim)
 
     def forward(self, x):
@@ -192,15 +192,15 @@
         pos_emb = False,
         flash_attn = False,
         dilation_rate = 1,  # added
         segment_size = 0,  # added
         casual = False,  # added
         use_xpos = False,  # added
         use_rel_pos_bias = False,  # added
-        distributed = False,  # added
+        # distributed = False,  # added
     ):
         super().__init__()
 
         # simplified configuration for each stage of the hierarchy
         # depth = (2, 2, 4) would translate to depth 2 at first stage, depth 2 second stage, depth 4 third
         # max_seq_len = (16, 8, 4) would translate to max sequence length of 16 at first stage, length of 8 at second stage, length of 4 for last
 
@@ -248,15 +248,15 @@
                 ff_dropout = ff_dropout,
                 ff_mult = ff_mult,
                 dilation_rate = dilation_rate,  # added
                 segment_size = segment_size,  # added
                 casual = casual,  # added
                 use_xpos = use_xpos,  # added
                 use_rel_pos_bias = use_rel_pos_bias,  # added
-                distributed = distributed,  # added
+                # distributed = distributed,  # added
                 rel_pos = rel_pos,
                 flash_attn = flash_attn
             ))
 
             proj = nn.Identity()
 
             if exists(next_h_dim) and next_h_dim != dim:
```

### Comparing `LongNet-0.4.0/LongNet/attend.py` & `LongNet-0.4.1/LongNet/attend.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/attention.py` & `LongNet-0.4.1/LongNet/iterations/DilatedAttentionV2.py`

 * *Files 20% similar despite different names*

```diff
@@ -81,33 +81,36 @@
         # For each attention head
         for head_idx, attention in enumerate(self.attentions):
             # Calculate offset for this head
             offset = head_idx % self.dilation_rate
 
             # Apply offset and segment for this head
             x_ = x[:, offset::self.dilation_rate, :]
-            x_ = x_.contiguous().view(batch_size, 1, -1, self.segment_size, self.d_model)  # Add an extra dimension for the number of heads
+
+            #calculate the number of paddding elements needed
+            pad_len = self.segment_size - (x_.shape[1] % self.segment_size)
+            
+            #pad the sequence if necessary
+            if pad_len < self.segment_size:
+                pad = torch.zeros((batch_size, pad_len, self.d_model), device=device, dtype=dtype)
+                x_ = torch.cat([x_, pad], dim=1)
+
+            #reshape the sequence into segments
+            x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
+
+            #add an extra idmension for the number of heads
+            x_ = x_.unsqueeze(1)
 
             # Process each segment separately
             elements_attns = []
-            for idx in range(x_.shape[2]):
-                element = x_[:, :, idx, :, :].to(dtype)
+            for idx in range(x_.shape[1]):
+                element = x_[:, idx, :, :].to(dtype)
                 element_attn = attention(element, element, element)
                 elements_attns.append(element_attn)
 
-            attn_output = torch.cat(elements_attns, dim=2)
-
-
-
-            #option2
-            # elements_attns = [attention(element.to(dtype), element.to(dtype), element.to(dtype)) for element in x_]
-            # attn_output = torch.cat(elements_attns, dim=1)
-
-
-            
             # If using relative positional bias, add it
             if self.use_rel_pos_bias:
                 attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
 
             # If using casual attention, apply mask
             if self.casual:
                 mask = self.get_mask(attn_output.size(1), attn_output.size(1))
@@ -129,48 +132,7 @@
         # Apply the weights to the outputs of the different heads
         outputs_weighted = sum(w * out for w, out in zip(weights, all_head_outputs))
 
         # Return the weighted outputs
         return outputs_weighted
 
 
-
-class MultiHeadDilatedAttention:
-    def __init__():
-        pass
-
-
-
-
-
-
-
-class LongNetTransformer(nn.Module):
-    def __init__(self, d_model, num_heads, dilation_rates, segment_sizes):
-        super(LongNetTransformer, self).__init__()
-        assert len(dilation_rates) == len(segment_sizes), "dilation_rates and segment_sizes should have the same length"
-
-
-        self.d_model = d_model
-        self.num_heads = num_heads
-        self.dilation_rates = dilation_rates
-        self.segment_sizes = segment_sizes
-        
-        self.dilated_attention_layers = nn.ModuleList(
-            [DilatedAttention(d_model, num_heads, dilation_rate, segment_size)]
-            for dilation_rate, segment_size in zip(dilation_rates, segment_sizes)
-        )
-
-    def forward(self, x):
-        #accumlate outputs from different layers
-        outputs = []
-
-        #process each dilated attention layer
-        for i in range(len(self.dilated_attention_layers)):
-            output = self.dilated_attention_layers[i](x)
-            outputs.append(output)
-
-        #combine the outputs
-        output = torch.sum(torch.stack(outputs), dim=0)
-
-        return output
-
```

### Comparing `LongNet-0.4.0/LongNet/iterations/BlocksparseDilatedAttention.py` & `LongNet-0.4.1/LongNet/iterations/BlocksparseDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/iterations/DilatedAttentionOP.py` & `LongNet-0.4.1/LongNet/iterations/DilatedAttentionOP.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/iterations/DilatedAttentionOld.py` & `LongNet-0.4.1/LongNet/iterations/DilatedAttentionOld.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/iterations/DistributedDilatedAttention.py` & `LongNet-0.4.1/LongNet/iterations/DistributedDilatedAttention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/iterations/DynamicDilatedAttention.py` & `LongNet-0.4.1/LongNet/iterations/MultiModal.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 import torch 
 import torch.nn as nn
 import torch.nn.functional as F
 
 from LongNet.utils import XPOS, RelativePositionBias
-from LongNet.attend import FlashAttention
+from LongNet.attend import FlashMHA
 
-# Replace this with your correct GPU device
 device = "cuda:0"
 dtype=torch.float16
 
 
-
-
-class DynamicDilatedAttention(nn.Module):
-    def __init__(self, d_model, num_heads, num_rates, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
-        super(DynamicDilatedAttention, self).__init__()
+#second iteration the weighted sum of the different dilated + offsets for the different heads
+class DilatedAttention(nn.Module):
+    def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, casual=False, use_xpos=False, use_rel_pos_bias=False):
+        super(DilatedAttention, self).__init__()
         self.d_model = d_model
         self.num_heads = num_heads
-        self.casual = casual  # Define this before FlashAttention
 
-        # Generate geometric sequences for dilation rates and segment sizes
-        self.dilation_rates = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
-        self.segment_sizes = torch.logspace(start=0, end=num_rates-1, steps=num_rates, base=2, dtype=torch.int, device=device)
+        self.dilation_rate = dilation_rate
+        self.segment_size = segment_size
 
-        self.attention = [FlashAttention(causal=self.casual, dropout=dropout).to(device) for _ in range(num_rates)] # Corrected here]
+        self.attentions = nn.ModuleList([FlashMHA(embed_dim=d_model, num_heads=num_heads, device=device, dtype=dtype) for _ in range(self.dilation_rate)])
         self.dropout = nn.Dropout(dropout)
+        self.casual = casual
 
         self.use_xpos = use_xpos
         self.use_rel_pos_bias = use_rel_pos_bias
 
         if use_xpos:
             self.xpos = XPOS(head_dim=d_model//num_heads)
         if use_rel_pos_bias:
@@ -41,47 +38,62 @@
 
     def forward(self, x):
         batch_size, seq_len, _ = x.shape
 
         if self.use_xpos:
             x = self.xpos(x)
 
-        # Initialize tensor to store outputs
-        outputs = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
+        #collect outputs from each attention head
+        all_head_outputs = []
+        for head_idx, attention in enumerate(self.attentions):
+            offset = head_idx % self.dilation_rate
+
+            x_ = x[:, offset::self.dilation_rate, :]  # Apply offset for each head
+            x_ = x_.contiguous().view(batch_size, -1, self.segment_size, self.d_model)
+
+            attn_output, _ = attention(x_, x_, x_)
+            if self.use_rel_pos_bias:
+                attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
+
+            if self.casual:
+                mask = self.get_mask(attn_output.size(1), attn_output.size(1))
+                attn_output = attn_output.masked_fill(mask, float('-inf'))
+
+            attn_output = self.dropout(attn_output)
+
+            #resize back to original size
+            attn_output_resized = torch.zeros((batch_size, seq_len, self.d_model), device=device, dtype=dtype)
+            attn_output_resized[:, offset::self.dilation_rate, :] = attn_output.contiguous().view(batch_size, -1, self.d_model)
+            
+            all_head_outputs.append(attn_output_resized)
 
-        # Initialize tensor to store softmax denominators
-        softmax_denominators = torch.zeros((batch_size, seq_len, self.num_heads), device=device, dtype=dtype)
+        #calculate the weights for the different dilated attentions
+        weights = self.softmax(torch.tensor([1.0 / self.dilation_rate for _ in range(self.dilation_rate)], device=device, dtype=dtype))
 
-        for head_idx, attention in enumerate(self.attention):
-            dilation_rate = self.dilation_rates[head_idx]
-            segment_size = self.segment_sizes[head_idx]
-
-            for offset in range(dilation_rate):
-                x_ = x[:, offset::dilation_rate, :]  # Apply offset for each head
-                x_ = x_.contiguous().view(batch_size, -1, segment_size, self.d_model)
-
-                attn_output, attn_weights, *_ = attention(x_, x_, x_)  # Collect all additional return values into a list
-                
-                if self.use_rel_pos_bias:
-                    attn_output += self.relative_bias(batch_size, attn_output.size(1), attn_output.size(1))
-
-                if self.casual:
-                    mask = self.get_mask(attn_output.size(1), attn_output.size(1))
-                    attn_output = attn_output.masked_fill(mask, float('-inf'))
-
-                attn_output = self.dropout(attn_output)
-
-                # Add output to the corresponding positions in the outputs tensor
-                outputs[:, offset::dilation_rate, :] += attn_output.contiguous().view(batch_size, -1, self.d_model)
-                
-                # Add softmax denominators to the corresponding positions in the softmax_denominators tensor
-                softmax_denominators[:, offset::dilation_rate, :] += attn_weights.sum(dim=-1)
+        #apply the weights to the outputs of the different heads
+        outputs_weighted = sum(w * out for w, out in zip(weights, all_head_outputs))
+
+        return outputs_weighted
 
-        # Calculate the weights for the different dilated attentions
-        weights = self.softmax(softmax_denominators)
 
-        # Apply the weights to the outputs
-        outputs_weighted = weights * outputs
 
-        return outputs_weighted
 
+class MultiModalDilationAttention(nn.Module):
+    def __init__(self, d_model, num_heads, dilation_rate, segment_size, dropout=0.0, casual=False, num_modalities=2):
+        super(MultiModalDilationAttention, self).__init__()
+
+        self.d_model = d_model
+        self.num_modalities = num_modalities
+        self.dilated_attns = nn.ModuleList(
+            [DilatedAttention(d_model, num_heads, dilation_rate, segment_size, dropout, casual) for _ in range(num_modalities)]
+        )
+        self.cross_modality_attn = DilatedAttention(num_modalities * d_model, num_heads, dilation_rate, segment_size, dropout, casual)
+
+    def forward(self, x):
+        modality_outputs = []
+        for modality_data, attn in zip(x, self.dilated_attns):
+            modality_outputs.append(attn(modality_data))
+        
+        cross_modality_input = torch.cat(modality_outputs, dim=-1)
+        cross_modality_output = self.cross_modality_attn_(cross_modality_input)
 
+        return cross_modality_output
```

### Comparing `LongNet-0.4.0/LongNet/iterations/topk.py` & `LongNet-0.4.1/LongNet/iterations/topk.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/model.py` & `LongNet-0.4.1/LongNet/model.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/architecture/config.py` & `LongNet-0.4.1/LongNet/torchscale/architecture/config.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/architecture/decoder.py` & `LongNet-0.4.1/LongNet/torchscale/architecture/decoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/architecture/encoder.py` & `LongNet-0.4.1/LongNet/torchscale/architecture/encoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/architecture/encoder_decoder.py` & `LongNet-0.4.1/LongNet/torchscale/architecture/encoder_decoder.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/architecture/utils.py` & `LongNet-0.4.1/LongNet/torchscale/architecture/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/droppath.py` & `LongNet-0.4.1/LongNet/torchscale/component/droppath.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/embedding.py` & `LongNet-0.4.1/LongNet/torchscale/component/embedding.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/feedforward_network.py` & `LongNet-0.4.1/LongNet/torchscale/component/feedforward_network.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/multihead_attention.py` & `LongNet-0.4.1/LongNet/torchscale/component/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/multiway_network.py` & `LongNet-0.4.1/LongNet/torchscale/component/multiway_network.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/relative_position_bias.py` & `LongNet-0.4.1/LongNet/torchscale/component/relative_position_bias.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/xmoe/global_groups.py` & `LongNet-0.4.1/LongNet/torchscale/component/xmoe/global_groups.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/xmoe/moe_layer.py` & `LongNet-0.4.1/LongNet/torchscale/component/xmoe/moe_layer.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/xmoe/routing.py` & `LongNet-0.4.1/LongNet/torchscale/component/xmoe/routing.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/component/xpos_relative_position.py` & `LongNet-0.4.1/LongNet/torchscale/component/xpos_relative_position.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/torchscale/model/BEiT3.py` & `LongNet-0.4.1/LongNet/torchscale/model/BEiT3.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/training.py` & `LongNet-0.4.1/LongNet/training.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet/utils.py` & `LongNet-0.4.1/LongNet/utils.py`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/LongNet.egg-info/PKG-INFO` & `LongNet-0.4.1/LongNet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.4.0
+Version: 0.4.1
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.4.0/LongNet.egg-info/SOURCES.txt` & `LongNet-0.4.1/LongNet.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 LongNet.egg-info/SOURCES.txt
 LongNet.egg-info/dependency_links.txt
 LongNet.egg-info/requires.txt
 LongNet.egg-info/top_level.txt
 LongNet/iterations/BlocksparseDilatedAttention.py
 LongNet/iterations/DilatedAttentionOP.py
 LongNet/iterations/DilatedAttentionOld.py
+LongNet/iterations/DilatedAttentionV2.py
+LongNet/iterations/DilatedAttentionv5.py
 LongNet/iterations/DistributedDilatedAttention.py
 LongNet/iterations/DynamicDilatedAttention.py
 LongNet/iterations/MultiModal.py
 LongNet/iterations/__init__.py
 LongNet/iterations/topk.py
 LongNet/torchscale/__init__.py
 LongNet/torchscale/architecture/__init__.py
```

### Comparing `LongNet-0.4.0/PKG-INFO` & `LongNet-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LongNet
-Version: 0.4.0
+Version: 0.4.1
 Summary: LongNet - Pytorch
 Home-page: https://github.com/kyegomez/LongNet
 Author: Kye Gomez
 Author-email: kye@apac.ai
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering
 Classifier: Development Status :: 4 - Beta
```

### Comparing `LongNet-0.4.0/README.md` & `LongNet-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `LongNet-0.4.0/setup.py` & `LongNet-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 # 
 
 setup(
   name = 'LongNet',
   packages = find_packages(exclude=[]),
-  version = '0.4.0',
+  version = '0.4.1',
   license='MIT',
   description = 'LongNet - Pytorch',
   author = 'Kye Gomez',
   author_email = 'kye@apac.ai',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/kyegomez/LongNet',
   keywords = [
```

### Comparing `LongNet-0.4.0/test/test.py` & `LongNet-0.4.1/test/test.py`

 * *Files identical despite different names*

