# Comparing `tmp/mama-0.7.9.tar.gz` & `tmp/mama-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mama-0.7.9.tar", last modified: Mon Feb 13 15:33:31 2023, max compression
+gzip compressed data, was "mama-0.8.0.tar", last modified: Mon Jul 17 21:31:56 2023, max compression
```

## Comparing `mama-0.7.9.tar` & `mama-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2023-01-17 13:35:55.000000 mama-0.7.9/LICENSE
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-13 15:33:31.315010 mama-0.7.9/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11098 2023-02-08 12:22:13.000000 mama-0.7.9/README.md
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/
--rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2023-01-17 13:35:55.000000 mama-0.7.9/mama/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12341 2023-02-09 15:58:10.000000 mama-0.7.9/mama/artifactory.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    34198 2023-02-09 14:32:53.000000 mama-0.7.9/mama/build_config.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    19930 2023-02-13 10:05:48.000000 mama-0.7.9/mama/build_dependency.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    48418 2023-02-09 12:33:47.000000 mama-0.7.9/mama/build_target.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    12118 2023-02-09 14:04:24.000000 mama-0.7.9/mama/cmake_configure.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    13149 2023-01-30 22:00:52.000000 mama-0.7.9/mama/dependency_chain.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2023-01-17 13:35:55.000000 mama-0.7.9/mama/init_project.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10595 2023-02-09 13:58:46.000000 mama-0.7.9/mama/main.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2023-01-17 13:35:55.000000 mama-0.7.9/mama/msbuild.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     7023 2023-01-17 13:35:55.000000 mama-0.7.9/mama/package.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     6781 2023-01-30 15:22:01.000000 mama-0.7.9/mama/papa_deploy.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-18 13:01:37.000000 mama-0.7.9/mama/parse_mamafile.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/platforms/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-09 13:03:03.000000 mama-0.7.9/mama/platforms/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     3880 2023-02-09 15:04:34.000000 mama-0.7.9/mama/platforms/oclea.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/types/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-30 15:17:16.000000 mama-0.7.9/mama/types/artifactory_pkg.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/asset.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-30 22:10:20.000000 mama-0.7.9/mama/types/dep_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    10157 2023-02-09 11:39:01.000000 mama-0.7.9/mama/types/git.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2023-01-17 13:35:55.000000 mama-0.7.9/mama/types/local_source.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)    15125 2023-02-13 15:30:38.000000 mama-0.7.9/mama/util.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama/utils/
--rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-01-17 13:35:55.000000 mama-0.7.9/mama/utils/__init__.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2023-01-17 13:35:55.000000 mama-0.7.9/mama/utils/nonblocking_io.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     5739 2023-01-30 15:55:08.000000 mama-0.7.9/mama/utils/sub_process.py
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1221 2023-01-30 19:27:23.000000 mama-0.7.9/mama/utils/system.py
-drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-02-13 15:33:31.315010 mama-0.7.9/mama.egg-info/
--rw-r--r--   0 jorma     (1000) jorma     (1000)    11908 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/PKG-INFO
--rw-r--r--   0 jorma     (1000) jorma     (1000)      770 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/SOURCES.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/dependency_links.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/entry_points.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)       44 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/requires.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-02-13 15:33:31.000000 mama-0.7.9/mama.egg-info/top_level.txt
--rw-r--r--   0 jorma     (1000) jorma     (1000)     1127 2023-02-13 10:05:09.000000 mama-0.7.9/pyproject.toml
--rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-02-13 15:33:31.315010 mama-0.7.9/setup.cfg
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1062 2022-10-15 13:42:02.000000 mama-0.8.0/LICENSE
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-17 21:31:56.420707 mama-0.8.0/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11354 2023-07-17 21:28:34.000000 mama-0.8.0/README.md
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      141 2022-10-15 12:52:32.000000 mama-0.8.0/mama/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12572 2023-03-08 20:41:13.000000 mama-0.8.0/mama/artifactory.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    38745 2023-07-17 19:15:48.000000 mama-0.8.0/mama/build_config.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    23348 2023-07-14 21:51:07.000000 mama-0.8.0/mama/build_dependency.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    51121 2023-07-17 21:14:34.000000 mama-0.8.0/mama/build_target.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    13639 2023-07-17 13:34:28.000000 mama-0.8.0/mama/cmake_configure.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    14557 2023-07-17 12:51:12.000000 mama-0.8.0/mama/dependency_chain.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     5368 2022-10-14 21:28:27.000000 mama-0.8.0/mama/init_project.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    11372 2023-07-17 12:54:02.000000 mama-0.8.0/mama/main.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1796 2022-10-14 21:35:20.000000 mama-0.8.0/mama/msbuild.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     7828 2023-04-07 22:30:06.000000 mama-0.8.0/mama/package.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     6773 2023-03-08 20:52:02.000000 mama-0.8.0/mama/papa_deploy.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1732 2023-01-31 19:23:36.000000 mama-0.8.0/mama/parse_mamafile.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/platforms/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2023-02-10 12:13:25.000000 mama-0.8.0/mama/platforms/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     3348 2023-07-17 21:12:25.000000 mama-0.8.0/mama/platforms/mips.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     4765 2023-07-17 19:14:06.000000 mama-0.8.0/mama/platforms/oclea.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/types/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:55.000000 mama-0.8.0/mama/types/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1051 2023-01-31 19:23:36.000000 mama-0.8.0/mama/types/artifactory_pkg.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      789 2022-10-13 07:46:30.000000 mama-0.8.0/mama/types/asset.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      830 2023-01-31 19:23:36.000000 mama-0.8.0/mama/types/dep_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12615 2023-07-14 21:38:06.000000 mama-0.8.0/mama/types/git.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1065 2022-10-13 16:33:15.000000 mama-0.8.0/mama/types/local_source.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    15666 2023-05-09 09:22:21.000000 mama-0.8.0/mama/util.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama/utils/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        0 2022-10-14 22:47:54.000000 mama-0.8.0/mama/utils/__init__.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1038 2022-10-14 18:37:11.000000 mama-0.8.0/mama/utils/nonblocking_io.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     9784 2023-04-09 16:20:29.000000 mama-0.8.0/mama/utils/sub_process.py
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1439 2023-03-06 14:41:17.000000 mama-0.8.0/mama/utils/system.py
+drwxr-xr-x   0 jorma     (1000) jorma     (1000)        0 2023-07-17 21:31:56.420707 mama-0.8.0/mama.egg-info/
+-rw-r--r--   0 jorma     (1000) jorma     (1000)    12164 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/PKG-INFO
+-rw-r--r--   0 jorma     (1000) jorma     (1000)      793 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/SOURCES.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        1 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/dependency_links.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       40 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/entry_points.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       76 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/requires.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)        5 2023-07-17 21:31:56.000000 mama-0.8.0/mama.egg-info/top_level.txt
+-rw-r--r--   0 jorma     (1000) jorma     (1000)     1180 2023-07-17 21:29:07.000000 mama-0.8.0/pyproject.toml
+-rw-r--r--   0 jorma     (1000) jorma     (1000)       38 2023-07-17 21:31:56.420707 mama-0.8.0/setup.cfg
```

### Comparing `mama-0.7.9/LICENSE` & `mama-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/PKG-INFO` & `mama-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mama
-Version: 0.7.9
+Version: 0.8.0
 Summary: A modular C++ build tool even your mama can use
 Author-email: Jorma Rebane <jorma.rebane@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/RedFox20/Mama
 Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
 Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
 Classifier: Development Status :: 3 - Alpha
@@ -39,29 +39,30 @@
 private git repositories. Package versioning is done through git tags or branches.
 
 Custom build systems are also supported. For additional documentation explore: [build_target.py](mama/build_target.py)
 
 
 ## Who is this FOR?
 Anyone who develops cross-platform C++ libraries or applications which
-target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea].
+target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea, MIPS].
 And anyone who is not satisfied with system-wide dependencies and linker
 bugs caused by incompatible system-wide libraries on Linux.
 
 If you require an easy to use, reproducible project/namespace scoped package+build system, this is for you.
 Your builds will not rely on hard to setup system packages, all you need to do is type `mama build`.
 
 ### Supported platforms ###
-- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7)
-- Linux (Ubuntu) (64-bit x86_64, 32-bit x86)
-- MacOS (64-bit x86_64, 64-bit arm64)
-- iOS (64-bit arm64)
-- Android (64-bit arm64, 32-bit armv7)
-- Raspberry (32-bit armv7)
-- Oclea (64-bit arm64)
+- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7) default is latest MSVC
+- Linux (Ubuntu) (64-bit x86_64, 32-bit x86) both GCC and Clang
+- MacOS (64-bit x86_64, 64-bit arm64) via config.macos_version
+- iOS (64-bit arm64) via config.ios_version
+- Android (64-bit arm64, 32-bit armv7) via env ANDROID_HOME
+- Raspberry (32-bit armv7) via env RASPI_HOME
+- Oclea (64-bit arm64) via config.set_oclea_toolchain()
+- MIPS (mips mipsel, mips64, mips64el) via config.set_mips_toolchain()
 
 ## Who is this NOT for?
 Single platform projects with platform specific build configuration and system wide dependency management
 such as Linux exclusive G++ projects using apt-get libraries or iOS-only apps using cocoapods.
 
 
 ## Artifactory
@@ -254,15 +255,15 @@
 The package `setuptools>=65.0` is required, ensure the version is correct with `pip3 show setuptools`.
 
 You can set up local development with `$ pip3 install -e . --no-cache-dir` but make sure you have latest setuptools (>65.0) and latest pip3 (>22.3). This command will fail with older toolkits.
 
 Uploading a source distributionP:
 1. Get dependencies: `pip3 install build twine`
 2. Build sdist: `python -m build`
-3. Upload with twine: `twine upload dist/*`
+3. Upload with twine: `twine upload --skip-existing dist/*`
 It will prompt for Username and Password, unless you set up ~/.pypirc file:
 ```
 [distutils]
 index-servers = pypi
 [pypi]
 username=<your-mama-pypi-username>
 password=<your-mama-pypi-password>
```

### Comparing `mama-0.7.9/README.md` & `mama-0.8.0/mama.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+Metadata-Version: 2.1
+Name: mama
+Version: 0.8.0
+Summary: A modular C++ build tool even your mama can use
+Author-email: Jorma Rebane <jorma.rebane@gmail.com>
+License: MIT
+Project-URL: Homepage, https://github.com/RedFox20/Mama
+Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
+Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Mama Build Tool
 Mama - A modular C++ build tool even your mama can use
 
 The main goal of this project is to provide extremely convenient in-source builds
 for cross platform projects. Building is as simple as `mama build windows` - no ceremony~!
 
 CMake projects with trivial configurations and no dependencies can be handled
@@ -19,29 +39,30 @@
 private git repositories. Package versioning is done through git tags or branches.
 
 Custom build systems are also supported. For additional documentation explore: [build_target.py](mama/build_target.py)
 
 
 ## Who is this FOR?
 Anyone who develops cross-platform C++ libraries or applications which
-target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea].
+target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea, MIPS].
 And anyone who is not satisfied with system-wide dependencies and linker
 bugs caused by incompatible system-wide libraries on Linux.
 
 If you require an easy to use, reproducible project/namespace scoped package+build system, this is for you.
 Your builds will not rely on hard to setup system packages, all you need to do is type `mama build`.
 
 ### Supported platforms ###
-- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7)
-- Linux (Ubuntu) (64-bit x86_64, 32-bit x86)
-- MacOS (64-bit x86_64, 64-bit arm64)
-- iOS (64-bit arm64)
-- Android (64-bit arm64, 32-bit armv7)
-- Raspberry (32-bit armv7)
-- Oclea (64-bit arm64)
+- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7) default is latest MSVC
+- Linux (Ubuntu) (64-bit x86_64, 32-bit x86) both GCC and Clang
+- MacOS (64-bit x86_64, 64-bit arm64) via config.macos_version
+- iOS (64-bit arm64) via config.ios_version
+- Android (64-bit arm64, 32-bit armv7) via env ANDROID_HOME
+- Raspberry (32-bit armv7) via env RASPI_HOME
+- Oclea (64-bit arm64) via config.set_oclea_toolchain()
+- MIPS (mips mipsel, mips64, mips64el) via config.set_mips_toolchain()
 
 ## Who is this NOT for?
 Single platform projects with platform specific build configuration and system wide dependency management
 such as Linux exclusive G++ projects using apt-get libraries or iOS-only apps using cocoapods.
 
 
 ## Artifactory
@@ -234,15 +255,15 @@
 The package `setuptools>=65.0` is required, ensure the version is correct with `pip3 show setuptools`.
 
 You can set up local development with `$ pip3 install -e . --no-cache-dir` but make sure you have latest setuptools (>65.0) and latest pip3 (>22.3). This command will fail with older toolkits.
 
 Uploading a source distributionP:
 1. Get dependencies: `pip3 install build twine`
 2. Build sdist: `python -m build`
-3. Upload with twine: `twine upload dist/*`
+3. Upload with twine: `twine upload --skip-existing dist/*`
 It will prompt for Username and Password, unless you set up ~/.pypirc file:
 ```
 [distutils]
 index-servers = pypi
 [pypi]
 username=<your-mama-pypi-username>
 password=<your-mama-pypi-password>
```

### Comparing `mama-0.7.9/mama/artifactory.py` & `mama-0.8.0/mama/artifactory.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,20 +46,20 @@
         git:Git = p
         version = git.get_commit_hash(target.dep)
         if not version:
             return None # nothing to do at this point
 
     name = target.name
     # triplets information to make this package platform unique
-    platform = target.config.name() # eg 'windows', 'linux', 'oclea'
+    platform, os_major, os_minor = target.config.get_distro_info()
     compiler = target.config.compiler_version()
     arch = target.config.arch # eg 'x86', 'arm64'
     build_type = 'release' if target.config.release else 'debug'
 
-    return f'{name}-{platform}-{compiler}-{arch}-{build_type}-{version}'
+    return f'{name}-{platform}-{os_major}-{compiler}-{arch}-{build_type}-{version}'
 
 
 keyr = None
 def _get_keyring():
     global keyr
     if not keyr: # lazy init keyring, because it loads certs and other slow stuff
         import keyring
@@ -124,15 +124,15 @@
         except ftplib.Error as e:
             console(f'artifactory login failed: {e}')
             _remove_artifactory_ftp_credentials(url)
         else:
             return # success
 
 
-def artifactory_sanitize_url(url):
+def artifactory_sanitize_url(url: str):
     return url.replace('ftp://', '').replace('http://','').replace('https://','')
 
 
 def artifactory_upload(ftp:ftplib.FTP_TLS, target_name:str, file_path:str):
     size = os.path.getsize(file_path)
     transferred = 0
     lastpercent = 0
@@ -245,21 +245,21 @@
     if target.dep.dep_source.is_git:
         git: Git = target.dep.dep_source
         git.save_status(target.dep)
 
     return (True, dependencies)
 
 
-def _fetch_package(target:BuildTarget, url, archive, build_dir):
+def _fetch_package(target:BuildTarget, url, archive, cache_dir):
     remote_file = f'http://{url}/{target.name}/{archive}.zip'
     try:
