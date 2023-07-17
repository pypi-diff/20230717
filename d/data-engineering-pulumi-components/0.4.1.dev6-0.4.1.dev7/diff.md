# Comparing `tmp/data-engineering-pulumi-components-0.4.1.dev6.tar.gz` & `tmp/data-engineering-pulumi-components-0.4.1.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-engineering-pulumi-components-0.4.1.dev6.tar", max compression
+gzip compressed data, was "data-engineering-pulumi-components-0.4.1.dev7.tar", max compression
```

## Comparing `data-engineering-pulumi-components-0.4.1.dev6.tar` & `data-engineering-pulumi-components-0.4.1.dev7.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0        0 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/__init__.py
--rw-r--r--   0        0        0       95 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/auth0/__init__.py
--rw-r--r--   0        0        0     4454 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/auth0/create_application.py
--rw-r--r--   0        0        0     1694 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/__init__.py
--rw-r--r--   0        0        0    12025 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/bucket.py
--rw-r--r--   0        0        0      557 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py
--rw-r--r--   0        0        0      856 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/curated_bucket.py
--rw-r--r--   0        0        0     1132 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/fail_bucket.py
--rw-r--r--   0        0        0     1179 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/landing_bucket.py
--rw-r--r--   0        0        0     2182 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py
--rw-r--r--   0        0        0      585 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py
--rw-r--r--   0        0        0     4276 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py
--rw-r--r--   0        0        0     9018 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/glue/glue_job.py
--rw-r--r--   0        0        0    16667 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/glue/glue_move_script.py
--rw-r--r--   0        0        0     6713 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py
--rw-r--r--   0        0        0     6626 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py
--rw-r--r--   0        0        0     3262 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py
--rw-r--r--   0        0        0     3236 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py
--rw-r--r--   0        0        0      962 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py
--rw-r--r--   0        0        0      933 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py
--rw-r--r--   0        0        0     2282 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py
--rw-r--r--   0        0        0     2751 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py
--rw-r--r--   0        0        0     1001 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py
--rw-r--r--   0        0        0     1390 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py
--rw-r--r--   0        0        0     1437 2022-08-31 14:47:32.990562 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py
--rw-r--r--   0        0        0 10008354 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.tar.gz
--rw-r--r--   0        0        0     8773 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py
--rw-r--r--   0        0        0     6685 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/move_object_function.py
--rw-r--r--   0        0        0     3155 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py
--rw-r--r--   0        0        0    10974 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/validate_function.py
--rw-r--r--   0        0        0     4379 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/rest_apigateway.py
--rw-r--r--   0        0        0     2766 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py
--rw-r--r--   0        0        0     2077 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/roles/create_upload_role.py
--rw-r--r--   0        0        0      213 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/pipelines/__init__.py
--rw-r--r--   0        0        0     2428 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py
--rw-r--r--   0        0        0     4585 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py
--rw-r--r--   0        0        0     8557 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/utils.py
--rw-r--r--   0        0        0      638 2022-08-31 14:47:33.022564 data-engineering-pulumi-components-0.4.1.dev6/pyproject.toml
--rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev6/setup.py
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev6/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/__init__.py
+-rw-r--r--   0        0        0       95 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/__init__.py
+-rw-r--r--   0        0        0     4454 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/create_application.py
+-rw-r--r--   0        0        0     1728 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/__init__.py
+-rw-r--r--   0        0        0     4212 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket.py
+-rw-r--r--   0        0        0    10416 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket_policy.py
+-rw-r--r--   0        0        0      772 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/cloudtrail_log_bucket.py
+-rw-r--r--   0        0        0      684 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/curated_bucket.py
+-rw-r--r--   0        0        0     1181 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/fail_bucket.py
+-rw-r--r--   0        0        0     1387 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/landing_bucket.py
+-rw-r--r--   0        0        0     2182 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py
+-rw-r--r--   0        0        0      634 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py
+-rw-r--r--   0        0        0     4276 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py
+-rw-r--r--   0        0        0     9018 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_job.py
+-rw-r--r--   0        0        0    16667 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_move_script.py
+-rw-r--r--   0        0        0     6713 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py
+-rw-r--r--   0        0        0     6626 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py
+-rw-r--r--   0        0        0     3262 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py
+-rw-r--r--   0        0        0     3236 2022-09-05 15:43:02.273771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py
+-rw-r--r--   0        0        0      962 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py
+-rw-r--r--   0        0        0      933 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py
+-rw-r--r--   0        0        0     2282 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py
+-rw-r--r--   0        0        0     2751 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py
+-rw-r--r--   0        0        0     1001 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py
+-rw-r--r--   0        0        0     1390 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py
+-rw-r--r--   0        0        0     1437 2022-09-05 15:43:02.281771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py
+-rw-r--r--   0        0        0 10008354 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.tar.gz
+-rw-r--r--   0        0        0     8773 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py
+-rw-r--r--   0        0        0     6685 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/move_object_function.py
+-rw-r--r--   0        0        0     3155 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py
+-rw-r--r--   0        0        0    10974 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/validate_function.py
+-rw-r--r--   0        0        0     4379 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/rest_apigateway.py
+-rw-r--r--   0        0        0     2766 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py
+-rw-r--r--   0        0        0     2077 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_upload_role.py
+-rw-r--r--   0        0        0      213 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/__init__.py
+-rw-r--r--   0        0        0     2428 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py
+-rw-r--r--   0        0        0     5170 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py
+-rw-r--r--   0        0        0     8557 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/utils.py
+-rw-r--r--   0        0        0      638 2022-09-05 15:43:02.309771 data-engineering-pulumi-components-0.4.1.dev7/pyproject.toml
+-rw-r--r--   0        0        0     1849 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev7/setup.py
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 data-engineering-pulumi-components-0.4.1.dev7/PKG-INFO
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/auth0/create_application.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/auth0/create_application.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/__init__.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from .buckets.bucket import Bucket, BucketPutPermissionsArgs
+from .buckets.bucket_policy import BucketPutPermissionsArgs
+from .buckets.bucket import Bucket
 from .buckets.curated_bucket import CuratedBucket
 from .buckets.fail_bucket import FailBucket
 from .buckets.landing_bucket import LandingBucket
 from .buckets.pulumi_backend_bucket import PulumiBackendBucket
 from .buckets.raw_history_bucket import RawHistoryBucket
 from .buckets.cloudtrail_log_bucket import CloudTrailLogBucket
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/bucket_policy.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 import json
-import re
-from typing import Optional, Sequence, Union
-
-import pulumi_aws.s3 as s3
-from pulumi_aws.s3 import BucketCorsRuleArgs
+import pulumi_aws as aws
+from pulumi import ComponentResource, Output, ResourceOptions
+from typing import Sequence, Optional, Union
 from data_engineering_pulumi_components.utils import (
-    Tagger,
     validate_principal,
     is_anonymous_user,
 )
