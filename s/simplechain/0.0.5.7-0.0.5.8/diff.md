# Comparing `tmp/simplechain-0.0.5.7.tar.gz` & `tmp/simplechain-0.0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplechain-0.0.5.7.tar", last modified: Tue May 16 02:03:38 2023, max compression
+gzip compressed data, was "simplechain-0.0.5.8.tar", last modified: Mon Jul 17 00:58:39 2023, max compression
```

## Comparing `simplechain-0.0.5.7.tar` & `simplechain-0.0.5.8.tar`

### file list

```diff
@@ -1,66 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.474006 simplechain-0.0.5.7/
--rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.7/LICENSE
--rw-rw-rw-   0        0        0      602 2023-05-16 02:03:38.473005 simplechain-0.0.5.7/PKG-INFO
--rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.7/README.rst
--rw-rw-rw-   0        0        0       42 2023-05-16 02:03:38.474006 simplechain-0.0.5.7/setup.cfg
--rw-rw-rw-   0        0        0     1105 2023-05-16 02:03:21.000000 simplechain-0.0.5.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.287109 simplechain-0.0.5.7/simplechain/
--rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.7/simplechain/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.314861 simplechain-0.0.5.7/simplechain/pipeline/
--rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.7/simplechain/pipeline/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.319866 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/__init__.py
--rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.7/simplechain/pipeline/data_loaders/user_input.py
--rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.7/simplechain/pipeline/module.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.337883 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/__init__.py
--rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/base_template.py
--rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/conversation_prompts.py
--rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/database_prompts.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.349893 simplechain-0.0.5.7/simplechain/pipeline/providers/
--rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/__init__.py
--rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/database.py
--rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/pipeline/providers/search.py
--rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.7/simplechain/pipeline/standard_modules.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.359902 simplechain-0.0.5.7/simplechain/stack/
--rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.7/simplechain/stack/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.375917 simplechain-0.0.5.7/simplechain/stack/databases/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.7/simplechain/stack/databases/__init__.py
--rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.7/simplechain/stack/databases/base.py
--rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.7/simplechain/stack/databases/sql.py
--rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.7/simplechain/stack/factory.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.377919 simplechain-0.0.5.7/simplechain/stack/image_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.7/simplechain/stack/image_generators/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.388929 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/
--rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/__init__.py
--rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.7/simplechain/stack/pdf_loaders/base.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.404944 simplechain-0.0.5.7/simplechain/stack/search_engines/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/__init__.py
--rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/base.py
--rw-rw-rw-   0        0        0     2887 2023-03-05 21:26:57.000000 simplechain-0.0.5.7/simplechain/stack/search_engines/google_serper.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.425963 simplechain-0.0.5.7/simplechain/stack/text_embedders/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/__init__.py
--rw-rw-rw-   0        0        0     2146 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/ai21.py
--rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/base.py
--rw-rw-rw-   0        0        0     1103 2023-04-28 01:52:29.000000 simplechain-0.0.5.7/simplechain/stack/text_embedders/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.432969 simplechain-0.0.5.7/simplechain/stack/text_generators/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/__init__.py
--rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/base.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.456990 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/
--rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/__init__.py
--rw-rw-rw-   0        0        0     2196 2023-04-28 01:54:45.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/ai21.py
--rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/llm.py
--rw-rw-rw-   0        0        0     1165 2023-04-28 01:54:17.000000 simplechain-0.0.5.7/simplechain/stack/text_generators/llms/openai.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.467000 simplechain-0.0.5.7/simplechain/stack/vector_databases/
--rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/__init__.py
--rw-rw-rw-   0        0        0     3929 2023-05-16 02:02:59.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/annoy_vd.py
--rw-rw-rw-   0        0        0     1531 2023-05-08 23:43:20.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/base.py
--rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.7/simplechain/stack/vector_databases/faiss.py
--rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.7/simplechain/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.298846 simplechain-0.0.5.7/simplechain.egg-info/
--rw-rw-rw-   0        0        0      602 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1846 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-16 02:03:38.000000 simplechain-0.0.5.7/simplechain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-16 02:03:38.472005 simplechain-0.0.5.7/tests/
--rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.7/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.451621 simplechain-0.0.5.8/
+-rw-rw-rw-   0        0        0     1091 2023-03-02 13:34:38.000000 simplechain-0.0.5.8/LICENSE
+-rw-rw-rw-   0        0        0      602 2023-07-17 00:58:39.451621 simplechain-0.0.5.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2902 2023-04-11 15:12:28.000000 simplechain-0.0.5.8/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-17 00:58:39.451621 simplechain-0.0.5.8/setup.cfg
+-rw-rw-rw-   0        0        0     1105 2023-07-17 00:57:42.000000 simplechain-0.0.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.338519 simplechain-0.0.5.8/simplechain/
+-rw-rw-rw-   0        0        0        0 2023-03-05 22:14:57.000000 simplechain-0.0.5.8/simplechain/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.366545 simplechain-0.0.5.8/simplechain/decorators/
+-rw-rw-rw-   0        0        0       91 2023-07-15 16:20:26.000000 simplechain-0.0.5.8/simplechain/decorators/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:17:25.000000 simplechain-0.0.5.8/simplechain/decorators/modules.py
+-rw-rw-rw-   0        0        0      508 2023-07-15 16:16:48.000000 simplechain-0.0.5.8/simplechain/decorators/prompts.py
+-rw-rw-rw-   0        0        0        0 2023-07-15 16:17:39.000000 simplechain-0.0.5.8/simplechain/decorators/stack.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.384560 simplechain-0.0.5.8/simplechain/pipeline/
+-rw-rw-rw-   0        0        0      419 2023-03-07 20:36:53.000000 simplechain-0.0.5.8/simplechain/pipeline/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.390566 simplechain-0.0.5.8/simplechain/pipeline/data_loaders/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:04:39.000000 simplechain-0.0.5.8/simplechain/pipeline/data_loaders/__init__.py
+-rw-rw-rw-   0        0        0      138 2023-03-05 22:18:13.000000 simplechain-0.0.5.8/simplechain/pipeline/data_loaders/user_input.py
+-rw-rw-rw-   0        0        0     1222 2023-03-08 22:10:48.000000 simplechain-0.0.5.8/simplechain/pipeline/module.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.404579 simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:41:29.000000 simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/__init__.py
+-rw-rw-rw-   0        0        0      223 2023-03-05 22:32:39.000000 simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/base_template.py
+-rw-rw-rw-   0        0        0     4162 2023-03-07 18:33:03.000000 simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/conversation_prompts.py
+-rw-rw-rw-   0        0        0     1867 2023-03-05 22:32:39.000000 simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/database_prompts.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.407581 simplechain-0.0.5.8/simplechain/pipeline/providers/
+-rw-rw-rw-   0        0        0        0 2023-03-05 21:07:33.000000 simplechain-0.0.5.8/simplechain/pipeline/providers/__init__.py
+-rw-rw-rw-   0        0        0      534 2023-03-07 04:38:40.000000 simplechain-0.0.5.8/simplechain/pipeline/providers/database.py
+-rw-rw-rw-   0        0        0      373 2023-03-05 21:26:57.000000 simplechain-0.0.5.8/simplechain/pipeline/providers/search.py
+-rw-rw-rw-   0        0        0      869 2023-03-08 23:29:30.000000 simplechain-0.0.5.8/simplechain/pipeline/standard_modules.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.417590 simplechain-0.0.5.8/simplechain/stack/
+-rw-rw-rw-   0        0        0      188 2023-04-28 01:33:47.000000 simplechain-0.0.5.8/simplechain/stack/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.427600 simplechain-0.0.5.8/simplechain/stack/databases/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:08:11.000000 simplechain-0.0.5.8/simplechain/stack/databases/__init__.py
+-rw-rw-rw-   0        0        0      519 2023-03-09 17:10:16.000000 simplechain-0.0.5.8/simplechain/stack/databases/base.py
+-rw-rw-rw-   0        0        0     8271 2023-03-10 19:12:08.000000 simplechain-0.0.5.8/simplechain/stack/databases/sql.py
+-rw-rw-rw-   0        0        0     1759 2023-04-28 02:00:57.000000 simplechain-0.0.5.8/simplechain/stack/factory.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.428600 simplechain-0.0.5.8/simplechain/stack/image_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:34.000000 simplechain-0.0.5.8/simplechain/stack/image_generators/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.430602 simplechain-0.0.5.8/simplechain/stack/pdf_loaders/
+-rw-rw-rw-   0        0        0        0 2023-04-10 15:02:16.000000 simplechain-0.0.5.8/simplechain/stack/pdf_loaders/__init__.py
+-rw-rw-rw-   0        0        0       92 2023-04-28 01:23:48.000000 simplechain-0.0.5.8/simplechain/stack/pdf_loaders/base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.432604 simplechain-0.0.5.8/simplechain/stack/search_engines/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:42:47.000000 simplechain-0.0.5.8/simplechain/stack/search_engines/__init__.py
+-rw-rw-rw-   0        0        0      214 2023-03-05 21:26:57.000000 simplechain-0.0.5.8/simplechain/stack/search_engines/base.py
+-rw-rw-rw-   0        0        0     2887 2023-07-17 00:56:04.000000 simplechain-0.0.5.8/simplechain/stack/search_engines/google_serper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.435608 simplechain-0.0.5.8/simplechain/stack/text_embedders/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:13.000000 simplechain-0.0.5.8/simplechain/stack/text_embedders/__init__.py
+-rw-rw-rw-   0        0        0     2146 2023-07-17 00:55:08.000000 simplechain-0.0.5.8/simplechain/stack/text_embedders/ai21.py
+-rw-rw-rw-   0        0        0      329 2023-04-28 01:54:45.000000 simplechain-0.0.5.8/simplechain/stack/text_embedders/base.py
+-rw-rw-rw-   0        0        0     1103 2023-07-17 00:54:56.000000 simplechain-0.0.5.8/simplechain/stack/text_embedders/openai.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.437609 simplechain-0.0.5.8/simplechain/stack/text_generators/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:47:34.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/__init__.py
+-rw-rw-rw-   0        0        0      184 2023-03-08 18:14:03.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/base.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.440612 simplechain-0.0.5.8/simplechain/stack/text_generators/llms/
+-rw-rw-rw-   0        0        0        0 2023-03-05 00:03:03.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/llms/__init__.py
+-rw-rw-rw-   0        0        0     2196 2023-07-17 00:55:34.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/llms/ai21.py
+-rw-rw-rw-   0        0        0      784 2023-03-08 18:14:03.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/llms/llm.py
+-rw-rw-rw-   0        0        0     1165 2023-07-17 00:55:38.000000 simplechain-0.0.5.8/simplechain/stack/text_generators/llms/openai.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.449619 simplechain-0.0.5.8/simplechain/stack/vector_databases/
+-rw-rw-rw-   0        0        0        0 2023-03-04 23:53:21.000000 simplechain-0.0.5.8/simplechain/stack/vector_databases/__init__.py
+-rw-rw-rw-   0        0        0     3959 2023-07-17 00:56:19.000000 simplechain-0.0.5.8/simplechain/stack/vector_databases/annoy_vd.py
+-rw-rw-rw-   0        0        0     1561 2023-05-16 03:29:33.000000 simplechain-0.0.5.8/simplechain/stack/vector_databases/base.py
+-rw-rw-rw-   0        0        0     2451 2023-04-10 19:19:49.000000 simplechain-0.0.5.8/simplechain/stack/vector_databases/faiss.py
+-rw-rw-rw-   0        0        0      708 2023-03-05 00:01:34.000000 simplechain-0.0.5.8/simplechain/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.354533 simplechain-0.0.5.8/simplechain.egg-info/
+-rw-rw-rw-   0        0        0      602 2023-07-17 00:58:39.000000 simplechain-0.0.5.8/simplechain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1981 2023-07-17 00:58:39.000000 simplechain-0.0.5.8/simplechain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 00:58:39.000000 simplechain-0.0.5.8/simplechain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-07-17 00:58:39.000000 simplechain-0.0.5.8/simplechain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 00:58:39.450621 simplechain-0.0.5.8/tests/
+-rw-rw-rw-   0        0        0       33 2023-03-01 21:32:35.000000 simplechain-0.0.5.8/tests/__init__.py
```

### Comparing `simplechain-0.0.5.7/LICENSE` & `simplechain-0.0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/PKG-INFO` & `simplechain-0.0.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.7
+Version: 0.0.5.8
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.7/README.rst` & `simplechain-0.0.5.8/README.rst`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/setup.py` & `simplechain-0.0.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5.7'
+VERSION = '0.0.5.8'
 DESCRIPTION = 'A package of AI services in modular form'
 LONG_DESCRIPTION = 'A package of AI services in modular form easily configurable and deployable'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="simplechain",
```

