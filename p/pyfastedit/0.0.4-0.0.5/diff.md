# Comparing `tmp/pyfastedit-0.0.4.tar.gz` & `tmp/pyfastedit-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfastedit-0.0.4.tar", last modified: Tue Jul 11 14:34:14 2023, max compression
+gzip compressed data, was "pyfastedit-0.0.5.tar", last modified: Mon Jul 17 17:11:40 2023, max compression
```

## Comparing `pyfastedit-0.0.4.tar` & `pyfastedit-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5113 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/README.md
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.222572 pyfastedit-0.0.4/fastedit/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2462 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/editor.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.326572 pyfastedit-0.0.4/fastedit/rome/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/rome/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2710 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/compute_u.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8776 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/compute_v.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5243 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/repr_tools.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2853 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/rome_hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6092 2023-07-11 14:33:46.000000 pyfastedit-0.0.4/fastedit/rome/rome_main.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.402572 pyfastedit-0.0.4/fastedit/utils/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      698 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/context.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1987 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/generate.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      361 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/hparams.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      755 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/mtloader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/nethook.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/prints.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1863 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/fastedit/utils/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-11 14:34:14.406572 pyfastedit-0.0.4/pyfastedit.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      626 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-11 14:34:13.000000 pyfastedit-0.0.4/pyfastedit.egg-info/top_level.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-11 14:34:14.410572 pyfastedit-0.0.4/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-11 14:33:47.000000 pyfastedit-0.0.4/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:11:40.141464 pyfastedit-0.0.5/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-17 17:11:40.141464 pyfastedit-0.0.5/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5113 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/README.md
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:11:39.865465 pyfastedit-0.0.5/fastedit/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       81 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2865 2023-07-17 17:10:05.000000 pyfastedit-0.0.5/fastedit/editor.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:11:39.977465 pyfastedit-0.0.5/fastedit/rome/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       60 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/rome/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2710 2023-07-17 17:10:05.000000 pyfastedit-0.0.5/fastedit/rome/compute_u.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8874 2023-07-17 17:10:05.000000 pyfastedit-0.0.5/fastedit/rome/compute_v.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5243 2023-07-17 17:10:05.000000 pyfastedit-0.0.5/fastedit/rome/repr_tools.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3027 2023-07-17 17:10:05.000000 pyfastedit-0.0.5/fastedit/rome/rome_hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6092 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/rome/rome_main.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:11:40.089464 pyfastedit-0.0.5/fastedit/utils/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      698 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/context.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1987 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/generate.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      361 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/hparams.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1581 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/mtloader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    15518 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/nethook.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      727 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/prints.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1863 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/fastedit/utils/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-07-17 17:11:40.137464 pyfastedit-0.0.5/pyfastedit.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6054 2023-07-17 17:11:39.000000 pyfastedit-0.0.5/pyfastedit.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      626 2023-07-17 17:11:39.000000 pyfastedit-0.0.5/pyfastedit.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-07-17 17:11:39.000000 pyfastedit-0.0.5/pyfastedit.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       90 2023-07-17 17:11:39.000000 pyfastedit-0.0.5/pyfastedit.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-07-17 17:11:39.000000 pyfastedit-0.0.5/pyfastedit.egg-info/top_level.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-07-17 17:11:40.141464 pyfastedit-0.0.5/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1830 2023-07-17 17:10:06.000000 pyfastedit-0.0.5/setup.py
```

### Comparing `pyfastedit-0.0.4/LICENSE` & `pyfastedit-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/PKG-INFO` & `pyfastedit-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyfastedit-0.0.4/README.md` & `pyfastedit-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/editor.py` & `pyfastedit-0.0.5/fastedit/editor.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,55 +6,58 @@
 from .rome import ROMEHyperParams, apply_rome_to_model
 from .utils.prints import print_loud
 from .utils.template import Template
 from .utils.mtloader import load_model_and_tokenizer
 from .utils.generate import generate_fast, generate_interactive
 
 
