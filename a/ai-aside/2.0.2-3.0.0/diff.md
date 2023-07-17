# Comparing `tmp/ai-aside-2.0.2.tar.gz` & `tmp/ai-aside-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai-aside-2.0.2.tar", last modified: Wed Jul  5 13:47:52 2023, max compression
+gzip compressed data, was "ai-aside-3.0.0.tar", last modified: Mon Jul 17 15:04:42 2023, max compression
```

## Comparing `ai-aside-2.0.2.tar` & `ai-aside-3.0.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1269 2023-07-05 13:47:44.000000 ai-aside-2.0.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-05 13:47:44.000000 ai-aside-2.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-05 13:47:44.000000 ai-aside-2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-07-05 13:47:52.948860 ai-aside-2.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-07-05 13:47:44.000000 ai-aside-2.0.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside/
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/settings/production.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/ai_aside/summaryhook_aside/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      761 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     7288 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/block.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      484 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/common.py
--rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/devstack.py
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/text_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1836 2023-07-05 13:47:44.000000 ai-aside-2.0.2/ai_aside/summaryhook_aside/waffle.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.944860 ai-aside-2.0.2/ai_aside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     7878 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      906 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      209 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       31 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-05 13:47:52.000000 ai-aside-2.0.2/ai_aside.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      138 2023-07-05 13:47:44.000000 ai-aside-2.0.2/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-05 13:47:44.000000 ai-aside-2.0.2/requirements/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-05 13:47:52.948860 ai-aside-2.0.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5399 2023-07-05 13:47:44.000000 ai-aside-2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-05 13:47:52.948860 ai-aside-2.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      252 2023-07-05 13:47:44.000000 ai-aside-2.0.2/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-07-17 15:04:38.000000 ai-aside-3.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-07-17 15:04:38.000000 ai-aside-3.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      203 2023-07-17 15:04:38.000000 ai-aside-3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     8385 2023-07-17 15:04:42.959770 ai-aside-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6071 2023-07-17 15:04:38.000000 ai-aside-3.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside/
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8487 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/block.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1627 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/platform_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/ai_aside/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      460 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/common.py
+-rw-r--r--   0 runner    (1001) docker     (122)      655 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/devstack.py
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1821 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/text_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      317 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1838 2023-07-17 15:04:38.000000 ai-aside-3.0.0/ai_aside/waffle.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.955770 ai-aside-3.0.0/ai_aside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     8385 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      759 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-07-17 15:04:42.000000 ai-aside-3.0.0/ai_aside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      154 2023-07-17 15:04:38.000000 ai-aside-3.0.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      561 2023-07-17 15:04:38.000000 ai-aside-3.0.0/requirements/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-07-17 15:04:42.959770 ai-aside-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5302 2023-07-17 15:04:38.000000 ai-aside-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-17 15:04:42.959770 ai-aside-3.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     9822 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2296 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2360 2023-07-17 15:04:38.000000 ai-aside-3.0.0/tests/test_text_utils.py
```

### Comparing `ai-aside-2.0.2/CHANGELOG.rst` & `ai-aside-3.0.0/CHANGELOG.rst`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,24 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+3.0.0 – 2023-07-16
+**********************************************
+
+Features
+=========
+* Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
+* Added models to summaryhook_aside (Has migrations)
+* Catch exceptions in a couple of locations so the aside cannot crash content.
+
 2.0.2 – 2023-07-05
 **********************************************
 
 Fix
 =====
 
 * Updated HTML parser to remove tags with their content for specific cases like `<script>` or `<style>`.
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_l_z4pc93_/tmphx_g1o1z_TarContainer/0/1.rst", line 60, column 0: CDATA terminal not found*

 * *File "/tmp/diffoscope_l_z4pc93_/tmphx_g1o1z_TarContainer/0/1.rst", line 60, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,13 @@
 Change Log ########## .. All enhancements and patches to ai_aside will be
 documented in this file. It adheres to the structure of https://
 keepachangelog.com/ , but in reStructuredText instead of Markdown (for ease of
 incorporation into Sphinx documentation and the PyPI description). This project
 adheres to Semantic Versioning (https://semver.org/). .. There should always be
 an "Unreleased" section for changes pending release. Unreleased **********
-2.0.2 â 2023-07-05 ********************************************** Fix ===== *
-Updated HTML parser to remove tags with their content for specific cases like `
+3.0.0 â 2023-07-16 ********************************************** Features
+========= * Summary content handler now requires a staff user identity,
+otherwise returns 403. This is a breaking change. * Added models to
+summaryhook_aside (Has migrations) * Catch exceptions in a couple of locations
+so the aside cannot crash content. 2.0.2 â 2023-07-05
+********************************************** Fix ===== * Updated HTML parser
+to remove tags with their content for specific cases like `
```