### Comparing `simplechain-0.0.5.7/simplechain/pipeline/module.py` & `simplechain-0.0.5.8/simplechain/pipeline/module.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/conversation_prompts.py` & `simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/conversation_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/pipeline/prompt_templates/database_prompts.py` & `simplechain-0.0.5.8/simplechain/pipeline/prompt_templates/database_prompts.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/pipeline/providers/database.py` & `simplechain-0.0.5.8/simplechain/pipeline/providers/database.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/pipeline/standard_modules.py` & `simplechain-0.0.5.8/simplechain/pipeline/standard_modules.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/databases/base.py` & `simplechain-0.0.5.8/simplechain/stack/databases/base.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/databases/sql.py` & `simplechain-0.0.5.8/simplechain/stack/databases/sql.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/factory.py` & `simplechain-0.0.5.8/simplechain/stack/factory.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/search_engines/google_serper.py` & `simplechain-0.0.5.8/simplechain/stack/search_engines/google_serper.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/text_embedders/ai21.py` & `simplechain-0.0.5.8/simplechain/stack/text_embedders/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/text_embedders/openai.py` & `simplechain-0.0.5.8/simplechain/stack/text_embedders/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/ai21.py` & `simplechain-0.0.5.8/simplechain/stack/text_generators/llms/ai21.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/llm.py` & `simplechain-0.0.5.8/simplechain/stack/text_generators/llms/llm.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/text_generators/llms/openai.py` & `simplechain-0.0.5.8/simplechain/stack/text_generators/llms/openai.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/stack/vector_databases/annoy_vd.py` & `simplechain-0.0.5.8/simplechain/stack/vector_databases/annoy_vd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import os
-from typing import Tuple, List, Any, Literal, Dict
+from typing import List, Any, Literal, Dict
 
