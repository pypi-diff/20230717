# Comparing `tmp/snapctl-0.2.5.tar.gz` & `tmp/snapctl-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.2.5.tar", max compression
+gzip compressed data, was "snapctl-0.2.6.tar", max compression
```

## Comparing `snapctl-0.2.5.tar` & `snapctl-0.2.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.5/README.md
--rw-r--r--   0        0        0      399 2023-07-17 05:05:15.425994 snapctl-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.5/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.5/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.5/snapctl/commands/__init__.py
--rw-r--r--   0        0        0     8993 2023-07-17 05:04:59.590853 snapctl-0.2.5/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.5/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.5/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.5/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.5/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.5/snapctl/utils/echo.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0      971 2023-07-17 16:26:27.384137 snapctl-0.2.6/README.md
+-rw-r--r--   0        0        0      399 2023-07-17 15:31:21.284704 snapctl-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-17 15:14:31.467451 snapctl-0.2.6/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.6/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.6/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     8886 2023-07-17 14:24:47.287813 snapctl-0.2.6/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1575 2023-07-17 16:24:55.892589 snapctl-0.2.6/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.6/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.6/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.6/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.6/snapctl/utils/echo.py
+-rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 snapctl-0.2.6/PKG-INFO
```

### Comparing `snapctl-0.2.5/snapctl/commands/byosnap.py` & `snapctl-0.2.6/snapctl/commands/byosnap.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,15 +103,14 @@
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         else:
           response = subprocess.run([
             f'echo "{ecr_repo_token}" | docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to connect to the Snapser Container Repository. Please get the latest token from the Web app.')
-          error(f'docker login --username {ecr_repo_username} --password {ecr_repo_token} {ecr_repo_url}')
           return False
       success('Login Successful')
 
       # Build your snap
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
```

### Comparing `snapctl-0.2.5/snapctl/main.py` & `snapctl-0.2.6/snapctl/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 import typer
 
 from snapctl.commands.byosnap import ByoSnap
 from snapctl.types.definitions import ResponseType
 from snapctl.utils.echo import error, success, info
 
+__version__ = '0.2.6'
+
 app = typer.Typer()
 
-# Commands
+def version_callback(value: bool = True):
+  if value:
+    typer.echo(f"Snapctl version: {__version__}")
+    raise typer.Exit()
+
 @app.callback()
-def callback():
-  """
-  Snapser CLI Tool
-  """
+def common(
+    ctx: typer.Context,
+    version: bool = typer.Option(
+      None, "--version",
+      help="Get the Snapctl version.",
+      callback=version_callback
+    ),
+):
+    pass
 
 # command: Optional[str] = typer.Argument(None)
 @app.command()
 def byosnap(
   command: str = typer.Argument(..., help="BYOSnap Commands: " + ", ".join(ByoSnap.COMMANDS) + "."),
   path: str = typer.Argument(..., help="Path to your snap code"),
   tag: str = typer.Argument(..., help="Tag for your snap"),
```