-def test_rome(data: str, model: str, config: str, template: Optional[str] = "default") -> None:
+def test_rome(
+    data: str, model: str, config: str, template: Optional[str] = "default",
+    output: Optional[str] = None, checkpointing: Optional[bool] = False
+) -> None:
     r"""
     Edits a pre-trained model using model-editing algorithms.
 
     Args:
         data (`str`):
             The path of the `json` file containing the samples for editing.
         model (`str`):
             The name or path of the pre-trained transformer model to be edited.
         config (`str`):
             The name of the hyper-parameters to use for editing the model.
         template (`str`, *optional*, defaults to `default`):
             The name of the template to use in generation.
-
-    Returns:
-        diff_weights (`Dict[str, Tensor]`):
-            A dict of diff weights that have been changed.
+        output (`str`, *optional*, defaults to `None`):
+            The path to save the edited model.
+        checkpointing (`bool`, *optional*, defaults to `False`):
+            Whether to enable gradient checkpointing or not.
     """
 
     assert os.path.exists(data), "data not found"
 
     with open(data, "r", encoding="utf-8") as f:
         requests = json.load(f)
 
     queries = [query for request in requests for query in request["queries"]]
 
-    model, tokenizer, batch_first = load_model_and_tokenizer(model)
+    model_old, tokenizer, batch_first = load_model_and_tokenizer(model, checkpointing)
     template = Template(name=template)
 
     print_loud("Retrieving hyperparameters")
     hparams = ROMEHyperParams.from_name(config)
     print(hparams)
 
     if len(queries) > 0:
         print_loud("Generating pre-update text")
-        pre_update_text = generate_fast(model, tokenizer, queries, template, max_length=100)
+        pre_update_text = generate_fast(model_old, tokenizer, queries, template, max_length=100)
         print("\n\n".join([queries[i] + " " + pre_update_text[i] for i in range(len(queries))]))
 
     print_loud(f"Applying rome to model")
     model_new, _ = apply_rome_to_model(
-        model,
+        model_old,
         tokenizer,
         requests,
         hparams,
         batch_first,
         return_diff_weights=False
     )
 
@@ -62,10 +65,15 @@
         print_loud("Generating post-update text")
         post_update_text = generate_fast(model_new, tokenizer, queries, template, max_length=100)
         print("\n\n".join([queries[i] + " " + post_update_text[i] for i in range(len(queries))]))
 
     print_loud("Starting interactively generation interface")
     generate_interactive(model_new, tokenizer, template)
 
+    if output is not None:
+        model_new.config.use_cache = True
+        model_new.save_pretrained(output, max_shard_size="10GB")
+        tokenizer.save_pretrained(output)
+
 
 if __name__ == "__main__":
     fire.Fire(test_rome)
```

### Comparing `pyfastedit-0.0.4/fastedit/rome/compute_u.py` & `pyfastedit-0.0.5/fastedit/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/rome/compute_v.py` & `pyfastedit-0.0.5/fastedit/rome/compute_v.py`

 * *Files 4% similar despite different names*

```diff
@@ -115,15 +115,15 @@
         nll_loss_each = -(loss * mask).sum(dim=1) / target_len
         nll_loss = nll_loss_each.mean()
         kl_loss = torch.nn.functional.kl_div(kl_distr_init, kl_log_probs, log_target=True, reduction="batchmean")
         kl_loss *= hparams.kl_factor
         loss = nll_loss + kl_loss
         print(f"loss {np.round(loss.item(), 3)} = "
               f"{np.round(nll_loss.item(), 3)} + {np.round(kl_loss.item(), 3)} "
-              f"avg prob of [{request['target']}] {torch.exp(-nll_loss_each).mean().item()}")
+              f"avg prob of [{request['target']}] {np.round(torch.exp(-nll_loss_each).mean().item(), 4)}")
 
         if loss < 5e-3: # early-stopping
             break
 
         if it == hparams.v_num_grad_steps - 1:
             break
 