-        return download_file(remote_file, build_dir, force=True, 
+        return download_file(remote_file, cache_dir, force=True, 
                              message=f'    Artifactory fetch {url}/{archive} ')
     except Exception as e:
-        if target.config.verbose:
+        if target.config.verbose or target.config.force_artifactory:
             error(f'    Artifactory fetch failed with {e} {url}/{archive}.zip')
 
         d:DepSource = target.dep.dep_source
         # this is an artifactory pkg, so the url MUST exist
         if d.is_pkg:
             raise RuntimeError(f'Artifactory package {d} did not exist at {url}')
 
@@ -271,18 +271,18 @@
                 if target.config.verbose:
                     error(f'    Resetting Git status file: {target.name}')
                 d.reset_status(target.dep)
 
         return None
 
 
-def unzip_and_load_target(target:BuildTarget, local_file:str, build_dir:str) -> Tuple[bool, list]:
-    success, num_extracted = try_unzip(local_file, build_dir)
+def unzip_and_load_target(target:BuildTarget, local_file:str) -> Tuple[bool, list]:
+    success, num_extracted = try_unzip(local_file, target.dep.build_dir)
     if success:
-        return artifactory_load_target(target, build_dir, num_files_copied = num_extracted)
+        return artifactory_load_target(target, target.dep.build_dir, num_files_copied = num_extracted)
     else:
         error(f'    Artifactory unzip failed, possibly corrupt package {local_file}')
         os.remove(local_file) # it's probably corrupted
         return (False, None)
 
 
 def artifactory_fetch_and_reconfigure(target:BuildTarget) -> Tuple[bool, list]:
@@ -293,26 +293,27 @@
     url = target.config.artifactory_ftp
     if not url:
         return (False, None)
 
     archive = artifactory_archive_name(target)
     if not archive:
         return (False, None)
+    
+    cache_dir = target.dep.dep_dir #target.dep.workspace
+    local_file = normalized_join(cache_dir, f'{archive}.zip')
 
-    url = artifactory_sanitize_url(url)
-    build_dir = target.build_dir()
-    local_file = normalized_join(build_dir, f'{archive}.zip')
-
-    if os.path.exists(local_file):
+    # cache is normally used, however `mama update` will ignore the cache and re-downloads the latest
+    if os.path.exists(local_file) and not (target.config.update and target.is_current_target()):
         if (target.is_current_target() or target.config.no_specific_target()) \
-            and not target.test:
+            and not target.config.test:
             console(f'    Artifactory cache {local_file}')
-        success, deps = unzip_and_load_target(target, local_file, build_dir)
+        success, deps = unzip_and_load_target(target, local_file)
         if success: return (success, deps)
 
     # use mama verbose to show the failure msgs
-    local_file = _fetch_package(target, url, archive, build_dir)
+    url = artifactory_sanitize_url(url)
+    local_file = _fetch_package(target, url, archive, cache_dir)
     if not local_file:
         return (False, None)
     console(f'    Artifactory unzip {archive}')
-    return unzip_and_load_target(target, local_file, build_dir)
+    return unzip_and_load_target(target, local_file)
```

### Comparing `mama-0.7.9/mama/build_config.py` & `mama-0.8.0/mama/build_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-import os, sys, multiprocessing, tempfile
+import os, sys, tempfile, platform, psutil
 from mama.platforms.oclea import Oclea
+from mama.platforms.mips import Mips
 import mama.util as util
 from .utils.system import System, console
 from .utils.sub_process import execute, execute_piped
 
 if System.linux:
     import distro
 
@@ -22,28 +23,33 @@
         self.update  = False
         self.deploy  = False
         # if root mamafile has defined an artifacts URL
         # this will upload deploy archive through SFTP
         self.upload  = False
         # currently for uploads only, uploads only if package already not uploaded
         self.if_needed = False
+        # if `art` is specified, then artifactory download is mandatory, no source builds are done
+        self.force_artifactory = False
+        # if `noart` is specified, then artifactory is temporarily ignored
+        self.disable_artifactory = False
         self.reclone   = False
         self.mama_init = False
         self.print     = True
         self.verbose   = False
         self.test      = ''
         self.start     = ''
         # supported platforms
         self.windows = False
         self.linux   = False
         self.macos   = False
         self.ios     = False
         self.android = False
         self.raspi   = False
         self.oclea : Oclea = None
+        self.mips : Mips = None
         # compilers
         self.clang = True # prefer clang on linux
         self.gcc   = False
         self.clang_path = ''
         self.gcc_path = ''
         # can be used to overide C and C++ compiler paths
         self.cc_path = ''
@@ -54,15 +60,16 @@
         self.compiler_cmd = False
         self.fortran = ''
         # build optimization
         self.release = True
         self.debug   = False
         # valid architectures: x86, x64, arm, arm64
         self.arch    = None
-        self.jobs    = multiprocessing.cpu_count()
+        self.distro  = None  # distro information (name, major, minor)
+        self.jobs    = psutil.cpu_count()
         self.target  = None
         self.flags   = None
         self.open    = None
         # use this to customize ios sdk version
         self.ios_version   = '16.0' # 16: ios 16
         # use this to customize macos sdk version
         self.macos_version = '13.0' # 13: macos 13
@@ -106,14 +113,16 @@
             elif arg == 'build':     self.build   = True
             elif arg == 'clean':     self.clean   = True
             elif arg == 'rebuild':   self.rebuild = True
             elif arg == 'update':    self.update  = True
             elif arg == 'deploy':    self.deploy  = True
             elif arg == 'upload':    self.upload  = True
             elif arg == 'if_needed': self.if_needed = True
+            elif arg == 'art':       self.force_artifactory = True
+            elif arg == 'noart':     self.disable_artifactory = True
             # Updates, Builds and Deploys the project as a package
             elif arg == 'serve':
                 self.build = True
                 self.update = True
                 self.deploy = True
             elif arg == 'reclone':
                 console('WARNING: Argument `reclone` is deprecated, use `wipe` instead.')
@@ -129,14 +138,15 @@
             elif arg == 'windows': self.set_platform(windows=True)
             elif arg == 'linux':   self.set_platform(linux=True)
             elif arg == 'macos':   self.set_platform(macos=True)
             elif arg == 'ios':     self.set_platform(ios=True)
             elif arg == 'android': self.set_platform(android=True)
             elif arg == 'raspi':   self.set_platform(raspi=True)
             elif arg == 'oclea':   self.set_platform(oclea=True)
+            elif arg == 'mips':    self.set_platform(mips=True)
             elif arg == 'x86':     self.set_arch('x86')
             elif arg == 'x64':     self.set_arch('x64')
             elif arg == 'arm':     self.set_arch('arm')
             elif arg == 'arm64':   self.set_arch('arm64')
             elif arg == 'aarch64': 
                 console('warning: aarch64 is the same as arm64, setting to arm64')
                 self.set_arch('arm64')
@@ -194,29 +204,48 @@
             arg = ' '.join(arg.split(','))
         if not args:
             return arg
         return args + ' ' + arg
 
 
     def set_platform(self, windows=False, linux=False, macos=False, \
-                           ios=False, android=False, raspi=False, oclea=False):
-        self.windows = windows
-        self.linux   = linux
-        self.macos   = macos
-        self.ios     = ios
-        self.android = android
-        self.raspi   = raspi
-        if not oclea: self.oclea = None
-        elif not self.oclea: self.oclea = Oclea(self)
+                           ios=False, android=False, raspi=False, \
+                           oclea=False, mips=False):
+        """ Ensures only a single platform is set """
+        platforms = [False]*8
+        if windows: platforms[0] = True
+        elif linux:  platforms[1] = True
+        elif macos:  platforms[2] = True
+        elif ios:    platforms[3] = True
+        elif android: platforms[4] = True
+        elif raspi: platforms[5] = True
+        elif oclea: platforms[6] = True
+        elif mips: platforms[7] = True
+
+        def get_new_value(old_value, enable, type=None):
+            if old_value and not enable:
+                return None if type else False
+            if enable and not old_value:
+                return type(self) if type else True
+            return old_value
+        self.windows = get_new_value(self.windows, platforms[0])
+        self.linux   = get_new_value(self.linux,   platforms[1])
+        self.macos   = get_new_value(self.macos,   platforms[2])
+        self.ios     = get_new_value(self.ios,     platforms[3])
+        self.android = get_new_value(self.android, platforms[4])
+        self.raspi   = get_new_value(self.raspi,   platforms[5])
+        self.oclea   = get_new_value(self.oclea,   platforms[6], Oclea)
+        self.mips    = get_new_value(self.mips,    platforms[7], Mips)
         return True
 
 
     def is_platform_set(self):
         return self.windows or self.linux or self.macos \
-            or self.ios or self.android or self.raspi or self.oclea
+            or self.ios or self.android or self.raspi \
+            or self.oclea or self.mips
 
 
     def check_platform(self):
         if not self.is_platform_set():
             self.set_platform(windows=System.windows, linux=System.linux, macos=System.macos)
             if not self.is_platform_set():
                 raise RuntimeError(f'Unsupported platform {sys.platform}: Please specify platform!')
@@ -225,30 +254,71 @@
         if not self.arch:
             # macos has now moved to arm64 starting with M1 series chips
             if self.macos:        self.set_arch('arm64')
             elif self.ios:        self.set_arch('arm64')
             elif self.android:    self.set_arch('arm64')
             elif self.raspi:      self.set_arch('arm')
             elif self.oclea:      self.set_arch('arm64')
+            elif self.mips:       self.set_arch(self.mips.mips_arch)
             elif System.is_64bit: self.set_arch('x64')
             else:                 self.set_arch('x86')
 
         # Arch itself is validated in set_arch(), 
         # however we need to validate if arch is allowed on platform
         if self.arch:
             if self.linux and 'arm' in self.arch:
                 raise RuntimeError(f'Unsupported arch={self.arch} on linux platform! Build with android instead')
             if self.raspi and self.arch != 'arm':
                 raise RuntimeError(f'Unsupported arch={self.arch} on raspi platform! Supported=arm')
             if self.oclea and self.arch != 'arm64':
                 raise RuntimeError(f'Unsupported arch={self.arch} on Oclea platform! Supported=arm64')
+            if self.mips and self.arch not in self.mips.supported_arches:
+                raise RuntimeError(f'Unsupported arch={self.arch} on MIPS platform! Supported={self.mips.supported_arches}')
+
+
+    def get_distro_info(self):
+        if self.distro:
+            return self.distro
+        if self.windows:
+            version = platform.version().split('.') + ['0']
+            self.distro = (self.name(), int(version[0]), int(version[1]))
+        elif self.macos:
+            version = self.macos_version.split('.') + ['0']
+            self.distro = (self.name(), int(version[0]), int(version[1]))
+        elif self.ios:
+            version = self.ios_version.split('.') + ['0']
+            self.distro = (self.name(), int(version[0]), int(version[1]))
+        elif self.android:
+            version = self.android_api.split('-')[1]
+            self.distro = (self.name(), int(version), 0)
+        elif self.raspi:
+            # TODO: RASPI version
+            self.distro = (self.name(), 0, 0)
+        elif self.oclea:
+            # TODO: OCLEA version
+            self.distro = (self.name(), 0, 0)
+        elif self.mips:
+            # TODO: MIPS version
+            self.distro = (self.name(), 0, 0)
+        elif self.linux:
+            try:
+                dist = distro.info()
+                major = int(dist['version_parts']['major'])
+                minor = int(dist['version_parts']['minor'])
+                self.distro = (dist['id'], major, minor)
+            except Exception as err:
+                console(f'Failed to parse linux distro; falling back to Ubuntu 16.04 LTS: {err}', color='red')
+                self.distro = ('ubuntu', 16, 4)
+        else:
+            self.distro = (platform.system().lower(), int(platform.release()), 0)
+        return self.distro
 
 
     def set_arch(self, arch):
-        arches = ['x86', 'x64', 'arm', 'arm64']
+        arches = ['x86', 'x64', 'arm', 'arm64', 'mips', 'mipsel', 'mips64', 'mips64el']
         if not arch in arches:
             raise RuntimeError(f"Unrecognized architecture {arch}! Valid options are: {arches}")
         self.arch = arch
 
 
     def is_64bit_build(self):
         return (self.arch == 'x64' or self.arch == 'arm64')
@@ -258,14 +328,15 @@
         if self.windows: return 'windows'
         if self.linux:   return 'linux'
         if self.macos:   return 'macos'
         if self.ios:     return 'ios'
         if self.android: return 'android'
         if self.raspi:   return 'raspi'
         if self.oclea:   return 'oclea'
+        if self.mips:    return 'mips'
         return 'build'
 
 
     ## These are the hard references to all build directory variations
     ## All parts of the codebase should use these, instead of raw strings
     ## This will avoid accidental mismatches
     def build_dir_win64(self): return 'windows'
@@ -277,14 +348,15 @@
     def build_dir_macosarm64(self): return 'macosarm' # arm64
     def build_dir_macos64(self): return 'macos' # x64
     def build_dir_ios(self): return 'ios' # arm64
     def build_dir_android64(self): return 'android'
     def build_dir_android32(self): return 'android32'
     def build_dir_raspi32(self): return 'raspi'
     def build_dir_oclea64(self): return 'oclea'
