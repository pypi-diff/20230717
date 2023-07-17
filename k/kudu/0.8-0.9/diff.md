# Comparing `tmp/kudu-0.8.tar.gz` & `tmp/kudu-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/kudu-0.8.tar", last modified: Tue Jan 19 12:34:43 2021, max compression
+gzip compressed data, was "dist/kudu-0.9.tar", last modified: Tue Mar 23 10:08:03 2021, max compression
```

## Comparing `kudu-0.8.tar` & `kudu-0.9.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2021-01-19 12:34:43.000000 kudu-0.8/
--rwxr-xr-x   0 joshua    (1000) joshua    (1000)     1191 2021-01-19 12:27:31.000000 kudu-0.8/setup.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      825 2021-01-19 12:34:43.000000 kudu-0.8/PKG-INFO
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      825 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/PKG-INFO
--rw-r--r--   0 joshua    (1000) joshua    (1000)      489 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/SOURCES.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)       51 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/requires.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        5 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/top_level.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)       44 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/entry_points.txt
--rw-r--r--   0 joshua    (1000) joshua    (1000)        1 2021-01-19 12:34:43.000000 kudu-0.8/kudu.egg-info/dependency_links.txt
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2021-01-19 12:34:43.000000 kudu-0.8/kudu/
--rw-r--r--   0 joshua    (1000) joshua    (1000)      694 2021-01-19 09:57:27.000000 kudu-0.8/kudu/types.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1355 2021-01-19 09:57:27.000000 kudu-0.8/kudu/config.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       83 2021-01-19 09:57:27.000000 kudu-0.8/kudu/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1730 2021-01-19 09:57:27.000000 kudu-0.8/kudu/defaults.py
--rwxr-xr-x   0 joshua    (1000) joshua    (1000)     1025 2021-01-19 09:57:27.000000 kudu-0.8/kudu/__main__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)      571 2021-01-19 09:57:27.000000 kudu-0.8/kudu/api.py
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2021-01-19 12:34:43.000000 kudu-0.8/kudu/commands/
--rw-r--r--   0 joshua    (1000) joshua    (1000)        0 2021-01-19 09:57:27.000000 kudu-0.8/kudu/commands/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2150 2021-01-19 09:57:27.000000 kudu-0.8/kudu/commands/pull.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1684 2021-01-19 09:57:27.000000 kudu-0.8/kudu/commands/push.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     4982 2021-01-19 09:57:27.000000 kudu-0.8/kudu/commands/link.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1351 2021-01-19 09:57:27.000000 kudu-0.8/kudu/commands/init.py
-drwxr-xr-x   0 joshua    (1000) joshua    (1000)        0 2021-01-19 12:34:43.000000 kudu-0.8/kudu/tests/
--rw-r--r--   0 joshua    (1000) joshua    (1000)        0 2021-01-19 09:57:27.000000 kudu-0.8/kudu/tests/__init__.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1761 2021-01-19 09:57:27.000000 kudu-0.8/kudu/tests/test_pull.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1476 2021-01-19 09:57:27.000000 kudu-0.8/kudu/tests/test_push.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)     2179 2021-01-19 09:57:27.000000 kudu-0.8/kudu/tests/test_link.py
--rw-r--r--   0 joshua    (1000) joshua    (1000)       38 2021-01-19 12:34:43.000000 kudu-0.8/setup.cfg
--rw-r--r--   0 joshua    (1000) joshua    (1000)     1108 2021-01-19 09:57:27.000000 kudu-0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-23 10:08:03.000000 kudu-0.9/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1182 2021-03-23 10:07:55.000000 kudu-0.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-03-23 10:08:03.000000 kudu-0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-23 10:08:03.000000 kudu-0.9/kudu/
+-rw-r--r--   0 runner    (1001) docker     (121)     1377 2021-03-23 10:07:55.000000 kudu-0.9/kudu/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2021-03-23 10:07:55.000000 kudu-0.9/kudu/mkztemp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2059 2021-03-23 10:07:55.000000 kudu-0.9/kudu/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-23 10:08:03.000000 kudu-0.9/kudu/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-23 10:07:55.000000 kudu-0.9/kudu/commands/init.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-23 10:07:55.000000 kudu-0.9/kudu/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2158 2021-03-23 10:07:55.000000 kudu-0.9/kudu/commands/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2021-03-23 10:07:55.000000 kudu-0.9/kudu/commands/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5019 2021-03-23 10:07:55.000000 kudu-0.9/kudu/commands/link.py
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2021-03-23 10:07:55.000000 kudu-0.9/kudu/api.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1027 2021-03-23 10:07:55.000000 kudu-0.9/kudu/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-23 10:08:03.000000 kudu-0.9/kudu/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1429 2021-03-23 10:07:55.000000 kudu-0.9/kudu/tests/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2357 2021-03-23 10:07:55.000000 kudu-0.9/kudu/tests/test_link.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-03-23 10:07:55.000000 kudu-0.9/kudu/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2044 2021-03-23 10:07:55.000000 kudu-0.9/kudu/tests/test_push.py
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2021-03-23 10:07:55.000000 kudu-0.9/kudu/types.py
+-rw-r--r--   0 runner    (1001) docker     (121)       83 2021-03-23 10:07:55.000000 kudu-0.9/kudu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1276 2021-03-23 10:07:55.000000 kudu-0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       44 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       75 2021-03-23 10:08:03.000000 kudu-0.9/kudu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      825 2021-03-23 10:08:03.000000 kudu-0.9/PKG-INFO
```

### Comparing `kudu-0.8/setup.py` & `kudu-0.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -13,29 +13,26 @@
     classifiers=[
         'Intended Audience :: Developers',
         'Topic :: Utilities',
         'License :: OSI Approved :: BSD License',
         'Natural Language :: English',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.6',
         'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.2',
-        'Programming Language :: Python :: 3.3',
-        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
     ],
     keywords='cli',
     packages=find_packages(),
     install_requires=[
-        'click<8',
-        'GitPython',
-        'PyYAML',
-        'requests>=2.20.1',
-        'watchdog',
+        'requests>=2.25.1',
+        'PyYAML>=5.4.1',
+        'watchdog>=0.10.6,<1.0.0',
+        'click>=7.1.2,<8.0.0',
     ],
     entry_points={
-        'console_scripts': [
-            'kudu = kudu.__main__:cli',
-        ],
+        'console_scripts': ['kudu = kudu.__main__:cli',],
     },
 )
