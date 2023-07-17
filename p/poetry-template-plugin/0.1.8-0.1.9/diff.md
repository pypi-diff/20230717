# Comparing `tmp/poetry_template_plugin-0.1.8.tar.gz` & `tmp/poetry_template_plugin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_template_plugin-0.1.8.tar", max compression
+gzip compressed data, was "poetry_template_plugin-0.1.9.tar", max compression
```

## Comparing `poetry_template_plugin-0.1.8.tar` & `poetry_template_plugin-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2022-11-15 08:54:24.474790 poetry_template_plugin-0.1.8/README.md
--rw-r--r--   0        0        0    24068 2023-03-17 20:33:33.549125 poetry_template_plugin-0.1.8/poetry_template_plugin/plugin.py
--rw-r--r--   0        0        0      752 2023-03-17 20:33:12.427925 poetry_template_plugin-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 poetry_template_plugin-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-11-15 08:54:24.474790 poetry_template_plugin-0.1.9/README.md
+-rw-r--r--   0        0        0    25770 2023-07-16 18:48:53.162600 poetry_template_plugin-0.1.9/poetry_template_plugin/plugin.py
+-rw-r--r--   0        0        0      752 2023-07-16 18:05:47.199591 poetry_template_plugin-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      464 1970-01-01 00:00:00.000000 poetry_template_plugin-0.1.9/PKG-INFO
```

### Comparing `poetry_template_plugin-0.1.8/poetry_template_plugin/plugin.py` & `poetry_template_plugin-0.1.9/poetry_template_plugin/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import os
 import pickle
 import re
 import shutil
 import stat
 import subprocess
 import tempfile
+import textwrap
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Match, Tuple
 
 import merge3
 import tomlkit
 from cleo.application import Application
@@ -29,14 +30,15 @@
 
 
 class TemplateState:
     files: Dict[Path, FileState]
     repository: str
     questions: Dict[str, Any]
     context: Dict[str, Any]
+    log_id: str | None = None
 
     def __init__(self, repository: str, context: Dict[str, Any]):
         self.repository = repository
         self.files = {}
         self.questions = {}
         self.context = context
 
@@ -94,31 +96,62 @@
         if conflict:
             color = "red"
         self.print(f"<fg={color}>{icon}  {path} {extra}</>")
 
 
 class TemplateCommand(TemplateBaseCommand):
     def handle_command(self, state: TemplateState, target_dir: Path) -> None:
+        logs = self.get_logs(state)
+        files = self.get_files(state)
+
+        if not target_dir.exists():
+            os.makedirs(target_dir)
+        os.chdir(target_dir)
+
+        new_logs = []
+        for rec in logs:
+            if rec[0] == state.log_id:
+                break
+            new_logs.append(rec)
+
+        self.handle_files(state, files, new_logs)
+        self.done()
+
+    def get_files(self, state) -> Dict[Path, "File"]:
         tmp_dir = tempfile.mkdtemp()
+        cwd = os.getcwd()
         try:
             subprocess.check_output(
                 ["git", "clone", "--depth=1", f"ssh://{state.repository}", tmp_dir],
                 stderr=subprocess.DEVNULL,
             )
             os.chdir(tmp_dir)
             files = self.init_template(state)
         finally:
+            os.chdir(cwd)
             shutil.rmtree(tmp_dir)
+        return files
 
-        if not target_dir.exists():
-            os.makedirs(target_dir)
-        os.chdir(target_dir)
-
-        self.handle_files(state, files)
-        self.done()
+    def get_logs(self, state: TemplateState) -> List[Tuple[str, str, str, str]]:
+        tmp_dir = tempfile.mkdtemp()
+        cwd = os.getcwd()
+        try:
+            subprocess.check_output(
+                ["git", "clone", "--bare", f"ssh://{state.repository}", tmp_dir],
+                stderr=subprocess.DEVNULL,
+            )
+            os.chdir(tmp_dir)
+            result = subprocess.check_output(
+                ["git", "--no-pager", "log", '--pretty=%H#%an#%aI#%s'],
+                stderr=subprocess.DEVNULL,
+            ).decode("utf-8")
+        finally:
+            os.chdir(cwd)
+            shutil.rmtree(tmp_dir)
+        return [tuple(x.split('#', 3)) for x in result.splitlines()]
 
     def init_template(self, state: TemplateState) -> Dict[Path, "File"]:
         files = {
             p: {"flag": "protected", "readonly": True}
             for p in Path(".").glob("**/*")
             if not p.is_relative_to(".git") and not p.is_dir()
         }
