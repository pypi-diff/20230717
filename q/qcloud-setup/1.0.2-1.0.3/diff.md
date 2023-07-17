# Comparing `tmp/qcloud_setup-1.0.2.tar.gz` & `tmp/qcloud_setup-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcloud_setup-1.0.2.tar", last modified: Wed Jul 12 11:16:17 2023, max compression
+gzip compressed data, was "qcloud_setup-1.0.3.tar", last modified: Mon Jul 17 02:55:23 2023, max compression
```

## Comparing `qcloud_setup-1.0.2.tar` & `qcloud_setup-1.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.199137 qcloud_setup-1.0.2/
--rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.2/LICENSE.txt
--rw-r-----   0 agilbert   (501) staff       (20)    15720 2023-07-12 11:16:17.198858 qcloud_setup-1.0.2/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)    14693 2023-07-12 11:14:59.000000 qcloud_setup-1.0.2/README.md
--rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-12 11:15:50.000000 qcloud_setup-1.0.2/pyproject.toml
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.196915 qcloud_setup-1.0.2/qcloud_setup.egg-info/
--rw-r-----   0 agilbert   (501) staff       (20)    15720 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/PKG-INFO
--rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/SOURCES.txt
--rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/dependency_links.txt
--rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/entry_points.txt
--rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/requires.txt
--rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-12 11:16:17.000000 qcloud_setup-1.0.2/qcloud_setup.egg-info/top_level.txt
--rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-12 11:16:17.199181 qcloud_setup-1.0.2/setup.cfg
--rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-12 11:15:35.000000 qcloud_setup-1.0.2/setup.py
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.195692 qcloud_setup-1.0.2/src/
-drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-12 11:16:17.198281 qcloud_setup-1.0.2/src/qcloud_setup/
--rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.2/src/qcloud_setup/__init__.py
--rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/api-gateway.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/cognito.yaml
--rw-r-----   0 agilbert   (501) staff       (20)     6125 2023-06-25 23:43:46.000000 qcloud_setup-1.0.2/src/qcloud_setup/iam-policy.yaml
--rwxr-x---   0 agilbert   (501) staff       (20)    53484 2023-06-29 02:23:13.000000 qcloud_setup-1.0.2/src/qcloud_setup/qcloud_admin.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.091042 qcloud_setup-1.0.3/
+-rw-r-----   0 agilbert   (501) staff       (20)      543 2023-06-22 05:32:28.000000 qcloud_setup-1.0.3/LICENSE.txt
+-rw-r-----   0 agilbert   (501) staff       (20)    16573 2023-07-17 02:55:23.090812 qcloud_setup-1.0.3/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)    15546 2023-07-17 02:45:41.000000 qcloud_setup-1.0.3/README.md
+-rw-r-----   0 agilbert   (501) staff       (20)      747 2023-07-17 02:52:37.000000 qcloud_setup-1.0.3/pyproject.toml
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.088929 qcloud_setup-1.0.3/qcloud_setup.egg-info/
+-rw-r-----   0 agilbert   (501) staff       (20)    16573 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/PKG-INFO
+-rw-r-----   0 agilbert   (501) staff       (20)      422 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/SOURCES.txt
+-rw-r-----   0 agilbert   (501) staff       (20)        1 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/dependency_links.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       51 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/entry_points.txt
+-rw-r-----   0 agilbert   (501) staff       (20)      151 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/requires.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       13 2023-07-17 02:55:23.000000 qcloud_setup-1.0.3/qcloud_setup.egg-info/top_level.txt
+-rw-r-----   0 agilbert   (501) staff       (20)       38 2023-07-17 02:55:23.091089 qcloud_setup-1.0.3/setup.cfg
+-rw-r-----   0 agilbert   (501) staff       (20)      914 2023-07-17 02:52:44.000000 qcloud_setup-1.0.3/setup.py
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.087565 qcloud_setup-1.0.3/src/
+drwxr-x---   0 agilbert   (501) staff       (20)        0 2023-07-17 02:55:23.090563 qcloud_setup-1.0.3/src/qcloud_setup/
+-rw-r-----   0 agilbert   (501) staff       (20)        0 2023-06-25 11:45:44.000000 qcloud_setup-1.0.3/src/qcloud_setup/__init__.py
+-rw-r-----   0 agilbert   (501) staff       (20)    21623 2023-06-25 23:43:46.000000 qcloud_setup-1.0.3/src/qcloud_setup/api-gateway.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     6219 2023-06-25 23:43:46.000000 qcloud_setup-1.0.3/src/qcloud_setup/cognito.yaml
+-rw-r-----   0 agilbert   (501) staff       (20)     5729 2023-07-17 02:00:33.000000 qcloud_setup-1.0.3/src/qcloud_setup/iam-policy.yaml
+-rwxr-x---   0 agilbert   (501) staff       (20)    56143 2023-07-17 02:42:47.000000 qcloud_setup-1.0.3/src/qcloud_setup/qcloud_admin.py
```

### Comparing `qcloud_setup-1.0.2/LICENSE.txt` & `qcloud_setup-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.2/PKG-INFO` & `qcloud_setup-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud_setup
-Version: 1.0.2
+Version: 1.0.3
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -119,19 +119,21 @@
    will need to deactivate the key and generate a new one.
 
 To install the access key, run the following command and enter both the access key
 and the secret key:
 ```
 qcloud_setup  --configure-aws
 ```