-import numpy as np
 from annoy import AnnoyIndex
 
 from simplechain.stack.vector_databases.base import VectorDatabase
 
 
 def get_index(path_to_file: str, embed_size: int,
               metric: Literal["angular", "euclidean", "manhattan", "hamming", "dot"]) -> AnnoyIndex:
@@ -19,22 +18,23 @@
 
 def get_metadata(path_to_metadata_file: str) -> List[Any]:
     # Create metadata file if it doesn't exist
     if not os.path.isfile(path_to_metadata_file):
         # write an empty list to the file
         with open(path_to_metadata_file, "a") as f:
             json.dump([], f)
-            f.close()
         return []
 
     # Load json from file
-    metadata = json.loads(open(path_to_metadata_file, 'r').read())
+    with open(path_to_metadata_file, "r") as f:
+        metadata = json.load(f)
     return metadata
 
 
+
 class Annoy(VectorDatabase):
     def __init__(self, embed_size: int, path_to_index_file: str, path_to_metadata_file: str,
                  metric: Literal["angular", "euclidean", "manhattan", "hamming", "dot"] = "angular", n_trees: int = 10):
         """
         Annoy vector database
         :param metric: Distance metric to use
         :param n_trees: Number of trees to use
@@ -85,27 +85,28 @@
         """
         Given a query embed, get the k nearest neighbors with their distances
         :param include_distances:
         :param query_embed:
         :param k:
         :return: k nearest neighbors with their distances
         """
-
         results = {}
         nearest_neighbors = self.index.get_nns_by_vector(query_embed, k, search_k=-1, include_distances=include_distances)
         results["ids"] = nearest_neighbors[0]
         if include_distances:
             results["distances"] = nearest_neighbors[1]
         results["metadata"] = [self.metadata[i] for i in results["ids"]]  # Get metadata for each id
 
         return results
 
     def get_item_given_index(self, index: int, include_embeds: bool = True, include_metadata: bool = True) -> Dict:
         """
         Given an index, get the name and embed of the item
