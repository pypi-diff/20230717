# Comparing `tmp/claude_ai-0.0.1.tar.gz` & `tmp/claude_ai-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "claude_ai-0.0.1.tar", last modified: Mon Jul 17 07:51:29 2023, max compression
+gzip compressed data, was "claude_ai-0.0.2.tar", last modified: Mon Jul 17 08:01:56 2023, max compression
```

## Comparing `claude_ai-0.0.1.tar` & `claude_ai-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 07:51:29.955113 claude_ai-0.0.1/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      108 2023-07-17 07:51:29.954865 claude_ai-0.0.1/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3215 2023-07-17 07:04:23.000000 claude_ai-0.0.1/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 07:51:29.954454 claude_ai-0.0.1/claude_ai.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      108 2023-07-17 07:51:29.000000 claude_ai-0.0.1/claude_ai.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)      182 2023-07-17 07:51:29.000000 claude_ai-0.0.1/claude_ai.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-17 07:51:29.000000 claude_ai-0.0.1/claude_ai.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        9 2023-07-17 07:51:29.000000 claude_ai-0.0.1/claude_ai.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       10 2023-07-17 07:51:29.000000 claude_ai-0.0.1/claude_ai.egg-info/top_level.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-17 07:51:29.955214 claude_ai-0.0.1/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      236 2023-07-17 07:41:55.000000 claude_ai-0.0.1/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:01:56.242886 claude_ai-0.0.2/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      108 2023-07-17 08:01:56.242635 claude_ai-0.0.2/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3215 2023-07-17 07:55:04.000000 claude_ai-0.0.2/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-07-17 08:01:56.242245 claude_ai-0.0.2/claude_ai.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      108 2023-07-17 08:01:56.000000 claude_ai-0.0.2/claude_ai.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      182 2023-07-17 08:01:56.000000 claude_ai-0.0.2/claude_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-07-17 08:01:56.000000 claude_ai-0.0.2/claude_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        9 2023-07-17 08:01:56.000000 claude_ai-0.0.2/claude_ai.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       10 2023-07-17 08:01:56.000000 claude_ai-0.0.2/claude_ai.egg-info/top_level.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-07-17 08:01:56.242974 claude_ai-0.0.2/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      236 2023-07-17 08:01:54.000000 claude_ai-0.0.2/setup.py
```

### Comparing `claude_ai-0.0.1/README.md` & `claude_ai-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This library provides a simple way to interact with the Claude AI API. You can use it to get organizations, get conversations, send messages, and upload files.
 
 ## Installation
 
 First, you need to install this library. You can do this via pip:
 
 ```bash
-pip install claude_ai
+pip install claude-ai
 ```
 
 ## Usage
 
 First, you need to import the `ClaudeAPIWrapper` class from `claude_ai.claude`. Then, you can create a `ClaudeAPIWrapper` object using your session key.
 
 ```python
```