```

### Comparing `kudu-0.8/PKG-INFO` & `kudu-0.9/kudu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: kudu
-Version: 0.8
+Version: 0.9
 Summary: A deployment command line program in Python.
 Home-page: https://github.com/torfeld6/kudu
 Author: Joshua Heller
 Author-email: joshua@torfeld6.com
 License: BSD
 Description: UNKNOWN
 Keywords: cli
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kudu-0.8/kudu.egg-info/PKG-INFO` & `kudu-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 1.1
 Name: kudu
-Version: 0.8
+Version: 0.9
 Summary: A deployment command line program in Python.
 Home-page: https://github.com/torfeld6/kudu
 Author: Joshua Heller
 Author-email: joshua@torfeld6.com
 License: BSD
 Description: UNKNOWN
 Keywords: cli
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.6
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.2
-Classifier: Programming Language :: Python :: 3.3
-Classifier: Programming Language :: Python :: 3.4
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
```

### Comparing `kudu-0.8/kudu/types.py` & `kudu-0.9/kudu/types.py`

 * *Files identical despite different names*

### Comparing `kudu-0.8/kudu/config.py` & `kudu-0.9/kudu/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 
 import click
 import yaml
 
 
 def write_config(data, path='.kudu.yml'):
     with open(path, 'w+') as stream:
-        yaml.safe_dump(data, stream, default_flow_style=False, allow_unicode=True)
+        yaml.safe_dump(
+            data, stream, default_flow_style=False, allow_unicode=True
+        )
 
 
 def read_config(path='.kudu.yml'):
     try:
         with open(path, 'r+') as stream:
             try:
                 from yaml import CLoader as Loader, CDumper as Dumper
```

### Comparing `kudu-0.8/kudu/defaults.py` & `kudu-0.9/kudu/defaults.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,40 +2,60 @@
 import re
 import subprocess
 
 import click
 
 
 def default_pitcher_folders():
-    click.echo('Your Pitcher Folders are configured automatically based on your iOS simulator devices. Please check '
-               'that they are accurate. You can suppress this message by setting them explicitly. Run the following '
-               'command and follow the instructions in your editor to edit your configuration file:\n\n'
-               '\tkudu config --global --edit\n')
+    click.echo(
+        'Your Pitcher Folders are configured automatically based on your iOS simulator devices. Please check '
+        'that they are accurate. You can suppress this message by setting them explicitly. Run the following '
+        'command and follow the instructions in your editor to edit your configuration file:\n\n'
+        '\tkudu config --global --edit\n'
+    )
 
     ios_sim_devices = []
 
     try:
-        instruments_output = subprocess.check_output(['instruments', '-s', 'devices']).splitlines()
+        instruments_output = subprocess.check_output([
+            'instruments', '-s', 'devices'
+        ]).splitlines()
         prog = re.compile(r"iPad .+\[([^\]]+)")
-        devices_path = os.path.expanduser('~/Library/Developer/CoreSimulator/Devices/')
+        devices_path = os.path.expanduser(
+            '~/Library/Developer/CoreSimulator/Devices/'
+        )
 
         for line in instruments_output:
             prog_match = prog.match(line)
             if prog_match:
                 device_guid = prog_match.group(1)
-                find_output = subprocess.check_output(
-                    ['find', os.path.join(devices_path, device_guid), '-name', 'Pitcher Folders']).strip()
+                find_output = subprocess.check_output([
+                    'find',
+                    os.path.join(devices_path, device_guid), '-name',
+                    'Pitcher Folders'
+                ]).strip()
                 if find_output:
-                    ios_sim_devices.append({'name': line, 'guid': device_guid, 'pitcher_folders': find_output})
+                    ios_sim_devices.append({
+                        'name': line,
+                        'guid': device_guid,
+                        'pitcher_folders': find_output
+                    })
     except OSError:
         pass
 
     if len(ios_sim_devices) > 0:
         ios_sim_device_index = 0
 
         if len(ios_sim_devices) > 1:
             for key, device in enumerate(ios_sim_devices):
                 click.echo('%d. %s' % (key + 1, device['name']))
-            ios_sim_device_index = int(click.prompt('Please select a device', type=click.Choice(
-                [str(key + 1) for key, device in enumerate(ios_sim_devices)]))) - 1
+            ios_sim_device_index = int(
+                click.prompt(
+                    'Please select a device',
+                    type=click.Choice([
+                        str(key + 1)
+                        for key, device in enumerate(ios_sim_devices)
+                    ])
+                )
+            ) - 1
 
         return ios_sim_devices[ios_sim_device_index]['pitcher_folders']
```

### Comparing `kudu-0.8/kudu/__main__.py` & `kudu-0.9/kudu/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,31 +7,36 @@
 from kudu.commands.link import link
 from kudu.commands.pull import pull
 from kudu.commands.push import push
 from kudu.config import ConfigOption
 
 
 @click.group()
-@click.option('--username', '-u', cls=ConfigOption, prompt=True, envvar='KUDU_USERNAME')
-@click.option('--password', '-p', cls=ConfigOption, prompt=True, hide_input=True, envvar='KUDU_PASSWORD')
+@click.option(
+    '--username', '-u', cls=ConfigOption, prompt=True, envvar='KUDU_USERNAME'
+)
+@click.option(
+    '--password',
+    '-p',
+    cls=ConfigOption,
+    prompt=True,
+    hide_input=True,
+    envvar='KUDU_PASSWORD'
+)
 @click.option('--token', '-t', cls=ConfigOption, envvar='KUDU_TOKEN')
 @click.pass_context
 def cli(ctx, username, password, token):
     if not token:
         try:
             token = authenticate(username, password)
         except ValueError:
             click.echo('Invalid username or password', err=True)
             exit(1)
 
-    ctx.obj = {
-        'username': username,
-        'password': password,
-        'token': token
-    }
+    ctx.obj = {'username': username, 'password': password, 'token': token}
 
 
 cli.add_command(init)
 cli.add_command(pull)
 cli.add_command(push)
 cli.add_command(link)
```

### Comparing `kudu-0.8/kudu/api.py` & `kudu-0.9/kudu/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,28 @@
 api_url = 'https://api.pitcher.com'
 pitcher_file_categories = ['presentation', 'zip', 'interface']
 
 
 def request(method, url, token=None, **kwargs):
     return getattr(requests, method)(
         api_url + url,
-        headers={'Authorization': 'Token %s' % token} if token else None,
+        headers={
+            'Authorization': 'Token %s' % token
+        } if token else None,
         **kwargs
     )
 
 
 def authenticate(username, password):
-    res = request('post', '/auth/user/', json={
-        'username': username,
-        'password': password
-    })
+    res = request(
+        'post',
+        '/auth/user/',
+        json={
+            'username': username,
+            'password': password
+        }
+    )
 
     if res.status_code != 200:
         raise ValueError
 
     return res.json().get('token')
