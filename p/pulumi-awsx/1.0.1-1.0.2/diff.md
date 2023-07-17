# Comparing `tmp/pulumi_awsx-1.0.1.tar.gz` & `tmp/pulumi_awsx-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_awsx-1.0.1.tar", last modified: Thu Dec  8 15:31:58 2022, max compression
+gzip compressed data, was "pulumi_awsx-1.0.2.tar", last modified: Tue Feb  7 11:34:30 2023, max compression
```

## Comparing `pulumi_awsx-1.0.1.tar` & `pulumi_awsx-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.420420 pulumi_awsx-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2022-12-08 15:31:58.420420 pulumi_awsx-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.412420 pulumi_awsx-1.0.1/pulumi_awsx/
--rw-------   0 runner    (1001) docker     (123)     2193 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/__init__.py
--rw-------   0 runner    (1001) docker     (123)     7642 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.416420 pulumi_awsx-1.0.1/pulumi_awsx/awsx/
--rw-------   0 runner    (1001) docker     (123)      223 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/awsx/__init__.py
--rw-------   0 runner    (1001) docker     (123)    56292 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/awsx/_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.416420 pulumi_awsx-1.0.1/pulumi_awsx/cloudtrail/
--rw-------   0 runner    (1001) docker     (123)      265 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/cloudtrail/__init__.py
--rw-------   0 runner    (1001) docker     (123)    23442 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/cloudtrail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.416420 pulumi_awsx-1.0.1/pulumi_awsx/ec2/
--rw-------   0 runner    (1001) docker     (123)      366 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/__init__.py
--rw-------   0 runner    (1001) docker     (123)     1345 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/_enums.py
--rw-------   0 runner    (1001) docker     (123)    30936 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/_inputs.py
--rw-------   0 runner    (1001) docker     (123)     3890 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/default_vpc.py
--rw-------   0 runner    (1001) docker     (123)     3017 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/get_default_vpc.py
--rw-------   0 runner    (1001) docker     (123)    36064 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ec2/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.416420 pulumi_awsx-1.0.1/pulumi_awsx/ecr/
--rw-------   0 runner    (1001) docker     (123)      336 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecr/__init__.py
--rw-------   0 runner    (1001) docker     (123)      521 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecr/_enums.py
--rw-------   0 runner    (1001) docker     (123)     7566 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecr/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    12944 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecr/image.py
--rw-------   0 runner    (1001) docker     (123)    14482 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecr/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.420420 pulumi_awsx-1.0.1/pulumi_awsx/ecs/
--rw-------   0 runner    (1001) docker     (123)      399 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/__init__.py
--rw-------   0 runner    (1001) docker     (123)    84791 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    41699 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/ec2_service.py
--rw-------   0 runner    (1001) docker     (123)    31315 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/ec2_task_definition.py
--rw-------   0 runner    (1001) docker     (123)    40415 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/fargate_service.py
--rw-------   0 runner    (1001) docker     (123)    30218 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/ecs/fargate_task_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.420420 pulumi_awsx-1.0.1/pulumi_awsx/lb/
--rw-------   0 runner    (1001) docker     (123)      384 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/lb/__init__.py
--rw-------   0 runner    (1001) docker     (123)    87068 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/lb/_inputs.py
--rw-------   0 runner    (1001) docker     (123)    34637 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/lb/application_load_balancer.py
--rw-------   0 runner    (1001) docker     (123)    32049 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/lb/network_load_balancer.py
--rw-------   0 runner    (1001) docker     (123)    11164 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/lb/target_group_attachment.py
--rw-------   0 runner    (1001) docker     (123)     2770 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/provider.py
--rw-------   0 runner    (1001) docker     (123)       41 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/pulumi_awsx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-08 15:31:58.416420 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-08 15:31:58.000000 pulumi_awsx-1.0.1/pulumi_awsx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-08 15:31:58.420420 pulumi_awsx-1.0.1/setup.cfg
--rw-------   0 runner    (1001) docker     (123)     2145 2022-12-08 15:31:57.000000 pulumi_awsx-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx/
+-rw-------   0 runner    (1001) docker     (123)     2193 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     7642 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx/awsx/
+-rw-------   0 runner    (1001) docker     (123)      223 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    56292 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/awsx/_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/
+-rw-------   0 runner    (1001) docker     (123)      265 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    23442 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/ec2/
+-rw-------   0 runner    (1001) docker     (123)      366 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/__init__.py
+-rw-------   0 runner    (1001) docker     (123)     1345 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/_enums.py
+-rw-------   0 runner    (1001) docker     (123)    30936 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)     3890 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/default_vpc.py
+-rw-------   0 runner    (1001) docker     (123)     3017 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/get_default_vpc.py
+-rw-------   0 runner    (1001) docker     (123)    36064 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ec2/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.831109 pulumi_awsx-1.0.2/pulumi_awsx/ecr/
+-rw-------   0 runner    (1001) docker     (123)      336 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/__init__.py
+-rw-------   0 runner    (1001) docker     (123)      521 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/_enums.py
+-rw-------   0 runner    (1001) docker     (123)     7566 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    12944 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/image.py
+-rw-------   0 runner    (1001) docker     (123)    14482 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecr/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.835109 pulumi_awsx-1.0.2/pulumi_awsx/ecs/
+-rw-------   0 runner    (1001) docker     (123)      399 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    84791 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    41699 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_service.py
+-rw-------   0 runner    (1001) docker     (123)    31315 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_task_definition.py
+-rw-------   0 runner    (1001) docker     (123)    40415 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_service.py
+-rw-------   0 runner    (1001) docker     (123)    30218 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_task_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.835109 pulumi_awsx-1.0.2/pulumi_awsx/lb/
+-rw-------   0 runner    (1001) docker     (123)      384 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/__init__.py
+-rw-------   0 runner    (1001) docker     (123)    87068 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/_inputs.py
+-rw-------   0 runner    (1001) docker     (123)    34637 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/application_load_balancer.py
+-rw-------   0 runner    (1001) docker     (123)    32049 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/network_load_balancer.py
+-rw-------   0 runner    (1001) docker     (123)    11164 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/lb/target_group_attachment.py
+-rw-------   0 runner    (1001) docker     (123)     2770 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/provider.py
+-rw-------   0 runner    (1001) docker     (123)       41 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:34:30.827108 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7137 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/pulumi_awsx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 11:34:30.839109 pulumi_awsx-1.0.2/setup.cfg
+-rw-------   0 runner    (1001) docker     (123)     2145 2023-02-07 11:34:30.000000 pulumi_awsx-1.0.2/setup.py
```

### Comparing `pulumi_awsx-1.0.1/PKG-INFO` & `pulumi_awsx-1.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
@@ -89,14 +89,19 @@
         Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
         
         1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
         2. Refactor to replace the classic components with the new top-level components.
         
         **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
         
