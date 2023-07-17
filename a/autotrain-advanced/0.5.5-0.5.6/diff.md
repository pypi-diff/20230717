# Comparing `tmp/autotrain-advanced-0.5.5.tar.gz` & `tmp/autotrain-advanced-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autotrain-advanced-0.5.5.tar", last modified: Tue Jul 11 12:12:53 2023, max compression
+gzip compressed data, was "autotrain-advanced-0.5.6.tar", last modified: Mon Jul 17 12:38:46 2023, max compression
```

## Comparing `autotrain-advanced-0.5.5.tar` & `autotrain-advanced-0.5.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.5/LICENSE
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.5/README.md
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/setup.cfg
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.5/setup.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-11 12:12:45.000000 autotrain-advanced-0.5.5/src/autotrain/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38472 2023-06-21 11:15:37.000000 autotrain-advanced-0.5.5/src/autotrain/app.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/cli/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.5/src/autotrain/cli/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.5/src/autotrain/cli/autotrain.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.5/src/autotrain/cli/run_app.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14109 2023-07-11 10:08:31.000000 autotrain-advanced-0.5.5/src/autotrain/cli/run_llm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.5/src/autotrain/config.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/dataset.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.5/src/autotrain/help.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.5/src/autotrain/languages.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.5/src/autotrain/params.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/preprocessor/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/tabular.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/text.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.5/src/autotrain/preprocessor/vision.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/project.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.5/src/autotrain/splits.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.5/src/autotrain/tasks.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain/trainers/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/__init__.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/callbacks.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9966 2023-07-11 12:12:06.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/clm.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-06-20 15:50:18.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/dreambooth.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/image_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/lm_trainer.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/text_classification.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5525 2023-07-11 12:12:21.000000 autotrain-advanced-0.5.5/src/autotrain/trainers/utils.py
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.5/src/autotrain/utils.py
-drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-11 12:12:53.809706 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/PKG-INFO
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1187 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/SOURCES.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/dependency_links.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/entry_points.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3057 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/requires.txt
--rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-11 12:12:53.000000 autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/top_level.txt
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    11357 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.6/LICENSE
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      485 2023-01-05 12:49:14.000000 autotrain-advanced-0.5.6/README.md
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      354 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/setup.cfg
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2130 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.6/setup.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/autotrain/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      691 2023-07-17 12:38:35.000000 autotrain-advanced-0.5.6/src/autotrain/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    38466 2023-07-17 12:32:57.000000 autotrain-advanced-0.5.6/src/autotrain/app.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/autotrain/cli/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      310 2023-02-01 13:00:34.000000 autotrain-advanced-0.5.6/src/autotrain/cli/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      937 2023-07-06 09:04:02.000000 autotrain-advanced-0.5.6/src/autotrain/cli/autotrain.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1268 2023-06-21 11:15:59.000000 autotrain-advanced-0.5.6/src/autotrain/cli/run_app.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-07-13 15:03:01.000000 autotrain-advanced-0.5.6/src/autotrain/cli/run_dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14109 2023-07-11 10:08:31.000000 autotrain-advanced-0.5.6/src/autotrain/cli/run_llm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      306 2023-04-29 09:05:02.000000 autotrain-advanced-0.5.6/src/autotrain/config.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    12533 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.6/src/autotrain/dataset.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1483 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.6/src/autotrain/help.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)      197 2023-04-14 11:28:41.000000 autotrain-advanced-0.5.6/src/autotrain/languages.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    17211 2023-06-21 06:25:20.000000 autotrain-advanced-0.5.6/src/autotrain/params.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/autotrain/preprocessor/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-02-11 08:10:09.000000 autotrain-advanced-0.5.6/src/autotrain/preprocessor/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1741 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.6/src/autotrain/preprocessor/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     3991 2023-04-29 09:05:23.000000 autotrain-advanced-0.5.6/src/autotrain/preprocessor/tabular.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9231 2023-04-29 09:05:46.000000 autotrain-advanced-0.5.6/src/autotrain/preprocessor/text.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     6549 2023-05-31 09:41:05.000000 autotrain-advanced-0.5.6/src/autotrain/preprocessor/vision.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8164 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.6/src/autotrain/project.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       64 2023-01-05 12:46:52.000000 autotrain-advanced-0.5.6/src/autotrain/splits.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2779 2023-04-25 18:01:52.000000 autotrain-advanced-0.5.6/src/autotrain/tasks.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/autotrain/trainers/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        0 2023-06-15 09:39:07.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/__init__.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1305 2023-07-05 07:53:30.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/callbacks.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9966 2023-07-11 12:12:06.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/clm.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    34306 2023-06-20 15:50:18.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/dreambooth.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    10026 2023-06-20 11:50:06.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/image_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)    14726 2023-06-22 02:39:49.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/lm_trainer.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     9119 2023-06-20 09:52:02.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/text_classification.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     5525 2023-07-13 15:02:50.000000 autotrain-advanced-0.5.6/src/autotrain/trainers/utils.py
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     8242 2023-06-21 11:52:51.000000 autotrain-advanced-0.5.6/src/autotrain/utils.py
+drwxrwxr-x   0 abhishek  (1000) abhishek  (1000)        0 2023-07-17 12:38:46.487667 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1462 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/PKG-INFO
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     1223 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/SOURCES.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)        1 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/dependency_links.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       59 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/entry_points.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)     2849 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/requires.txt
+-rw-rw-r--   0 abhishek  (1000) abhishek  (1000)       10 2023-07-17 12:38:46.000000 autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/top_level.txt
```

### Comparing `autotrain-advanced-0.5.5/LICENSE` & `autotrain-advanced-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/PKG-INFO` & `autotrain-advanced-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.5/setup.py` & `autotrain-advanced-0.5.6/setup.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/__init__.py` & `autotrain-advanced-0.5.6/src/autotrain/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,8 +12,8 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 # Lint as: python3
 # pylint: enable=line-too-long
 
