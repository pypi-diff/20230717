# Comparing `tmp/aws_securityhub_suppression-0.3.1.tar.gz` & `tmp/aws_securityhub_suppression-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws_securityhub_suppression-0.3.1.tar", max compression
+gzip compressed data, was "aws_securityhub_suppression-0.3.2.tar", max compression
```

## Comparing `aws_securityhub_suppression-0.3.1.tar` & `aws_securityhub_suppression-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      836 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/README.md
--rw-r--r--   0        0        0     1453 2023-07-14 18:51:48.883242 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/__init__.py
--rw-r--r--   0        0        0      948 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/account.py
--rw-r--r--   0        0        0      515 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/check.py
--rw-r--r--   0        0        0      970 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/prepare.py
--rw-r--r--   0        0        0     1583 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/update.py
--rw-r--r--   0        0        0      793 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/context.py
--rw-r--r--   0        0        0      744 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/handler.py
--rw-r--r--   0        0        0     1133 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/documentation_generator.py
--rw-r--r--   0        0        0     1303 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/finding.py
--rw-r--r--   0        0        0      830 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/__init__.py
--rw-r--r--   0        0        0      793 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/environment.yaml
--rw-r--r--   0        0        0      158 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/workload.yaml
--rw-r--r--   0        0        0     1307 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppress_findings.py
--rw-r--r--   0        0        0      759 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppression.py
--rw-r--r--   0        0        0      561 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload.py
--rw-r--r--   0        0        0     2011 2023-07-14 18:51:48.147229 aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload_generator.py
--rw-r--r--   0        0        0     1220 2023-07-14 18:51:48.883242 aws_securityhub_suppression-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      836 2023-07-17 09:47:19.089617 aws_securityhub_suppression-0.3.2/README.md
+-rw-r--r--   0        0        0     1450 2023-07-17 09:47:20.009625 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-17 09:47:19.089617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/account.py
+-rw-r--r--   0        0        0      515 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/check.py
+-rw-r--r--   0        0        0      970 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/prepare.py
+-rw-r--r--   0        0        0     1615 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/update.py
+-rw-r--r--   0        0        0      793 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/context.py
+-rw-r--r--   0        0        0      744 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/handler.py
+-rw-r--r--   0        0        0     1133 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/documentation_generator.py
+-rw-r--r--   0        0        0     1303 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/finding.py
+-rw-r--r--   0        0        0      830 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/schemas/__init__.py
+-rw-r--r--   0        0        0      793 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/schemas/environment.yaml
+-rw-r--r--   0        0        0      158 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/schemas/workload.yaml
+-rw-r--r--   0        0        0     1307 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/suppress_findings.py
+-rw-r--r--   0        0        0      759 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/suppression.py
+-rw-r--r--   0        0        0     1855 2023-07-17 09:47:19.093617 aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/workload_generator.py
+-rw-r--r--   0        0        0     1220 2023-07-17 09:47:20.009625 aws_securityhub_suppression-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1561 1970-01-01 00:00:00.000000 aws_securityhub_suppression-0.3.2/PKG-INFO
```

### Comparing `aws_securityhub_suppression-0.3.1/README.md` & `aws_securityhub_suppression-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/__init__.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from typing import List, Optional
 import glob
 import os
+from landingzone_organization.workload import Workload
 from aws_securityhub_suppression.account import Account
 from aws_securityhub_suppression.schemas import (
     WorkloadSchema,
     EnvironmentSchema,
     safe_load_file,
 )
-from aws_securityhub_suppression.workload import Workload
 from aws_securityhub_suppression.suppression import Suppression
 from aws_securityhub_suppression.finding import Finding
 
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 
 def load_workloads(workload_path: str) -> List[Workload]:
     workloads = glob.glob(os.path.join(workload_path, "**/info.yaml"), recursive=True)
 
     def load_workload(file: str) -> Optional[Workload]:
         return load_workload_by_file(file)
```

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/account.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/account.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/__init__.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/check.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/check.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/prepare.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/prepare.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/commands/update.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/commands/update.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 def cli() -> None:
     """
     Execute the suppression script
     """
     pass
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.pass_obj
 @click.argument("config-path")
 def suppression(ctx: Context, config_path: str) -> None:
     """
     Suppress all registered findings for all workloads
     """
     ctx.info("Suppress all registered findings for all workloads")
@@ -29,15 +29,15 @@
     for workload in workloads:
         click.echo(f"\tWorkload: {workload.name}")
         SuppressFindings(
             client=ctx.session.client("securityhub"), workload=workload
         ).execute()
 
 
-@cli.command()
+@cli.command()  # type: ignore
 @click.pass_obj
 @click.argument("template-path")
 @click.argument("config-path")
 def docs(ctx: Context, template_path: str, config_path: str) -> None:
     """
     Generate suppression documentation for all workloads
     """
```

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/context.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/context.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/cli/handler.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/cli/handler.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/documentation_generator.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/documentation_generator.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/finding.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/finding.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/__init__.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/schemas/environment.yaml` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/schemas/environment.yaml`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppress_findings.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/suppress_findings.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/suppression.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/suppression.py`

 * *Files identical despite different names*

### Comparing `aws_securityhub_suppression-0.3.1/aws_securityhub_suppression/workload_generator.py` & `aws_securityhub_suppression-0.3.2/aws_securityhub_suppression/workload_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,26 +17,22 @@
     def __ensure_folder(path: str) -> None:
         if not os.path.isdir(path):
             os.mkdir(path)
 
     def __resolve_workload_info(self, file: str) -> dict:
         info = {
             "Name": self.__workload.name,
-            "Environments": list(
-                map(lambda account: account.environment, self.__workload.accounts)
-            ),
+            "Environments": self.__workload.environments,
         }
 
         if os.path.isfile(file):
             with open(file, "r") as fh:
                 info = yaml.safe_load(fh)
                 info["Name"] = self.__workload.name
-                info["Environments"] = list(
-                    map(lambda account: account.environment, self.__workload.accounts)
-                )
+                info["Environments"] = self.__workload.environments
 
         return info
 
     @staticmethod
     def __resolve_account_info(account: Account) -> dict:
         return {
             "Name": account.name,
```

### Comparing `aws_securityhub_suppression-0.3.1/pyproject.toml` & `aws_securityhub_suppression-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aws-securityhub-suppression"
-version = "0.3.1"
+version = "0.3.2"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aws_securityhub_suppression"}]
 
 [tool.poetry.group.dev.dependencies]
@@ -23,15 +23,15 @@
 branch = "main"
 upload_to_pypi = true
 upload_to_release = true
 build_command = "pip install poetry && poetry build"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-landingzone-organization = "^0.4.0"
+landingzone-organization = "^0.6.3"
 click = "^8.1.3"
 pyyaml = "^6.0"
 jinja2 = "^3.1.2"
 xenon = "^0.9.0"
 jsonschema = "^4.18.3"
```

### Comparing `aws_securityhub_suppression-0.3.1/PKG-INFO` & `aws_securityhub_suppression-0.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: aws-securityhub-suppression
-Version: 0.3.1
+Version: 0.3.2
 Summary: 
 License: MIT
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.18.3,<5.0.0)
-Requires-Dist: landingzone-organization (>=0.4.0,<0.5.0)
+Requires-Dist: landingzone-organization (>=0.6.3,<0.7.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: xenon (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
 
 # AWS SecurityHub - Suppression
 
 [![Maintenance](https://img.shields.io/badge/Maintained-yes-green.svg)](https://github.com/Nr18/aws-securityhub-suppression/graphs/commit-activity)
```