+        ### Notable changes
+        
+        - Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+        - Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
+        
         ## References
         
         * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
         * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
         * [Examples](./examples)
         * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_awsx Version: 1.0.1 Summary: Pulumi Amazon
+Metadata-Version: 2.1 Name: pulumi_awsx Version: 1.0.2 Summary: Pulumi Amazon
 Web Services (AWS) AWSX Components. Home-page: https://pulumi.com License:
 Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/
 workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions) [!
 [Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://
 slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
 %40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx) [![Python
@@ -64,13 +64,20 @@
 only supported components in TypeScript. All the existing components from the
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
-require additional code changes and resource re-creation. ## References *
-[Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/) * [API Reference
-Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/) *
-[Examples](./examples) * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/
-guides/crosswalk/aws/) Keywords: pulumi aws awsx kind/component category/cloud
-Platform: UNKNOWN Description-Content-Type: text/markdown
+require additional code changes and resource re-creation. ### Notable changes -
+Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
+ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
+because other components depended on the concrete VPC component class. The new
+components in v1 no longer have hard dependencies on other resources, so
+instead the subnets from the existing VPC can be passed into other components
+directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
+aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
+packages/awsx/api-docs/) * [Examples](./examples) * [Crosswalk for AWS Guide]
+(https://www.pulumi.com/docs/guides/crosswalk/aws/) Keywords: pulumi aws awsx
+kind/component category/cloud Platform: UNKNOWN Description-Content-Type: text/
+markdown
```

### Comparing `pulumi_awsx-1.0.1/README.md` & `pulumi_awsx-1.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -82,13 +82,18 @@
 Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
 
 1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
 2. Refactor to replace the classic components with the new top-level components.
 
 **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
 
+### Notable changes
+
+- Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+- Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
+
 ## References
 
 * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
 * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
 * [Examples](./examples)
 * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

#### html2text {}

```diff
@@ -60,12 +60,18 @@
 only supported components in TypeScript. All the existing components from the
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
-require additional code changes and resource re-creation. ## References *
-[Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/) * [API Reference
-Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/) *
-[Examples](./examples) * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/
-guides/crosswalk/aws/)
+require additional code changes and resource re-creation. ### Notable changes -
+Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
+ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
+because other components depended on the concrete VPC component class. The new
+components in v1 no longer have hard dependencies on other resources, so
+instead the subnets from the existing VPC can be passed into other components
+directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
+aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
+packages/awsx/api-docs/) * [Examples](./examples) * [Crosswalk for AWS Guide]
+(https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/__init__.py` & `pulumi_awsx-1.0.2/pulumi_awsx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/_utilities.py` & `pulumi_awsx-1.0.2/pulumi_awsx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/awsx/_inputs.py` & `pulumi_awsx-1.0.2/pulumi_awsx/awsx/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/cloudtrail/trail.py` & `pulumi_awsx-1.0.2/pulumi_awsx/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ec2/_enums.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ec2/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ec2/_inputs.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ec2/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ec2/default_vpc.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ec2/default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ec2/get_default_vpc.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ec2/get_default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ec2/vpc.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecr/_enums.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecr/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecr/_inputs.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecr/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecr/image.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecr/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecr/repository.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecs/_inputs.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecs/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecs/ec2_service.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecs/ec2_task_definition.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecs/ec2_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecs/fargate_service.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/ecs/fargate_task_definition.py` & `pulumi_awsx-1.0.2/pulumi_awsx/ecs/fargate_task_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/lb/_inputs.py` & `pulumi_awsx-1.0.2/pulumi_awsx/lb/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/lb/application_load_balancer.py` & `pulumi_awsx-1.0.2/pulumi_awsx/lb/application_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/lb/network_load_balancer.py` & `pulumi_awsx-1.0.2/pulumi_awsx/lb/network_load_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/lb/target_group_attachment.py` & `pulumi_awsx-1.0.2/pulumi_awsx/lb/target_group_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx/provider.py` & `pulumi_awsx-1.0.2/pulumi_awsx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx.egg-info/PKG-INFO` & `pulumi_awsx-1.0.2/pulumi_awsx.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-awsx
-Version: 1.0.1
+Version: 1.0.2
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 Home-page: https://pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions)
         [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
         [![NPM version](https://badge.fury.io/js/%40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx)
@@ -89,14 +89,19 @@
         Before version 1, this package only supported components in TypeScript. All the existing components from the 0.x releases are now available in the `classic` namespace. The `classic` namespace will remain until the next major version release but will only receive updates for critical security fixes.
         
         1. Change references from `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour.
         2. Refactor to replace the classic components with the new top-level components.
         
         **Note:** The new top-level components (outside the `classic` namespace) may require additional code changes and resource re-creation.
         
+        ### Notable changes
+        
+        - Removed ECS Cluster as this did not add any functionaly over the [AWS Classic ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/ecs/cluster/).
+        - Removed `Vpc.fromExistingIds()` as this was originally added because other components depended on the concrete VPC component class. The new components in v1 no longer have hard dependencies on other resources, so instead the subnets from the existing VPC can be passed into other components directly.
+        
         ## References
         
         * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/)
         * [API Reference Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/)
         * [Examples](./examples)
         * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/guides/crosswalk/aws/)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi-awsx Version: 1.0.1 Summary: Pulumi Amazon