-from pulumi import ComponentResource, ResourceOptions, Output
-from pulumi_aws import Provider
-
-
-class InvalidBucketNameError(Exception):
-    pass
 
 
 class AnonymousUserError(Exception):
     pass
 
 
 class BucketPutPermissionsArgs:
@@ -43,143 +34,76 @@
                 if not isinstance(path, str):
                     raise TypeError("Each path must be of type str")
                 if not path.startswith("/") or not path.endswith("/"):
                     raise ValueError("Each path must start and end with '/'")
         self.paths = paths
 
 
-def _bucket_name_is_valid(name: str) -> bool:
-    """
-    Checks if an S3 bucket name is valid.
-
-    See https://docs.aws.amazon.com/AmazonS3/latest/userguide/bucketnamingrules.html
-
-    Parameters
-    ----------
-    name : str
-        The name of the bucket.
-
-    Returns
-    -------
-    bool
-        If the name is valid.
-    """
-    match = re.match(
-        pattern=(
-            # ensure name is between 3 and 63 characters long
-            r"(?=^.{3,63}$)"
-            # ensure name is not formatted like an IP address
-            r"(?!^(\d+\.)+\d+$)"
-            # match zero or more labels followed by a single period
-            r"(^(([a-z0-9]|[a-z0-9][a-z0-9\-]*[a-z0-9])\.)*"
-            # ensure final label doesn't end in a period or dash
-            r"([a-z0-9]|[a-z0-9][a-z0-9\-]*[a-z0-9])$)"
-        ),
-        string=name,
-    )
-    if match:
-        return True
-    else:
-        return False
-
-
-class Bucket(ComponentResource):
+class BucketPolicyBuilder(ComponentResource):
     def __init__(
         self,
-        name: str,
-        tagger: Tagger,
-        cors_rules: BucketCorsRuleArgs = None,
-        t: Optional[str] = None,
-        lifecycle_rules: Sequence[s3.BucketLifecycleRuleArgs] = None,
+        Bucket,
         put_permissions: Optional[Sequence[BucketPutPermissionsArgs]] = None,
-        versioning: Optional[s3.BucketVersioningArgs] = None,
-        provider: Provider = None,
+        t: Optional[str] = None,
         opts: Optional[ResourceOptions] = None,
-    ) -> None:
+    ):
+        """
+        Pass a bucket and some permissions to this object to build a bucket policy and
+        attach it to a bucket.
+        """
         if t is None:
-            t = "data-engineering-pulumi-components:aws:Bucket"
+            t = "data-engineering-pulumi-components:aws:BucketPolicyBuilder"
+        self._name = Bucket._name + "_BucketPolicyBuilder"
         super().__init__(
             t=t,
-            name=name,
+            name=self._name,
             props=None,
             opts=opts,
         )
-        if not isinstance(name, str):
-            raise TypeError("name must be of type str")
-        if not isinstance(tagger, Tagger):
-            raise TypeError("tagger must be of type Tagger")
-
-        if not _bucket_name_is_valid(name=name):
-            raise InvalidBucketNameError("name is not valid")
-
-        self._name = name
-
-        self._bucket = s3.Bucket(
-            resource_name=f"{name}-bucket",
-            acl=s3.CannedAcl.PRIVATE,
-            cors_rules=cors_rules,
-            bucket=name,
-            force_destroy=True,
-            lifecycle_rules=lifecycle_rules,
-            server_side_encryption_configuration={
-                "rule": {
-                    "apply_server_side_encryption_by_default": {
-                        "sse_algorithm": "AES256"
-                    }
-                }
-            },
-            tags=tagger.create_tags(name=name),
-            versioning=versioning,
-            opts=ResourceOptions(parent=self)
-            if provider is None
-            else ResourceOptions(parent=self, provider=provider),
-        )
-        self._bucketPublicAccessBlock = s3.BucketPublicAccessBlock(
-            resource_name=f"{name}-bucket-public-access-block",
-            bucket=self._bucket.id,
-            block_public_acls=True,
-            block_public_policy=True,
-            ignore_public_acls=True,
-            restrict_public_buckets=True,
-            opts=ResourceOptions(parent=self._bucket),
-        )
 
-        if put_permissions:
-            self.add_permissions(put_permissions=put_permissions)
+        if getattr(Bucket, "_put_permissions", None) is not None:
+            raise Exception("put_permissions are already set")
 
-        outputs = {
-            "arn": self._bucket.arn,
-            "id": self._bucket.id,
-            "name": self._bucket.bucket,
-        }
+        self.Bucket = Bucket
+        self._put_permissions = put_permissions
+        self._statements = []
 
-        for name, value in outputs.items():
-            setattr(self, name, value)
+    @property
+    def add_basic_access_permissions(
+        self,
+    ):
+        self._statements = Output.all(
+            bucket_arn=self.Bucket._bucket.arn,
+            **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
+            if self._put_permissions
+            else {},
+        ).apply(self._get_basic_access_policy)
 
-        self.register_outputs(outputs)
+        return self
 
-    def _get_policy(self, args):
+    def _get_basic_access_policy(self, args):
         bucket_arn = args.pop("bucket_arn")
-        block_access = args.pop("block_access")
 
         all_principals = []
         statements = []
         for item in args.values():
             principal = item["principal"]
             paths = item["paths"]
             all_principals.append(principal)
