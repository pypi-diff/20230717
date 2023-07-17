# Comparing `tmp/balcony-0.1.6.tar.gz` & `tmp/balcony-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balcony-0.1.6.tar", max compression
+gzip compressed data, was "balcony-0.1.7.tar", max compression
```

## Comparing `balcony-0.1.6.tar` & `balcony-0.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.6/LICENSE
--rw-r--r--   0        0        0     3621 2023-06-27 21:55:30.541972 balcony-0.1.6/README.md
--rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.6/balcony/__init__.py
--rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.6/balcony/__main__.py
--rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.6/balcony/aws.py
--rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.6/balcony/botocore_utils.py
--rw-r--r--   0        0        0    22612 2023-07-16 15:42:35.736562 balcony-0.1.6/balcony/cli.py
--rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.6/balcony/config.py
--rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.6/balcony/custom_nodes/__init__.py
--rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.6/balcony/custom_nodes/codebuild.py
--rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.6/balcony/custom_nodes/ecs.py
--rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.6/balcony/custom_nodes/iam.py
--rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.6/balcony/custom_nodes/lambda_functions.py
--rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.6/balcony/custom_nodes/s3.py
--rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.6/balcony/custom_nodes/ses.py
--rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.6/balcony/custom_nodes/ssm.py
--rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.6/balcony/custom_tf_import_configs/_example_import_conf.yaml
--rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.6/balcony/custom_tf_import_configs/ec2.yaml
--rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.6/balcony/custom_tf_import_configs/ecs.yaml
--rw-r--r--   0        0        0     1897 2023-07-16 10:50:18.867726 balcony-0.1.6/balcony/custom_tf_import_configs/iam.yaml
--rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.6/balcony/custom_tf_import_configs/rds.yaml
--rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.6/balcony/custom_tf_import_configs/s3.yaml
--rw-r--r--   0        0        0     3388 2023-07-16 17:09:09.656301 balcony-0.1.6/balcony/custom_tf_import_configs/vpc.yaml
--rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.6/balcony/custom_yamls/_example_service.yaml
--rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.6/balcony/custom_yamls/ec2.yaml
--rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.6/balcony/custom_yamls/ecs.yaml
--rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.6/balcony/custom_yamls/iam.yaml
--rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.6/balcony/custom_yamls/s3.yaml
--rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.6/balcony/errors.py
--rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.6/balcony/nodes.py
--rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.6/balcony/reader.py
--rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.6/balcony/registries.py
--rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.6/balcony/relations.py
--rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.6/balcony/terraform_import/__init__.py
--rw-r--r--   0        0        0     9506 2023-07-16 17:10:19.590346 balcony-0.1.6/balcony/terraform_import/importer.py
--rw-r--r--   0        0        0     1262 2023-06-23 11:28:38.779925 balcony-0.1.6/balcony/terraform_import/models.py
--rw-r--r--   0        0        0     3666 2023-07-16 16:00:20.534235 balcony-0.1.6/balcony/terraform_import/parsers.py
--rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.6/balcony/terraform_import/wizard.py
--rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.6/balcony/test.py
--rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.6/balcony/utils.py
--rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.6/balcony/yaml_config.py
--rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.6/balcony/yaml_validators.py
--rw-r--r--   0        0        0      748 2023-07-16 17:17:23.467052 balcony-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 balcony-0.1.6/setup.py
--rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 balcony-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-26 12:31:10.748997 balcony-0.1.7/LICENSE
+-rw-r--r--   0        0        0     3621 2023-06-27 21:55:30.541972 balcony-0.1.7/README.md
+-rw-r--r--   0        0        0      933 2023-04-29 21:23:00.565222 balcony-0.1.7/balcony/__init__.py
+-rw-r--r--   0        0        0       52 2023-04-09 17:39:37.780212 balcony-0.1.7/balcony/__main__.py
+-rw-r--r--   0        0        0     5622 2023-04-21 19:12:44.411429 balcony-0.1.7/balcony/aws.py
+-rw-r--r--   0        0        0    15169 2023-06-27 10:41:54.525900 balcony-0.1.7/balcony/botocore_utils.py
+-rw-r--r--   0        0        0    22612 2023-07-17 18:22:23.044112 balcony-0.1.7/balcony/cli.py
+-rw-r--r--   0        0        0     3723 2023-06-27 12:34:24.543878 balcony-0.1.7/balcony/config.py
+-rw-r--r--   0        0        0      488 2023-04-29 22:03:44.770391 balcony-0.1.7/balcony/custom_nodes/__init__.py
+-rw-r--r--   0        0        0      540 2023-04-09 17:41:34.066674 balcony-0.1.7/balcony/custom_nodes/codebuild.py
+-rw-r--r--   0        0        0     4856 2023-04-07 12:10:50.547169 balcony-0.1.7/balcony/custom_nodes/ecs.py
+-rw-r--r--   0        0        0     7305 2023-04-09 17:41:50.509945 balcony-0.1.7/balcony/custom_nodes/iam.py
+-rw-r--r--   0        0        0      728 2023-04-07 12:11:06.485573 balcony-0.1.7/balcony/custom_nodes/lambda_functions.py
+-rw-r--r--   0        0        0     1086 2023-04-09 17:41:59.998051 balcony-0.1.7/balcony/custom_nodes/s3.py
+-rw-r--r--   0        0        0      632 2023-04-09 17:42:05.685496 balcony-0.1.7/balcony/custom_nodes/ses.py
+-rw-r--r--   0        0        0     1320 2023-04-09 17:42:11.817275 balcony-0.1.7/balcony/custom_nodes/ssm.py
+-rw-r--r--   0        0        0        0 2023-06-18 18:05:04.079497 balcony-0.1.7/balcony/custom_tf_import_configs/_example_import_conf.yaml
+-rw-r--r--   0        0        0     2306 2023-07-16 15:42:11.020304 balcony-0.1.7/balcony/custom_tf_import_configs/ec2.yaml
+-rw-r--r--   0        0        0      312 2023-06-27 00:04:18.331870 balcony-0.1.7/balcony/custom_tf_import_configs/ecs.yaml
+-rw-r--r--   0        0        0     1610 2023-07-17 18:20:28.021261 balcony-0.1.7/balcony/custom_tf_import_configs/iam.yaml
+-rw-r--r--   0        0        0     1845 2023-06-27 20:18:18.446771 balcony-0.1.7/balcony/custom_tf_import_configs/rds.yaml
+-rw-r--r--   0        0        0      336 2023-06-22 11:23:28.065064 balcony-0.1.7/balcony/custom_tf_import_configs/s3.yaml
+-rw-r--r--   0        0        0     4257 2023-07-17 18:18:53.104515 balcony-0.1.7/balcony/custom_tf_import_configs/vpc.yaml
+-rw-r--r--   0        0        0     3149 2023-04-15 19:49:24.900287 balcony-0.1.7/balcony/custom_yamls/_example_service.yaml
+-rw-r--r--   0        0        0      842 2023-07-16 11:53:29.831094 balcony-0.1.7/balcony/custom_yamls/ec2.yaml
+-rw-r--r--   0        0        0        0 2023-04-05 13:32:52.449913 balcony-0.1.7/balcony/custom_yamls/ecs.yaml
+-rw-r--r--   0        0        0     1501 2023-04-15 17:54:11.807061 balcony-0.1.7/balcony/custom_yamls/iam.yaml
+-rw-r--r--   0        0        0      313 2023-04-15 18:00:26.309547 balcony-0.1.7/balcony/custom_yamls/s3.yaml
+-rw-r--r--   0        0        0      418 2023-04-09 17:40:20.070136 balcony-0.1.7/balcony/errors.py
+-rw-r--r--   0        0        0    48806 2023-06-26 21:17:28.989726 balcony-0.1.7/balcony/nodes.py
+-rw-r--r--   0        0        0    17448 2023-06-27 11:52:38.036399 balcony-0.1.7/balcony/reader.py
+-rw-r--r--   0        0        0     3226 2023-04-15 19:59:07.673952 balcony-0.1.7/balcony/registries.py
+-rw-r--r--   0        0        0    13165 2023-04-09 17:39:54.863685 balcony-0.1.7/balcony/relations.py
+-rw-r--r--   0        0        0        0 2023-06-18 17:41:34.879852 balcony-0.1.7/balcony/terraform_import/__init__.py
+-rw-r--r--   0        0        0    10693 2023-07-17 17:11:29.424367 balcony-0.1.7/balcony/terraform_import/importer.py
+-rw-r--r--   0        0        0     1320 2023-07-17 16:45:25.594486 balcony-0.1.7/balcony/terraform_import/models.py
+-rw-r--r--   0        0        0     3877 2023-07-17 16:46:47.909479 balcony-0.1.7/balcony/terraform_import/parsers.py
+-rw-r--r--   0        0        0    16069 2023-06-27 13:47:03.229109 balcony-0.1.7/balcony/terraform_import/wizard.py
+-rw-r--r--   0        0        0     2980 2023-06-19 18:24:25.368221 balcony-0.1.7/balcony/test.py
+-rw-r--r--   0        0        0     6553 2023-07-07 16:07:51.678302 balcony-0.1.7/balcony/utils.py
+-rw-r--r--   0        0        0     2171 2023-06-27 11:55:23.845723 balcony-0.1.7/balcony/yaml_config.py
+-rw-r--r--   0        0        0     2049 2023-06-18 17:05:58.939803 balcony-0.1.7/balcony/yaml_validators.py
+-rw-r--r--   0        0        0      748 2023-07-17 18:31:02.099122 balcony-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     4911 1970-01-01 00:00:00.000000 balcony-0.1.7/setup.py
+-rw-r--r--   0        0        0     4727 1970-01-01 00:00:00.000000 balcony-0.1.7/PKG-INFO
```

### Comparing `balcony-0.1.6/LICENSE` & `balcony-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/README.md` & `balcony-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/__init__.py` & `balcony-0.1.7/balcony/__init__.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/aws.py` & `balcony-0.1.7/balcony/aws.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/botocore_utils.py` & `balcony-0.1.7/balcony/botocore_utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/cli.py` & `balcony-0.1.7/balcony/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,21 +429,21 @@
             "[underline][yellow bold][WARNING][/] [bold][--paginate, -p][/] option [bold red]is NOT set[/]. You're likely to get incomplete data.[/]"
         )
 
     if list_available_resources:
         service_resource_list = get_importable_resources()
 
         def render_importable_resources(service_and_resource_tuples: List[Tuple]):
