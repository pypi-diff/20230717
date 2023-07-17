# Comparing `tmp/prelude-cli-1.3.0.tar.gz` & `tmp/prelude-cli-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude-cli-1.3.0.tar", last modified: Tue Jun 27 14:55:22 2023, max compression
+gzip compressed data, was "prelude-cli-1.3.1.tar", last modified: Mon Jul 17 19:33:02 2023, max compression
```

## Comparing `prelude-cli-1.3.0.tar` & `prelude-cli-1.3.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:55:22.096797 prelude-cli-1.3.0/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-27 14:55:22.096856 prelude-cli-1.3.0/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.0/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:55:22.093868 prelude-cli-1.3.0/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.0/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.0/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:55:22.094746 prelude-cli-1.3.0/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.0/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:55:22.096568 prelude-cli-1.3.0/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     4376 2023-06-22 22:23:23.000000 prelude-cli-1.3.0/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.0/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)     7956 2023-06-12 21:16:47.000000 prelude-cli-1.3.0/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     3895 2023-06-12 21:16:47.000000 prelude-cli-1.3.0/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     2279 2023-05-18 19:30:30.000000 prelude-cli-1.3.0/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)     1139 2023-05-03 13:30:52.000000 prelude-cli-1.3.0/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-06-27 14:55:22.094538 prelude-cli-1.3.0/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      832 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      598 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       32 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2023-06-27 14:55:22.000000 prelude-cli-1.3.0/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.0/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      663 2023-06-27 14:55:22.097080 prelude-cli-1.3.0/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.275609 prelude-cli-1.3.1/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-07-17 19:33:02.275701 prelude-cli-1.3.1/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude-cli-1.3.1/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.272566 prelude-cli-1.3.1/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      775 2023-05-02 14:19:17.000000 prelude-cli-1.3.1/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-05-03 13:30:52.000000 prelude-cli-1.3.1/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.273384 prelude-cli-1.3.1/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      263 2023-06-27 14:52:45.000000 prelude-cli-1.3.1/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.275391 prelude-cli-1.3.1/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     4543 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude-cli-1.3.1/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)     8431 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     4138 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     3041 2023-07-17 19:18:31.000000 prelude-cli-1.3.1/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      658 2023-07-17 14:47:48.000000 prelude-cli-1.3.1/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2023-07-17 19:33:02.273204 prelude-cli-1.3.1/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      832 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      598 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       32 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2023-07-17 19:33:02.000000 prelude-cli-1.3.1/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude-cli-1.3.1/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      663 2023-07-17 19:33:02.275965 prelude-cli-1.3.1/setup.cfg
```

### Comparing `prelude-cli-1.3.0/LICENSE` & `prelude-cli-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.0/PKG-INFO` & `prelude-cli-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.0
+Version: 1.3.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.0/prelude_cli/cli.py` & `prelude-cli-1.3.1/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.0/prelude_cli/views/build.py` & `prelude-cli-1.3.1/prelude_cli/views/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
 @click.option('-q', '--techniques', help='comma-separated list of valid MITRE ATT&CK codes [e.g. T1557,T1040]', default=None, type=str)
 @click.option('-a', '--advisory', default=None, hidden=True, type=str)
 @click.pass_obj
 @handle_api_error
 def create_test(controller, name, unit, test, techniques, advisory):
     """ Create or update a security test """
-    with Spinner():
+    with Spinner(description='Creating new test'):
         t = controller.create_test(
             name=name,
             unit=unit,
             test_id=test,
             techniques=techniques,
             advisory=advisory
         )
@@ -45,15 +45,15 @@
         basename = f'{t["id"]}.go'
         template = pkg_resources.read_text(templates, 'template.go')
         template = template.replace('$ID', t['id'])
         template = template.replace('$NAME', name)
         template = template.replace('$UNIT', unit or '')
         template = template.replace('$CREATED', str(datetime.utcnow()))
         