+    def build_dir_mips(self): return 'mips'
     def build_dir_default(self): return 'build'
 
 
     def platform_build_dir_name(self):
         """
         Gets the build folder name depending on platform and architecture.
         By default 64-bit architectures use the platform name, eg 'windows' or 'linux'
@@ -306,24 +378,26 @@
         if self.ios: # Apple dropped 32-bit support
             return self.build_dir_ios()
         if self.android:
             if self.is_target_arch_arm64(): return self.build_dir_android64()
             return self.build_dir_android32()
         if self.raspi: return self.build_dir_raspi32()  # Only 32-bit raspi
         if self.oclea: return self.build_dir_oclea64()  # Only 64-bit oclea aarch64 (arm64)
+        if self.mips: return self.build_dir_mips()
+
         return self.build_dir_default()
 
 
     def set_build_config(self, release=False, debug=False):
         self.release = release
         self.debug   = debug
         return True
 
 
-    def set_artifactory_ftp(self, ftp_url, auth='store'):
+    def set_artifactory_ftp(self, ftp_url: str, auth='store'):
         """ @see BuildTarget.set_artifactory_ftp() for documentation """
         self.artifactory_ftp = ftp_url
         self.artifactory_auth = auth
 
 
     def prefer_clang(self, target_name):
         if not self.linux or self.raspi or self.clang: return
@@ -358,32 +432,36 @@
     def enable_fortran(self, path=''):
         if self.fortran: return
         self.fortran = path if path else self.find_default_fortran_compiler()
 
 
     # returns: root path where the compilers exist and the discovered suffix
     #          (root_path, suffix)
-    def find_compiler_root(self, suggested_path, compiler, suffixes):
+    def find_compiler_root(self, suggested_path, compiler, suffixes, dumpfullversion):
         roots = []
         if suggested_path: roots.append(suggested_path)
         roots += ['/etc/alternatives/', '/usr/bin/', '/usr/local/bin/', '/bin/']
         candidates = []
         for root in roots:
             for suffix in suffixes:
                 cc_path = root + compiler + suffix
                 if os.path.exists(cc_path):
-                    version = self._get_gcc_clang_fullversion(cc_path) # eg 9.4.0
+                    version = self._get_gcc_clang_fullversion(cc_path, dumpfullversion) # eg 9.4.0
+                    if self.verbose: console(f'Compiler {cc_path} version: {version}')
                     candidates.append((root, suffix, version))
         if not candidates:
             raise EnvironmentError(f'Could not find {compiler} from {roots} with any suffix {suffixes}')
 
         def version_to_int(version_str):
             major_minor_patch = version_str.split('.')
             integer = 0
-            for part in major_minor_patch: integer = integer*10 + int(part)
+            for part in major_minor_patch:
+                integer = integer*10 + int(part) if part else integer
+            if integer == 0:
+                console(f"Failed to check version for candidate='{version_str}'")
             return integer
 
         # sort by version, descending eg 10.3, 9.4, 8.3
         candidates.sort(key=lambda x: version_to_int(x[2]), reverse=True)
 
         # print this out for debugging on CI machines if they select verbose
         if self.verbose:
@@ -395,56 +473,71 @@
             console(f'==> Selected {compiler+suffix} ({version}) at {root+compiler+suffix} <==')
         return root, suffix, version
 
 
     def get_preferred_compiler_paths(self):
         if self.cc_path and self.cxx_path and self.cxx_version:
             return (self.cc_path, self.cxx_path, self.cxx_version)
+
+        # no preferred cc path for MSVC
+        if self.windows:
+            return (self.cc_path, self.cxx_path, self.cxx_version)
+
         if self.raspi:  # only GCC available for this platform
             ext = '.exe' if System.windows else ''
             self.cc_path  = f'{self.raspi_bin()}arm-linux-gnueabihf-gcc{ext}'
             self.cxx_path = f'{self.raspi_bin()}arm-linux-gnueabihf-g++{ext}'
-            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path)
+            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path, dumpfullversion=True)
         elif self.oclea:
             self.cc_path  = f'{self.oclea.bin()}aarch64-oclea-linux-gcc'
             self.cxx_path = f'{self.oclea.bin()}aarch64-oclea-linux-g++'
-            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path)
+            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path, dumpfullversion=True)
+        elif self.mips:
+            self.cc_path  = f'{self.mips.compiler_prefix()}gcc'
+            self.cxx_path = f'{self.mips.compiler_prefix()}g++'
+            self.cxx_version = self._get_gcc_clang_fullversion(self.cc_path, dumpfullversion=True)
         elif self.clang:
             suffixes = ['-12','-11','-10','-9','-8','-7','-6','']
-            self.clang_path, suffix, ver = self.find_compiler_root(self.clang_path, 'clang++', suffixes)
+            self.clang_path, suffix, ver = self.find_compiler_root(self.clang_path, 'clang++', suffixes, dumpfullversion=False)
             self.cc_path = f'{self.clang_path}clang{suffix}'
             self.cxx_path = f'{self.clang_path}clang++{suffix}'
             self.cxx_version = ver
         elif self.gcc:
             suffixes = ['-11','-10','-9','-8','-7','-6','']
-            self.gcc_path, suffix, ver = self.find_compiler_root(self.gcc_path, 'g++', suffixes)
+            self.gcc_path, suffix, ver = self.find_compiler_root(self.gcc_path, 'g++', suffixes, dumpfullversion=True)
             self.cc_path = f'{self.gcc_path}gcc{suffix}'
             self.cxx_path = f'{self.gcc_path}g++{suffix}'
             self.cxx_version = ver
 
         if self.cc_path and self.cxx_path and self.cxx_version:
             return (self.cc_path, self.cxx_path, self.cxx_version)
 
         raise EnvironmentError('No preferred compiler for this platform!')
 
 
-    def _get_gcc_clang_fullversion(self, cc_path):
-        return execute_piped(f'{cc_path} -dumpfullversion').strip() # eg 9.4.0
+    def _get_gcc_clang_fullversion(self, cc_path, dumpfullversion):
+        if dumpfullversion:
+            version = execute_piped(f'{cc_path} -dumpfullversion').strip() # eg 9.4.0
+            if version.count('.') >= 1:
+                return version
+        # clang++ doesn't support -dumpfullversion in latest releases -_-
+        return execute_piped(f'{cc_path} -dumpversion').strip()
 
 
     def compiler_version(self):
         if self.windows:
             msvc_tools = self.get_msvc_tools_path()
             version = os.path.basename(msvc_tools.rstrip('\\//')).split('.')[0]
             return f'msvc{version}'
-        elif self.linux or self.raspi or self.oclea:
+        elif self.linux or self.raspi or self.oclea or self.mips:
             cc, _, version = self.get_preferred_compiler_paths()
-            major_version = version.split('.')[0]
-            if 'gcc' in cc: return f'gcc{major_version}'
-            if 'clang' in cc: return f'clang{major_version}'
+            version_parts = version.split('.')
+            major_version, minor_version = version_parts[0], version_parts[1]
+            if 'gcc' in cc: return f'gcc{major_version}.{minor_version}'
+            if 'clang' in cc: return f'clang{major_version}.{minor_version}'
             raise EnvironmentError(f'Unrecognized compiler {cc}!')
         elif self.macos:
             return self.macos_version
         elif self.ios:
             return self.ios_version
         elif self.android:
             return self.android_api
@@ -539,24 +632,30 @@
                 if self.print: console(f'Found RASPI TOOLS: {self.raspi_compilers}\n    sysroot: {self.raspi_system}')
                 return
         raise EnvironmentError(f'''No Raspberry PI toolchain compilers detected! 
 Default search paths: {paths} 
 Define env RASPI_HOME with path to Raspberry tools.''')
 
 
-    def set_oclea_toolchain(self, toolchain_dir):
+    def set_oclea_toolchain(self, toolchain_dir=None, toolchain_file=None):
+        """
+        Sets the toolchain dir where these subdirs exist:
+            aarch64-oclea-linux/
+            x86_64-ocleasdk-linux/
+        And optionally also sets the CMake toolchain file via `toolchain_file`
+        """
+        self.oclea.init_toolchain(toolchain_dir, toolchain_file)
+
+
+    def set_mips_toolchain(self, arch, toolchain_dir=None, toolchain_file=None):
         """