-            statements.append(
-                {
-                    "Effect": "Allow",
-                    "Principal": {"AWS": [principal]},
-                    "Action": ["s3:PutObject", "s3:PutObjectAcl"],
-                    "Resource": [bucket_arn + path + "*" for path in paths]
-                    if paths
-                    else [bucket_arn + "/*"],
-                }
+            statements.extend(
+                [
+                    {
+                        "Effect": "Allow",
+                        "Principal": {"AWS": [principal]},
+                        "Action": ["s3:PutObject", "s3:PutObjectAcl"],
+                        "Resource": [bucket_arn + path + "*" for path in paths]
+                        if paths
+                        else [bucket_arn + "/*"],
+                    }
+                ]
             )
         statements.extend(
             [
                 {
                     "Effect": "Deny",
                     "Principal": {"AWS": all_principals},
                     "Action": ["s3:PutObject"],
@@ -208,31 +132,32 @@
                     "Resource": [bucket_arn + "/*"],
                     "Condition": {
                         "Null": {"s3:x-amz-server-side-encryption": ["true"]},
                     },
                 },
             ]
         )
-        if block_access:
-            statements.extend(
-                [
-                    {
-                        "Effect": "Deny",
-                        "Principal": {"AWS": "*"},
-                        "Action": "s3:*",
-                        "Resource": [bucket_arn + path for path in paths]
-                        + [bucket_arn + path + "*" for path in paths]
-                        if paths
-                        else [bucket_arn, bucket_arn + "/*"],
-                        "Condition": {"StringLike": {"aws:PrincipalArn": "*/alpha_*"}},
-                    }
-                ]
-            )
 
-        return json.dumps({"Version": "2012-10-17", "Statement": statements})
+        return statements
+
+    @property
+    def add_glue_permissions(self):
+        self._glue_statements = Output.all(
+            bucket_arn=self.Bucket._bucket.arn,
+            **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
+            if self._put_permissions
+            else {},
+        ).apply(self._get_policy_glue)
+
+        self._statements = Output.all(
+            statements=self._statements,
+            glue_statements=self._glue_statements,
+        ).apply(lambda args: args.pop("statements") + args.pop("glue_statements"))
+
+        return self
 
     def _get_policy_glue(self, args):
         bucket_arn = args.pop("bucket_arn")
 
         all_principals = []
         statements = []
         for item in args.values():
@@ -255,93 +180,115 @@
                     "Resource": [bucket_arn + path for path in paths]
                     + [bucket_arn + path + "*" for path in paths]
                     if paths
                     else [bucket_arn, bucket_arn + "/*"],
                 }
             )
 
-        return json.dumps({"Version": "2012-10-17", "Statement": statements})
+        return statements
 
-    def _get_cloudtrail_policy(self, args):
+    @property
+    def add_access_block(self):
+        self._access_block_statements = Output.all(
+            bucket_arn=self.Bucket._bucket.arn,
+            **{str(i): item.__dict__ for i, item in enumerate(self._put_permissions)}
+            if self._put_permissions
+            else {},
+        ).apply(self._access_block_policy)
+
+        self._statements = Output.all(
+            statements=self._statements,
+            access_block_statements=self._access_block_statements,
+        ).apply(
+            lambda args: args.pop("statements") + args.pop("access_block_statements")
+        )
+
+        return self
+
+    def _access_block_policy(self, args):
         bucket_arn = args.pop("bucket_arn")