```

### Comparing `kudu-0.8/kudu/commands/pull.py` & `kudu-0.9/kudu/commands/pull.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,28 +58,28 @@
     res = requests.get(download_url, stream=True)
     with open(path, 'w+b') as f:
         copyfileobj(res.raw, f)
 
 
 @click.command()
 @click.option(
-    '--file', '-f', 'pf',
+    '--file',
+    '-f',
+    'pf',
     cls=ConfigOption,
     config_name='file_id',
     prompt='File ID',
     type=PitcherFileType()
 )
-@click.option(
-    '--path', '-p',
-    type=click.Path(),
-    default=lambda: os.getcwd()
-)
+@click.option('--path', '-p', type=click.Path(), default=lambda: os.getcwd())
 @click.pass_context
 def pull(ctx, pf, path):
-    download_url = api_request('get', '/files/%d/download-url/' % pf['id'], token=ctx.obj['token']).json()
+    download_url = api_request(
+        'get', '/files/%d/download-url/' % pf['id'], token=ctx.obj['token']
+    ).json()
 
     if isdir(path):
         filename_root, filename_ext = os.path.splitext(pf['filename'])
 
         if filename_ext == '.zip':
             to_dir(download_url, path, filename_root, pf['category'])
         else:
```

### Comparing `kudu-0.8/kudu/commands/link.py` & `kudu-0.9/kudu/commands/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 import os
 import time
 from fnmatch import fnmatch
 from os import getcwd
-from os.path import join, splitext, split
+from os.path import join, split, splitext
 from shutil import copyfile
 
 import click
-from watchdog.events import FileSystemEventHandler, EVENT_TYPE_MODIFIED, EVENT_TYPE_MOVED, EVENT_TYPE_CREATED
+from watchdog.events import (
+    EVENT_TYPE_CREATED, EVENT_TYPE_MODIFIED, EVENT_TYPE_MOVED,
+    FileSystemEventHandler
+)
 from watchdog.observers import Observer
 
 from kudu.config import ConfigOption
 from kudu.defaults import default_pitcher_folders
 from kudu.types import PitcherFileType
 
 
 class PitcherFilePathConverter(object):
+
     def __init__(self, pfile):
         self.pfile = pfile
 
     def convert(self, relpath):
         raise NotImplementedError()
 
 
@@ -38,14 +42,15 @@
     def convert(self, relpath):
         if fnmatch(relpath, join('iPadOnly', '*')):
             relpath = os.sep.join(split(relpath)[1:])
         return super(PresentationPathConverter, self).convert(relpath)
 
 
 class InterfacePathConverter(PitcherFilePathConverter):
+
     def convert(self, relpath):
         if fnmatch(relpath, join('interface', '*')):
             dirname = splitext(self.pfile['filename'])[0]
             relpath = join(dirname, *split(relpath)[1:])
         return relpath
 
 
@@ -53,15 +58,16 @@
 
     def __init__(self, src, dst, converter):
         self.src = src
         self.dst = dst
         self.converter = converter
 
     def on_any_event(self, event):
-        if event.event_type in [EVENT_TYPE_MODIFIED, EVENT_TYPE_MOVED, EVENT_TYPE_CREATED] and not event.is_directory:
+        if event.event_type in [EVENT_TYPE_MODIFIED, EVENT_TYPE_MOVED,
+                                EVENT_TYPE_CREATED] and not event.is_directory:
             src_path = event.src_path if event.event_type != EVENT_TYPE_MOVED else event.dest_path
             src_relpath = os.path.relpath(src_path)
 
             dst_relpath = self.converter.convert(src_relpath)
             dst_path = join(self.dst, dst_relpath)
             dst_dirpath = os.path.dirname(dst_path)
 
@@ -93,15 +99,15 @@
 
 
 def copyfiles(src, dst, converter):
     total = countfiles(src)
     curr = 0
 
     if not os.path.exists(dst):
-        os.makedirs(dst, 0755)
+        os.makedirs(dst, 0o755)
 
     click.echo('Copying files', nl=False)
 
     for root, dirs, files in os.walk(src):
 
         for name in files:
             curr += 1
@@ -132,21 +138,32 @@
             time.sleep(1)
     except KeyboardInterrupt:
         observer.stop()
     observer.join()
 
 
 @click.command()