-        Sets the oclea toolchain root directory, where
-        aarch64-oclea-linux/
-        x86_64-ocleasdk-linux/
-        directories exist.
+        Sets the toolchain dir for MIPS platform where at least the `bin` dir should exist
+        And optionally also sets the CMake toolchain file via `toolchain_file`
         """
-        if not os.path.exists(toolchain_dir):
-            raise FileNotFoundError(f'Toolchain directory not found: {toolchain_dir}')
-        self.oclea.init_oclea_path(toolchain_dir)
+        self.mips.init_toolchain(arch, toolchain_dir, toolchain_file)
 
 
     def find_default_fortran_compiler(self):
         paths = []
         if System.linux:
             paths += [util.find_executable_from_system('gfortran')]
         
@@ -570,15 +669,15 @@
     def get_visualstudio_path(self):
         if self._visualstudio_path:
             return self._visualstudio_path
         if not System.windows:
             raise EnvironmentError('VisualStudio tools support not available on this platform!')
 
         vswhere_exe = "C:\\Program Files (x86)\\Microsoft Visual Studio\\Installer\\vswhere.exe"
-        vspath = execute_piped(f'{vswhere_exe} -latest -nologo -property installationPath')
+        vspath = execute_piped(f'"{vswhere_exe}" -latest -nologo -property installationPath')
         if vspath and os.path.exists(vspath):
             self._visualstudio_path = vspath
             if self.verbose: console(f'Detected VisualStudio: {vspath}')
             return vspath
         
         paths = []
         vs_variants = [ 'Enterprise', 'Professional', 'Community'  ]
@@ -690,48 +789,35 @@
     def get_msvc_lib64(self):
         return f'{self.get_msvc_tools_path()}\\lib\\x64'
 
 
     def install_clang6(self):
         if System.windows: raise OSError('Install Visual Studio 2019 with Clang support')
         if System.macos:   raise OSError('Install Xcode to get Clang on macOS')
-        
+
+        id, major, _ = self.get_distro_info()
+        if id != "ubuntu": raise OSError('install_clang6 only supports ubuntu')
         suffix = '1404'
-        try:
-            dist = distro.info()
-            if dist['id'] != "ubuntu": raise OSError('install_clang6 only supports Ubuntu')
-            majorVersion = int(dist['version_parts']['major'])
-            if majorVersion >= 16:
-                suffix = '1604'
-            console(f'Choosing {suffix} for kernel major={majorVersion}')
-        except Exception as err:
-            console(f'Failed to parse linux distro; falling back to {suffix}: {err}')
+        if major >= 16: suffix = '1604'
 
+        console(f'Choosing {suffix} for kernel major={major}')
         self.install_clang(clang_major='6', clang_ver='6.0', suffix=suffix)
 
 
     def install_clang11(self):
         if System.windows: raise OSError('Install Visual Studio 2019 with Clang support')
         if System.macos:   raise OSError('Install Xcode to get Clang on macOS')
-        
+
+        id, major, minor = self.get_distro_info()
+        if id != "ubuntu": raise OSError('install_clang11 only supports ubuntu')
         suffix = '1604'
-        try:
-            dist = distro.info()
-            if dist['id'] != "ubuntu": raise OSError('install_clang11 only supports Ubuntu')
-            majorVersion = int(dist['version_parts']['major'])
-            minorVersion = int(dist['version_parts']['minor'])
-            if majorVersion >= 20 and minorVersion >= 10:
-                suffix = '2010'
-            elif majorVersion >= 20:
-                suffix = '2004'
-            elif majorVersion >= 16:
-                suffix = '1604'
-            console(f'Choosing {suffix} for kernel major={majorVersion} minor={minorVersion}')
-        except Exception as err:
-            console(f'Failed to parse linux distro; falling back to {suffix}: {err}')
+        if major >= 20 and minor >= 10: suffix = '2010'
+        elif major >= 20: suffix = '2004'
+        elif major >= 16: suffix = '1604'
+        console(f'Choosing {suffix} for kernel major={major} minor={minor}')
 
         self.install_clang(clang_major='11', clang_ver='11.0', suffix=suffix)
 
 
     def install_clang(self, clang_major, clang_ver, suffix):
         clang_major = '11'
         clang_ver = '11.0'
@@ -751,18 +837,18 @@
         execute(f'sudo update-alternatives --set clang   /usr/bin/clang-{clang_ver}')
         execute(f'sudo update-alternatives --set clang++ /usr/bin/clang++-{clang_ver}')
 
 
     def install_msbuild(self):
         if System.windows: raise OSError('Install Visual Studio 2019 to get MSBuild on Windows')
         if System.macos:   raise OSError('install_msbuild not implemented for macOS')
-        
-        dist = distro.info()
-        if dist['id'] != "ubuntu": raise OSError('install_msbuild only supports Ubuntu')
-        codename = dist['codename']
+
+        id, _, _ = self.get_distro_info()
+        if id != "ubuntu": raise OSError('install_msbuild only supports ubuntu')
+        codename = distro.info()['codename']
 
         execute('curl https://packages.microsoft.com/keys/microsoft.asc | gpg --dearmor > /tmp/microsoft.gpg')
         execute('sudo mv /tmp/microsoft.gpg /etc/apt/trusted.gpg.d/microsoft.gpg')
         execute(f"sudo sh -c 'echo \"deb [arch=amd64] https://packages.microsoft.com/repos/microsoft-ubuntu-{codename}-prod {codename} main\" > /etc/apt/sources.list.d/dotnetdev.list'")
         execute('sudo apt-get install apt-transport-https')
         execute('sudo apt-get update')
         execute('sudo apt-get install dotnet-sdk-2.1')
@@ -779,18 +865,19 @@
         else:            return f'lib{library}.a'
 
 
     def libext(self):
         return 'lib' if self.windows else 'a'
 
 
-    def targets_all(self):
+    def targets_all(self) -> bool:
         return self.target == 'all'
 
 
-    def target_matches(self, target_name):
-        return self.targets_all() or self.target == target_name
+    def target_matches(self, target_name: str) -> bool:
+        return self.targets_all() \
+            or (self.target and self.target.lower() == target_name.lower())
 
 
-    def no_specific_target(self):
+    def no_specific_target(self) -> bool:
         return (not self.target) or self.targets_all()
```

### Comparing `mama-0.7.9/mama/build_dependency.py` & `mama-0.8.0/mama/build_dependency.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,96 +32,111 @@
         self.always_build = False
         self.should_rebuild = False
         self.nothing_to_build = False
         self.already_loaded = False
         self.already_executed = False
         self.currently_loading = False
         self.from_artifactory = False # if true, this Dependency was loaded from Artifactory
+        self.did_check_artifactory = False # if true, artifactory was already checked and can be skipped
         self.is_root = parent is None # Root deps are always built
         self.children: List[BuildDependency] = []
         self.product_sources = []
-        self.flattened_deps: List[BuildDependency] = [] # used for debugging
+        self.flattened_deps: List[BuildDependency] = [] # flat dependencies only, nothing else
 
         self.src_dir = None # source directory where the code is located
         self.dep_dir = None # dependency dir where platform build dirs are kept
         self.build_dir = None # {dep_dir}/{config.platform_build_dir_name()}
         self.dep_source = dep_source
         self.name = dep_source.name
 
         if dep_source.is_git:
             git:Git = dep_source
             self.mamafile = git.mamafile # git.mamafile is the relative path
             if parent:
                 self.mamafile = parent.get_mamafile_path_relative_to_us(self.name, git.mamafile)
-            self.target_args = git.args
+            self._add_args(git.args)
             self.update_dep_dir()
             # put the git repo in workspace
             self.src_dir = normalized_join(self.dep_dir, self.name)
         elif dep_source.is_pkg:
             if not config.artifactory_ftp:
                 raise RuntimeError(f'add_artifactory_pkg({self.name}) failed because config.artifactory_ftp is not set!')
             self.src_dir = None # there is no src_dir when using artifactory packages
             self.create_build_target()
             self.update_dep_dir()
         elif dep_source.is_src:
             src:LocalSource = dep_source
             self.mamafile = src.mamafile
-            self.target_args = src.args
+            self._add_args(src.args)
             self.always_build = src.always_build
 
             if parent:
                 self.mamafile = parent.get_mamafile_path_relative_to_us(self.name, src.mamafile)
                 self.src_dir = parent.path_relative_to_us(src.rel_path)
             else:
                 self.src_dir = normalized_path(src.rel_path)
 
             if self.mamafile and not os.path.exists(self.mamafile):
                 raise OSError(f'{self.name} mamafile path does not exist: {self.mamafile}')
             if not os.path.exists(self.src_dir):
                 raise OSError(f'{self.name} source dir does not exist: {self.src_dir}')
 
             self.create_build_target()
-            self.name = str(self.target.name) # might change due to mamafile ??
+            self.name = str(self.target.name) # name can change due to mamafile !!
             self.update_dep_dir()
         else:
             raise RuntimeError(f'{self.name} src or git or pkg not configured. Specify at least one.')
 
 
+    def __str__(self): return f'BuildDependency {self.name} {self.dep_source}'
+    def __repr__(self): return f'BuildDependency {self.name} {self.dep_source}'
+
+
     @staticmethod
-    def get_loaded_dependency(name:str) -> BuildDependency:
+    def get_loaded_dependency(name: str) -> BuildDependency:
         if name in BuildDependency.loaded_deps:
             return BuildDependency.loaded_deps[name]
         return None
 
 
-    def update_existing_dependency(self, dep_source:DepSource):
+    def _add_args(self, args):
+        if args: # only add non-empty args (bugfix)
+            for arg in args:
+                if arg:
+                    self.target_args.append(arg)
+
+
+    def update_existing_dependency(self, dep_source: DepSource):
         if dep_source.is_git or dep_source.is_src:
-            self.target_args += dep_source.args
+            self._add_args(dep_source.args)
             if self.target:
                 self.target._set_args(self.target_args)
 
 
-    def add_child(self, dep_source:DepSource) -> BuildDependency:
+    def add_child(self, dep_source: DepSource) -> BuildDependency:
         """
         Adds a new child dependency to this BuildDependency
         """
         dep = BuildDependency.get_loaded_dependency(dep_source.name)
         if dep:
             # reuse & update existing dep
             dep.update_existing_dependency(dep_source)
         else:
             # add new
             dep = BuildDependency(self, self.config, self.workspace, dep_source)
             BuildDependency.loaded_deps[dep_source.name] = dep
+            if self.config.verbose:
+                console(f'  - Target {self.name: <16} ADD {dep}', color=Color.BLUE)
 
         if dep in self.children:
             raise RuntimeError(f"BuildTarget {self.name} add dependency '{dep.name}'"\
                                 " failed because it has already been added")
 
         self.children.append(dep)
+        return dep
 
 
     def get_children(self) -> List[BuildDependency]:
         """ Gets already resolved dependencies """
         if self.children is None:
             raise RuntimeError(f'Target {self.name} child dependencies unresolved')
         return self.children
@@ -204,46 +219,76 @@
             self.currently_loading = True
             changed = self._load()
         finally:
             self.currently_loading = False
         return changed
 
 
-    def _load(self):
-        self.create_build_target()  ## parses target mamafile
-        self.update_dep_dir()
+    def _load_target(self) -> BuildTarget:
+        self.create_build_target() ## parses target mamafile
+        self.update_dep_dir() ## requires target mamafile workspace
         self.create_build_dir_if_needed()
+        return self.target
 
-        if self.target.config.verbose:
-            console(f'  - Load Target {self.name} ({self.dep_source.get_type_string()})', color=Color.BLUE)
+    def _git_checkout_if_needed(self) -> bool:
+        if not self.is_root and self.dep_source.is_git:
+            git:Git = self.dep_source
+            return git.dependency_checkout(self)
+        return False
 
-        target = self.target
+
+    def _load(self):
         conf = self.config
-        is_target = conf.target_matches(target.name)
+        if conf.verbose:
+            console(f'  - Target {self.name: <16} LOAD ({self.dep_source.get_type_string()})', color=Color.BLUE)
+
+        is_target = self.is_current_target()
+
+        # for root targets, always load the BuildTarget immediately, we need the root workspace from its mamafile
+        if self.is_root:
+            target = self._load_target()
+        # for non-root targets, only create the required dirs
+        else:
+            self.update_dep_dir()
+            self.create_build_dir_if_needed()
+
+        git_changed = self._git_checkout_if_needed() ## pull Git before loading target Mamafile
+
+        target = self._load_target() ## load target for Git and Src
         if conf.clean and is_target:
-            self.clean()
+            self.clean() ## requires a parsed mamafile target
+
+        # if artifactory_fetch_and_reconfigure succeeds, it will overwrite products and libs
+        # and sets self.from_artifactory
+        loaded_from_pkg = False
+        should_load_art = self.should_load_artifactory()
+        if should_load_art and self.can_fetch_artifactory(print=True, which='LOAD'):
+            self.did_check_artifactory = True
+            fetched, dependencies = artifactory_fetch_and_reconfigure(target)
+            if fetched:
+                for dep_name in dependencies:
+                    self.add_child(dep_name)
+                loaded_from_pkg = True
+            elif self.dep_source.is_pkg:
+                raise RuntimeError(f'  - Target {self.name} failed to load artifactory pkg {self.dep_source}')
+        elif should_load_art and self.is_force_art_target():
+            raise RuntimeError(f'  - Target {self.name} failed to find artifactory pkg {self.dep_source} but `art` was specified')
 
         # load any build products from previous builds
-        if not self.is_root:
+        if not self.is_root and not loaded_from_pkg:
             self.load_build_products(target)
 
-        # if this succeeds, it will overwrite products and libs
-        # and sets self.from_artifactory
-        loaded_from_pkg = self.load_artifactory_package(target)
-        git_changed = False
-        if not loaded_from_pkg and not self.is_root and self.dep_source.is_git:
-            git:Git = self.dep_source
-            git_changed = git.dependency_checkout(self)
-
+        if conf.verbose:
+            console(f'  - Target {self.name: <16} load settings and dependencies')
         target.settings() ## customization point for project settings
         target.dependencies() ## customization point for additional dependencies
 
         if not loaded_from_pkg and self.is_root:
             # fetch the compiler immediately from root settings
-            self.config.get_preferred_compiler_paths()
+            conf.get_preferred_compiler_paths()
 
         build = False
         if conf.build or conf.update:
             build = self._should_build(conf, target, is_target, git_changed, loaded_from_pkg)
             if build:
                 self.create_build_dir_if_needed() # in case we just cleaned
             if git_changed:
@@ -253,99 +298,123 @@
         self.already_loaded = True
         self.should_rebuild = build
         if conf.list:
             self._print_list(conf, target)
         return build
 
 
-    def load_artifactory_package(self, target):
-        # always load during rebuild
-        # don't load anything during cleaning, because it will get cleaned anyways
-        can_load = self.config.rebuild or not self.config.clean
-        load_art = can_load and \
-            (self.dep_source.is_pkg or os.path.exists(self.papa_package_file()) or self.is_first_time_build())
-        if load_art:
-            fetched, dependencies = artifactory_fetch_and_reconfigure(target)
-            if fetched:
-                for dep_name in dependencies:
-                    self.add_child(dep_name)
-                return True
-            elif self.dep_source.is_pkg:
-                raise RuntimeError(f'  - Target {target.name} failed to load artifactory pkg {self.dep_source}')
-        return False
+    def can_fetch_artifactory(self, print: bool, which: str):
+        if self.is_root or self.did_check_artifactory:
+            return False
+
+        force_art = self.config.force_artifactory
+        disable_art = self.config.disable_artifactory
+        is_target = self.is_current_target()
+
+        def noart(r):
+            if print and (self.config.print or force_art):
+                console(f'  - Target {self.name: <16} NO ARTIFACTORY PKG [{which} {r}]', color=Color.YELLOW)
+            self.did_check_artifactory = True
+            return False
+
+        if disable_art:
+            return noart('noart override')
+        elif is_target and not force_art:
+            # don't load during rebuild -- defer to source based builds in that case
+            if self.config.rebuild: return noart('target rebuild')
+            # don't load anything during cleaning -- because it will get cleaned anyways
+            if self.config.clean: return noart('target clean')
+        elif print and (self.config.verbose or force_art):
+            console(f'  - Target {self.name: <16} CHECK ARTIFACTORY PKG [{which}]', color=Color.YELLOW)
+
+        return True
+
+
+    def is_force_art_target(self):
+        return not self.is_root and self.config.force_artifactory and self.is_current_target()
+
+
+    def should_load_artifactory(self):
+        if self.is_root or self.did_check_artifactory:
+            return False
+        should_load = self.dep_source.is_pkg \
+            or os.path.exists(self.papa_package_file()) \
+            or self.is_first_time_build()
+        is_force_art_target = self.is_force_art_target()
+        return should_load or is_force_art_target
 
 
     def _print_list(self, conf, target):
         if conf.print:
             console(f'  - Target {target.name: <16}')
 
 
-    def _should_build(self, conf, target, is_target, git_changed, loaded_from_pkg):
-            def build(r):
-                if conf.print:
-                    args = f'{target.args}' if target.args else ''
-                    console(f'  - Target {target.name: <16}   BUILD [{r}]  {args}', color=Color.YELLOW)
-                return True
-
-            if conf.target and not is_target: # if we called: "target=SpecificProject"
-                return False # skip build if target doesn't match
-
-            ## build also entails packaging
-            if conf.clean and is_target: return build('cleaned target')
-            if self.is_root:             return build('root target')
-            if self.always_build:        return build('always build')
-            if git_changed:              return build('git commit changed')
-            if self.dep_source.is_pkg:   return build('artifactory pkg')
-
-            # if we call `update this_target`
-            if conf.update and conf.target == target.name:
-                return build('update target='+conf.target)
-
-            # if the project has been built at least once or downloaded from artifactory package
-            # then there will be a list of build products
-            # if any of those are missing, then this needs to be rebuilt to re-acquire them
-            missing_product = self.find_first_missing_build_product()
-            if missing_product:
-                return build(f'{missing_product} does not exist')
-
-            # project has not defined `nothing_to_build` which is for header-only projects
-            # thus we need to check if build should execute
-            can_build = not loaded_from_pkg and not self.nothing_to_build
-            if can_build:
-                # there are no build products defined at all, it hasn't been built or downloaded
-                if not target.build_products:
-                    if not self.has_build_files():
-                        return build('not built yet')
-                    return build('no build dependencies')
-
-                # we have build products, and none of them are missing
-                if target.build_products and not missing_product:
-                    pass # added this condition for clarity -- all should be OK
-
-            # something changed in the mamafile, or artifactory package
-            # and the list of dependency targets changed, thus we need to rebuild
-            missing_dep = self.find_missing_dependency()
-            if missing_dep: return build(f'{missing_dep} was removed')
-
-            if not self.from_artifactory:
-                if self.update_mamafile_tag(): return build(target.name+'/mamafile.py modified')
-                if self.update_cmakelists_tag(): return build(target.name+'/CMakeLists.txt modified')
-
+    def _should_build(self, conf:BuildConfig, target:BuildTarget, is_target, git_changed, loaded_from_pkg):
+        def build(r):
             if conf.print:
-                console(f'  - Target {target.name: <16}   OK', color=Color.GREEN)
-            return False # do not build, all is ok
+                args = f'{target.args}' if target.args else ''
+                console(f'  - Target {target.name: <16} BUILD [{r}]  {args}', color=Color.YELLOW)
+            return True
+
+        if conf.target and not is_target: # if we called: "target=SpecificProject"
+            return False # skip build if target doesn't match
+
+        ## build also entails packaging
+        if conf.clean and is_target: return build('cleaned target')
+        if self.is_root:             return build('root target')
+        if self.always_build:        return build('always build')
+        if git_changed:              return build('git commit changed')
+        if self.dep_source.is_pkg:   return build('artifactory pkg')
+
+        # if we call `update this_target`
+        if conf.update and conf.target == target.name:
+            return build('update target='+conf.target)
+
+        # if the project has been built at least once or downloaded from artifactory package
+        # then there will be a list of build products
+        # if any of those are missing, then this needs to be rebuilt to re-acquire them
+        missing_product = self.find_first_missing_build_product()
+        if missing_product:
+            return build(f'{missing_product} does not exist')
+
+        # project has not defined `nothing_to_build` which is for header-only projects
+        # thus we need to check if build should execute
+        can_build = not loaded_from_pkg and not self.nothing_to_build
+        if can_build:
+            # there are no build products defined at all, it hasn't been built or downloaded
+            if not target.build_products:
+                if not self.has_build_files():
+                    return build('not built yet')
+                return build('no build dependencies')
+
+            # we have build products, and none of them are missing
+            if target.build_products and not missing_product:
+                pass # added this condition for clarity -- all should be OK
+
+        # something changed in the mamafile, or artifactory package
+        # and the list of dependency targets changed, thus we need to rebuild
+        missing_dep = self.find_missing_dependency()
+        if missing_dep: return build(f'{missing_dep} was removed')
+
+        if not self.from_artifactory:
+            if self.update_mamafile_tag(): return build(target.name+'/mamafile.py modified')
+            if self.update_cmakelists_tag(): return build(target.name+'/CMakeLists.txt modified')
+
+        if conf.print:
+            console(f'  - Target {target.name: <16} OK', color=Color.GREEN)
+        return False # do not build, all is ok
 
 
     def after_load(self):
         if self.config.no_specific_target():
             first_changed = next((c for c in self.children if c.should_rebuild), None)
             if first_changed and not self.should_rebuild:
                 self.should_rebuild = True
                 if self.config.print:
-                    console(f'  - Target {self.name: <16}   BUILD [{first_changed.name} changed]')
+                    console(f'  - Target {self.name: <16} BUILD [{first_changed.name} changed]')
                 self.create_build_dir_if_needed() # in case we just cleaned
 
 
     def successful_build(self):
         self.update_mamafile_tag()
         self.update_cmakelists_tag()
         self.save_dependency_list()
@@ -357,17 +426,22 @@
     def create_build_target(self):
         if self.target:
             self.target._set_args(self.target_args)
             return
 
         # load the default mama.BuildTarget class
         mamaBuildTarget = getattr(sys.modules['mama.build_target'], 'BuildTarget')
+        mamaFilePath = self.mamafile_path()
+        if mamaFilePath and self.config.verbose:
+            exists = os.path.exists(mamaFilePath)
+            relpath = os.path.relpath(mamaFilePath)
+            console(f'  - Target {self.name: <16} Load Mamafile: {relpath} (Exists={exists})', color=Color.BLUE)
 
         # this will load the specific `<class project(mama.build_target)>` class
-        project, buildTarget = parse_mamafile(self.config, mamaBuildTarget, self.mamafile_path())
+        project, buildTarget = parse_mamafile(self.config, mamaBuildTarget, mamaFilePath)
         if project and buildTarget:
             buildStatics = buildTarget.__dict__
             if not self.workspace:
                 if   'workspace'        in buildStatics: self.workspace = buildStatics['workspace']
                 elif 'local_workspace'  in buildStatics: self.workspace = buildStatics['local_workspace']
                 elif 'global_workspace' in buildStatics: self.workspace = buildStatics['global_workspace']
                 else:                                    self.workspace = 'build'
@@ -377,39 +451,44 @@
                 elif 'global_workspace' in buildStatics: self.config.global_workspace = True
                 if not self.config.global_workspace:
                     self.config.workspaces_root = self.src_dir
             self.target = buildTarget(name=project, config=self.config, dep=self, args=self.target_args)
         else:
             if not self.workspace:
                 self.workspace = 'build'
+            if self.config.verbose:
+                console(f'  - Target {self.name: <16} Using Default BuildTarget Project={project} BuildTarget={buildTarget}', color=Color.YELLOW)
             self.target = mamaBuildTarget(name=self.name, config=self.config, dep=self, args=self.target_args)
 
 
+    def is_current_target(self):
+        return self.config.target_matches(self.name)
+
+
     def is_root_or_config_target(self):
-        if self.config.target:
-            return self.config.target_matches(self.name)
-        return self.is_root
+        return self.is_root or self.is_current_target()
 
 
     def cmakelists_path(self):
-        return os.path.join(self.src_dir, 'CMakeLists.txt')
+        cmake_lists_path = self.target.cmake_lists_path if self.target else 'CMakeLists.txt'
+        return normalized_join(self.src_dir, cmake_lists_path)
 
 
     def cmakelists_exists(self):
         return os.path.exists(self.cmakelists_path())
 
 
     def ensure_cmakelists_exists(self):
         if not os.path.exists(self.cmakelists_path()):
             raise IOError(f'Could not find {self.cmakelists_path()}! Add a CMakelists.txt, or add `self.nothing_to_build()` to configuration step. Also note that filename CMakeLists.txt is case sensitive.')
 
 
     def mamafile_path(self):
         if self.mamafile: return self.mamafile
-        if self.src_dir: return os.path.join(self.src_dir, 'mamafile.py')
+        if self.src_dir: return normalized_join(self.src_dir, 'mamafile.py')
         return None
 
 
     def mamafile_exists(self):
         return os.path.exists(self.mamafile_path())
 
 
@@ -480,15 +559,15 @@
                 return last.strip()
         return None # Nothing missing
 
 
     ## Clean
     def clean(self):
         if self.config.print:
-            console(f'  - Target {self.name: <16}   CLEAN  {self.config.platform_build_dir_name()}')
+            console(f'  - Target {self.name: <16} CLEAN  {self.config.platform_build_dir_name()}')
 
         if self.build_dir == '/' or not os.path.exists(self.build_dir):
             return
 
         self.target.clean() # Customization point
         shutil.rmtree(self.build_dir, ignore_errors=True)
```

### Comparing `mama-0.7.9/mama/build_target.py` & `mama-0.8.0/mama/build_target.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 from typing import List, TYPE_CHECKING
-import os.path, shutil
+import os.path, time
 
 from .types.git import Git
 from .types.local_source import LocalSource
 from .types.asset import Asset
 from .types.artifactory_pkg import ArtifactoryPkg
 
 from .artifactory import artifactory_fetch_and_reconfigure
@@ -63,14 +63,15 @@
         self.cmake_raspi_toolchain = '' # Custom Raspberry toolchain file for this target only
         self.cmake_ios_toolchain   = '' # Custom iOS toolchain file for this target only
         self.cmake_opts       = []
         self.cmake_cxxflags   = dict()
         self.cmake_cflags     = dict()
         self.cmake_ldflags    = dict()
         self.cmake_build_type = 'Debug' if config.debug else 'RelWithDebInfo'
+        self.cmake_lists_path = 'CMakeLists.txt' # relative to source_dir
         self.enable_exceptions = True
         self.enable_unix_make  = False
         self.enable_ninja_build = True and config.ninja_path # attempt to use Ninja
         self.enable_fortran_build = False
         self.enable_cxx_build = True
         self.enable_multiprocess_build = True
         self.clean_intermediate_files = True # delete .o and .obj files after build success if not root or always_build
@@ -85,24 +86,26 @@
         self.windows = self.config.windows # convenient alias
         self.linux   = self.config.linux
         self.macos   = self.config.macos
         self.ios     = self.config.ios
         self.android = self.config.android
         self.raspi   = self.config.raspi
         self.oclea   = self.config.oclea
+        self.mips    = self.config.mips
         self.os_windows = System.windows
         self.os_linux   = System.linux
         self.os_macos   = System.macos
         self._set_args(args)
 
 
-    def _set_args(self, args:List[str]):
+    def _set_args(self, args: List[str]):
         if not isinstance(args, list):
             raise RuntimeError(f'BuildTarget {self.name} target args must be a list')
-        self.args += args
+        for arg in args:
+            if arg: self.args.append(arg)
         #console(f'Added args to {self.name}: {self.args}')
 
 
     def children(self) -> List[BuildDependency]:
         """ Get resolved child dependencies """
         return self.dep.get_children()
 
@@ -154,15 +157,15 @@
         NOTE: Currently only FTP is supported
         """
         if not self.dep.is_root:
             return
         self.config.set_artifactory_ftp(ftp_url=ftp_url, auth=auth)
 
 
