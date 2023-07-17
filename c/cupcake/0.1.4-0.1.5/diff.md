# Comparing `tmp/cupcake-0.1.4.tar.gz` & `tmp/cupcake-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cupcake-0.1.4.tar", max compression
+gzip compressed data, was "cupcake-0.1.5.tar", max compression
```

## Comparing `cupcake-0.1.4.tar` & `cupcake-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.4/LICENSE
--rw-r--r--   0        0        0      549 2023-04-26 15:54:10.021402 cupcake-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.4/src/cupcake/__init__.py
--rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.4/src/cupcake/cascade.py
--rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.4/src/cupcake/confee.py
--rw-r--r--   0        0        0      650 2023-04-17 16:48:12.052154 cupcake-0.1.4/src/cupcake/data/cmake_file_name.py
--rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.4/src/cupcake/data/new/.gitignore
--rw-r--r--   0        0        0      457 2023-04-17 16:32:26.489411 cupcake-0.1.4/src/cupcake/data/new/CMakeLists.txt
--rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.4/src/cupcake/data/new/conanfile.py
--rw-r--r--   0        0        0      215 2023-04-18 03:25:43.426297 cupcake-0.1.4/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
--rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.4/src/cupcake/data/new/src/lib{{name}}.cpp
--rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.4/src/cupcake/data/new/src/{{name}}.cpp
--rw-r--r--   0        0        0      187 2023-04-17 16:32:36.189898 cupcake-0.1.4/src/cupcake/data/new/tests/CMakeLists.txt
--rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.4/src/cupcake/data/new/tests/{{name}}.cpp
--rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.4/src/cupcake/data/query/CMakeLists.txt
--rw-r--r--   0        0        0    32755 2023-04-26 15:52:37.305011 cupcake-0.1.4/src/cupcake/main.py
--rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.4/src/cupcake/scratch.py
--rw-r--r--   0        0        0     1033 2023-04-26 15:54:47.661366 cupcake-0.1.4/setup.py
--rw-r--r--   0        0        0      578 2023-04-26 15:54:47.661583 cupcake-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      761 2023-03-01 17:58:55.790012 cupcake-0.1.5/LICENSE
+-rw-r--r--   0        0        0      549 2023-07-17 17:47:25.990664 cupcake-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-03-13 22:19:09.065654 cupcake-0.1.5/src/cupcake/__init__.py
+-rw-r--r--   0        0        0     4023 2023-03-13 20:49:00.721516 cupcake-0.1.5/src/cupcake/cascade.py
+-rw-r--r--   0        0        0     2345 2023-03-24 13:54:18.178294 cupcake-0.1.5/src/cupcake/confee.py
+-rw-r--r--   0        0        0      650 2023-04-17 16:48:12.052154 cupcake-0.1.5/src/cupcake/data/cmake_file_name.py
+-rw-r--r--   0        0        0       35 2023-03-08 23:12:26.626449 cupcake-0.1.5/src/cupcake/data/new/.gitignore
+-rw-r--r--   0        0        0      457 2023-04-17 16:32:26.489411 cupcake-0.1.5/src/cupcake/data/new/CMakeLists.txt
+-rw-r--r--   0        0        0     1534 2023-04-04 16:25:50.085034 cupcake-0.1.5/src/cupcake/data/new/conanfile.py
+-rw-r--r--   0        0        0      215 2023-04-18 03:25:43.426297 cupcake-0.1.5/src/cupcake/data/new/include/{{name}}/{{name}}.hpp
+-rw-r--r--   0        0        0       87 2022-04-07 22:23:55.073837 cupcake-0.1.5/src/cupcake/data/new/src/lib{{name}}.cpp
+-rw-r--r--   0        0        0      143 2022-04-07 22:49:53.297481 cupcake-0.1.5/src/cupcake/data/new/src/{{name}}.cpp
+-rw-r--r--   0        0        0      187 2023-04-17 16:32:36.189898 cupcake-0.1.5/src/cupcake/data/new/tests/CMakeLists.txt
+-rw-r--r--   0        0        0      169 2022-04-07 22:20:24.683135 cupcake-0.1.5/src/cupcake/data/new/tests/{{name}}.cpp
+-rw-r--r--   0        0        0      177 2023-03-01 15:12:58.048397 cupcake-0.1.5/src/cupcake/data/query/CMakeLists.txt
+-rw-r--r--   0        0        0    34281 2023-07-17 17:42:08.452480 cupcake-0.1.5/src/cupcake/main.py
+-rw-r--r--   0        0        0     6725 2023-03-08 20:46:34.258683 cupcake-0.1.5/src/cupcake/scratch.py
+-rw-r--r--   0        0        0     1033 2023-07-17 17:47:52.096605 cupcake-0.1.5/setup.py
+-rw-r--r--   0        0        0      578 2023-07-17 17:47:52.096816 cupcake-0.1.5/PKG-INFO
```

### Comparing `cupcake-0.1.4/LICENSE` & `cupcake-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/pyproject.toml` & `cupcake-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cupcake"
-version = "0.1.4"
+version = "0.1.5"
 description = "Make C++ a piece of cake."
 authors = ["John Freeman <jfreeman08@gmail.com>"]
 packages = [{include = "cupcake", from = "src"}]
 
 [tool.poetry.scripts]
 cupcake = 'cupcake.main:main'