### Comparing `ai-aside-2.0.2/LICENSE.txt` & `ai-aside-3.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.2/PKG-INFO` & `ai-aside-3.0.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.2
+Version: 3.0.0
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -44,15 +44,26 @@
   cd ai-aside
 
   # Set up a virtualenv using virtualenvwrapper with the same name as the repo and activate it
   mkvirtualenv -p python3.8 ai-aside
 
 Local testing
 ~~~~~~~~~~~~~
-To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run ``pip install -e /edx/src/ai-aside``.  The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run::
+
+  pip install -e /edx/src/ai-aside
+
+The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+
+Run Migrations
+..............
+You will also need to run migrations for local testing. Using the same lms or cms shell as before, run::
+
+  ./manage.py lms migrate ai_aside
+
 
 Testing in Docker with AI-spot
 ..............................
 
 If you are running both devstack and a local instance of the supporting ai-spot in docker, you need two pieces of special setup to let ai-spot call the aside handler and retrieve content.
 
 The first is to connect ai-spot to the devstack network with a docker command::
@@ -196,14 +207,24 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+3.0.0 – 2023-07-16
+**********************************************
+
+Features
+=========
+* Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
+* Added models to summaryhook_aside (Has migrations)
+* Catch exceptions in a couple of locations so the aside cannot crash content.
+
 2.0.2 – 2023-07-05
 **********************************************
 
 Fix
 =====
 
 * Updated HTML parser to remove tags with their content for specific cases like `<script>` or `<style>`.
```

### Comparing `ai-aside-2.0.2/README.rst` & `ai-aside-3.0.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,26 @@
   cd ai-aside
 
   # Set up a virtualenv using virtualenvwrapper with the same name as the repo and activate it
   mkvirtualenv -p python3.8 ai-aside
 
 Local testing
 ~~~~~~~~~~~~~
-To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run ``pip install -e /edx/src/ai-aside``.  The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run::
+
+  pip install -e /edx/src/ai-aside
+
+The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+
+Run Migrations
+..............
+You will also need to run migrations for local testing. Using the same lms or cms shell as before, run::
+
+  ./manage.py lms migrate ai_aside
+
 
 Testing in Docker with AI-spot
 ..............................
 
 If you are running both devstack and a local instance of the supporting ai-spot in docker, you need two pieces of special setup to let ai-spot call the aside handler and retrieve content.
 
 The first is to connect ai-spot to the devstack network with a docker command::