-        return json.dumps(
-            {
-                "Version": "2012-10-17",
-                "Statement": [
-                    {
-                        "Sid": "AWSCloudTrailAclCheck",
-                        "Effect": "Allow",
-                        "Principal": {"Service": "cloudtrail.amazonaws.com"},
-                        "Action": "s3:GetBucketAcl",
-                        "Resource": bucket_arn,
-                    },
+        statements = []
+        for item in args.values():
+            paths = item["paths"]
+            statements.extend(
+                [
                     {
-                        "Sid": "AWSCloudTrailWrite",
-                        "Effect": "Allow",
-                        "Principal": {"Service": "cloudtrail.amazonaws.com"},
-                        "Action": "s3:PutObject",
-                        "Resource": bucket_arn + "/*",
-                        "Condition": {
-                            "StringEquals": {
-                                "s3:x-amz-acl": "bucket-owner-full-control"
-                            }
-                        },
+                        "Effect": "Deny",
+                        "Principal": {"AWS": "*"},
+                        "Action": "s3:*",
+                        "Resource": [bucket_arn + path for path in paths]
+                        + [bucket_arn + path + "*" for path in paths]
+                        if paths
+                        else [bucket_arn, bucket_arn + "/*"],
+                        "Condition": {"StringLike": {"aws:PrincipalArn": "*/alpha_*"}},
                     },
-                ],
-            }
-        )
-
-    def add_permissions(
-        self,
-        put_permissions: Sequence[BucketPutPermissionsArgs],
-        glue_permissions: bool = False,
-        block_access: bool = False,
-        cloud_trail_permissions: bool = False,
-    ):
-        if not getattr(self, "_put_permissions", None):
-            self._put_permissions = put_permissions
-            if cloud_trail_permissions:
-                policy = Output.all(
-                    bucket_arn=self._bucket.arn,
-                ).apply(self._get_cloudtrail_policy)
-            elif glue_permissions:
-                policy = Output.all(
-                    bucket_arn=self._bucket.arn,
-                    **{str(i): item.__dict__ for i, item in enumerate(put_permissions)},
-                ).apply(self._get_policy_glue)
-            else:
-                policy = Output.all(
-                    bucket_arn=self._bucket.arn,
-                    block_access=block_access,
-                    **{str(i): item.__dict__ for i, item in enumerate(put_permissions)},
-                ).apply(self._get_policy)
-
-            self._bucketPolicy = s3.BucketPolicy(
-                resource_name=f"{self._name}-bucket-policy",
-                bucket=self._bucket.id,
-                policy=policy,
-                opts=ResourceOptions(parent=self._bucket),
+                ]
             )
-        else:
-            raise Exception("put_permissions are already set")
 
-    def add_cors_rules(
-        self,
-        cors_allowed_headers: list,
-        cors_allowed_origins: list,
-    ):
+        return statements
+
+    @property
+    def add_cloud_trail_permissions(self):
+        self._cloudtrail_statements = Output.all(
+            bucket_arn=self.Bucket._bucket.arn,
+        ).apply(self._get_cloudtrail_policy)
+
+        self._statements = Output.all(
+            statements=self._statements,
+            cloudtrail_statements=self._cloudtrail_statements,
+        ).apply(lambda args: args.pop("statements") + args.pop("cloudtrail_statements"))
+
+        return self
+
+    def _get_cloudtrail_policy(self, args):
+        bucket_arn = args.pop("bucket_arn")
+
         return [
-            BucketCorsRuleArgs(
-                allowed_headers=cors_allowed_headers,
-                allowed_methods=[
-                    "PUT",
-                    "POST",
-                ],
-                allowed_origins=cors_allowed_origins,
-                expose_headers=[
-                    "x-amz-server-side-encryption",
-                    "x-amz-request-id",
-                    "x-amz-id-2",
-                ],
-                max_age_seconds=3000,
-            )
+            {
+                "Sid": "AWSCloudTrailAclCheck",
+                "Effect": "Allow",
+                "Principal": {"Service": "cloudtrail.amazonaws.com"},
+                "Action": "s3:GetBucketAcl",
+                "Resource": bucket_arn,
+            },
+            {
+                "Sid": "AWSCloudTrailWrite",
+                "Effect": "Allow",
+                "Principal": {"Service": "cloudtrail.amazonaws.com"},
+                "Action": "s3:PutObject",
+                "Resource": bucket_arn + "/*",
+                "Condition": {
+                    "StringEquals": {"s3:x-amz-acl": "bucket-owner-full-control"}
+                },
+            },
         ]
+
+    def _get_final_policy_doc(self):
+        # Every operation to an Output object needs to be an apply or a Pulumi function
+        return self._statements.apply(
+            lambda l: json.dumps({"Version": "2012-10-17", "Statement": l})
+        )
+
+    def _create_bucket_policy(self, policy_doc: Output):
+        # Some of the glue outputs aren't compatible with direct reference in the
+        # bucket policy creation, so it all needs to be wrapped in an output object.
+        return Output.all(
+            name=self.Bucket._name,
+            bucket_id=self.Bucket._bucket.id,
+            policy_doc=policy_doc,
+            bucket=self.Bucket,
+        ).apply(
+            lambda args: aws.s3.BucketPolicy(
+                resource_name=f"{args['name']}-bucket-policy",
+                bucket=args["bucket_id"],
+                policy=args["policy_doc"],  # needs to be json
+                opts=ResourceOptions(parent=args["bucket"]),
+            )
+        )
+
+    def build(self):
+        self._policy_doc = self._get_final_policy_doc()
+        self._policy = self._create_bucket_policy(self._policy_doc)
+        # Tag the bucket with put permissions so another policy is not added
+        self.Bucket._put_permissions = self._put_permissions
+
+        return self._policy
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/curated_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/curated_bucket.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,23 @@
-from typing import Optional, Sequence
-from data_engineering_pulumi_components.aws.buckets.bucket import (
-    Bucket,
-    BucketPutPermissionsArgs,
-)
+from typing import Optional
+from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ResourceOptions
 from pulumi_aws import Provider
 
 
 class CuratedBucket(Bucket):
     def __init__(
         self,
         name: str,
         tagger: Tagger,
-        put_permissions: Optional[Sequence[BucketPutPermissionsArgs]] = None,
         provider: Provider = None,
         opts: Optional[ResourceOptions] = None,
     ) -> None:
         super().__init__(
             name=name + "-curated",
             tagger=tagger,
             t="data-engineering-pulumi-components:aws:CuratedBucket",
-            put_permissions=put_permissions,
             cors_rules=None,
             provider=provider,
             opts=opts,
         )
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/fail_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/fail_bucket.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional
-
 from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ResourceOptions
 import pulumi_aws as aws
 
 
 class FailBucket(Bucket):
@@ -26,7 +25,8 @@
                             days=14,
                         )
                     ),
                 )
             ],
             opts=opts,
         )