-    def add_local(self, name, source_dir, mamafile=None, always_build=False, args=[]):
+    def add_local(self, name, source_dir, mamafile=None, always_build=False, args=[]) -> BuildDependency:
         """
         Add a local dependency. This can be a git submodule or just some local folder.
         which contains its own CMakeLists.txt.
         Optionally you can override the default 'mamafile.py' with your own.
 
         If the local dependency folder does not contain a `mamafile.py`, you will have to
         provide your own relative or absolute mamafile path.
@@ -174,19 +177,20 @@
         will have to check `self.args` for any arguments of interest.
         ```
         self.add_local('zlib', '3rdparty/zlib')
         self.add_local('zlib', '3rdparty/zlib', mamafile='mama/zlib.py')
         self.add_local('avdecoder', 'lib/avdecoder', always_build=True)
         ```
         """
-        if self.dep.from_artifactory: return # ignore if already loaded from artifactory
-        self.dep.add_child(LocalSource(name, source_dir, mamafile, always_build, args))
+        if self.dep.from_artifactory: # already loaded from artifactory?
+            return self.get_dependency(name)
+        return self.dep.add_child(LocalSource(name, source_dir, mamafile, always_build, args))
 
 
-    def add_git(self, name, git_url, git_branch='', git_tag='', mamafile=None, args=[]):
+    def add_git(self, name, git_url, git_branch='', git_tag='', mamafile=None, args=[]) -> BuildDependency:
         """
         Add a remote GIT dependency.
         The dependency will be cloned and updated according to mamabuild.
         Use `mama update` to force update the git repositories.
     
         If the remote GIT repository does not contain a `mamafile.py`, you will have to
         provide your own relative or absolute mamafile path.
@@ -197,19 +201,20 @@
         ```
         self.add_git('ReCpp', 'git@github.com:RedFox20/ReCpp.git')
         self.add_git('ReCpp', 'git@github.com:RedFox20/ReCpp.git', git_branch='master')
         self.add_git('opencv', 'https://github.com/opencv/opencv.git', 
                      git_branch='3.4', mamafile='mama/opencv_cfg.py')
         ```
         """
-        if self.dep.from_artifactory: return # ignore if already loaded from artifactory
-        self.dep.add_child(Git(name, git_url, git_branch, git_tag, mamafile, args))
+        if self.dep.from_artifactory: # already loaded from artifactory?
+            return self.get_dependency(name)
+        return self.dep.add_child(Git(name, git_url, git_branch, git_tag, mamafile, args))
 
 
-    def add_artifactory_pkg(self, name, version='latest', fullname=None):
+    def add_artifactory_pkg(self, name, version='latest', fullname=None) -> BuildDependency:
         """
         Adds an Artifactory only dependency.
         The dependency will be downloaded from the artifactory url.
 
         If the remote artifactory does not contain this package,
         an error is thrown during build.
 
@@ -222,19 +227,20 @@
 
         ```
         self.add_artifactory_pkg('mylib', version='latest')
         self.add_artifactory_pkg('mylib', version='df76b66')
         self.add_artifactory_pkg('mylib', fullname='mylib-linux-x64-release-df76b66')
         ```
         """
-        if self.dep.from_artifactory: return # ignore if already loaded from artifactory
-        self.dep.add_child(ArtifactoryPkg(name, version=version, fullname=fullname))
+        if self.dep.from_artifactory: # already loaded from artifactory?
+            return self.get_dependency(name)
+        return self.dep.add_child(ArtifactoryPkg(name, version=version, fullname=fullname))
 
 
-    def get_dependency(self, name):
+    def get_dependency(self, name: str) -> BuildDependency:
         """
         Finds a child dependency by name.
         ```
             zlib_dep = self.get_dependency('zlib')
         ```
         """
         if self.dep.name == name:
@@ -676,32 +682,75 @@
 
 
     def prefer_clang(self):
         """ Configures the entire build chain to prefer Clang if possible """
         self.config.prefer_clang(self.name)
 
 
+    def _get_cxx_std(self):
+        return self.cmake_cxxflags.get('/std' if self.windows else '-std', '')
+
+    def _set_cxx_std(self, std):
+        self.cmake_cxxflags['/std' if self.windows else '-std'] = std
+
+
+    def enable_cxx23(self):
+        """ Enable C++23 standard """
+        self._set_cxx_std('c++latest' if self.windows else 'c++2b')
+
+    def is_enabled_cxx23(self):
+        if 'CXX23' in self.args: return True
+        std = self._get_cxx_std()
+        return 'c++23' in std or 'c++2b' in std or 'c++latest' in std
+
+
     def enable_cxx20(self):
-        """Enable a specific C++ standard"""
-        self.cmake_cxxflags['/std' if self.windows else '-std'] = 'c++latest' if self.windows else 'c++2a'
+        """Enable C++20 standard"""
+        if self.mips or self.raspi or self.oclea:
+            self._set_cxx_std('c++2a') # older toolchains typically need c++2a
+        else:
+            self._set_cxx_std('c++20')
+
+    def is_enabled_cxx20(self):
+        if 'CXX20' in self.args: return True
+        std = self._get_cxx_std()
+        return 'c++20' in std or 'c++2a' in std
 
 
     def enable_cxx17(self):
-        """Enable a specific C++ standard"""
-        self.cmake_cxxflags['/std' if self.windows else '-std'] = 'c++17'
+        """Enable C++17 standard"""
+        if 'g++' in self.config.cxx_path and self.config.cxx_version < 8:
+            self._set_cxx_std('c++1z') # older toolchains typically need c++1z
+        else:
+            self._set_cxx_std('c++17')
+
+    def is_enabled_cxx17(self):
+        if 'CXX17' in self.args: return True
+        std = self._get_cxx_std()
+        return 'c++17' in std or 'c++1z' in std
 
 
     def enable_cxx14(self):
-        """Enable a specific C++ standard"""
-        self.cmake_cxxflags['/std' if self.windows else '-std'] = 'c++14'
+        """Enable C++14 standard"""
+        self._set_cxx_std('c++14')
+
+    def is_enabled_cxx14(self):
+        if 'CXX14' in self.args: return True
+        std = self._get_cxx_std()
+        return 'c++14' in std
 
 
     def enable_cxx11(self):
-        """Enable a specific C++ standard"""
-        self.cmake_cxxflags['/std' if self.windows else '-std'] = 'c++11'
+        """Enable C++11 standard"""
+        self._set_cxx_std('c++11')
+
+    def is_enabled_cxx11(self):
+        if 'CXX11' in self.args: return True
+        std = self._get_cxx_std()
+        return 'c++11' in std
 
 
     def copy(self, src, dst):
         """
         Utility for copying files and folders
         ```
             # copies built .so into an android archive
@@ -823,73 +872,78 @@
                 self.nothing_to_build()
         ```
         """
         self.dep.nothing_to_build = True
         self.dep.should_rebuild = False
 
 
-    def run(self, command, src_dir=False):
+    def run(self, command, src_dir=False, exit_on_fail=True):
         """
         Run a command in the build or source folder.
         Can be used for any custom commands or custom build systems.
         src_dir -- [False] If true, then command is relative to source directory.
         ```
             self.run('./configure')
             self.run('make release -j7')
         ```
         """
         dir = self.source_dir() if src_dir else self.build_dir()
-        execute(f'cd {dir} && {command}', echo=True)
+        res = execute(f'cd {dir} && {command}', echo=True, throw=not exit_on_fail)
+        if res != 0 and exit_on_fail:
+            exit(res)
 
 
     def run_program(self, working_dir, command):
         """
         Run any program in any directory. Can be used for custom tools.
         ```
             self.run_program(self.source_dir('bin'), 
                              self.source_dir('bin/DbTool'))
         ```
         """
-        execute_echo(working_dir, command)
+        execute_echo(working_dir, command, exit_on_fail=True)
 
 
     ## TODO: Move this into a new utility
     def gdb(self, command, src_dir=True):
         """
         Run a command with gdb in the build folder.
         ```
             self.gdb('bin/NanoMeshTests')
         ```
         """
-        if self.android or self.ios or self.raspi or self.oclea:
-            console('Cannot run tests for Android, iOS, Raspi, Oclea builds.')
+        if self.android or self.ios or self.raspi or self.oclea or self.mips:
+            console('Cannot run tests for Android, iOS, Raspi, Oclea, MIPS builds.')
             return # nothing to run
 
         split = command.split(' ', 1)
         cmd = split[0].lstrip('.')
         args = split[1] if len(split) >= 2 else ''
         path = self.source_dir() if src_dir else self.build_dir()
         path = f"{path}/{os.path.dirname(cmd).lstrip('/')}"
         exe = os.path.basename(cmd)
 
+        if System.windows and self.windows and '.exe' not in exe:
+            exe += '.exe'
+
         if self.windows:
             if not src_dir: path = f'{path}/{self.cmake_build_type}'
-            gdb = f'{exe} {args}'
+            gdb = f'{path}/{exe} {args}'
         elif self.macos:
             # b: batch, q: quiet, -o r: run
             # -k bt: on crash, backtrace
             # -k q: on crash, quit 
             gdb = f'lldb -b -o r -k bt -k q  -- ./{exe} {args}'
         else: # linux
             # r: run;  bt: give backtrace;  q: quit when done;
             gdb = f'gdb -batch -return-child-result -ex=r -ex=bt -ex=q --args ./{exe} {args}'
 
-        if not (os.path.exists(f'{path}/{exe}') or os.path.exists(f'{path}/{exe}.exe')):
+        if not os.path.exists(f'{path}/{exe}'):
             raise IOError(f'Could not find {path}/{exe}')