-            header = f"[bold green]{'TerraformResourceType':<30} {'Service':>15} {'Resource':45}[/]\n".format()
+            header = f"[bold green]{'TerraformResourceType':<50} {'Service':>15} {'Resource':45}[/]\n".format()
             result = header
 
             for i, (terraform_type, service_name, resource_name) in enumerate(
                 service_and_resource_tuples
             ):
-                cur_line = f"{terraform_type:<30} {service_name:>15} {resource_name:45}"
+                cur_line = f"{terraform_type:<50} {service_name:>15} {resource_name:45}"
                 if i % 2:
                     cur_line = f"[bold]{cur_line}[/]"
                 result += cur_line + "\n"
             return result
 
         rendered_service_resource_list = render_importable_resources(
             service_resource_list
```

### Comparing `balcony-0.1.6/balcony/config.py` & `balcony-0.1.7/balcony/config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/codebuild.py` & `balcony-0.1.7/balcony/custom_nodes/codebuild.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/ecs.py` & `balcony-0.1.7/balcony/custom_nodes/ecs.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/iam.py` & `balcony-0.1.7/balcony/custom_nodes/iam.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/lambda_functions.py` & `balcony-0.1.7/balcony/custom_nodes/lambda_functions.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/s3.py` & `balcony-0.1.7/balcony/custom_nodes/s3.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/ses.py` & `balcony-0.1.7/balcony/custom_nodes/ses.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_nodes/ssm.py` & `balcony-0.1.7/balcony/custom_nodes/ssm.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_tf_import_configs/ec2.yaml` & `balcony-0.1.7/balcony/custom_tf_import_configs/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_tf_import_configs/iam.yaml` & `balcony-0.1.7/balcony/custom_tf_import_configs/iam.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -38,23 +38,16 @@
   jmespath_query: '[].Roles[]'
   operation_name: ListRoles
   resource_node: Role
   service: iam
   to_resource_name_jinja2_template: '{{ ''role-'' ~ RoleName }}'
   to_resource_type: aws_iam_role
 
-- id_generator_jinja2_template: '{{ GroupName ~ '':'' ~ PolicyName }}'
-  jmespath_query: '[]'
-  operation_name: GetGroupPolicy
-  resource_node: GroupPolicy
-  service: iam
-  to_resource_name_jinja2_template: '{{ GroupName ~ ''-'' ~ PolicyName }}'
-  to_resource_type: aws_iam_group_policy
-
 - id_generator_jinja2_template: '{{ UserName ~ '':''  ~ PolicyName }}'
   jmespath_query: '[]'
   operation_name: GetUserPolicy
   resource_node: UserPolicy
   service: iam
   to_resource_name_jinja2_template: '{{ UserName ~ ''-'' ~ PolicyName }}'
   to_resource_type: aws_iam_user_policy
 
+
```

### Comparing `balcony-0.1.6/balcony/custom_tf_import_configs/rds.yaml` & `balcony-0.1.7/balcony/custom_tf_import_configs/rds.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_yamls/_example_service.yaml` & `balcony-0.1.7/balcony/custom_yamls/_example_service.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_yamls/ec2.yaml` & `balcony-0.1.7/balcony/custom_yamls/ec2.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/custom_yamls/iam.yaml` & `balcony-0.1.7/balcony/custom_yamls/iam.yaml`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/nodes.py` & `balcony-0.1.7/balcony/nodes.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/reader.py` & `balcony-0.1.7/balcony/reader.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/registries.py` & `balcony-0.1.7/balcony/registries.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/relations.py` & `balcony-0.1.7/balcony/relations.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/terraform_import/importer.py` & `balcony-0.1.7/balcony/terraform_import/importer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 import re
 import textwrap
 from typing import Dict, List, Tuple, Union
 import jmespath
 from terraform_import.models import TerraformImportConfig
-from terraform_import.parsers import parse_custom_terraform_import_configs_from_files, _TERRAFORM_TYPES_KEY
+from terraform_import.parsers import (
+    parse_custom_terraform_import_configs_from_files,
+    _TERRAFORM_TYPES_KEY,
+)
 from config import get_logger
 from aws import BalconyAWS
 from jinja2 import Environment
 
 logger = get_logger(__name__)
+# cache for read & parsed custom terraform import configuration .yml files
 _terraform_import_configurations = None
 
 
 def get_custom_terraform_import_config_dict() -> Dict:
     global _terraform_import_configurations
     if _terraform_import_configurations:
         return _terraform_import_configurations
 
-    _terraform_import_configurations = parse_custom_terraform_import_configs_from_files()
+    _terraform_import_configurations = (
+        parse_custom_terraform_import_configs_from_files()
+    )
     return _terraform_import_configurations
 
 
 def extract_resource_tags_as_kwargs(data: dict) -> dict:
     tags_as_kwargs = {}
     tag_list = data.get("Tags", [])
     if not tag_list or not isinstance(tag_list, list):
@@ -42,66 +48,87 @@
         kwargs = data.copy()
         kwargs["data"] = data
         # if there's add it as tag_Name variable
         tags_as_kwargs = extract_resource_tags_as_kwargs(data)
         kwargs.update(tags_as_kwargs)
         rendered_output = template.render(**kwargs).strip()
         result.append(rendered_output)
+    # if the data is a list, render the template for each item
     elif isinstance(data, list):
-        # if the data is a list, render the template for each item
-        kwargs = {"data": data}
+        kwargs = {}
         for an_item in data:
+            kwargs["data"] = an_item
             kwargs["item"] = an_item
             rendered_output = template.render(**kwargs).strip()
-            rendered_list = [_.strip() for _ in rendered_output.split(' ') if _]
+            rendered_list = [_.strip() for _ in rendered_output.split(" ") if _]
             result.extend(rendered_list)
     elif isinstance(data, str):
         kwargs = {
             "item": data,
             "data": data,
         }
         rendered_output = template.render(**kwargs).strip()
         result.append(rendered_output)
     return result
 
 
 def gen_resource_name_and_import_id_from_op_data_(
-    operation_data, jmespath_query, to_resource_name_tpl, id_generator_tpl
+    operation_data,
+    jmespath_query,
+    to_resource_name_tpl,
+    id_generator_tpl,
+    multiline_output=False,
 ):
     result = []
-    is_basic_j2_template = '{%' not in to_resource_name_tpl.lstrip()
-    if jmespath_query and is_basic_j2_template:
+
+    resource_data = operation_data
+
+    if not multiline_output:
+        # NON MULTILINE OUTPUT
         # filter the operation data if jmespath_query is given
         # and render them one by one
-        list_of_resource_data = jmespath.search(jmespath_query, operation_data)
-        logger.debug(f"Filtered data using jmespath query: {jmespath_query}")
+        if jmespath_query:
+            resource_data = jmespath.search(jmespath_query, operation_data)
+            logger.debug(
+                f"Filtered data using jmespath query: [bold]{jmespath_query}[/]"
+            )
 
-        for a_resource_data in list_of_resource_data:
+        for a_resource_data in resource_data:
             resource_name_list = render_jinja2_template_with_data(
                 a_resource_data, to_resource_name_tpl
             )
             import_id_list = render_jinja2_template_with_data(
                 a_resource_data, id_generator_tpl
             )
             result.extend(list(zip(resource_name_list, import_id_list)))
-
         return result
     else:
+        # MULTILINE OUTPUT
         # no jmespath query given, use the whole operation data
         # assumes there's multiple lines of output from the template
 
+        if jmespath_query:
+            resource_data = jmespath.search(jmespath_query, operation_data)
+            logger.debug(
+                f"Filtered data using jmespath query: [bold]{jmespath_query}[/]"
+            )
+
         multiline_resource_name_list = render_jinja2_template_with_data(
-            operation_data, to_resource_name_tpl
+            resource_data, to_resource_name_tpl
         )
         multiline_import_id_list = render_jinja2_template_with_data(
-            operation_data, id_generator_tpl
+            resource_data, id_generator_tpl
         )
-        # split them on newlines
 
-        assert len(multiline_resource_name_list) == len(multiline_import_id_list)
+        if len(multiline_resource_name_list) != len(multiline_import_id_list):
+            logger.debug(
+                f"[red bold]Error: multiline output lists are not equal length. {multiline_resource_name_list=} -- {multiline_import_id_list=}"
+            )
+            return []
+
         r = list(zip(multiline_resource_name_list, multiline_import_id_list))
         return r
 
 
 def generate_terraform_import_block(to_resource_type, to_resource_name, import_id):
     jinja_tmpl = textwrap.dedent(
         """
@@ -128,16 +155,18 @@
     importable_services_and_resources = []
     for service_name, resource_config_dict in custom_tf_config_dict.items():
         if service_name == _TERRAFORM_TYPES_KEY:
             continue  # skip the _terraform_types cache key
         for resource_node_name, resource_config_list in resource_config_dict.items():
             for resource_config in resource_config_list:
                 terraform_resource_type = resource_config.to_resource_type
-                importable_services_and_resources.append((terraform_resource_type, service_name, resource_node_name))
-    return list(sorted(importable_services_and_resources, key=lambda x: x[1]+x[2]))
+                importable_services_and_resources.append(
+                    (terraform_resource_type, service_name, resource_node_name)
+                )
+    return list(sorted(importable_services_and_resources, key=lambda x: x[1] + x[2]))
 
 
 def sanitize_resource_name_and_import_ids(list_of_tuples):
     result = []
     for resource_name, import_id in list_of_tuples:
         # change anything that's not a letter, number, dash or underscore to underscore
         sanitized_resource_name = re.sub(r"[^A-Za-z0-9\-_]", "_", resource_name)
@@ -157,27 +186,27 @@
 
     if service and resource_node:
         config_for_resource_node = custom_tf_config_dict.get(service, {}).get(
             resource_node, []
         )
         return config_for_resource_node
     elif terraform_resource_type:
-        config_list_for_tf_type = custom_tf_config_dict.get(_TERRAFORM_TYPES_KEY, {}).get(
-            terraform_resource_type, False
-        )
+        config_list_for_tf_type = custom_tf_config_dict.get(
+            _TERRAFORM_TYPES_KEY, {}
+        ).get(terraform_resource_type, False)
         if not config_list_for_tf_type:
             return False
         return config_list_for_tf_type
     return False
 
 
 def generate_import_block_from_import_config(
     balcony_client: BalconyAWS,
     tf_import_config: TerraformImportConfig,
-    follow_pagination: bool = False
+    follow_pagination: bool = False,
 ) -> List[str]:
     tf_import_blocks: List[str] = []
 
     operation_name = tf_import_config.operation_name
     service = tf_import_config.service
     resource_node = tf_import_config.resource_node
     jmespath_query = tf_import_config.jmespath_query
@@ -201,14 +230,15 @@
         return False
 
     resource_name_and_import_ids = gen_resource_name_and_import_id_from_op_data_(
         operation_data,
         jmespath_query,
         tf_import_config.to_resource_name_jinja2_template,
         tf_import_config.id_generator_jinja2_template,
+        multiline_output=tf_import_config.multiline_output,
     )
 
     # Replace unsupported chars from the to-resource-name with underscore
     sanitized_resource_name_and_import_ids = sanitize_resource_name_and_import_ids(
         resource_name_and_import_ids
     )
 
@@ -220,33 +250,41 @@
         tf_import_block = generate_terraform_import_block(
             tf_import_config.to_resource_type, to_resource_name, import_id
         )
         tf_import_blocks.append(tf_import_block)
     return tf_import_blocks
 
 
-
 def generate_import_block_for_resource(
     balcony_client: BalconyAWS,
     service: str = None,
     resource_node: str = None,
     terraform_resource_type: str = None,
     follow_pagination: bool = False,
 ):
+    operation_markup = f"[bold][green]{service}[/].[blue]{resource_node}[/][/]"
+    if (not service or not resource_node) and terraform_resource_type:
+        operation_markup = f"[bold cyan]{terraform_resource_type}[/]"
+
+    logger.debug(f"[underline bold][green]Starting to Generate[/] Terraform import blocks for[/] {operation_markup}.")
     resulting_tf_import_blocks = []
-    tf_import_configs = get_import_config_for(service, resource_node, terraform_resource_type)
+    tf_import_configs = get_import_config_for(
+        service, resource_node, terraform_resource_type
+    )
     if not tf_import_configs:
         logger.debug(
             f"[red bold]No custom terraform import config found for {service}.{resource_node}. Please check out docs https://oguzhan-yilmaz.github.io/balcony/ for more info on developing it your own."
         )
         return False
 
     for tf_import_config in tf_import_configs:
-        tf_import_blocks = generate_import_block_from_import_config(balcony_client, tf_import_config, follow_pagination)
+        tf_import_blocks = generate_import_block_from_import_config(
+            balcony_client, tf_import_config, follow_pagination
+        )
         if not tf_import_blocks:
             logger.debug(
                 f"[red bold]No data found for {tf_import_config.to_resource_type} — {tf_import_config.resource_node}.{tf_import_config.operation_name}."
             )
-            return False
         resulting_tf_import_blocks.extend(tf_import_blocks)
-        
-    return resulting_tf_import_blocks
+    
+    logger.debug(f"[underline bold][green]Done Generating[/] Terraform import blocks for[/] {operation_markup}.")
+    return resulting_tf_import_blocks
```

### Comparing `balcony-0.1.6/balcony/terraform_import/models.py` & `balcony-0.1.7/balcony/terraform_import/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-from typing import List, Dict, Optional, Any
-from pydantic import BaseModel, validator
+from typing import List, Optional
+from pydantic import BaseModel  # , validator
 
 
 class TerraformImportConfig(BaseModel):
     service: str  # ec2
     resource_node: str  # Instances
     operation_name: str  # DescribeInstances
     jmespath_query: Optional[str]  # Reservations[].Instances[]
     to_resource_type: str  # aws_instance
-    to_resource_name_jinja2_template: str  # "{{ .InstanceId }}"
-    id_generator_jinja2_template: str  # "{{ .InstanceId }}"
-
-    @validator("to_resource_name_jinja2_template")
-    def validate_to_resource_name_jinja2_template(cls, value):
-        # Add your validation logic here
-        # You can raise a ValueError if the value is invalid
-        return value
-
-    @validator("id_generator_jinja2_template")
-    def validate_id_generator_jinja2_template(cls, value):
-        # Add your validation logic here
-        # You can raise a ValueError if the value is invalid
-        return value
+    to_resource_name_jinja2_template: str  # "{{ InstanceId }}"
+    id_generator_jinja2_template: str
+    multiline_output: Optional[bool]
+
+    # TODO: code the validators
+    # @validator("to_resource_name_jinja2_template")
+    # def validate_to_resource_name_jinja2_template(cls, value):
+    #     # Add your validation logic here
+    #     # You can raise a ValueError if the value is invalid
+    #     return value
+
+    # @validator("id_generator_jinja2_template")
+    # def validate_id_generator_jinja2_template(cls, value):
+    #     # Add your validation logic here
+    #     # You can raise a ValueError if the value is invalid
+    #     return value
 
 
 class MaintainersBlock(BaseModel):
     """List of maintainers for the terraform import config file."""
 
     name: str
     github: Optional[str]
```

### Comparing `balcony-0.1.6/balcony/terraform_import/parsers.py` & `balcony-0.1.7/balcony/terraform_import/parsers.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 from config import (
     get_logger,
     YAML_TF_IMPORT_CONFIGS_DIRECTORY,
     USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY,
 )
 from terraform_import.models import (
     CustomTerraformImportConfigFile,
-    TerraformImportConfig,
+    # TerraformImportConfig,
 )
 from typing import Union, Tuple
 import yaml
 from collections import defaultdict
 
 logger = get_logger(__name__)
-_TERRAFORM_TYPES_KEY='_terraform_types'
+_TERRAFORM_TYPES_KEY = "_terraform_types"
 
 
 def parse_json_to_tf_import_config(
     input_configuration_dict: str,
 ) -> Union[bool, CustomTerraformImportConfigFile]:
     try:
         return CustomTerraformImportConfigFile(**input_configuration_dict)
@@ -45,16 +45,21 @@
     except Exception as e:
         return False, e
 
 
 def parse_custom_terraform_import_configs_from_files():
     terraform_configurations_dict = defaultdict(lambda: defaultdict(dict))
 
-    parse_directories = [YAML_TF_IMPORT_CONFIGS_DIRECTORY,] # noqa
-    _are_same_directories = USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY == YAML_TF_IMPORT_CONFIGS_DIRECTORY.as_posix()
+    parse_directories = [
+        YAML_TF_IMPORT_CONFIGS_DIRECTORY,
+    ]  # noqa
+    _are_same_directories = (
+        USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY
+        == YAML_TF_IMPORT_CONFIGS_DIRECTORY.as_posix()
+    )
     if USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY and not _are_same_directories:
         # might not be defined
         parse_directories.append(USER_DEFINED_YAML_TF_IMPORT_CONFIGS_DIRECTORY)
 
     for yaml_directory in parse_directories:
         config_filenames = find_all_yaml_files(yaml_directory)
         logger.debug(
@@ -64,23 +69,31 @@
         for conf_filename in config_filenames:
             conf, error = parse_yaml_file_to_tf_import_config(conf_filename)
             if error:
                 logger.error(f"Error while parsing {conf_filename}: {error}")
                 continue
             for tf_config in conf.import_configurations:
                 # doing it this way allows overrides from the user defined configs
-                r_node = terraform_configurations_dict.get(tf_config.service, {}).get(tf_config.resource_node, False)
+                r_node = terraform_configurations_dict.get(tf_config.service, {}).get(
+                    tf_config.resource_node, False
+                )
                 if r_node is False:
                     terraform_configurations_dict[tf_config.service][
                         tf_config.resource_node
                     ] = [tf_config]
                 else:
                     terraform_configurations_dict[tf_config.service][
                         tf_config.resource_node
                     ].append(tf_config)
                 # add it to _TERRAFORM_TYPES_KEY
-                tf_conf_list = terraform_configurations_dict[_TERRAFORM_TYPES_KEY].get(tf_config.to_resource_type, [])
+                tf_conf_list = terraform_configurations_dict[_TERRAFORM_TYPES_KEY].get(
+                    tf_config.to_resource_type, []
+                )
                 if not tf_conf_list:
-                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][tf_config.to_resource_type] = [tf_config]
+                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][
+                        tf_config.to_resource_type
+                    ] = [tf_config]
                 else:
-                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][tf_config.to_resource_type].append(tf_config)
+                    terraform_configurations_dict[_TERRAFORM_TYPES_KEY][
+                        tf_config.to_resource_type
+                    ].append(tf_config)
     return terraform_configurations_dict
```

### Comparing `balcony-0.1.6/balcony/terraform_import/wizard.py` & `balcony-0.1.7/balcony/terraform_import/wizard.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/test.py` & `balcony-0.1.7/balcony/test.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/utils.py` & `balcony-0.1.7/balcony/utils.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/yaml_config.py` & `balcony-0.1.7/balcony/yaml_config.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/balcony/yaml_validators.py` & `balcony-0.1.7/balcony/yaml_validators.py`

 * *Files identical despite different names*

### Comparing `balcony-0.1.6/pyproject.toml` & `balcony-0.1.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "balcony"
-version = "0.1.6"
+version = "0.1.7"
 description = "Read any resource in your AWS Account. You can generate terraform code for them, too."
 authors = ["Oguzhan Yilmaz <oguzhanylmz271@gmail.com>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.scripts]
 balcony = "balcony.cli:run_app"
```

### Comparing `balcony-0.1.6/setup.py` & `balcony-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'typer>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']}
 
 setup_kwargs = {
     'name': 'balcony',
-    'version': '0.1.6',
+    'version': '0.1.7',
     'description': 'Read any resource in your AWS Account. You can generate terraform code for them, too.',
     'long_description': '# balcony\n\n\n<div style="display: flex;">\n  <a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/docker-publish.yml/badge.svg" alt="Build and publish a Docker image to ghcr.io"></a>\n  <span style="width: 5px"></span>\n\n<a href="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment"><img src="https://github.com/oguzhan-yilmaz/balcony/actions/workflows/pages/pages-build-deployment/badge.svg" alt="Build and Deploy Documentation website"></a>\n</div>\n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-fill the required parameters for AWS API calls \n- Read the JSON data of any AWS resource in your account\n- Generate [Terraform Import Blocks](https://developer.hashicorp.com/terraform/language/import)\n- Generate actual `.tf` Terraform Resource code\n\nbalcony uses _read-only_ operations, it does not take any action on the used AWS account.\n\n\n### [Visit the Documentation Website](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n<!-- ### [**Go to QuickStart Page to get started using _balcony_**](quickstart.md) -->\n\n### Installation\n\n```bash\npip3 install balcony\n```\n\nVisit [**Installation & QuickStart Page**](https://oguzhan-yilmaz.github.io/balcony/quickstart/) to get started using _balcony_\n\n```bash  title="Basic usage"\n# see options\nbalcony\n\n# list available resources of ec2\nbalcony aws ec2 \n\n# read a resource\nbalcony aws s3 Buckets\n\n# generate terraform import blocks for a resource\nbalcony terraform-import s3 Buckets\n```\n\n\n## Features\n\n### Read any AWS Resource\nRelated Docs: [QuickStart](https://oguzhan-yilmaz.github.io/balcony/quickstart/)\n\n\n![](visuals/reading-a-resource-node.gif)\n\n---\n\n### Generate Terraform Import Blocks\n\nTerraform v1.5 introduced [import blocks](https://developer.hashicorp.com/terraform/language/import) that allows users to define their imports as code.\n\n`balcony terraform-import <service> <resource-name>` command generates these import blocks for you.\n\n`balcony terraform-import --list` to see the list of supported resources.\n\nRelated Docs: [Generate Terraform Import Blocks](https://oguzhan-yilmaz.github.io/balcony/terraform-import/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-import-blocks-example.gif)\n\n\n---\n\n### Generate actual Terraform Resource Code \n\nIf you have:\n\n- initialized terraform project\n- `import_blocks.tf` file that\'s generated with `balcony terraform-import` command\n\nyou can run `terraform plan -generate-config-out=generated.tf` to generate actual `.tf` resource code.\n\nThis feature is achieved with a Docker image.\n\nRelated Docs: [Generate Terraform Code with Docker Image](https://oguzhan-yilmaz.github.io/balcony/terraform-import-docker/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/docker-gen-tf-code-ec2-insances-example.gif)\n\n\n---\n\n### Interactive Wizard to create balcony import configurations \n\nBalcony doesn\'t know how to create terraform `import blocks` for all of the AWS resources.\n\nIt can be taught how to do it by creating `import-configurations` yaml files, but it\'s a manual process. This is where the interactive wizard comes in.\n\nInteractive Wizards asks you required questions to automatically create the `import-configurations` yaml files.\n\nRelated Docs: [Terraform Import Configuration Wizard](https://oguzhan-yilmaz.github.io/balcony/terraform-import-wizard/)\n\n![](https://raw.githubusercontent.com/oguzhan-yilmaz/balcony-assets/main/gifs/terraform-wizard-security-groups-example.gif)\n',
     'author': 'Oguzhan Yilmaz',
     'author_email': 'oguzhanylmz271@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 ['*'], 'balcony': ['custom_tf_import_configs/*', 'custom_yamls/*']}
 install_requires = \ ['Jinja2>=3.1.2,<4.0.0', 'PyYAML>=6.0,<7.0',
 'boto3>=1.24.80,<2.0.0', 'inflect>=6.0.0,<7.0.0', 'jmespath>=1.0.1,<2.0.0',
 'mkdocs-autorefs>=0.4.1,<0.5.0', 'mkdocs-material>=8.5.7,<10.0.0',
 'mkdocstrings[python]>=0.21.2,<0.22.0', 'pydantic>=1.10.7,<2.0.0',
 'rich>=13.3.4,<14.0.0', 'typer>=0.7.0,<0.8.0'] entry_points = \
 {'console_scripts': ['balcony = balcony.cli:run_app']} setup_kwargs = { 'name':
-'balcony', 'version': '0.1.6', 'description': 'Read any resource in your AWS
+'balcony', 'version': '0.1.7', 'description': 'Read any resource in your AWS
 Account. You can generate terraform code for them, too.', 'long_description':
 '# balcony\n\n\n
 \n [Build_and_publish_a_Docker_image_to_ghcr.io]\n \n\n[Build_and_Deploy
 Documentation_website]\n
 \n\n\nbalcony is a modern CLI tool that with some killer features:\n\n- Auto-
 fill the required parameters for AWS API calls \n- Read the JSON data of any
 AWS resource in your account\n- Generate [Terraform Import Blocks](https://
```

### Comparing `balcony-0.1.6/PKG-INFO` & `balcony-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balcony
-Version: 0.1.6
+Version: 0.1.7
 Summary: Read any resource in your AWS Account. You can generate terraform code for them, too.
 License: GPL-3.0-or-later
 Author: Oguzhan Yilmaz
 Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: balcony Version: 0.1.6 Summary: Read any resource
+Metadata-Version: 2.1 Name: balcony Version: 0.1.7 Summary: Read any resource
 in your AWS Account. You can generate terraform code for them, too. License:
 GPL-3.0-or-later Author: Oguzhan Yilmaz Author-email: oguzhanylmz271@gmail.com
 Requires-Python: >=3.7,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Requires-Dist: Jinja2
```

