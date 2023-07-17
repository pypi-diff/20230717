# Comparing `tmp/alphawave-0.3.9.tar.gz` & `tmp/alphawave-0.3.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alphawave-0.3.9.tar", last modified: Fri Jul 14 18:04:03 2023, max compression
+gzip compressed data, was "alphawave-0.3.91.tar", last modified: Mon Jul 17 20:18:02 2023, max compression
```

## Comparing `alphawave-0.3.9.tar` & `alphawave-0.3.91.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.9/LICENSE
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-14 18:04:03.562178 alphawave-0.3.9/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.9/README.md
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1021 2023-07-14 18:03:56.000000 alphawave-0.3.9/pyproject.toml
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-14 18:04:03.562178 alphawave-0.3.9/setup.cfg
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/alphawave/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9961 2023-07-14 00:35:05.000000 alphawave-0.3.9/src/alphawave/AlphaWave.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.9/src/alphawave/Colorize.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.9/src/alphawave/DefaultResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.9/src/alphawave/JSONResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.9/src/alphawave/MemoryFork.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.9/src/alphawave/OSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.9/src/alphawave/OpenAIClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-14 17:58:30.000000 alphawave-0.3.9/src/alphawave/PythonResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.9/src/alphawave/RepairTestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.9/src/alphawave/Response.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6594 2023-07-09 00:19:51.000000 alphawave-0.3.9/src/alphawave/TOMLResponseValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.9/src/alphawave/TestClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.9/src/alphawave/TestClientTest.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.9/src/alphawave/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.9/src/alphawave/alphawaveTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.9/src/alphawave/internalTypes.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.9/src/alphawave/jsonParser.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/alphawave.egg-info/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     9438 2023-07-14 18:04:03.000000 alphawave-0.3.9/src/alphawave.egg-info/PKG-INFO
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-14 18:04:03.000000 alphawave-0.3.9/src/alphawave.egg-info/SOURCES.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-14 18:04:03.000000 alphawave-0.3.9/src/alphawave.egg-info/dependency_links.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-14 18:04:03.000000 alphawave-0.3.9/src/alphawave.egg-info/requires.txt
--rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-14 18:04:03.000000 alphawave-0.3.9/src/alphawave.egg-info/top_level.txt
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/alphawave_agents/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    17679 2023-07-12 20:04:10.000000 alphawave-0.3.9/src/alphawave_agents/Agent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.9/src/alphawave_agents/AgentCommandSection.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7008 2023-07-12 19:17:12.000000 alphawave-0.3.9/src/alphawave_agents/AgentCommandValidator.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-07-12 19:12:18.000000 alphawave-0.3.9/src/alphawave_agents/AskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.9/src/alphawave_agents/CompleteTaskCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.9/src/alphawave_agents/ConfirmAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1423 2023-07-12 19:12:30.000000 alphawave-0.3.9/src/alphawave_agents/FinalAnswerCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1518 2023-07-12 19:12:07.000000 alphawave-0.3.9/src/alphawave_agents/MathCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.9/src/alphawave_agents/PromptCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     7938 2023-07-12 19:12:49.000000 alphawave-0.3.9/src/alphawave_agents/SchemaBasedCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.9/src/alphawave_agents/SentimentAnalysis.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.9/src/alphawave_agents/SetPropertyCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.9/src/alphawave_agents/__init__.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.9/src/alphawave_agents/agentTypes.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/alphawave_pyexts/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.9/src/alphawave_pyexts/FsInference.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.9/src/alphawave_pyexts/LLMClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2858 2023-07-12 19:14:52.000000 alphawave-0.3.9/src/alphawave_pyexts/SearchCommand.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.9/src/alphawave_pyexts/chat.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.9/src/alphawave_pyexts/configuration_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.9/src/alphawave_pyexts/conversation.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.9/src/alphawave_pyexts/handler.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/src/alphawave_pyexts/llmsearch/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.9/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-12 19:15:47.000000 alphawave-0.3.9/src/alphawave_pyexts/llmsearch/search_service.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.9/src/alphawave_pyexts/modelling_RW.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.9/src/alphawave_pyexts/serverUtils.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)     6919 2023-07-11 19:49:15.000000 alphawave-0.3.9/src/alphawave_pyexts/utilityV2.py
-drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-14 18:04:03.562178 alphawave-0.3.9/tests/
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.9/tests/testOSClient.py
--rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.9/tests/testOpenAiClient.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.360847 alphawave-0.3.91/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1070 2023-06-05 21:12:30.000000 alphawave-0.3.91/LICENSE
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-17 20:18:02.360847 alphawave-0.3.91/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8859 2023-06-18 19:15:49.000000 alphawave-0.3.91/README.md
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1022 2023-07-17 20:17:53.000000 alphawave-0.3.91/pyproject.toml
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       38 2023-07-17 20:18:02.360847 alphawave-0.3.91/setup.cfg
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.352847 alphawave-0.3.91/src/
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.356847 alphawave-0.3.91/src/alphawave/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9961 2023-07-14 00:35:05.000000 alphawave-0.3.91/src/alphawave/AlphaWave.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1370 2023-06-10 00:08:35.000000 alphawave-0.3.91/src/alphawave/Colorize.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      740 2023-06-18 18:50:38.000000 alphawave-0.3.91/src/alphawave/DefaultResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     8173 2023-07-09 19:31:41.000000 alphawave-0.3.91/src/alphawave/JSONResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1173 2023-06-19 22:47:36.000000 alphawave-0.3.91/src/alphawave/MemoryFork.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7164 2023-07-11 18:23:11.000000 alphawave-0.3.91/src/alphawave/OSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     5926 2023-07-11 18:29:03.000000 alphawave-0.3.91/src/alphawave/OpenAIClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4120 2023-07-16 20:12:02.000000 alphawave-0.3.91/src/alphawave/PythonResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1365 2023-07-10 16:02:12.000000 alphawave-0.3.91/src/alphawave/RepairTestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3008 2023-06-15 23:14:04.000000 alphawave-0.3.91/src/alphawave/Response.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6594 2023-07-09 00:19:51.000000 alphawave-0.3.91/src/alphawave/TOMLResponseValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      800 2023-06-15 04:12:01.000000 alphawave-0.3.91/src/alphawave/TestClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1515 2023-06-15 04:12:10.000000 alphawave-0.3.91/src/alphawave/TestClientTest.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:12.000000 alphawave-0.3.91/src/alphawave/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1377 2023-07-11 21:25:58.000000 alphawave-0.3.91/src/alphawave/alphawaveTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     4163 2023-06-04 18:16:08.000000 alphawave-0.3.91/src/alphawave/internalTypes.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      782 2023-06-07 21:02:29.000000 alphawave-0.3.91/src/alphawave/jsonParser.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.356847 alphawave-0.3.91/src/alphawave.egg-info/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     9439 2023-07-17 20:18:02.000000 alphawave-0.3.91/src/alphawave.egg-info/PKG-INFO
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1818 2023-07-17 20:18:02.000000 alphawave-0.3.91/src/alphawave.egg-info/SOURCES.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        1 2023-07-17 20:18:02.000000 alphawave-0.3.91/src/alphawave.egg-info/dependency_links.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      199 2023-07-17 20:18:02.000000 alphawave-0.3.91/src/alphawave.egg-info/requires.txt
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)       44 2023-07-17 20:18:02.000000 alphawave-0.3.91/src/alphawave.egg-info/top_level.txt
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.360847 alphawave-0.3.91/src/alphawave_agents/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    17679 2023-07-12 20:04:10.000000 alphawave-0.3.91/src/alphawave_agents/Agent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1715 2023-07-11 02:39:22.000000 alphawave-0.3.91/src/alphawave_agents/AgentCommandSection.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7018 2023-07-16 16:56:57.000000 alphawave-0.3.91/src/alphawave_agents/AgentCommandValidator.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1428 2023-07-12 19:12:18.000000 alphawave-0.3.91/src/alphawave_agents/AskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1871 2023-06-07 03:14:30.000000 alphawave-0.3.91/src/alphawave_agents/CompleteTaskCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1336 2023-06-06 16:52:41.000000 alphawave-0.3.91/src/alphawave_agents/ConfirmAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1423 2023-07-12 19:12:30.000000 alphawave-0.3.91/src/alphawave_agents/FinalAnswerCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1518 2023-07-12 19:12:07.000000 alphawave-0.3.91/src/alphawave_agents/MathCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     3249 2023-07-12 00:55:02.000000 alphawave-0.3.91/src/alphawave_agents/PromptCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     7938 2023-07-12 19:12:49.000000 alphawave-0.3.91/src/alphawave_agents/SchemaBasedCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2452 2023-06-09 18:41:37.000000 alphawave-0.3.91/src/alphawave_agents/SentimentAnalysis.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2149 2023-06-06 16:59:49.000000 alphawave-0.3.91/src/alphawave_agents/SetPropertyCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)        0 2023-06-06 23:52:38.000000 alphawave-0.3.91/src/alphawave_agents/__init__.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1859 2023-07-06 03:51:05.000000 alphawave-0.3.91/src/alphawave_agents/agentTypes.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.360847 alphawave-0.3.91/src/alphawave_pyexts/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11096 2023-06-24 23:27:36.000000 alphawave-0.3.91/src/alphawave_pyexts/FsInference.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6397 2023-07-11 18:37:11.000000 alphawave-0.3.91/src/alphawave_pyexts/LLMClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2858 2023-07-12 19:14:52.000000 alphawave-0.3.91/src/alphawave_pyexts/SearchCommand.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    11610 2023-06-22 19:47:31.000000 alphawave-0.3.91/src/alphawave_pyexts/chat.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     2607 2023-06-24 00:18:59.000000 alphawave-0.3.91/src/alphawave_pyexts/configuration_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    23275 2023-07-08 16:36:14.000000 alphawave-0.3.91/src/alphawave_pyexts/conversation.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     1154 2023-06-24 03:11:55.000000 alphawave-0.3.91/src/alphawave_pyexts/handler.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.360847 alphawave-0.3.91/src/alphawave_pyexts/llmsearch/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    13645 2023-07-11 19:55:51.000000 alphawave-0.3.91/src/alphawave_pyexts/llmsearch/google_search_concurrent.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)      972 2023-07-12 19:15:47.000000 alphawave-0.3.91/src/alphawave_pyexts/llmsearch/search_service.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    47520 2023-06-24 00:15:02.000000 alphawave-0.3.91/src/alphawave_pyexts/modelling_RW.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    12724 2023-07-02 15:55:18.000000 alphawave-0.3.91/src/alphawave_pyexts/serverUtils.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)     6919 2023-07-11 19:49:15.000000 alphawave-0.3.91/src/alphawave_pyexts/utilityV2.py
+drwxrwxr-x   0 bruce     (1000) bruce     (1000)        0 2023-07-17 20:18:02.360847 alphawave-0.3.91/tests/
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14779 2023-06-07 17:09:31.000000 alphawave-0.3.91/tests/testOSClient.py
+-rw-rw-r--   0 bruce     (1000) bruce     (1000)    14639 2023-06-18 18:49:14.000000 alphawave-0.3.91/tests/testOpenAiClient.py
```

### Comparing `alphawave-0.3.9/LICENSE` & `alphawave-0.3.91/LICENSE`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/PKG-INFO` & `alphawave-0.3.91/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.9
+Version: 0.3.91
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.9/README.md` & `alphawave-0.3.91/README.md`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/pyproject.toml` & `alphawave-0.3.91/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "alphawave"
-version = "0.3.9"
+version = "0.3.91"
 authors = [
   { name="Steven Ickman", email="author@example.com" },
   { name="Bruce DAmbrosio", email="bruce.dambrosio@gmail.com" },
 ]
 
 description = "AlphaWave-py - Functions for smaller Large Language Models (sLLMs)"