-        execute_echo(path, gdb)
+        execute_echo(cwd=path, cmd=gdb)
 
 
     ########## Customization Points ###########
 
 
     def settings(self):
         """
@@ -1136,44 +1190,60 @@
     def clean_target(self):
         self.dep.clean()
 
 
     def cmake_build(self):
         if self.config.print:
             console('\n\n#############################################################')
-            console(f"CMakeBuild {self.name}  ({self.cmake_build_type})")
+            console(f"CMakeBuild {self.name} ({self.cmake_build_type})")
+        config_start = time.time()
         self.dep.ensure_cmakelists_exists()
         cmake.inject_env(self)
         cmake.run_config(self) # THROWS on CMAKE failure
+        config_stop = time.time()
+        build_start = config_stop
         cmake.run_build(self, install=True) # THROWS on CMAKE failure
+        build_stop = time.time()
+        if self.config.print:
+            e_config = util.get_time_str(config_stop - config_start)
+            e_build = util.get_time_str(build_stop - build_start)
+            e_total = util.get_time_str(build_stop - config_start)
+            console(f"CMakeBuild {self.name} ({self.cmake_build_type}) config {e_config} build {e_build} total {e_total}", color='green')
 
 
     def is_test_target(self):
         """
         TRUE if this build target was specified along with `test` command.
         This matches `all`, specific cmdline targets, and the `root` target.
         ```
         mama test              # the root target
         mama test this_target  # specific target
         mama test all          # all targets
         ```
         """
-        return self.config.test and self.dep.is_root_or_config_target()
+        if not self.config.test:
+            return False
+        # `mama test` --> only test root target
+        if not self.config.target and self.dep.is_root:
+            return True
+        # `mama test ReCpp` --> only test current target
+        # `mama test all` --> current target matches all
+        return self.config.target and self.dep.is_current_target()
 
 
     def is_current_target(self):
         """
         TRUE if this BuildTarget is a configuration target for
         build/test/etc. This matches 'all' or specific cmdline targets:
         ```
             mama build
             mama build this_target
         ```
         """
-        return self.config.target_matches(self.name)
+        return self.dep.is_current_target()
 
 
     ## Build only this target
     def _execute_tasks(self):
         if self.dep.already_executed:
             return
         try:
@@ -1185,21 +1255,25 @@
             import traceback
             console(f'  [BUILD FAILED]  {self.dep.name}  \n{err}\n\n')
             traceback.print_exc()
             exit(-1) # exit without further stack trace
 
 
     def try_automatic_artifactory_fetch(self):
-        is_deploy = self.config.deploy or self.config.upload
-        is_target = not self.config.rebuild and self.is_current_target()
+        if not self.dep.can_fetch_artifactory(print=True, which='AUTO'):
+            return None
+
         # auto-fetch if:
-        # - not a deploy task
-        # - not the current build target eg `mama build this_target`
         # - is not the root project, roots should never be fetched
-        if not is_deploy and not is_target and not self.dep.is_root:
+        # - not a deploy/upload task
+        # - not the current build target eg `mama build this_target`
+        is_target = not self.dep.is_root and self.is_current_target()
+        is_deploy = self.config.deploy or self.config.upload
+        is_build = self.config.build
+        if is_target and not is_deploy and not is_build:
             fetched, _ = artifactory_fetch_and_reconfigure(self) # this will reconfigure packaging
             return fetched
         return None
 
 
     ## TODO: move all of this into a new utility
     def _execute_build_tasks(self):
```

### Comparing `mama-0.7.9/mama/cmake_configure.py` & `mama-0.8.0/mama/cmake_configure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 import os
-from .utils.system import System, console
-from .utils.sub_process import SubProcess, execute
+from .utils.system import System, console, Color
+from .utils.sub_process import SubProcess, execute_piped_echo
 
 if TYPE_CHECKING:
     from .build_target import BuildTarget
     from .build_config import BuildConfig
 
 
 def _rerunnable_cmake_conf(cmd, cwd, allow_rerun, target:BuildTarget, delete_cmakecache:bool = False):
@@ -53,37 +53,63 @@
 
     def get_flags():
         flags = ''
         options = target.cmake_opts + _default_options(target) + target.get_product_defines()
         for opt in options: flags += '-D'+opt+' '
         return flags
 
+    type_flags = f'-DCMAKE_BUILD_TYPE={target.cmake_build_type}'
     cmake_flags = get_flags()
     generator = _generator(target)
-    src_dir = target.source_dir()
-    cmd = f'cmake {generator} {cmake_flags} -DCMAKE_INSTALL_PREFIX="." "{src_dir}"'
+    src_dir = os.path.dirname(target.dep.cmakelists_path())
+    src_dir = src_dir if src_dir else target.source_dir()
+    install_prefix = '-DCMAKE_INSTALL_PREFIX="."'
+    # # use install prefix override for libraries, but for root target, leave it open-ended
+    # install_prefix = '' if target.dep.is_root else '-DCMAKE_INSTALL_PREFIX="."'
+    cmd = f'cmake {generator} {type_flags} {cmake_flags} {install_prefix} "{src_dir}"'
     _rerunnable_cmake_conf(cmd, target.build_dir(), True, target)
 
 
-def run_build(target:BuildTarget, install:bool, extraflags=''):
+def is_rerunnable_error(output:str):
+    """ Checks output string if a rerunnable error occurred. 
+        These are non-fatal errors that disappear with a simple cmake configure. """
+    return 'Makefile: No such file or directory' in output
+
+
+def run_build(target:BuildTarget, install:bool, extraflags='', rerun=True):
     build_dir = target.build_dir()
     flags = _build_config(target, install)
     extraflags = _buildsys_flags(target)
-    execute(f'cmake --build {build_dir} {flags} {extraflags}', echo=target.config.verbose)
+    cmd = f'cmake --build {build_dir} {flags} {extraflags}'
+    if target.config.verbose:
+        console(cmd, color=Color.GREEN)
+    status, output = execute_piped_echo(build_dir, cmd, echo=True)
+    if status != 0:
+        if rerun and is_rerunnable_error(output):
+            if target.config.verbose:
+                console(f'Build {target.name} failed, attempting to rerun config', color=Color.GREEN)
+            cmake_cache = target.build_dir('CMakeCache.txt')
+            if os.path.exists(cmake_cache):
+                os.remove(cmake_cache)
+            run_config(target)
+            run_build(target, install, extraflags, rerun=False)
+        else:
+            raise Exception(f'{cmd} failed with return code {status}')
 
 
 def _generator(target:BuildTarget):
     config:BuildConfig = target.config
     if target.enable_unix_make:   return '-G "Unix Makefiles"'
     if config.windows:            return f'-G "{config.get_visualstudio_cmake_id()}" -A {config.get_visualstudio_cmake_arch()}'
     if target.enable_ninja_build: return '-G "Ninja"'
     if config.android:            return '-G "Unix Makefiles"'
     if config.linux:              return '-G "Unix Makefiles"'
     if config.raspi:              return '-G "Unix Makefiles"'
     if config.oclea:              return '-G "Unix Makefiles"'
+    if config.mips:               return '-G "Unix Makefiles"'
     if config.ios:                return '-G "Xcode"'
     if config.macos:              return '-G "Xcode"'
     else:                         return ''
 
 
 def _make_program(target:BuildTarget):
     config:BuildConfig = target.config
@@ -95,19 +121,20 @@
             return f'{config.android_ndk()}\\prebuilt\\windows-x86_64\\bin\\make.exe' # CodeBlocks - Unix Makefiles
         elif System.macos:
             return f'{config.android_ndk()}/prebuilt/darwin-x86_64/bin/make' # CodeBlocks - Unix Makefiles
     return ''
 
 
 def _custom_compilers(target:BuildTarget):
-    config:BuildConfig = target.config
-    cc, cxx, ver = config.get_preferred_compiler_paths()
-    compilers = [f'CMAKE_C_COMPILER={cc}']
-    if target.enable_cxx_build:
-        compilers.append(f'CMAKE_CXX_COMPILER={cxx}')
+    compilers = []
+    cc, cxx, ver = target.config.get_preferred_compiler_paths()
+    if cc:
+        compilers.append(f'CMAKE_C_COMPILER={cc}')
+        if target.enable_cxx_build:
+            compilers.append(f'CMAKE_CXX_COMPILER={cxx}')
     return compilers
 
 
 def _default_options(target:BuildTarget):
     config:BuildConfig = target.config
     cxxflags:dict = target.cmake_cxxflags
     ldflags:dict = target.cmake_ldflags
@@ -162,23 +189,25 @@
             add_flag('-stdlib', 'libc++')
     elif config.raspi:
         add_flag('--sysroot', config.raspi_sysroot())
         for path in config.raspi_includes():
             add_flag(f'-I {path}')
     elif config.oclea:
         config.oclea.get_cxx_flags(add_flag)
+    elif config.mips:
+        config.mips.get_cxx_flags(add_flag)
 
     if config.flags:
         add_flag(config.flags)
 
     opt = [
         "CMAKE_POSITION_INDEPENDENT_CODE=ON",
         "CMAKE_EXPORT_COMPILE_COMMANDS=ON" # for tools like clang-tidy and .vscode intellisense
     ]
-    if config.linux or config.raspi or config.oclea:
+    if config.linux or config.raspi or config.oclea or config.mips:
         opt += _custom_compilers(target)
     
     if target.enable_fortran_build and config.fortran:
         opt += [f'CMAKE_Fortran_COMPILER={config.fortran}']
 
     cxxflags_str = get_flags_string(cxxflags)
     if cxxflags_str and target.enable_cxx_build:
@@ -231,14 +260,16 @@
         ]
         if target.cmake_raspi_toolchain:
             toolchain = target.source_dir(target.cmake_raspi_toolchain)
             if config.print: console(f'Toolchain: {toolchain}')
             opt += [f'CMAKE_TOOLCHAIN_FILE="{toolchain}"']
     elif config.oclea:
         opt += config.oclea.get_cmake_build_opts()
+    elif config.mips:
+        opt += config.mips.get_cmake_build_opts()
     elif config.macos:
         pass
     elif config.ios:
         opt += [
             'IOS_PLATFORM=OS',
             'CMAKE_SYSTEM_NAME=Darwin',
             'CMAKE_XCODE_EFFECTIVE_PLATFORMS=-iphoneos',
```

### Comparing `mama-0.7.9/mama/dependency_chain.py` & `mama-0.8.0/mama/dependency_chain.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         allowed = ['.a', '.so']
     elif target.linux: # TODO: android builds on Linux are impossible with this approach 
         allowed = ['.a', '.so']
     elif target.macos:
         allowed = ['.a', '.dylib', '.bundle']
     elif target.ios:
         allowed = ['.a', '.dylib', '.framework']
-    elif target.raspi or target.oclea:
+    elif target.raspi or target.oclea or target.mips:
         allowed = ['.a', '.so']
 
     #print(f'{target.name: <16} exported: {target.exported_libs}')
     for lib in target.exported_libs:
         for ext in allowed:
             if lib.endswith(ext):
                 filtered.append(lib)
@@ -60,18 +60,17 @@
                 ordered.remove(child)
             ordered.append(child)
             add_unique_items(child.get_children())
     add_unique_items(root.get_children())
     return ordered
 
 
-def get_full_flattened_deps(root: BuildDependency):
-    """ Information list of dep names """
-    deps = [root] + _get_flattened_deps(root)
-    return [dep.name for dep in deps]
+def get_flat_deps(root: BuildDependency):
+    """ Gets flat dependencies, including root """
+    return [root] + _get_flattened_deps(root)
 
 
 def _get_mama_dependencies_cmake(root: BuildDependency, build:str):
     if not root.get_children():
         return ''
     return f'include("{root.dep_dir}/{build}/mama-dependencies.cmake")'
 
@@ -98,21 +97,28 @@
     bin_exists = os.path.exists(bin_build_cmds)
 
     # choose the latest one
     if src_exists and bin_exists and os.path.getmtime(src_build_cmds) > os.path.getmtime(bin_build_cmds):
         # for src_dir paths we use `${workspaceFolder}` macro:
         return '${workspaceFolder}/build/compile_commands.json'
     if bin_exists:
+        # for build dir paths, check if build dir is relative to src dir
+        if dep.build_dir.startswith(dep.src_dir):
+            # if so, we chop off the src dir and use `${workspaceFolder}/`
+            rel_build_dir = f'${{workspaceFolder}}{dep.build_dir[len(dep.src_dir):]}/compile_commands.json'
+            return rel_build_dir
         return bin_build_cmds # absolute path for build dir paths
     return None
 
 
 def _save_vscode_compile_commands(dep: BuildDependency):
     if not dep.src_dir: # for artifactory pkgs, there is no src_dir
         return
+    if dep.config.oclea or dep.config.mips or dep.config.raspi or dep.config.android:
+        return # don't overwrite compile commands for cross-compilations
     cpp_props_path = f'{dep.src_dir}/.vscode/c_cpp_properties.json'
     if not os.path.exists(cpp_props_path):
         return
 
     commands_path = _get_compile_commands_path(dep)
     if not commands_path:
         return
@@ -164,16 +170,19 @@
     if not root.build_dir_exists():
         return # probably CLEAN, so nothing to save
     outfile = f'{root.build_dir}/mama-dependencies.cmake'
     text = \
 '''
 # This file is auto-generated by mama build. Do not modify by hand!
 '''
-    includes_defs = []
-    root.flattened_deps = [root] + _get_flattened_deps(root)
+    includes_def, package_text = _get_dependency_cmake_defines(root)
+    includes_defs = [includes_def]
+    text += package_text
+
+    root.flattened_deps = _get_flattened_deps(root)
     for dep in root.flattened_deps:
         includes_def, package_text = _get_dependency_cmake_defines(dep)
         includes_defs.append(includes_def)
         text += package_text
 
     # and finally, set the MAMA_INCLUDES and MAMA_LIBS
     includes = ' '.join(includes_defs)
@@ -224,28 +233,28 @@
         set(MAMA_ARCH_ARM64 TRUE)
         {get_build_dir_defines(c.build_dir_android64())}
     else()
         set(MAMA_ARCH_ARM32 TRUE)
         {get_build_dir_defines(c.build_dir_android32())}
     endif()
 elseif(WIN32)
-    if(MAMA_CMAKE_ARCH MATCHES "(amd64)|(AMD64)|(IA64)|(x86_64)|(X86_64)")
+    if(MAMA_CMAKE_ARCH MATCHES "(amd64)|(AMD64)|(IA64)|(x64)|(X64)|(x86_64)|(X86_64)")
         set(MAMA_ARCH_X64 TRUE)
         {get_build_dir_defines(c.build_dir_win64())}
     elseif(MAMA_CMAKE_ARCH MATCHES "(X86)|(x86)|(i386)|(i686)")
         set(MAMA_ARCH_X86 TRUE)
         {get_build_dir_defines(c.build_dir_win32())}
     elseif(MAMA_CMAKE_ARCH MATCHES "ARM64")
         set(MAMA_ARCH_ARM64 TRUE)
         {get_build_dir_defines(c.build_dir_winarm64())}
     elseif(MAMA_CMAKE_ARCH MATCHES "ARM")
         set(MAMA_ARCH_ARM32 TRUE)
         {get_build_dir_defines(c.build_dir_winarm32())}
     else()
-        message(FATAL_ERROR "MAMA: Unrecognized target architecture ${{MAMA_CMAKE_ARCH}}")
+        message(FATAL_ERROR "MAMA: Unrecognized target architecture '${{MAMA_CMAKE_ARCH}}'")
     endif()
 elseif(APPLE)
   if(IOS_PLATFORM)
         set(IOS TRUE)
         set(MAMA_ARCH_ARM64 TRUE) # Always arm64
         {get_build_dir_defines(c.build_dir_ios())}
   else()
@@ -253,36 +262,41 @@
     if(MAMA_CMAKE_ARCH MATCHES "x86_64") # (older x64)
         set(MAMA_ARCH_X64 TRUE)
         {get_build_dir_defines(c.build_dir_macos64())}
     elseif(MAMA_CMAKE_ARCH MATCHES "(arm64)|(ARM64)") # (M1 and later)
         set(MAMA_ARCH_ARM64 TRUE)
         {get_build_dir_defines(c.build_dir_macosarm64())}
     else()
-        message(FATAL_ERROR "MAMA: Unrecognized macOS architecture")
+        message(FATAL_ERROR "MAMA: Unrecognized macOS architecture '${{MAMA_CMAKE_ARCH}}'")
     endif()
   endif()
 elseif(RASPI)
         set(MAMA_ARCH_ARM32 TRUE)
         {get_build_dir_defines(c.build_dir_raspi32())}
 elseif(OCLEA)
         set(MAMA_ARCH_ARM64 TRUE)
+        add_compile_definitions(OCLEA=1)
         {get_build_dir_defines(c.build_dir_oclea64())}
+elseif(MIPS)
+        set(MAMA_ARCH_MIPS TRUE)
+        add_compile_definitions(MIPS=1)
+        {get_build_dir_defines(c.build_dir_mips())}
 elseif(UNIX)
     set(LINUX TRUE)
     if(MAMA_CMAKE_ARCH MATCHES "(amd64)|(AMD64)|(IA64)|(x86_64)")
         set(MAMA_ARCH_X64 TRUE)
         {get_build_dir_defines(c.build_dir_linux64())}
     elseif(MAMA_CMAKE_ARCH MATCHES "(X86)|(x86)|(i386)|(i686)")
         set(MAMA_ARCH_X86 TRUE)
         {get_build_dir_defines(c.build_dir_linux32())}
     else()
-        message(FATAL_ERROR "MAMA: Unrecognized Linux architecture")
+        message(FATAL_ERROR "MAMA: Unrecognized Linux architecture '${{MAMA_CMAKE_ARCH}}'")
     endif()
 else()
-    message(FATAL_ERROR "mama build: Unsupported Platform!")
+    message(FATAL_ERROR "mama build: Unsupported Platform! '${{MAMA_CMAKE_ARCH}}'")
 endif()
 
 # Overrides linkage on MSVC to non-debug run-time library (TODO: make this configurable)
 if(MSVC)
     add_definitions(-D_ITERATOR_DEBUG_LEVEL=0)
     foreach(MODE "_DEBUG" "_MINSIZEREL" "_RELEASE" "_RELWITHDEBINFO")
         string(REPLACE "/MDd" "/MD" TMP "${{CMAKE_C_FLAGS${{MODE}}}}")
@@ -317,57 +331,66 @@
                     changed |= load_dependency(child)
 
             dep.after_load()
             return changed
         load_dependency(root)
 
 
-def execute_task_chain(root: BuildDependency):
-    if root.already_executed:
-        return
-
-    if not os.path.exists(_mama_cmake_path(root)):
-        _save_mama_cmake_and_dependencies_cmake(root) # save a dummy mama.cmake before build
-
-    for dep in root.get_children():
-        execute_task_chain(dep)
-
-    if root.config.verbose:
-        console(f'  - Execute Tasks: {root.name}', color=Color.BLUE)
-
-    if root.already_executed:
-        error(f"Critical Error: '{root.name}' executed by child project")
-        raise RuntimeError(f"Cyclical Dependency detected for '{root.name}'")
-
-    _save_mama_cmake_and_dependencies_cmake(root)
-    root.target._execute_tasks()
-
-    # saves a helper autocomplete includes txt file to make adding .vscode include paths easier
-    _save_vscode_compile_commands(root)
-
-    if root.config.verbose and root.is_root_or_config_target():
-        names = [dep.name for dep in root.flattened_deps]
-        dep_names = " ".join(names) if root.flattened_deps else '<none>'
-        console(f'  - {root.name} Dependencies:  {dep_names}')
-        
-        all_deps = [root] + root.flattened_deps
-        libs = []
-        for dep in all_deps:
-            libs += [(dep.name, 'L', lib) for lib in dep.target.exported_libs]
-            libs += [(dep.name, 'S', lib) for lib in dep.target.exported_syslibs]
-
-        if libs:
-            console(f'  - {root.name} Exported Libs:')
-            for lib in libs:
-                console(f'    {lib[0]} [{lib[1]}] {lib[2]}')
-        else:
-            console(f'  - {root.name} Exported Libs: <none>')
+def print_dependencies(root: BuildDependency):
+    names = [dep.name for dep in root.flattened_deps]
+    dep_names = " ".join(names) if root.flattened_deps else '<none>'
+    console(f'  - {root.name} Dependencies:  {dep_names}')
+
+    all_deps = [root] + root.flattened_deps
+    libs = []
+    for dep in all_deps:
+        libs += [(dep.name, 'L', lib) for lib in dep.target.exported_libs]
+        libs += [(dep.name, 'S', lib) for lib in dep.target.exported_syslibs]
+
+    if libs:
+        console(f'  - {root.name} Exported Libs:')
+        for lib in libs:
+            console(f'    {lib[0]} [{lib[1]}] {lib[2]}')
+    else:
+        console(f'  - {root.name} Exported Libs: <none>')
+
+
+def execute_task_chain(flat_deps_reverse: List[BuildDependency]):
+    for dep in flat_deps_reverse:
+        if not os.path.exists(_mama_cmake_path(dep)):
+            _save_mama_cmake_and_dependencies_cmake(dep) # save a dummy mama.cmake before build
+
+        if dep.config.verbose:
+            console(f'  - Execute Tasks: {dep.name}', color=Color.BLUE)
+
+        # validate we're not building twice
+        if dep.already_executed:
+            error(f"Critical Error: '{dep.name}' executed by child project")
+            raise RuntimeError(f"Cyclical Dependency detected for '{dep.name}'")
+
+        # go through all child deps and make sure they executed
+        for c in dep.get_children():
+            if not c.already_executed:
+                error(f"Critical Error: child '{c.name}' has not been executed before executing target '{dep.name}'")
+                raise RuntimeError(f"Child target not executed before target which requires it: {c.name}")
+
+        _save_mama_cmake_and_dependencies_cmake(dep)
+        dep.target._execute_tasks()
+
+        # saves a helper autocomplete includes txt file to make adding .vscode include paths easier
+        _save_vscode_compile_commands(dep)
+
+        if dep.config.verbose and not dep.config.test:
+            if dep.is_root_or_config_target():
+                print_dependencies(dep)
+            # else:
+            #     print_dependencies(dep) # TODO: different output for non-root targets
 
 
-def find_dependency(root: BuildDependency, name) -> BuildDependency:
+def find_dependency(root: BuildDependency, name: str) -> BuildDependency:
     """ This is mainly used for finding root target or specific command line target """
-    if root.name == name:
+    if root.name.lower() == name.lower():
         return root
     for dep in root.get_children():
         found = find_dependency(dep, name)
         if found: return found
     return None
```

### Comparing `mama-0.7.9/mama/init_project.py` & `mama-0.8.0/mama/init_project.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/main.py` & `mama-0.8.0/mama/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from .types.local_source import LocalSource
 from .utils.system import Color, console
 from .utils.sub_process import execute
 from .util import glob_with_extensions, glob_folders_with_name_match
 from .build_config import BuildConfig
 from .build_target import BuildTarget
 from .build_dependency import BuildDependency
-from .dependency_chain import load_dependency_chain, execute_task_chain, find_dependency, get_full_flattened_deps
+from .dependency_chain import load_dependency_chain, execute_task_chain, find_dependency, get_flat_deps
 from .init_project import mama_init_project
 
 def print_title():
     console(f'========= Mama Build Tool ==========')
 
 def print_usage():
     console('mama [actions...] [args...]')
@@ -25,14 +25,16 @@
     console('    serve      - Equivalent of `update build deploy`')
     console('    clean      - clean main project or specific target')
     console('    rebuild    - clean, update and build main project or specific target')
     console('    reclone    - wipe specific target dependency and clone it again')
     console('    wipe       - alias of reclone')
     console('    upload     - uploads target package to artifactory server')
     console('    if_needed  - only uploads if package does not exist on server')
+    console('    art        - always fetch pkgs from artifactory, failure will throw an error')
+    console('    noart      - temporarily ignore artifactory pkgs fetch')
     console('    test       - run tests for main project or specific target')
     console('    start=arg  - start a specific tool via mamafile.start(args)')
     console('    add        - add new dependency')
     console('    new        - create new mama build file')
     console('    open=<tgt> - open a project file')
     console('    help       - shows this help list')
     console('  install utils:')
@@ -129,27 +131,38 @@
     if config.target and config.target != 'all':
         dep = find_dependency(root, config.target)
         if dep is None:
             console(f"ERROR: specified target='{config.target}' not found!")
             exit(-1)
 
 
+def print_package_exports(dep: BuildDependency):
+    target:BuildTarget = dep.target
+    if dep.from_artifactory or target.try_automatic_artifactory_fetch():
+        console(f'    Target {target.name} fetched from artifactory')
+    else:
+        target.package()
+    target.print_exports(abs_paths=True)
+
+
 def main():
     if sys.version_info < (3, 6):
         console('FATAL ERROR: MamaBuild requires Python 3.6')
         exit(-1)
 
     if len(sys.argv) == 1 or 'help' in sys.argv:
         print_title()
         print_usage()
         exit(-1)
 
     config = BuildConfig(sys.argv[1:])
     if config.print:
         print_title()
+        if config.verbose:
+            console(f'Build jobs={config.jobs}')
 
     source_dir = os.getcwd()
     name = os.path.basename(source_dir)
     local_src = LocalSource(name, source_dir, mamafile=None, always_build=False, args=[])
     workspace = None # figure out the workspace from the root mamafile.py
     root = BuildDependency(None, config, workspace, local_src)
 
@@ -192,34 +205,40 @@
         dep = find_dependency(root, config.target)
         if not dep:
             console(f'init command failed: target {config.target} not found')
             exit(-1)
         mama_init_project(dep)
         return
 
+    flat_deps = get_flat_deps(root)
+    flat_deps_reverse = list(reversed(flat_deps))
+
     if config.list:
-        console(f'    Dependency List: {get_full_flattened_deps(root)}')
-        if config.target:
+        flat_deps_names = [d.name for d in flat_deps]
+        if config.targets_all() or config.target == None:
+            console(f'    ALL Dependency List: {flat_deps_names}', Color.BLUE)
+            for dep in flat_deps:
+                print_package_exports(dep)
+        else:
             dep = find_dependency(root, config.target)
-            if dep:
-                target:BuildTarget = dep.target
-                if dep.from_artifactory or target.try_automatic_artifactory_fetch():
-                    console(f'    Target {target.name} fetched from artifactory')
-                else:
-                    target.package()
-                target.print_exports(abs_paths=True)
+            console(f'    {dep.name} Dependency List: {flat_deps_names}', Color.BLUE)
+            print_package_exports(dep)
         return
 
     if config.android: config.android_home()
     if config.raspi:   config.raspi_bin()
-    if config.oclea:   config.oclea.bin()
+    if config.oclea:   config.oclea.init_default()
+    if config.mips:    config.mips.init_default()
 
     if config.verbose:
-        console(f'Executing task chain for build:', Color.BLUE)
-    execute_task_chain(root)
+        chain = ' -> '.join([d.name for d in flat_deps_reverse])
+        console(f'Executing task chain for build:\n    {chain}', Color.BLUE)
+        print_package_exports(root)
+
+    execute_task_chain(flat_deps_reverse)
 
     if config.open:
         open_project(config, root)
 
 
 def __main__():
     main()
```

### Comparing `mama-0.7.9/mama/msbuild.py` & `mama-0.8.0/mama/msbuild.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/package.py` & `mama-0.8.0/mama/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+from __future__ import annotations
+from typing import TYPE_CHECKING
 import os
 from .utils.system import console
 from .util import normalized_path, glob_with_name_match
 from .types.asset import Asset
 
+if TYPE_CHECKING:
+    from .build_target import BuildTarget
 
 def is_a_static_library(lib):
     return lib.endswith('.a') or lib.endswith('.lib')
 
 
 def is_a_dynamic_library(lib):
     return lib.endswith('.dll')    or lib.endswith('.pdb') \
@@ -138,41 +142,58 @@
     if assets:
         for full_asset in assets:
             target.exported_assets.append(Asset(assets_path, full_asset, category))
         return True
     return False
 
 
-def find_syslib(target, name, apt, required):
+def find_syslib(target: BuildTarget, name, apt, required: bool):
     if target.ios or target.macos:
         if not name.startswith('-framework '):
             raise EnvironmentError(f'Expected "-framework name" but got "{name}"')
         return name # '-framework Foundation'
     elif target.linux:
         for candidate in [
             lambda: f'/usr/lib/x86_64-linux-gnu/{name}',
             lambda: f'/usr/lib/x86_64-linux-gnu/lib{name}.so',
             lambda: f'/usr/lib/x86_64-linux-gnu/lib{name}.a',
             lambda: f'/usr/lib/lib{name}.so',
             lambda: f'/usr/lib/lib{name}.a' ]:
             if os.path.isfile(candidate()):
                 return name # example: we found `libdl.so`, so just return `dl` for the linker
-        if not required: return False
+        if not required: return None
         if apt: raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try `sudo apt install {apt}`')
         raise IOError(f'Error {target.name} failed to find REQUIRED SysLib: {name}  Try installing it with apt.')
     else:
         return name # just export it. expect system linker to find it.
 
 
-def export_syslib(target, name, apt, required):
-    lib = find_syslib(target, name, apt, required)
-    #console(f'Exporting syslib: {name}:{lib}')
-    target.exported_syslibs.append(lib)
-    target.exported_syslibs = get_unique_basenames(target.exported_syslibs)
-    return True
+def export_syslib(target: BuildTarget, name, apt: bool, required: bool):
+    """
+    - target: The build target where to add the export syslib
+    - name: Name of the system library, eg: lzma
+    - apt: if true, then apt suggestion is given
+    - required: if true, then an exception is thrown if syslib is not found
+    """
+    try:
+        lib = find_syslib(target, name, apt, required)
+        if lib:
+            #console(f'Exporting syslib: {name}:{lib}')
+            target.exported_syslibs.append(lib)
+            target.exported_syslibs = get_unique_basenames(target.exported_syslibs)
+            return True
+    except IOError:
+        if target.config.clean:
+            # just export it. expect system linker to find it.
+            target.exported_syslibs.append(name)
+            target.exported_syslibs = get_unique_basenames(target.exported_syslibs)
+            return True
+        else:
+            raise
+    return False
 
 
 def get_lib_basename(syslib):
     if syslib.startswith('-framework '):
         return syslib
     return os.path.basename(syslib)
```

### Comparing `mama-0.7.9/mama/papa_deploy.py` & `mama-0.8.0/mama/papa_deploy.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
             append(relpath)
 
 
 def papa_deploy_to(target:BuildTarget, package_full_path:str,
                    r_includes:bool, r_dylibs:bool, 
                    r_syslibs:bool, r_assets:bool):
     config = target.config
-    detail_echo = config.print and config.target_matches(target.name) and (not config.test)
+    detail_echo = config.print and target.is_current_target() and (not config.test)
     if detail_echo: console(f'  - PAPA Deploy {package_full_path}')
 
     dependencies = _gather_dependencies(target)
 
     if not os.path.exists(package_full_path): # check to avoid Access Denied errors
         os.makedirs(package_full_path, exist_ok=True)
```

### Comparing `mama-0.7.9/mama/parse_mamafile.py` & `mama-0.8.0/mama/parse_mamafile.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/types/artifactory_pkg.py` & `mama-0.8.0/mama/types/artifactory_pkg.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/types/asset.py` & `mama-0.8.0/mama/types/asset.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/types/dep_source.py` & `mama-0.8.0/mama/types/dep_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/types/git.py` & `mama-0.8.0/mama/types/git.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 import os, shutil, stat, string
 from .dep_source import DepSource
 from ..utils.system import Color, System, console, error
-from ..utils.sub_process import execute, execute_piped
-from ..util import is_dir_empty, write_text_to, read_lines_from
+from ..utils.sub_process import SubProcess, execute, execute_piped
+from ..util import is_dir_empty, write_text_to, read_lines_from, path_join
 
 
 if TYPE_CHECKING:
     from ..build_target import BuildTarget
     from ..build_config import BuildConfig
     from ..build_dependency import BuildDependency
 
@@ -126,15 +126,15 @@
 
 
     def fetch_origin(self, dep: BuildDependency):
         self.run_git(dep, f"pull origin {self.branch_or_tag()} -q")
 
 
     def git_status_file(self, dep: BuildDependency):
-        return dep.target.build_dir('git_status')
+        return path_join(dep.build_dir, 'git_status')
 
 
     def save_status(self, dep: BuildDependency):
         commit = self.get_commit_hash(dep)
         status = f"{self.url}\n{self.tag}\n{self.branch}\n{commit}\n"
         if dep.config.verbose:
             console(f'    {self.name}  write git status commit={commit}')
@@ -191,30 +191,76 @@
             if self.tag and self.tag_changed:
                 self.run_git(dep, "reset --hard")
             self.run_git(dep, f"checkout {branch}")
 
 
     def reclone_wipe(self, dep: BuildDependency):
         if dep.config.print:
-            console(f'  - Target {dep.name: <16}   RECLONE WIPE')
+            console(f'  - Target {dep.name: <16} RECLONE WIPE')
         if os.path.exists(dep.dep_dir):
             if System.windows: # chmod everything to user so we can delete:
                 for root, dirs, files in os.walk(dep.dep_dir):
                     for d in dirs:  os.chmod(os.path.join(root, d), stat.S_IWUSR)
                     for f in files: os.chmod(os.path.join(root, f), stat.S_IWUSR)
             shutil.rmtree(dep.dep_dir)
 
 
+    def clone_with_filtered_progress(self, cmd, dep: BuildDependency):
+        output = ''
+        if dep.config.verbose:
+            console(cmd, color=Color.YELLOW)
+            result = execute(cmd, throw=False)
+        else:
+            current_percent = -1
+            def print_output(line:str):
+                nonlocal output, current_percent
+                if 'remote: Counting objects:' in line or \
+                    'remote: Compressing objects:' in line or \
+                    'Receiving objects:' in line or \
+                    'Resolving deltas:' in line or \
+                    'Updating files:' in line:
+                    if dep.config.print:
+                        parts = line.split('%')[0].split(':')
+                        percent = int(parts[len(parts)-1].strip())
+                        if current_percent != percent:
+                            current_percent = percent
+                            status = 'status             '
+                            if 'remote: Counting objects:' in line:      status = 'counting objects   '
+                            elif 'remote: Compressing objects:' in line: status = 'compressing objects'
+                            elif 'Receiving objects:' in line:           status = 'receiving objects  '
+                            elif 'Resolving deltas:' in line:            status = 'resolving deltas   '
+                            elif 'Updating files:' in line:              status = 'updating files     '
+                            print(f'\r  - Target {dep.name: <16} CLONE {status} {current_percent:3}%', end='')
+                elif 'Cloning into ' in line:
+                    pass
+                elif line:
+                    output += line
+                    output += '\n'
+            result = SubProcess.run(cmd, io_func=print_output)
+        # handle the result:
+        if dep.config.print:
+            if result == 0:
+                console(f'\r  - Target {dep.name: <16} CLONE SUCCESS                  ', color=Color.BLUE)
+                if dep.config.verbose and output:
+                    console(output, end='')
+            else:
+                console(f'\r  - Target {dep.name: <16} CLONE FAILED ({result})              ', color=Color.RED)
+                if output:
+                    console(output, end='')
+                raise RuntimeError(f'Target {self.name} clone failed: {cmd}')
+
+
     def clone_or_pull(self, dep: BuildDependency, wiped=False):
         if is_dir_empty(dep.src_dir):
             if not wiped and dep.config.print:
-                console(f"  - Target {dep.name: <16}   CLONE because src is missing", color=Color.BLUE)
+                console(f"  - Target {dep.name: <16} CLONE because src is missing", color=Color.BLUE)
             branch = self.branch_or_tag()
             if branch: branch = f" --branch {self.branch_or_tag()}"
-            execute(f"git clone --recurse-submodules --depth 1 {branch} {self.url} {dep.src_dir}", dep.config.verbose)
+            cmd = f"git clone --recurse-submodules --depth 1 {branch} {self.url} {dep.src_dir}"
+            self.clone_with_filtered_progress(cmd, dep)
             self.checkout_current_branch(dep)
         else:
             if dep.config.print:
                 console(f"  - Pulling {dep.name: <16}  SCM change detected", color=Color.BLUE)
             self.checkout_current_branch(dep)
             execute("git submodule update --init --recursive")
             if not self.tag: # pull if not a tag
@@ -227,19 +273,20 @@
         Do a git repository checkout. Can be an expensive operation.
         If an existing artifactory package exists, then this step is skipped
         """
         if not dep.source_dir_exists():  # we MUST pull here
             self.clone_or_pull(dep)
             return True
 