@@ -150,19 +150,19 @@
         module_template=hparams.rewrite_module_tmp,
         fact_token_strategy=hparams.fact_token,
         batch_first=batch_first
     )
 
     # Solving the linear system to compute the right vector
     right_vector = (target - cur_output) / torch.dot(cur_input, left_vector)
-    print(f"Delta norm: {(target - cur_output).norm().item()}")
-    print(f"Change in target norm: {target_init.norm().item()} to {target.norm().item()} => "
-          f"{(target.norm() - target_init.norm()).item()}")
-    print(f"Division Factor: {torch.dot(cur_input, left_vector).item()}")
-    print(f"Right vector norm: {right_vector.norm()}")
+    print(f"Delta norm: {np.round((target - cur_output).norm().item(), 3)}")
+    print(f"Change in target norm: {np.round(target_init.norm().item(), 3)} to {np.round(target.norm().item(), 3)} => "
+          f"{np.round((target.norm() - target_init.norm()).item(), 3)}")
+    print(f"Division Factor: {np.round(torch.dot(cur_input, left_vector).item(), 3)}")
+    print(f"Right vector norm: {np.round(right_vector.norm().item(), 3)}")
 
     return right_vector
 
 
 def get_module_input_output_at_word(
     model: PreTrainedModel,
     tokenizer: PreTrainedTokenizer,
```

### Comparing `pyfastedit-0.0.4/fastedit/rome/repr_tools.py` & `pyfastedit-0.0.5/fastedit/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/rome/rome_hparams.py` & `pyfastedit-0.0.5/fastedit/rome/rome_hparams.py`

 * *Files 8% similar despite different names*

```diff
@@ -52,23 +52,29 @@
             mom2_n_samples=100000,
             mom2_dtype="float16"
         )
 
         if name == "gpj-j-6b":
             pass
         elif name == "llama-7b":
+            r"""
+            Supports: LLaMA-7B, Baichuan-7B, InternLM-7B...
+            """
             data.update(dict(
                 v_loss_layer=31,
                 rewrite_module_tmp="model.layers.{}.mlp.down_proj",
                 layer_module_tmp="model.layers.{}",
                 mlp_module_tmp="model.layers.{}.mlp",
                 attn_module_tmp="model.layers.{}.self_attn",
                 ln_f_module="model.norm"
             ))
         elif name == "llama-13b":
+            r"""
+            Supports LLaMA-13B, Baichuan-13B...
+            """
             data.update(dict(
                 layers=[10],
                 v_loss_layer=39,
                 rewrite_module_tmp="model.layers.{}.mlp.down_proj",
                 layer_module_tmp="model.layers.{}",
                 mlp_module_tmp="model.layers.{}.mlp",
                 attn_module_tmp="model.layers.{}.self_attn",
```

### Comparing `pyfastedit-0.0.4/fastedit/rome/rome_main.py` & `pyfastedit-0.0.5/fastedit/rome/rome_main.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/utils/context.py` & `pyfastedit-0.0.5/fastedit/utils/context.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/utils/generate.py` & `pyfastedit-0.0.5/fastedit/utils/generate.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/utils/nethook.py` & `pyfastedit-0.0.5/fastedit/utils/nethook.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/utils/prints.py` & `pyfastedit-0.0.5/fastedit/utils/prints.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/fastedit/utils/template.py` & `pyfastedit-0.0.5/fastedit/utils/template.py`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/pyfastedit.egg-info/PKG-INFO` & `pyfastedit-0.0.5/pyfastedit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfastedit
-Version: 0.0.4
+Version: 0.0.5
 Summary: Editing large language models within 10 seconds
 Home-page: https://github.com/hiyouga/FastEdit
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyfastedit-0.0.4/pyfastedit.egg-info/SOURCES.txt` & `pyfastedit-0.0.5/pyfastedit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyfastedit-0.0.4/setup.py` & `pyfastedit-0.0.5/setup.py`

 * *Files identical despite different names*