-        with Spinner():
+        with Spinner(description='Applying default template to new test'):
             controller.upload(test_id=t['id'], filename=basename, data=template)
             t['attachments'] = [basename]
 
         test_dir = PurePath(t['id'], basename)
         Path(t['id']).mkdir(parents=True, exist_ok=True)
         
         with open(test_dir, 'w', encoding='utf8') as test_code:
@@ -68,15 +68,15 @@
 @click.option('-u', '--unit', help='unit identifier', default=None, type=str)
 @click.option('-q', '--techniques', help='comma-separated list of valid MITRE ATT&CK codes [e.g. T1557,T1040]', default=None, type=str)
 @click.option('-a', '--advisory', help='alert identifier [CVE ID, Advisory ID, etc]', default=None, hidden=True, type=str)
 @click.pass_obj
 @handle_api_error
 def update_test(controller, test, name, unit, techniques, advisory):
     """ Create or update a security test """
-    with Spinner():
+    with Spinner(description='Updating test'):
         test = controller.update_test(
             test_id=test,
             name=name,
             unit=unit,
             techniques=techniques,
             advisory=advisory
         )
@@ -86,15 +86,15 @@
 @build.command('delete-test')
 @click.argument('test')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_test(controller, test):
     """ Delete a test """
-    with Spinner():
+    with Spinner(description='Removing test'):
         controller.delete_test(test_id=test)
     click.secho(f'Deleted {test}', fg='green')
 
 
 @build.command('upload')
 @click.argument('path', type=click.Path(exists=True))
 @click.option('-t', '--test', help='test identifier', default=None, type=str)
@@ -106,15 +106,15 @@
         match = UUID.search(path)
         if match:
             return match.group(0)
         raise FileNotFoundError('You must supply a test ID or include it in the path')
 
     def upload(p: Path):
         with open(p, 'rb') as data:
-            with Spinner():
+            with Spinner(description='Uploading to test'):
                 controller.upload(
                     test_id=identifier, 
                     filename=p.name, 
                     data=data.read(), 
                     binary=True
                 )
             click.secho(f'Uploaded {p.name}', fg='green')
```

### Comparing `prelude-cli-1.3.0/prelude_cli/views/configure.py` & `prelude-cli-1.3.1/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.0/prelude_cli/views/detect.py` & `prelude-cli-1.3.1/prelude_cli/views/detect.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 @click.option('-s', '--serial_num', help='serial number of this machine', type=str, required=True)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default='')
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
 def register_endpoint(controller, host, serial_num, edr_id, tags):
     """ Register a new endpoint """
-    with Spinner():
+    with Spinner(description='Registering endpoint'):
         token = controller.register_endpoint(
             host=host, 
             serial_num=serial_num, 
             edr_id=edr_id, 
             tags=tags
         )
     click.secho(token)
@@ -42,54 +42,54 @@
 @click.option('-h', '--host', help='hostname of this machine', type=str, default=None)
 @click.option('-e', '--edr_id', help='EDR id', type=str, default=None)
 @click.option('-t', '--tags', help='a comma-separated list of tags for this endpoint', type=str, default=None)
 @click.pass_obj
 @handle_api_error
 def update_endpoint(controller, endpoint_id, host, edr_id, tags):
     """ Register a new endpoint """
-    with Spinner():
+    with Spinner(description='Updating endpoint'):
         ep = controller.update_endpoint(
             endpoint_id=endpoint_id,
             host=host,
             edr_id=edr_id,
             tags=tags
         )
     print_json(data=ep)
 
 
 @detect.command('tests')
 @click.pass_obj
 @handle_api_error
 def list_tests(controller):
     """ List all security tests """
-    with Spinner():
+    with Spinner(description='Fetching all security tests'):
         data = controller.list_tests()
     print_json(data=data)
 
 
 @detect.command('test')
 @click.argument('test_id')
 @click.pass_obj
 @handle_api_error
 def get_test(controller, test_id):
     """ List properties for a test """