+        :param include_metadata:
+        :param include_embeds:
         :param index:
         :return:
         """
         results = {}
         if include_embeds:
             results["embed"] = self.index.get_item_vector(index)
         if include_metadata:
```

### Comparing `simplechain-0.0.5.7/simplechain/stack/vector_databases/base.py` & `simplechain-0.0.5.8/simplechain/stack/vector_databases/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from typing import Tuple, List, Any, Dict
+from typing import Tuple, List, Any, Dict, Literal
 
 import numpy as np
 
 
 class VectorDatabase(ABC):
     @abstractmethod
     def add(self, embed: List[float], metadata: Any):
@@ -30,27 +30,27 @@
         """
         Build the database
         :return:
         """
         pass
 
     @abstractmethod
-    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: bool = False) -> Dict:
+    def get_nearest_neighbors(self, query_embed: List[float], k: int = 1, include_distances: Literal[True, False] = False) -> Dict:
         """
         Given a query embed, get the k nearest neighbors with their distances
+        :param include_distances:
         :param query_embed:
         :param k:
         :return: a list of k nearest neighbours with their payloads and distances
         """
         pass
 
     @abstractmethod
     def get_item_given_index(self, index: int, include_embeds: bool = True, include_metadata: bool = True) -> Dict:
         """
         Given an index, get the name and embed of the item
         :param include_metadata:
         :param include_embeds:
-        :param return_embed:
         :param index:
         :return:
         """
         pass
```

### Comparing `simplechain-0.0.5.7/simplechain/stack/vector_databases/faiss.py` & `simplechain-0.0.5.8/simplechain/stack/vector_databases/faiss.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain/utils.py` & `simplechain-0.0.5.8/simplechain/utils.py`

 * *Files identical despite different names*

### Comparing `simplechain-0.0.5.7/simplechain.egg-info/PKG-INFO` & `simplechain-0.0.5.8/simplechain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplechain
-Version: 0.0.5.7
+Version: 0.0.5.8
 Summary: A package of AI services in modular form
 Author: Rahel Gunaratne
 Author-email: rahel.gunaratne@gmail.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `simplechain-0.0.5.7/simplechain.egg-info/SOURCES.txt` & `simplechain-0.0.5.8/simplechain.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 setup.py
 simplechain/__init__.py
 simplechain/utils.py
 simplechain.egg-info/PKG-INFO
 simplechain.egg-info/SOURCES.txt
 simplechain.egg-info/dependency_links.txt
 simplechain.egg-info/top_level.txt
+simplechain/decorators/__init__.py
+simplechain/decorators/modules.py
+simplechain/decorators/prompts.py
+simplechain/decorators/stack.py
 simplechain/pipeline/__init__.py
 simplechain/pipeline/module.py
 simplechain/pipeline/standard_modules.py
 simplechain/pipeline/data_loaders/__init__.py
 simplechain/pipeline/data_loaders/user_input.py
 simplechain/pipeline/prompt_templates/__init__.py
 simplechain/pipeline/prompt_templates/base_template.py
```