```

### Comparing `ai-aside-2.0.2/ai_aside/apps.py` & `ai-aside-3.0.0/ai_aside/apps.py`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.2/ai_aside/summaryhook_aside/block.py` & `ai-aside-3.0.0/ai_aside/block.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# pyright: reportMissingImports=false
-
-"""Xblock aside enabling OpenAI driven summaries"""
+"""Xblock aside enabling OpenAI driven summaries."""
 
+import logging
 from datetime import datetime
 
 from django.conf import settings
 from django.template import Context, Template
 from web_fragments.fragment import Fragment
 from webob import Response
 from xblock.core import XBlock, XBlockAside
 
-from ai_aside.summaryhook_aside.text_utils import html_to_text
-from ai_aside.summaryhook_aside.waffle import summary_enabled, summary_staff_only
+from ai_aside.platform_imports import get_block, get_text_transcript
+from ai_aside.text_utils import html_to_text
+from ai_aside.waffle import summary_enabled, summary_staff_only
+
+log = logging.getLogger(__name__)
 
 # map block types to what ai-spot expects for content types
 CATEGORY_TYPE_MAP = {
     "html": "TEXT",
     "video": "VIDEO",
 }
 
@@ -37,55 +39,48 @@
 """
 
 
 def _format_date(date):
     return date.strftime('%Y-%m-%d %H:%M:%S') if isinstance(date, datetime) else None
 
 
+def _staff_user(block):
+    return getattr(block.runtime, 'user_is_staff', False)
+
+
 def _render_summary(context):
     template = Template(summary_fragment)
     return template.render(Context(context))
 
 
 def _extract_child_contents(child, category):
     """
     Process the child contents based on its category.
-    """
-
-    try:
-        # pylint: disable=import-outside-toplevel
-        from xmodule.video_block.transcripts_utils import get_transcript
-    except ImportError:
-        return None
 
+    Returns a string.
+    """
     if category == 'html':
-        try:
-            content_html = child.get_html()
-            text = html_to_text(content_html)
+        content_html = child.get_html()
+        text = html_to_text(content_html)
 
-            return text
-        except AttributeError:
-            return None
+        return text
 
     if category == 'video':
-        try:
-            transcript, _, _ = get_transcript(child, output_format='txt')
-            return transcript
-        except AttributeError:
-            return None
+        transcript = get_text_transcript(child)
+        return transcript
 
     return None
 
 
 def _parse_children_contents(block):
     """
-    Extracts the analyzable contents from its children.
-    Returns length and an item list
-    """
+    Extract the analyzable contents from block children.
 
+    Returns length and an item list.
+    """
     if not _check_summarizable(block):
         return 0, []
 
     content_items = []
 
     children = block.get_children()
     content_length = 0
@@ -110,59 +105,52 @@
         })
 
     return content_length, content_items
 
 
 def _check_summarizable(block):
     """
-    Only if a unit contains HTML blocks with at least a child
-    with sufficient text in them is it worth injecting the summarizer.
+    First pass check if a block has or does not have sufficient text to summarize.
+
     We don't sanitize the content due to performance in this first check.
     """
-
     children = block.get_children()
 
     content_length = 0
 
     for child in children:
-        try:
-            category = child.category
-            if category == 'html':
-                content_length += len(child.get_html())
-                if content_length > settings.SUMMARY_HOOK_MIN_SIZE:
-                    return True
-
-            if category == 'video':
+        category = child.category
+        if category == 'html':
+            content_length += len(child.get_html())
+            if content_length > settings.SUMMARY_HOOK_MIN_SIZE:
                 return True
 
-        except AttributeError:
-            pass
+        if category == 'video':
+            return True
 
     return False
 
 
 class SummaryHookAside(XBlockAside):
     """
-    XBlock aside that injects AI summary javascript
+    XBlock aside that injects AI summary javascript.
     """
 
-    def _get_block(self):
-        """
-        Gets the block wrapped by this aside.
-        """
-
-        from xmodule.modulestore.django import modulestore  # pylint: disable=import-error, import-outside-toplevel
-        return modulestore().get_item(self.scope_ids.usage_id.usage_key)
-
     @XBlock.handler
     def summary_handler(self, request=None, suffix=None):  # pylint: disable=unused-argument
         """
-        Shell handler to the summary xblock aside.
+        Extract and return summarizable text from unit children.
+
+        Only services and staff users are allowed to fetch summary text, everyone else
+        gets an unhelpful 403.
         """
-        block = self._get_block()
+        if not _staff_user(self):
+            return Response(status=403)
+
+        block = get_block(self.scope_ids.usage_id.usage_key)
         valid = self.should_apply_to_block(block)
 
         if not valid:
             return Response(status=404)
 
         published_on = getattr(block, 'published_on', None)
         edited_on = getattr(block, 'published_on', None)
@@ -189,52 +177,95 @@
             'edited_on': _format_date(edited_on),
         }
         return Response(json_body=json)
 
     @XBlockAside.aside_for('student_view')
     def student_view_aside(self, block, context=None):  # pylint: disable=unused-argument
         """
-        Renders the aside contents for the student view
+        Render the aside contents for the student view.
+
+        Returns a Fragment.
+
+        This function absorbs all exceptions to protect the LMS,
+        delegating real work to _student_view_can_throw
+        """
+        try:
+            return self._student_view_can_throw(block)
+        except Exception as ex:  # pylint: disable=broad-exception-caught
+            log.error(f'Summary hook aside suppressed exception during student_view_aside: {ex}')
+            return Fragment('')
+
+    def _student_view_can_throw(self, block):
+        """
+        Render the aside contents for the student view.
+
+        Returns a Fragment.
+
+        This function can throw exceptions.
         """
         fragment = Fragment('')
 
         # Check if there is content that worths summarizing
         length, _ = _parse_children_contents(block)
         if length < settings.SUMMARY_HOOK_MIN_SIZE:
             return fragment
 
-        # thirdparty=true connects to the unauthenticated handler for now,
-        # we will secure it in ACADEMIC-16187
-        handler_url = self.runtime.handler_url(self, 'summary_handler', thirdparty=True)
-
-        # enable ai-spot to see the LMS when they are installed together in devstack
-        aispot_lms_name = settings.AISPOT_LMS_NAME
-        if aispot_lms_name != '':
-            handler_url = handler_url.replace('localhost', aispot_lms_name)
+        handler_url = self._summary_handler_url()
 
         fragment.add_content(
             _render_summary(
                 {
                     'data_url_api': settings.SUMMARY_HOOK_HOST,
                     'data_course_id': block.scope_ids.usage_id.course_key,
                     'data_content_id': block.scope_ids.usage_id,
                     'data_handler_url': handler_url,
                     'js_url': settings.SUMMARY_HOOK_HOST + settings.SUMMARY_HOOK_JS_PATH,
                 }
             )
         )
         return fragment
 
+    def _summary_handler_url(self):
+        """
+        Generate the summary handler URL for this block.
+
+        A separate function to handle overrides required
+        for the unusual use of the handler (non-edx codebase edx service)
+        and to override the URL for use in devstack.
+        """
+        # thirdparty=true gives the full host name and unauthenticated handler
+        handler_url = self.runtime.handler_url(self, 'summary_handler', thirdparty=True)
+        # but we want the authenticated handler
+        handler_url = handler_url.replace('handler_noauth', 'handler')
+        # enable ai-spot to see the LMS when they are installed together in devstack
+        aispot_lms_name = settings.AISPOT_LMS_NAME
+        if aispot_lms_name != '':
+            handler_url = handler_url.replace('localhost', aispot_lms_name)
+        return handler_url
+
     @classmethod
     def should_apply_to_block(cls, block):
         """
-        Overrides base XBlockAside implementation. Indicates whether this aside should
-        apply to a given block type, course, and user.
+        Determine whether this aside should apply to a given block type, course, and user.
+
+        This function absorbs all exceptions to protect the LMS,
+        delegating real work to _should_apply_throws.
         """
+        try:
+            return cls._should_apply_can_throw(block)
+        except Exception as ex:  # pylint: disable=broad-exception-caught
+            log.error(f'Summary hook aside suppressed exception during should_apply_to_block: {ex}')
+            return False
+
+    @classmethod
+    def _should_apply_can_throw(cls, block):
+        """
+        Determine whether this aside should apply to a given block type, course, and user.
 
+        This function can throw exceptions.
+        """
         if getattr(block, 'category', None) != 'vertical':
             return False
         course_key = block.scope_ids.usage_id.course_key
-        if (getattr(block.runtime, 'user_is_staff', False)
-                and summary_staff_only(course_key)):
+        if _staff_user(block) and summary_staff_only(course_key):
             return True
         return summary_enabled(course_key)
```

