# Comparing `tmp/ec2ninja-1.0-py3-none-any.whl.zip` & `tmp/ec2ninja-1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,8 @@
-Zip file size: 2109 bytes, number of entries: 7
+Zip file size: 1835 bytes, number of entries: 6
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-22 07:51 ec2ninja/__init__.py
--rw-rw-r--  2.0 unx     1859 b- defN 23-Jul-15 16:03 ec2ninja/manager.py
--rw-rw-r--  2.0 unx      114 b- defN 23-Jul-17 17:18 ec2ninja-1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jul-17 17:18 ec2ninja-1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       47 b- defN 23-Jul-17 17:18 ec2ninja-1.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        9 b- defN 23-Jul-17 17:18 ec2ninja-1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      536 b- defN 23-Jul-17 17:18 ec2ninja-1.0.dist-info/RECORD
-7 files, 2657 bytes uncompressed, 1151 bytes compressed:  56.7%
+-rw-rw-r--  2.0 unx     1816 b- defN 23-May-22 08:00 ec2ninja/manager.py
+-rw-rw-r--  2.0 unx       99 b- defN 23-May-22 08:04 ec2ninja-1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-22 08:04 ec2ninja-1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-22 08:04 ec2ninja-1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      441 b- defN 23-May-22 08:04 ec2ninja-1.1.dist-info/RECORD
+6 files, 2457 bytes uncompressed, 1031 bytes compressed:  58.0%
```

## zipnote {}

```diff
@@ -1,22 +1,19 @@
 Filename: ec2ninja/__init__.py
 Comment: 
 
 Filename: ec2ninja/manager.py
 Comment: 
 
-Filename: ec2ninja-1.0.dist-info/METADATA
+Filename: ec2ninja-1.1.dist-info/METADATA
 Comment: 
 
-Filename: ec2ninja-1.0.dist-info/WHEEL
+Filename: ec2ninja-1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ec2ninja-1.0.dist-info/entry_points.txt
+Filename: ec2ninja-1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ec2ninja-1.0.dist-info/top_level.txt
-Comment: 
-
-Filename: ec2ninja-1.0.dist-info/RECORD
+Filename: ec2ninja-1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ec2ninja/manager.py

```diff
@@ -1,13 +1,11 @@
 import boto3
 import logging
 import subprocess
 
-
-logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger(__name__)
 
 def start_instance(instance_id):
     ec2 = boto3.resource('ec2')
     instance = ec2.Instance(instance_id)
     if instance.state['Name'] == 'running':
         logger.info(f'Instance {instance_id} is already running')
@@ -46,9 +44,8 @@
 
 def ssh_to_instance(instance_id, username, private_key_file):
     ec2 = boto3.resource('ec2')
     instance = ec2.Instance(instance_id)
     ip_address = instance.public_ip_address
     ssh_command = f'ssh -i {private_key_file} {username}@{ip_address}'
     logger.info(f'SSHing into instance {instance_id}')
-    subprocess.run(ssh_command.split(), check=True)
-
+    subprocess.run(ssh_command.split(), check=True)
```