+        # Lack of policy is currently intentional
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/pulumi_backend_bucket.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/buckets/raw_history_bucket.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from typing import Optional
-
 from data_engineering_pulumi_components.aws.buckets.bucket import Bucket
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ResourceOptions
 
 
 class RawHistoryBucket(Bucket):
     def __init__(
@@ -12,7 +11,8 @@
         super().__init__(
             name=name + "-raw-history",
             tagger=tagger,
             t="data-engineering-pulumi-components:aws:RawHistoryBucket",
             versioning={"enabled": True},
             opts=opts,
         )
+        # Lack of policy is currently intentional
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/cloud_trail/cloud_trail.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/glue/glue_job.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_job.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/glue/glue_move_script.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/glue/glue_move_script.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/authorisation_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/copy_object_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_databases_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/get_tables_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/authorise_/authorise_.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/copy/copy_.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_databases/get_databases.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/get_tables/get_tables.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/move/move.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/notify/notify_lambda_failure.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/upload_/upload_.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.tar.gz` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/dependencies.tar.gz`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/lambda_handlers/validate/validate.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/move_object_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/move_object_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/upload_object_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/lambdas/validate_function.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/lambdas/validate_function.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/rest_apigateway.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/rest_apigateway.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_list_bucket_role.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/aws/roles/create_upload_role.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/aws/roles/create_upload_role.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/landing_to_raw_history.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/pipelines/raw_history_to_curated.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from data_engineering_pulumi_components.aws.glue.glue_job import GlueComponent
 from data_engineering_pulumi_components.aws import (
     BucketPutPermissionsArgs,
     CopyObjectFunction,
     CuratedBucket,
     RawHistoryBucket,
 )
+from data_engineering_pulumi_components.aws.buckets.bucket_policy import (
+    BucketPolicyBuilder,
+)
 from data_engineering_pulumi_components.utils import Tagger
 from pulumi import ComponentResource, ResourceOptions
 from pulumi_aws import Provider
 from pulumi_aws.glue import CatalogDatabase
 import os
 from pathlib import Path
 
@@ -43,33 +46,43 @@
         )
         self._curatedBucket = CuratedBucket(
             name=name,
             tagger=tagger,
             provider=stack_provider,
             opts=ResourceOptions(parent=self, provider=stack_provider),
         )