### Comparing `ai-aside-2.0.2/ai_aside/summaryhook_aside/settings/devstack.py` & `ai-aside-3.0.0/ai_aside/settings/devstack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Devstack settings values."""
+"""devstack settings values."""
 
 import os
 from os.path import abspath, dirname, join
 
 
 def plugin_settings(settings):
     """ Override/set summary hook devstack settings"""
```

### Comparing `ai-aside-2.0.2/ai_aside/summaryhook_aside/text_utils.py` & `ai-aside-3.0.0/ai_aside/text_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,59 +6,57 @@
 from re import sub
 
 from django.conf import settings
 
 
 def cleanup_text(text):
     """
-    Removes litter from replacing or manipulating text
+    Remove litter from replacing or manipulating text.
     """
     stripped = sub(r'[^\S\r\n]+', ' ', text)  # Removing extra spaces
     stripped = sub(r'\n{2,}', '\n', stripped)  # Removing extra new lines
     stripped = sub(r'(\s+)?\n(\s+)?', '\n', stripped)  # Removing starting extra spacesbetween new lines
     stripped = sub(r'(^(\s+)\n?)|(\n(\s+)?$)', '', stripped)  # Trim
 
     return stripped
 
 
 class _HTMLToTextHelper(HTMLParser):  # lint-amnesty, pylint: disable=abstract-method
     """
-    Helper function for html_to_text below
+    Helper function for html_to_text below.
     """
+
     _is_content = True
 
     def __init__(self):
         HTMLParser.__init__(self)
         self.reset()
         self.fed = []
 
     def handle_starttag(self, tag, _):
-        """This runs when a new tag is found. We use this to exclude unwanted content."""
+        """On each tag, check whether this is a tag we think is content."""
         tags_to_filter = getattr(settings, 'HTML_TAGS_TO_REMOVE', None)
         self._is_content = not (tags_to_filter and tag in tags_to_filter)
 
     def handle_data(self, data):
-        """takes the data in separate chunks"""
+        """Handle tag data by appending text we think is content."""
         if self._is_content:
             self.fed.append(data)
 
     def handle_entityref(self, name):