@@ -149,15 +182,15 @@
             else:
                 content = path.read_bytes()
             mode = path.stat().st_mode & (stat.S_IXUSR | stat.S_IXGRP | stat.S_IXOTH)
             path = (path.parent / path.name[1:]) if (path.name.startswith("@") or path.name.startswith("#")) else path
             result[path] = FILES.get(path.suffix, File)(state.files.setdefault(path, {}), path, options, mode, content)
         return result
 
-    def handle_files(self, state: TemplateState, files: Dict[Path, "File"]) -> None:
+    def handle_files(self, state: TemplateState, files: Dict[Path, "File"], logs: List[Tuple[str, str, str, str]]) -> None:
         raise NotImplementedError()
 
     def done(self) -> None:
         self.print("\u2728 Done!")
 
     def walk_template_files(
         self, files: Dict[Path, Dict[str, Any]], patterns: List[str] | str, fn: Callable[[Dict[Path, Any], Path], Any]
@@ -229,18 +262,19 @@
         target = Path(os.getcwd()) / self.argument("target")
         if target.exists() and not target.is_dir():
             raise RuntimeError(f"File {target} exists.")
         if any(target.glob("*")):
             raise RuntimeError(f"Target directory {target} is not empty.")
         return target
 
-    def handle_files(self, state: TemplateState, files: Dict[Path, "File"]) -> None:
+    def handle_files(self, state: TemplateState, files: Dict[Path, "File"], logs: List[Tuple[str, str, str, str]]) -> None:
         self.print("\U0001f680 Init template...")
         for file in files.values():
             self.write_file(file)
+        state.log_id = logs[0][0]
 
     def done(self) -> None:
         self.call("update")
         super().done()
 
 
 class TemplateUpdateCommand(TemplateCommand):
@@ -287,19 +321,24 @@
             self.print("<fg=yellow>\u2757 There are unresolved conflicts:</>")
             for path, meta in conflicts:
                 self.print_file(path, **meta)
             self.print("")
             self.print("<fg=yellow>\u2757 Resolve conflicts and tag files using `poetry template fix`</>")
             raise RuntimeError("Cancelled")
 
-    def handle_files(self, state: TemplateState, files: Dict[Path, "File"]) -> None:
+    def handle_files(self, state: TemplateState, files: Dict[Path, "File"], logs: List[Tuple[str, str, str, str]]) -> None:
         self.print("\U0001f680 Start update...")
         self.print("")
         self.check_conflicts(state)
 
+        for rec in logs:
+            self.print(f"<fg=magenta>{rec[1]} <fg=yellow>{rec[2]}</></>:")
+            self.print(f"{textwrap.indent(rec[3], '  ')}")
+            self.print("")
+
         remove: List[Path] = []
         write: List[File] = []
 
         for what, file in self.get_update_files(state, files):
             if what == "delete":
                 self.print(f"<fg=yellow>\u2757 [-] <fg=magenta>{file}</> will be deleted</>")
                 assert isinstance(file, Path)
@@ -339,31 +378,39 @@
                 path = p.parent
                 while path != Path(".") and not any(path.glob("*")):
                     path.rmdir()
                     path = path.parent
                 state.files.pop(p)
             self.print("")
 
+        state.log_id = logs[0][0]
+
     def done(self) -> None:
         if self.option("update"):
             self.call("update")
         super().done()
 
 
 class TemplateIncomingCommand(TemplateUpdateCommand):
     dump_state = False
     name = "template incoming"
     description = "Show incoming changes."
     arguments = []
     options = []
 
-    def handle_files(self, state: TemplateState, files: Dict[Path, "File"]) -> None:
+    def handle_files(self, state: TemplateState, files: Dict[Path, "File"], logs: List[Tuple[str, str, str, str]]) -> None:
         self.print("\U0001f680 Check incoming updates...")
         self.print("")
         self.check_conflicts(state)
+
+        for rec in logs:
+            self.print(f"<fg=magenta>{rec[1]} <fg=yellow>{rec[2]}</></>:")
+            self.print(f"{textwrap.indent(rec[3], '  ')}")
+            self.print("")
+
         for what, file in self.get_update_files(state, files):
             if what == "delete":
                 self.print(f"<fg=yellow>\u2757 [-] <fg=magenta>{file}</> will be deleted</>")
                 self.print("=" * 79)
                 continue
             assert isinstance(file, File)
             if what == "create":
```

### Comparing `poetry_template_plugin-0.1.8/pyproject.toml` & `poetry_template_plugin-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-template-plugin"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["aachurin <aachurin@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 poetry = "^1.2"
```