+        is_target = dep.is_current_target()
         config = dep.config
         changed = False
-        if config.update:
+
+        if config.update and is_target:
             changed = self.check_status(dep)
-        is_target = config.target_matches(self.name)
 
         wiped = False
         should_wipe = self.url_changed and not self.missing_status
         if should_wipe or (is_target and config.reclone):
             self.reclone_wipe(dep)
             wiped = True
         else:
```

### Comparing `mama-0.7.9/mama/types/local_source.py` & `mama-0.8.0/mama/types/local_source.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/util.py` & `mama-0.8.0/mama/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os, stat, shutil, zipfile
 from typing import List, Tuple
 import time, ssl, pathlib, random
 from .utils.system import System, console
 from .utils.sub_process import execute
 from urllib import request
-from datetime import datetime, timezone
+from datetime import datetime
+from dateutil import tz
 
 def is_file_modified(src, dst):
     return os.path.getmtime(src) == os.path.getmtime(dst) and\
            os.path.getsize(src) == os.path.getsize(dst)
 
 
 def find_executable_from_system(name):
@@ -48,52 +49,52 @@
         console(f'Deploying framework to {deployPath}')
         execute(f'rm -rf {deployPath}')
         shutil.copytree(framework, deployPath)
         return True
     return False
 
 