```

### Comparing `cupcake-0.1.4/src/cupcake/cascade.py` & `cupcake-0.1.5/src/cupcake/cascade.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/src/cupcake/confee.py` & `cupcake-0.1.5/src/cupcake/confee.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/src/cupcake/data/cmake_file_name.py` & `cupcake-0.1.5/src/cupcake/data/cmake_file_name.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/src/cupcake/data/new/conanfile.py` & `cupcake-0.1.5/src/cupcake/data/new/conanfile.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/src/cupcake/main.py` & `cupcake-0.1.5/src/cupcake/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import pathlib
 import re
 import shlex
 import shutil
 import subprocess
 import sys
 import tempfile
+import time
 import urllib.parse
 
 from cupcake import cascade, confee
 
 def run(command, *args, **kwargs):
     # TODO: Print this in a special color.
     print(' '.join(shlex.quote(str(arg)) for arg in command), flush=True)
@@ -32,15 +33,17 @@
 
 def tee(command, *args, log, **kwargs):
     proc = subprocess.Popen(
         command, *args,
         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, **kwargs
     )
     with open(log, 'wb') as logf:
-        line = ' '.join(shlex.quote(str(arg)) for arg in command).encode()
+        line = ' '.join(shlex.quote(str(arg)) for arg in command)
+        line += '\n'
+        line = line.encode()
         logf.write(line)
         sys.stdout.buffer.write(line)
         for line in proc.stdout:
             logf.write(line)
             sys.stdout.buffer.write(line)
     if proc.wait() != 0:
         raise SystemExit(proc.returncode)
@@ -285,15 +288,15 @@
                         elif not skip:
                             cml_out.write(added_line)
                             mode = MODE_FINISH
                     cml_out.write(line)
             if mode == MODE_INSERT:
                 cml_out.write(added_line)
             elif mode == MODE_FIND:
