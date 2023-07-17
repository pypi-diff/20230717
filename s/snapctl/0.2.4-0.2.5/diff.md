# Comparing `tmp/snapctl-0.2.4.tar.gz` & `tmp/snapctl-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snapctl-0.2.4.tar", max compression
+gzip compressed data, was "snapctl-0.2.5.tar", max compression
```

## Comparing `snapctl-0.2.4.tar` & `snapctl-0.2.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.4/README.md
--rw-r--r--   0        0        0      399 2023-04-27 23:57:44.481693 snapctl-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.4/snapctl/__init__.py
--rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.4/snapctl/__main__.py
--rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.4/snapctl/commands/__init__.py
--rw-r--r--   0        0        0     8106 2023-04-27 23:57:35.572397 snapctl-0.2.4/snapctl/commands/byosnap.py
--rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.4/snapctl/main.py
--rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.4/snapctl/types/__init__.py
--rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.4/snapctl/types/definitions.py
--rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.4/snapctl/utils/__init__.py
--rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.4/snapctl/utils/echo.py
--rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      138 2023-04-11 06:06:23.860220 snapctl-0.2.5/README.md
+-rw-r--r--   0        0        0      399 2023-07-17 05:05:15.425994 snapctl-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 05:47:56.822347 snapctl-0.2.5/snapctl/__init__.py
+-rw-r--r--   0        0        0       47 2023-03-24 21:28:04.581292 snapctl-0.2.5/snapctl/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:58:03.721459 snapctl-0.2.5/snapctl/commands/__init__.py
+-rw-r--r--   0        0        0     8993 2023-07-17 05:04:59.590853 snapctl-0.2.5/snapctl/commands/byosnap.py
+-rw-r--r--   0        0        0     1297 2023-04-11 06:05:15.495245 snapctl-0.2.5/snapctl/main.py
+-rw-r--r--   0        0        0        0 2023-04-11 05:59:24.957443 snapctl-0.2.5/snapctl/types/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-11 04:34:25.684424 snapctl-0.2.5/snapctl/types/definitions.py
+-rw-r--r--   0        0        0        0 2023-04-11 06:00:21.052854 snapctl-0.2.5/snapctl/utils/__init__.py
+-rw-r--r--   0        0        0      321 2023-03-10 06:45:50.660269 snapctl-0.2.5/snapctl/utils/echo.py
+-rw-r--r--   0        0        0      571 1970-01-01 00:00:00.000000 snapctl-0.2.5/PKG-INFO
```

### Comparing `snapctl-0.2.4/snapctl/commands/byosnap.py` & `snapctl-0.2.5/snapctl/commands/byosnap.py`

 * *Files 7% similar despite different names*

```diff
@@ -67,14 +67,16 @@
     # Get the data
     # url = self.token_parts[0]
     # web_app_token = self.token_parts[1]
     service_id = self.token_parts[2]
     ecr_repo_url = self.token_parts[3]
     ecr_repo_username = self.token_parts[4]
     ecr_repo_token = self.token_parts[5]
+    image_tag = f'{service_id}.{self.tag}'
+    full_ecr_repo_url = f'{ecr_repo_url}:{image_tag}'
     try:
       # Check dependencies
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
@@ -93,15 +95,15 @@
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
         progress.add_task(description=f'Logging into Snapser Image Registry...', total=None)
         if platform == 'win32':
           response = subprocess.run([
-            f'docker login --username {ecr_repo_username} --password {ecr_repo_token} {ecr_repo_url}'
+            'docker', 'login', '--username', ecr_repo_username, '--password', ecr_repo_token, ecr_repo_url
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         else:
           response = subprocess.run([
             f'echo "{ecr_repo_token}" | docker login --username {ecr_repo_username} --password-stdin {ecr_repo_url}'
           ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to connect to the Snapser Container Repository. Please get the latest token from the Web app.')
@@ -112,33 +114,44 @@
       # Build your snap
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
         progress.add_task(description=f'Building your snap...', total=None)
-        response = subprocess.run([
-          #f"docker build --no-cache -t {tag} {path}"
-          f"docker build --platform linux/arm64 -t {service_id}.{self.tag} {self.path}"
-        ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        if platform == "win32":
+          response = subprocess.run([
+            #f"docker build --no-cache -t {tag} {path}"
+            'docker', 'build', '--platform', 'linux/arm64', '-t', image_tag, self.path
+          ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        else:
+          response = subprocess.run([
+            #f"docker build --no-cache -t {tag} {path}"
+            f"docker build --platform linux/arm64 -t {image_tag} {self.path}"
+          ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to build docker.')
           return False
       success('Build Successfull')
 
       # Tag the repo
       with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
         transient=True,
       ) as progress:
         progress.add_task(description=f'Tagging your snap...', total=None)
-        response = subprocess.run([
-          f"docker tag {service_id}.{self.tag} {ecr_repo_url}:{service_id}.{self.tag}"
-        ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        if platform == "win32":
+           response = subprocess.run([
+            'docker', 'tag', image_tag, full_ecr_repo_url
+          ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+        else:
+          response = subprocess.run([
+            f"docker tag {image_tag} {full_ecr_repo_url}"
+          ], shell=True, stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
         if response.returncode:
           error('Unable to tag your snap.')
           return False
       success('Tag Successfull')
 
       return True
     except:
@@ -146,27 +159,34 @@
       return False
 
   def push(self) -> bool:
     # url = self.token_parts[0]
     # web_app_token = self.token_parts[1]
     service_id = self.token_parts[2]
     ecr_repo_url = self.token_parts[3]
+    image_tag = f'{service_id}.{self.tag}'
+    full_ecr_repo_url = f'{ecr_repo_url}:{image_tag}'
     # ecr_repo_username = self.token_parts[4]
     # ecr_repo_token = self.token_parts[5]
 
     # Push the image
     with Progress(
       SpinnerColumn(),
       TextColumn("[progress.description]{task.description}"),
       transient=True,
     ) as progress:
       progress.add_task(description=f'Pushing your snap...', total=None)
-      response = subprocess.run([
-        f"docker push {ecr_repo_url}:{service_id}.{self.tag}"
-      ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+      if platform == "win32":
+        response = subprocess.run([
+          'docker', 'push', full_ecr_repo_url
+        ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
+      else:
+        response = subprocess.run([
+          f"docker push {full_ecr_repo_url}"
+        ], shell=True, )#stdout=subprocess.DEVNULL, stderr=subprocess.STDOUT)
       if response.returncode:
         error('Unable to push your snap.')
         return False
     success('Snap Upload Successfull')
     return True
 
   def upload_docs(self) -> bool:
```

### Comparing `snapctl-0.2.4/snapctl/main.py` & `snapctl-0.2.5/snapctl/main.py`

 * *Files identical despite different names*

### Comparing `snapctl-0.2.4/PKG-INFO` & `snapctl-0.2.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snapctl
-Version: 0.2.4
+Version: 0.2.5
 Summary: Snapser CLI Tool
 Author: Ajinkya Apte
 Author-email: aj@snapser.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

