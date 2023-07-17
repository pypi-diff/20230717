# Comparing `tmp/bilix-1.0a0.tar.gz` & `tmp/bilix-1.0a1.tar.gz`

## Comparing `bilix-1.0a0.tar` & `bilix-1.0a1.tar`

### file list

```diff
@@ -1,61 +1,66 @@
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/__init__.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/__main__.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/_process.py
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/exception.py
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/ffmpeg.py
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/log.py
--rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/utils.py
--rw-r--r--   0        0        0     3461 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/assign.py
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/core.py
--rw-r--r--   0        0        0     6446 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/handler.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/cli/main.py
--rw-r--r--   0        0        0    10400 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader.py
--rw-r--r--   0        0        0     8952 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader_m3u8.py
--rw-r--r--   0        0        0    10165 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/base_downloader_part.py
--rw-r--r--   0        0        0     4245 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/download/utils.py
--rw-r--r--   0        0        0     1309 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/abc.py
--rw-r--r--   0        0        0     3945 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/cli_progress.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/progress/ws_progress.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/__init__.py
--rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/api.py
--rw-r--r--   0        0        0     4670 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/api_test.py
--rw-r--r--   0        0        0    27218 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/downloader.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/downloader_test.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/informer.py
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/bilibili/informer_test.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/__init__.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/api.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/api_test.py
--rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/cctv/downloader.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/__init__.py
--rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/api.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/api_test.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/downloader.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/douyin/downloader_test.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/__init__.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/api.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/api_test.py
--rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/hanime1/downloader.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/__init__.py
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/api.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/api_test.py
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/jable/downloader.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/__init__.py
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/api.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/api_test.py
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/downloader.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/tiktok/downloader_test.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/__init__.py
--rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/api.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/api_test.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/downloader.py
--rw-r--r--   0        0        0    23731 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yhdmp/yhdmp.js
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/__init__.py
--rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/api.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/api_test.py
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bilix-1.0a0/bilix/sites/yinghuacd/downloader.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bilix-1.0a0/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 bilix-1.0a0/LICENSE
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 bilix-1.0a0/README.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 bilix-1.0a0/pyproject.toml
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 bilix-1.0a0/PKG-INFO
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/__init__.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/__main__.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/_process.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/exception.py
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/ffmpeg.py
+-rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/log.py
+-rw-r--r--   0        0        0     3406 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/utils.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/cli/assign.py
+-rw-r--r--   0        0        0     9848 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/cli/core.py
+-rw-r--r--   0        0        0     6478 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/cli/handler.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/cli/main.py
+-rw-r--r--   0        0        0     6008 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/download/auto_downloader.py
+-rw-r--r--   0        0        0    11779 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/download/base_downloader.py
+-rw-r--r--   0        0        0     8859 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/download/base_downloader_m3u8.py
+-rw-r--r--   0        0        0    10018 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/download/base_downloader_part.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/download/utils.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/progress/abc.py
+-rw-r--r--   0        0        0     3944 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/progress/cli_progress.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/progress/ws_progress.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/__init__.py
+-rw-r--r--   0        0        0    17993 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/api.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/api_test.py
+-rw-r--r--   0        0        0    30099 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/downloader.py
+-rw-r--r--   0        0        0     2927 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/downloader_test.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/informer.py
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/bilibili/informer_test.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/cctv/__init__.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/cctv/api.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/cctv/api_test.py
+-rw-r--r--   0        0        0     3194 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/cctv/downloader.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/douyin/__init__.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/douyin/api.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/douyin/api_test.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/douyin/downloader.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/douyin/downloader_test.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/hanime1/__init__.py
+-rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/hanime1/api.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/hanime1/api_test.py
+-rw-r--r--   0        0        0     2065 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/hanime1/downloader.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/jable/__init__.py
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/jable/api.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/jable/api_test.py
+-rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/jable/downloader.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/tiktok/__init__.py
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/tiktok/api.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/tiktok/api_test.py
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/tiktok/downloader.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/tiktok/downloader_test.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yhdmp/__init__.py
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yhdmp/api.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yhdmp/api_test.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yhdmp/downloader.py
+-rw-r--r--   0        0        0    23731 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yhdmp/yhdmp.js
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yinghuacd/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yinghuacd/api.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yinghuacd/api_test.py
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/yinghuacd/downloader.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/youtube/__init__.py
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/youtube/api.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/youtube/api_test.py
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 bilix-1.0a1/bilix/sites/youtube/downloader.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 bilix-1.0a1/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 bilix-1.0a1/LICENSE
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 bilix-1.0a1/README.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 bilix-1.0a1/pyproject.toml
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 bilix-1.0a1/PKG-INFO
```

### Comparing `bilix-1.0a0/bilix/_process.py` & `bilix-1.0a1/bilix/_process.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/exception.py` & `bilix-1.0a1/bilix/exception.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/ffmpeg.py` & `bilix-1.0a1/bilix/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/utils.py` & `bilix-1.0a1/bilix/utils.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/cli/assign.py` & `bilix-1.0a1/bilix/cli/assign.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,15 @@
         yield ModuleInfo(f'bilix.sites.{site.name}', site.name)
 
 
 def base_module_infos():
     infos = (
         ModuleInfo('bilix.download.base_downloader_m3u8', cmp_key='m3u8'),
         ModuleInfo('bilix.download.base_downloader_part', cmp_key='file'),
+        ModuleInfo('bilix.download.auto_downloader', cmp_key='autov'),
     )
     for info in infos:
         yield info
 
 
 def sorted_modules(method: str, keys: List[str]) -> List[ModuleInfo]:
     pattern = re.compile(r"https?://(?:[\w-]*\.)?([\w-]+)\.([\w-]+)")
@@ -66,20 +67,24 @@
     infos = chain(base_module_infos(), sites_module_infos())
     return sorted(infos, key=key, reverse=True)
 
 
 def handler_classes(module: ModuleType):
     """find and yield all available handler class in module"""
     attrs = getattr(module, '__all__', None)