+Metadata-Version: 2.1 Name: pulumi-awsx Version: 1.0.2 Summary: Pulumi Amazon
 Web Services (AWS) AWSX Components. Home-page: https://pulumi.com License:
 Apache-2.0 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Description: [![Actions Status](https://github.com/pulumi/pulumi-awsx/
 workflows/master/badge.svg)](https://github.com/pulumi/pulumi-awsx/actions) [!
 [Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://
 slack.pulumi.com) [![NPM version](https://badge.fury.io/js/
 %40pulumi%2Fawsx.svg)](https://www.npmjs.com/package/@pulumi/awsx) [![Python
@@ -64,13 +64,20 @@
 only supported components in TypeScript. All the existing components from the
 0.x releases are now available in the `classic` namespace. The `classic`
 namespace will remain until the next major version release but will only
 receive updates for critical security fixes. 1. Change references from
 `@pulumi/awsx` to `@pulumi/awsx/classic` to maintain existing behaviour. 2.
 Refactor to replace the classic components with the new top-level components.
 **Note:** The new top-level components (outside the `classic` namespace) may
-require additional code changes and resource re-creation. ## References *
-[Tutorial](https://www.pulumi.com/blog/crosswalk-for-aws-1-0/) * [API Reference
-Documentation](https://www.pulumi.com/registry/packages/awsx/api-docs/) *
-[Examples](./examples) * [Crosswalk for AWS Guide](https://www.pulumi.com/docs/
-guides/crosswalk/aws/) Keywords: pulumi aws awsx kind/component category/cloud
-Platform: UNKNOWN Description-Content-Type: text/markdown
+require additional code changes and resource re-creation. ### Notable changes -
+Removed ECS Cluster as this did not add any functionaly over the [AWS Classic
+ECS Cluster resource](https://www.pulumi.com/registry/packages/aws/api-docs/
+ecs/cluster/). - Removed `Vpc.fromExistingIds()` as this was originally added
+because other components depended on the concrete VPC component class. The new
+components in v1 no longer have hard dependencies on other resources, so
+instead the subnets from the existing VPC can be passed into other components
+directly. ## References * [Tutorial](https://www.pulumi.com/blog/crosswalk-for-
+aws-1-0/) * [API Reference Documentation](https://www.pulumi.com/registry/
+packages/awsx/api-docs/) * [Examples](./examples) * [Crosswalk for AWS Guide]
+(https://www.pulumi.com/docs/guides/crosswalk/aws/) Keywords: pulumi aws awsx
+kind/component category/cloud Platform: UNKNOWN Description-Content-Type: text/
+markdown
```

### Comparing `pulumi_awsx-1.0.1/pulumi_awsx.egg-info/SOURCES.txt` & `pulumi_awsx-1.0.2/pulumi_awsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-1.0.1/setup.py` & `pulumi_awsx-1.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.0.1"
-PLUGIN_VERSION = "1.0.1"
+VERSION = "1.0.2"
+PLUGIN_VERSION = "1.0.2"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'awsx', PLUGIN_VERSION])
         except OSError as error:
```