-        if not add_tables_to_db:
+        if add_tables_to_db is False:
             self._copyObjectFunction = CopyObjectFunction(
                 destination_bucket=self._curatedBucket,
                 name=name,
                 source_bucket=raw_history_bucket,
                 tagger=tagger,
                 opts=ResourceOptions(parent=self),
             )
 
-            self._curatedBucket.add_permissions(
+            bpb = BucketPolicyBuilder(
+                Bucket=self._curatedBucket,
                 put_permissions=[
                     BucketPutPermissionsArgs(
                         principal=self._copyObjectFunction._role.arn
                     )
                 ],
-                block_access=block_access,
             )
-        else:
-            # create database of multiple_db_in_bucket option is not true
+            if block_access is True:
+                self._curatedBucket._bucketPolicy = (
+                    bpb.add_basic_access_permissions.add_access_block.build()
+                )
+            if block_access is False:
+                self._curatedBucket._bucketPolicy = (
+                    bpb.add_basic_access_permissions.build()
+                )
+
+        if add_tables_to_db is True:
+            # create database if multiple_db_in_bucket option is false
+
             if multiple_db_in_bucket == "False":
                 db_name = name.replace("-", "_")
                 self._database = CatalogDatabase(
                     resource_name=f"{name}-database",
                     description=f"A Glue Database for tables from {name}",
                     name=f"{db_name}",
                     opts=ResourceOptions(provider=default_provider),
@@ -103,20 +116,20 @@
                 ),
                 trigger_on_demand=db_refresh_on_create,
                 trigger_on_schedule=db_refresh_schedule,
                 high_memory_worker=high_memory_worker,
                 number_of_workers=number_of_workers,
             )
 
-            raw_history_bucket.add_permissions(
+            raw_history_bucket._bucketPolicy = BucketPolicyBuilder(
+                Bucket=raw_history_bucket,
                 put_permissions=[
                     BucketPutPermissionsArgs(principal=self._glueMoveJob._role.arn)
                 ],
-                glue_permissions=True,
-            )
+            ).add_glue_permissions.build()
 
-            self._curatedBucket.add_permissions(
+            self._curatedBucket._bucketPolicy = BucketPolicyBuilder(
+                Bucket=self._curatedBucket,
                 put_permissions=[
                     BucketPutPermissionsArgs(principal=self._glueMoveJob._role.arn)
                 ],
-                glue_permissions=True,
-            )
+            ).add_glue_permissions.build()
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/data_engineering_pulumi_components/utils.py` & `data-engineering-pulumi-components-0.4.1.dev7/data_engineering_pulumi_components/utils.py`

 * *Files identical despite different names*

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/pyproject.toml` & `data-engineering-pulumi-components-0.4.1.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-engineering-pulumi-components"
-version = "v0.4.1.dev6"
+version = "v0.4.1.dev7"
 description = "Reusable components for use in Pulumi Python projects"
 authors = ["MoJ Data Engineering Team <data-engineering@digital.justice.gov.uk>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = "^1.17.00"
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/setup.py` & `data-engineering-pulumi-components-0.4.1.dev7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
  'protobuf>=4.21.5,<5.0.0',
  'pulumi-auth0>=2.13.0,<3.0.0',
  'pulumi-aws>=5.0.0,<6.0.0',
  'pulumi>=3.38.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'data-engineering-pulumi-components',
-    'version': '0.4.1.dev6',
+    'version': '0.4.1.dev7',
     'description': 'Reusable components for use in Pulumi Python projects',
     'long_description': 'None',
     'author': 'MoJ Data Engineering Team',
     'author_email': 'data-engineering@digital.justice.gov.uk',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `data-engineering-pulumi-components-0.4.1.dev6/PKG-INFO` & `data-engineering-pulumi-components-0.4.1.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-engineering-pulumi-components
-Version: 0.4.1.dev6
+Version: 0.4.1.dev7
 Summary: Reusable components for use in Pulumi Python projects
 License: MIT
 Author: MoJ Data Engineering Team
 Author-email: data-engineering@digital.justice.gov.uk
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