```

### Comparing `alphawave-0.3.9/src/alphawave/AlphaWave.py` & `alphawave-0.3.91/src/alphawave/AlphaWave.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/Colorize.py` & `alphawave-0.3.91/src/alphawave/Colorize.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/DefaultResponseValidator.py` & `alphawave-0.3.91/src/alphawave/DefaultResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/JSONResponseValidator.py` & `alphawave-0.3.91/src/alphawave/JSONResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/MemoryFork.py` & `alphawave-0.3.91/src/alphawave/MemoryFork.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/OSClient.py` & `alphawave-0.3.91/src/alphawave/OSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/OpenAIClient.py` & `alphawave-0.3.91/src/alphawave/OpenAIClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/PythonResponseValidator.py` & `alphawave-0.3.91/src/alphawave/PythonResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/RepairTestClient.py` & `alphawave-0.3.91/src/alphawave/RepairTestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/Response.py` & `alphawave-0.3.91/src/alphawave/Response.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/TOMLResponseValidator.py` & `alphawave-0.3.91/src/alphawave/TOMLResponseValidator.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/TestClient.py` & `alphawave-0.3.91/src/alphawave/TestClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/TestClientTest.py` & `alphawave-0.3.91/src/alphawave/TestClientTest.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/alphawaveTypes.py` & `alphawave-0.3.91/src/alphawave/alphawaveTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/internalTypes.py` & `alphawave-0.3.91/src/alphawave/internalTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave/jsonParser.py` & `alphawave-0.3.91/src/alphawave/jsonParser.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave.egg-info/PKG-INFO` & `alphawave-0.3.91/src/alphawave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alphawave
-Version: 0.3.9
+Version: 0.3.91
 Summary: AlphaWave-py - Functions for smaller Large Language Models (sLLMs)
 Author-email: Steven Ickman <author@example.com>, Bruce DAmbrosio <bruce.dambrosio@gmail.com>
 Project-URL: Homepage, https://tuuyi.io/alphawave
 Project-URL: Bug Tracker, https://github.com/Stevenic/alphawave-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `alphawave-0.3.9/src/alphawave.egg-info/SOURCES.txt` & `alphawave-0.3.91/src/alphawave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/Agent.py` & `alphawave-0.3.91/src/alphawave_agents/Agent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/AgentCommandSection.py` & `alphawave-0.3.91/src/alphawave_agents/AgentCommandSection.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/AgentCommandValidator.py` & `alphawave-0.3.91/src/alphawave_agents/AgentCommandValidator.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self._commands = commands
 
     def validate_response(self, memory, functions, tokenizer, response, remaining_attempts) -> Union[AgentThought, None]:
         try:
           #print(f"***** AgentCommandValidator validate syntax: \n{self._syntax}\nresponse\n{response}")
           message = response['message']
           raw_text = message if isinstance(message, str) else message.get('content', '')