-                print(f'nowhere to insert call to `find_package` in {cml}')
+                print(f'nowhere to insert call to `find_package` in {self.path}')
                 return
             cml_out.flush()
             shutil.copy(cml_out.name, self.path)
 
 test_template = """
 {{ cmake }} --build {{ cmakeDir }}
 {% if multiConfig %} --config {{ flavor }} {% endif %}
@@ -476,58 +479,89 @@
         if not conanfile_path.exists():
             return
         return conanfile_path
 
     @cascade.command()
     @cascade.option('--profile', help='Name of Conan profile.')
     # TODO: Add option to configure shared linkage.
+    @cascade.option(
+        '-o', 'options',
+        help='Conan options to set. Repeatable.',
+        multiple=True,
+    )
     def conan(
         self,
         source_dir_,
         conanfile_path_,
         build_dir_,
         log_dir_,
         config_,
         CONAN,
         state_,
         flavor_,
         profile,
+        options,
     ):
         """Configure Conan."""
         if not conanfile_path_:
             return
         # TODO: Respect `conan config get general.default_profile`.
         profile = confee.resolve(profile, config_.conan.profile, 'default')
+        # Options are a little unique.
+        # We must start with `config.conan.options` (default `{}`),
+        # override with `options`,
+        # and then write the result to `config.conan.options`.
+        copts = config_.conan.options({})
+        for option in options:
+            match = re.match(r'^([^=]+)(?:=(.+))?$', option)
+            if not match:
+                raise SystemExit(f'bad option: `{option}`')
+            name = match.group(1)
+            value = match.group(2)
+            if value is None:
+                value = 'TRUE'
+            copts[name] = value
+        if copts:
+            config_.conan.options = copts
+        elif config_.conan.options:
+            del config_.conan.options
+
         # TODO: Accept parameter to override settings.
         # TODO: Find path to profile.
         profile_path = pathlib.Path.home() / '.conan/profiles' / profile
         m = hashlib.sha256()
+        # TODO: Separate values with markers to disambiguate.
         m.update(profile_path.read_bytes())
         m.update(conanfile_path_.read_bytes())
+        for name, value in copts.items():
+            m.update(name.encode())
+            m.update(value.encode())
         id = m.hexdigest()
         old_flavors = state_.conan.flavors([])
         new_flavors = list({*config_.flavors([]), flavor_})
         diff_flavors = [f for f in new_flavors if f not in old_flavors]
         conan_dir = build_dir_ / 'conan'
         if state_.conan:
             if state_.conan.id() == id:
                 if not diff_flavors:
                     return state_.conan
             else:
                 shutil.rmtree(conan_dir, ignore_errors=True)
                 diff_flavors = new_flavors
         conan_dir.mkdir(parents=True, exist_ok=True)
-        base_command = [
+        command = [
             CONAN, 'install', source_dir_, '--build', 'missing',
             '--output-folder', conan_dir,
             '--profile:build', profile, '--profile:host', profile,
         ]
+        for option in options:
+            command.extend(['--options', option])
         for flavor in diff_flavors:
             tee(
-                [*base_command, '--settings', f'build_type={FLAVORS[flavor_]}'],
+                [*command, '--settings', f'build_type={FLAVORS[flavor_]}'],
                 log=log_dir_ / 'conan',
                 cwd=conan_dir,
             )
         state_.conan.id = id
         state_.conan.flavors = new_flavors
         # TODO: Find layout. How?
         toolchain = conan_dir / 'conan_toolchain.cmake'
@@ -601,14 +635,16 @@
             if value is None:
                 value = 'TRUE'
             cvars[name] = value
         for name in unvariables:
             cvars.pop(name, None)
         if cvars:
             config_.cmake.variables = cvars
+        elif config_.cmake.variables:
+            del config_.cmake.variables
 
         generator = confee.resolve(generator, config_.cmake.generator, None)
         shared = confee.resolve(shared, config_.cmake.shared, False)
         with_tests = confee.resolve(with_tests, config_.cmake.tests, True)
         prefixes = confee.resolve(prefixes or None, config_.cmake.prefixes, [])
         # TODO: Convenience API for hashing identities.
         m = hashlib.sha256()
@@ -697,22 +733,25 @@
             build_dir_ /= flavor_
         return build_dir_
 
     @cascade.command()
     @cascade.option(
         '--jobs', '-j', help='Maximum number of simultaneous jobs.'
     )
-    def build(self, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs):
+    @cascade.argument('target', required=False)
+    def build(self, CMAKE, build_dir_, log_dir_, cmake_dir_, flavor_, cmake, jobs, target):
         """Build the selected flavor."""
         command = [CMAKE, '--build', cmake_dir_, '--verbose']
         if cmake.multiConfig():
             command.extend(['--config', FLAVORS[flavor_]])
         command.append('--parallel')
         if jobs is not None:
             command.append(jobs)
+        if target is not None:
+            command.extend(['--target', target])
         tee(command, log=log_dir_ / 'build')
         return cmake
 
     @cascade.command()
     @cascade.argument('executable', required=False)
     @cascade.argument('arguments', nargs=-1)
     def exe(self, CMAKE, cmake_dir_, flavor_, cmake, executable, arguments):
@@ -736,28 +775,28 @@
             '--config',
             FLAVORS[flavor_],
             '--prefix',
             prefix_,
         ])
 
     @cascade.command()
-    def test(self, config_, CMAKE, cmake_dir_, flavor_, cmake):
+    def test(self, config_, CMAKE, log_dir_, cmake_dir_, flavor_, cmake):
         """Test the selected flavor."""
         template = confee.resolve(None, config_.scripts.test, test_template)
         template = jinja2.Template(template)
         context = {
             'cmake': CMAKE,
             'cmakeDir': cmake_dir_,
             'multiConfig': cmake.multiConfig(),
             'flavor': FLAVORS[flavor_],
         }
         command = shlex.split(template.render(**context))
         env = os.environ.copy()
         env['CTEST_OUTPUT_ON_FAILURE'] = 'ON'
-        run(command, env=env)
+        tee(command, log=log_dir_ / 'test', env=env)
 
     @cascade.command()
     @cascade.argument('path', required=False, default='.')
     @cascade.option(
         '--name', help='Package name. Default is the directory name.'
     )
     @cascade.option(
@@ -934,8 +973,13 @@
             run([CONAN, 'export', path])
 
     @cascade.command()
     def clean(self, build_dir_path_):
         """Remove the build directory."""
         shutil.rmtree(build_dir_path_, ignore_errors=True)
 
+start = time.time()
 Cupcake()
+raise SystemExit("bye")
+print("hello")
+finish = time.time()
+print(f"{finish - start}s")
```

### Comparing `cupcake-0.1.4/src/cupcake/scratch.py` & `cupcake-0.1.5/src/cupcake/scratch.py`

 * *Files identical despite different names*

### Comparing `cupcake-0.1.4/setup.py` & `cupcake-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
  'tomlkit>=0.10.1,<0.11.0']
 
 entry_points = \
 {'console_scripts': ['cupcake = cupcake.main:main']}
 
 setup_kwargs = {
     'name': 'cupcake',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Make C++ a piece of cake.',
     'long_description': None,
     'author': 'John Freeman',
     'author_email': 'jfreeman08@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `cupcake-0.1.4/PKG-INFO` & `cupcake-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cupcake
-Version: 0.1.4
+Version: 0.1.5
 Summary: Make C++ a piece of cake.
 Author: John Freeman
 Author-email: jfreeman08@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
```