-__version__ = "0.5.5"
+__version__ = "0.5.6"
```

### Comparing `autotrain-advanced-0.5.5/src/autotrain/app.py` & `autotrain-advanced-0.5.6/src/autotrain/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -540,15 +540,15 @@
                     autotrain_username = gr.Dropdown(
                         label="AutoTrain Username",
                         choices=who_is_training,
                         value=who_is_training[0] if who_is_training else "",
                     )
                     autotrain_backend = gr.Dropdown(
                         label="AutoTrain Backend",
-                        choices=["HuggingFace Internal", "HuggingFace Spaces/Local"],
+                        choices=["HuggingFace Internal", "HuggingFace Spaces"],
                         value="HuggingFace Internal",
                         interactive=True,
                     )
                 with gr.Row():
                     project_name = gr.Textbox(label="Project name", value="", lines=1, max_lines=1, interactive=True)
                     project_type = gr.Dropdown(
                         label="Project Type", choices=list(APP_TASKS.keys()), value=list(APP_TASKS.keys())[0]
```

### Comparing `autotrain-advanced-0.5.5/src/autotrain/cli/autotrain.py` & `autotrain-advanced-0.5.6/src/autotrain/cli/autotrain.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/cli/run_app.py` & `autotrain-advanced-0.5.6/src/autotrain/cli/run_app.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/cli/run_llm.py` & `autotrain-advanced-0.5.6/src/autotrain/cli/run_llm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/dataset.py` & `autotrain-advanced-0.5.6/src/autotrain/dataset.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/help.py` & `autotrain-advanced-0.5.6/src/autotrain/help.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/params.py` & `autotrain-advanced-0.5.6/src/autotrain/params.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/preprocessor/dreambooth.py` & `autotrain-advanced-0.5.6/src/autotrain/preprocessor/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/preprocessor/tabular.py` & `autotrain-advanced-0.5.6/src/autotrain/preprocessor/tabular.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/preprocessor/text.py` & `autotrain-advanced-0.5.6/src/autotrain/preprocessor/text.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/preprocessor/vision.py` & `autotrain-advanced-0.5.6/src/autotrain/preprocessor/vision.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/project.py` & `autotrain-advanced-0.5.6/src/autotrain/project.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/tasks.py` & `autotrain-advanced-0.5.6/src/autotrain/tasks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/callbacks.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/callbacks.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/clm.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/clm.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/dreambooth.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/dreambooth.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/image_classification.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/image_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/lm_trainer.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/lm_trainer.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/text_classification.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/text_classification.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/trainers/utils.py` & `autotrain-advanced-0.5.6/src/autotrain/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain/utils.py` & `autotrain-advanced-0.5.6/src/autotrain/utils.py`

 * *Files identical despite different names*

### Comparing `autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/PKG-INFO` & `autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autotrain-advanced
-Version: 0.5.5
+Version: 0.5.6
 Home-page: https://github.com/huggingface/autotrain-advanced
 Download-URL: https://github.com/huggingface/autotrain-advanced/tags
 Author: HuggingFace Inc.
 Author-email: autotrain@huggingface.co
 License: Apache 2.0
 Keywords: automl autonlp autotrain huggingface
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `autotrain-advanced-0.5.5/src/autotrain_advanced.egg-info/SOURCES.txt` & `autotrain-advanced-0.5.6/src/autotrain_advanced.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/autotrain/project.py
 src/autotrain/splits.py
 src/autotrain/tasks.py
 src/autotrain/utils.py
 src/autotrain/cli/__init__.py
 src/autotrain/cli/autotrain.py
 src/autotrain/cli/run_app.py
+src/autotrain/cli/run_dreambooth.py
 src/autotrain/cli/run_llm.py
 src/autotrain/preprocessor/__init__.py
 src/autotrain/preprocessor/dreambooth.py
 src/autotrain/preprocessor/tabular.py
 src/autotrain/preprocessor/text.py
 src/autotrain/preprocessor/vision.py
 src/autotrain/trainers/__init__.py
```