-def has_contents_changed(filename, new_contents):
+def has_contents_changed(filename: str, new_contents: str):
     if not os.path.exists(filename):
         return True
     return read_text_from(filename) != new_contents
 
 
-def save_file_if_contents_changed(filename, new_contents):
+def save_file_if_contents_changed(filename: str, new_contents: str):
     if not has_contents_changed(filename, new_contents):
         return
     write_text_to(filename, new_contents)
 
 
-def path_join(first, second):
+def path_join(first: str, second: str) -> str:
     """ Always join with forward/ slashes """
     first  = first.rstrip('/\\')
     second = second.lstrip('/\\')
     if not first: return second
     if not second: return first
     return first + '/' + second
 
 
-def forward_slashes(pathstring):
+def forward_slashes(pathstring: str) -> str:
     """ Replace all back\\ slashes with forward/ slashes"""
     return pathstring.replace('\\', '/')
 
 
-def back_slashes(pathstring):
+def back_slashes(pathstring: str) -> str:
     """ Replace all forward/ slashes with back\\ slashes"""
     return pathstring.replace('/', '\\')
 
 
-def normalized_path(pathstring):
+def normalized_path(pathstring: str) -> str:
     """ Normalizes a path to ABSOLUTE path and all forward/ slashes """
     pathstring = os.path.abspath(pathstring)
     return pathstring.replace('\\', '/').rstrip()
 
 
-def normalized_join(path1, *pathsN):
+def normalized_join(path1: str, *pathsN) -> str:
     """ Joins N paths and the calls normalized_path() """
     return normalized_path(os.path.join(path1, *pathsN))
 
 
 def glob_with_extensions(rootdir, extensions):
     results = []
     for dirpath, _, dirfiles in os.walk(rootdir):
@@ -154,26 +155,26 @@
     if old_tag != new_tag:
         console(f" tagchange '{old_tag.strip()}'\n"+
                 f"      ---> '{new_tag.strip()}'")
         return True
     return False
 
 
-def read_text_from(file_path):
+def read_text_from(file_path) -> str:
     return pathlib.Path(file_path).read_text()
 
 
 def write_text_to(file, text):
     dirname = os.path.dirname(file)
     if not os.path.exists(dirname):
         os.makedirs(dirname, exist_ok=True)
     pathlib.Path(file).write_text(text, encoding='utf-8')
 
 
-def read_lines_from(file):
+def read_lines_from(file) -> List[str]:
     if not os.path.exists(file):
         return []
     with pathlib.Path(file).open(encoding='utf-8') as f:
         return f.readlines()
 
 
 def get_file_size_str(size):
@@ -254,23 +255,24 @@
     Only extracts the files if their current size or modified time mismatches.
     Always sets modified time from the zipfile info.
     Preserves symlinks. And sets the correct file permission attributes.
     Returns # of files actually extracted.
     """
     def get_zipinfo_datetime(zipmember: zipfile.ZipInfo) -> datetime:
         zt = zipmember.date_time # tuple: year, month, day, hour, min, sec
-        return datetime(zt[0], zt[1], zt[2], zt[3], zt[4], zt[5], tzinfo=timezone.utc)
+        # ZIP uses localtime
+        return datetime(zt[0], zt[1], zt[2], zt[3], zt[4], zt[5], tzinfo=tz.tzlocal())
 
     def has_file_changed(zipmember: zipfile.ZipInfo, dst_path):
         st: os.stat_result = None
         try:
             st = os.stat(dst_path, follow_symlinks=False)
             if st.st_size != zipmember.file_size:
                 return True
-            dst_mtime: datetime = datetime.fromtimestamp(st.st_mtime, timezone.utc)
+            dst_mtime: datetime = datetime.fromtimestamp(st.st_mtime, tz=tz.tzlocal())
             src_mtime = get_zipinfo_datetime(zipmember)
             if dst_mtime != src_mtime:
                 return True
         except (OSError, ValueError):
             return True # does not exist
         return False
 
@@ -304,28 +306,33 @@
                         shutil.copyfileobj(src, dst)
         for zipmember, dst_path in unzipped_files:
             # set the correct permissions for files and folders
             perm = stat.S_IMODE(zipmember.external_attr >> 16)
             os.chmod(dst_path, perm)
             # always set the modification date from the zipmember timestamp,
             # this way we can avoid unnecessarily modifying files and causing full rebuilds
-            mtime = get_zipinfo_datetime(zipmember).timestamp()
-            os.utime(dst_path, times=(mtime, mtime), follow_symlinks=False)
+            time = get_zipinfo_datetime(zipmember)
+            #print(f'    | {dst_path} {time}')
+            mtime = time.timestamp()
+            if System.windows:
+                os.utime(dst_path, times=(mtime, mtime))
+            else:
+                os.utime(dst_path, times=(mtime, mtime), follow_symlinks=False)
 
     return len(unzipped_files)
 
 
-def try_unzip(local_file:str, build_dir:str) -> bool:
+def try_unzip(local_file:str, extract_dir:str) -> bool:
     """
     Attempts to unzip an archive, returns a tuple (success: bool, num_extracted: int)
     If (success: True, num_extracted: 0) is returned, it means none of the destination files
     were different from the zip contents, and zero extractions were performed
     """
     try:
-        files_extracted = unzip(local_file, build_dir)
+        files_extracted = unzip(local_file, extract_dir)
         return (True, files_extracted)
     except zipfile.BadZipFile as e:
         return (False, -1)
 
 
 def download_and_unzip(remote_file, extract_dir, local_file):
     if local_file and os.path.exists(local_file):
@@ -336,19 +343,25 @@
         return None
     unzip(local_file, extract_dir)
     console(f'Extracted {local_file} to {extract_dir}')
     return extract_dir
 
 
 def _should_copy(src, dst):
-    if not os.path.exists(dst):
-        return True
+    src_stat = None
+    try:
+        src_stat = os.stat(src)
+    except (OSError, ValueError):
+        return False # does not exist, nothing to copy
 
-    src_stat = os.stat(src)
-    dst_stat = os.stat(dst)
+    dst_stat = None
+    try:
+        dst_stat = os.stat(dst)
+    except (OSError, ValueError):
+        return True # dst doesn't exist, definitely need to copy it
 
     if src_stat.st_size != dst_stat.st_size:
         #console(f'_should_copy true src.size != dst.size\n┌──{src}\n└─>{dst}')
         return True
     if src_stat.st_mtime != dst_stat.st_mtime:
         #console(f'_should_copy true src.mtime != dst.mtime\n┌<──{src}\n└──> {dst}')
         return True
```

### Comparing `mama-0.7.9/mama/utils/nonblocking_io.py` & `mama-0.8.0/mama/utils/nonblocking_io.py`

 * *Files identical despite different names*

### Comparing `mama-0.7.9/mama/utils/system.py` & `mama-0.8.0/mama/utils/system.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,10 @@
 import sys, subprocess
 from termcolor import colored
 
-
-class Color:
-    DEFAULT = None
-    RED = "red"
-    GREEN = "green"
-    YELLOW = "yellow"
-    BLUE = "blue"
-
-
-def get_colored_text(s, color):
-    return colored(s, color=color) if color else s
-
-
-def console(s, color=None):
-    """ Always flush to support most build environments """
-    print(get_colored_text(s, color), flush=True)
-
-
-def error(s):
-    """ Prints a message as an error, usually colored red """
-    console(s, color=Color.RED)
-
-
 is_windows = sys.platform == 'win32'
 is_linux   = sys.platform.startswith('linux')
 is_macos   = sys.platform == 'darwin'
 if not (is_windows or is_linux or is_macos):
     raise RuntimeError(f'MamaBuild unsupported platform {sys.platform}')
 
 
@@ -45,7 +22,36 @@
 
 
 class System:
     windows = is_windows
     linux   = is_linux
     macos   = is_macos
     is_64bit = is_64
+
+
+class Color:
+    DEFAULT = None
+    RED = "red"
+    GREEN = "green"
+    YELLOW = "yellow"
+    BLUE = "blue"
+
+
+# on windows use colorama to enable ANSI color escape sequences
+if System.windows:
+    from colorama import just_fix_windows_console
+    just_fix_windows_console()
+
+
+def get_colored_text(text:str, color):
+    return colored(text, color=color) if color else text
+
+
+def console(text:str, color=None, end="\n"):
+    """ Always flush to support most build environments """
+    print(get_colored_text(text, color), end=end, flush=True)
+
+
+def error(text:str):
+    """ Prints a message as an error, usually colored red """
+    console(text, color=Color.RED)
+
```

### Comparing `mama-0.7.9/mama.egg-info/PKG-INFO` & `mama-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: mama
-Version: 0.7.9
-Summary: A modular C++ build tool even your mama can use
-Author-email: Jorma Rebane <jorma.rebane@gmail.com>
-License: MIT
-Project-URL: Homepage, https://github.com/RedFox20/Mama
-Project-URL: Bug Tracker, https://github.com/RedFox20/Mama/issues
-Keywords: mama,build,mamabuild,c,c++,tool,cmake,simple,easy,package,manager,cross-platform
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Mama Build Tool
 Mama - A modular C++ build tool even your mama can use
 
 The main goal of this project is to provide extremely convenient in-source builds
 for cross platform projects. Building is as simple as `mama build windows` - no ceremony~!
 
 CMake projects with trivial configurations and no dependencies can be handled
@@ -39,29 +19,30 @@
 private git repositories. Package versioning is done through git tags or branches.
 
 Custom build systems are also supported. For additional documentation explore: [build_target.py](mama/build_target.py)
 
 
 ## Who is this FOR?
 Anyone who develops cross-platform C++ libraries or applications which
-target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea].
+target any combination of [Windows, Linux, macOS, iOS, Android, Raspberry, Oclea, MIPS].
 And anyone who is not satisfied with system-wide dependencies and linker
 bugs caused by incompatible system-wide libraries on Linux.
 
 If you require an easy to use, reproducible project/namespace scoped package+build system, this is for you.
 Your builds will not rely on hard to setup system packages, all you need to do is type `mama build`.
 
 ### Supported platforms ###
-- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7)
-- Linux (Ubuntu) (64-bit x86_64, 32-bit x86)
-- MacOS (64-bit x86_64, 64-bit arm64)
-- iOS (64-bit arm64)
-- Android (64-bit arm64, 32-bit armv7)
-- Raspberry (32-bit armv7)
-- Oclea (64-bit arm64)
+- Windows (64-bit x86_64, 32-bit x86, 64-bit arm64, 32-bit armv7) default is latest MSVC
+- Linux (Ubuntu) (64-bit x86_64, 32-bit x86) both GCC and Clang
+- MacOS (64-bit x86_64, 64-bit arm64) via config.macos_version
+- iOS (64-bit arm64) via config.ios_version
+- Android (64-bit arm64, 32-bit armv7) via env ANDROID_HOME
+- Raspberry (32-bit armv7) via env RASPI_HOME
+- Oclea (64-bit arm64) via config.set_oclea_toolchain()
+- MIPS (mips mipsel, mips64, mips64el) via config.set_mips_toolchain()
 
 ## Who is this NOT for?
 Single platform projects with platform specific build configuration and system wide dependency management
 such as Linux exclusive G++ projects using apt-get libraries or iOS-only apps using cocoapods.
 
 
 ## Artifactory
@@ -254,15 +235,15 @@
 The package `setuptools>=65.0` is required, ensure the version is correct with `pip3 show setuptools`.
 
 You can set up local development with `$ pip3 install -e . --no-cache-dir` but make sure you have latest setuptools (>65.0) and latest pip3 (>22.3). This command will fail with older toolkits.
 
 Uploading a source distributionP:
 1. Get dependencies: `pip3 install build twine`
 2. Build sdist: `python -m build`
-3. Upload with twine: `twine upload dist/*`
+3. Upload with twine: `twine upload --skip-existing dist/*`
 It will prompt for Username and Password, unless you set up ~/.pypirc file:
 ```
 [distutils]
 index-servers = pypi
 [pypi]
 username=<your-mama-pypi-username>
 password=<your-mama-pypi-password>
```

### Comparing `mama-0.7.9/mama.egg-info/SOURCES.txt` & `mama-0.8.0/mama.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 mama.egg-info/PKG-INFO
 mama.egg-info/SOURCES.txt
 mama.egg-info/dependency_links.txt
 mama.egg-info/entry_points.txt
 mama.egg-info/requires.txt
 mama.egg-info/top_level.txt
 mama/platforms/__init__.py
+mama/platforms/mips.py
 mama/platforms/oclea.py
 mama/types/__init__.py
 mama/types/artifactory_pkg.py
 mama/types/asset.py
 mama/types/dep_source.py
 mama/types/git.py
 mama/types/local_source.py
```

### Comparing `mama-0.7.9/pyproject.toml` & `mama-0.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mama"
-version = "0.7.9"
+version = "0.8.0"
 description = "A modular C++ build tool even your mama can use"
 license = { text = "MIT" }
 authors = [
     { name="Jorma Rebane", email="jorma.rebane@gmail.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.6"
@@ -17,14 +17,17 @@
     'simple', 'easy', 'package', 'manager', 'cross-platform'
 ]
 dependencies = [
     "distro",
     "keyring",
     "keyrings.cryptfile",
     "termcolor",
+    "colorama",
+    "python-dateutil",
+    "psutil",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Build Tools",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
```