-        """appends the reference to the body"""
+        """If there is an entity, append the reference to the text."""
         if self._is_content:
             self.fed.append('&%s;' % name)
 
     def get_data(self):
-        """joins together the seperate chunks into one cohesive string"""
+        """Join together the separate data chunks into one cohesive string."""
         return ''.join(self.fed)
 
 
 def html_to_text(html):
-    """
-    Strips the html tags off of the text to return plaintext
-    """
-
+    """Strip the html tags off of the text to return plaintext."""
     htmlstripper = _HTMLToTextHelper()
     htmlstripper.feed(html)
     text = htmlstripper.get_data()
     text = cleanup_text(text)
 
     return text
```

### Comparing `ai-aside-2.0.2/ai_aside/summaryhook_aside/waffle.py` & `ai-aside-3.0.0/ai_aside/waffle.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """
 Waffle flag controlling summary hook distribution.
+
 Xblocks do not generally use waffle flags,
 import at use time method taken from the LTI Xblock
 """
 
 # Namespace
 WAFFLE_NAMESPACE = 'summaryhook'
 
@@ -31,15 +32,15 @@
 # .. toggle_tickets: ACADEMIC-15709 (2U)
 # .. toggle_warning: None.
 SUMMARYHOOK_STAFF_ONLY = 'summaryhook_staff_only'
 
 
 def _get_summaryhook_waffle_flag(flag_name):
     """
-    Import and return Waffle flag for enabling the summary hook
+    Import and return Waffle flag for enabling the summary hook.
     """
     # pylint: disable=import-error,import-outside-toplevel
     from openedx.core.djangoapps.waffle_utils import CourseWaffleFlag
     return CourseWaffleFlag(f'{WAFFLE_NAMESPACE}.{flag_name}', __name__)
 
 
 def summary_enabled(course_key):
```

### Comparing `ai-aside-2.0.2/ai_aside.egg-info/PKG-INFO` & `ai-aside-3.0.0/ai_aside.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-aside
-Version: 2.0.2
+Version: 3.0.0
 Summary: A plugin containing xblocks and apps supporting GPT and other LLM use on edX.
 Home-page: https://github.com/openedx/ai-aside
 Author: edX
 Author-email: ashultz@edx.org
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -44,15 +44,26 @@
   cd ai-aside
 
   # Set up a virtualenv using virtualenvwrapper with the same name as the repo and activate it
   mkvirtualenv -p python3.8 ai-aside
 
 Local testing
 ~~~~~~~~~~~~~
-To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run ``pip install -e /edx/src/ai-aside``.  The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+To test your changes locally, you will need to install the package from your local branch into edx-platform. For example, if using devstack, copy or clone your branch into <devstack-parent>/src/ai-aside. Then, in an lms or cms shell, run::
+
+  pip install -e /edx/src/ai-aside
+
+The plug-in configuration will automatically be picked up once installed, and changes will be hot reloaded.
+
+Run Migrations
+..............
+You will also need to run migrations for local testing. Using the same lms or cms shell as before, run::
+
+  ./manage.py lms migrate ai_aside
+
 
 Testing in Docker with AI-spot
 ..............................
 
 If you are running both devstack and a local instance of the supporting ai-spot in docker, you need two pieces of special setup to let ai-spot call the aside handler and retrieve content.
 
 The first is to connect ai-spot to the devstack network with a docker command::
@@ -196,14 +207,24 @@
    This project adheres to Semantic Versioning (https://semver.org/).
 
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
+
+3.0.0 – 2023-07-16
+**********************************************
+
+Features
+=========
+* Summary content handler now requires a staff user identity, otherwise returns 403. This is a breaking change.
+* Added models to summaryhook_aside (Has migrations)
+* Catch exceptions in a couple of locations so the aside cannot crash content.
+
 2.0.2 – 2023-07-05
 **********************************************
 
 Fix
 =====
 
 * Updated HTML parser to remove tags with their content for specific cases like `<script>` or `<style>`.
```

### Comparing `ai-aside-2.0.2/requirements/constraints.txt` & `ai-aside-3.0.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `ai-aside-2.0.2/setup.py` & `ai-aside-3.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,14 @@
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
     ],
     entry_points={
         "lms.djangoapp": [
             "ai_aside = ai_aside.apps:AiAsideConfig",
-            "summaryhook = ai_aside.summaryhook_aside.apps:SummaryHookConfig",
         ],
         "xblock_asides.v1": [
-            "summaryhook_aside = ai_aside.summaryhook_aside.block:SummaryHookAside",
+            "summaryhook_aside = ai_aside.block:SummaryHookAside",
         ],
     },
 
 )
```