-You will need to enter a supported AWS region (currently us-east-1) which will
-determine where the cluster resources are located.  Please contact Q-Chem
-support (support@q-chem.com) if you require a different region.
+The AWS region you enter will determine where the cluster resources are located.
+Note that some compute instances may not be available in some regions.
 
-These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+The access keys are stored on the local machine (in ~/.qcloud\_admin.cfg), which 
+shoud have user read access only.  If you wish to administer the cluster from another
+machine you will need to repeat the `--configure-aws` step on that machine and re-enter
+the keys.
 
 
 ## 3) Create IAM policy 
 
 We will now add IAM permissions to the qcloud user via a custom policy.  The
 policy is most easily created via a CloudFormation template that can be
 generated with:
@@ -242,29 +244,38 @@
 ## 5) Launching the cluster
 
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
+The configuration file is automatically updated with values for the place holders
+as the various resources are created.  
 
-The launch option updates the configuration file with values for the placeholders.
-
-**Note:** Progress of the stack launch is printed to the terminal and will take
-several minutes.
+**Notes:** 
+1. Some steps in the launch process can take several minutes to complete, in
+   particular building the cluster stack.  Migrating the Q-Cloud software to
+   your region can take a variable amount of time depending on network load.
+2. If you terminate the the qcloud\_setup script during the creation process
+   the stack will continue to be created.  Use the `--delete` option to
+   actually delete or stop the stack creation.  
+3. Interrupting the launch process may leave a temporary snapshot lying around.
+   To delete this, log into the [AWS console](https://signin.aws.amazon.com/) and
+   navigate to EC2 &#8594; Snapshots.  Any Q-Cloud snapshots can be safely deleted
+   as long as you are not currently launching a cluster.
 
 Once launched, you will need to send the following information to
 license@q-chem.com to obtain your license activation key:
 
-- Elastic IP address 
 - Order number
 - Name 
 - University / Institution
+- Elastic IP address (provided as output from the launch command)
 
-Once you have your activation key you can install it as follows:
+Once you have your activation key, you can install it as follows:
 ```
 qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
 This command requires access to the SSH key generated during the configuration
 step, which should be either in the current directory or in your home directory
 under ~/.ssh.
```

### Comparing `qcloud_setup-1.0.2/README.md` & `qcloud_setup-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,21 @@
    will need to deactivate the key and generate a new one.
 
 To install the access key, run the following command and enter both the access key
 and the secret key:
 ```
 qcloud_setup  --configure-aws
 ```
-You will need to enter a supported AWS region (currently us-east-1) which will
-determine where the cluster resources are located.  Please contact Q-Chem
-support (support@q-chem.com) if you require a different region.
+The AWS region you enter will determine where the cluster resources are located.
+Note that some compute instances may not be available in some regions.
 
-These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+The access keys are stored on the local machine (in ~/.qcloud\_admin.cfg), which 
+shoud have user read access only.  If you wish to administer the cluster from another
+machine you will need to repeat the `--configure-aws` step on that machine and re-enter
+the keys.
 
 
 ## 3) Create IAM policy 
 
 We will now add IAM permissions to the qcloud user via a custom policy.  The
 policy is most easily created via a CloudFormation template that can be
 generated with:
@@ -217,29 +219,38 @@
 ## 5) Launching the cluster
 
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
+The configuration file is automatically updated with values for the place holders
+as the various resources are created.  
 
-The launch option updates the configuration file with values for the placeholders.
-
-**Note:** Progress of the stack launch is printed to the terminal and will take
-several minutes.
+**Notes:** 
+1. Some steps in the launch process can take several minutes to complete, in
+   particular building the cluster stack.  Migrating the Q-Cloud software to
+   your region can take a variable amount of time depending on network load.
+2. If you terminate the the qcloud\_setup script during the creation process
+   the stack will continue to be created.  Use the `--delete` option to
+   actually delete or stop the stack creation.  
+3. Interrupting the launch process may leave a temporary snapshot lying around.
+   To delete this, log into the [AWS console](https://signin.aws.amazon.com/) and
+   navigate to EC2 &#8594; Snapshots.  Any Q-Cloud snapshots can be safely deleted
+   as long as you are not currently launching a cluster.
 
 Once launched, you will need to send the following information to
 license@q-chem.com to obtain your license activation key:
 
-- Elastic IP address 
 - Order number
 - Name 
 - University / Institution
+- Elastic IP address (provided as output from the launch command)
 
-Once you have your activation key you can install it as follows:
+Once you have your activation key, you can install it as follows:
 ```
 qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
 This command requires access to the SSH key generated during the configuration
 step, which should be either in the current directory or in your home directory
 under ~/.ssh.
```

### Comparing `qcloud_setup-1.0.2/pyproject.toml` & `qcloud_setup-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qcloud_setup"
-version = "1.0.2"
+version = "1.0.3"
 description = "Q-Cloud setup utility for cluster administrators" 
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE.txt"}
 keywords = ["qcloud", "qchem", "q-cloud", "q-chem"] 
 authors = [
   {name = "Q-Chem Inc.", email = "support@q-chem.com" }
```

### Comparing `qcloud_setup-1.0.2/qcloud_setup.egg-info/PKG-INFO` & `qcloud_setup-1.0.3/qcloud_setup.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcloud-setup
-Version: 1.0.2
+Version: 1.0.3
 Summary: Q-Cloud setup utility for cluster administrators
 Home-page: https://q-chem.com
 Author: Andrew Gilbert
 Author-email: "Q-Chem Inc." <support@q-chem.com>
 License: Confidential property of Q-Chem, Inc.
         Copyright (c) 1993 by Q-Chem, Inc. (unpublished)
         All rights reserved.
@@ -119,19 +119,21 @@
    will need to deactivate the key and generate a new one.
 
 To install the access key, run the following command and enter both the access key
 and the secret key:
 ```
 qcloud_setup  --configure-aws
 ```
-You will need to enter a supported AWS region (currently us-east-1) which will
-determine where the cluster resources are located.  Please contact Q-Chem
-support (support@q-chem.com) if you require a different region.
+The AWS region you enter will determine where the cluster resources are located.
+Note that some compute instances may not be available in some regions.
 
-These access keys are stored on the local machine (in ~/.qcloud\_admin.cfg) 
+The access keys are stored on the local machine (in ~/.qcloud\_admin.cfg), which 
+shoud have user read access only.  If you wish to administer the cluster from another
+machine you will need to repeat the `--configure-aws` step on that machine and re-enter
+the keys.
 
 
 ## 3) Create IAM policy 
 
 We will now add IAM permissions to the qcloud user via a custom policy.  The
 policy is most easily created via a CloudFormation template that can be
 generated with:
@@ -242,29 +244,38 @@
 ## 5) Launching the cluster
 
 Once a configuration file has been generated, the service stacks can be
 launched with the following:
 ```
 qcloud_setup  --launch 
 ```
+The configuration file is automatically updated with values for the place holders
+as the various resources are created.  
 
-The launch option updates the configuration file with values for the placeholders.
-
-**Note:** Progress of the stack launch is printed to the terminal and will take
-several minutes.
+**Notes:** 
+1. Some steps in the launch process can take several minutes to complete, in
+   particular building the cluster stack.  Migrating the Q-Cloud software to
+   your region can take a variable amount of time depending on network load.
+2. If you terminate the the qcloud\_setup script during the creation process
+   the stack will continue to be created.  Use the `--delete` option to
+   actually delete or stop the stack creation.  
+3. Interrupting the launch process may leave a temporary snapshot lying around.
+   To delete this, log into the [AWS console](https://signin.aws.amazon.com/) and
+   navigate to EC2 &#8594; Snapshots.  Any Q-Cloud snapshots can be safely deleted
+   as long as you are not currently launching a cluster.
 
 Once launched, you will need to send the following information to
 license@q-chem.com to obtain your license activation key:
 
-- Elastic IP address 
 - Order number
 - Name 
 - University / Institution
+- Elastic IP address (provided as output from the launch command)
 
-Once you have your activation key you can install it as follows:
+Once you have your activation key, you can install it as follows:
 ```
 qcloud_setup  --activation-key XXXX-XXXX-XXXX-XXXX-XXXX
 ```
 This command requires access to the SSH key generated during the configuration
 step, which should be either in the current directory or in your home directory
 under ~/.ssh.
```

### Comparing `qcloud_setup-1.0.2/setup.py` & `qcloud_setup-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_namespace_packages
 
 setup(
     name="qcloud_setup",
     python_requires='>=3.7',
-    version="1.0.2",
+    version="1.0.3",
     url="https://q-chem.com",
     author="Andrew Gilbert",
     author_email="support@q-chem.com",
     description="Utility for setting up Q-Cloud administrators",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(where="src"),
```

### Comparing `qcloud_setup-1.0.2/src/qcloud_setup/api-gateway.yaml` & `qcloud_setup-1.0.3/src/qcloud_setup/api-gateway.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.2/src/qcloud_setup/cognito.yaml` & `qcloud_setup-1.0.3/src/qcloud_setup/cognito.yaml`

 * *Files identical despite different names*

### Comparing `qcloud_setup-1.0.2/src/qcloud_setup/iam-policy.yaml` & `qcloud_setup-1.0.3/src/qcloud_setup/iam-policy.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -31,73 +31,69 @@
       - iam:CreatePolicy
       - iam:DeletePolicy
       - iam:CreateRole
       - iam:DeleteRole
       - iam:AttachRolePolicy
       - iam:DetachRolePolicy
       - iam:DeleteRolePolicy
-      - iam:PassRole
       - iam:ListPolicyVersions
       Resource:
       - !Sub arn:aws:iam::${AWS::AccountId}:policy/*
       - !Sub arn:aws:iam::${AWS::AccountId}:role/*
       Effect: Allow
     - Action:
       - iam:PassRole
       Condition:
        StringEqualsIfExists:
          iam:PassedToService:
          - lambda.amazonaws.com
          - ec2.amazonaws.com
          - spotfleet.amazonaws.com
+         - apigateway.amazonaws.com
       Resource:
-      - !Sub arn:aws:iam::${AWS::AccountId}:role/parallelcluster/*
+      - !Sub arn:aws:iam::${AWS::AccountId}:policy/*
+      - !Sub arn:aws:iam::${AWS::AccountId}:role/*
       Effect: Allow
     - Action:
       - iam:GetServiceLinkedRoleDeletionStatus
       - iam:DeleteServiceLinkedRole
       Resource:
       - arn:aws:iam::*:role/aws-service-role/cognito-idp.amazonaws.com/AWSServiceRoleForAmazonCognitoIdp*
       - arn:aws:iam::*:role/aws-service-role/email.cognito-idp.amazonaws.com/AWSServiceRoleForAmazonCognitoIdpEmail*
       Effect: Allow
+    - Action: iam:CreateServiceLinkedRole
+      Resource: "*"
+      Condition:
+       StringEquals:
+         iam:AWSServiceName:
+         - cognito-idp.amazonaws.com
+         - email.cognito-idp.amazonaws.com
+      Effect: Allow
     - Action:
+      - ec2:Describe*
+      - ec2:*KeyPair
+      - ec2:*LaunchTemplate*
+      - ec2:*NetworkInterface
+      - ec2:*PlacementGroup
+      - ec2:ModifyVolume*
+      - ec2:RevokeSecurityGroup*
+      - ec2:AuthorizeSecurityGroup*
+      - ec2:*SecurityGroup
+      - ec2:*Snapshot
+      - ec2:ModifyNetworkInterfaceAttribute
       - ec2:AllocateAddress
       - ec2:AssociateAddress
-      - ec2:AttachNetworkInterface
-      - ec2:AuthorizeSecurityGroupEgress
-      - ec2:AuthorizeSecurityGroupIngress
+      - ec2:ReleaseAddress
       - ec2:CreateFleet
-      - ec2:CreateKeyPair
-      - ec2:DeleteKeyPair
-      - ec2:Describe*
-      - ec2:CreateLaunchTemplate
-      - ec2:CreateLaunchTemplateVersion
-      - ec2:CreateNetworkInterface
-      - ec2:CreatePlacementGroup
-      - ec2:CreateSecurityGroup
-      - ec2:CreateSnapshot
-      - ec2:CreateTags
       - ec2:CreateVolume
-      - ec2:CreateLaunchTemplate
-      - ec2:DeleteLaunchTemplate
-      - ec2:DeleteNetworkInterface
-      - ec2:DeletePlacementGroup
-      - ec2:DeleteSecurityGroup
       - ec2:DeleteVolume
+      - ec2:CreateTags
       - ec2:DisassociateAddress
-      - ec2:ModifyLaunchTemplate
-      - ec2:ModifyNetworkInterfaceAttribute
-      - ec2:ModifyVolume
-      - ec2:ModifyVolumeAttribute
-      - ec2:ReleaseAddress
-      - ec2:RevokeSecurityGroupEgress
-      - ec2:RevokeSecurityGroupIngress
       - ec2:RunInstances
       - ec2:TerminateInstances
-      - ec2:DescribeAvailabilityZones
       - ec2:CreateInternetGateway
       - ec2:CreateVpcEndpoint
       - ec2:CreateRoute
       - ec2:CreateVpc
       - ec2:CreateRouteTable
       - ec2:AttachInternetGateway
       - ec2:ModifyVpcAttribute
@@ -173,24 +169,17 @@
       - route53:ChangeTagsForResource
       - route53:CreateHostedZone
       - route53:DeleteHostedZone
       - route53:GetChange
       - route53:GetHostedZone
       - route53:ListResourceRecordSets
       - route53:ListQueryLoggingConfigs
+      - route53:AssociateVPCWithHostedZone
       - sns:GetSMSSandboxAccountStatus
       - ses:ListIdentities
       - ses:GetIdentityVerificationAttributes
       - sns:ListPlatformApplications
       Resource: "*"
       Effect: Allow
     - Action: secretsmanager:DescribeSecret
       Resource: !Sub arn:aws:secretsmanager:*:${AWS::AccountId}:secret:*
       Effect: Allow
-    - Action: iam:CreateServiceLinkedRole
-      Resource: "*"
-      Condition:
-       StringEquals:
-         iam:AWSServiceName:
-         - cognito-idp.amazonaws.com
-         - email.cognito-idp.amazonaws.com
-      Effect: Allow
```

### Comparing `qcloud_setup-1.0.2/src/qcloud_setup/qcloud_admin.py` & `qcloud_setup-1.0.3/src/qcloud_setup/qcloud_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,86 @@
 from pathlib import Path
 from pprint import pprint
 from collections import defaultdict, OrderedDict
 
 import importlib.resources 
 
 
-DEBUG = False
-VERSION = "v6.1.0"
+SOURCE_SNAPSHOT = "snap-07e1149ce851713a8"
+SOURCE_REGION   = "us-east-1"
+VERSION         = "v6.1.0"
 
+DEBUG = False
 
 
 def debug(s):
     if DEBUG: pprint(s)
  
 
 class QCloudError(Exception):
     pass
 
 
+def copy_snapshot(session):
+    global SOURCE_SNAPSHOT
+    global SOURCE_REGION
+
+    source_snapshot = SOURCE_SNAPSHOT
+    source_region   = SOURCE_REGION
+
+    if "QCLOUD_SNAPSHOT_ID" in os.environ:
+       source_snapshot = os.getenv('QCLOUD_SNAPSHOT_ID')
+
+    if "QCLOUD_SNAPSHOT_REGION" in os.environ:
+       source_region = os.getenv('QCLOUD_SNAPSHOT_REGION')
+
+    snapshot_id = None
+
+    client  = session.client("ec2")
+    response = client.copy_snapshot(
+       SourceRegion=source_region, 
+       SourceSnapshotId=source_snapshot,
+       Description='Q-Cloud {}'.format(VERSION)
+    )   
+    snapshot_id = response['SnapshotId']
+    watch_snapshot_progress(session, snapshot_id)
+
+    return snapshot_id
+
+
+def watch_snapshot_progress(session, snapshot_id):
+    client = session.client('ec2')
+    done   = False
+    
+    while not done:
+        response = client.describe_snapshots(SnapshotIds=[snapshot_id])
+        snapshot = response['Snapshots'][0]
+        prog = snapshot['Progress']
+
+        if prog == "100%":
+            checklist("Migrating Q-Cloud software","COMPLETE ", True)
+            return
+        else:
+            for i in range(128):
+                checklist("Migrating Q-Cloud software","{}".format(progress(i)))
+                sleep(0.1)
+
+
+def remove_snapshot(session, snapshot_id):
+    if not snapshot_id: return
+
+    checklist("Cleaning up temporary installation files")
+    client = session.client("ec2")
+    response = client.delete_snapshot(
+       SnapshotId=snapshot_id
+    )   
+    checklist("Cleaning up temporary installation files","COMPLETE",True)
+
+
+
 def get_snapshot_id(region):
     snapshots = { 
        "us-east-1" : "snap-07e1149ce851713a8",
     }
 
     if "QCLOUD_SNAPSHOT_ID" in os.environ:
        id = os.getenv('QCLOUD_SNAPSHOT_ID')
@@ -113,15 +172,14 @@
         checklist("Writing cluster configuration")
         with open(fname, 'w', encoding='utf8') as outfile:
             yaml.dump(self.config, outfile, Dumper=YamlDumper, default_flow_style=False, allow_unicode=True)
         checklist("Cluster configuration written to:", fname, True)
 
 
 
-
 def checklist(key, value="", check=False):
     verbose = True
     tick = u'\u2713'
     if verbose and check:
        print("[{0}] {1: <42} {2}".format(tick,key,value))
     elif verbose:
        print("[ ] {0: <42} {1}".format(key,value), end='\r')
@@ -366,17 +424,14 @@
 
         tags = vpc.get('Tags',[])
         for tag in tags:
             if tag['Key'] == 'Name':
                 vpc_descriptions[-1] += "    " + tag['Value']
                 if tag['Value'] == 'Q-Cloud VPC':
                     vpc_id = vpc['VpcId']
-                    #if not interactive:
-                    #   checklist("Using existing Q-Cloud VPC:", vpc_id, True)
-                    #   return vpc_id
 
     vpc_descriptions.append("Create new")
     last = len(vpc_descriptions)-1
     prompt = "VPC to use:"
     if vpc_id:
        index = vpc_ids.index(vpc_id)
     else:
@@ -677,16 +732,16 @@
              }
     scheduling = {'Scheduler': 'slurm' }
     scheduling['SlurmSettings'] = { 'ScaledownIdletime': 5 }
     scheduling['SlurmQueues'] = [ queue ]
     config.set('Scheduling', scheduling)
 
     # SharedStorage
-    snapshot_id = get_snapshot_id(session.region_name)
-    qcloud = {'EbsSettings': { 'Size': 5, 'SnapshotId': snapshot_id, 
+    #snapshot_id = get_snapshot_id(session.region_name)
+    qcloud = {'EbsSettings': { 'Size': 5, 'SnapshotId': 'SNAPSHOT_ID', 
               'Encrypted': False,
               'VolumeType': 'gp2'}, 
               'MountDir': '/mnt/qcloud',
               'Name': 'qcloud-ebs',
               'StorageType': 'Ebs' }
 
     jobs   = {'EbsSettings': { 'Size': job_volume, 'VolumeType': 'gp2'}, 
@@ -818,15 +873,15 @@
            if (response == 'y' or response == 'yes'):
               if stack_name.endswith("cluster"):
                  detach_execute_policy(session, stack_name)
               client.delete_stack(StackName = stack_name)
               deleted.append(stack_name)
               if stack_name.endswith("api-gateway"):
                  api_bucket_name = get_resource_id(session, stack_name, 'ApiBucket')
-                 if not bucket_is_empty(session, api_bucket_name):
+                 if api_bucket_name and not bucket_is_empty(session, api_bucket_name):
                     print("Bucket {} is not empty and will NOT be deleted".format(api_bucket_name))
              
     for stack_name in deleted:
         print_stack_status(session,stack_name)
 
 
 
@@ -1142,53 +1197,87 @@
     do_cognito = not nocognito
     do_gateway = True
     do_cluster = True 
 
     if do_cognito:
        if not admin_email:
           #admin_email = get_cognito_email()
-          admin_email = 'anybody@anywhere.com'
+          admin_email = 'anybody@example.com'
        launch_cognito(session, cognito_stack, admin_email)
 
     if do_gateway:
        cognitoArn = get_userpool_arn(session, cognito_stack)
        launch_api_gateway(session, api_stack, cognitoArn)
        checklist("Updating config file with API resources")
        execute_policy_arn = get_resource_id(session, api_stack, 'ExecutePolicy')
        api_bucket_name = get_resource_id(session, api_stack, 'ApiBucket')
        update_config_file(cluster_stack, api_bucket_name, execute_policy_arn) 
-       checklist("Updating config file with API resources","done",True)
+       checklist("Updating config file with API resources","COMPLETE",True)
 
     if do_cluster:
-       launch_cluster(session, cluster_stack)
+       if not stack_exists(session,cluster_stack):
+           snapshot_id = copy_snapshot(session)
+           update_config_snapshot(cluster_stack, snapshot_id)
+           launch_cluster(session, cluster_stack)
+           remove_snapshot(session,snapshot_id)
+
        update_lambda(session, cluster_stack, api_stack)
        post_launch(session, name)
-       checklist("Q-Cloud cluster {} launch:".format(name), "SUCCESS", True)
+       get_cluster_ip(cluster_stack)
+       checklist("Q-Cloud cluster {} launch".format(name), "SUCCESS", True)
 
 
+def get_cluster_ip(stack_name):
+    checklist("Retrieving elastic IP address")
+    config = ConfigFile(stack_name)
+    fname  = config.fname()
+    
+    with open(fname) as file:
+         text = file.read()
+
+    ip = re.search("ElasticIp:\s*(.+)", text)
+    if ip:
+       checklist("Retrieving elastic IP address", ip.group(1), True)
+    else:
+        print("[x] Failed to determine elastic IP, check config file")
+
 
 def update_lambda(session, cluster_stack, api_stack):
     instance_id = get_resource_id(session, cluster_stack, 'HeadNode')
-    checklist("Setting instance ID for lambda functions:", instance_id)
+    checklist("Updating config file with instance ID")
     lambda_qcloud = get_resource_id(session, api_stack, 'LambdaFunctionQCloud')
     lambda_s3submit = get_resource_id(session, api_stack, 'LambdaFunctionS3Submit')
     update_lambda_env(session, lambda_qcloud, instance_id)
     update_lambda_env(session, lambda_s3submit, instance_id)
-    checklist("Setting instance ID for lambda functions:", instance_id, True)
+    checklist("Updating config file with instance ID", "COMPLETE", True)
  
 
-
 def update_lambda_env(session, lambda_id, instance_id):
     client = session.client("lambda")
     response = client.update_function_configuration(
         FunctionName = lambda_id,
         Environment = { 'Variables': { 'INSTANCE_ID': instance_id } }
     )
 
 
+def update_config_snapshot(stack_name, snapshot_id):
+    checklist("Updating config file with snapshot")
+    config = ConfigFile(stack_name)
+    fname  = config.fname()
+    
+    with open(fname) as file:
+         text = file.read()
+
+    text = re.sub("SnapshotId:.+", "SnapshotId: {}".format(snapshot_id), text)
+
+    with open(fname, "w") as file:
+         file.write(text)
+
+    checklist("Updating config file with snapshot", "COMPLETE", True)
+
 
 def update_config_file(stack_name, api_bucket_name, execute_policy_arn):
     config = ConfigFile(stack_name)
     fname  = config.fname()
     
     with open(fname) as file:
          text = file.read()
@@ -1380,15 +1469,15 @@
     checklist("Updating packages")
     cmd = "/mnt/qcloud/bin/post_install"
     ssh_stdin, ssh_stdout, ssh_stderr = ssh_client.exec_command(cmd)
     ssh_stdout.channel.recv_exit_status()
     lines = ssh_stdout.readlines()
     debug(lines)
 
-    checklist("Performing post launch configuration","", True);
+    checklist("Performing post launch configuration","COMPLETE", True);
 
 
 def ssh_connection(session, name):
     checklist("Getting stack information")
     cloudformation = session.resource('cloudformation') 
     stack_name = "{}-cluster".format(name)
 
@@ -1561,14 +1650,15 @@
         parser.add_argument("--shell", dest="shell", action='store_true',
             help="open shell connection to the head node")
 
 
         args, extra_args = parser.parse_known_args()
 
         if args.debug:
+           global DEBUG
            DEBUG = True
 
         if args.config_aws:
             configure_session()
             exit(0)
 
         if args.gen_iam:
```

