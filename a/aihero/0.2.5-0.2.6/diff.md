# Comparing `tmp/aihero-0.2.5.tar.gz` & `tmp/aihero-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aihero-0.2.5.tar", last modified: Thu Jul 13 15:08:09 2023, max compression
+gzip compressed data, was "aihero-0.2.6.tar", last modified: Mon Jul 17 06:22:27 2023, max compression
```

## Comparing `aihero-0.2.5.tar` & `aihero-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.096153 aihero-0.2.5/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.5/LICENSE
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 15:08:09.096412 aihero-0.2.5/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.5/README.md
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.092381 aihero-0.2.5/aihero/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       29 2023-07-12 04:51:12.000000 aihero-0.2.5/aihero/__init__.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 14:51:50.000000 aihero-0.2.5/aihero/client.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.5/aihero/exceptions.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.5/aihero/openai_helper.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1202 2023-07-13 14:38:04.000000 aihero-0.2.5/aihero/project.py
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     5086 2023-07-13 14:49:15.000000 aihero-0.2.5/aihero/promptstash.py
-drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-13 15:08:09.095618 aihero-0.2.5/aihero.egg-info/
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/PKG-INFO
--rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/SOURCES.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/dependency_links.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        6 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/requires.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-13 15:08:09.000000 aihero-0.2.5/aihero.egg-info/top_level.txt
--rw-r--r--   0 rahulparundekar   (501) staff       (20)     1009 2023-07-13 15:08:09.097592 aihero-0.2.5/setup.cfg
--rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.5/setup.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.047639 aihero-0.2.6/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1072 2023-07-10 05:44:36.000000 aihero-0.2.6/LICENSE
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-17 06:22:27.047899 aihero-0.2.6/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      395 2023-07-13 06:32:11.000000 aihero-0.2.6/README.md
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.040615 aihero-0.2.6/aihero/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      242 2023-07-14 19:26:45.000000 aihero-0.2.6/aihero/__init__.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     3143 2023-07-13 14:51:50.000000 aihero-0.2.6/aihero/client.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      402 2023-07-10 05:44:36.000000 aihero-0.2.6/aihero/exceptions.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     2158 2023-07-12 04:51:12.000000 aihero-0.2.6/aihero/openai_helper.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1202 2023-07-13 14:38:04.000000 aihero-0.2.6/aihero/project.py
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     4919 2023-07-15 17:44:18.000000 aihero-0.2.6/aihero/promptstash.py
+drwxr-xr-x   0 rahulparundekar   (501) staff       (20)        0 2023-07-17 06:22:27.046991 aihero-0.2.6/aihero.egg-info/
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1371 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/PKG-INFO
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)      306 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/SOURCES.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        1 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/dependency_links.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       13 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/requires.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)        7 2023-07-17 06:22:27.000000 aihero-0.2.6/aihero.egg-info/top_level.txt
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)     1017 2023-07-17 06:22:27.048884 aihero-0.2.6/setup.cfg
+-rw-r--r--   0 rahulparundekar   (501) staff       (20)       69 2023-07-10 05:44:36.000000 aihero-0.2.6/setup.py
```

### Comparing `aihero-0.2.5/LICENSE` & `aihero-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aihero-0.2.5/PKG-INFO` & `aihero-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.5
+Version: 0.2.6
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.5/aihero/client.py` & `aihero-0.2.6/aihero/client.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.5/aihero/openai_helper.py` & `aihero-0.2.6/aihero/openai_helper.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.5/aihero/project.py` & `aihero-0.2.6/aihero/project.py`

 * *Files identical despite different names*

### Comparing `aihero-0.2.5/aihero/promptstash.py` & `aihero-0.2.6/aihero/promptstash.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,128 +10,130 @@
         self,
         project_id: str,
         client: Client,
     ):
         self._project_id = project_id
         self._client = client
 
-    def variant(
+    def stash_template(
         self,
         template_id: str,
-        variant: str = None,
         body: str = None,
         name: str = None,
         description: str = None,
         prompt_format: str = "f-string",
         sections: str = None,
         author: str = None,
         other: dict = None,
     ):
-        if variant is None and body is None:
+        prompt_template_dict = {
+            "body": body,
+            "prompt_format": prompt_format,
+            "sections": {},
+            "author": "",
+            "other": {},
+        }
+        if name:
+            prompt_template_dict["name"] = name
+        if description:
+            prompt_template_dict["description"] = description
+        if sections:
+            prompt_template_dict["sections"] = sections
+        if author:
+            prompt_template_dict["author"] = author
+        if other:
+            prompt_template_dict["other"] = other
+        # No variant found
+        prompt_template_dict = self._client.post(
+            f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}",
+            obj=prompt_template_dict,
+            error_msg=f"Couldn't stash prompt template {template_id} for project {self._project_id}",
+            network_errors={
+                400: "Please check the prompt_variant or the arguments.",
+                403: f"Could not access project {self._project_id}. Please check the API key.",
+            },
+        )
+        return prompt_template_dict["variant"]
+
+    def variant(self, template_id: str, variant: str = None):
+        if variant is None:
             prompt_template_dict = self._client.get(
                 f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}",
                 error_msg=f"Could fetch prompt template {template_id} for project {self._project_id}",
                 network_errors={
                     400: "Please check the prompt_template_id.",
                     403: f"Could not access project {self._project_id}. Please check the API key.",
                 },
             )
         else:
-            if variant:
-                prompt_template_dict = self._client.get(
-                    f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}/variants/{variant}",
-                    error_msg=f"Could fetch variant {variant} of prompt template {template_id} for project {self._project_id}",
-                    network_errors={
-                        400: "Please check the prompt_variant.",
-                        403: f"Could not access project {self._project_id}. Please check the API key.",
-                    },
-                )
-            else:
-                prompt_template_dict = {
-                    "body": body,
-                    "prompt_format": prompt_format,
-                    "sections": {},
-                    "author": "",
-                    "other": {},
-                }
-                if name:
-                    prompt_template_dict["name"] = name
-                if description:
-                    prompt_template_dict["description"] = description
-                if sections:
-                    prompt_template_dict["sections"] = sections
-                if author:
-                    prompt_template_dict["author"] = author
-                if other:
-                    prompt_template_dict["other"] = other
-                # No variant found
-                prompt_template_dict = self._client.post(
-                    f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}",
-                    obj=prompt_template_dict,
-                    error_msg=f"Could update variant {variant} of prompt template {template_id} for project {self._project_id}",
-                    network_errors={
-                        400: "Please check the prompt_variant or the arguments.",
-                        403: f"Could not access project {self._project_id}. Please check the API key.",
-                    },
-                )
-            return prompt_template_dict["variant"], prompt_template_dict["template"]
+            prompt_template_dict = self._client.get(
+                f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}/variants/{variant}",
+                error_msg=f"Could fetch variant {variant} of prompt template {template_id} for project {self._project_id}",
+                network_errors={
+                    400: "Please check the prompt_variant.",
+                    403: f"Could not access project {self._project_id}. Please check the API key.",
+                },
+            )
+            return prompt_template_dict["template"]
 
-    def _sync_stash(
+    def _sync_stash_completion(
         self,
         template_id: str,
         variant: str,
+        inputs: str,
         prompt: str,
         output: str,
-        inputs: str = None,
+        trace_id: str = None,
         other: dict = None,
     ):
+        inputs_embedding, err = get_embedding(inputs)
+        if err:
+            warn("Error generating embedding for inputs in child thread.")
+            raise AIHeroException(err)
         prompt_embedding, err = get_embedding(prompt)
         if err:
             warn("Error generating embedding for prompt in child thread.")
             raise AIHeroException(err)
         output_embedding, err = get_embedding(output)
         if err:
             warn("Error generating embedding for output in child thread.")
             raise AIHeroException(err)
 
         stash_obj = {
+            "inputs": inputs,
             "prompt": prompt,
             "output": output,
+            "inputs_embedding": inputs_embedding,
             "prompt_embedding": prompt_embedding,
             "output_embedding": output_embedding,
+            "trace_id": trace_id,
         }
 
-        if inputs:
-            inputs_embedding, err = get_embedding(inputs)
-            if err:
-                warn("Error generating embedding for output in child thread.")
-                raise AIHeroException(err)
-            stash_obj["inputs"] = inputs
-            stash_obj["inputs_embedding"] = inputs_embedding
-
         if other is None:
             other = {}
         other.update({"embedding_model": "text-embedding-ada-002"})
         stash_obj["other"] = other
 
         self._client.post(
             f"/tools/promptstash/projects/{self._project_id}/prompt_templates/{template_id}/variants/{variant}/stash",
             obj=stash_obj,
             timeout=30,
         )
         print("Prompt stashed.")
 
-    def stash(
+    def stash_completion(
         self,
+        template_id: str,
         variant: str,
+        inputs: str,
         prompt: str,
         output: str,
-        inputs: str = None,
         other: dict = None,
+        trace_id: str = None,
     ):
         if has_key():
             Thread(
-                target=self._sync_stash,
-                args=(variant, prompt, output, inputs, other),
+                target=self._sync_stash_completion,
+                args=(template_id, variant, prompt, output, inputs, trace_id, other),
             ).start()
         else:
             raise AIHeroException("No OPENAI_API_KEY in env variables.")
```

### Comparing `aihero-0.2.5/aihero.egg-info/PKG-INFO` & `aihero-0.2.6/aihero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aihero
-Version: 0.2.5
+Version: 0.2.6
 Summary: AI Hero Python SDK
 Home-page: https://github.com/ai-hero/python-client-sdk
 Author: AI Hero Team
 Author-email: team@aihero.studio
 License: MIT
 Keywords: AI Hero,Spotcheck,MLOps,AI,Data Annotation,Labeling,Model Training,Model Serving,Model Deployment
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aihero-0.2.5/setup.cfg` & `aihero-0.2.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = aihero
-version = 0.2.5
+version = 0.2.6
 description = AI Hero Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ai-hero/python-client-sdk
 author = AI Hero Team
 author_email = team@aihero.studio
 license = MIT
@@ -23,12 +23,13 @@
 	Topic :: Software Development :: Libraries
 keywords = AI Hero, Spotcheck, MLOps, AI, Data Annotation, Labeling, Model Training, Model Serving, Model Deployment
 
 [options]
 packages = aihero
 install_requires = 
 	httpx
+	openai
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

