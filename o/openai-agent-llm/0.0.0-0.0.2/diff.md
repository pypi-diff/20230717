# Comparing `tmp/openai-agent-llm-0.0.0.tar.gz` & `tmp/openai-agent-llm-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai-agent-llm-0.0.0.tar", last modified: Mon Jul 17 03:10:17 2023, max compression
+gzip compressed data, was "openai-agent-llm-0.0.2.tar", last modified: Mon Jul 17 03:28:07 2023, max compression
```

## Comparing `openai-agent-llm-0.0.0.tar` & `openai-agent-llm-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 03:10:17.606053 openai-agent-llm-0.0.0/
--rw-rw-rw-   0        0        0      315 2023-07-17 03:10:17.604052 openai-agent-llm-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     6323 2023-07-07 03:03:31.000000 openai-agent-llm-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-17 03:10:17.565054 openai-agent-llm-0.0.0/openai_agent_llm/
--rw-rw-rw-   0        0        0    16833 2023-07-17 03:08:48.000000 openai-agent-llm-0.0.0/openai_agent_llm/__init__.py
--rw-rw-rw-   0        0        0      756 2023-07-06 04:59:16.000000 openai-agent-llm-0.0.0/openai_agent_llm/constants.py
--rw-rw-rw-   0        0        0     4661 2023-07-06 08:18:43.000000 openai-agent-llm-0.0.0/openai_agent_llm/protocol.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:10:17.591053 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/
--rw-rw-rw-   0        0        0      315 2023-07-17 03:10:17.000000 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      334 2023-07-17 03:10:17.000000 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 03:10:17.000000 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-07-17 03:10:17.000000 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-07-17 03:10:17.000000 openai-agent-llm-0.0.0/openai_agent_llm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-17 03:10:17.606053 openai-agent-llm-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      976 2023-07-17 03:09:16.000000 openai-agent-llm-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 03:10:17.600052 openai-agent-llm-0.0.0/test/
--rw-rw-rw-   0        0        0        0 2023-07-07 01:25:34.000000 openai-agent-llm-0.0.0/test/__init__.py
--rw-rw-rw-   0        0        0     1198 2023-07-14 10:00:30.000000 openai-agent-llm-0.0.0/test/api.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:28:07.730390 openai-agent-llm-0.0.2/
+-rw-rw-rw-   0        0        0     4250 2023-07-17 03:28:07.730390 openai-agent-llm-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3735 2023-07-17 03:27:21.000000 openai-agent-llm-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 03:28:07.694389 openai-agent-llm-0.0.2/openai_agent_llm/
+-rw-rw-rw-   0        0        0    16833 2023-07-17 03:08:48.000000 openai-agent-llm-0.0.2/openai_agent_llm/__init__.py
+-rw-rw-rw-   0        0        0      756 2023-07-06 04:59:16.000000 openai-agent-llm-0.0.2/openai_agent_llm/constants.py
+-rw-rw-rw-   0        0        0     4661 2023-07-06 08:18:43.000000 openai-agent-llm-0.0.2/openai_agent_llm/protocol.py
+drwxrwxrwx   0        0        0        0 2023-07-17 03:28:07.727403 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/
+-rw-rw-rw-   0        0        0     4250 2023-07-17 03:28:07.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      350 2023-07-17 03:28:07.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 03:28:07.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-07-17 03:28:07.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-17 03:28:07.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 03:22:11.000000 openai-agent-llm-0.0.2/openai_agent_llm.egg-info/zip-safe
+-rw-rw-rw-   0        0        0      800 2023-07-17 03:28:07.733376 openai-agent-llm-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      193 2023-07-17 03:22:01.000000 openai-agent-llm-0.0.2/setup.py
```

### Comparing `openai-agent-llm-0.0.0/openai_agent_llm/__init__.py` & `openai-agent-llm-0.0.2/openai_agent_llm/__init__.py`

 * *Files identical despite different names*

### Comparing `openai-agent-llm-0.0.0/openai_agent_llm/constants.py` & `openai-agent-llm-0.0.2/openai_agent_llm/constants.py`

 * *Files identical despite different names*

### Comparing `openai-agent-llm-0.0.0/openai_agent_llm/protocol.py` & `openai-agent-llm-0.0.2/openai_agent_llm/protocol.py`

 * *Files identical despite different names*