-          if (self._syntax == 'JSON' and '{' not in raw_text) or (self._syntax == 'TOML' and 'response' not in raw_text.lower()):
+          if (self._syntax == 'JSON' and '{"command":' not in raw_text) or (self._syntax == 'TOML' and 'response' not in raw_text.lower()):
               # means no form found, assume llm doesn't need to use a command
               return {
                   'type': 'Validation',
                   'valid': True,
                   'value': raw_text,
                   'feedback': 'no command'
               }
```

### Comparing `alphawave-0.3.9/src/alphawave_agents/AskCommand.py` & `alphawave-0.3.91/src/alphawave_agents/AskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/CompleteTaskCommand.py` & `alphawave-0.3.91/src/alphawave_agents/CompleteTaskCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/ConfirmAnswerCommand.py` & `alphawave-0.3.91/src/alphawave_agents/ConfirmAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/FinalAnswerCommand.py` & `alphawave-0.3.91/src/alphawave_agents/FinalAnswerCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/MathCommand.py` & `alphawave-0.3.91/src/alphawave_agents/MathCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/PromptCommand.py` & `alphawave-0.3.91/src/alphawave_agents/PromptCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/SchemaBasedCommand.py` & `alphawave-0.3.91/src/alphawave_agents/SchemaBasedCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/SentimentAnalysis.py` & `alphawave-0.3.91/src/alphawave_agents/SentimentAnalysis.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/SetPropertyCommand.py` & `alphawave-0.3.91/src/alphawave_agents/SetPropertyCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_agents/agentTypes.py` & `alphawave-0.3.91/src/alphawave_agents/agentTypes.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/FsInference.py` & `alphawave-0.3.91/src/alphawave_pyexts/FsInference.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/LLMClient.py` & `alphawave-0.3.91/src/alphawave_pyexts/LLMClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/SearchCommand.py` & `alphawave-0.3.91/src/alphawave_pyexts/SearchCommand.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/chat.py` & `alphawave-0.3.91/src/alphawave_pyexts/chat.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/configuration_RW.py` & `alphawave-0.3.91/src/alphawave_pyexts/configuration_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/conversation.py` & `alphawave-0.3.91/src/alphawave_pyexts/conversation.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/handler.py` & `alphawave-0.3.91/src/alphawave_pyexts/handler.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/llmsearch/google_search_concurrent.py` & `alphawave-0.3.91/src/alphawave_pyexts/llmsearch/google_search_concurrent.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/llmsearch/search_service.py` & `alphawave-0.3.91/src/alphawave_pyexts/llmsearch/search_service.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/modelling_RW.py` & `alphawave-0.3.91/src/alphawave_pyexts/modelling_RW.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/serverUtils.py` & `alphawave-0.3.91/src/alphawave_pyexts/serverUtils.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/src/alphawave_pyexts/utilityV2.py` & `alphawave-0.3.91/src/alphawave_pyexts/utilityV2.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/tests/testOSClient.py` & `alphawave-0.3.91/tests/testOSClient.py`

 * *Files identical despite different names*

### Comparing `alphawave-0.3.9/tests/testOpenAiClient.py` & `alphawave-0.3.91/tests/testOpenAiClient.py`

 * *Files identical despite different names*