-@click.option('--file', '-f', 'pfile',
-              cls=ConfigOption, config_name='file_id',
-              prompt=True, type=PitcherFileType(category=['zip', 'presentation', '']))
-@click.option('--pitcher-folders', '-pf',
-              cls=ConfigOption, config_name='pitcher_folders',
-              prompt=True, default=lambda: default_pitcher_folders(),
-              type=click.Path(exists=True, file_okay=False, writable=True))
+@click.option(
+    '--file',
+    '-f',
+    'pfile',
+    cls=ConfigOption,
+    config_name='file_id',
+    prompt=True,
+    type=PitcherFileType(category=['zip', 'presentation', ''])
+)
+@click.option(
+    '--pitcher-folders',
+    '-pf',
+    cls=ConfigOption,
+    config_name='pitcher_folders',
+    prompt=True,
+    default=lambda: default_pitcher_folders(),
+    type=click.Path(exists=True, file_okay=False, writable=True)
+)
 def link(pfile, pitcher_folders):
     cwd = getcwd()
 
     if pfile['category'] == 'zip':
         converter = InteractivePathConverter(pfile)
     elif pfile['category'] == 'presentation':
         converter = PresentationPathConverter(pfile)
```

### Comparing `kudu-0.8/kudu/commands/init.py` & `kudu-0.9/kudu/commands/init.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,35 @@
 
 @click.command()
 @click.pass_context
 def init(ctx):
     if click.confirm('Would you like to create a new file?'):
         file_id = create_file(ctx.obj['token'])
     else:
-        file_id = validate_file(click.prompt('File ID', type=int), ctx.obj['token'])
+        file_id = validate_file(
+            click.prompt('File ID', type=int), ctx.obj['token']
+        )
 
     write_config({'file_id': file_id})
 
 
 def create_file(token):
     app_id = click.prompt('Instance ID', type=int)
     file_body = click.prompt('File Body')
 
     res = request(
-        'post', '/files/',
+        'post',
+        '/files/',
         json={
-            'app': app_id,
-            'body': file_body,
-            'downloadUrl': 'https://admin.pitcher.com/downloads/Pitcher%20HTML5%20Folder.zip'
+            'app':
+                app_id,
+            'body':
+                file_body,
+            'downloadUrl':
+                'https://admin.pitcher.com/downloads/Pitcher%20HTML5%20Folder.zip'
         },
         token=token
     )
     json = res.json()
 
     if res.status_code != 201:
         if json.get('app'):
```

### Comparing `kudu-0.8/kudu/tests/test_pull.py` & `kudu-0.9/kudu/tests/test_pull.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,48 @@
-from os.path import join, exists
+from os.path import exists, join
 from zipfile import ZipFile
 
 from click.testing import CliRunner
 
 from kudu.__main__ import cli
 from kudu.config import write_config
 
 
-def test_pull_file():
-    runner = CliRunner()
-    with runner.isolated_filesystem():
-        result = runner.invoke(cli, ['pull', '-f', 519629])
-        assert result.exit_code == 0
-        assert exists('index.html')
-        assert exists('thumbnail.png')
-        assert exists(join('folder', 'foobar.json'))
-
-
-def test_pull_project():
-    runner = CliRunner()
-    with runner.isolated_filesystem():
-        write_config({'file_id': 519629})
-        result = runner.invoke(cli, ['pull'])
-        assert result.exit_code == 0
-        assert exists('index.html')
-        assert exists('thumbnail.png')
-        assert exists(join('folder', 'foobar.json'))
-
-
 def test_interface():
     runner = CliRunner()
     with runner.isolated_filesystem():
         write_config({'file_id': 527702})
         result = runner.invoke(cli, ['pull'])
         assert result.exit_code == 0
         assert exists(join('interface', 'index.html'))
         assert exists(join('interface_1', 'index.html'))
         assert exists(join('lang', 'AR.csv'))
 
 
-def test_json_with_path():
+def test_json_path():
     runner = CliRunner()
     with runner.isolated_filesystem():
-        result = runner.invoke(cli, ['pull', '-f', 703251, '-p', 'test.json'])
+        result = runner.invoke(cli, ['pull', '-f', 519631, '-p', 'test.json'])
         assert result.exit_code == 0
         assert exists('test.json')
 
 
-def test_zip_with_path():
+def test_zip():
+    runner = CliRunner()
+    with runner.isolated_filesystem():
+        write_config({'file_id': 519629})
+        result = runner.invoke(cli, ['pull'])
+        assert result.exit_code == 0
+        assert exists('index.html')
+        assert exists('thumbnail.png')
+        assert exists(join('folder', 'foobar.json'))
+
+
+def test_zip_path():
     runner = CliRunner()
     with runner.isolated_filesystem():
