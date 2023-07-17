# Comparing `tmp/mkdocs_unused_files-0.1.7-py3-none-any.whl.zip` & `tmp/mkdocs_unused_files-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4112 bytes, number of entries: 8
+Zip file size: 4173 bytes, number of entries: 8
 -rw-r--r--  2.0 unx        0 b- defN 23-Jan-25 12:48 mkdocs_unused_files/__init__.py
--rw-r--r--  2.0 unx     3454 b- defN 23-Mar-30 06:42 mkdocs_unused_files/plugin.py
--rw-r--r--  2.0 unx     1057 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/LICENSE
--rw-r--r--  2.0 unx      899 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       77 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       20 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      723 b- defN 23-Mar-30 06:51 mkdocs_unused_files-0.1.7.dist-info/RECORD
-8 files, 6322 bytes uncompressed, 2820 bytes compressed:  55.4%
+-rw-r--r--  2.0 unx     3724 b- defN 23-Jul-17 15:01 mkdocs_unused_files/plugin.py
+-rw-r--r--  2.0 unx     1057 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      899 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       77 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       20 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      723 b- defN 23-Jul-17 15:23 mkdocs_unused_files-0.2.0.dist-info/RECORD
+8 files, 6592 bytes uncompressed, 2881 bytes compressed:  56.3%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
 Filename: mkdocs_unused_files/__init__.py
 Comment: 
 
 Filename: mkdocs_unused_files/plugin.py
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/LICENSE
+Filename: mkdocs_unused_files-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/METADATA
+Filename: mkdocs_unused_files-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/WHEEL
+Filename: mkdocs_unused_files-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/entry_points.txt
+Filename: mkdocs_unused_files-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/top_level.txt
+Filename: mkdocs_unused_files-0.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: mkdocs_unused_files-0.1.7.dist-info/RECORD
+Filename: mkdocs_unused_files-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mkdocs_unused_files/plugin.py

```diff
@@ -1,10 +1,11 @@
 import os
 import logging
 import urllib.parse
+from fnmatch import fnmatch
 from mkdocs.config import config_options
 from mkdocs.plugins import BasePlugin
 from bs4 import BeautifulSoup
 
 log = logging.getLogger('mkdocs')
 
 class UnusedFilesPlugin(BasePlugin):
@@ -46,15 +47,20 @@
             for file in files:
                 # Add all files with the given types to file_list
                 # If no types were given, add all files except Markdown files
                 if not file.endswith("md") and self._matches_type(file):
                     # Create entry from relative path between full path and docs_dir + filename
                     # When path and docs_dir are identical, relpath returns ".". We use normpath() to resolve that
                     entry = os.path.normpath(os.path.join(os.path.relpath(path, config.docs_dir), file))
-                    if entry in self.config['excluded_files']:
+                    # Check whether file is excluded
+                    is_excluded = False
+                    for excluded_file in self.config['excluded_files']:
+                        if fnmatch(file, excluded_file):
+                            is_excluded = True
+                    if is_excluded:
                         continue
                     self.file_list.append(entry)
 
     def on_page_content(self, html, page, config, files):
         if not self.config['enabled']:
             return
         soup = BeautifulSoup(html, 'html.parser')
```

## Comparing `mkdocs_unused_files-0.1.7.dist-info/LICENSE` & `mkdocs_unused_files-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mkdocs_unused_files-0.1.7.dist-info/METADATA` & `mkdocs_unused_files-0.2.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-unused-files
-Version: 0.1.7
+Version: 0.2.0
 Summary: An MkDocs plugin to find unused (orphaned) files in your project.
 Home-page: https://github.com/wilhelmer/mkdocs-unused-files.git
 Author: Lars Wilhelmer
 Author-email: lars@wilhelmer.de
 License: MIT
 Keywords: mkdocs
 Classifier: Development Status :: 4 - Beta
```

## Comparing `mkdocs_unused_files-0.1.7.dist-info/RECORD` & `mkdocs_unused_files-0.2.0.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 mkdocs_unused_files/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-mkdocs_unused_files/plugin.py,sha256=8i36DE4TN_E9ameBSsWQmku9WvkZWAmk5p6fCsxqVKg,3454
-mkdocs_unused_files-0.1.7.dist-info/LICENSE,sha256=l_aq6Ck7Pdjl6NspuSMc7O0sLCqbsdA8cGuX_mfyPCM,1057
-mkdocs_unused_files-0.1.7.dist-info/METADATA,sha256=aoabiIZHhdSi45cMes4w5fGMteFfig7nWh1kRoy5zWo,899
-mkdocs_unused_files-0.1.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mkdocs_unused_files-0.1.7.dist-info/entry_points.txt,sha256=pxxsTzp99TkrYk0Tuw_qqxm1499Srd15iUOBWle1qX8,77
-mkdocs_unused_files-0.1.7.dist-info/top_level.txt,sha256=UnE7CfvDi55e_mYysxk4NH2_-sw2wyzxjEQcKOL0Jh4,20
-mkdocs_unused_files-0.1.7.dist-info/RECORD,,
+mkdocs_unused_files/plugin.py,sha256=WzYGLfN4JSYnnJftvR886odsDxv2FdNmRztWNxKbik8,3724
+mkdocs_unused_files-0.2.0.dist-info/LICENSE,sha256=l_aq6Ck7Pdjl6NspuSMc7O0sLCqbsdA8cGuX_mfyPCM,1057
+mkdocs_unused_files-0.2.0.dist-info/METADATA,sha256=A_xEOSGxq91N2ODnZe0-dpcZDd93-dlyjlK2zEDkKwg,899
+mkdocs_unused_files-0.2.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mkdocs_unused_files-0.2.0.dist-info/entry_points.txt,sha256=pxxsTzp99TkrYk0Tuw_qqxm1499Srd15iUOBWle1qX8,77
+mkdocs_unused_files-0.2.0.dist-info/top_level.txt,sha256=UnE7CfvDi55e_mYysxk4NH2_-sw2wyzxjEQcKOL0Jh4,20
+mkdocs_unused_files-0.2.0.dist-info/RECORD,,
```