-    with Spinner():
+    with Spinner(description='Fetching data for test'):
         data = controller.get_test(test_id=test_id)
     print_json(data=data)
 
 
 @detect.command('download')
 @click.argument('test')
 @click.pass_obj
 @handle_api_error
 def download(controller, test):
     """ Download a test to your local environment """
     click.secho(f'Downloading {test}')
     Path(test).mkdir(parents=True, exist_ok=True)
-    with Spinner():
+    with Spinner(description='Downloading test'):
         attachments = controller.get_test(test_id=test).get('attachments')
 
         for attach in attachments:
             if Path(attach).suffix:
                 code = controller.download(test_id=test, filename=attach)
                 with open(PurePath(test, attach), 'wb') as f:
                     f.write(code)
@@ -102,82 +102,82 @@
               help='provide a run_code',
               default=RunCode.DAILY.name, show_default=True,
               type=click.Choice([r.name for r in RunCode], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
 def enable_test(controller, test, run_code, tags):
     """ Add test to your queue """
-    with Spinner():
+    with Spinner(description='Enabling test'):
         controller.enable_test(ident=test, run_code=RunCode[run_code.upper()].value, tags=tags)
 
 
 @detect.command('disable-test')
 @click.argument('test')
 @click.option('-t', '--tags', help='only disable for these tags (comma-separated list)', type=str, default='')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def disable_test(controller, test, tags):
     """ Remove test from your queue """
-    with Spinner():
+    with Spinner(description='Disabling test'):
         controller.disable_test(ident=test, tags=tags)
 
 
 @detect.command('social-stats')
 @click.argument('test')
 @click.option('-d', '--days', help='days to look back', default=30, type=int, show_default=True)
 @click.pass_obj
 @handle_api_error
 def social_statistics(controller, test, days):
     """ Pull social statistics for a specific test """
-    with Spinner():
+    with Spinner(description='Fetching social statistics'):
         data = controller.social_stats(ident=test, days=days)
     print_json(data=data)
 
 
 @detect.command('delete-endpoint')
 @click.argument('endpoint_id')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def delete_endpoint(controller, endpoint_id):
     """Delete a probe/endpoint"""
-    with Spinner():
+    with Spinner(description='Deleting endpoint'):
         controller.delete_endpoint(ident=endpoint_id)
 
 
 @detect.command('queue')
 @click.pass_obj
 @handle_api_error
 def queue(controller):
     """ List all tests in your active queue """
-    with Spinner():
+    with Spinner(description='Fetching active tests from queue'):
         iam = IAMController(account=controller.account)
         queue = iam.get_account().get('queue')
     print_json(data=queue)
 
 
 @detect.command('endpoints')
 @click.option('-d', '--days', help='only show endpoints that have run at least once in the past DAYS days', default=90, type=int)
 @click.pass_obj
 @handle_api_error
 def endpoints(controller, days):
     """ List all active endpoints associated to your account """
-    with Spinner():
+    with Spinner(description='Fetching endpoints'):
         data = controller.list_endpoints(days=days)
     print_json(data=data)
 
 
 @detect.command('advisories')
 @click.pass_obj
 @click.option('-y', '--year', help='View advisories from a specific year', default=None, type=int)
 @handle_api_error
 def advisories(controller, year):
     """ List all Prelude advisories """
-    with Spinner():
+    with Spinner(description='Fetching advisories'):
         data = controller.list_advisories(year=year)
     print_json(data=data)
 
 
 @detect.command('clone')
 @click.pass_obj
 @handle_api_error
@@ -193,15 +193,15 @@
                 code = controller.download(test_id=test['id'], filename=attach)
                 with open(PurePath(test['id'], attach), 'wb') as f:
                     f.write(code)
 
     async def start_cloning():
         await asyncio.gather(*[fetch(test) for test in controller.list_tests()])
 
-    with Spinner():
+    with Spinner(description='Downloading all tests'):
         asyncio.run(start_cloning())
     click.secho('Project cloned successfully', fg='green')
 
 
 @detect.command('activity')
 @click.option('-v', '--view',
               help='retrieve a specific result view',
@@ -228,10 +228,10 @@
     if endpoints:
         filters['endpoints'] = endpoints
     if status:
         filters['statuses'] = status
     if dos:
         filters['dos'] = dos
 
-    with Spinner():
+    with Spinner(description='Fetching activity'):
         data = controller.describe_activity(view=view, filters=filters)
     print_json(data=data)
```

### Comparing `prelude-cli-1.3.0/prelude_cli/views/iam.py` & `prelude-cli-1.3.1/prelude_cli/views/iam.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 @handle_api_error
 @click.confirmation_option(prompt='Overwrite local account credentials for selected profile?')
 def register_account(controller):
     """ Register a new account """
     email = click.prompt('Enter your email')
     name = click.prompt('(Optional) Enter your name', default='', show_default=False)
     company = click.prompt('(Optional) Enter your associated company', default='', show_default=False)
-    with Spinner():
+    with Spinner(description='Creating new account'):
         data = controller.new_account(user_email=email, user_name=name, company=company)
     print_json(data=data)
     print("\nCheck your email to verify your account.\n")
 
 
 @iam.command('update-account')
 @click.option('-m', '--mode',
@@ -39,28 +39,28 @@
               help='provide your associated company',
               default=None, show_default=False,
               type=str)
 @click.pass_obj
 @handle_api_error
 def update_account(controller, mode, company):
     """ Update an account """
-    with Spinner():
+    with Spinner(description='Updating account information'):
         data = controller.update_account(
             mode=Mode[mode.upper()].value if mode else None,
             company=company
         )
     print_json(data=data)
 
 
 @iam.command('account')
 @click.pass_obj
 @handle_api_error
 def describe_account(controller):
     """ Get account details """
-    with Spinner():
+    with Spinner(description='Fetching account details'):
         data = controller.get_account()
     print_json(data=data)
 
 
 @iam.command('create-user')
 @click.option('-d', '--days', help='days this user will remain active', default=365, type=int)
 @click.option('-p', '--permission', help='user permission level', default=Permission.SERVICE.name,
@@ -68,15 +68,15 @@
 @click.option('-n', '--name', help='name of user', default=None, show_default=False, type=str)
 @click.argument('email')
 @click.pass_obj
 @handle_api_error
 def create_user(controller, days, permission, name, email):
     """ Create a new user in your account """
     expires = datetime.utcnow() + timedelta(days=days)
-    with Spinner():
+    with Spinner(description='Creating new user'):
         data = controller.create_user(
             email=email,
             permission=Permission[permission.upper()].value,
             name=name,
             expires=expires
         )
     print_json(data=data)
@@ -87,31 +87,31 @@
 @iam.command('delete-user')
 @click.confirmation_option(prompt='Are you sure?')
 @click.argument('handle')
 @click.pass_obj
 @handle_api_error
 def delete_user(controller, handle):
     """ Remove a user from your account """
-    with Spinner():
+    with Spinner(description='Deleting user'):
         controller.delete_user(handle=handle)
 
 
 @iam.command('logs')
 @click.option('-d', '--days', help='days back to search from today', default=7, type=int)
 @click.option('-l', '--limit', help='limit the number of results', default=1000, type=int)
 @click.pass_obj
 @handle_api_error
 def logs(controller, days, limit):
     """ Get audit logs """
-    with Spinner():
+    with Spinner(description='Fetching logs'):
         data = controller.audit_logs(days=days, limit=limit)
     print_json(data=data)
 
 
 @iam.command('purge')
 @click.confirmation_option(prompt='Are you sure?')
 @click.pass_obj
 @handle_api_error
 def purge(controller):
     """ Delete your account """
-    with Spinner():
+    with Spinner(description='Purging account from existence'):
         controller.purge_account()
```

### Comparing `prelude-cli-1.3.0/prelude_cli/views/partner.py` & `prelude-cli-1.3.1/prelude_cli/views/partner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,70 @@
 import click
 
 from rich import print_json
 
+from prelude_sdk.models.codes import Control
 from prelude_cli.views.shared import handle_api_error, Spinner
 from prelude_sdk.controllers.partner_controller import PartnerController
 
 
 @click.group()
 @click.pass_context
 def partner(ctx):
     """ Partner system commands """
     ctx.obj = PartnerController(account=ctx.obj)
 
 
 @partner.command('attach')
-@click.argument('name')
-@click.option('--api', default='', help='API endpoint of the partner')
+@click.argument('partner',
+              type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
+@click.option('--api', required=True, help='API endpoint of the partner')
 @click.option('--user', default='', help='user identifier')
 @click.option('--secret', default='', help='secret for OAUTH use cases')
 @click.pass_obj
 @handle_api_error
-def attach_partner(controller, name, api, user, secret):
+def attach_partner(controller, partner, api, user, secret):
     """ Attach an EDR to Detect """
-    with Spinner():
-        data = controller.attach(name=name, api=api, user=user, secret=secret)
+    with Spinner(description='Attaching partner'):
+        data = controller.attach(partner_code=Control[partner.upper()].value, api=api, user=user, secret=secret)
     print_json(data=data)
 
 
 @partner.command('detach')
 @click.confirmation_option(prompt='Are you sure?')
-@click.argument('name')
+@click.argument('partner',
+              type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.pass_obj
 @handle_api_error
-def detach_partner(controller, name):
+def detach_partner(controller, partner):
     """ Detach an existing partner from your account """
-    with Spinner():
-        controller.detach(name=name)
+    with Spinner(description='Detaching partner'):
+        controller.detach(partner_code=Control[partner.upper()].value)
 
 
 @partner.command('endpoints')
-@click.argument('name')
+@click.argument('partner',
+              type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.option('--platform', required=True, help='platform name (e.g. "windows")', type=click.Choice(['windows', 'linux', 'darwin'], case_sensitive=False))
 @click.option('--hostname', default='', help='hostname pattern (e.g. "mycompany-c24oi444")')
 @click.option('--offset', default=0, help='API pagination offset', type=int)
 @click.pass_obj
 @handle_api_error
-def partner_endpoints(controller, name, platform, hostname, offset):
+def partner_endpoints(controller, partner, platform, hostname, offset):
     """ Get a list of endpoints from a partner """
-    with Spinner():
-        data = controller.endpoints(partner_name=name, platform=platform, hostname=hostname, offset=offset)
+    with Spinner(description='Fetching endpoints from partner'):
+        data = controller.endpoints(partner_code=Control[partner.upper()].value, platform=platform, hostname=hostname, offset=offset)
     print_json(data=data)
 
 
 @partner.command('deploy')
 @click.confirmation_option(prompt='Are you sure?')
-@click.argument('name')
+@click.argument('partner',
+              type=click.Choice([c.name for c in Control if c != Control.INVALID], case_sensitive=False))
 @click.option('--host_ids', required=True, help='a list of host IDs to deploy to', multiple=True, default=[])
 @click.pass_obj
 @handle_api_error
-def partner_deploy(controller, name, host_ids):
+def partner_deploy(controller, partner, host_ids):
     """ Deploy probes to hosts associated to a partner """
-    with Spinner():
-        data = controller.deploy(partner_name=name, host_ids=host_ids)
+    with Spinner(description='Deploying probes to hosts'):
+        data = controller.deploy(partner_code=Control[partner.upper()].value, host_ids=host_ids)
     print_json(data=data)
```

### Comparing `prelude-cli-1.3.0/prelude_cli.egg-info/PKG-INFO` & `prelude-cli-1.3.1/prelude_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.3.0
+Version: 1.3.1
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `prelude-cli-1.3.0/prelude_cli.egg-info/SOURCES.txt` & `prelude-cli-1.3.1/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude-cli-1.3.0/setup.cfg` & `prelude-cli-1.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.3.0
+version = 1.3.1
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.3.0
+	prelude-sdk == 1.3.1
 	click > 8
 	rich
 
 [options.entry_points]
 console_scripts = 
 	prelude = prelude_cli.cli:cli
```