-        result = runner.invoke(cli, ['pull', '-f', 527702, '-p', 'test.zip'])
+        result = runner.invoke(cli, ['pull', '-f', 519629, '-p', 'test.zip'])
         assert result.exit_code == 0
         assert exists('test.zip')
 
         zip_file = ZipFile('test.zip')
         assert zip_file.testzip() is None
```

### Comparing `kudu-0.8/kudu/tests/test_link.py` & `kudu-0.9/kudu/tests/test_link.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,18 @@
     runner = CliRunner()
     with runner.isolated_filesystem():
         src = getcwd()
 
         mkdir('interface')
         open(os.path.join('interface', 'test.html'), 'wb').close()
 
-        link.copyfiles(src, dst, link.InterfacePathConverter({'filename': 'interface_xy.zip'}))
+        link.copyfiles(
+            src, dst,
+            link.InterfacePathConverter({'filename': 'interface_xy.zip'})
+        )
         assert os.path.exists(os.path.join(dst, 'interface_xy', 'test.html'))
 
     shutil.rmtree(dst)
 
 
 def test_presentation_path_converter():
     dst = os.path.join(tempfile.gettempdir(), str(time.time()))
@@ -36,36 +39,49 @@
         src = getcwd()
 
         open('index.html', 'wb').close()
         open('thumbnail.png', 'wb').close()
         mkdir('iPadOnly')
         open(os.path.join('iPadOnly', 'iPad.html'), 'wb').close()
 
-        link.copyfiles(src, dst, link.PresentationPathConverter({'filename': '1234_4321.zip'}))
-        assert os.path.exists(os.path.join(dst, 'slides', '1234_4321', 'index.html'))
-        assert os.path.exists(os.path.join(dst, 'slides', '1234_4321', '1234_4321.png'))
-        assert os.path.exists(os.path.join(dst, 'slides', '1234_4321', 'iPad.html'))
+        link.copyfiles(
+            src, dst,
+            link.PresentationPathConverter({'filename': '1234_4321.zip'})
+        )
+        assert os.path.exists(
+            os.path.join(dst, 'slides', '1234_4321', 'index.html')
+        )
+        assert os.path.exists(
+            os.path.join(dst, 'slides', '1234_4321', '1234_4321.png')
+        )
+        assert os.path.exists(
+            os.path.join(dst, 'slides', '1234_4321', 'iPad.html')
+        )
 
     shutil.rmtree(dst)
 
 
 def test_copy_files_event_handler():
     dst = os.path.join(tempfile.gettempdir(), str(time.time()))
     mkdir(dst)
 
     runner = CliRunner()
     with runner.isolated_filesystem():
         src = getcwd()
-        converter = link.PresentationPathConverter({'filename': '1234_4321.zip'})
+        converter = link.PresentationPathConverter({
+            'filename': '1234_4321.zip'
+        })
         event_handler = link.CopyFilesEventHandler(src, dst, converter)
 
         class TestEvent(object):
             event_type = events.EVENT_TYPE_MODIFIED
             src_path = os.path.join(src, 'index.html')
             is_directory = False
 
         open('index.html', 'wb').close()
         event_handler.on_any_event(TestEvent)
 
-        assert os.path.exists(os.path.join(dst, 'slides', '1234_4321', 'index.html'))
+        assert os.path.exists(
+            os.path.join(dst, 'slides', '1234_4321', 'index.html')
+        )
 
     shutil.rmtree(dst)
```

### Comparing `kudu-0.8/README.md` & `kudu-0.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,20 @@
 ## Release History
  - [0.8 (2019-10-29)](#08-2021-01-19)
  - [0.7 (2019-10-29)](#07-2019-10-29)
  - [0.6 (2019-10-28)](#06-2019-10-28)
  - [0.5 (2019-06-17)](#05-2019-06-17)
  - [0.4 (2019-04-29)](#04-2019-04-29)
  - [0.2 (2019-04-29)](#02-2019-04-29)
+
+### 0.9 (2021-03-23)
+- adds push command category rules
+- loosens up install requirements
+- adds OS Independent test matrix
+- moves interface folder based on filename
  
 ### 0.8 (2021-01-19)
 - adds support for iOS UIs
  
 ### 0.7 (2019-10-29)
 - adds path option to pull command
 - downloads into current folder without config file  #4
```