-    attrs = attrs or dir(module)
+    if attrs is None:
+        attrs = dir(module)
     for attr_name in attrs:
         if attr_name.startswith('_'):
             continue
         handler_cls = getattr(module, attr_name)
-        if not issubclass(handler_cls, Handler):
+        try:
+            if not issubclass(handler_cls, Handler):
+                continue
+        except TypeError:
             continue
         yield handler_cls
 
 
 def assign(method: str, keys: List[str]) -> Handler:
     if len(keys) == 0:
         raise UsageError("at least one key is required")
```

### Comparing `bilix-1.0a0/bilix/cli/core.py` & `bilix-1.0a1/bilix/cli/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 """
 use handler to provide click(typer) cli service
 """
 from importlib import import_module
 from typing import List, Optional, Union, get_origin, get_args, Annotated
 from click import UsageError, Context, Command
-from rich.padding import Padding
 from rich.panel import Panel
 from rich.table import Table
 from typer import rich_utils
 from typer.models import OptionInfo, ParameterInfo, ParamMeta
 from typer.core import TyperCommand, TyperOption, TyperArgument
 from typer.main import get_click_param
-from typer.rich_utils import STYLE_OPTIONS_PANEL_BORDER, ALIGN_OPTIONS_PANEL, highlighter
-from bilix import __version__
+from typer.rich_utils import STYLE_OPTIONS_PANEL_BORDER, ALIGN_OPTIONS_PANEL
 from bilix.cli.assign import assign, sites_module_infos, base_module_infos, sorted_modules, handler_classes
 from bilix.cli.handler import ParamInfo, Handler
 from bilix.log import logger
 from rich import print as rprint
 from rich.markdown import Markdown
 
 
@@ -26,15 +24,14 @@
 
     if annotation == p.empty and default != p.empty:
         annotation = type(default)
     elif (origin := get_origin(annotation)) is Union:
         annotation = get_args(annotation)[0]  # use the first type in Union, it's a convention
     elif origin is Annotated:
         # base_annotation, *convertors = get_args(annotation)
-        # todo metavar
         annotation = str
     # convert default to OptionInfo to ensure no ArgumentInfo is created
     if not isinstance(default, ParameterInfo):
         default = OptionInfo(default=... if default == p.empty else default, help=p.desc)
     return ParamMeta(name=p.name, annotation=annotation, default=default)
 
 
@@ -208,18 +205,19 @@
             self.help = f"✨ {ctx.obj['method'].desc}"
             return rich_utils.rich_format_help(
                 obj=self,
                 ctx=ctx,
                 markup_mode=self.rich_markup_mode,
             )
         else:
-            rprint(Padding(
-                highlighter(f"⚡️ bilix: a lightning-fast async download tool. Version {__version__}"),
-                1
-            ))
+            rich_utils.rich_format_help(
+                obj=self,
+                ctx=ctx,
+                markup_mode=self.rich_markup_mode,
+            )
             msg = "bilix supports many sites:\n"
             for info in sorted(sites_module_infos(), key=lambda x: x.cmp_key):  # alphasort
                 msg += f"* {info.cmp_key}\n"
             msg += "\n✨ use `bilix help <site>` to see more\n"
             rprint(Panel(
                 Markdown(msg),
                 border_style=STYLE_OPTIONS_PANEL_BORDER,
```

### Comparing `bilix-1.0a0/bilix/cli/handler.py` & `bilix-1.0a1/bilix/cli/handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
     pattern: re.Pattern = None
     cli_info: Dict[str, MethodInfo]
 
     @classmethod
     def decide_handle(cls, method_name: str, keys: Tuple[str, ...]) -> bool:
         """check if the method and keys can be handled by this handler"""
         if cls.pattern:
-            return cls.pattern.match(keys[0]) is not None
+            return cls.pattern.match(keys[0]) is not None and method_name in cls.cli_info
         else:
             return method_name in cls.cli_info
 
     @classmethod
     def handle(
             cls,
             method_name: str,
```

### Comparing `bilix-1.0a0/bilix/cli/main.py` & `bilix-1.0a1/bilix/cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 import asyncio
 import click
-from click.testing import CliRunner
 from bilix import __version__
 from bilix.log import logger
 from bilix.cli.core import CustomCommand
 from bilix.progress.cli_progress import CLIProgress
 
 
 def handle_version(ctx: click.Context, param, value):
     if not value or ctx.resilient_parsing:
         return
     print(f"Version {__version__}")
     ctx.exit()
 
 
-@click.command(cls=CustomCommand)
+@click.command(cls=CustomCommand,
+               help=f"""⚡️ bilix: a lightning-fast async download tool. Version {__version__}""")
 @click.option(
     "--debug",
     is_flag=True,
     is_eager=True,
-    expose_value=False,
     help="Enable debug mode.",
 )
 @click.option(
     "--version", '-v',
     is_flag=True,
     is_eager=True,
     expose_value=False,
     callback=handle_version,
     help="Show version and exit",
 )
 @click.pass_context
-def main(ctx, method, keys, **options):
+def main(ctx, method=None, keys=None, **options):
+    if method is None and keys is None:
+        print(ctx.get_help())
+        ctx.exit()
+    debug = options.pop('debug')
     loop = asyncio.new_event_loop()  # avoid deprecated warning in 3.11
     asyncio.set_event_loop(loop)
     logger.debug(f"method: {method}, keys: {keys}, options: {options}")
 
     handler_cls = ctx.obj['handler_cls']
     init_options = {op: options[op] for op in ctx.obj['init_options']}
     method_options = {op: options[op] for op in ctx.obj['method_options']}
     handler, cor = handler_cls.handle(method, keys, init_options, method_options)
 
     try:
         CLIProgress.start()
         loop.run_until_complete(cor)
     except KeyboardInterrupt:
-        logger.info('[cyan]提示：用户中断，重复执行命令可继续下载')
+        logger.interrupted()
+    except Exception as e:
+        if debug:
+            raise e
+        else:
+            logger.error(f"Unexpected Exception: {repr(e)}. Use --debug to see more information.")
     finally:
         CLIProgress.stop()
```

### Comparing `bilix-1.0a0/bilix/download/base_downloader.py` & `bilix-1.0a1/bilix/download/base_downloader.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import asyncio
 import inspect
-import logging
 import time
 import random
 from collections import defaultdict
 from functools import wraps
-from typing import Union, Optional, Callable, Dict, Any, Tuple, List, Set, Annotated, get_origin, get_args, \
-    get_type_hints
+from typing import Union, Optional, Callable, Dict, Any, Tuple, List, Set, Annotated, get_origin, get_args
 from contextlib import asynccontextmanager
 from urllib.parse import urlparse
 import aiofiles
 import httpx
 
 from bilix.cli.handler import Handler, HandlerMeta
-from bilix.log import logger as dft_logger
-from bilix.download.utils import req_retry, path_check, parse_speed_str, str2path
+from bilix.log import logger as dft_logger, CustomLogger
+from bilix.download.utils import path_check, parse_speed_str, str2path
 from bilix.progress.abc import Progress
 from bilix.progress.cli_progress import CLIProgress
 from pathlib import Path, PurePath
 
 
 def is_instance_of_generic_type(value: Any, target_type: Any) -> bool:
     origin = get_origin(target_type)
@@ -111,15 +109,15 @@
             self,
             *,
             client: httpx.AsyncClient = None,
             browser: str = None,
             speed_limit: Annotated[float, parse_speed_str] = None,
             stream_retry: int = 5,
             progress: Progress = None,
-            logger: logging.Logger = None,
+            logger: CustomLogger = None,
     ):
         """
         :param client: client used for http request
         :param browser: load cookies from which browser
         :param stream_retry: retry times for http stream
         :param speed_limit: global download rate for the downloader. should be a float (Byte/s unit) or str (e.g. 1.5MB)
         :param progress: progress obj used to output download progress
@@ -146,38 +144,66 @@
     async def __aexit__(self, exc_type, exc_val, exc_tb):
         await self.client.__aexit__(exc_type, exc_val, exc_tb)
 
     async def aclose(self):
         """Close transport and proxies for httpx client"""
         await self.client.aclose()
 
-    async def get_static(self, url: str, path: Annotated[Path, str2path], convert_func=None) -> Path:
+    async def get_static(self, url: str, path: Annotated[Path, str2path], convert_func=None, task_id=None) -> Path:
         """
         download static file from url
         :param url:
         :param path: file path without suffix
         :param convert_func: function used to convert http bytes content, must be named like ...2...
+        :param task_id: task id used to update progress, if None, progress will not be updated
         :return: downloaded file path
         """
         # use suffix from convert_func's name
         if convert_func:
             suffix = '.' + convert_func.__name__.split('2')[-1]
         # try to find suffix from url
         else:
             suffix = PurePath(urlparse(url).path).suffix
         path = path.with_name(path.name + suffix)
         exist, path = path_check(path)
         if exist:
-            self.logger.info(f'[green]已存在[/green] {path.name}')
+            if task_id is None:
+                self.logger.exist(path.name)
             return path
-        res = await req_retry(self.client, url)
-        content = convert_func(res.content) if convert_func else res.content
+
+        async def update_progress_total(length):
+            if (t := self.progress.tasks[task_id].total) is None:
+                await self.progress.update(task_id, total=length, visible=True)
+            else:
+                await self.progress.update(task_id, total=length + t)
+
+        for times in range(1 + self.stream_retry):
+            content = bytearray()
+            try:
+                async with self.client.stream('GET', url) as r, self._stream_context(times):
+                    r.raise_for_status()
+                    if task_id is not None and 'content-length' in r.headers and not content:
+                        await update_progress_total(int(r.headers['content-length']))
+                    async for chunk in r.aiter_bytes(chunk_size=self._chunk_size):
+                        content.extend(chunk)
+                        if task_id is not None:
+                            await self.progress.update(task_id, advance=len(chunk))
+                        await self._check_speed(len(chunk))
+                if task_id is not None and 'content-length' not in r.headers:
+                    await update_progress_total(len(content))
+                break
+            except (httpx.HTTPStatusError, httpx.TransportError):
+                continue
+        else:
+            raise Exception(f"STREAM max retry {url}")
+        content = convert_func(bytes(content)) if convert_func else content
         async with aiofiles.open(path, 'wb') as f:
             await f.write(content)
-        self.logger.info(f'[cyan]已完成[/cyan] {path.name}')
+        if task_id is None:
+            self.logger.done(path.name)
         return path
 
     def _change_sore(self, exc: Union[httpx.HTTPStatusError, httpx.TransportError]):
         """change url score according to exception"""
         # todo clean score
         if isinstance(exc, httpx.HTTPStatusError):
             self._url_score[exc.request.url] -= 4
```

### Comparing `bilix-1.0a0/bilix/download/base_downloader_m3u8.py` & `bilix-1.0a1/bilix/download/base_downloader_m3u8.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         """
         if path.is_dir():
             path = (path / PurePath(urlparse(m3u8_url).path).stem).with_suffix('.mp4')
         if time_range:
             path = path.with_stem(f"{path.stem}-{time_range[0]}-{time_range[1]}")
         exist, path = path_check(path)
         if exist:
-            self.logger.info(f"[green]已存在[/green] {path.name}")
+            self.logger.exist(path.name)
             return path
         async with self.v_sema:
             task_id = await self.progress.add_task(total=None, description=path.name)
             m3u8_info = await self.to_invariant_m3u8(m3u8_url)
             cors = []
             p_sema = asyncio.Semaphore(self.part_concurrency)
             total_time = 0
@@ -126,15 +126,15 @@
             file_list = await asyncio.gather(*cors)
         await ffmpeg.concat(file_list, path)
         if time_range:
             path_tmp = path.with_stem(str(uuid.uuid4()))
             # to save key frame, use 0 as start time instead of s, clip will be a little longer than expected
             await ffmpeg.time_range_clip(path, 0, end_time - start_time + s, path_tmp)
             os.rename(path_tmp, path)
-        self.logger.info(f"[cyan]已完成[/cyan] {path.name}")
+        self.logger.done(path.name)
         await self.progress.update(task_id, visible=False)
         return path
 
     async def _update_task_total(self, task_id, time_part: float, update_size: int):
         task = self.progress.tasks[task_id]
         if task.total is None:
             confirmed_t = time_part
@@ -150,15 +150,14 @@
         if exists:
             downloaded = os.path.getsize(path)
             await self._update_task_total(task_id, time_part=seg.duration, update_size=downloaded)
             await self.progress.update(task_id, advance=downloaded)
             return path
         seg_url = seg.absolute_uri
         async with p_sema:
-            content = None
             for times in range(1 + self.stream_retry):
                 content = bytearray()
                 try:
                     async with self.client.stream("GET", seg_url,
                                                   follow_redirects=True) as r, self._stream_context(times):
                         r.raise_for_status()
                         # pre-update total if content-length is provided and first time to get content
@@ -171,15 +170,15 @@
                             await self._check_speed(len(chunk))
                     if 'content-length' not in r.headers:  # after-update total if content-length is not provided
                         await self._update_task_total(task_id, time_part=seg.duration, update_size=len(content))
                     break
                 except (httpx.HTTPStatusError, httpx.TransportError):
                     continue
             else:
-                raise Exception(f"STREAM 超过重复次数 {seg_url}")
+                raise Exception(f"STREAM max retry {seg_url}")
         content = self._after_seg(seg, content)
         # in case encrypted
         if seg.key:
             content = await self._decrypt(seg, content)
         async with aiofiles.open(path, 'wb') as f:
             await f.write(content)
         return path
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bilix-1.0a0/bilix/download/base_downloader_part.py` & `bilix-1.0a1/bilix/download/base_downloader_part.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         :param task_id:
         :return:
         """
         upper = task_id is not None and self.progress.tasks[task_id].fields.get('upper', None)
         exist, path = path_check(path)
         if exist:
             if not upper:
-                self.logger.info(f'[green]已存在[/green] {path.name}')
+                self.logger.exist(path.name)
             return path
 
         urls = [url_or_urls] if isinstance(url_or_urls, str) else [url for url in url_or_urls]
         init_start, init_end = map(int, init_range.split('-'))
         seg_start, seg_end = map(int, seg_range.split('-'))
         res = await req_retry(self.client, urls[0], follow_redirects=True,
                               headers={'Range': f'bytes={seg_start}-{seg_end}'})
@@ -143,15 +143,15 @@
         await merge_files(file_list, path_tmp)
         if set_s:
             await ffmpeg.time_range_clip(path_tmp, start=0, t=end_time - start_time + s, output_path=path)
         else:
             await ffmpeg.time_range_clip(path_tmp, start=s, t=end_time - start_time, output_path=path)
         if not upper:  # no upstream task
             await self.progress.update(task_id, visible=False)
-            self.logger.info(f"[cyan]已完成[/cyan] {path.name}")
+            self.logger.done(path.name)
         return path
 
     async def get_file(
             self,
             url_or_urls: Union[str, Iterable[str]],
             path: Annotated[Path, str2path] = Path('.'),
             task_id=None
@@ -167,26 +167,26 @@
         urls = [url_or_urls] if isinstance(url_or_urls, str) else [url for url in url_or_urls]
         upper = task_id is not None and self.progress.tasks[task_id].fields.get('upper', None)
 
         if not path.is_dir():
             exist, path = path_check(path)
             if exist:
                 if not upper:
-                    self.logger.info(f'[green]已存在[/green] {path.name}')
+                    self.logger.exist(path.name)
                 return path
 
         total, req_filename = await self._pre_req(urls)
 
         if path.is_dir():
             file_name = req_filename if req_filename else PurePath(urlparse(urls[0]).path).name
             path /= file_name
             exist, path = path_check(path)
             if exist:
                 if not upper:
-                    self.logger.info(f'[green]已存在[/green] {path.name}')
+                    self.logger.exist(path.name)
                 return path
 
         if task_id is not None:
             await self.progress.update(
                 task_id,
                 total=self.progress.tasks[task_id].total + total if self.progress.tasks[task_id].total else total)
         else:
@@ -197,15 +197,15 @@
             start = i * part_length
             end = (i + 1) * part_length - 1 if i < self.part_concurrency - 1 else total - 1
             cors.append(self._get_file_part(urls, path=path, part_range=(start, end), task_id=task_id))
         file_list = await asyncio.gather(*cors)
         await merge_files(file_list, new_path=path)
         if not upper:
             await self.progress.update(task_id, visible=False)
-            self.logger.info(f"[cyan]已完成[/cyan] {path.name}")
+            self.logger.done(path.name)
         return path
 
     async def _get_file_part(self, urls: List[str], path: Path, part_range: Tuple[int, int],
                              task_id) -> Path:
         start, end = part_range
         part_path = path.with_name(f'{path.name}.{part_range[0]}-{part_range[1]}')
         exist, part_path = path_check(part_path)
@@ -222,19 +222,19 @@
                 async with \
                         self.client.stream("GET", urls[url_idx], follow_redirects=True,
                                            headers={'Range': f'bytes={start}-{end}'}) as r, \
                         self._stream_context(times), \
                         aiofiles.open(part_path, 'ab') as f:
                     r.raise_for_status()
                     if r.history:  # avoid twice redirect
-                        urls[url_idx] = r.url
+                        urls[url_idx] = str(r.url)
                     async for chunk in r.aiter_bytes(chunk_size=self._chunk_size):
                         await f.write(chunk)
                         start += len(chunk)
                         await self.progress.update(task_id, advance=len(chunk))
                         await self._check_speed(len(chunk))
                 break
             except (httpx.HTTPStatusError, httpx.TransportError):
                 continue
         else:
-            raise Exception(f"STREAM 超过重复次数 {part_path.name}")
+            raise Exception(f"STREAM max retry {part_path.name}")
         return part_path
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bilix-1.0a0/bilix/download/utils.py` & `bilix-1.0a1/bilix/download/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,19 +39,19 @@
             pre_exc = e
             await asyncio.sleep(.1 * (times + 1))
         except httpx.HTTPStatusError as e:
             logger.warning(f'{method} {e.response.status_code} {url}')
             pre_exc = e
             await asyncio.sleep(1. * (times + 1))
         except Exception as e:
-            logger.warning(f'{method} {e.__class__.__name__} 未知异常 url: {url}')
+            logger.warning(f'{method} Unknown Exception {e.__class__.__name__} url: {url}')
             raise e
         else:
             return res
-    logger.error(f"{method} 超过重复次数 {url_or_urls}")
+    logger.error(f"{method} max retry {url_or_urls}")
     raise pre_exc
 
 
 def eclipse_str(s: str, max_len: int = 100):
     if len(s) <= max_len:
         return s
     else:
```

### Comparing `bilix-1.0a0/bilix/progress/abc.py` & `bilix-1.0a1/bilix/progress/abc.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         """return current active speed (bit/s)"""
 
     @abstractmethod
     async def add_task(
             self,
             description: str,
             start: bool = True,
-            total: Optional[float] = 100.0,
+            total: Optional[float] = None,
             completed: int = 0,
             visible: bool = True,
             **fields,
     ):
         """async add a task to progress"""
 
     @abstractmethod
```

### Comparing `bilix-1.0a0/bilix/progress/cli_progress.py` & `bilix-1.0a1/bilix/progress/cli_progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         mid = (max_length - 3) // 2
         return description if len(description) < max_length else f'{description[:mid]}...{description[-mid:]}'
 
     async def add_task(
             self,
             description: str,
             start: bool = True,
-            total: Optional[float] = 100.0,
+            total: Optional[float] = None,
             completed: int = 0,
             visible: bool = True,
             **fields: Any,
     ) -> TaskID:
         task_id = self._progress.add_task(description=self._cat_description(description),
                                           start=start, total=total, completed=completed, visible=visible, **fields)
         self._active_ids.add(task_id)
```

### Comparing `bilix-1.0a0/bilix/progress/ws_progress.py` & `bilix-1.0a1/bilix/progress/ws_progress.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/bilibili/api.py` & `bilix-1.0a1/bilix/sites/bilibili/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,43 +159,59 @@
     data = dict(sorted(params.items()))
     data_str = "&".join([f"{k}={v}" for k, v in data.items()]) + request_token
     md5 = hashlib.md5(data_str.encode("utf-8")).hexdigest()
     params["w_rid"] = md5
     return params
 
 
+def _find_mid(space_url: str):
+    return re.search(r'^https://space.bilibili.com/(\d+)/?', space_url).group(1)
+
+
 @raise_api_error
-async def get_up_info(client: httpx.AsyncClient, url_or_mid: str, pn=1, ps=30, order="pubdate", keyword=""):
+async def get_up_video_info(client: httpx.AsyncClient, url_or_mid: str, pn=1, ps=30, order="pubdate", keyword=""):
     """
     获取up主信息
 
     :param url_or_mid:
     :param pn:
     :param ps:
     :param order:
     :param keyword:
     :param client:
     :return:
     """
     if url_or_mid.startswith("http"):
-        mid = re.findall(r"/(\d+)", url_or_mid)[0]
+        mid = _find_mid(url_or_mid)
     else:
         mid = url_or_mid
 
     params = {"mid": mid, "order": order, "ps": ps, "pn": pn, "keyword": quote(keyword or "")}
     await _add_sign(client, params)
 
     res = await req_retry(client, "https://api.bilibili.com/x/space/wbi/arc/search", params=params)
     info = json.loads(res.text)
     up_name = info["data"]["list"]["vlist"][0]["author"]
     total_size = info["data"]["page"]["count"]
     bv_ids = [i["bvid"] for i in info["data"]["list"]["vlist"]]
     return up_name, total_size, bv_ids
 
 
+async def get_up_info(client: httpx.AsyncClient, url_or_mid: str):
+    if url_or_mid.startswith("http"):
+        mid = _find_mid(url_or_mid)
+    else:
+        mid = url_or_mid
+    params = {"mid": mid}
+    await _add_sign(client, params)
+    res = await req_retry(client, "https://api.bilibili.com/x/space/wbi/acc/info", params=params)
+    data = json.loads(res.text)['data']
+    return data
+
+
 class Media(BaseModel):
     base_url: str
     backup_url: List[str] = None
     size: int = None
     width: int = None
     height: int = None
     suffix: str = None
@@ -422,7 +438,33 @@
 @raise_api_error
 async def get_dm_urls(client: httpx.AsyncClient, aid, cid) -> List[str]:
     params = {'oid': cid, 'pid': aid, 'type': 1}
     res = await req_retry(client, f'https://api.bilibili.com/x/v2/dm/web/view', params=params)
     view = parse_view(res.content)
     total = int(view['dmSge']['total'])
     return [f'https://api.bilibili.com/x/v2/dm/web/seg.so?oid={cid}&type=1&segment_index={i + 1}' for i in range(total)]
+
+
+async def get_up_album_info(client: httpx.AsyncClient, url: str) -> Tuple[Dict, List[Dict]]:
+    """todo it seems that page_size is not working, count may be incorrect"""
+    uid = re.search(r'^https://space.bilibili.com/(\d+)/?', url).group(1)
+    up_meta = asyncio.create_task(get_up_info(client, uid))
+    res = await req_retry(client, f'https://api.bilibili.com/x/dynamic/feed/draw/upload_count?uid={uid}')
+    count = json.loads(res.text)['data']['all_count']
+    sema = asyncio.Semaphore(3)
+
+    async def get_page(p: int):
+        async with sema:
+            params = {'uid': uid, 'page_num': p, 'page_size': ps, 'biz': 'all'}
+            r = await req_retry(client, 'https://api.bilibili.com/x/dynamic/feed/draw/doc_list', params=params)
+            data = json.loads(r.text)['data']['items']
+            return data
+
+    pn, ps, cur = 0, 30, 0
+    cors = []
+    while cur < count:
+        cors.append(get_page(pn))
+        pn += 1
+        cur += ps
+    lst = await asyncio.gather(*cors)
+    lst = [item for d in lst for item in d]
+    return await up_meta, lst
```

### Comparing `bilix-1.0a0/bilix/sites/bilibili/api_test.py` & `bilix-1.0a1/bilix/sites/bilibili/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     time_from, time_to = time_from.strftime('%Y%m%d'), time_to.strftime('%Y%m%d')
     meta = await api.get_cate_meta(client)
     bvids = await api.get_cate_page_info(client, cate_id=meta['宅舞']['tid'], time_from=time_from, time_to=time_to)
     assert len(bvids) > 0 and bvids[0].startswith('BV')
 
 
 @pytest.mark.asyncio
-async def test_get_up_info():
-    up_name, total_size, bvids = await api.get_up_info(client, "316568752", keyword="什么")
+async def test_get_up_video_info():
+    up_name, total_size, bvids = await api.get_up_video_info(client, "316568752", keyword="什么")
     assert len(bvids) > 0 and bvids[0].startswith('BV')
 
 
 # GitHub actions problem...
 # @pytest.mark.asyncio
 # async.md def test_get_special_audio():
 #     # Dolby
@@ -81,15 +81,15 @@
 async def test_get_video_info():
     # 单个bv视频
     data = await api.get_video_info(client, "https://www.bilibili.com/video/BV1sS4y1b7qb?spm_id_from=333.999.0.0")
     assert len(data.pages) == 1
     assert data.p == 0
     assert data.bvid
     assert data.img_url.startswith('http://') or data.img_url.startswith('https://')
-    # assert data.dash  # todo since GitHub action can not get dash, there is no dash check...
+    assert data.dash
     # 多个bv视频
     data = await api.get_video_info(client, "https://www.bilibili.com/video/BV1jK4y1N7ST?p=5")
     assert len(data.pages) > 1
     assert data.p == 4
     assert data.bvid
     # 电视剧
     data = await api.get_video_info(client, "https://www.bilibili.com/bangumi/play/ss24053?spm_id_from=333.337.0.0")
@@ -121,7 +121,21 @@
 
 @pytest.mark.asyncio
 async def test_get_dm_info():
     data = await api.get_video_info(client,
                                     "https://www.bilibili.com/bangumi/play/ss33343?theme=movie&spm_id_from=333.337.0.0")
     data = await api.get_dm_urls(client, data.aid, data.cid)
     assert len(data) > 0
+
+
+@pytest.mark.asyncio
+async def test_get_up_info():
+    data = await api.get_up_info(client, "https://space.bilibili.com/1575476")
+    assert data['name']
+    assert data['mid'] == 1575476
+
+
+@pytest.mark.asyncio
+async def test_get_up_album_info():
+    up_info, up_album_info = await api.get_up_album_info(client, "https://space.bilibili.com/1575476/album")
+    assert len(up_album_info) > 0
+    assert up_info['name']
```

### Comparing `bilix-1.0a0/bilix/sites/bilibili/downloader.py` & `bilix-1.0a1/bilix/sites/bilibili/downloader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import asyncio
 import functools
 import logging
 import re
 from enum import Enum
 from pathlib import Path
-from typing import Union, Tuple, List, Annotated
+from typing import Union, Tuple, List, Annotated, Dict, Optional
 import aiofiles
 import httpx
 from datetime import datetime, timedelta
 from . import api
 from bilix.download.base_downloader_part import BaseDownloaderPart
 from bilix._process import SingletonPPE
 from bilix.utils import legal_title, cors_slice, valid_sess_data, t2s, json2srt
 from bilix.download.utils import req_retry, path_check, parse_speed_str, str2path, parse_time_range
 from bilix.exception import APIUnsupportedError, APIResourceError, APIError
 from bilix.progress.abc import Progress
 from bilix import ffmpeg
 from danmakuC.bilibili import proto2ass
 
 
+class UpOrder(str, Enum):
+    pubdate = 'pubdate'
+    click = 'click'
+    stow = 'stow'
+
+
 def _dm2ass_factory(width: int, height: int):
     async def dm2ass(protobuf_bytes: bytes) -> bytes:
         loop = asyncio.get_event_loop()
         f = functools.partial(proto2ass, protobuf_bytes, width, height, font_size=width / 40, )
         content = await loop.run_in_executor(SingletonPPE(), f)
         return content.encode('utf-8')
 
@@ -190,15 +196,15 @@
         if not self._cate_meta:
             self._cate_meta = asyncio.ensure_future(api.get_cate_meta(self.client))
             self._cate_meta = await self._cate_meta
         elif asyncio.isfuture(self._cate_meta):
             await self._cate_meta
         return self._cate_meta
 
-    class CateOrder(Enum):
+    class CateOrder(str, Enum):
         click = 'click'
         scores = 'scores'
         stow = 'stow'
         coin = 'coin'
         dm = 'dm'
 
     async def get_cate(self, cate_name: str, path: Annotated[Path, str2path] = Path('.'),
@@ -257,19 +263,14 @@
         func = self.get_series if series else self.get_video
         # noinspection PyArgumentList
         cors = [func(f"https://www.bilibili.com/video/{i}", path=path, quality=quality, codec=codec,
                      image=image, subtitle=subtitle, dm=dm, only_audio=only_audio)
                 for i in bvids]
         await asyncio.gather(*cors)
 
-    class UpOrder(Enum):
-        pubdate = 'pubdate'
-        click = 'click'
-        stow = 'stow'
-
     async def get_up(self, url_or_mid: str, path: Annotated[Path, str2path] = Path('.'),
                      num=10, order: UpOrder = UpOrder.pubdate, keyword='', quality: Union[str, int] = 0,
                      series=True, image=False, subtitle=False, dm=False, only_audio=False, codec='', ):
         """
         下载up主视频
         :cli short: up
         :param url_or_mid: b站用户空间页面url 或b站用户id，在空间页面的url中可以找到
@@ -283,15 +284,15 @@
         :param subtitle: 是否下载字幕
         :param dm: 是否下载弹幕
         :param only_audio: 是否仅下载音频
         :param codec: 视频编码
         :return:
         """
         ps = 30
-        up_name, total_size, bv_ids = await api.get_up_info(self.client, url_or_mid, 1, ps, order, keyword)
+        up_name, total_size, bv_ids = await api.get_up_video_info(self.client, url_or_mid, 1, ps, order, keyword)
         if self.hierarchy:
             path /= legal_title(f"【up】{up_name}")
             path.mkdir(parents=True, exist_ok=True)
         num = min(total_size, num)
         page_nums = num // ps + min(1, num % ps)
         cors = []
         for i in range(page_nums):
@@ -305,15 +306,15 @@
         await asyncio.gather(*cors)
 
     async def _get_up_by_page(self, url_or_mid, path: Path,
                               pn=1, num=30, order=UpOrder.pubdate, keyword='', quality: Union[str, int] = 0,
                               series=True, image=False, subtitle=False, dm=False, only_audio=False, codec='', ):
         ps = 30
         num = min(ps, num)
-        _, _, bvids = await api.get_up_info(self.client, url_or_mid, pn, ps, order, keyword)
+        _, _, bvids = await api.get_up_video_info(self.client, url_or_mid, pn, ps, order, keyword)
         bvids = bvids[:num]
         func = self.get_series if series else self.get_video
         # noinspection PyArgumentList
         await asyncio.gather(
             *[func(f'https://www.bilibili.com/video/{bv}', path=path, quality=quality, codec=codec,
                    image=image, subtitle=subtitle, dm=dm, only_audio=only_audio) for bv in bvids])
 
@@ -395,15 +396,15 @@
                     # 1. only video
                     if not audio and not only_audio:
                         tmp.append((video, path / f'{media_name}.mp4'))
                     # 2. video and audio
                     elif audio and not only_audio:
                         exists, media_path = path_check(path / f'{media_name}.mp4')
                         if exists:
-                            self.logger.info(f'[green]已存在[/green] {media_path.name}')
+                            self.logger.exist(media_path.name)
                         else:
                             tmp.append((video, path / f'{media_name}-v'))
                             tmp.append((audio, path / f'{media_name}-a'))
                             # task need to be merged
                             await self.progress.update(task_id=task_id, upper=ffmpeg.combine)
                     # 3. only audio
                     elif audio and only_audio:
@@ -433,15 +434,15 @@
                 if len(video_info.other) == 1:
                     m = video_info.other[0]
                     media_cors.append(
                         self.get_file(m.urls, path=path / f'{media_name}.{m.suffix}', task_id=task_id))
                 else:
                     exist, media_path = path_check(path / f'{media_name}.mp4')
                     if exist:
-                        self.logger.info(f'[green]已存在[/green] {media_path.name}')
+                        self.logger.exist(media_path.name)
                     else:
                         p_sema = asyncio.Semaphore(self.part_concurrency)
 
                         async def _get_file(media: api.Media, p: Path) -> Path:
                             async with p_sema:
                                 return await self.get_file(media.urls, path=p, task_id=task_id)
 
@@ -467,15 +468,15 @@
                         width, height = 1920, 1080
                     add_cors.append(self.get_dm(
                         url, path=extra_path, convert_func=_dm2ass_factory(width, height), video_info=video_info))
             path_lst, _ = await asyncio.gather(asyncio.gather(*media_cors), asyncio.gather(*add_cors))
 
         if upper := self.progress.tasks[task_id].fields.get('upper', None):
             await upper(path_lst, media_path)
-            self.logger.info(f'[cyan]已完成[/cyan] {media_path.name}')
+            self.logger.done(media_path.name)
         await self.progress.update(task_id, visible=False)
 
     async def get_dm(self, url: str, path: Annotated[Path, str2path] = Path('.'),
                      update: bool = False, convert_func=_dm2ass_factory(1920, 1080), video_info: api.VideoInfo = None):
         """
         下载视频的弹幕
         :cli short: dm
@@ -495,26 +496,26 @@
         if len(video_info.h1_title) > self.title_overflow and self.hierarchy and p_name:
             file_name = legal_title(p_name, "弹幕") + file_type
         else:
             file_name = legal_title(video_info.h1_title, p_name, "弹幕") + file_type
         file_path = path / file_name
         exist, file_path = path_check(file_path)
         if not update and exist:
-            self.logger.info(f"[green]已存在[/green] {file_name}")
+            self.logger.exist(file_name)
             return file_path
         dm_urls = await api.get_dm_urls(self.client, aid, cid)
         cors = [req_retry(self.client, dm_url) for dm_url in dm_urls]
         results = await asyncio.gather(*cors)
         content = b''.join(res.content for res in results)
         content = convert_func(content) if convert_func else content
         if asyncio.iscoroutine(content):
             content = await content
         async with aiofiles.open(file_path, 'wb') as f:
             await f.write(content)
-        self.logger.info(f"[cyan]已完成[/cyan] {file_name}")
+        self.logger.done(file_name)
         return file_path
 
     async def get_subtitle(self, url: str, path: Annotated[Path, str2path] = Path('.'),
                            convert_func=json2srt, video_info: api.VideoInfo = None):
         """
         下载视频的字幕文件
         :cli short: sub
@@ -539,10 +540,83 @@
                 file_name = legal_title(p_name, sub_name)
             else:
                 file_name = legal_title(video_info.h1_title, p_name, sub_name)
             cors.append(self.get_static(sub_url, path / file_name, convert_func=convert_func))
         paths = await asyncio.gather(*cors)
         return paths
 
+    async def get_up_album(self, url: str, path: Annotated[Path, str2path] = Path('.'),
+                           p_range: Tuple[int, int] = None,
+                           name_fmt: str = '【相簿】{up_name}/{ctime}-{doc_id}/'
+                           ):
+        """
+        下载up主的相簿
+        :cli short: upa
+        :param url: b站用户空间页面url
+        :param path: 保存路径
+        :param p_range: 下载范围，从0开始计数，左闭右开
+        :param name_fmt: 命名格式（以/分割层级），此层级支持的变量有：up_name
+        :return:
+        """
+        async with self.api_sema:
+            up_info, up_album_info = await api.get_up_album_info(self.client, url)
+        if p_range:
+            start, end = p_range
+            up_album_info = up_album_info[start: end]
+        if self.hierarchy:
+            up_name = legal_title(up_info['name'])
+            if name_fmt:
+                fmt, name_fmt = name_fmt.split('/', 1)
+                name = fmt.format(up_name=up_name)
+            else:
+                name = up_name
+            path = path / name
+            path.mkdir(parents=True, exist_ok=True)
+        await asyncio.gather(*[
+            self._get_album(album_info, path=path, name_fmt=name_fmt) for album_info in up_album_info
+        ])
+
+    async def _get_album(self, album_info: Dict, path: Annotated[Path, str2path] = Path('.'),
+                         name_fmt: str = '{ctime}-{doc_id}/'):
+        """
+        下载某个相簿
+        :param album_info:
+        :param path:
+        :param name_fmt: 命名格式，命名格式，此层级支持的变量有：ctime, doc_id
+        :return:
+        """
+        name_d = {
+            'ctime': datetime.fromtimestamp(album_info['ctime']).strftime('%Y-%m-%d'),
+            'doc_id': album_info['doc_id']
+        }
+        if name_fmt:
+            fmt, name_fmt = name_fmt.split('/', 1)
+            name = fmt.format(**name_d)
+        else:
+            name = '{ctime}-{doc_id}'.format(**name_d)
+        if self.hierarchy:
+            path = path / name
+            path.mkdir(parents=True, exist_ok=True)
+        cors = []
+        part_sema = asyncio.Semaphore(self.part_concurrency)
+
+        async def get_static(u, p):
+            async with part_sema:
+                await self.get_static(url=u, path=p, task_id=task_id)
+
+        task_id = await self.progress.add_task(description=name, visible=False)
+        for pic in album_info['pictures']:
+            file_name = pic['img_src'].rsplit('/', 1)[-1].split('.', 1)[0]
+            cors.append(get_static(pic['img_src'], path / file_name))
+        async with self.v_sema:
+            lst = await asyncio.gather(*cors, return_exceptions=True)
+        downloaded_paths = []
+        for res in lst:
+            if not isinstance(res, Exception):
+                downloaded_paths.append(res)
+        await self.progress.update(task_id, visible=False)
+        self.logger.done(name)
+        return downloaded_paths
+
     @classmethod
     def decide_handle(cls, method_name: str, keys: Tuple[str, ...]):
         return method_name in {'cate', 'get_cate'} or super().decide_handle(method_name, keys)
```

### Comparing `bilix-1.0a0/bilix/sites/bilibili/downloader_test.py` & `bilix-1.0a1/bilix/sites/bilibili/downloader_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,7 +78,14 @@
     data.dash.choose_quality(quality="360P", codec="hev")
     # hi-res
     data = await api.get_video_info(client, "https://www.bilibili.com/video/BV16K411S7sk")
     try:
         video, audio = data.dash.choose_quality(quality='1080P', codec="hev:fLaC")
     except KeyError:
         assert not os.getenv("BILI_TOKEN")
+
+
+@pytest.mark.asyncio
+async def test_get_up_album():
+    d = DownloaderBilibili()
+    await d.get_up_album("https://space.bilibili.com/233962606")
+    await d.aclose()
```

### Comparing `bilix-1.0a0/bilix/sites/bilibili/informer.py` & `bilix-1.0a1/bilix/sites/bilibili/informer.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,16 +24,16 @@
         :cli short: info
         :param key: 资源url，当前仅支持视频url
         :return:
         """
         await self.parse_url(key)(self, key)
 
     async def info_up(self, url: str):
-        up_name, total_size, bvids = await api.get_up_info(self.client, url)
-        rprint(up_name)
+        up_info = await api.get_up_info(self.client, url)
+        rprint(up_info)
 
     async def info_favour(self, url: str):
         pass
 
     async def info_collect_or_list(self, url: str):
         pass
```

### Comparing `bilix-1.0a0/bilix/sites/cctv/api.py` & `bilix-1.0a1/bilix/sites/cctv/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/cctv/downloader.py` & `bilix-1.0a1/bilix/sites/cctv/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/douyin/api.py` & `bilix-1.0a1/bilix/sites/douyin/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/douyin/downloader.py` & `bilix-1.0a1/bilix/sites/douyin/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/hanime1/api.py` & `bilix-1.0a1/bilix/sites/hanime1/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/hanime1/downloader.py` & `bilix-1.0a1/bilix/sites/hanime1/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/jable/api.py` & `bilix-1.0a1/bilix/sites/jable/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/jable/api_test.py` & `bilix-1.0a1/bilix/sites/jable/api_test.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/jable/downloader.py` & `bilix-1.0a1/bilix/sites/jable/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/tiktok/api.py` & `bilix-1.0a1/bilix/sites/tiktok/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/tiktok/downloader.py` & `bilix-1.0a1/bilix/sites/tiktok/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/yhdmp/api.py` & `bilix-1.0a1/bilix/sites/yhdmp/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/yhdmp/downloader.py` & `bilix-1.0a1/bilix/sites/yhdmp/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/yhdmp/yhdmp.js` & `bilix-1.0a1/bilix/sites/yhdmp/yhdmp.js`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/yinghuacd/api.py` & `bilix-1.0a1/bilix/sites/yinghuacd/api.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/bilix/sites/yinghuacd/downloader.py` & `bilix-1.0a1/bilix/sites/yinghuacd/downloader.py`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/LICENSE` & `bilix-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/README.md` & `bilix-1.0a1/README.md`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/pyproject.toml` & `bilix-1.0a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bilix-1.0a0/PKG-INFO` & `bilix-1.0a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bilix
-Version: 1.0a0
+Version: 1.0a1
 Summary: ⚡️Lightning-fast asynchronous download tool for bilibili and more
 Project-URL: Homepage, https://github.com/HFrost0/bilix
 Author-email: HFrost0 <hhlfrost@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
```

